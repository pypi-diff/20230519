# Comparing `tmp/twc_cli-2.0.0.tar.gz` & `tmp/twc_cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twc_cli-2.0.0.tar", max compression
+gzip compressed data, was "twc_cli-2.0.1.tar", max compression
```

## Comparing `twc_cli-2.0.0.tar` & `twc_cli-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    16236 2023-05-03 11:07:03.459112 twc_cli-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.0.0/COPYING
--rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.0.0/README.md
--rw-r--r--   0        0        0     1129 2023-05-03 11:07:09.215746 twc_cli-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.0.0/twc/__init__.py
--rw-r--r--   0        0        0     1828 2023-05-01 22:28:37.037517 twc_cli-2.0.0/twc/__main__.py
--rw-r--r--   0        0        0      442 2023-05-03 11:07:19.779020 twc_cli-2.0.0/twc/__version__.py
--rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.0.0/twc/api/__init__.py
--rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.0.0/twc/api/base.py
--rw-r--r--   0        0        0    31988 2023-05-02 19:49:18.973417 twc_cli-2.0.0/twc/api/client.py
--rw-r--r--   0        0        0     2260 2023-04-17 20:29:36.895547 twc_cli-2.0.0/twc/api/exceptions.py
--rw-r--r--   0        0        0     3202 2023-05-02 20:00:23.324980 twc_cli-2.0.0/twc/api/types.py
--rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.0.0/twc/apiwrap.py
--rw-r--r--   0        0        0      243 2023-05-01 13:40:32.452627 twc_cli-2.0.0/twc/commands/__init__.py
--rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.0.0/twc/commands/account.py
--rw-r--r--   0        0        0     7221 2023-05-02 19:57:14.010614 twc_cli-2.0.0/twc/commands/common.py
--rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.0.0/twc/commands/config.py
--rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.0.0/twc/commands/database.py
--rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.0.0/twc/commands/image.py
--rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.0.0/twc/commands/project.py
--rw-r--r--   0        0        0    66629 2023-05-02 20:25:09.354176 twc_cli-2.0.0/twc/commands/server.py
--rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.0.0/twc/commands/ssh_key.py
--rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.0.0/twc/commands/storage.py
--rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.0.0/twc/fmt.py
--rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.0.0/twc/typerx.py
--rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.0.0/twc/utils.py
--rw-r--r--   0        0        0      646 2023-04-30 21:08:17.345278 twc_cli-2.0.0/twc/vars.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    17215 2023-05-19 15:28:48.926753 twc_cli-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2023-02-27 16:18:31.000000 twc_cli-2.0.1/COPYING
+-rw-r--r--   0        0        0      843 2023-05-02 21:47:58.575180 twc_cli-2.0.1/README.md
+-rw-r--r--   0        0        0     1129 2023-05-19 15:30:05.479821 twc_cli-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-15 16:24:43.813223 twc_cli-2.0.1/twc/__init__.py
+-rw-r--r--   0        0        0     1828 2023-05-01 22:28:37.037517 twc_cli-2.0.1/twc/__main__.py
+-rw-r--r--   0        0        0      442 2023-05-19 15:29:59.126510 twc_cli-2.0.1/twc/__version__.py
+-rw-r--r--   0        0        0      128 2023-04-27 07:49:09.917167 twc_cli-2.0.1/twc/api/__init__.py
+-rw-r--r--   0        0        0     7781 2023-04-27 07:33:17.311019 twc_cli-2.0.1/twc/api/base.py
+-rw-r--r--   0        0        0    31988 2023-05-02 19:49:18.973417 twc_cli-2.0.1/twc/api/client.py
+-rw-r--r--   0        0        0     2279 2023-05-19 15:20:48.515105 twc_cli-2.0.1/twc/api/exceptions.py
+-rw-r--r--   0        0        0     3202 2023-05-02 20:00:23.324980 twc_cli-2.0.1/twc/api/types.py
+-rw-r--r--   0        0        0     2702 2023-04-27 08:25:15.189605 twc_cli-2.0.1/twc/apiwrap.py
+-rw-r--r--   0        0        0      243 2023-05-01 13:40:32.452627 twc_cli-2.0.1/twc/commands/__init__.py
+-rw-r--r--   0        0        0     5253 2023-05-01 16:59:46.116990 twc_cli-2.0.1/twc/commands/account.py
+-rw-r--r--   0        0        0     7221 2023-05-02 19:57:14.010614 twc_cli-2.0.1/twc/commands/common.py
+-rw-r--r--   0        0        0     8054 2023-05-01 17:04:38.382594 twc_cli-2.0.1/twc/commands/config.py
+-rw-r--r--   0        0        0    16052 2023-05-02 19:59:22.542511 twc_cli-2.0.1/twc/commands/database.py
+-rw-r--r--   0        0        0     8522 2023-05-02 19:59:29.622954 twc_cli-2.0.1/twc/commands/image.py
+-rw-r--r--   0        0        0    10798 2023-05-02 22:28:14.925192 twc_cli-2.0.1/twc/commands/project.py
+-rw-r--r--   0        0        0    66629 2023-05-02 20:25:09.354176 twc_cli-2.0.1/twc/commands/server.py
+-rw-r--r--   0        0        0     7941 2023-05-01 17:10:37.824666 twc_cli-2.0.1/twc/commands/ssh_key.py
+-rw-r--r--   0        0        0    19216 2023-05-01 17:12:04.101034 twc_cli-2.0.1/twc/commands/storage.py
+-rw-r--r--   0        0        0     6148 2023-04-17 22:18:55.659001 twc_cli-2.0.1/twc/fmt.py
+-rw-r--r--   0        0        0     6580 2023-05-01 20:29:58.139390 twc_cli-2.0.1/twc/typerx.py
+-rw-r--r--   0        0        0      651 2023-04-29 21:55:47.435595 twc_cli-2.0.1/twc/utils.py
+-rw-r--r--   0        0        0      646 2023-04-30 21:08:17.345278 twc_cli-2.0.1/twc/vars.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 twc_cli-2.0.1/PKG-INFO
```

### Comparing `twc_cli-2.0.0/CHANGELOG.md` & `twc_cli-2.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,22 @@
- # Версия 2.0.0 (2023.05.03)
+# Релизы Timeweb Cloud CLI
+
+В этом файле описаны все значимые изменения в Timeweb Cloud CLI. В выпусках мы придерживается правил [семантического версионирования](https://semver.org/lang/ru/).
+
+# Версия 2.0.1 (2023.05.19)
+
+## Добавлено
+
+- Теперь собираем программу также в формате zipapp (`.pyz`). Пакет zipapp это исполняемый ZIP-архив с приложением внутри. Он не требует установки, всё что нужно для запуска это интерпретатор Python 3.7 или выше, все зависимости уже добавлены в пакет.
+
+## Исправлено
+
+- Исправлена ошибка типов в модуле `twc.api.exceptions`, которая приводила к краху на Python ниже версии 3.10.
+
+# Версия 2.0.0 (2023.05.03)
 
 Это обновление значительно повышает качество кода, унифицирует интерфейсы и упрощает дальнейшую разработку. Проведён масштабный рефакторинг всей кодовой базы (~5,5 тыс строк кода на момент начала работы).
 
 Основные изменения в этом выпуске касаются парсера аргументов и API-клиента.
 
 > ❗**ВАЖНО**  
 > Версия 2.0.0 содержит обратно несовместимые изменения. Обязательно прочтите их список прежде чем обновляться.
```

### Comparing `twc_cli-2.0.0/COPYING` & `twc_cli-2.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/README.md` & `twc_cli-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/pyproject.toml` & `twc_cli-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twc-cli"
-version = "2.0.0"
+version = "2.0.1"
 description = "Timeweb Cloud Command Line Interface."
 authors = ["ge <dev@timeweb.cloud>"]
 homepage = "https://github.com/timeweb-cloud/twc"
 repository = "https://github.com/timeweb-cloud/twc"
 license="MIT"
 readme = "README.md"
 include = ["CHANGELOG.md", "COPYING"]
```

### Comparing `twc_cli-2.0.0/twc/__main__.py` & `twc_cli-2.0.1/twc/__main__.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/api/base.py` & `twc_cli-2.0.1/twc/api/base.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/api/client.py` & `twc_cli-2.0.1/twc/api/client.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/api/exceptions.py` & `twc_cli-2.0.1/twc/api/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """API client exceptions."""
 
-from typing import List
+from typing import List, Union
 from uuid import UUID
 
 from requests import HTTPError, PreparedRequest, Response
 
 
 class ErrResponse:
     """API error response schema."""
 
     def __init__(
         self,
         status_code: int = None,
         error_code: str = None,
-        message: str | List[str] = None,
+        message: Union[str, List[str]] = None,
         response_id: UUID = None,
     ):
         self.status_code = status_code
         self.error_code = error_code
         self.message = message
         self.response_id = response_id
 
@@ -27,15 +27,15 @@
 
     def __init__(
         self,
         request: PreparedRequest = None,
         response: Response = None,
         error_code: str = None,
         status_code: str = None,
-        message: str | List[str] = None,
+        message: Union[str, List[str]] = None,
         response_id: UUID = None,
     ):
         if message is not None:
             if isinstance(message, list):
                 description = "; ".join(message)
             else:
                 description = message
```

### Comparing `twc_cli-2.0.0/twc/api/types.py` & `twc_cli-2.0.1/twc/api/types.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/apiwrap.py` & `twc_cli-2.0.1/twc/apiwrap.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/account.py` & `twc_cli-2.0.1/twc/commands/account.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/common.py` & `twc_cli-2.0.1/twc/commands/common.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/config.py` & `twc_cli-2.0.1/twc/commands/config.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/database.py` & `twc_cli-2.0.1/twc/commands/database.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/image.py` & `twc_cli-2.0.1/twc/commands/image.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/project.py` & `twc_cli-2.0.1/twc/commands/project.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/server.py` & `twc_cli-2.0.1/twc/commands/server.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/ssh_key.py` & `twc_cli-2.0.1/twc/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/commands/storage.py` & `twc_cli-2.0.1/twc/commands/storage.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/fmt.py` & `twc_cli-2.0.1/twc/fmt.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/typerx.py` & `twc_cli-2.0.1/twc/typerx.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/utils.py` & `twc_cli-2.0.1/twc/utils.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/twc/vars.py` & `twc_cli-2.0.1/twc/vars.py`

 * *Files identical despite different names*

### Comparing `twc_cli-2.0.0/PKG-INFO` & `twc_cli-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twc-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Timeweb Cloud Command Line Interface.
 Home-page: https://github.com/timeweb-cloud/twc
 License: MIT
 Author: ge
 Author-email: dev@timeweb.cloud
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

