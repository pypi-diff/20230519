# Comparing `tmp/nonebot_plugin_stockhelper-0.1.1.tar.gz` & `tmp/nonebot_plugin_stockhelper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stockhelper-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_stockhelper-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_stockhelper-0.1.1.tar` & `nonebot_plugin_stockhelper-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7153 2023-05-19 04:51:37.724827 nonebot_plugin_stockhelper-0.1.1/nonebot_plugin_stockhelper/__init__.py
--rw-r--r--   0        0        0      423 2023-05-19 05:28:12.728661 nonebot_plugin_stockhelper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      389 2023-05-19 05:26:37.359982 nonebot_plugin_stockhelper-0.1.1/README.md
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 nonebot_plugin_stockhelper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7179 2023-05-19 10:16:17.055980 nonebot_plugin_stockhelper-0.1.2/nonebot_plugin_stockhelper/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-19 10:17:19.187580 nonebot_plugin_stockhelper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-05-19 05:26:37.359982 nonebot_plugin_stockhelper-0.1.2/README.md
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 nonebot_plugin_stockhelper-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_stockhelper-0.1.1/nonebot_plugin_stockhelper/__init__.py` & `nonebot_plugin_stockhelper-0.1.2/nonebot_plugin_stockhelper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 __usage__ = "给机器人发送'看 股票名'即可看股票实时估值,发送'关注'或'监控'或'jk'可令机器人为你持续关注某一股票。监控功能后面还能加上 通知波幅阈值，此值默认0.3，监控时后面不跟数字即为此值。若股票距离上次的涨跌幅超过该值，机器人会通知你。例：'关注 贵州茅台 0.5'，'监控 贵州茅台'，'监控 600519 0.7'。支持部分基金、全球股市。"
 __help__plugin_name__ = "看盘小助手"
 
 is_doing = {}
 flag = set()
 
-
+#
 def is_num(s):  # 判断是否为数字
     # 去除字符串两边的空格
     s = s.strip()
     flag = True
     # 判断是否是整数
     intRet = re.match("^[0-9]+$", s)
     # 判断是否是小数
@@ -37,16 +37,16 @@
             return flag
     else:
         flag = False
         return flag
     return flag
 
 
-gpjk = on_regex(r'^(监控|关注|jk)', priority=10, rule=to_me())
-show = on_regex(r'^(看股票|kgp)', priority=10, rule=to_me())
+gpjk = on_command('监控', aliases={'关注', 'jk'}, priority=10, rule=to_me())
+show = on_command('看股票', aliases={'kgp'}, priority=10, rule=to_me())
 stop = on_command("stop", priority=10, rule=to_me())
 clear = on_command("清空", permission=SUPERUSER)
 
 
 @clear.handle()
 async def clear_handler(bot: Bot, event: Event):
     is_doing = {}
```

### Comparing `nonebot_plugin_stockhelper-0.1.1/PKG-INFO` & `nonebot_plugin_stockhelper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-stockhelper
-Version: 0.1.1
+Version: 0.1.2
 Summary: 股票看盘助手
 Author: lcy
 Author-email: 863109569@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

