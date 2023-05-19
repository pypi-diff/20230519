# Comparing `tmp/xpanther-1.0.7.tar.gz` & `tmp/xpanther-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.0.7.tar", last modified: Thu May 18 11:49:38 2023, max compression
+gzip compressed data, was "xpanther-1.0.8.tar", last modified: Fri May 19 18:14:05 2023, max compression
```

## Comparing `xpanther-1.0.7.tar` & `xpanther-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:49:38.222537 xpanther-1.0.7/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     5854 2023-05-18 11:49:38.222537 xpanther-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5386 2023-02-19 14:07:14.000000 xpanther-1.0.7/README.md
--rw-rw-rw-   0        0        0      624 2023-05-18 11:49:03.000000 xpanther-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 11:49:38.226403 xpanther-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 11:49:38.175755 xpanther-1.0.7/xpanther/
--rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.7/xpanther/__init__.py
--rw-rw-rw-   0        0        0    19992 2023-05-07 13:42:55.000000 xpanther-1.0.7/xpanther/main.py
--rw-rw-rw-   0        0        0     2651 2023-05-18 11:49:03.000000 xpanther-1.0.7/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:49:38.220021 xpanther-1.0.7/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5854 2023-05-18 11:49:38.000000 xpanther-1.0.7/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-18 11:49:38.000000 xpanther-1.0.7/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:49:38.000000 xpanther-1.0.7/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-18 11:49:38.000000 xpanther-1.0.7/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 11:49:38.000000 xpanther-1.0.7/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.251338 xpanther-1.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5475 2023-05-19 18:14:05.249321 xpanther-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5007 2023-05-19 18:13:20.000000 xpanther-1.0.8/README.md
+-rw-rw-rw-   0        0        0      624 2023-05-19 17:53:50.000000 xpanther-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:14:05.251338 xpanther-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.206578 xpanther-1.0.8/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.8/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    19992 2023-05-19 17:48:05.000000 xpanther-1.0.8/xpanther/main.py
+-rw-rw-rw-   0        0        0     4649 2023-05-19 17:53:16.000000 xpanther-1.0.8/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:14:05.247616 xpanther-1.0.8/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5475 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 18:14:05.000000 xpanther-1.0.8/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.0.7/LICENSE` & `xpanther-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.7/PKG-INFO` & `xpanther-1.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.7
+Version: 1.0.8
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -19,93 +19,94 @@
 ## Find Unique Xpath expressions of HTML/XML elements.
 
 ### Mostly intended for Selenium and Appium automators.
 
 ### This python module's objective is to find unique xpath selector for any element in a document, using unique attributes/combination of attributes/parent or child relationship methods to find and write such expression for correctly identifying that element.
 
 ## How to install:
-    
-    pip install xpanther
-    
-or search it by 'xpanther' if you have editor with package installer.
+```python
+pip install xpanther
+```   
+_or search it by `xpanther` if you have editor with package installer. If it doesn't show up (happens in pycharm sometimes), go to global site-packages (`pip show xpanther`<--cmd command to find directory), find and copy xpanther package, and paste it to your project's venv._
 
-
-Then, import it to your file like:
+## This package contains 2 modules, `XPanther` and `XPantherIDE`, let's start with the powerhouse!
+Import XPanther to your file like:
   
-    from xpanther import XPanther
-    
-#### If it doesn't show up (happens in pycharm sometimes), go to global site-packages ({pip show xpanther}<--cmd command to find directory), find and copy xpanther package, and paste it to your project's venv.
+```python
+from xpanther import XPanther
+```
+
 
 ## How to use:
 
 #### Insert inside **_XPanther()_** the whole **HTML/XML** text, which can be in the form of:
 - **string**, 
 - the **path** to any local text file you might have or 
 - a page **url** (check below for optional-parameter page_url).
 
 #### Insert inside **._capture()_** the **outerHTML/whole** text of element to be found:
 - as a **string**
 - or alternatively an **integer**, which represents the index of that element in the DOM, starting from 1 as the first (check below for interesting usage of index input).
 
