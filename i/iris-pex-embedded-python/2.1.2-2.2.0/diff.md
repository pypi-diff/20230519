# Comparing `tmp/iris_pex_embedded_python-2.1.2.tar.gz` & `tmp/iris_pex_embedded_python-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.1.2.tar", last modified: Mon Apr 24 18:55:23 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.2.0.tar", last modified: Fri May 19 16:26:41 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.1.2.tar` & `iris_pex_embedded_python-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.773568 iris_pex_embedded_python-2.1.2/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.1.2/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-24 18:55:23.771821 iris_pex_embedded_python-2.1.2/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.2/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.2/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-24 18:55:23.773883 iris_pex_embedded_python-2.1.2/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-24 18:54:36.000000 iris_pex_embedded_python-2.1.2/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.692658 iris_pex_embedded_python-2.1.2/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.690857 iris_pex_embedded_python-2.1.2/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.707815 iris_pex_embedded_python-2.1.2/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.757154 iris_pex_embedded_python-2.1.2/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     7063 2023-04-21 08:18:02.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.768385 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112      824 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.421655 iris_pex_embedded_python-2.2.0/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.2.0/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    39287 2023-05-19 16:26:41.420477 iris_pex_embedded_python-2.2.0/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    38378 2023-05-19 16:25:15.000000 iris_pex_embedded_python-2.2.0/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.2.0/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-05-19 16:26:41.421955 iris_pex_embedded_python-2.2.0/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2074 2023-05-19 16:25:42.000000 iris_pex_embedded_python-2.2.0/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.385916 iris_pex_embedded_python-2.2.0/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.385399 iris_pex_embedded_python-2.2.0/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.392015 iris_pex_embedded_python-2.2.0/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.410348 iris_pex_embedded_python-2.2.0/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5354 2023-05-19 16:15:48.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112    10275 2023-05-17 11:46:10.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.418438 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    39287 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112      824 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       43 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.1.2/LICENSE` & `iris_pex_embedded_python-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/PKG-INFO` & `iris_pex_embedded_python-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: iris_pex_embedded_python
-Version: 2.1.2
-Summary: iris_pex_embedded_python
-Home-page: https://github.com/grongierisc/interoperability-embedded-python
-Author: grongier
-Author-email: guillaume.rongier@intersystems.com
-License: MIT
-Keywords: iris_pex_embedded_python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -64,14 +40,16 @@
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
+    - [7.12.4. migrate](#7124-migrate)
+      - [7.12.4.1 setting.py file](#71241-settingpy-file)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -716,23 +694,37 @@
             server.sendmail(sender, receivers, msg.as_string())
             print("Successfully sent email")
 
 ```
 If this operation is called using a MyRequest message, the my_message function will be called thanks to the dispatcher, otherwise the on_message function will be called.
 
 ## 7.9. The `director` class
-The Directorclass is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
+The Director class is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
 Instead these business services are created by a custom application by calling the Director.create_business_service() method.<br>
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+`start_production`: The start_production() method starts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to start.
+
+`stop_production`: The stop_production() method stops the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to stop.
+
+`restart_production`: The restart_production() method restarts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to restart.
+
+`list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
+
 **Returns**:
 an object that contains an instance of IRISBusinessService
 
 WIP example
 
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
@@ -840,14 +832,110 @@
 
 e.g :
 ```python
 from grongier.pex import Utils
 Utils.register_folder("/irisdev/app/src/python/demo/",1,"PEX")
 ```
 
+### 7.12.4. migrate
+
+Start an embedded python shell :
+
+```sh
+/usr/irissys/bin/irispython
+```
+
+Then use this static method to migrate the settings file to the iris framework.
+
+```python
+from grongier.pex import Utils
+Utils.migrate()
+```
+
+#### 7.12.4.1 setting.py file
+
+This file is used to store the settings of the interoperability components.
+
+It has two sections :
+* `CLASSES` : This section is used to store the classes of the interoperability components.
+* `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
+
+e.g :
+```python
+import bp
+from bo import *
+from bs import *
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': FileOperation,
+    'Python.FileOperationWithIrisAdapter': FileOperationWithIrisAdapter,
+}
+
+PRODUCTIONS = [
+    {
+        'dc.Python.Production': {
+        "@Name": "dc.Demo.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": {
+                    "@Target": "Host",
+                    "@Name": "%settings",
+                    "#text": "path=/tmp"
+                }
+            },
+            {
+                "@Name": "Python.RedditService",
+                "@Category": "",
+                "@ClassName": "Python.RedditService",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "limit=10\nother<10"
+                    }
+                ]
+            },
+            {
+                "@Name": "Python.FilterPostRoutingRule",
+                "@Category": "",
+                "@ClassName": "Python.FilterPostRoutingRule",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": ""
+            }
+        ]
+    }
+    }
+]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
@@ -858,8 +946,8 @@
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.1.2/README.md` & `iris_pex_embedded_python-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: iris_pex_embedded_python
+Version: 2.2.0
+Summary: iris_pex_embedded_python
+Home-page: https://github.com/grongierisc/interoperability-embedded-python
+Author: grongier
+Author-email: guillaume.rongier@intersystems.com
+License: MIT
+Keywords: iris_pex_embedded_python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -40,14 +64,16 @@
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
+    - [7.12.4. migrate](#7124-migrate)
+      - [7.12.4.1 setting.py file](#71241-settingpy-file)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -692,23 +718,37 @@
             server.sendmail(sender, receivers, msg.as_string())
             print("Successfully sent email")
 
 ```
 If this operation is called using a MyRequest message, the my_message function will be called thanks to the dispatcher, otherwise the on_message function will be called.
 
 ## 7.9. The `director` class
-The Directorclass is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
+The Director class is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
 Instead these business services are created by a custom application by calling the Director.create_business_service() method.<br>
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+`start_production`: The start_production() method starts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to start.
+
+`stop_production`: The stop_production() method stops the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to stop.
+
+`restart_production`: The restart_production() method restarts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to restart.
+
+`list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
+
 **Returns**:
 an object that contains an instance of IRISBusinessService
 
 WIP example
 
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
@@ -816,14 +856,110 @@
 
 e.g :
 ```python
 from grongier.pex import Utils
 Utils.register_folder("/irisdev/app/src/python/demo/",1,"PEX")
 ```
 
+### 7.12.4. migrate
+
+Start an embedded python shell :
+
+```sh
+/usr/irissys/bin/irispython
+```
+
+Then use this static method to migrate the settings file to the iris framework.
+
+```python
+from grongier.pex import Utils
+Utils.migrate()
+```
+
+#### 7.12.4.1 setting.py file
+
+This file is used to store the settings of the interoperability components.
+
+It has two sections :
+* `CLASSES` : This section is used to store the classes of the interoperability components.
+* `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
+
+e.g :
+```python
+import bp
+from bo import *
+from bs import *
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': FileOperation,
+    'Python.FileOperationWithIrisAdapter': FileOperationWithIrisAdapter,
+}
+
+PRODUCTIONS = [
+    {
+        'dc.Python.Production': {
+        "@Name": "dc.Demo.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": {
+                    "@Target": "Host",
+                    "@Name": "%settings",
+                    "#text": "path=/tmp"
+                }
+            },
+            {
+                "@Name": "Python.RedditService",
+                "@Category": "",
+                "@ClassName": "Python.RedditService",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "limit=10\nother<10"
+                    }
+                ]
+            },
+            {
+                "@Name": "Python.FilterPostRoutingRule",
+                "@Category": "",
+                "@ClassName": "Python.FilterPostRoutingRule",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": ""
+            }
+        ]
+    }
+    }
+]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
@@ -834,8 +970,8 @@
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.1.2/setup.py` & `iris_pex_embedded_python-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.1.2',
+        version='2.2.0',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
@@ -47,13 +47,15 @@
         ],
         package_dir={'': 'src'},
         packages=['grongier.pex','grongier.iris'],
         include_package_data=True,
         python_requires='>=3.6',
         install_requires=[
             "dacite>=1.6.0",
+            "xmltodict>=0.12.0",
+            "irissqlcli"
         ]
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.2/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.2.0/src/grongier/pex/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import ast
 import iris
