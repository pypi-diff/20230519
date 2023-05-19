# Comparing `tmp/djangoldp_application-1.1.2.tar.gz` & `tmp/djangoldp_application-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.1.2.tar", last modified: Fri May 19 14:58:01 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.1.3.tar", last modified: Fri May 19 15:15:49 2023, max compression
```

## Comparing `djangoldp_application-1.1.2.tar` & `djangoldp_application-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    15193 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5406 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 14:57:58.000000 djangoldp_application-1.1.2/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    15193 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 15:15:47.000000 djangoldp_application-1.1.3/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 15:15:49.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 15:15:31.000000 djangoldp_application-1.1.3/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.1.2/README.md` & `djangoldp_application-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/setup.cfg` & `djangoldp_application-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.1.3/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/views.py` & `djangoldp_application-1.1.3/djangoldp_application/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/models.py` & `djangoldp_application-1.1.3/djangoldp_application/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/admin.py` & `djangoldp_application-1.1.3/djangoldp_application/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 class ApplicationPackageParameterInline(admin.TabularInline):
     model = ApplicationPackageParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
 class ApplicationPackageAdmin(DjangoLDPAdmin):
-    list_display = ("urlid",)
+    list_display = ("urlid", "application", "package")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ApplicationPackageParameterInline]
     search_fields = [
         "urlid",
         "package__friendly_name",
         "package__short_description",
         "application__friendly_name",
@@ -105,15 +105,15 @@
 class ApplicationComponentParameterInline(admin.TabularInline):
     model = ApplicationComponentParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
 class ApplicationComponentAdmin(DjangoLDPAdmin):
-    list_display = ("urlid",)
+    list_display = ("urlid", "application", "component")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ApplicationComponentParameterInline]
     search_fields = [
         "urlid",
         "component__friendly_name",
         "component__short_description",
         "application__friendly_name",
@@ -125,15 +125,15 @@
 class ComponentExtensionParameterInline(admin.TabularInline):
     model = ComponentExtensionParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
 class ComponentExtensionAdmin(DjangoLDPAdmin):
-    list_display = ("urlid",)
+    list_display = ("urlid", "base_component", "component")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ComponentExtensionParameterInline]
     search_fields = [
         "urlid",
         "component__friendly_name",
         "component__short_description",
         "base_component__component__friendly_name",
```

### Comparing `djangoldp_application-1.1.2/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-1.1.3/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.2/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.1.3/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

