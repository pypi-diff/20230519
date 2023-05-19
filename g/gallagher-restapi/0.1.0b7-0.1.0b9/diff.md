# Comparing `tmp/gallagher_restapi-0.1.0b7.tar.gz` & `tmp/gallagher_restapi-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallagher_restapi-0.1.0b7.tar", max compression
+gzip compressed data, was "gallagher_restapi-0.1.0b9.tar", max compression
```

## Comparing `gallagher_restapi-0.1.0b7.tar` & `gallagher_restapi-0.1.0b9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      478 2023-05-12 05:56:23.035117 gallagher_restapi-0.1.0b7/gallagher_restapi/__init__.py
--rw-r--r--   0        0        0     3712 2023-05-12 09:18:44.285290 gallagher_restapi-0.1.0b7/gallagher_restapi/__main__.py
--rw-r--r--   0        0        0     9338 2023-05-12 09:14:19.249566 gallagher_restapi-0.1.0b7/gallagher_restapi/client.py
--rw-r--r--   0        0        0      408 2023-05-12 05:56:23.035117 gallagher_restapi-0.1.0b7/gallagher_restapi/exceptions.py
--rw-r--r--   0        0        0    22102 2023-05-12 09:22:15.429173 gallagher_restapi-0.1.0b7/gallagher_restapi/models.py
--rw-r--r--   0        0        0      382 2023-05-12 09:25:17.268835 gallagher_restapi-0.1.0b7/pyproject.toml
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b7/PKG-INFO
+-rw-r--r--   0        0        0      426 2023-05-15 07:51:41.038951 gallagher_restapi-0.1.0b9/gallagher_restapi/__init__.py
+-rw-r--r--   0        0        0     5484 2023-05-19 12:56:33.404630 gallagher_restapi-0.1.0b9/gallagher_restapi/__main__.py
+-rw-r--r--   0        0        0     9603 2023-05-19 12:53:25.150656 gallagher_restapi-0.1.0b9/gallagher_restapi/client.py
+-rw-r--r--   0        0        0      408 2023-05-12 05:56:23.035117 gallagher_restapi-0.1.0b9/gallagher_restapi/exceptions.py
+-rw-r--r--   0        0        0    24272 2023-05-19 12:08:19.617152 gallagher_restapi-0.1.0b9/gallagher_restapi/models.py
+-rw-r--r--   0        0        0      431 2023-05-19 13:03:39.408893 gallagher_restapi-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b9/PKG-INFO
```

### Comparing `gallagher_restapi-0.1.0b7/gallagher_restapi/client.py` & `gallagher_restapi-0.1.0b9/gallagher_restapi/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     FTApiFeatures,
     FTCardholder,
     FTEvent,
     FTEventGroup,
     FTItem,
     FTItemReference,
     FTITemTypes,