+import inspect
+import xmltodict
 
 class _Utils():
     @staticmethod
     def raise_on_error(sc):
         """
         If the status code is an error, raise an exception
         
@@ -20,15 +22,15 @@
             # get the parent directory of the current module
             # and append 'iris/Grongier/PEX' to it
             path = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'iris/Grongier/PEX')
 
         _Utils.raise_on_error(iris.cls('%SYSTEM.OBJ').LoadDir(path,'cubk',"*.cls",1))
 
     @staticmethod
-    def register_component(module:str,classname:str,path:str,overwrite:int,iris_classname:str):
+    def register_component(module:str,classname:str,path:str,overwrite:int=1,iris_classname:str='Python'):
         """
         It registers a component in the Iris database.
         
         :param module: The name of the module that contains the class
         :type module: str
         :param classname: The name of the class you want to register
         :type classname: str
@@ -40,15 +42,15 @@
         :type iris_classname: str
         :return: The return value is a string.
         """
 
         return iris.cls('Grongier.PEX.Utils').dispatchRegisterComponent(module,classname,path,overwrite,iris_classname)
 
     @staticmethod
-    def register_folder(path:str,overwrite:int,iris_package_name:str):
+    def register_folder(path:str,overwrite:int=1,iris_package_name:str='Python'):
         """
         > This function takes a path to a folder, and registers all the Python files in that folder as IRIS
         classes
         
         :param path: the path to the folder containing the files you want to register
         :type path: str
         :param overwrite: 
