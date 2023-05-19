# Comparing `tmp/nonebot_plugin_stockhelper-0.1.0.tar.gz` & `tmp/nonebot_plugin_stockhelper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stockhelper-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_stockhelper-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_stockhelper-0.1.0.tar` & `nonebot_plugin_stockhelper-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7147 2023-05-19 03:26:24.685769 nonebot_plugin_stockhelper-0.1.0/nonebot_plugin_stockhelper/__init__.py
--rw-r--r--   0        0        0      423 2023-05-19 03:45:00.014691 nonebot_plugin_stockhelper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      389 2023-05-19 03:59:56.853561 nonebot_plugin_stockhelper-0.1.0/README.md
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 nonebot_plugin_stockhelper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7153 2023-05-19 04:51:37.724827 nonebot_plugin_stockhelper-0.1.1/nonebot_plugin_stockhelper/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-19 05:28:12.728661 nonebot_plugin_stockhelper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-05-19 05:26:37.359982 nonebot_plugin_stockhelper-0.1.1/README.md
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 nonebot_plugin_stockhelper-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_stockhelper-0.1.0/nonebot_plugin_stockhelper/__init__.py` & `nonebot_plugin_stockhelper-0.1.1/nonebot_plugin_stockhelper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from nonebot.plugin import on_command,on_regex
+from nonebot.plugin import on_command,on_regex,on_command
 from nonebot.adapters.onebot.v11 import Bot, Event
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.rule import to_me
 from nonebot.permission import SUPERUSER
 import asyncio
 import efinance as ef
 import time
@@ -39,16 +39,16 @@
         flag = False
         return flag
     return flag
 
 
 gpjk = on_regex(r'^(监控|关注|jk)', priority=10, rule=to_me())
 show = on_regex(r'^(看股票|kgp)', priority=10, rule=to_me())
-stop = on_regex(r'^(stop)$', priority=10, rule=to_me())
-clear = on_regex("^(清空)$", permission=SUPERUSER)
+stop = on_command("stop", priority=10, rule=to_me())
+clear = on_command("清空", permission=SUPERUSER)
 
 
 @clear.handle()
 async def clear_handler(bot: Bot, event: Event):
     is_doing = {}
     flag = set()
     await clear.finish("清空股票功能成功")
```

### Comparing `nonebot_plugin_stockhelper-0.1.0/PKG-INFO` & `nonebot_plugin_stockhelper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-stockhelper
-Version: 0.1.0
+Version: 0.1.1
 Summary: 股票看盘助手
 Author: lcy
 Author-email: 863109569@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

