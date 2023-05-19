# Comparing `tmp/cqbot-0.0.6.tar.gz` & `tmp/cqbot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqbot-0.0.6.tar", last modified: Mon Apr 17 23:19:09 2023, max compression
+gzip compressed data, was "cqbot-0.0.7.tar", last modified: Fri May 19 16:07:11 2023, max compression
```

## Comparing `cqbot-0.0.6.tar` & `cqbot-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 23:19:09.710440 cqbot-0.0.6/
--rw-r--r--   0 yu         (501) staff       (20)     1063 2023-02-16 14:05:37.000000 cqbot-0.0.6/LICENSE
--rw-r--r--   0 yu         (501) staff       (20)     7950 2023-04-17 23:19:09.710103 cqbot-0.0.6/PKG-INFO
--rw-r--r--   0 yu         (501) staff       (20)     7571 2023-02-19 08:09:32.000000 cqbot-0.0.6/README.md
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 23:19:09.706907 cqbot-0.0.6/cqbot/
--rw-r--r--   0 yu         (501) staff       (20)      119 2023-02-19 07:23:57.000000 cqbot-0.0.6/cqbot/__init__.py
--rw-r--r--   0 yu         (501) staff       (20)    37544 2023-02-19 07:23:57.000000 cqbot-0.0.6/cqbot/action.py
--rw-r--r--   0 yu         (501) staff       (20)     9200 2023-04-17 23:19:07.000000 cqbot-0.0.6/cqbot/bot.py
--rw-r--r--   0 yu         (501) staff       (20)     2451 2023-04-17 22:45:36.000000 cqbot-0.0.6/cqbot/cmd.py
--rw-r--r--   0 yu         (501) staff       (20)    12592 2023-04-17 22:47:40.000000 cqbot-0.0.6/cqbot/cq.py
--rw-r--r--   0 yu         (501) staff       (20)     4323 2023-02-19 07:23:57.000000 cqbot-0.0.6/cqbot/enum.py
--rw-r--r--   0 yu         (501) staff       (20)    19764 2023-02-19 07:23:57.000000 cqbot-0.0.6/cqbot/event.py
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 23:19:09.709627 cqbot-0.0.6/cqbot.egg-info/
--rw-r--r--   0 yu         (501) staff       (20)     7950 2023-04-17 23:19:09.000000 cqbot-0.0.6/cqbot.egg-info/PKG-INFO
--rw-r--r--   0 yu         (501) staff       (20)      271 2023-04-17 23:19:09.000000 cqbot-0.0.6/cqbot.egg-info/SOURCES.txt
--rw-r--r--   0 yu         (501) staff       (20)        1 2023-04-17 23:19:09.000000 cqbot-0.0.6/cqbot.egg-info/dependency_links.txt
--rw-r--r--   0 yu         (501) staff       (20)       33 2023-04-17 23:19:09.000000 cqbot-0.0.6/cqbot.egg-info/requires.txt
--rw-r--r--   0 yu         (501) staff       (20)        6 2023-04-17 23:19:09.000000 cqbot-0.0.6/cqbot.egg-info/top_level.txt
--rw-r--r--   0 yu         (501) staff       (20)       38 2023-04-17 23:19:09.710562 cqbot-0.0.6/setup.cfg
--rw-r--r--   0 yu         (501) staff       (20)      847 2023-04-17 23:19:06.000000 cqbot-0.0.6/setup.py
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-05-19 16:07:11.849666 cqbot-0.0.7/
+-rw-r--r--   0 yu         (501) staff       (20)     1063 2023-02-16 14:05:37.000000 cqbot-0.0.7/LICENSE
+-rw-r--r--   0 yu         (501) staff       (20)     7950 2023-05-19 16:07:11.849198 cqbot-0.0.7/PKG-INFO
+-rw-r--r--   0 yu         (501) staff       (20)     7571 2023-02-19 08:09:32.000000 cqbot-0.0.7/README.md
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-05-19 16:07:11.843611 cqbot-0.0.7/cqbot/
+-rw-r--r--   0 yu         (501) staff       (20)      119 2023-02-19 07:23:57.000000 cqbot-0.0.7/cqbot/__init__.py
+-rw-r--r--   0 yu         (501) staff       (20)    37544 2023-02-19 07:23:57.000000 cqbot-0.0.7/cqbot/action.py
+-rw-r--r--   0 yu         (501) staff       (20)     9356 2023-05-19 16:07:08.000000 cqbot-0.0.7/cqbot/bot.py
+-rw-r--r--   0 yu         (501) staff       (20)     2451 2023-04-17 22:45:36.000000 cqbot-0.0.7/cqbot/cmd.py
+-rw-r--r--   0 yu         (501) staff       (20)    12592 2023-04-17 22:47:40.000000 cqbot-0.0.7/cqbot/cq.py
+-rw-r--r--   0 yu         (501) staff       (20)     4323 2023-02-19 07:23:57.000000 cqbot-0.0.7/cqbot/enum.py
+-rw-r--r--   0 yu         (501) staff       (20)    19764 2023-02-19 07:23:57.000000 cqbot-0.0.7/cqbot/event.py
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-05-19 16:07:11.848387 cqbot-0.0.7/cqbot.egg-info/
+-rw-r--r--   0 yu         (501) staff       (20)     7950 2023-05-19 16:07:11.000000 cqbot-0.0.7/cqbot.egg-info/PKG-INFO
+-rw-r--r--   0 yu         (501) staff       (20)      271 2023-05-19 16:07:11.000000 cqbot-0.0.7/cqbot.egg-info/SOURCES.txt
+-rw-r--r--   0 yu         (501) staff       (20)        1 2023-05-19 16:07:11.000000 cqbot-0.0.7/cqbot.egg-info/dependency_links.txt
+-rw-r--r--   0 yu         (501) staff       (20)       33 2023-05-19 16:07:11.000000 cqbot-0.0.7/cqbot.egg-info/requires.txt
+-rw-r--r--   0 yu         (501) staff       (20)        6 2023-05-19 16:07:11.000000 cqbot-0.0.7/cqbot.egg-info/top_level.txt
+-rw-r--r--   0 yu         (501) staff       (20)       38 2023-05-19 16:07:11.849827 cqbot-0.0.7/setup.cfg
+-rw-r--r--   0 yu         (501) staff       (20)      847 2023-05-19 16:07:08.000000 cqbot-0.0.7/setup.py
```

### Comparing `cqbot-0.0.6/LICENSE` & `cqbot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/PKG-INFO` & `cqbot-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/lhlyu/cqbot
 Author: lhlyu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `cqbot-0.0.6/README.md` & `cqbot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot/action.py` & `cqbot-0.0.7/cqbot/action.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot/bot.py` & `cqbot-0.0.7/cqbot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,24 @@
 from .action import *
 
 CONFIG_FILE = "./config.yml"
 LOG_FORMAT = "[%(asctime)s]-[%(levelname)s]: %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
+def task(f):
+    def wrapper(*args, **kwargs):
+        thr = Thread(target=f, args=args, kwargs=kwargs)
+        thr.start()
+
+    return wrapper
+
+
 class Bot(Event):
-    version: str = '0.0.6'
+    version: str = '0.0.7'
 
     def __init__(self, loglevel: int = logging.INFO, path: str = './'):
         """
         初始化
         :param loglevel: 日志等级，默认 logging.INFO
         :param path: config.yml 和 go-cqhttp 所在目录，这两个东西必须放在一起
         """
@@ -128,15 +136,14 @@
             if shell_msg.strip() == "":
                 continue
             print(shell_msg)
             if "CQ WebSocket 服务器已启动" in shell_msg:
                 time.sleep(1)
                 self.__running = True
 
-
     def __run_ws(self):
         """
         运行websocket连接go-cqhttp
         :return:
         """
 
         def on_message(ws, msg):
@@ -202,14 +209,15 @@
             PostType.META_EVENT: {
                 'on_meta_event_heartbeat': self.on_meta_event_heartbeat,
                 'on_meta_event_lifecycle': self.on_meta_event_lifecycle,
             },
         }
         logging.info('事件初始化成功')
 
+    @task
     def __call(self, message_data: dict[str, Any]):
         """
         根据消息类型调用指定的方法
         :param message_data:
         :return:
         """
         pt = message_data.get('post_type', None)
@@ -261,8 +269,8 @@
             ev = f'on_{msg.post_type.value}_{msg.meta_event_type.value}'
             fn = events.get(ev, None)
             if fn is None:
                 return
             fn(self.__action, msg)
 
 
-__all__ = ['Bot']
+__all__ = ['Bot']
```

### Comparing `cqbot-0.0.6/cqbot/cmd.py` & `cqbot-0.0.7/cqbot/cmd.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot/cq.py` & `cqbot-0.0.7/cqbot/cq.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot/enum.py` & `cqbot-0.0.7/cqbot/enum.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot/event.py` & `cqbot-0.0.7/cqbot/event.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.6/cqbot.egg-info/PKG-INFO` & `cqbot-0.0.7/cqbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/lhlyu/cqbot
 Author: lhlyu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `cqbot-0.0.6/setup.py` & `cqbot-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cqbot",
-    version="0.0.6",
+    version="0.0.7",
     description="go-cqhttp python 框架，可以用于快速塔建 bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

