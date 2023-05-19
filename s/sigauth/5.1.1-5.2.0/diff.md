# Comparing `tmp/sigauth-5.1.1-py3-none-any.whl.zip` & `tmp/sigauth-5.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6752 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-21 16:22 sigauth/__init__.py
--rw-r--r--  2.0 unx     5548 b- defN 21-Sep-21 16:22 sigauth/helpers.py
--rw-r--r--  2.0 unx      915 b- defN 21-Sep-21 16:22 sigauth/middleware.py
--rw-r--r--  2.0 unx      434 b- defN 21-Sep-21 16:22 sigauth/permissions.py
--rw-r--r--  2.0 unx     1091 b- defN 21-Sep-21 16:23 sigauth-5.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6512 b- defN 21-Sep-21 16:23 sigauth-5.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-21 16:23 sigauth-5.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 21-Sep-21 16:23 sigauth-5.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      688 b- defN 21-Sep-21 16:23 sigauth-5.1.1.dist-info/RECORD
-9 files, 15288 bytes uncompressed, 5568 bytes compressed:  63.6%
+Zip file size: 6757 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 14:49 sigauth/__init__.py
+-rw-r--r--  2.0 unx     5548 b- defN 23-May-19 14:49 sigauth/helpers.py
+-rw-r--r--  2.0 unx      915 b- defN 23-May-19 14:49 sigauth/middleware.py
+-rw-r--r--  2.0 unx      434 b- defN 23-May-19 14:49 sigauth/permissions.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6584 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 23-May-19 14:50 sigauth-5.2.0.dist-info/RECORD
+9 files, 15360 bytes uncompressed, 5573 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sigauth/middleware.py
 Comment: 
 
 Filename: sigauth/permissions.py
 Comment: 
 
-Filename: sigauth-5.1.1.dist-info/LICENSE
+Filename: sigauth-5.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: sigauth-5.1.1.dist-info/METADATA
+Filename: sigauth-5.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sigauth-5.1.1.dist-info/WHEEL
+Filename: sigauth-5.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sigauth-5.1.1.dist-info/top_level.txt
+Filename: sigauth-5.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sigauth-5.1.1.dist-info/RECORD
+Filename: sigauth-5.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sigauth-5.1.1.dist-info/LICENSE` & `sigauth-5.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sigauth-5.1.1.dist-info/METADATA` & `sigauth-5.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: sigauth
-Version: 5.1.1
+Version: 5.2.0
 Summary: Signature authentication library for Export Directory.
 Home-page: https://github.com/uktrade/directory-signature-auth
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Requires-Dist: django (<4.0.0,>=1.11.22)
+License-File: LICENSE
+Requires-Dist: django (<=4.2,>=3.2.19)
 Requires-Dist: djangorestframework (<4.0.0,>=3.4.7)
 Requires-Dist: mohawk (<2.0.0,>=0.3.4)
 Provides-Extra: test
-Requires-Dist: pytest (==6.1.0) ; extra == 'test'
-Requires-Dist: pytest-cov (==2.10.1) ; extra == 'test'
-Requires-Dist: pytest-django (==3.10.0) ; extra == 'test'
-Requires-Dist: flake8 (==3.8.3) ; extra == 'test'
-Requires-Dist: wheel (<1.0.0,>=0.31.0) ; extra == 'test'
-Requires-Dist: setuptools (<39.0.0,>=38.6.0) ; extra == 'test'
+Requires-Dist: pytest (==7.*) ; extra == 'test'
+Requires-Dist: pytest-cov (==4.*) ; extra == 'test'
+Requires-Dist: pytest-django (==4.*) ; extra == 'test'
+Requires-Dist: flake8 ; extra == 'test'
+Requires-Dist: wheel (<1.0.0,>=0.40.0) ; extra == 'test'
+Requires-Dist: setuptools ; extra == 'test'
 Requires-Dist: codecov ; extra == 'test'
 Requires-Dist: twine ; extra == 'test'
 
 # directory-signature-auth
 
 [![code-climate-image]][code-climate]
 [![circle-ci-image]][circle-ci]
```

## Comparing `sigauth-5.1.1.dist-info/RECORD` & `sigauth-5.2.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sigauth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sigauth/helpers.py,sha256=q8KBnAzIMFKcEWJhzOQeNXeUi0WBx--JwQKjB06AHlc,5548
 sigauth/middleware.py,sha256=FopB3wvZaGxR6kF8B7TKC_tY_35AG0asgmdGGft95LQ,915
 sigauth/permissions.py,sha256=lmPePeQxdkAQu16CnGSE8GEN6sobBZQgaiEM79d-CwU,434
-sigauth-5.1.1.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-sigauth-5.1.1.dist-info/METADATA,sha256=Yj-GivLucaYMHOdb3yqmXfUXnsQm9yAgBhS5Cfm6DH0,6512
-sigauth-5.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-sigauth-5.1.1.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
-sigauth-5.1.1.dist-info/RECORD,,
+sigauth-5.2.0.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+sigauth-5.2.0.dist-info/METADATA,sha256=tEWeFgzfdeManRRtkJmDYcUh7YnPTAmkmXhB7g4xCp0,6584
+sigauth-5.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sigauth-5.2.0.dist-info/top_level.txt,sha256=mGlNBeKJK-HbIfvTKK_jrdMOtW4K3QcZNoGYTRSzhUc,8
+sigauth-5.2.0.dist-info/RECORD,,
```

