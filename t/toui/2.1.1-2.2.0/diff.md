# Comparing `tmp/toui-2.1.1.tar.gz` & `tmp/toui-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.1.1.tar", last modified: Wed May 17 05:52:11 2023, max compression
+gzip compressed data, was "toui-2.2.0.tar", last modified: Fri May 19 13:00:16 2023, max compression
```

## Comparing `toui-2.1.1.tar` & `toui-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:52:11.919386 toui-2.1.1/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.1.1/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-17 05:52:11.918382 toui-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 05:52:11.859383 toui-2.1.1/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.1.1/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.1.1/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.1.1/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:52:11.863383 toui-2.1.1/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.1.1/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-17 05:52:11.919386 toui-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1517 2023-05-15 13:28:32.000000 toui-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:52:11.906382 toui-2.1.1/toui/
--rw-rw-rw-   0        0        0      266 2023-05-17 05:51:03.000000 toui-2.1.1/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.1.1/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.1.1/toui/_helpers.py
--rw-rw-rw-   0        0        0     9902 2023-05-15 13:04:45.000000 toui-2.1.1/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.1.1/toui/_signals.py
--rw-rw-rw-   0        0        0    27251 2023-05-17 05:39:09.000000 toui-2.1.1/toui/apps.py
--rw-rw-rw-   0        0        0    20537 2023-05-15 13:04:45.000000 toui-2.1.1/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.1.1/toui/exceptions.py
--rw-rw-rw-   0        0        0    17082 2023-05-15 13:04:45.000000 toui-2.1.1/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.1.1/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:52:11.917382 toui-2.1.1/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-17 05:52:11.000000 toui-2.1.1/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-17 05:52:11.000000 toui-2.1.1/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:52:11.000000 toui-2.1.1/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-05-17 05:52:11.000000 toui-2.1.1/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-17 05:52:11.000000 toui-2.1.1/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.673609 toui-2.2.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2994 2023-05-19 13:00:16.672291 toui-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.487424 toui-2.2.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.2.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.2.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.494627 toui-2.2.0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.2.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-19 13:00:16.674605 toui-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-05-19 12:59:06.000000 toui-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.660330 toui-2.2.0/toui/
+-rw-rw-rw-   0        0        0      266 2023-05-19 12:56:31.000000 toui-2.2.0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.2.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.2.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10419 2023-05-19 12:50:07.000000 toui-2.2.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.2.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    27251 2023-05-17 05:39:09.000000 toui-2.2.0/toui/apps.py
+-rw-rw-rw-   0        0        0    21033 2023-05-19 12:54:37.000000 toui-2.2.0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.2.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    17082 2023-05-15 13:04:45.000000 toui-2.2.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.2.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.671280 toui-2.2.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     2994 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.1.1/LICENSE` & `toui-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/PKG-INFO` & `toui-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.1.1
+Version: 2.2.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.1.1/README.md` & `toui-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/advanced_example_1_toui_blueprint.py` & `toui-2.2.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/example_1_simple_website.py` & `toui-2.2.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/example_2_simple_desktop_app.py` & `toui-2.2.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/example_3_updating_page.py` & `toui-2.2.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/example_4_function_with_arg.py` & `toui-2.2.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/examples/example_5_user_variables.py` & `toui-2.2.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/images/logo.png` & `toui-2.2.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/setup.py` & `toui-2.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,23 +13,34 @@
 name = "ToUI"
 version = __version__
 author = "Mubarak Almehairbi"
 description = "Creates user interfaces (websites and desktop apps) from HTML easily"
 package_name = "toui"
 requirements = []
 optional_requirements = ['flask-login', 'flask-sqlalchemy', 'flask-basicauth']
-with open(f"requirements.txt", "rt") as file:
-    for pkg in file.read().splitlines():
-        pkg_name = pkg.split("==")[0]
-        if pkg_name.lower().replace("_","-") in optional_requirements and small:
-            continue
-        pkg_version = pkg.split("==")[1]
-        pkg_major_version = pkg_version.split(".")[0]
-        req = f"{pkg_name}>={pkg_version},<{int(pkg_major_version)+1}"
-        requirements.append(req)
+
+reqs_txt = \
+"""beautifulsoup4==4.12.2
+Flask==2.2.5
+Flask_BasicAuth==0.2.0
+Flask_Caching==2.0.2
+Flask_Login==0.6.2
+flask_sock==0.6.0
+flask_sqlalchemy==3.0.3
+pywebview==4.1
+tinycss==0.4"""
+
+for pkg in reqs_txt.splitlines():
+    pkg_name = pkg.split("==")[0]
+    if pkg_name.lower().replace("_","-") in optional_requirements and small:
+        continue
+    pkg_version = pkg.split("==")[1]
+    pkg_major_version = pkg_version.split(".")[0]
+    req = f"{pkg_name}>={pkg_version},<{int(pkg_major_version)+1}"
+    requirements.append(req)
 
 
 setuptools.setup(
     name=package_name,
     version=version,
     author=author,
     description=description,
```

### Comparing `toui-2.1.1/toui/_helpers.py` & `toui-2.2.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/toui/_javascript_templates.py` & `toui-2.2.0/toui/_javascript_templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,14 +82,27 @@
         input_element.setAttribute("value", input_element.value)
         if (input_element.checked == true) {
             input_element.setAttribute("checked", "")
         } else {
             input_element.removeAttribute("checked")
         }
     }
+
+    var select_elements = document.getElementsByTagName("select")
+    for (var select_element of select_elements) {
+        select_element.setAttribute("value", select_element.value)
+        for (var i = 0; i < select_element.options.length; i++) {
+            option = select_element.options[i]
+            if (i == select_element.selectedIndex) {
+                option.setAttribute("selected", "")
+            } else {
+                option.removeAttribute("selected")
+            }
+        }
+    }
     return properties
 }
 
 async function _getFiles(kwargs) {
     var files = []
     var element = _getElement(kwargs['selector'])
     if (element.type == "file") {
```

### Comparing `toui-2.1.1/toui/_signals.py` & `toui-2.2.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/toui/apps.py` & `toui-2.2.0/toui/apps.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/toui/elements.py` & `toui-2.2.0/toui/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,21 +365,40 @@
     def get_value(self):
         """
         Gets the ``value`` attribute of the HTML element.
 
         Returns
         -------
         str
-         If the attribute exists.
+            If the attribute exists.
 
         None
             If the attribute does not exist.
 
         """
         return self.get_attr("value")
+    
+    def get_selected(self) -> 'Element':
+        """
+        Gets the selected option of the HTML element ``<select>``.
+
+        This method is used for ``<select>`` elements only.
+
+        Returns
+        -------
+        Element
+            If it has a selected option.
+
+        None
+            If it does not have a selected option.
+
+        """
+        for element in self.get_elements():
+            if element.has_attr("selected"):
+                return element
 
     def set_value(self, value):
         """
         Sets the value of the ``value`` attribute.
 
         Parameters
         ----------
```

### Comparing `toui-2.1.1/toui/pages.py` & `toui-2.2.0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/toui/structure.py` & `toui-2.2.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.1.1/toui.egg-info/PKG-INFO` & `toui-2.2.0/toui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.1.1
+Version: 2.2.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.1.1/toui.egg-info/SOURCES.txt` & `toui-2.2.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