+```python
+XPanther(dom).capture(element)
+```
+
 After writing this , run the code and the **xpath** of that element should be returned as value and printed in the console.
 
 #### Code execution illustrations:
 
 <img src="https://user-images.githubusercontent.com/108073687/219906727-07172ca3-b5e9-4170-9538-9d0c777fb4c5.jpg" width="900">
 <img src="https://user-images.githubusercontent.com/108073687/219906731-d7215aab-1526-440f-809a-f14c6f3b31ab.jpg" width="900">
     
 #### **The class has a few optional-parameters that you can change to modify it in the way you want:**
 
-- **xml**, default is False, you MUST set it to True if document is not HTML, this is because the xml document can contain uppercase characters in attributes, unlike html, so a different parser needs to be used.
+- `xml` (default: `False`): Set this to `True` if document is not HTML, this is because the xml document can contain uppercase characters in attributes, unlike html, so a different parser needs to be used.
 
-- **pre_formatted**, default is False, you can set it to True if you have already formatted document and don't want formatter of XPanther to change anything.
+- `pre_formatted` (default: `False`): Set this to `True` if you have already formatted document and don't want formatter of XPanther to change anything.
 
-- **url_input**, default is False, should set to True if you intend to insert page url intead of text or file as the dom parameter of this class.
+- `url_input` (default: `False`): Set this to `True` if you intend to insert page url intead of text or file as the dom parameter of this class.
 
-- **child_method**, default is True, you can set it to False if you don't want the Xpath to be found using its children, reason for this can depend on context.
+- `child_method` (default: `True`): Set this to `False` if you don't want the Xpath to be found using its children, reason for this can depend on context.
 
-- **show_all**, default is False, set it to True if you want all possible working xpaths found and not resort to only the one chosen by program.
+- `show_all` (default: `False`): Set this to `True` if you want all possible working xpaths found and not resort to only the one chosen by program.
 
-- **no_digits**, default is False, set it to True if you don't want element attributes that contain numbers.
+- `no_digits` (default: `False`): Set this to `True` if you don't want element attributes that contain numbers.
 
-- **print_output**, default is True, you might set it to False if you don't want the program to print anything in console but just return the xpath as a value in any variable or function.
+- `print_output` (default: `True`): Set this to `False` if you don't want the program to print anything in console but just return the xpath as a value in any variable or function.
 
-- **speed**, default is 'normal', other valid options are 'fast' -- (less detailed, faster execution), 'slow' -- (more detailed, slower execution), or an integer (maximum is 50, which represent the number of attributes of element program can take and proccess to find combinations of).
-          'slow' can take as much as 35 attributes of element to go on and find combinations of, it is my recommended maximum limit, any more than that might crash the computer.
+- `speed`  (default: `'normal'`): other valid options are `'fast'` -- (less detailed, faster execution), `'slow'` -- (more detailed, slower execution), or an integer (maximum is 50, which represent the number of attributes of element program can take and proccess to find combinations of).
           if you have a slow computer, better set it to 'fast', cause it takes lesser number of combination and lowers memory and performance consumption, thus increasing speed of execution.
 
-## For most optimal usage, keep this values as default, you have to only change  to xml=True if you are not dealing with HTML, and url_input=True if you like to fetch the HTML directly from link. 
+### For most optimal usage, keep this values as default, you have to only change  to xml=True if you are not dealing with HTML, and url_input=True if you like to fetch the HTML directly from link. 
 
 
 #### Interesting way which you can utilize putting an integer as parameter to capture(), is this function like here:
-
-      for x in range(100):
-          XPanther('xpath_test.txt').capture(x+1)
-
+```python
+for x in range(100):
+    XPanther('xpath_test.txt').capture(x+1)
+```
 Literally, create and write an unique xpath for every element in the document if you want (change the number in range() accordingly).
 
 
 
-## If you are into web automation, that's where **XPantherIDE** comes into play.
+# If you are into web automation, that's where `XPantherIDE` comes into play.
 
-XPantherIDE is a simple script, which opens a chrome browser on your preferred starting page url, and will register any click made in the page, after you close the browser as you normally would, every unique xpath of element you clicked upon will be shown in succession, thus making automation a lot easier, especially for people who struggle finding xpaths.
+`XPantherIDE` is a simple Selenium script, that tries to mimic an IDE for finding xpaths instantly on any web page with just 1 click.
 
 Import:
