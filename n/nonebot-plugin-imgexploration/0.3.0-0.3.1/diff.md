# Comparing `tmp/nonebot-plugin-imgexploration-0.3.0.tar.gz` & `tmp/nonebot-plugin-imgexploration-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-imgexploration-0.3.0.tar", last modified: Fri May 19 04:10:26 2023, max compression
+gzip compressed data, was "nonebot-plugin-imgexploration-0.3.1.tar", last modified: Fri May 19 04:37:04 2023, max compression
```

## Comparing `nonebot-plugin-imgexploration-0.3.0.tar` & `nonebot-plugin-imgexploration-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 04:10:26.861997 nonebot-plugin-imgexploration-0.3.0/
--rw-rw-rw-   0        0        0     1088 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      166 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2894 2023-05-19 04:10:26.860998 nonebot-plugin-imgexploration-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2141 2023-05-19 03:39:31.000000 nonebot-plugin-imgexploration-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 04:10:26.853997 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration/
--rw-rw-rw-   0        0        0     4314 2023-05-19 03:39:52.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration/__init__.py
--rw-rw-rw-   0        0        0    20846 2023-05-19 03:54:54.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration/imgexploration.py
-drwxrwxrwx   0        0        0        0 2023-05-19 04:10:26.859995 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/
--rw-rw-rw-   0        0        0     2894 2023-05-19 04:10:26.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-19 04:10:26.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 04:10:26.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-05-19 04:10:26.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-19 04:10:26.000000 nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      613 2023-05-19 04:10:17.000000 nonebot-plugin-imgexploration-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 04:10:26.861997 nonebot-plugin-imgexploration-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     8696 2023-05-19 04:10:17.000000 nonebot-plugin-imgexploration-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.397222 nonebot-plugin-imgexploration-0.3.1/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      166 2023-05-18 14:00:48.000000 nonebot-plugin-imgexploration-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2894 2023-05-19 04:37:04.396222 nonebot-plugin-imgexploration-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2141 2023-05-19 03:39:31.000000 nonebot-plugin-imgexploration-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.387222 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/
+-rw-rw-rw-   0        0        0     4314 2023-05-19 03:39:52.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/__init__.py
+-rw-rw-rw-   0        0        0    20816 2023-05-19 04:33:54.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/imgexploration.py
+drwxrwxrwx   0        0        0        0 2023-05-19 04:37:04.394223 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/
+-rw-rw-rw-   0        0        0     2894 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-19 04:37:04.000000 nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      613 2023-05-19 04:36:57.000000 nonebot-plugin-imgexploration-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 04:37:04.397222 nonebot-plugin-imgexploration-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     8696 2023-05-19 04:36:57.000000 nonebot-plugin-imgexploration-0.3.1/setup.py
```

### Comparing `nonebot-plugin-imgexploration-0.3.0/LICENSE.txt` & `nonebot-plugin-imgexploration-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.0/PKG-INFO` & `nonebot-plugin-imgexploration-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.3.0
+Version: 0.3.1
 Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: cpufan2001@gmail.com
 Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.0
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.1
 Summary: Nonebot2
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `nonebot-plugin-imgexploration-0.3.0/README.md` & `nonebot-plugin-imgexploration-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration/__init__.py` & `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration/imgexploration.py` & `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration/imgexploration.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
                 "Origin": "https://imgops.com",
                 "Referer": "https://imgops.com/",
                 "Accept-Encoding": "gzip, deflate, br",
                 "Accept-Language": "zh-CN,zh;q=0.9",
             }
             post = await self.client.post("https://imgops.com/store", files=files, data=data, headers=headers, timeout=10)
 
-            print(post.text)
             self.__imgopsUrl = "https:/" + post.text
         except Exception as e:
             self.__imgopsUrl = self.__pic_url
             logger.error(e)
 
     def setFront(self, big_size: int, nomal_size: int, small_size: int):
         """
```

### Comparing `nonebot-plugin-imgexploration-0.3.0/nonebot_plugin_imgexploration.egg-info/PKG-INFO` & `nonebot-plugin-imgexploration-0.3.1/nonebot_plugin_imgexploration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.3.0
+Version: 0.3.1
 Summary: Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: cpufan2001@gmail.com
 Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.0
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.3.1
 Summary: Nonebot2
 æä»¶ï¼GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: cpufan2001@gmail.com Keywords: nonebot nonebot-plugin imagesearch
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `nonebot-plugin-imgexploration-0.3.0/pyproject.toml` & `nonebot-plugin-imgexploration-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-imgexploration"
-version = "0.3.0"
+version = "0.3.1"
 description = "Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图"
 authors = ["cpufan"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_imgexploration"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot-plugin-imgexploration-0.3.0/setup.py` & `nonebot-plugin-imgexploration-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
     # Required
-    version="0.3.0",
+    version="0.3.1",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     # Optional
     description="Nonebot2 插件，Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

