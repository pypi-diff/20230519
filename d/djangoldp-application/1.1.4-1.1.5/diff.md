# Comparing `tmp/djangoldp_application-1.1.4.tar.gz` & `tmp/djangoldp_application-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.1.4.tar", last modified: Fri May 19 15:45:48 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.1.5.tar", last modified: Fri May 19 16:06:00 2023, max compression
```

## Comparing `djangoldp_application-1.1.4.tar` & `djangoldp_application-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    17158 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 15:45:45.000000 djangoldp_application-1.1.4/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:45:48.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 15:45:30.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 15:45:29.000000 djangoldp_application-1.1.4/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    17445 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 16:05:58.000000 djangoldp_application-1.1.5/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:06:00.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 16:05:42.000000 djangoldp_application-1.1.5/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.1.4/README.md` & `djangoldp_application-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/setup.cfg` & `djangoldp_application-1.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.1.5/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/views.py` & `djangoldp_application-1.1.5/djangoldp_application/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,20 @@
         for applicationComponent in application["components"]:
             component = Component.objects.get(id=applicationComponent.obj.component_id)
             insertComponent = {
                 "type": component.name,
                 "route": format(component.preferred_route),
                 "parameters": {},
                 "extensions": [],
+                "experimental": [],
             }
             if component.auto_import:
-                insertComponent["experimental"] = ["routing"]
+                insertComponent["experimental"].append("routing")
+            if component.auto_menu:
+                insertComponent["experimental"].append("menu")
             keys = []
             for parameter in applicationComponent.obj.parameters.all():
                 if parameter.key == "route":
                     insertComponent["route"] = format(parameter.value)
                     keys.append(parameter.key)
                 elif parameter.key == "defaultRoute":
                     insertComponent["defaultRoute"] = format(parameter.value)
@@ -179,17 +182,20 @@
                         insertComponent["parameters"][parameter.key] = [insertComponent["parameters"][parameter.key], format(parameter.default)]
             for extensionComponent in applicationComponent.obj.extensions.all():
                 extension = Component.objects.get(id=extensionComponent.component_id)
                 componentExtension = {
                     "type": extension.name,
                     "route": format(component.preferred_route),
                     "parameters": {},
+                    "experimental": [],
                 }
-                if extension.auto_import:
-                    componentExtension["experimental"] = ["routing"]
+                if component.auto_import:
+                    insertComponent["experimental"].append("routing")
+                if component.auto_menu:
+                    insertComponent["experimental"].append("menu")
                 keys = []
                 for parameter in extensionComponent.parameters.all():
                     if parameter.key == "route":
                         componentExtension["route"] = format(parameter.value)
                         keys.append(parameter.key)
                     elif parameter.key == "defaultRoute":
                         componentExtension["defaultRoute"] = format(parameter.value)
```

### Comparing `djangoldp_application-1.1.4/djangoldp_application/models.py` & `djangoldp_application-1.1.5/djangoldp_application/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/admin.py` & `djangoldp_application-1.1.5/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-1.1.5/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.4/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.1.5/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

