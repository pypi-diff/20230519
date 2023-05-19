# Comparing `tmp/arkprts-0.0.1.tar.gz` & `tmp/arkprts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.0.1.tar", last modified: Sun May  7 18:22:36 2023, max compression
+gzip compressed data, was "arkprts-0.1.0.tar", last modified: Fri May 19 19:22:47 2023, max compression
```

## Comparing `arkprts-0.0.1.tar` & `arkprts-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 18:22:36.947943 arkprts-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      940 2023-05-07 18:22:36.945944 arkprts-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      669 2023-05-07 15:53:48.000000 arkprts-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 18:22:36.845002 arkprts-0.0.1/arkprts/
--rw-rw-rw-   0        0        0       86 2023-05-07 16:47:49.000000 arkprts-0.0.1/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1720 2023-05-07 16:14:10.000000 arkprts-0.0.1/arkprts/__main__.py
--rw-rw-rw-   0        0        0    11405 2023-05-07 16:41:37.000000 arkprts-0.0.1/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.0.1/arkprts/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:22:36.924959 arkprts-0.0.1/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.0.1/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     7820 2023-05-07 15:50:15.000000 arkprts-0.0.1/arkprts/models/data.py
--rw-rw-rw-   0        0        0     5699 2023-05-07 15:59:50.000000 arkprts-0.0.1/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.0.1/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-07 18:22:36.909966 arkprts-0.0.1/arkprts.egg-info/
--rw-rw-rw-   0        0        0      940 2023-05-07 18:22:36.000000 arkprts-0.0.1/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-05-07 18:22:36.000000 arkprts-0.0.1/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 18:22:36.000000 arkprts-0.0.1/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-07 18:22:36.000000 arkprts-0.0.1/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 18:22:36.000000 arkprts-0.0.1/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2572 2023-05-07 16:08:30.000000 arkprts-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 18:22:36.947943 arkprts-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-04-30 23:29:47.000000 arkprts-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:22:36.932951 arkprts-0.0.1/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.0.1/tests/test_config.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.245955 arkprts-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-05-19 19:22:47.244954 arkprts-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.164483 arkprts-0.1.0/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.0/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.0/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.0/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.0/arkprts/errors.py
+-rw-rw-rw-   0        0        0     6033 2023-05-19 18:45:31.000000 arkprts-0.1.0/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.230962 arkprts-0.1.0/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.0/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     2724 2023-05-19 18:41:28.000000 arkprts-0.1.0/arkprts/models/base.py
+-rw-rw-rw-   0        0        0     8548 2023-05-19 19:13:33.000000 arkprts-0.1.0/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     6588 2023-05-19 18:47:58.000000 arkprts-0.1.0/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.0/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.218972 arkprts-0.1.0/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 19:22:47.000000 arkprts-0.1.0/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:22:47.246953 arkprts-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-05-19 19:21:52.000000 arkprts-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:22:47.241955 arkprts-0.1.0/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.0/tests/test_gamedata.py
```

### Comparing `arkprts-0.0.1/LICENSE` & `arkprts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.0.1/arkprts/__main__.py` & `arkprts-0.1.0/arkprts/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,27 +24,34 @@
     if args.nickname:
         users = await client.search_player(args.nickname, limit=10)
     else:
         users = await client.get_friends()
         print("Friends:", end="\n\n")
 
     for user in users:
+        if user.level < 5:
+            continue
+
         print(f"{user.nickname}#{user.nick_number} ({user.uid}) Lvl {user.level}")
-        print(f"Current stage: {user.main_stage_progress} | Characters: {user.char_cnt} | Secretery: {user.secretary}")
+        print(f"Resume: {user.resume}")
+        print(
+            f"Current stage: {user.main_stage_progress} | Characters: {user.char_cnt} | Furniture: {user.furn_cnt} | "
+            f"Secretary: {client.gamedata.get_operator(user.secretary).name}",
+        )
         print(f"Playing since: {user.register_ts.isoformat()}")
         print(f"Last Online: {user.last_online_time.isoformat()}")
 
         print("Support Operators: ", end="")
         for char in user.assist_char_list:
             if not char:
                 continue
-            print(f"{char.char_id} E{char.evolve_phase}L{char.level}", end="")
+            print(f"{char.static.name} E{char.evolve_phase}L{char.level}", end="")
             if char.skills:
                 print(f" S{char.skill_index+1}M{char.skills[char.skill_index].specialize_level}", end="")
 
