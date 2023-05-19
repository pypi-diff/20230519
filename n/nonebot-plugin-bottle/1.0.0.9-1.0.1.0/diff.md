# Comparing `tmp/nonebot_plugin_bottle-1.0.0.9.tar.gz` & `tmp/nonebot_plugin_bottle-1.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bottle-1.0.0.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_bottle-1.0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_bottle-1.0.0.9.tar` & `nonebot_plugin_bottle-1.0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7698 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/README.md
--rw-r--r--   0        0        0    19605 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/__init__.py
--rw-r--r--   0        0        0      636 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/config.py
--rw-r--r--   0        0        0    18547 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/data_source.py
--rw-r--r--   0        0        0     2647 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-r--r--   0        0        0     1426 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/model.py
--rw-r--r--   0        0        0      625 2023-05-18 13:29:46.533675 nonebot_plugin_bottle-1.0.0.9/pyproject.toml
--rw-r--r--   0        0        0     8461 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     7814 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/README.md
+-rw-r--r--   0        0        0    20745 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/config.py
+-rw-r--r--   0        0        0    18547 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/data_source.py
+-rw-r--r--   0        0        0     2647 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-r--r--   0        0        0     1426 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/model.py
+-rw-r--r--   0        0        0      625 2023-05-19 08:13:23.302371 nonebot_plugin_bottle-1.0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8577 1970-01-01 00:00:00.000000 nonebot_plugin_bottle-1.0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_bottle-1.0.0.9/README.md` & `nonebot_plugin_bottle-1.0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * 功能须知
     - 所有用户：
         - `扔漂流瓶`指令无字数限制，如需要可在代码中修改,**单扔一张图片也应加上指令后的空格**
         - `捡漂流瓶`若捡到的漂流瓶存在回复，则会显示最近三条(默认)，使用`查看漂流瓶`查看所有回复
         - `查看漂流瓶`为保证随机性，无评论时不展示漂流瓶内容，可在代码中修改。漂流瓶的发送者可以通过本指令查看内容，无论有无评论。
         - `评论漂流瓶`若机器人有被回复人好友，会发送被回复通知
         - `举报漂流瓶`五次(默认)后将自动删除，举报成功后会私聊SUPERUSER漂流瓶详情内容
-        - `删除漂流瓶`可以删除自己扔出的漂流瓶
+        - `删除漂流瓶`漂流瓶发送者可以删除自己扔出的漂流瓶。二次确认会触发删除操作的指令为：`是/Y/Yes/y/yes`。其他的均取消操作。
     - SUPERUSER:
         - `删除漂流瓶`可以删除任何一个漂流瓶
         - `清空漂流瓶`无确认过程，使用需谨慎
         - `恢复漂流瓶`可以恢复被删除的漂流瓶
         - `删除漂流瓶评论`是删除该发送者在该瓶的所有评论
         - `漂流瓶详情`将会发送漂流瓶发送者的QQ号和群号，所有回复人的QQ号
         - `漂流瓶黑名单`中`举报`选项是指`举报漂流瓶`的使用权限
```

### Comparing `nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/__init__.py` & `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import random
 import asyncio
 
+from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot import require, on_command
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
-from nonebot.params import Depends, CommandArg
+from nonebot.params import Depends, CommandArg, ArgStr
 
 require("nonebot_plugin_datastore")
 from nonebot_plugin_datastore import get_session
 from sqlalchemy.ext.asyncio.session import AsyncSession
 from nonebot.adapters.onebot.v11 import (
     GROUP,
     Bot,
@@ -399,32 +400,58 @@
         f"来自【{group_name}】的 {user_name} 的第{index}号漂流瓶：\n"
         + deserialize_message(bottle.content)
         + f"\n★前 {len(comments)} 条评论★\n{comment_str}\n【被捡到{bottle.picked}次，于{bottle.time.strftime('%Y-%m-%d %H:%M:%S')}扔出】"
     )
 
 
 @remove.handle()
