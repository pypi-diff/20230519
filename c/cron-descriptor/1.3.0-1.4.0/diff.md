# Comparing `tmp/cron_descriptor-1.3.0.tar.gz` & `tmp/cron_descriptor-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron_descriptor-1.3.0.tar", last modified: Fri May  5 12:10:03 2023, max compression
+gzip compressed data, was "cron_descriptor-1.4.0.tar", last modified: Fri May 19 07:46:15 2023, max compression
```

## Comparing `cron_descriptor-1.3.0.tar` & `cron_descriptor-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7196 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.682659 cron_descriptor-1.3.0/cron_descriptor/
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/CasingTypeEnum.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/DescriptionTypeEnum.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/Exception.py
--rw-rw-rw-   0 root         (0) root         (0)    25057 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/ExpressionDescriptor.py
--rw-rw-rw-   0 root         (0) root         (0)     9459 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/ExpressionParser.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/GetText.py
--rw-rw-rw-   0 root         (0) root         (0)     1697 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/Options.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/StringBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/cron_descriptor/locale/
--rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/cs_CZ.mo
--rw-rw-rw-   0 root         (0) root         (0)     2701 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/de_DE.mo
--rw-rw-rw-   0 root         (0) root         (0)     3719 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/en_US.mo
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/es_ES.mo
--rw-rw-rw-   0 root         (0) root         (0)     3203 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/fa_IR.mo
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/fr_FR.mo
--rw-rw-rw-   0 root         (0) root         (0)     2783 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/it_IT.mo
--rw-rw-rw-   0 root         (0) root         (0)     3039 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ja_JP.mo
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ko_KR.mo
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/nb_NO.mo
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/nl_NL.mo
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/pt_PT.mo
--rw-rw-rw-   0 root         (0) root         (0)     3116 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ru_RU.mo
--rw-rw-rw-   0 root         (0) root         (0)     2887 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/sk_SK.mo
--rw-rw-rw-   0 root         (0) root         (0)     3177 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/sv_SE.mo
--rw-rw-rw-   0 root         (0) root         (0)     4681 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ta_IN.mo
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/tr_TR.mo
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/uk_UA.mo
--rw-rw-rw-   0 root         (0) root         (0)     2675 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/zh_CN.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/cron_descriptor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7196 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1133 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3162 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:46:15.736442 cron_descriptor-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-19 07:46:15.736442 cron_descriptor-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:46:15.732442 cron_descriptor-1.4.0/cron_descriptor/
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/CasingTypeEnum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/DescriptionTypeEnum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/Exception.py
+-rw-rw-rw-   0 root         (0) root         (0)    25057 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/ExpressionDescriptor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/ExpressionParser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/GetText.py
+-rw-rw-rw-   0 root         (0) root         (0)     1697 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/Options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/StringBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:46:15.736442 cron_descriptor-1.4.0/cron_descriptor/locale/
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/cs_CZ.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/de_DE.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/en_US.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/es_ES.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3203 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/fa_IR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/fr_FR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/it_IT.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/ja_JP.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/ko_KR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/nb_NO.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/nl_NL.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/pt_PT.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/ru_RU.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/sk_SK.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/sv_SE.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4681 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/ta_IN.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/tr_TR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/uk_UA.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/vi_VN.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/cron_descriptor/locale/zh_CN.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:46:15.732442 cron_descriptor-1.4.0/cron_descriptor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-19 07:46:15.000000 cron_descriptor-1.4.0/cron_descriptor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-05-19 07:46:15.000000 cron_descriptor-1.4.0/cron_descriptor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 07:46:15.000000 cron_descriptor-1.4.0/cron_descriptor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 07:46:15.000000 cron_descriptor-1.4.0/cron_descriptor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 07:46:15.000000 cron_descriptor-1.4.0/cron_descriptor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 07:46:15.736442 cron_descriptor-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-05-19 07:45:21.000000 cron_descriptor-1.4.0/setup.py
```

### Comparing `cron_descriptor-1.3.0/LICENSE` & `cron_descriptor-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/PKG-INFO` & `cron_descriptor-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cron_descriptor
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python library that converts cron expressions into human readable strings.
 Home-page: https://github.com/Salamek/cron-descriptor
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: UNKNOWN
 Description: # Cron Descriptor