-            print("   ", end="")
+            print("  ", end="")
 
         print("\n")
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `arkprts-0.0.1/arkprts/client.py` & `arkprts-0.1.0/arkprts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Arknights client."""
+from __future__ import annotations
+
+import asyncio
 import dataclasses
 import json
+import logging
 import typing
 import uuid
 
 import aiohttp
-import pydantic
 
 from . import errors, models
+from .gamedata import GameData
 
 __all__ = ("Client",)
 
+logger: logging.Logger = logging.getLogger("arkprts")
+
 HEADERS = {
     "Content-Type": "application/json",
     "X-Unity-Version": "2017.4.39f1",
     "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 11; KB2000 Build/RP1A.201005.001)",
     "Connection": "Keep-Alive",
 }
 
@@ -42,34 +48,42 @@
     network: typing.Mapping[str, str] = dataclasses.field(default_factory=dict)
 
 
 class Client:
     """Arknights client."""
 
     config: Config
-    proxy: typing.Optional[str] = None
+    pure: bool
+    gamedata: GameData
+    proxy: str | None = None
 
-    uid: typing.Optional[str]
-    secret: typing.Optional[str]
+    uid: str | None
+    secret: str | None
 
     _seqnum: int
 
-    def __init__(self, **config: object) -> None:
+    def __init__(self, *, pure: bool = False, **config: object) -> None:
+        """Initialize the client.
+
+        If `pure` is set to `True`, the client will not attempt to download game data.
+        """
         self.config = Config(**config)
 
         self.uid = None
         self.secret = None
         self._seqnum = 1
+        self.pure = pure
+        self.gamedata = GameData()
 
     async def _request(
         self,
         method: str,
         url: str,
         *,
-        headers: typing.Optional[typing.Mapping[str, str]] = None,
+        headers: typing.Mapping[str, str] | None = None,
         **kwargs: typing.Any,
     ) -> typing.Any:
         """Make an arbitrary request."""
         headers = {**HEADERS, **(headers or {})}
 
         async with aiohttp.ClientSession() as session:
             async with session.request(method, url, headers=headers, **kwargs) as resp:
@@ -87,59 +101,69 @@
                 return data
 
     async def request(self, endpoint: str, *, method: str = "POST", **kwargs: typing.Any) -> typing.Any:
         """Make a request towards the game server."""
         if self.uid is None or self.secret is None:
             raise errors.NotLoggedInError("Not logged in.")
 
+        logger.debug("Sending request #%d to %s.", self._seqnum, endpoint)
         headers = {
             "secret": self.secret,
             "seqnum": str(self._seqnum),
             "uid": self.uid,
         }
         self._seqnum += 1  # tfw no x++
 
         return await self._request(method, f"{GAME_SERVER}/{endpoint}", headers=headers, **kwargs)
 
     async def _load_network_config(self) -> None:
         """Get network config."""
+        logger.debug("Loading network config.")
         data = await self._request("GET", f"{CONF_SERVER}/config/prod/official/network_config")
         content = json.loads(data["content"])
         self.config.sign = data["sign"]
         self.config.network = content["configs"][content["funcVer"]]["network"]
         self.config.network_version = content["configVer"]
 
     async def _load_version_config(self) -> None:
         """Get version config."""
+        logger.debug("Loading version config.")
         # for CN it's "/config/prod/official/Android/version"
         data = await self._request("GET", f"{ASSET_SERVER}/assetbundle/official/Android/version")
         self.config.assets_version = data["resVersion"]
         self.config.client_version = data["clientVersion"]
 
-    async def _initialize_config(self) -> None:
-        """Initialize config."""
+    async def start(self) -> None:
+        """Initialize config and download gamedata."""
+        tasks: list[typing.Awaitable[None]] = []
         if not self.config.network_version:
-            await self._load_network_config()
+            tasks.append(self._load_network_config())
         if not self.config.assets_version:
-            await self._load_version_config()
+            tasks.append(self._load_version_config())
+        if not self.pure:
+            tasks.append(self.gamedata.download_gamedata())
+
+        await asyncio.gather(*tasks)
 
     async def _get_access_token(self, channel_uid: str, yostar_token: str) -> str:
         """Get an access token from a channel uid and yostar token."""
+        logger.debug("Getting access token.")
         body = {
             "platform": "android",
             "uid": channel_uid,
             "token": yostar_token,
             "deviceId": self.config.device_id,
         }
         data = await self._request("POST", f"{PASSPORT_SERVER}/user/login", json=body)
         # print(data["yostar_username"])
         return data["accessToken"]
 
     async def _get_u8_token(self, channel_uid: str, access_token: str) -> str:
         """Get an arknights uid and u8 token from a channel uid and access token."""
+        logger.debug("Getting u8 token.")
         body = {
             "appId": "1",
             "channelId": "3",
             "extension": json.dumps({"uid": channel_uid, "token": access_token}),
             "worldId": "3",
             "platform": 1,
             "subChannel": "3",
@@ -150,15 +174,16 @@
         }
         data = await self._request("POST", f"{AUTH_SERVER}/u8/user/v1/getToken", json=body)
         self.uid = data["uid"]
         return data["token"]
 
     async def _get_secret(self, u8_token: str) -> str:
         """Get a secret from a u8 uid and token."""
-        await self._initialize_config()
+        logger.debug("Getting secret.")
+        await self.start()
         body = {
             "assetsVersion": self.config.assets_version,
             "clientVersion": self.config.client_version,
             "deviceId": self.config.device_id,
             "deviceId2": "",
             "deviceId3": "",
             "networkVersion": self.config.network_version,
@@ -169,32 +194,35 @@
         self.secret = ""
         data = await self.request("account/login", json=body)
         self.secret = data["secret"]
         return self.secret
 
     async def _request_yostar_auth(self, email: str) -> None:
         """Request to log in with a yostar account."""
+        logger.debug("Requesting yostar auth.")
         body = {
             "platform": "android",
             "account": email,
             "authlang": "en",
         }
         await self._request("POST", f"{PASSPORT_SERVER}/account/yostar_auth_request", json=body)
 
-    async def _submit_yostar_auth(self, email: str, code: str) -> typing.Tuple[str, str]:
+    async def _submit_yostar_auth(self, email: str, code: str) -> tuple[str, str]:
         """Submit a yostar auth code and receieve a yostar uid and temporary token."""
+        logger.debug("Submitting yostar auth.")
         body = {
             "account": email,
             "code": code,
         }
         data = await self._request("POST", f"{PASSPORT_SERVER}/account/yostar_auth_submit", json=body)
         return data["yostar_uid"], data["yostar_token"]
 
-    async def _get_yostar_token(self, email: str, yostar_uid: str, token: str) -> typing.Tuple[str, str]:
+    async def _get_yostar_token(self, email: str, yostar_uid: str, token: str) -> tuple[str, str]:
         """Get a channel uid and yostar token from a yostar uid and temporary token."""
+        logger.debug("Getting yostar token.")
         body = {
             "yostar_token": token,
             "deviceId": self.config.device_id,
             "channelId": "googleplay",
             "yostar_uid": yostar_uid,
             "createNew": "0",
             "yostar_username": email,
@@ -203,16 +231,17 @@
         return data["uid"], data["token"]
 
     async def login_with_token(self, channel_uid: str, yostar_token: str) -> None:
         """Login with a yostar token."""
         access_token = await self._get_access_token(channel_uid, yostar_token)
         u8_token = await self._get_u8_token(channel_uid, access_token)
         await self._get_secret(u8_token)
+        logger.info("Logged in with %s.", channel_uid)
 
-    async def login_with_email(self, email: typing.Optional[str] = None) -> None:
+    async def login_with_email(self, email: str | None = None) -> None:
         """Login with a yostar account. Uses stdin."""
         if not email:
             email = input("Enter email: ")
 
         await self._request_yostar_auth(email)
         print(f"Code has been sent to {email}")  # noqa: T201
 
@@ -261,26 +290,26 @@
         return await self._get_social_sort_list(0, ["level"], {"nickName": nickname, "nickNumber": nicknumber})
 
     async def search_player(
         self,
         nickname: str,
         nicknumber: str = "",
         *,
-        limit: typing.Optional[int] = None,
+        limit: int | None = None,
     ) -> typing.Sequence[models.Player]:
         """Search for a player and return a model."""
         uid_data = await self.get_raw_nicknamed(nickname, nicknumber)
         uids = sorted(uid_data["result"], key=lambda x: x["level"], reverse=True)[:limit]
         data = await self.get_raw_friend_info([uid["uid"] for uid in uids])
-        return pydantic.parse_obj_as(typing.Sequence[models.Player], data["friends"])
+        return [models.Player(client=self, **i) for i in data["friends"]]
 
-    async def get_friends(self, *, limit: typing.Optional[int] = None) -> typing.Sequence[models.Player]:
+    async def get_friends(self, *, limit: int | None = None) -> typing.Sequence[models.Player]:
         """Get friends and return a model."""
         uid_data = await self.get_raw_friends()
         uids = sorted(uid_data["result"], key=lambda x: x["level"], reverse=True)[:limit]
         data = await self.get_raw_friend_info([uid["uid"] for uid in uids])
-        return pydantic.parse_obj_as(typing.Sequence[models.Player], data["friends"])
+        return [models.Player(client=self, **i) for i in data["friends"]]
 
     async def get_data(self) -> models.User:
         """Get user sync data and return a model. Use raw data for more info."""
         data = await self.get_raw_data()
-        return pydantic.parse_obj_as(models.User, data["user"])
+        return models.User(client=self, **data["user"])
```

### Comparing `arkprts-0.0.1/arkprts/errors.py` & `arkprts-0.1.0/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.0.1/pyproject.toml` & `arkprts-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
@@ -37,15 +37,15 @@
 # A: Shadowing built-in
 # ARG: Unused function argument (duck-typing)
 # EM: String literal in exception
 # ERA: Commented-out code
 # FBT: Boolean in positional function type (duck-typing)
 # SLF: Private member access
 # TCH: Not using TYPE_CHECKING (ugly)
-# UP: Update from 3.8 (we use it)
+# TD: TODO comment conventions
 # ANN10: Missing type annotation for self/cls (useless)
 # ANN401: Use of typing.Any (complicates)
 # B008: Do not perform function calls in argument defaults (pydantic)
 # B027: Empty method in ABC (optional rewrite)
 # B905: zip without strict= (ugly)
 # C408: Unnecessary dict call (ugly)
 # D105: Missing docstring in magic method (useless)
@@ -62,15 +62,15 @@
   "A",
   "ARG",
   "EM",
   "ERA",
   "FBT",
   "SLF",
   "TCH",
-  "UP",
+  "TD",
   "ANN10",
   "ANN401",
   "B008",
   "B027",
   "B905",
   "C408",
   "D105",
```

