# Comparing `tmp/bastion_api-0.2.3.tar.gz` & `tmp/bastion_api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastion_api-0.2.3.tar", max compression
+gzip compressed data, was "bastion_api-0.2.4.tar", max compression
```

## Comparing `bastion_api-0.2.3.tar` & `bastion_api-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.2.3/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.2.3/README.md
--rw-r--r--   0        0        0      311 2023-05-18 13:29:02.531724 bastion_api-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.2.3/src/bastion_api/__init__.py
--rw-r--r--   0        0        0    34110 2023-05-18 13:29:02.527724 bastion_api-0.2.3/src/bastion_api/bastion.py
--rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.2.3/src/bastion_api/dto/__init__.py
--rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      536 2023-05-17 12:02:03.938377 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0      899 2023-05-17 12:02:03.910378 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc
--rw-r--r--   0        0        0     1098 2023-05-17 12:02:03.910378 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc
--rw-r--r--   0        0        0     5532 2023-05-17 12:03:24.517481 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc
--rw-r--r--   0        0        0     1979 2023-05-17 12:02:03.914378 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc
--rw-r--r--   0        0        0     2270 2023-05-17 12:02:03.914378 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc
--rw-r--r--   0        0        0     4478 2023-05-17 12:02:03.922378 bastion_api-0.2.3/src/bastion_api/dto/__pycache__/support.cpython-310.pyc
--rw-r--r--   0        0        0      212 2023-05-18 13:24:55.942013 bastion_api-0.2.3/src/bastion_api/dto/config.py
--rw-r--r--   0        0        0      957 2023-05-16 14:23:37.380494 bastion_api-0.2.3/src/bastion_api/dto/device_dto.py
--rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.2.3/src/bastion_api/dto/old_dto.py
--rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.2.3/src/bastion_api/dto/organization_dto.py
--rw-r--r--   0        0        0     8715 2023-05-17 13:42:34.587039 bastion_api-0.2.3/src/bastion_api/dto/pass_dto.py
--rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.2.3/src/bastion_api/dto/person_dto.py
--rw-r--r--   0        0        0     2558 2023-05-16 14:17:31.752162 bastion_api-0.2.3/src/bastion_api/dto/points_dto.py
--rw-r--r--   0        0        0     4916 2023-05-17 12:18:28.396213 bastion_api-0.2.3/src/bastion_api/dto/support.py
--rw-r--r--   0        0        0      994 2023-05-17 12:18:28.360214 bastion_api-0.2.3/src/bastion_api/handlers.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.2.4/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.2.4/README.md
+-rw-r--r--   0        0        0      311 2023-05-18 13:42:15.012470 bastion_api-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.2.4/src/bastion_api/__init__.py
+-rw-r--r--   0        0        0    34206 2023-05-18 13:41:28.608882 bastion_api-0.2.4/src/bastion_api/bastion.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.2.4/src/bastion_api/dto/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      536 2023-05-17 12:02:03.938377 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0      899 2023-05-17 12:02:03.910378 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1098 2023-05-17 12:02:03.910378 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     5532 2023-05-17 12:03:24.517481 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1979 2023-05-17 12:02:03.914378 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     2270 2023-05-17 12:02:03.914378 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     4478 2023-05-17 12:02:03.922378 bastion_api-0.2.4/src/bastion_api/dto/__pycache__/support.cpython-310.pyc
+-rw-r--r--   0        0        0      212 2023-05-18 13:24:55.942013 bastion_api-0.2.4/src/bastion_api/dto/config.py
+-rw-r--r--   0        0        0      957 2023-05-16 14:23:37.380494 bastion_api-0.2.4/src/bastion_api/dto/device_dto.py
+-rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.2.4/src/bastion_api/dto/old_dto.py
+-rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.2.4/src/bastion_api/dto/organization_dto.py
+-rw-r--r--   0        0        0     8763 2023-05-18 13:41:28.612882 bastion_api-0.2.4/src/bastion_api/dto/pass_dto.py
+-rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.2.4/src/bastion_api/dto/person_dto.py
+-rw-r--r--   0        0        0     2558 2023-05-16 14:17:31.752162 bastion_api-0.2.4/src/bastion_api/dto/points_dto.py
+-rw-r--r--   0        0        0     4916 2023-05-17 12:18:28.396213 bastion_api-0.2.4/src/bastion_api/dto/support.py
+-rw-r--r--   0        0        0      994 2023-05-17 12:18:28.360214 bastion_api-0.2.4/src/bastion_api/handlers.py
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.2.4/PKG-INFO
```

### Comparing `bastion_api-0.2.3/src/bastion_api/bastion.py` & `bastion_api-0.2.4/src/bastion_api/bastion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from http.cookies import SimpleCookie
 from typing import Dict, List
 from datetime import datetime as dt, timedelta as td
 from pydantic import BaseModel
 from aiohttp import ClientResponse, ClientSession
 from loguru import logger
 
-from dto.device_dto import DeviceDto
-from dto.organization_dto import OrgDto, DepartDto
-from dto.pass_dto import CardEventDto, CardDto, AttendanceDto, PassDto, MatValuePassDto, CarPassDto
-from dto.person_dto import PersonDto
-from dto.points_dto import EntryPointDto, AccessLevelDto, ControlAreaDto, AccessPointDto
-from dto.support import DictValDto, PassBriefDto
-from handlers import BastionIntegrationError, _handle_response
-from dto.config import BastionConfig
+from bastion_api.dto.device_dto import DeviceDto
+from bastion_api.dto.organization_dto import OrgDto, DepartDto
+from bastion_api.dto.pass_dto import CardEventDto, CardDto, AttendanceDto, PassDto, MatValuePassDto, CarPassDto
+from bastion_api.dto.person_dto import PersonDto
+from bastion_api.dto.points_dto import EntryPointDto, AccessLevelDto, ControlAreaDto, AccessPointDto
+from bastion_api.dto.support import DictValDto, PassBriefDto
+from bastion_api.dto.config import BastionConfig
+from bastion_api.handlers import BastionIntegrationError, _handle_response
 
 
 class Bastion:
     session = ClientSession
     config: BaseModel
     bastion_servers: []
     _code_for_url: str = ""
```

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/config.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/__pycache__/support.cpython-310.pyc` & `bastion_api-0.2.4/src/bastion_api/dto/__pycache__/support.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/device_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/device_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/old_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/old_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/organization_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/organization_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/pass_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/pass_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from typing import List
 
 from pydantic import BaseModel
 
-from person_dto import PersonDto
-from points_dto import EntryPointDto, AccessLevelDto
-from support import TimeIntervalDto, PersonBriefDto, MatValueDto, CarDto, PassBriefDto
+from bastion_api.dto.person_dto import PersonDto
+from bastion_api.dto.points_dto import EntryPointDto, AccessLevelDto
+from bastion_api.dto.support import TimeIntervalDto, PersonBriefDto, MatValueDto, CarDto, PassBriefDto
 
 
 class PassDto:
     class NewPassPerson(BaseModel):
         """create_or_update_pass"""
         personData: PersonDto  # Набор персональных данных пропуска
         entryPoints: List[EntryPointDto] = ""  # Массив точек прохода
```

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/person_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/person_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/points_dto.py` & `bastion_api-0.2.4/src/bastion_api/dto/points_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/dto/support.py` & `bastion_api-0.2.4/src/bastion_api/dto/support.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/src/bastion_api/handlers.py` & `bastion_api-0.2.4/src/bastion_api/handlers.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.3/PKG-INFO` & `bastion_api-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastion-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Модуль интеграции с API Бастоин ИКС
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

