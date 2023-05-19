# Comparing `tmp/python-negar-1.2.tar.gz` & `tmp/python-negar-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-negar-1.2.tar", last modified: Tue Mar 28 19:00:52 2023, max compression
+gzip compressed data, was "python-negar-1.2.1.tar", last modified: Fri May 19 07:45:40 2023, max compression
```

## Comparing `python-negar-1.2.tar` & `python-negar-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-03-28 19:00:52.717454 python-negar-1.2/
--rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2/AUTHORS
--rw-r--r--   0 javad     (1000) javad     (1000)     6453 2023-03-28 18:59:30.000000 python-negar-1.2/Changelog.txt
--rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      149 2022-03-28 12:06:56.000000 python-negar-1.2/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     8546 2023-03-28 19:00:52.717454 python-negar-1.2/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-03-28 19:00:52.717454 python-negar-1.2/negar/
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2/negar/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)     5045 2023-03-28 18:59:35.000000 python-negar-1.2/negar/constants.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-03-28 19:00:52.717454 python-negar-1.2/negar/data/
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2/negar/data/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2/negar/data/untouchable.dat
--rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2/negar/gui.py
--rw-r--r--   0 javad     (1000) javad     (1000)    14262 2022-12-21 09:17:55.000000 python-negar-1.2/negar/virastar.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-03-28 19:00:52.717454 python-negar-1.2/python_negar.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     8546 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-03-28 19:00:52.000000 python-negar-1.2/python_negar.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-03-28 19:00:52.717454 python-negar-1.2/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.341991 python-negar-1.2.1/
+-rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.1/AUTHORS
+-rw-r--r--   0 javad     (1000) javad     (1000)     6531 2023-05-19 07:44:53.000000 python-negar-1.2.1/Changelog.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.1/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      149 2022-03-28 12:06:56.000000 python-negar-1.2.1/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-05-19 07:45:40.338657 python-negar-1.2.1/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.1/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/negar/
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.1/negar/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-05-19 07:23:16.000000 python-negar-1.2.1/negar/constants.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/negar/data/
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.1/negar/data/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.1/negar/data/untouchable.dat
+-rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.1/negar/gui.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    14546 2023-05-19 07:36:41.000000 python-negar-1.2.1/negar/virastar.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-19 07:45:40.338657 python-negar-1.2.1/python_negar.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-05-19 07:45:40.000000 python-negar-1.2.1/python_negar.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-05-19 07:45:40.341991 python-negar-1.2.1/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.1/setup.py
```

### Comparing `python-negar-1.2/Changelog.txt` & `python-negar-1.2.1/Changelog.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.2.1 - 2023-05-23
+-- Fix an issue with punctuation like  '،ساختمان'
+
 1.2 - 2023-03-28
 -- Fix GUI execution issue
 
 1.1.17 - 2022-12-21
 -- Fix the issue with می and نمی when they come as nouns, not prefixes.
 -- Several new untouchable words: تنهای/تنهایی/تک‌وتنهایی
```

### Comparing `python-negar-1.2/LICENSE` & `python-negar-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-negar-1.2/PKG-INFO` & `python-negar-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2
+Version: 1.2.1
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2/README.md` & `python-negar-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python-negar-1.2/negar/constants.py` & `python-negar-1.2.1/negar/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-__version__ = "1.2"
+__version__ = "1.2.1"
 
 DATAFILE = Path(__file__).parent.absolute() / "data/untouchable.dat"
 USERFILE = Path.home() / ".python-negar"
 
 INFO = f"""قابلیت های ویراستار ' نگار  ' -- نسخه {__version__} :
 * جایگزینی
 	╛═ خط تیره های پیاپی نظیر (--) و (---) با معادل های استاندارد شان
```

### Comparing `python-negar-1.2/negar/data/untouchable.dat` & `python-negar-1.2.1/negar/data/untouchable.dat`

 * *Files identical despite different names*

### Comparing `python-negar-1.2/negar/virastar.py` & `python-negar-1.2.1/negar/virastar.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,21 @@
         self._trim_leading_trailing_whitespaces = parse_args('trim-lt-whitespaces')
 
         UnTouchable() # to generate the untouchable words
         self.cleanup()
 
     def cleanup(self):
         self._handle_urls(State.save)
+        # fix punctuation spaces at first
+        # : ; , ! ? and their Persian counterparts should have one space after and no space before
+        self.text = re.sub(
+            r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
+            r'\1 ',
+            self.text
+        )
         if self._trim_leading_trailing_whitespaces:
             self.text = '\n'.join([line.strip() for line in self.text.split('\n')])
         self.cleanup_spacing()      if self._cleanup_spacing else None
         self.fix_dashes()           if self._fix_dashes else None
         self.fix_three_dots()       if self._fix_three_dots else None
         self.fix_english_quotes()   if self._fix_english_quotes else None
         self.fix_hamzeh()           if self._fix_hamzeh else None
@@ -238,20 +245,20 @@
 
     def fix_spacing_for_braces_and_quotes(self):
         """Fixes the braces and quotes spacing problems."""
         # ()[]{}""«» should have one space before and no space after (inside)
         for begin, end in zip(['\(','\[','\{','"','«'], ['\)','\]','\}','"','»']):
             self.text = re.sub(rf'[ ‌]*({begin})\s*([^{end}]+?)\s*?({end})[ ‌]*',
                 r' \1\2\3 ', self.text )
-        # : ; , ! ? and their Persian counterparts should have one space after and no space before
-        self.text = re.sub(
-            r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
-            r'\1 ',
-            self.text
-        )
+        # # : ; , ! ? and their Persian counterparts should have one space after and no space before
+        # self.text = re.sub(
+        #     r'[ ‌ ]*([:;,؛،.؟!]{1})[ ‌ ]*',
+        #     r'\1 ',
+        #     self.text
+        # )
         # special case for versioning numbers like 1.2.7
         self.text = re.sub(r'([\d])([.])\s([\d])([.])\s([\d])', r'\1\2\3\4\5', self.text)
         # special case for floating-point numbers like 12.7
         self.text = re.sub(r'([\d])([.])\s([\d])', r'\1\2\3', self.text)
         self.text = re.sub(
             r'[ ‌ ]*((؟\s+!){1})[ ‌ ]*',
             r'؟! ',
```

### Comparing `python-negar-1.2/python_negar.egg-info/PKG-INFO` & `python-negar-1.2.1/python_negar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2
+Version: 1.2.1
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2/setup.py` & `python-negar-1.2.1/setup.py`

 * *Files identical despite different names*

