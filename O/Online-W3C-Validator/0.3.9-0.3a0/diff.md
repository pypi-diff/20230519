# Comparing `tmp/Online-W3C-Validator-0.3.9.tar.gz` & `tmp/Online-W3C-Validator-0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Online-W3C-Validator-0.3.9.tar", last modified: Tue May 29 06:09:21 2018, max compression
+gzip compressed data, was "dist/Online-W3C-Validator-0.3a0.tar", last modified: Thu Jan 11 00:55:12 2018, max compression
```

## Comparing `Online-W3C-Validator-0.3.9.tar` & `Online-W3C-Validator-0.3a0.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)     4580 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/PKG-INFO
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)      378 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/ChangeLog
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       14 2018-05-29 06:02:01.000000 Online-W3C-Validator-0.3.9/requirements.txt
-drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       14 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/top_level.txt
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)     4580 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/PKG-INFO
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)        1 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/dependency_links.txt
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)        1 2018-05-29 06:07:15.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/not-zip-safe
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       64 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/entry_points.txt
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)      473 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/SOURCES.txt
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       13 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/requires.txt
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       47 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/pbr.json
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)      110 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/AUTHORS
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)      953 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/setup.cfg
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)     3117 2018-05-29 05:26:42.000000 Online-W3C-Validator-0.3.9/README.rst
-drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-05-29 06:09:21.000000 Online-W3C-Validator-0.3.9/w3c_validator/
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)     3871 2018-05-29 05:15:30.000000 Online-W3C-Validator-0.3.9/w3c_validator/validator.py
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)      273 2018-05-29 05:18:10.000000 Online-W3C-Validator-0.3.9/w3c_validator/__init__.py
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)     1073 2018-01-09 06:49:48.000000 Online-W3C-Validator-0.3.9/LICENSE
--rw-r--r--   0 rcir178   (1000) rcir178   (1000)       81 2018-05-29 05:14:44.000000 Online-W3C-Validator-0.3.9/setup.py
+drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)     4337 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/PKG-INFO
+drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)       14 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/top_level.txt
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)     4337 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/PKG-INFO
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)        1 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/dependency_links.txt
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)       64 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/entry_points.txt
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)      347 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/SOURCES.txt
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)        9 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/requires.txt
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)       79 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/setup.cfg
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)     2971 2018-01-10 04:00:39.000000 Online-W3C-Validator-0.3a0/README.md
+drwxr-xr-x   0 rcir178   (1000) rcir178   (1000)        0 2018-01-11 00:55:12.000000 Online-W3C-Validator-0.3a0/w3c_validator/
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)     3831 2018-01-10 01:59:29.000000 Online-W3C-Validator-0.3a0/w3c_validator/validator.py
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)       92 2018-01-11 00:54:57.000000 Online-W3C-Validator-0.3a0/w3c_validator/__init__.py
+-rw-r--r--   0 rcir178   (1000) rcir178   (1000)     1358 2018-01-10 02:22:25.000000 Online-W3C-Validator-0.3a0/setup.py
```

### Comparing `Online-W3C-Validator-0.3.9/PKG-INFO` & `Online-W3C-Validator-0.3a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: Online-W3C-Validator
-Version: 0.3.9
+Version: 0.3a0
 Summary: UNKNOWN
 Home-page: https://github.com/nad2000/W3C-Validator
 Author: Radomirs Cirskis
 Author-email: nad2000@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nad2000/W3C-Validator
-Description: Online W3C Validator
-        ====================
+Description-Content-Type: UNKNOWN
+Description: # Online W3C Validator
         
-        Pure Python command line for HTML validation using W3C online validator.
-        It could be very handy for using it in a CI pipline.
+        Pure Python command line for HTML validation using W3C online validator. It could be very handy for using it in a CI pipline.
         
-        Installation
-        ------------
+        ## Installation
         
-        .. code:: bash
+        ```bash
+        pip install -U Online-W3C-Validator
+        ```
         
-           pip install -U Online-W3C-Validator
-        
-        How to use
-        ----------
+        ## How to use
         
         You can user the CLI command:
         
-        .. code:: bash
-        
-           w3c_validator http://www.google.com some_file.html
+        ```bash
+        w3c_validator http://www.google.com some_file.html
+        ```
         
         Example output:
         
