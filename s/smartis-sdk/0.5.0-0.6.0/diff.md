# Comparing `tmp/smartis_sdk-0.5.0.tar.gz` & `tmp/smartis_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartis_sdk-0.5.0.tar", max compression
+gzip compressed data, was "smartis_sdk-0.6.0.tar", max compression
```

## Comparing `smartis_sdk-0.5.0.tar` & `smartis_sdk-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.5.0/README.md
--rw-r--r--   0        0        0     1199 2023-05-19 02:54:47.956990 smartis_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.5.0/src/smartis_sdk/__init__.py
--rw-r--r--   0        0        0     6652 2023-05-19 02:26:28.370014 smartis_sdk-0.5.0/src/smartis_sdk/client.py
--rw-r--r--   0        0        0     2283 2023-05-19 02:25:28.173470 smartis_sdk-0.5.0/src/smartis_sdk/common.py
--rw-r--r--   0        0        0     3646 2023-05-19 02:45:40.086379 smartis_sdk-0.5.0/src/smartis_sdk/entity.py
--rw-r--r--   0        0        0      279 2023-05-12 08:01:58.268061 smartis_sdk-0.5.0/src/smartis_sdk/errors.py
--rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.5.0/src/smartis_sdk/utils.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0      155 2023-05-19 19:34:42.248592 smartis_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0     1190 2023-05-19 21:50:05.665095 smartis_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.6.0/src/smartis_sdk/__init__.py
+-rw-r--r--   0        0        0     7263 2023-05-19 21:45:29.250625 smartis_sdk-0.6.0/src/smartis_sdk/client.py
+-rw-r--r--   0        0        0     2389 2023-05-19 19:39:36.114699 smartis_sdk-0.6.0/src/smartis_sdk/common.py
+-rw-r--r--   0        0        0     3899 2023-05-19 20:06:36.365105 smartis_sdk-0.6.0/src/smartis_sdk/entity.py
+-rw-r--r--   0        0        0      279 2023-05-12 08:01:58.268061 smartis_sdk-0.6.0/src/smartis_sdk/errors.py
+-rw-r--r--   0        0        0      804 2023-05-19 21:43:57.006908 smartis_sdk-0.6.0/src/smartis_sdk/utils.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 smartis_sdk-0.6.0/PKG-INFO
```

### Comparing `smartis_sdk-0.5.0/LICENSE` & `smartis_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.5.0/pyproject.toml` & `smartis_sdk-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "smartis_sdk"
-version = "0.5.0"
+version = "0.6.0"
 description = "SDK для Smartis API"
 license = "MIT"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-requests = "^2.30.0"
+requests = "^2"
 pydantic = ">=2.0a1"
-pandas = "^2.0.1"
+pandas = "^2"
 
 [tool.poetry.dev-dependencies]
 coverage = "^7"
 pytest = "^7"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `smartis_sdk-0.5.0/src/smartis_sdk/client.py` & `smartis_sdk-0.6.0/src/smartis_sdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import json
 import time
 from enum import Enum
 
 import requests
 from pydantic import ValidationError, BaseModel
 
-from .entity import Ads, Ad, Payload, CrmCustomFields, CustomField
+from .entity import Ads, Ad, Payload, CrmCustomFields, CrmCustomField, CrmCustomFieldGroups
 from .entity import Campaigns, Campaign
 from .entity import Channels, Placements
 from .entity import Keywords, Keyword
 from .common import Method
 from .errors import ApiLimitError
 import logging
 
+from .utils import clean_column_ids
+
 
 class ContentType(Enum):
     application = "application/json"
 
 
 def status_code_handler(response: requests.Response, retry: int) -> None:
     """Обработка статус кодов"""
@@ -101,40 +103,49 @@
         all_ads: list[Ad] = []
         items: Ads = self._get_entity(ads_ids, Method.get_ads, Ads)
         all_ads.extend(items.items)
         return all_ads
 
     def _get_entity(self, ids: list, method: Method, model: BaseModel) -> BaseModel:
         params = {"ids": ids}
-        if method == Method.get_crm_custom_fields:
+        if method in [Method.get_crm_custom_fields, Method.get_crm_custom_field_groups]:
             params["smartis_crm_token"] = self.crm_token
         params_json = json.dumps(params)
         response = self._prepare(method, parameters=params_json)
         if response.status_code != 200:
             raise ConnectionError(f"status code: {str(response.status_code)}")
-        print(response.json())
         try:
             return model.model_validate(response.json())
         except ValidationError as e:
             raise ValueError from e
 
     def get_keywords(self, keywords_ids: list) -> list[Keyword]:
         all_keywords: list[Keyword] = []
         items: Keywords = self._get_entity(keywords_ids, Method.get_keywords, Keywords)
         all_keywords.extend(items.items)
         return all_keywords
 
-    def get_crm_custom_field(self, fields_ids: list) -> list[CustomField]:
+    def get_crm_custom_fields(self, fields_ids: list) -> list[CrmCustomField]:
         if self.crm_token is None:
             raise ValueError("Not found crm token")
-        all_fields: list[CustomField] = []
+        fields_ids = clean_column_ids(fields_ids, "field_")
+        all_fields: list[CrmCustomField] = []
         items: CrmCustomFields = self._get_entity(fields_ids, Method.get_crm_custom_fields, CrmCustomFields)
         all_fields.extend(items.items)
         return all_fields
 
+    def get_crm_custom_field_groups(self, fields_ids: list) -> list[CrmCustomField]:
+        if self.crm_token is None:
+            raise ValueError("Not found crm token")
+        fields_ids = clean_column_ids(fields_ids, "field_cf_group_")
+        all_fields: list[CrmCustomField] = []
+        items: CrmCustomFields = self._get_entity(fields_ids, Method.get_crm_custom_field_groups, CrmCustomFieldGroups)
+        all_fields.extend(items.items)
+        return all_fields
+
     def get_report(self, payload: Payload, retry: int = TRY_REQUEST) -> requests.Response:
         """Выполнение запросов с обработкой ошибок"""
         payload_json = payload.to_json()
         try:
             time.sleep(self.REQUEST_PAUSE)
             answer = requests.post(f"{self.host}reports/getReport", headers=self.header, data=payload_json)
             status_code_handler(answer, self.TRY_REQUEST)
@@ -153,7 +164,9 @@
         else:
             return answer
 
     def retry_get_report(self, payload: Payload) -> requests.Response:
         logging.info("Количество ошибок больше заданного! Пауза 10 мин")
         time.sleep(self.FORCE_PAUSE)
         return self.get_report(payload)
+
+
```