```

### Comparing `cron_descriptor-1.3.0/README.md` & `cron_descriptor-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/CasingTypeEnum.py` & `cron_descriptor-1.4.0/cron_descriptor/CasingTypeEnum.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/DescriptionTypeEnum.py` & `cron_descriptor-1.4.0/cron_descriptor/DescriptionTypeEnum.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/Exception.py` & `cron_descriptor-1.4.0/cron_descriptor/Exception.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/ExpressionDescriptor.py` & `cron_descriptor-1.4.0/cron_descriptor/ExpressionDescriptor.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/ExpressionParser.py` & `cron_descriptor-1.4.0/cron_descriptor/ExpressionParser.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/GetText.py` & `cron_descriptor-1.4.0/cron_descriptor/GetText.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/Options.py` & `cron_descriptor-1.4.0/cron_descriptor/Options.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/StringBuilder.py` & `cron_descriptor-1.4.0/cron_descriptor/StringBuilder.py`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/__init__.py` & `cron_descriptor-1.4.0/cron_descriptor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 from .Options import Options
 from .ExpressionDescriptor import ExpressionDescriptor, get_description
 from .DescriptionTypeEnum import DescriptionTypeEnum
 from .CasingTypeEnum import CasingTypeEnum
 from .Exception import MissingFieldException, FormatException, WrongArgumentException
 
 
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 __all__ = ['Options', 'ExpressionDescriptor', 'get_description', 'DescriptionTypeEnum',
            'CasingTypeEnum', 'MissingFieldException', 'FormatException', 'WrongArgumentException']
```

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/cs_CZ.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/cs_CZ.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/de_DE.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/de_DE.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/en_US.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/en_US.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/es_ES.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/es_ES.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/fa_IR.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/fa_IR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/fr_FR.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/fr_FR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/it_IT.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/it_IT.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/ja_JP.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/ja_JP.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/ko_KR.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/ko_KR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/nb_NO.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/nb_NO.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/nl_NL.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/nl_NL.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/pt_PT.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/pt_PT.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/ru_RU.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/ru_RU.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/sk_SK.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/sk_SK.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/sv_SE.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/sv_SE.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/ta_IN.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/ta_IN.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/tr_TR.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/tr_TR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/uk_UA.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/uk_UA.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor/locale/zh_CN.mo` & `cron_descriptor-1.4.0/cron_descriptor/locale/zh_CN.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.3.0/cron_descriptor.egg-info/PKG-INFO` & `cron_descriptor-1.4.0/cron_descriptor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cron-descriptor
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python library that converts cron expressions into human readable strings.
 Home-page: https://github.com/Salamek/cron-descriptor
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: UNKNOWN
 Description: # Cron Descriptor
```

### Comparing `cron_descriptor-1.3.0/cron_descriptor.egg-info/SOURCES.txt` & `cron_descriptor-1.4.0/cron_descriptor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 cron_descriptor/locale/pt_PT.mo
 cron_descriptor/locale/ru_RU.mo
 cron_descriptor/locale/sk_SK.mo
 cron_descriptor/locale/sv_SE.mo
 cron_descriptor/locale/ta_IN.mo
 cron_descriptor/locale/tr_TR.mo
 cron_descriptor/locale/uk_UA.mo
+cron_descriptor/locale/vi_VN.mo
 cron_descriptor/locale/zh_CN.mo
```

### Comparing `cron_descriptor-1.3.0/setup.py` & `cron_descriptor-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     if sys.version_info >= (3, 0):
         long_description = open('README.md', encoding='utf-8').read()
     else:
         long_description = open('README.md').read()
     
     setuptools.setup(
         name="cron_descriptor",
-        version="1.3.0",
+        version="1.4.0",
         description="A Python library that converts cron expressions "
                     "into human readable strings.",
         author="Adam Schubert",
         author_email="adam.schubert@sg1-game.net",
         url="https://github.com/Salamek/cron-descriptor",
         long_description=long_description,
         long_description_content_type='text/markdown',
```