-    
-    from xpanther import XPantherIDE
-    
+```python
+from xpanther import XPantherIDE
+```
 Use:
-
-    XPantherIDE('page_url').start()
-    
-#### Output from using XPantherIDE:
-   <img src="https://user-images.githubusercontent.com/108073687/218467068-292fab8b-844d-4566-a180-31af161fbbaa.jpg" width = "500">
+```python
+XPantherIDE('page_url').start()
+```   
     
-
---**DISCLAIMER**-- This script is still experimental, buttons that can redirect the page don't return value for the moment, this is a bug that will be fixed in the future.
+#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again.
 
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.0.7/README.md` & `xpanther-1.0.8/xpanther.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,98 +1,112 @@
+Metadata-Version: 2.1
+Name: xpanther
+Version: 1.0.8
+Summary: Find Unique Xpath of any HTML/XML element
+Author-email: Flori Batusha <floribatusha0@gmail.com>
+Project-URL: Check Github, https://github.com/riflosnake/XPanther
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # XPanther
         
         
 <img src="https://user-images.githubusercontent.com/108073687/219871468-2fb5c446-dbb4-43eb-83c3-41d1f90c682d.jpg" width="500" height="300">
 
 ## Find Unique Xpath expressions of HTML/XML elements.
 
 ### Mostly intended for Selenium and Appium automators.
 
 ### This python module's objective is to find unique xpath selector for any element in a document, using unique attributes/combination of attributes/parent or child relationship methods to find and write such expression for correctly identifying that element.
 
 ## How to install:
-    
-    pip install xpanther
-    
-or search it by 'xpanther' if you have editor with package installer.
-
+```python
+pip install xpanther
+```   
+_or search it by `xpanther` if you have editor with package installer. If it doesn't show up (happens in pycharm sometimes), go to global site-packages (`pip show xpanther`<--cmd command to find directory), find and copy xpanther package, and paste it to your project's venv._
 
-Then, import it to your file like:
+## This package contains 2 modules, `XPanther` and `XPantherIDE`, let's start with the powerhouse!
+Import XPanther to your file like:
   
-    from xpanther import XPanther
-    
-#### If it doesn't show up (happens in pycharm sometimes), go to global site-packages ({pip show xpanther}<--cmd command to find directory), find and copy xpanther package, and paste it to your project's venv.
+```python
+from xpanther import XPanther
+```
+
 
 ## How to use:
 
 #### Insert inside **_XPanther()_** the whole **HTML/XML** text, which can be in the form of:
 - **string**, 
 - the **path** to any local text file you might have or 
 - a page **url** (check below for optional-parameter page_url).
 
 #### Insert inside **._capture()_** the **outerHTML/whole** text of element to be found:
 - as a **string**
 - or alternatively an **integer**, which represents the index of that element in the DOM, starting from 1 as the first (check below for interesting usage of index input).
 
+```python
+XPanther(dom).capture(element)
+```
+
 After writing this , run the code and the **xpath** of that element should be returned as value and printed in the console.
 
 #### Code execution illustrations:
 
 <img src="https://user-images.githubusercontent.com/108073687/219906727-07172ca3-b5e9-4170-9538-9d0c777fb4c5.jpg" width="900">
 <img src="https://user-images.githubusercontent.com/108073687/219906731-d7215aab-1526-440f-809a-f14c6f3b31ab.jpg" width="900">
     
 #### **The class has a few optional-parameters that you can change to modify it in the way you want:**
 
-- **xml**, default is False, you MUST set it to True if document is not HTML, this is because the xml document can contain uppercase characters in attributes, unlike html, so a different parser needs to be used.
+- `xml` (default: `False`): Set this to `True` if document is not HTML, this is because the xml document can contain uppercase characters in attributes, unlike html, so a different parser needs to be used.
 
-- **pre_formatted**, default is False, you can set it to True if you have already formatted document and don't want formatter of XPanther to change anything.
+- `pre_formatted` (default: `False`): Set this to `True` if you have already formatted document and don't want formatter of XPanther to change anything.
 