@@ -60,15 +62,15 @@
         for filename in os.listdir(path):
             if filename.endswith(".py"): 
                 _Utils._register_file(filename, path, overwrite, iris_package_name)
             else:
                 continue
 
     @staticmethod
-    def register_file(file:str,overwrite:int,iris_package_name:str):
+    def register_file(file:str,overwrite:int=1,iris_package_name:str='Python'):
         """
         It takes a file name, a boolean to overwrite existing components, and the name of the Iris
         package that the file is in. It then opens the file, parses it, and looks for classes that extend
         BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
         with the module name, class name, path, overwrite boolean, and the full Iris package name
         
         :param file: the name of the file containing the component
@@ -78,15 +80,15 @@
         :param iris_package_name: the name of the iris package that you want to register the components to
         :type iris_package_name: str
         """
         head_tail = os.path.split(file)
         return _Utils._register_file(head_tail[1],head_tail[0],overwrite,iris_package_name)
 
     @staticmethod
-    def _register_file(filename:str,path:str,overwrite:int,iris_package_name:str):
+    def _register_file(filename:str,path:str,overwrite:int=1,iris_package_name:str='Python'):
         """
         It takes a file name, a path, a boolean to overwrite existing components, and the name of the Iris
         package that the file is in. It then opens the file, parses it, and looks for classes that extend
         BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
         with the module name, class name, path, overwrite boolean, and the full Iris package name
         
         :param filename: the name of the file containing the component
@@ -114,15 +116,15 @@
                 if  extend in ('BusinessOperation','BusinessProcess','BusinessService','DuplexService','DuplexProcess','DuplexOperation','InboundAdapter','OutboundAdapter'):
                     module = _Utils.filename_to_module(filename)
                     iris_class_name = f"{iris_package_name}.{module}.{klass.name}"
                     # strip "_" for iris class name
                     iris_class_name = iris_class_name.replace('_','')
                     _Utils.register_component(module, klass.name, path, overwrite, iris_class_name)
     @staticmethod
-    def register_package(package:str,path:str,overwrite:int,iris_package_name:str):
+    def register_package(package:str,path:str,overwrite:int=1,iris_package_name:str='Python'):
         """
         It takes a package name, a path to the package, a flag to overwrite existing files, and the name of
         the iris package to register the files to. It then loops through all the files in the package and
         registers them to the iris package
         
         :param package: the name of the package you want to register
         :type package: str
@@ -154,7 +156,86 @@
         packages = path.replace(os.sep, ('.'))
         if len(packages) >1:
             module = packages+'.'+mod
         else:
             module = mod
 
         return module