-async def rem(
+async def _(
     bot: Bot,
     matcher: Matcher,
     event: GroupMessageEvent,
+    state: T_State,
     arg: Message = CommandArg(),
     session: AsyncSession = Depends(get_session),
 ):
     index = arg.extract_plain_text().strip()
     bottle = await get_bottle(index=index, matcher=matcher, session=session)
-    if (
-        str(event.user_id) in list(bot.config.superusers)
-        or bottle.user_id == event.user_id
-    ):
+    if str(event.user_id) in bot.config.superusers or bottle.user_id == event.user_id:
+        message_parts = deserialize_message(bottle.content)
+        content_preview = ""
+        for part in message_parts:
+            if part.type == "text":
+                # 文字截取
+                text = part.data["text"]
+                content_preview += text[:20] + "..." if len(text) > 20 else text
+            elif part.type == "image":
+                # 图片处理
+                content_preview += "[图片]"
+        state["index"] = index
+        state["session"] = session
+        state["matcher"] = matcher
+        await remove.send(f"你是否要删除漂流瓶（Y/N）？漂流瓶将会永久失去。（真的很久！）\n漂流瓶内容：{content_preview}")
+    else:
+        await remove.finish("删除失败！你没有相关的权限！")
+
+
+proceed = ["是", "Y", "Yes", "y", "yes"]
+
+
+@remove.got("prompt")
+async def _(state: T_State, conf: str = ArgStr("prompt")):
+    if conf in proceed:
+        index = state["index"]
+        matcher = state["matcher"]
+        session = state["session"]
+        bottle = await get_bottle(index=index, matcher=matcher, session=session)
         bottle.is_del = True
         await session.commit()
-        await remove.finish(f"成功删除 {index} 号漂流瓶！")
+        await remove.send(f"成功删除 {index} 号漂流瓶！")
     else:
-        await remove.finish("删除失败！你没有相关的权限！")
+        await remove.finish("取消删除操作。")
 
 
 ###### SUPERUSER命令 ######
 
 
 @resume.handle()
 async def _(
```

### Comparing `nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/config.py` & `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/data_source.py` & `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py` & `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/migrations/449e066410fd_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.9/nonebot_plugin_bottle/model.py` & `nonebot_plugin_bottle-1.0.1.0/nonebot_plugin_bottle/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bottle-1.0.0.9/pyproject.toml` & `nonebot_plugin_bottle-1.0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bottle"
-version = "1.0.0.9"
+version = "1.0.1.0"
 description = "Bottle post plugin in Nonebot"
 authors = ["Todysheep <todysheep@163.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Todysheep/nonebot_plugin_bottle"
 repository = "https://github.com/Todysheep/nonebot_plugin_bottle"
```

### Comparing `nonebot_plugin_bottle-1.0.0.9/PKG-INFO` & `nonebot_plugin_bottle-1.0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0.9
+Version: 1.0.1.0
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 License: GNU GPLv3
 Author: Todysheep
 Author-email: todysheep@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -46,15 +46,15 @@
 * 功能须知
     - 所有用户：
         - `扔漂流瓶`指令无字数限制，如需要可在代码中修改,**单扔一张图片也应加上指令后的空格**
         - `捡漂流瓶`若捡到的漂流瓶存在回复，则会显示最近三条(默认)，使用`查看漂流瓶`查看所有回复
         - `查看漂流瓶`为保证随机性，无评论时不展示漂流瓶内容，可在代码中修改。漂流瓶的发送者可以通过本指令查看内容，无论有无评论。
         - `评论漂流瓶`若机器人有被回复人好友，会发送被回复通知
         - `举报漂流瓶`五次(默认)后将自动删除，举报成功后会私聊SUPERUSER漂流瓶详情内容
-        - `删除漂流瓶`可以删除自己扔出的漂流瓶
+        - `删除漂流瓶`漂流瓶发送者可以删除自己扔出的漂流瓶。二次确认会触发删除操作的指令为：`是/Y/Yes/y/yes`。其他的均取消操作。
     - SUPERUSER:
         - `删除漂流瓶`可以删除任何一个漂流瓶
         - `清空漂流瓶`无确认过程，使用需谨慎
         - `恢复漂流瓶`可以恢复被删除的漂流瓶
         - `删除漂流瓶评论`是删除该发送者在该瓶的所有评论
         - `漂流瓶详情`将会发送漂流瓶发送者的QQ号和群号，所有回复人的QQ号
         - `漂流瓶黑名单`中`举报`选项是指`举报漂流瓶`的使用权限
```

