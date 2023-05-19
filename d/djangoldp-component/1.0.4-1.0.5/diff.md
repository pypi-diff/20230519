# Comparing `tmp/djangoldp_component-1.0.4.tar.gz` & `tmp/djangoldp_component-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_component-1.0.4.tar", last modified: Tue Mar 28 15:10:36 2023, max compression
+gzip compressed data, was "dist/djangoldp_component-1.0.5.tar", last modified: Fri May 19 16:05:51 2023, max compression
```

## Comparing `djangoldp_component-1.0.4.tar` & `djangoldp_component-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      540 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      294 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)     9392 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-28 15:10:33.000000 djangoldp_component-1.0.4/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:10:35.000000 djangoldp_component-1.0.4/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-28 15:10:17.000000 djangoldp_component-1.0.4/djangoldp_component/migrations/0002_delete_dependency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-19 16:05:49.000000 djangoldp_component-1.0.5/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:05:51.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-19 16:05:33.000000 djangoldp_component-1.0.5/djangoldp_component/migrations/0002_delete_dependency.py
```

### Comparing `djangoldp_component-1.0.4/README.md` & `djangoldp_component-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.4/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-1.0.5/djangoldp_component.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 djangoldp_component.egg-info/PKG-INFO
 djangoldp_component.egg-info/SOURCES.txt
 djangoldp_component.egg-info/dependency_links.txt
 djangoldp_component.egg-info/requires.txt
 djangoldp_component.egg-info/top_level.txt
 djangoldp_component/migrations/0001_initial.py
 djangoldp_component/migrations/0002_delete_dependency.py
+djangoldp_component/migrations/0003_component_auto_menu.py
 djangoldp_component/migrations/__init__.py
```

### Comparing `djangoldp_component-1.0.4/setup.cfg` & `djangoldp_component-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.4/djangoldp_component/models.py` & `djangoldp_component-1.0.5/djangoldp_component/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     preferred_route = models.CharField(
         max_length=255, blank=True, null=True, default="false"
     )
     auto_import = models.BooleanField(
         default=False,
         help_text="Enable the experimental routing functionnality, does not require script declaration.",
     )
+    auto_menu = models.BooleanField(
+        default=False,
+        help_text="Enable the experimental menu functionnality, require a solid-***-menu component.",
+    )
     slug = models.SlugField(unique=True, blank=True, null=True)
 
     def __str__(self):
         try:
             return "{} ({})".format(self.friendly_name, self.urlid)
         except:
             return self.urlid
@@ -51,26 +55,28 @@
         owner_perms = ["inherit", "change", "delete"]
         rdf_context = {
             "friendly_name": "sib:friendlyName",
             "name": "sib:tag",
             "short_description": "sib:shortDescription",
             "preferred_route": "sib:route",
             "auto_import": "sib:componentAutoImport",
+            "auto_menu": "sib:componentAutoMenu",
             "creator": "foaf:user",
             "parameters": "ldp:Container",
             "script_tags": "ldp:Container",
         }
         rdf_type = "sib:component"
         serializer_fields = [
             "@id",
             "friendly_name",
             "name",
             "short_description",
             "preferred_route",
             "auto_import",
+            "auto_menu",
             "creator",
             "parameters",
             "script_tags",
         ]
         superuser_perms = ["view"]
         verbose_name = _("component")
         verbose_name_plural = _("components")
```

### Comparing `djangoldp_component-1.0.4/djangoldp_component/admin.py` & `djangoldp_component-1.0.5/djangoldp_component/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.4/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-1.0.5/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

