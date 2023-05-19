# Comparing `tmp/nonebot_plugin_imgexploration-0.2.3.tar.gz` & `tmp/nonebot_plugin_imgexploration-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_imgexploration-0.2.3.tar", last modified: Mon Feb 13 13:03:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_imgexploration-0.2.4.tar", last modified: Mon Feb 13 13:33:37 2023, max compression
```

## Comparing `nonebot_plugin_imgexploration-0.2.3.tar` & `nonebot_plugin_imgexploration-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 13:03:04.277815 nonebot_plugin_imgexploration-0.2.3/
--rw-rw-rw-   0        0        0     1088 2022-12-26 13:04:44.000000 nonebot_plugin_imgexploration-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      166 2022-12-26 13:05:40.000000 nonebot_plugin_imgexploration-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2620 2023-02-13 13:03:04.276818 nonebot_plugin_imgexploration-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1914 2023-02-01 08:25:58.000000 nonebot_plugin_imgexploration-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 13:03:04.269836 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration/
--rw-rw-rw-   0        0        0     4019 2023-02-13 13:01:44.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration/__init__.py
--rw-rw-rw-   0        0        0    19661 2023-02-13 13:01:44.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration/imgexploration.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:03:04.275821 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/
--rw-rw-rw-   0        0        0     2620 2023-02-13 13:03:04.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-02-13 13:03:04.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 13:03:04.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-02-13 13:03:04.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-02-13 13:03:04.000000 nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      491 2023-02-13 13:02:51.000000 nonebot_plugin_imgexploration-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-13 13:03:04.277815 nonebot_plugin_imgexploration-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1911 2023-02-13 13:02:48.000000 nonebot_plugin_imgexploration-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-13 13:33:37.029155 nonebot_plugin_imgexploration-0.2.4/
+-rw-rw-rw-   0        0        0     1088 2022-12-26 13:04:44.000000 nonebot_plugin_imgexploration-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      166 2022-12-26 13:05:40.000000 nonebot_plugin_imgexploration-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2656 2023-02-13 13:33:37.028052 nonebot_plugin_imgexploration-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1950 2023-02-13 13:33:13.000000 nonebot_plugin_imgexploration-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-02-13 13:33:36.995538 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/
+-rw-rw-rw-   0        0        0     4082 2023-02-13 13:28:02.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/__init__.py
+-rw-rw-rw-   0        0        0    19661 2023-02-13 13:13:35.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/imgexploration.py
+drwxrwxrwx   0        0        0        0 2023-02-13 13:33:37.027055 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/
+-rw-rw-rw-   0        0        0     2656 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-02-13 13:33:36.000000 nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      491 2023-02-13 13:33:30.000000 nonebot_plugin_imgexploration-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-13 13:33:37.029155 nonebot_plugin_imgexploration-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2023-02-13 13:33:27.000000 nonebot_plugin_imgexploration-0.2.4/setup.py
```

### Comparing `nonebot_plugin_imgexploration-0.2.3/LICENSE.txt` & `nonebot_plugin_imgexploration-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imgexploration-0.2.3/PKG-INFO` & `nonebot_plugin_imgexploration-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_imgexploration
-Version: 0.2.3
+Version: 0.2.4
 Summary: Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: 554950835@qq.com
 Keywords: ssh linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -64,16 +64,18 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号
+proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+
 saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+
 SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_imgexploration Version: 0.2.3
+Metadata-Version: 2.1 Name: nonebot_plugin_imgexploration Version: 0.2.4
 Summary: GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: 554950835@qq.com Keywords: ssh linux Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -18,15 +18,16 @@
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å· saucenao_apikey=xxxxx #saucenao apikey
-å¨https://saucenao.com/user.php?page=search-apiæ³¨åè·å
-SESSION_EXPIRE_TIMEOUT=180 #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://
-v2.nonebot.dev/docs/api/config#Config-session_expire_timeout ``` ##
-ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
+saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
+user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
+#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
+config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
+æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

### Comparing `nonebot_plugin_imgexploration-0.2.3/README.md` & `nonebot_plugin_imgexploration-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,18 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号
+proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+
 saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+
 SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å· saucenao_apikey=xxxxx #saucenao apikey
-å¨https://saucenao.com/user.php?page=search-apiæ³¨åè·å
-SESSION_EXPIRE_TIMEOUT=180 #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://
-v2.nonebot.dev/docs/api/config#Config-session_expire_timeout ``` ##
-ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
+saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
+user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
+#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
+config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
+æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

### Comparing `nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration/__init__.py` & `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from nonebot.params import Arg, CommandArg
 from nonebot.adapters.onebot.v11 import Bot, Message, MessageSegment, GroupMessageEvent, PrivateMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from .imgexploration import Imgexploration
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(name="查找图片出处", description="通过saucenao、ascii2d、Google、Yandx查询图片出处", usage="command:搜图")
-proxy_port = getattr(nonebot.get_driver().config, "proxy_port", int)
-saucenao_apikey = getattr(nonebot.get_driver().config, "saucenao_apikey", str)
+
+proxy_port = getattr(nonebot.get_driver().config, "proxy_port", None)
+saucenao_apikey = getattr(nonebot.get_driver().config, "saucenao_apikey", "a778025bd4644780c9edd82970484548786fb583")
+
+proxies = f"http://127.0.0.1:{proxy_port}" if proxy_port else None
 
 
 def numspilt(args: str, max: int):
     args_list = list(args.split())
     r_li = []
     for arg in args_list:
         if arg.isnumeric() and 1 <= int(arg) <= max:
@@ -39,16 +42,16 @@
 
 @imgexploration.got("Message_pic", prompt="请发送要搜索的图片")
 async def get_pic(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent, GuildMessageEvent], state: T_State, msgpic: Message = Arg("Message_pic")):
     for segment in msgpic:
         if segment.type == "image":
             pic_url: str = segment.data["url"]  # 图片链接
             logger.success(f"获取到图片: {pic_url}")
-            async with httpx.AsyncClient(proxies=f"http://127.0.0.1:{proxy_port}") as client:
-                search = Imgexploration(pic_url=pic_url, client=client,proxy=f"http://127.0.0.1:{proxy_port}", saucenao_apikey=saucenao_apikey)
+            async with httpx.AsyncClient(proxies=proxies) as client:
+                search = Imgexploration(pic_url=pic_url, client=client, proxy=proxies, saucenao_apikey=saucenao_apikey)
                 await imgexploration.send(message=Message(MessageSegment.text("搜索进行中……")), reply_message=True)
                 await search.doSearch()
             result_dict = search.getResultDict()
             state["result_dict"] = result_dict
             await imgexploration.send(
                 message=Message(
                     MessageSegment.image(file=result_dict["pic"]) + MessageSegment.text("请在180s内发送序号以获得对应结果的链接，一次可以发送多个序号，例如：1 5 6"),
```

### Comparing `nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration/imgexploration.py` & `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration/imgexploration.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imgexploration-0.2.3/nonebot_plugin_imgexploration.egg-info/PKG-INFO` & `nonebot_plugin_imgexploration-0.2.4/nonebot_plugin_imgexploration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-imgexploration
-Version: 0.2.3
+Version: 0.2.4
 Summary: Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图
 Home-page: https://github.com/cpuopt/nonebot_plugin_imgexploration
 Author: cpufan
 Author-email: 554950835@qq.com
 Keywords: ssh linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -64,16 +64,18 @@
 nonebot.load_plugin('nonebot_plugin_guild_patch')
 ```
 </details>
 
 ## 二.**配置**  
 ### 1.env中的配置
 ```
-proxy_port=xxxx  #代理端口号
+proxy_port=xxxx  #代理端口号(不使用本地代理可缺省)
+
 saucenao_apikey=xxxxx  #saucenao apikey 在https://saucenao.com/user.php?page=search-api注册获取
+
 SESSION_EXPIRE_TIMEOUT=180 #等待用户回复的超时时间(可选) https://v2.nonebot.dev/docs/api/config#Config-session_expire_timeout
 ```  
 ## 三.**使用**  
 ### 
 ```
 /搜图
 /搜图 <图片>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.2.3
+Metadata-Version: 2.1 Name: nonebot-plugin-imgexploration Version: 0.2.4
 Summary: GoogleãYandxååºäºPicImageSearchçsaucenaoãascii2dæå¾ Home-
 page: https://github.com/cpuopt/nonebot_plugin_imgexploration Author: cpufan
 Author-email: 554950835@qq.com Keywords: ssh linux Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -18,15 +18,16 @@
 HarmonyOS_Sans_SC_Light.ttf ``` https://developer.harmonyos.com/cn/docs/design/
 des-guides/font-0000001157868583 å®è£å°ç³»ç»å­ä½å³å¯ ### 3.ä¾èµ (nb-
 cliæpipå®è£æ ééç½®ä¾èµ)  å±å¼/æ¶èµ· ``` pip install -
 r requirements.txt ``` go-cqhttp é¢éæ¯æééè¡¥ä¸`nonebot-plugin-guild-
 patch` ``` pip install nonebot-plugin-guild-patch ```
 å¨å è½½æ¬æä»¶åæ·»å  ``` nonebot.load_plugin
 ('nonebot_plugin_guild_patch') ```  ## äº.**éç½®** ### 1.envä¸­çéç½® ```
-proxy_port=xxxx #ä»£çç«¯å£å· saucenao_apikey=xxxxx #saucenao apikey
-å¨https://saucenao.com/user.php?page=search-apiæ³¨åè·å
-SESSION_EXPIRE_TIMEOUT=180 #ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://
-v2.nonebot.dev/docs/api/config#Config-session_expire_timeout ``` ##
-ä¸.**ä½¿ç¨** ### ``` /æå¾ /æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
+proxy_port=xxxx #ä»£çç«¯å£å·(ä¸ä½¿ç¨æ¬å°ä»£çå¯ç¼ºç)
+saucenao_apikey=xxxxx #saucenao apikey å¨https://saucenao.com/
+user.php?page=search-apiæ³¨åè·å SESSION_EXPIRE_TIMEOUT=180
+#ç­å¾ç¨æ·åå¤çè¶æ¶æ¶é´(å¯é) https://v2.nonebot.dev/docs/api/
+config#Config-session_expire_timeout ``` ## ä¸.**ä½¿ç¨** ### ``` /æå¾ /
+æå¾ <å¾ç> ``` ### **ä½¿ç¨ç¤ºä¾**
                [https://p.inari.site/usr/369/63b6cfe0cd8a8.jpg]
 ### æå¾ç»æ
                [https://p.inari.site/usr/369/63b6cd6f24abc.jpg]
```

### Comparing `nonebot_plugin_imgexploration-0.2.3/setup.py` & `nonebot_plugin_imgexploration-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = fd.read()
 
 
 setuptools.setup(
 
     name="nonebot_plugin_imgexploration",
 
-    version="0.2.3",
+    version="0.2.4",
 
     description="Google、Yandx和基于PicImageSearch的saucenao、ascii2d搜图",
 
     long_description=long_description,
 
     long_description_content_type="text/markdown",
```