-        ::
-        
-           INFO:w3c_validator.validator:Files to validate:
-             http://www.google.com
-           INFO:w3c_validator.validator:Number of files: 1
-           INFO:w3c_validator.validator:validating: http://www.google.com ...
-           error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-           error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-           error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           error: line 5: Attribute “width” not allowed on element “div” at this point.
-           error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           error: line 5: The “center” element is obsolete. Use CSS instead.
-           error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-        
-        Or you can use the fuction **validdate** provied by the package, that
-        thakes either HTML file name or URL as a single parameter an returns
-        JSON object with the validation output.
-        
-        .. code:: py
-        
-           from w3c_validator import validate
-        
-           messages = validate("http://www.google.com")["messages"]
-           for m in messages:
-               print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+        ```
+        INFO:w3c_validator.validator:Files to validate: 
+          http://www.google.com
+        INFO:w3c_validator.validator:Number of files: 1
+        INFO:w3c_validator.validator:validating: http://www.google.com ...
+        error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+        error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+        error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        error: line 5: Attribute “width” not allowed on element “div” at this point.
+        error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        error: line 5: The “center” element is obsolete. Use CSS instead.
+        error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+        ```
+        
+        Or you can use the fuction **validdate** provied by the package, that thakes either HTML file name or URL as a single parameter an returns JSON object with the validation output.
+        
+        ```py
+        from w3c_validator import validate
+        
+        messages = validate("http://www.google.com")["messages"]
+        for m in messages:
+            print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+        ```
         
         Example output:
         