-- **url_input**, default is False, should set to True if you intend to insert page url intead of text or file as the dom parameter of this class.
+- `url_input` (default: `False`): Set this to `True` if you intend to insert page url intead of text or file as the dom parameter of this class.
 
-- **child_method**, default is True, you can set it to False if you don't want the Xpath to be found using its children, reason for this can depend on context.
+- `child_method` (default: `True`): Set this to `False` if you don't want the Xpath to be found using its children, reason for this can depend on context.
 
-- **show_all**, default is False, set it to True if you want all possible working xpaths found and not resort to only the one chosen by program.
+- `show_all` (default: `False`): Set this to `True` if you want all possible working xpaths found and not resort to only the one chosen by program.
 
-- **no_digits**, default is False, set it to True if you don't want element attributes that contain numbers.
+- `no_digits` (default: `False`): Set this to `True` if you don't want element attributes that contain numbers.
 
-- **print_output**, default is True, you might set it to False if you don't want the program to print anything in console but just return the xpath as a value in any variable or function.
+- `print_output` (default: `True`): Set this to `False` if you don't want the program to print anything in console but just return the xpath as a value in any variable or function.
 
-- **speed**, default is 'normal', other valid options are 'fast' -- (less detailed, faster execution), 'slow' -- (more detailed, slower execution), or an integer (maximum is 50, which represent the number of attributes of element program can take and proccess to find combinations of).
-          'slow' can take as much as 35 attributes of element to go on and find combinations of, it is my recommended maximum limit, any more than that might crash the computer.
+- `speed`  (default: `'normal'`): other valid options are `'fast'` -- (less detailed, faster execution), `'slow'` -- (more detailed, slower execution), or an integer (maximum is 50, which represent the number of attributes of element program can take and proccess to find combinations of).
           if you have a slow computer, better set it to 'fast', cause it takes lesser number of combination and lowers memory and performance consumption, thus increasing speed of execution.
 
-## For most optimal usage, keep this values as default, you have to only change  to xml=True if you are not dealing with HTML, and url_input=True if you like to fetch the HTML directly from link. 
+### For most optimal usage, keep this values as default, you have to only change  to xml=True if you are not dealing with HTML, and url_input=True if you like to fetch the HTML directly from link. 
 
 
 #### Interesting way which you can utilize putting an integer as parameter to capture(), is this function like here:
-
-      for x in range(100):
-          XPanther('xpath_test.txt').capture(x+1)
-
+```python
+for x in range(100):
+    XPanther('xpath_test.txt').capture(x+1)
+```
 Literally, create and write an unique xpath for every element in the document if you want (change the number in range() accordingly).
 
 
 
-## If you are into web automation, that's where **XPantherIDE** comes into play.
+# If you are into web automation, that's where `XPantherIDE` comes into play.
 
-XPantherIDE is a simple script, which opens a chrome browser on your preferred starting page url, and will register any click made in the page, after you close the browser as you normally would, every unique xpath of element you clicked upon will be shown in succession, thus making automation a lot easier, especially for people who struggle finding xpaths.
+`XPantherIDE` is a simple Selenium script, that tries to mimic an IDE for finding xpaths instantly on any web page with just 1 click.
 
 Import:
-    
-    from xpanther import XPantherIDE
-    
+```python
+from xpanther import XPantherIDE
+```
 Use:
-
-    XPantherIDE('page_url').start()
-    
-#### Output from using XPantherIDE:
-   <img src="https://user-images.githubusercontent.com/108073687/218467068-292fab8b-844d-4566-a180-31af161fbbaa.jpg" width = "500">
+```python
+XPantherIDE('page_url').start()
+```   
     
-
---**DISCLAIMER**-- This script is still experimental, buttons that can redirect the page don't return value for the moment, this is a bug that will be fixed in the future.
+#### After you run the program, the browser will open, and you can start finding xpaths by `right-clicking` over elements. A pop up alert will appear showing the xpath, you must accept/close the pop up before trying again.
 
 ### **Both programs are open to improvements or new ideas!**
```

### Comparing `xpanther-1.0.7/xpanther/main.py` & `xpanther-1.0.8/xpanther/main.py`

 * *Files identical despite different names*

