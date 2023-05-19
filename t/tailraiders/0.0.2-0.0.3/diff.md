# Comparing `tmp/tailraiders-0.0.2.tar.gz` & `tmp/tailraiders-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.2.tar", last modified: Tue May 16 22:44:44 2023, max compression
+gzip compressed data, was "tailraiders-0.0.3.tar", last modified: Fri May 19 18:33:11 2023, max compression
```

## Comparing `tailraiders-0.0.2.tar` & `tailraiders-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.413922 tailraiders-0.0.2/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      678 2023-05-16 22:44:44.412784 tailraiders-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-16 22:14:49.000000 tailraiders-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 22:44:44.414928 tailraiders-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-16 22:44:25.000000 tailraiders-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.377720 tailraiders-0.0.2/tailraiders/
--rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 tailraiders-0.0.2/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.400764 tailraiders-0.0.2/tailraiders/boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 tailraiders-0.0.2/tailraiders/boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.401769 tailraiders-0.0.2/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 tailraiders-0.0.2/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.406130 tailraiders-0.0.2/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0       46 2023-05-16 12:15:36.000000 tailraiders-0.0.2/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     2645 2023-05-16 22:35:53.000000 tailraiders-0.0.2/tailraiders/gajalaka/nan.py
--rw-rw-rw-   0        0        0     2337 2023-05-16 21:59:03.000000 tailraiders-0.0.2/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.408588 tailraiders-0.0.2/tailraiders/plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.2/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.409981 tailraiders-0.0.2/tailraiders/protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 tailraiders-0.0.2/tailraiders/protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.410485 tailraiders-0.0.2/tailraiders/trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.2/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.399413 tailraiders-0.0.2/tailraiders.egg-info/
--rw-rw-rw-   0        0        0      678 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-05-16 22:44:44.000000 tailraiders-0.0.2/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.429534 tailraiders-0.0.3/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      695 2023-05-19 18:33:11.429534 tailraiders-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-05-19 18:28:04.000000 tailraiders-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:33:11.430805 tailraiders-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-18 20:40:04.000000 tailraiders-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.366356 tailraiders-0.0.3/tailraiders/
+-rw-rw-rw-   0        0        0      841 2023-05-19 18:27:22.000000 tailraiders-0.0.3/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.404021 tailraiders-0.0.3/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0       44 2023-05-19 18:26:14.000000 tailraiders-0.0.3/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     1149 2023-05-17 11:17:42.000000 tailraiders-0.0.3/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.411009 tailraiders-0.0.3/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 tailraiders-0.0.3/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.422440 tailraiders-0.0.3/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      163 2023-05-19 18:25:51.000000 tailraiders-0.0.3/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     2644 2023-05-19 17:19:07.000000 tailraiders-0.0.3/tailraiders/gajalaka/nan.py
+-rw-rw-rw-   0        0        0     2337 2023-05-16 21:59:03.000000 tailraiders-0.0.3/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.424439 tailraiders-0.0.3/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.3/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.425439 tailraiders-0.0.3/tailraiders/protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 tailraiders-0.0.3/tailraiders/protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.426883 tailraiders-0.0.3/tailraiders/trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.3/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.399680 tailraiders-0.0.3/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-05-19 18:33:11.000000 tailraiders-0.0.3/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.2/LICENSE` & `tailraiders-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.2/PKG-INFO` & `tailraiders-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
-tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
+Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
-You can install the package by using the following code:
-'''
-pip install TailraiderAlliance
-'''
+You can install the package by using the following code:<br>
+**pip install tailraiders**
+
+## Extra information
+
```

### Comparing `tailraiders-0.0.2/setup.py` & `tailraiders-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.2',
+    version = '0.0.3',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

### Comparing `tailraiders-0.0.2/tailraiders/gajalaka/nan.py` & `tailraiders-0.0.3/tailraiders/gajalaka/nan.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         th : int (default = 20)
             The percentage threshold of when columns should be dropped
 
         Returns:
         ----------------
         None :
-            It makes it so that self.df is now edited to no longer have the dropped columns
+            It makes it so that self.df is now edited to no longer has the dropped columns
         """
 
         self.nan_df = self.check[self.check['perc nan'] > th]
         dropcols = list(self.nan_df.index)
         print(f'The columns {dropcols} are being dropped')
         self.df = self.df.drop(dropcols, axis = 1)
         self.__init__(self.df)
```

### Comparing `tailraiders-0.0.2/tailraiders/gajalaka/plots.py` & `tailraiders-0.0.3/tailraiders/gajalaka/plots.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.2/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.0.3/tailraiders.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
-tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
+Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
-You can install the package by using the following code:
-'''
-pip install TailraiderAlliance
-'''
+You can install the package by using the following code:<br>
+**pip install tailraiders**
+
+## Extra information
+
```