-        ::
+        ```
+        Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+        Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
+        Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
+        ...
+        ```
+        
+        ## Contact
+        
+        For bugs please use [GitHub issues](https://github.com/RonenNess/html_validator/issues).
+        For other matters feel free to contact me at nad2000@gmail.com.
         
-           Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-           Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
-           Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
-           ...
-        
-        Contact
-        -------
-        
-        For bugs please use `GitHub issues`_. For other matters feel free to
-        contact me at nad2000@gmail.com.
-        
-        .. _GitHub issues: https://github.com/RonenNess/html_validator/issues
-        
-        
-Keywords: html validator
-html
-validator
-checker
-html5
-w3
+Keywords: html validator,html,validator,checker,html5,w3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Online-W3C-Validator-0.3.9/Online_W3C_Validator.egg-info/PKG-INFO` & `Online-W3C-Validator-0.3a0/Online_W3C_Validator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: Online-W3C-Validator
-Version: 0.3.9
+Version: 0.3a0
 Summary: UNKNOWN
 Home-page: https://github.com/nad2000/W3C-Validator
 Author: Radomirs Cirskis
 Author-email: nad2000@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nad2000/W3C-Validator
-Description: Online W3C Validator
-        ====================
+Description-Content-Type: UNKNOWN
+Description: # Online W3C Validator
         
-        Pure Python command line for HTML validation using W3C online validator.
-        It could be very handy for using it in a CI pipline.
+        Pure Python command line for HTML validation using W3C online validator. It could be very handy for using it in a CI pipline.
         
-        Installation
-        ------------
+        ## Installation
         
-        .. code:: bash
+        ```bash
+        pip install -U Online-W3C-Validator
+        ```
         
-           pip install -U Online-W3C-Validator
-        
-        How to use
-        ----------
+        ## How to use
         
         You can user the CLI command:
         
-        .. code:: bash
-        
-           w3c_validator http://www.google.com some_file.html
+        ```bash
+        w3c_validator http://www.google.com some_file.html
+        ```
         
         Example output:
         
-        ::
-        
-           INFO:w3c_validator.validator:Files to validate:
-             http://www.google.com
-           INFO:w3c_validator.validator:Number of files: 1
-           INFO:w3c_validator.validator:validating: http://www.google.com ...
-           error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-           error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-           error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           error: line 5: Attribute “width” not allowed on element “div” at this point.
-           error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           error: line 5: The “center” element is obsolete. Use CSS instead.
-           error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-        
-        Or you can use the fuction **validdate** provied by the package, that
-        thakes either HTML file name or URL as a single parameter an returns
-        JSON object with the validation output.
-        
-        .. code:: py
-        
-           from w3c_validator import validate
-        
-           messages = validate("http://www.google.com")["messages"]
-           for m in messages:
-               print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+        ```
+        INFO:w3c_validator.validator:Files to validate: 
+          http://www.google.com
+        INFO:w3c_validator.validator:Number of files: 1
+        INFO:w3c_validator.validator:validating: http://www.google.com ...
+        error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+        error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+        error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        error: line 5: Attribute “width” not allowed on element “div” at this point.
+        error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        error: line 5: The “center” element is obsolete. Use CSS instead.
+        error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+        ```
+        
+        Or you can use the fuction **validdate** provied by the package, that thakes either HTML file name or URL as a single parameter an returns JSON object with the validation output.
+        
+        ```py
+        from w3c_validator import validate
+        
+        messages = validate("http://www.google.com")["messages"]
+        for m in messages:
+            print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+        ```
         
         Example output:
         
-        ::
+        ```
+        Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+        Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
+        Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+        Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
+        Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
+        ...
+        ```
+        
+        ## Contact
+        
+        For bugs please use [GitHub issues](https://github.com/RonenNess/html_validator/issues).
+        For other matters feel free to contact me at nad2000@gmail.com.
         
-           Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-           Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
-           Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-           Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
-           Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
-           ...
-        
-        Contact
-        -------
-        
-        For bugs please use `GitHub issues`_. For other matters feel free to
-        contact me at nad2000@gmail.com.
-        
-        .. _GitHub issues: https://github.com/RonenNess/html_validator/issues
-        
-        
-Keywords: html validator
-html
-validator
-checker
-html5
-w3
+Keywords: html validator,html,validator,checker,html5,w3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Online-W3C-Validator-0.3.9/README.rst` & `Online-W3C-Validator-0.3a0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,63 @@
-Online W3C Validator
-====================
+# Online W3C Validator
 
-Pure Python command line for HTML validation using W3C online validator.
-It could be very handy for using it in a CI pipline.
+Pure Python command line for HTML validation using W3C online validator. It could be very handy for using it in a CI pipline.
 
-Installation
-------------
+## Installation
 
-.. code:: bash
+```bash
+pip install -U Online-W3C-Validator
+```
 
-   pip install -U Online-W3C-Validator
-
-How to use
-----------
+## How to use
 
 You can user the CLI command:
 
-.. code:: bash
-
-   w3c_validator http://www.google.com some_file.html
+```bash
+w3c_validator http://www.google.com some_file.html
+```
 
 Example output:
 
-::
-
-   INFO:w3c_validator.validator:Files to validate:
-     http://www.google.com
-   INFO:w3c_validator.validator:Number of files: 1
-   INFO:w3c_validator.validator:validating: http://www.google.com ...
-   error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-   error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-   error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-   error: line 5: Attribute “width” not allowed on element “div” at this point.
-   error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-   error: line 5: The “center” element is obsolete. Use CSS instead.
-   error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-
-Or you can use the fuction **validdate** provied by the package, that
-thakes either HTML file name or URL as a single parameter an returns
-JSON object with the validation output.
-
-.. code:: py
-
-   from w3c_validator import validate
-
-   messages = validate("http://www.google.com")["messages"]
-   for m in messages:
-       print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+```
+INFO:w3c_validator.validator:Files to validate: 
+  http://www.google.com
+INFO:w3c_validator.validator:Number of files: 1
+INFO:w3c_validator.validator:validating: http://www.google.com ...
+error: line 2: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+error: line 2: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+error: line 5: Attribute “width” not allowed on element “div” at this point.
+error: line 5: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+error: line 5: The “center” element is obsolete. Use CSS instead.
+error: line 5: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+```
+
+Or you can use the fuction **validdate** provied by the package, that thakes either HTML file name or URL as a single parameter an returns JSON object with the validation output.
+
+```py
+from w3c_validator import validate
+
+messages = validate("http://www.google.com")["messages"]
+for m in messages:
+    print("Type: %(type)s, Line: %(lastLine)d, Description: %(message)s" % m)
+```
 
 Example output:
 
-::
-
-   Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
-   Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
-   Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-   Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
-   Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
-   Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
-   Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
-   Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
-   Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
-   ...
-
-Contact
--------
+```
+Type: error, Line: 2, Description: CSS: “display”: “inline-box” is not a “display” value in “inline-box” in “.ds”.
+Type: error, Line: 2, Description: The “bgcolor” attribute on the “body” element is obsolete. Use CSS instead.
+Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+Type: error, Line: 5, Description: Attribute “width” not allowed on element “div” at this point.
+Type: error, Line: 5, Description: Element “nobr” not allowed as child of element “div” in this context. (Suppressing further errors from this subtree.)
+Type: error, Line: 5, Description: The “center” element is obsolete. Use CSS instead.
+Type: error, Line: 5, Description: The “clear” attribute on the “br” element is obsolete. Use CSS instead.
+Type: error, Line: 5, Description: The “align” attribute on the “div” element is obsolete. Use CSS instead.
+Type: error, Line: 5, Description: Attribute “nowrap” not allowed on element “div” at this point.
+...
+```
 
-For bugs please use `GitHub issues`_. For other matters feel free to
-contact me at nad2000@gmail.com.
+## Contact
 
-.. _GitHub issues: https://github.com/RonenNess/html_validator/issues
+For bugs please use [GitHub issues](https://github.com/RonenNess/html_validator/issues).
+For other matters feel free to contact me at nad2000@gmail.com.
```

### Comparing `Online-W3C-Validator-0.3.9/w3c_validator/validator.py` & `Online-W3C-Validator-0.3a0/w3c_validator/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     is_remote = filename.startswith("http://") or filename.startswith(
         "https://")
     with tempfile.TemporaryFile() if is_remote else open(
             filename, "rb") as f:
 
         if is_remote:
-            r = requests.get(filename, verify=False)
+            r = requests.get(filename)
             f.write(r.content)
             f.seek(0)
 
         # if is_css:
         #     cmd = (
         #         "curl -sF \"file=@%s;type=text/css\" -F output=json -F warning=0 %s"
         #         % (quoted_filename, CSS_VALIDATOR_URL))
@@ -56,16 +56,15 @@
         # else:
         r = requests.post(
             HTML_VALIDATOR_URL,
             files={"file": (filename, f, "text/html")},
             data={
                 "out": "json",
                 "showsource": "yes",
-            },
-            verify=False)
+            })
 
     return r.json()
 
 
 def main():
     """Parser the command line and run the validator."""
     parser = argparse.ArgumentParser(
```