+
+    @staticmethod
+    def migrate():
+        """ 
+        Read the settings.py file and register all the components
+        settings.py file has two dictionaries:
+            * CLASSES
+                * key: the name of the class
+                * value: an instance of the class
+            * PRODUCTIONS
+                list of dictionaries:
+                * key: the name of the production
+                * value: a dictionary containing the settings for the production
+        """
+        # try to load the settings file
+        try:
+            from settings import CLASSES, PRODUCTIONS
+        except ImportError:
+            # return an error if the settings file is not found
+            # and explain how to create it
+            raise ImportError("settings.py file not found. Please create it in the same directory as the main.py file. See the documentation for more information.")
+        _Utils.set_classes_settings(CLASSES)
+        _Utils.set_productions_settings(PRODUCTIONS)
+
+
+    @staticmethod
+    def set_classes_settings(class_items):
+        """
+        It takes a dictionary of classes and returns a dictionary of settings for each class
+        
+        :param class_items: a dictionary of classes
+        :return: a dictionary of settings for each class
+        """
+        for key, value in class_items.items():
+            path = os.path.dirname(inspect.getfile(value))
+            _Utils.register_component(value.__module__,value.__name__,path,1,key)
+
+    @staticmethod
+    def set_productions_settings(production_list):
+        """
+        It takes a list of dictionaries and registers the productions
+        """
+        # for each production in the list
+        for production in production_list:
+            # get the production name (first key in the dictionary)
+            production_name = list(production.keys())[0]
+            # set the first key to 'production'
+            production['Production'] = production.pop(production_name)
+            # transform the json as an xml
+            xml = _Utils.dict_to_xml(production)
+            # register the production
+            _Utils.register_production(production_name,xml)
+    
+    @staticmethod
+    def dict_to_xml(json):
+        """
+        It takes a json and returns an xml
+        
+        :param json: a json
+        :return: an xml
+        """
+        return xmltodict.unparse(json)  
+    
+    @staticmethod
+    def register_production(production_name,xml):
+        """
+        It takes a production name and an xml and registers the production
+        
+        :param production_name: the name of the production
+        :type production_name: str
+        :param xml: the xml of the production
+        :type xml: str
+        """
+        # split the production name in the package name and the production name
+        # the production name is the last part of the string
+        package = '.'.join(production_name.split('.')[:-1])
+        production_name = production_name.split('.')[-1]
+        # register the production
+        _Utils.raise_on_error(iris.cls('Grongier.PEX.Utils').CreateProduction(package,production_name,xml))
```

### Comparing `iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.1.2
+Version: 2.2.0
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,14 +64,16 @@
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
+    - [7.12.4. migrate](#7124-migrate)
+      - [7.12.4.1 setting.py file](#71241-settingpy-file)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -716,23 +718,37 @@
             server.sendmail(sender, receivers, msg.as_string())
             print("Successfully sent email")
 
 ```
 If this operation is called using a MyRequest message, the my_message function will be called thanks to the dispatcher, otherwise the on_message function will be called.
 
 ## 7.9. The `director` class
-The Directorclass is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
+The Director class is used for nonpolling business services, that is, business services which are not automatically called by the production framework (through the inbound adapter) at the call interval.<br>
 Instead these business services are created by a custom application by calling the Director.create_business_service() method.<br>
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+`start_production`: The start_production() method starts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to start.
+
+`stop_production`: The stop_production() method stops the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to stop.
+
+`restart_production`: The restart_production() method restarts the production.<br>
+**Parameters**:
+- **production_name**: a string that specifies the name of the production to restart.
+
+`list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
+
 **Returns**:
 an object that contains an instance of IRISBusinessService
 
 WIP example
 
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
@@ -840,14 +856,110 @@
 
 e.g :
 ```python
 from grongier.pex import Utils
 Utils.register_folder("/irisdev/app/src/python/demo/",1,"PEX")
 ```
 
+### 7.12.4. migrate
+
+Start an embedded python shell :
+
+```sh
+/usr/irissys/bin/irispython
+```
+
+Then use this static method to migrate the settings file to the iris framework.
+
+```python
+from grongier.pex import Utils
+Utils.migrate()
+```
+
+#### 7.12.4.1 setting.py file
+
+This file is used to store the settings of the interoperability components.
+
+It has two sections :
+* `CLASSES` : This section is used to store the classes of the interoperability components.
+* `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
+
+e.g :
+```python
+import bp
+from bo import *
+from bs import *
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': FileOperation,
+    'Python.FileOperationWithIrisAdapter': FileOperationWithIrisAdapter,
+}
+
+PRODUCTIONS = [
+    {
+        'dc.Python.Production': {
+        "@Name": "dc.Demo.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": {
+                    "@Target": "Host",
+                    "@Name": "%settings",
+                    "#text": "path=/tmp"
+                }
+            },
+            {
+                "@Name": "Python.RedditService",
+                "@Category": "",
+                "@ClassName": "Python.RedditService",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "limit=10\nother<10"
+                    }
+                ]
+            },
+            {
+                "@Name": "Python.FilterPostRoutingRule",
+                "@Category": "",
+                "@ClassName": "Python.FilterPostRoutingRule",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "false",
+                "@Schedule": ""
+            }
+        ]
+    }
+    }
+]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
```

### Comparing `iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