### Comparing `smartis_sdk-0.5.0/src/smartis_sdk/common.py` & `smartis_sdk-0.6.0/src/smartis_sdk/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     get_attributions = MethodFields("reports/getModelAttributions", "modelAttributions", "id")
     get_channels = MethodFields("reports/getChannels", "", "")
     get_placements = MethodFields("reports/getPlacements", "", "")
     get_campaigns = MethodFields("reports/getCampaigns", "", "")
     get_ads = MethodFields("reports/getAds", "", "")
     get_keywords = MethodFields("reports/getKeywords", "", "")
     get_crm_custom_fields = MethodFields("crm/crmCustomField/get", "crmCustomFields", "")
+    get_crm_custom_field_groups = MethodFields("crm/crmCustomFieldGroup/get", "crmCustomFieldGroups", "")
 
 
 class GroupBy(Enum):
     ADS = "ad_id"
     DAY = "day"
     PLACEMENT = "placement_id"
     CAMPAIGN = "campaigns"
```

### Comparing `smartis_sdk-0.5.0/src/smartis_sdk/entity.py` & `smartis_sdk-0.6.0/src/smartis_sdk/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,31 +47,41 @@
     keyword: str
 
 
 class Keywords(BaseModel):
     items: list[Keyword]= Field(alias='keywords')
 
 
-class CustomField(BaseModel):
+class CrmCustomField(BaseModel):
     id: int
     crm_account_id: int
     element_type_id: int
     custom_field_title: str
     field_type_id: int
     is_multiple: int
     group_id: int
     description: str
     status: int
     is_filter: int
     filter_param_id: int
     default_visibility: int
 
+class CrmCustomFieldGroup(BaseModel):
+    id: int
+    title: str
+    crm_account_id: int
+    default_visibility: int
+    sort: int
+
 
 class CrmCustomFields(BaseModel):
-    items: list[CustomField] = Field(alias='crmCustomFields')
+    items: list[CrmCustomField] = Field(alias='crmCustomFields')
+
+class CrmCustomFieldGroups(BaseModel):
+    items: list[CrmCustomFieldGroup] = Field(alias='crmCustomFieldGroups')
 
 
 class Ad(BaseModel):
     id: int
     external_id: str
     placement_id: int
     campaign_id: int | None
```

### Comparing `smartis_sdk-0.5.0/PKG-INFO` & `smartis_sdk-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: smartis-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: SDK для Smartis API
 License: MIT
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pandas (>=2,<3)
 Requires-Dist: pydantic (>=2.0a1)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2,<3)
 Description-Content-Type: text/markdown
 
 # Smartis SDK (Unofficial)
 
+Обертка для API Smartis  https://my.smartis.bi/api/documentation
+Актуально для версии API = `1.13`
+
```