+    FTPersonalDataFieldDefinition,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class BaseClient:
+class Client:
     """Gallagher REST api base client."""
 
     api_features: FTApiFeatures
     item_types: FTITemTypes
 
     def __init__(
         self,
@@ -50,14 +51,16 @@
         self.httpx_client.headers = httpx.Headers(
             {
                 "Authorization": f"GGL-API-KEY {api_key}",
                 "Content-Type": "application/json",
             }
         )
         self.httpx_client.timeout.read = 60
+        self.event_groups: dict[str, FTEventGroup] = {}
+        self.event_types: dict[str, FTItem] = {}
 
     async def _async_request(
         self,
         method: str,
         endpoint: str,
         *,
         data: dict[str, Any] | None = None,
@@ -89,15 +92,15 @@
         if response.status_code == httpx.codes.NOT_FOUND:
             raise RequestError(
                 "Requested item does not exist or "
                 "your operator does not have the privilege to view it"
             )
         if response.status_code == httpx.codes.BAD_REQUEST:
             raise RequestError(response.json()["message"])
-        if response.status_code == httpx.codes.CREATED:
+        if response.status_code in [httpx.codes.CREATED, httpx.codes.NO_CONTENT]:
             return True
         return response.json()
 
     async def authenticate(self) -> None:
         """Connect to Server to authenticate."""
         response = await self._async_request("GET", f"{self.server_url}/api/")
         self.api_features = FTApiFeatures(**response["features"])
@@ -127,45 +130,48 @@
         items: list[FTItem] = []
         if response := await self._async_request(
             "GET", self.api_features.href("items"), params=params
         ):
             items = [FTItem(**item) for item in response["results"]]
         return items
 
-
-class CardholderClient(BaseClient):
-    """REST api cardholder client for Gallagher Command Center."""
-
-    async def get_personal_data_field(self, name: str | None = None) -> list[FTItem]:
+    async def get_personal_data_field(
+        self, name: str | None = None, extra_fields: list[str] = []
+    ) -> list[FTItem]:
         """Return List of available personal data fields."""
         pdfs: list[FTItem] = []
         params = {}
         if name:
-            params = {"name": name}
+            params["name"] = name
+        if extra_fields:
+            params["fields"] = ",".join(extra_fields)
 
         if response := await self._async_request(
             "GET", self.api_features.href("personalDataFields"), params=params
         ):
-            pdfs = [FTItem(**pdf) for pdf in response]
+            pdfs = [
+                FTPersonalDataFieldDefinition.from_dict(pdf)
+                for pdf in response["results"]
+            ]
 
         return pdfs
 
     async def get_cardholder(
         self,
         *,
-        ftitem_id: int | None = None,
+        id: int | None = None,
         name: str | None = None,
         pdfs: dict[str, str] | None = None,
-        detailed: bool = False,
+        extra_fields: list[str] = [],
     ) -> list[FTCardholder]:
         """Return list of cardholders."""
         cardholders: list[FTCardholder] = []
-        if ftitem_id:
+        if id:
             response: dict[str, Any] = await self._async_request(
-                "GET", f"{self.api_features.href('cardholders')}/{ftitem_id}"
+                "GET", f"{self.api_features.href('cardholders')}/{id}"
             )
             if response:
                 return [FTCardholder.from_dict(response)]
 
         else:
             if name and not isinstance(name, str):
                 raise ValueError("name field must be a string value.")
@@ -182,56 +188,59 @@
                     # if pdf name is correct we expect the result to include one item only
                     if not (
                         pdf_field := await self.get_personal_data_field(name=pdf_name)
                     ):
                         raise GllApiError(f"pdf field: {pdf_name} not found")
                     params.update({f"pdf_{pdf_field[0].id}": value})
 
+            if extra_fields:
+                params["fields"] = ",".join(extra_fields)
+
             response = await self._async_request(
                 "GET", self.api_features.href("cardholders"), params=params
             )
             if response["results"]:
-                if detailed:
-                    for cardholder in response["results"]:
-                        cardholder_details = await self._async_request(
-                            "GET", cardholder["href"]
-                        )
-                        cardholders.append(FTCardholder.from_dict(cardholder_details))
-                else:
-                    cardholders = [
-                        FTCardholder.from_dict(cardholder)
-                        for cardholder in response["results"]
-                    ]
+                cardholders = [
+                    FTCardholder.from_dict(cardholder)
+                    for cardholder in response["results"]
+                ]
         return cardholders
 
-    async def create_cardholder(self, cardholder: FTCardholder) -> FTItemReference:
-        """Create a new cardholder in Gallagher."""
+    async def add_cardholder(self, cardholder: FTCardholder) -> FTItemReference:
+        """Add a new cardholder in Gallagher."""
         return await self._async_request(
             "POST", self.api_features.href("cardholders"), data=cardholder.as_dict
         )
 
+    async def update_cardholder(self, cardholder: FTCardholder) -> bool:
+        """Update existing cardholder in Gallagher."""
+        return await self._async_request(
+            "PATCH",
+            cardholder.href,
+            data=cardholder.as_dict,
+        )
 
-class EventClient(BaseClient):
-    """REST api event client for Gallagher Command Center."""
-
-    event_groups: dict[str, FTEventGroup]
-    event_types: dict[str, FTItem]
+    async def remove_cardholder(self, cardholder: FTCardholder) -> bool:
+        """Remove existing cardholder in Gallagher."""
+        return await self._async_request(
+            "DELETE",
+            cardholder.href,
+        )
 
     async def get_event_types(self) -> None:
         """Return list of event types."""
         response = await self._async_request(
             "GET", self.api_features.href("events/eventGroups")
         )
         self.event_groups = {
             FTEventGroup.from_dict(event_group).name: FTEventGroup.from_dict(
                 event_group
             )
             for event_group in response["eventGroups"]
         }
-        self.event_types = {}
         for event_group in self.event_groups.values():
             self.event_types.update(
                 {event_type.name: event_type for event_type in event_group.event_types}
             )
 
     async def get_events(
         self, event_filter: EventFilter | None = None
```

### Comparing `gallagher_restapi-0.1.0b7/gallagher_restapi/models.py` & `gallagher_restapi-0.1.0b9/gallagher_restapi/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 from enum import Enum
 from typing import Any
 
 import pytz
 
 
 class FTITemTypes(Enum):
-    """Enumrate FTItem types."""
+    """Enumerate FTItem types."""
+
+
+class PatchAction(str, Enum):
+    """Enumerate Patch actions."""
+
+    ADD: str = "add"
+    UPDATE: str = "update"
+    REMOVE: str = "remove"
 
 
 @dataclass
 class FTApiFeatures:
     """FTApiFeatures class."""
 
     accessGroups: dict[str, Any]
@@ -43,15 +51,15 @@
     roles: dict[str, Any]
     schedules: dict[str, Any]
     visits: dict[str, Any]
 
     def href(self, feature: str) -> str:
         """
         Return href link for feature.
-        For subfeteatures use format feature/subfeature
+        For sub_features use format main_feature/sub_feature
         """
         main_feature = sub_feature = ""
         try:
             if "/" in feature:
                 main_feature, sub_feature = feature.split("/")
             else:
                 main_feature = feature
@@ -65,23 +73,23 @@
         return attr[sub_feature or main_feature]["href"]
 
 
 @dataclass
 class FTItemReference:
     """FTItem reference class."""
 
-    href: str = ""
+    href: str
 
 
 @dataclass
 class FTStatus:
     """FTStatus class."""
 
     value: str
-    type: str
+    type: str = ""
 
 
 @dataclass
 class FTItemType:
     """FTItemType class."""
 
     id: str
@@ -91,43 +99,43 @@
 @dataclass
 class FTItem:
     """FTItem class."""
 
     id: str
     name: str = ""
     href: str = ""
-    type: dict = ""
+    type: dict = field(default_factory=dict)
 
 
 @dataclass
 class FTLinkItem:
     """FTLinkItem class."""
 
     name: str
     href: str = ""
 
 
 @dataclass
 class FTAccessGroupMembership:
     """FTAccessGroupMembership base class."""
 
+    href: str = ""
     status: FTStatus = field(init=False)
-    access_group: FTLinkItem = field(init=False)
+    accessGroup: FTLinkItem = field(init=False)
     active_from: datetime = field(init=False)
     active_until: datetime = field(init=False)
-    href: str = ""
 
     @property
-    def as_dict(self) -> dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Return json string for post and update."""
-        _dict: dict[str, Any] = {"accessgroup": {"href": self.href}}
-        if self.active_from:
-            _dict["from"] = f"{self.active_from.isoformat()}Z"
-        if self.active_until:
-            _dict["until"] = f"{self.active_until.isoformat()}Z"
+        _dict: dict[str, Any] = {"accessGroup": {"href": self.href}}
+        if active_from := getattr(self, "active_from", None):
+            _dict["from"] = f"{active_from.isoformat()}Z"
+        if active_until := getattr(self, "active_until", None):
+            _dict["until"] = f"{active_until.isoformat()}Z"
         return _dict
 
     @classmethod
     def assign_membership(
         cls,
         access_group: FTItem,
         active_from: datetime | None = None,
@@ -144,16 +152,16 @@
     @classmethod
     def from_dict(cls, kwargs: dict[str, Any]) -> FTAccessGroupMembership:
         """Return FTAccessGroupMembership object from dict."""
         _cls = FTAccessGroupMembership()
 
         if status := kwargs.get("status"):
             _cls.status = FTStatus(**status)
-        if access_group := kwargs.get("accessGroup"):
-            _cls.access_group = FTLinkItem(**access_group)
+        if accessGroup := kwargs.get("accessGroup"):
+            _cls.accessGroup = FTLinkItem(**accessGroup)
         if active_from := kwargs.get("from"):
             _cls.active_from = datetime.fromisoformat(active_from[:-1]).replace(
                 tzinfo=pytz.utc
             )
         if active_until := kwargs.get("until"):
             _cls.active_until = datetime.fromisoformat(active_until[:-1]).replace(
                 tzinfo=pytz.utc
@@ -162,99 +170,127 @@
 
 
 @dataclass
 class FTCardholderCard:
     """FTCardholder card base class."""
 
     type: FTLinkItem | FTItem
+    href: str = field(init=False)
     number: str = field(init=False)
-    card_serial_number: str = field(init=False)
-    issue_level: int = field(init=False)
+    cardSerialNumber: str = field(init=False)
+    issueLevel: int = field(init=False)
     status: FTStatus = field(init=False)
     active_from: datetime = field(init=False)
     active_until: datetime = field(init=False)
 
     @property
-    def as_dict(self) -> dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Return json string for post and update."""
         _dict: dict[str, Any] = {"type": {"href": self.type.href}}
-        if self.number:
-            _dict["number"] = self.number
-        if self.issue_level:
-            _dict["issueLevel"] = self.issue_level
-        if self.active_from:
-            _dict["from"] = f"{self.active_from.isoformat()}Z"
-        if self.active_until:
-            _dict["until"] = f"{self.active_until.isoformat()}Z"
+        _dict["href"] = self.href
+        if number := getattr(self, "number", None):
+            _dict["number"] = number
+        if issueLevel := getattr(self, "issueLevel", None):
+            _dict["issueLevel"] = issueLevel
+        if active_from := getattr(self, "active_from", None):
+            _dict["from"] = f"{active_from.isoformat()}Z"
+        if active_until := getattr(self, "active_until", None):
+            _dict["until"] = f"{active_until.isoformat()}Z"
+        if status := getattr(self, "status", None):
+            _dict["status"] = status
         return _dict
 
     @classmethod
     def create_card(
         cls,
         card_type: FTItem,
         number: str = "",
-        issue_level: int | None = None,
+        issueLevel: int | None = None,
         active_from: datetime | None = None,
         active_until: datetime | None = None,
     ) -> FTCardholderCard:
         """Create an FTCardholder card object."""
         _cls = FTCardholderCard(type=card_type)
         if number:
             _cls.number = number
-        if issue_level:
-            _cls.issue_level = issue_level
+        if issueLevel:
+            _cls.issueLevel = issueLevel
         if active_from:
             _cls.active_from = active_from
         if active_until:
             _cls.active_until = active_until
         return _cls
 
     @classmethod
     def from_dict(cls, kwargs: dict[str, Any]) -> FTCardholderCard:
         """Return FTCardholderCard object from dict."""
         _cls = FTCardholderCard(type=FTLinkItem(**kwargs["type"]))
+        _cls.href = kwargs["href"]
         if number := kwargs.get("number"):
             _cls.number = number
-        if issue_level := kwargs.get("issueLevel"):
-            _cls.issue_level = issue_level
+        _cls.issueLevel = kwargs.get("issueLevel")
+
         if status := kwargs.get("status"):
             _cls.status = FTStatus(**status)
         if active_from := kwargs.get("from"):
             _cls.active_from = datetime.fromisoformat(active_from[:-1]).replace(
                 tzinfo=pytz.utc
             )
         if active_until := kwargs.get("until"):
             _cls.active_until = datetime.fromisoformat(active_until[:-1]).replace(
                 tzinfo=pytz.utc
             )
         return _cls
 
 
-@dataclass
-class FTPersonalDataDefinition:
-    """FTPersonalDataDefinition class."""
+@dataclass(init=False)
+class FTPersonalDataFieldDefinition:
+    """FTPersonalDataFieldDefinition class."""
 
     id: str
     name: str
+    description: str
     type: str
+    division: FTItemReference | None = None
+    default: str = ""
     href: str = ""
+    required: bool = False
+    unique: bool = False
+    accessGroups: list[FTLinkItem] = field(default_factory=list)
+    regex: str = ""
+    regexDescription: str = ""
+    contentType: str = ""
+    isProfileImage: bool = False
+
+    @classmethod
+    def from_dict(cls, kwargs: dict[str, Any]) -> FTPersonalDataFieldDefinition:
+        """Return FTPersonalDataFieldDefinition object from dict."""
+        _cls = FTPersonalDataFieldDefinition()
+        for key, value in kwargs.items():
+            if not isinstance(value, dict | list):
+                setattr(_cls, key, value)
+            if key == "division":
+                _cls.division = FTItemReference(**value)
+            if key == "accessGroups":
+                _cls.accessGroups = [FTLinkItem(**group) for group in value]
+        return _cls
 
 
 @dataclass
 class FTCardholderPdfValue:
     """FTCardholderPdfValue class."""
 
     name: str
+    href: str = ""
     value: str | FTItemReference = field(init=False)
     notifications: bool = field(init=False)
-    definition: FTPersonalDataDefinition = field(init=False)
-    href: str = field(init=False)
+    definition: FTItem = field(init=False)
 
     @property
-    def as_dict(self) -> dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Return json string for post and update."""
         return {f"@{self.name}": {"notifications": self.notifications}}
 
     @classmethod
     def create_pdf(
         cls, pdf_definition: FTItem, value: str, enable_notification: bool = False
     ) -> FTCardholderPdfValue:
@@ -270,17 +306,19 @@
         for name, info in kwargs.items():
             _cls = FTCardholderPdfValue(name=name[1:])
             if value := info.get("value"):
                 _cls.value = (
                     FTItemReference(**value) if isinstance(value, dict) else value
                 )
             if definition := info.get("definition"):
-                _cls.definition = FTPersonalDataDefinition(**definition)
+                _cls.definition = FTPersonalDataFieldDefinition.from_dict(definition)
             if href := info.get("href"):
                 _cls.href = href
+            if "notifications" in info:
+                _cls.notifications = info["notifications"]
         return _cls
 
 
 @dataclass
 class FTCardholderField:
     """Class to represent FTCardholder field."""
 
@@ -297,14 +335,15 @@
     FTCardholderField(name="lastName"),
     FTCardholderField(name="shortName"),
     FTCardholderField(name="description"),
     FTCardholderField(name="authorised"),
     FTCardholderField(
         name="lastSuccessfulAccessTime",
         from_dict=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
+        to_dict=lambda val: f"{val.isoformat()}Z",
     ),
     FTCardholderField(
         name="lastSuccessfulAccessZone",
         from_dict=lambda val: FTLinkItem(**val),
     ),
     FTCardholderField(name="serverDisplayName"),
     FTCardholderField(name="division", from_dict=lambda val: FTItem(**val)),
@@ -372,78 +411,97 @@
 class FTCardholder:
     """FTCardholder details class."""
 
     href: str = field(init=False)
     id: str = field(init=False)
     division: FTItemReference | None = None
     name: str = field(init=False)
-    firstName: str = field(default="")
-    lastName: str = field(default="")
-    shortName: str = field(default="")
-    description: str = field(default="")
+    firstName: str = ""
+    lastName: str = ""
+    shortName: str = ""
+    description: str = ""
     authorised: bool = field(default=False)
     pdfs: dict[str, Any] = field(default_factory=dict)
     lastSuccessfulAccessTime: datetime = field(init=False)
     lastSuccessfulAccessZone: FTLinkItem = field(init=False)
     serverDisplayName: str = field(init=False)
     disableCipherPad: bool = field(default=False)
-    usercode: str = field(default="")
+    usercode: str = ""
     operatorLoginEnabled: bool = field(default=False)
-    operatorUsername: str = field(default="")
-    operatorPassword: str = field(default="")
+    operatorUsername: str = ""
+    operatorPassword: str = ""
     operatorPasswordExpired: bool = field(default=False)
     windowsLoginEnabled: bool = field(default=False)
-    windowsUsername: str = field(default="")
+    windowsUsername: str = ""
     personalDataDefinitions: dict[str, FTCardholderPdfValue] | None = field(
         default=None
     )
-    cards: list[FTCardholderCard] | None = None
-    accessGroups: list[FTAccessGroupMembership] | None = None
+    cards: list[FTCardholderCard] | dict[str, list[FTCardholderCard]] | None = None
+    accessGroups: list[FTAccessGroupMembership] | dict[
+        str, list[FTAccessGroupMembership]
+    ] | None = None
     # operator_groups: str
     # competencies: str
     # edit: str
     updateLocation: FTItemReference | None = None
-    notes: str = field(default="")
+    notes: str = ""
     # relationships: Any | None = None
     lockers: Any | None = None
     elevatorGroups: Any | None = None
     lastPrintedOrEncodedTime: datetime | None = None
     lastPrintedOrEncodedIssueLevel: int | None = None
     # redactions: Any | None = None
 
     @property
     def as_dict(self) -> dict[str, Any]:
         """Return serialized str."""
         _dict: dict[str, Any] = {}
         for cardholder_field in FTCARDHOLDER_FIELDS:
-            try:
-                if value := getattr(self, cardholder_field.name):
+            if value := getattr(self, cardholder_field.name, None):
+                if cardholder_field.name in [
+                    "cards",
+                    "accessGroups",
+                ] and isinstance(value, dict):
+                    _dict[cardholder_field.name] = {
+                        key: cardholder_field.to_dict(val) for key, val in value.items()
+                    }
+                else:
                     _dict[cardholder_field.name] = cardholder_field.to_dict(value)
-            except AttributeError:
-                continue
 
         if self.pdfs:
             _dict.update({f"@{name}": value for name, value in self.pdfs.items()})
         return json.loads(json.dumps(_dict, default=lambda o: o.__dict__))
 
     @classmethod
     def from_dict(cls, kwargs: dict[str, Any]) -> FTCardholder:
         """Return FTCardholder object from dict."""
-
         _cls = FTCardholder()
         for cardholder_field in FTCARDHOLDER_FIELDS:
             if value := kwargs.get(cardholder_field.name):
                 setattr(_cls, cardholder_field.name, cardholder_field.from_dict(value))
 
         for cardholder_pdf in list(kwargs.keys()):
             if cardholder_pdf.startswith("@"):
                 _cls.pdfs[cardholder_pdf[1:]] = kwargs[cardholder_pdf]
 
         return _cls
 
+    @classmethod
+    def patch(cls, cardholder: FTCardholder, **kwargs: Any) -> FTCardholder:
+        """Return FTCardholder object from dict."""
+        _cls = FTCardholder()
+        _cls.href = cardholder.href
+        for key, value in kwargs.items():
+            try:
+                setattr(_cls, key, value)
+            except AttributeError as err:
+                print(err)
+                continue
+        return _cls
+
 
 # Gallagher alarm and event models
 @dataclass
 class FTAlarm:
     """FTAlarm summary class"""
 
     state: str
```

