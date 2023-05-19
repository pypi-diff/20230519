# Comparing `tmp/realtouch-0.1.6.tar.gz` & `tmp/realtouch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtouch-0.1.6.tar", last modified: Mon May 15 00:08:45 2023, max compression
+gzip compressed data, was "realtouch-0.1.7.tar", last modified: Fri May 19 16:11:32 2023, max compression
```

## Comparing `realtouch-0.1.6.tar` & `realtouch-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-15 00:08:45.599700 realtouch-0.1.6/
--rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.6/LICENSE
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-15 00:08:45.599432 realtouch-0.1.6/PKG-INFO
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-15 00:08:45.595119 realtouch-0.1.6/realtouch/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-15 00:08:45.596751 realtouch-0.1.6/realtouch/src/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-15 00:08:45.598888 realtouch-0.1.6/realtouch/src/realtouch.egg-info/
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-15 00:08:45.000000 realtouch-0.1.6/realtouch/src/realtouch.egg-info/PKG-INFO
--rw-r--r--   0 k          (501) staff       (20)      277 2023-05-15 00:08:45.000000 realtouch-0.1.6/realtouch/src/realtouch.egg-info/SOURCES.txt
--rw-r--r--   0 k          (501) staff       (20)        1 2023-05-15 00:08:45.000000 realtouch-0.1.6/realtouch/src/realtouch.egg-info/dependency_links.txt
--rw-r--r--   0 k          (501) staff       (20)       16 2023-05-15 00:08:45.000000 realtouch-0.1.6/realtouch/src/realtouch.egg-info/requires.txt
--rw-r--r--   0 k          (501) staff       (20)       10 2023-05-15 00:08:45.000000 realtouch-0.1.6/realtouch/src/realtouch.egg-info/top_level.txt
--rw-r--r--   0 k          (501) staff       (20)    21128 2023-05-15 00:02:46.000000 realtouch-0.1.6/realtouch/src/realtouch.py
--rw-r--r--   0 k          (501) staff       (20)       38 2023-05-15 00:08:45.599784 realtouch-0.1.6/setup.cfg
--rw-r--r--   0 k          (501) staff       (20)      852 2023-05-15 00:08:42.000000 realtouch-0.1.6/setup.py
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.955582 realtouch-0.1.7/
+-rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.7/LICENSE
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-19 16:11:32.955251 realtouch-0.1.7/PKG-INFO
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.950146 realtouch-0.1.7/realtouch/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.952076 realtouch-0.1.7/realtouch/src/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-19 16:11:32.954507 realtouch-0.1.7/realtouch/src/realtouch.egg-info/
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/PKG-INFO
+-rw-r--r--   0 k          (501) staff       (20)      277 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/SOURCES.txt
+-rw-r--r--   0 k          (501) staff       (20)        1 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/dependency_links.txt
+-rw-r--r--   0 k          (501) staff       (20)       16 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/requires.txt
+-rw-r--r--   0 k          (501) staff       (20)       10 2023-05-19 16:11:32.000000 realtouch-0.1.7/realtouch/src/realtouch.egg-info/top_level.txt
+-rw-r--r--   0 k          (501) staff       (20)    23629 2023-05-19 15:41:55.000000 realtouch-0.1.7/realtouch/src/realtouch.py
+-rw-r--r--   0 k          (501) staff       (20)       38 2023-05-19 16:11:32.955724 realtouch-0.1.7/setup.cfg
+-rw-r--r--   0 k          (501) staff       (20)      852 2023-05-19 09:06:04.000000 realtouch-0.1.7/setup.py
```

### Comparing `realtouch-0.1.6/LICENSE` & `realtouch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `realtouch-0.1.6/PKG-INFO` & `realtouch-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.6
+Version: 0.1.7
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.6/realtouch/src/realtouch.egg-info/PKG-INFO` & `realtouch-0.1.7/realtouch/src/realtouch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.6
+Version: 0.1.7
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.6/realtouch/src/realtouch.py` & `realtouch-0.1.7/realtouch/src/realtouch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import time
 from dataclasses import dataclass, asdict
 from enum import Enum
 from typing import Union, Any
 import requests
 from loguru import logger
 import re
 from pathlib import Path
@@ -64,14 +65,15 @@
             else:
                 result.append(asdict(loc))
         return result
     except Exception as e:
         logger.exception(e)
         return location
 
+
 class Robot:
     def __init__(self, ip: str):
         self.ip = ip
         self._phones: dict[int, Phone] = {}
         self.__load()
 
     def __load(self):
@@ -428,15 +430,15 @@
     def locate_image(
             self, template: Union[Path, bytes],
             image: Union[Path, bytes] = None,
             location: Union[ImgLocation, list[ImgLocation], ImgArea, list[ImgArea]] = ImgLocation.FULL,
             threshold=0.8
     ) -> list[TemplateLocation]:
         """
-        图查图. 仅作为实验用途. 如果效果可能不完美, 可以自行使用其它库去实现.
+        图查图. 仅作为实验用途. 如果效果不完美, 可以自行使用其它库去实现.
 
         :param template: 被查找的模版路径或者bytes
         :param image: 默认查找当前手机画面, 也可以提供被查图的路径或bytes
         :param location: 只查找指定位置
         :param threshold: 特征点集合阈值 , 0-∞, 越小越严格, 越大越宽松
         :return:
         """
@@ -478,14 +480,19 @@
     def hide_keyboard(self):
         """
         隐藏输入法键盘
         :return:
         """
         return self.enter_text(TextAction.KEYCODE_CLOSE)
 
+    def waited_update(self, before=2, after=2):
+        time.sleep(before)
+        self.update()
+        time.sleep(after)
+
 
 class Phone:
     def __init__(
             self,
             position: int,
             robot: Robot,
             data: dict
@@ -517,54 +524,100 @@
         :param file: 文件路径
         :param name: 自定义文件名, 需要包含扩展名!!
         :return:
         """
         with open(file, 'rb') as f:
             files = {'file': f if not name else (name, f)}
             url = f'http://{self.robot.ip}/api/upload/{self.position}/'
-            requests.post(
+            res = requests.post(
                 url, files=files,
-                timeout=(100, 100)
+                timeout=(1000, 1000)
             )
+            logger.debug(res)
+
+    def _page_changed(self, current_page: callable = None, next_page: callable = None,
+                      **kwargs):
+        self.screen.waited_update()
+        if callable(current_page):
+            current = current_page()
+            if not current:
+                return True
+        if callable(next_page):
+            next_ = next_page()
+            if next_:
+                return True
+        if not callable(current_page) and not callable(next_page):
+            return True
+
+    def _checked_call(self, func: callable, current_page: callable,
+                      next_page: callable, retry=3):
+        for _ in range(retry):
+            func()
+            if self._page_changed(current_page, next_page):
+                return True
+        return False
 
     def touch(self, x: Union[int, float] = None, y: Union[int, float] = None, z: Union[int, float] = None,
               speed: Union[int, float] = None, raw=False, lift=True, delay=0,
+              current_page: callable = None,
+              next_page: callable = None,
+              retry: int = 3,
               **kwargs):
         """
-
+        点击某个坐标
+        可以利用当前页以及下一页的检测函数判断是否已经成功点击. 如果current_page()返回False或者next_page()返回True,则退出
         :param x: (0-1) 百分比, > 1 实际像素
         :param y: (0-1) 百分比, > 1 实际像素
         :param z: z高度. 除非知道如何使用 否则不建议使用
         :param speed: 移动速度
         :param raw: 用mm尺寸. 除非知道如何使用 否则不建议使用
         :param lift: 是否抬起
         :param delay: 抬起延迟
+        :param next_page: 检查是否已经切换到下个页面
+        :param current_page: 检查是否已经离开到当前页面
+        :param retry: 页面无变化重试次数
         :param kwargs:
         :return:
         """
-        return self.robot.call_func(self.position, 'self/touch', x=x, y=y, z=z, speed=speed, raw=raw, lift=lift,
-                                    delay=delay, **kwargs)
+        return self._checked_call(
+            lambda: self.robot.call_func(self.position, 'self/touch', x=x, y=y, z=z, speed=speed, raw=raw, lift=lift,
+                                         delay=delay, **kwargs),
+            current_page=current_page, next_page=next_page, retry=retry
+        )
 
     def drag(self, x1: Union[int, float] = None, y1: Union[int, float] = None, x2: Union[int, float] = None,
-             y2: Union[int, float] = None, speed=55000, lift=True, raw=False, precise=False, delay=0.1):
+             y2: Union[int, float] = None, speed=55000, lift=True, raw=False, precise=False, delay=0.1,
+             current_page: callable = None,
+             next_page: callable = None,
+             retry: int = 3,
+             ):
         """
 
         :param x1: 起始X (0-1) 百分比, > 1 实际像素
         :param y1: 起始Y (0-1) 百分比, > 1 实际像素
         :param x2: 结束X (0-1) 百分比, > 1 实际像素
         :param y2: 结束Y (0-1) 百分比, > 1 实际像素
         :param speed: 移动速度
         :param lift: 是否抬起
         :param raw: 用mm尺寸. 除非知道如何使用 否则不建议使用
         :param precise: 精确还是不精确. 不精确: 会模拟真实滑屏时的加速抬起
         :param delay: 抬起延迟
+        :param next_page: 检查是否已经切换到下个页面
+        :param current_page: 检查是否已经离开到当前页面
+        :param retry: 页面无变化重试次数
         :return:
         """
-        return self.robot.call_func(self.position, 'self/drag', x1=x1, y1=y1, x2=x2, y2=y2, speed=speed, lift=lift,
-                                    raw=raw, precise=precise, delay=delay)
+
+        return self._checked_call(
+            lambda: self.robot.call_func(
+                self.position, 'self/drag', x1=x1, y1=y1, x2=x2, y2=y2, speed=speed, lift=lift,
+                raw=raw, precise=precise, delay=delay
+            ),
+            current_page=current_page, next_page=next_page, retry=retry
+        )
 
     def swipe_up(self):
         """
         模拟人手随机向上滑屏
         :return:
         """
         return self.robot.call_func(self.position, 'self/swipe-up')
@@ -632,34 +685,44 @@
 
     def touch_text(self, text: Union[str, re.Pattern],
                    index=0,
                    location: Union[
                        ImgLocation, list[ImgLocation],
                        ImgArea, list[ImgArea]] = ImgLocation.FULL,
                    contain=True,
-                   offset: tuple[float, float] = (0.0, 0.0), jitter_x=True):
+                   offset: tuple[float, float] = (0.0, 0.0), jitter_x=True,
+                   current_page: callable = None,
+                   next_page: callable = None,
+                   retry: int = 3,
+                   ):
         """
         点击屏幕里的文字
         :param text: 需要点击的文字或者regex
         :param index: 点击第几个匹配的文字 默认第一个
         :param location: ImgLocation 或者 ImgArea, 可以多个组合去匹配想要匹配的区域
         :param contain: 包含还是完全匹配
         :param offset: 偏移, 比如想点击文字左边的按钮可以用 (-0.05, 0) UI界面鼠标放在手机屏幕上可以看比例. 原点是左上角, 向下Y+, 向右x+
         :param jitter_x: 是否左右随机一点
-        :return:
-        """
-        return self.robot.call_func(
-            self.position,
-            'self/touch_text',
-            text=str(text),
-            index=index,
-            location=location,
-            contain=contain,
-            offset=list(offset),
-            jitter_x=jitter_x
+        :param next_page: 检查是否已经切换到下个页面
+        :param current_page: 检查是否已经离开到当前页面
+        :param retry: 页面无变化重试次数
+        :return:
+        """
+        return self._checked_call(
+            lambda: self.robot.call_func(
+                self.position,
+                'self/touch_text',
+                text=str(text),
+                index=index,
+                location=location,
+                contain=contain,
+                offset=list(offset),
+                jitter_x=jitter_x
+            ),
+            current_page=current_page, next_page=next_page, retry=retry
         )
 
     def move(self, x: Union[int, float] = None, y: Union[int, float] = None, z: Union[int, float] = None,
              speed: Union[int, float] = None, raw=False):
         """
 
         :param x: X (0-1) 百分比, > 1 实际像素
```

### Comparing `realtouch-0.1.6/setup.py` & `realtouch-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="realtouch",
-    version="0.1.6",
+    version="0.1.7",
     author="realTouch Dev",
     author_email="contact@realtouch.dev",
     description="realTouch Robot SDK",
     long_description="realTouch Robot SDK",
     long_description_content_type="text/markdown",
     url="https://realtouch.dev",
     packages=find_packages(),
```

