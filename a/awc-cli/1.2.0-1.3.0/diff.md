# Comparing `tmp/awc_cli-1.2.0-py2.py3-none-any.whl.zip` & `tmp/awc_cli-1.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 22050 bytes, number of entries: 18
--rw-r--r--  2.0 unx      122 b- defN 23-May-09 15:46 awc_cli/__init__.py
--rw-r--r--  2.0 unx      508 b- defN 23-Apr-15 23:24 awc_cli/__main__.py
+Zip file size: 22198 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      122 b- defN 23-May-19 16:04 awc_cli/__init__.py
+-rw-r--r--  2.0 unx      562 b- defN 23-May-19 15:59 awc_cli/__main__.py
 -rw-r--r--  2.0 unx      423 b- defN 23-Apr-15 23:09 awc_cli/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 17:08 awc_cli/py.typed
 -rw-r--r--  2.0 unx     2799 b- defN 23-Apr-29 18:40 awc_cli/repl.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Apr-15 23:14 awc_cli/util.py
 -rw-r--r--  2.0 unx      490 b- defN 23-Apr-15 21:10 awc_cli/cmd/__init__.py
 -rw-r--r--  2.0 unx     4713 b- defN 23-May-09 15:45 awc_cli/cmd/admin_cmds.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Apr-15 23:23 awc_cli/cmd/cmds.py
 -rw-r--r--  2.0 unx     3326 b- defN 23-Apr-15 23:23 awc_cli/cmd/mgr.py
--rw-r--r--  2.0 unx     2532 b- defN 23-May-07 23:53 awc_cli/cmd/user_cmds.py
--rw-------  2.0 unx    35115 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1271 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.2.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1397 b- defN 23-May-09 15:51 awc_cli-1.2.0.dist-info/RECORD
-18 files, 54941 bytes uncompressed, 19778 bytes compressed:  64.0%
+-rw-r--r--  2.0 unx     2875 b- defN 23-May-19 16:03 awc_cli/cmd/user_cmds.py
+-rw-------  2.0 unx    35115 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1291 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.3.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1397 b- defN 23-May-19 16:07 awc_cli-1.3.0.dist-info/RECORD
+18 files, 55358 bytes uncompressed, 19926 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: awc_cli/cmd/mgr.py
 Comment: 
 
 Filename: awc_cli/cmd/user_cmds.py
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/LICENSE
+Filename: awc_cli-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/METADATA
+Filename: awc_cli-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/WHEEL
+Filename: awc_cli-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/entry_points.txt
+Filename: awc_cli-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/top_level.txt
+Filename: awc_cli-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/zip-safe
+Filename: awc_cli-1.3.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc_cli-1.2.0.dist-info/RECORD
+Filename: awc_cli-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc_cli/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc_cli"""
 
 from typing import Final
 
-__version__: Final[str] = "1.2.0"
+__version__: Final[str] = "1.3.0"
```

## awc_cli/__main__.py

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc cli -- main"""
 
 from warnings import filterwarnings as filter_warnings
 
 import awc
+import awc.api
 
 from .config import INSTANCE, KEY
 from .repl import repl
 
 
 def main() -> int:
     """entry / main function"""
 
-    with awc.Awc(INSTANCE, KEY) as api:
-        return repl(api)
+    with awc.Awc(INSTANCE, KEY) as awc_api:
+        awc.api.visit(awc_api)
+        return repl(awc_api)
 
 
 if __name__ == "__main__":
     assert main.__annotations__.get("return") is int, "main() should return an integer"
 
     filter_warnings("error", category=Warning)
     raise SystemExit(main())
```

## awc_cli/cmd/user_cmds.py

```diff
@@ -3,14 +3,15 @@
 """user commands"""
 
 import typing
 
 import awc
 import awc.api
 import awc.exc
+import lxml.etree as etree  # type: ignore
 
 from ..config import ADMIN_CLR
 from ..util import err
 from . import Command
 from .mgr import CommandManager
 
 USER_CMDS: typing.Final[CommandManager] = CommandManager()
@@ -112,7 +113,21 @@
 @USER_CMDS.nonempty
 def anon(api: awc.Awc, cmd: Command) -> int:
     """post an anonymous message
     usage : anon <message>"""
 
     print(awc.api.anon(api, cmd.cmd))
     return 0
+
+
+@USER_CMDS.new
+def visits(api: awc.Awc, *_: typing.Any) -> int:
+    """get visit count
+    usage : visits"""
+
+    print(
+        etree.fromstring(awc.api.visit(api))  # type: ignore
+        .xpath("//svg:text", namespaces={"svg": "http://www.w3.org/2000/svg"})[0]
+        .text
+    )
+
+    return 0
```

## Comparing `awc_cli-1.2.0.dist-info/LICENSE` & `awc_cli-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc_cli-1.2.0.dist-info/METADATA` & `awc_cli-1.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: cli for https://server.ari-web.xyz/
 Home-page: https://ari-web.xyz/gh/awc-cli
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,comments,api,https,awc
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: awc (>=3.0.0)
+Requires-Dist: awc (>=3.2.0)
 Requires-Dist: sqlparse
+Requires-Dist: lxml
 
 # awc-cli
 
 > cli for https://server.ari-web.xyz/ using https://ari-web.xyz/gh/awc
 
 # configuration
```

## Comparing `awc_cli-1.2.0.dist-info/RECORD` & `awc_cli-1.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-awc_cli/__init__.py,sha256=oanou2efHmixFXNe1rLhv0JAnz2cKJnTH-FTCc8J3f8,122
-awc_cli/__main__.py,sha256=4yHZMkIHuTIIDs61cc1graPrMLDf52djTpUrIydnBHI,508
+awc_cli/__init__.py,sha256=w4d_sTupvrYAg5k2vg7p2hGmlVFtOWQyBrbCexmXp7k,122
+awc_cli/__main__.py,sha256=fKZWuYNHAyzQy4G6vPy3AJgVnNsfjjgQ4qqU2jdldOY,562
 awc_cli/config.py,sha256=LOb3rgb14ui92pGUmnk63JEiOoTO3VOxF9xFtvzN-Ic,423
 awc_cli/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc_cli/repl.py,sha256=PXZZfqVa9x9Y6DTkIcPNqm1cKAWVQA34JMeu99LntP8,2799
 awc_cli/util.py,sha256=vxJ0DwU9Bwk87H4MfgBg7rkhMWd-aO_xskib4Uxq7To,1790
 awc_cli/cmd/__init__.py,sha256=jwBEdqk3lhwYnMuhY8Srkoo__3FYKd3q9DEv8BpEmeA,490
 awc_cli/cmd/admin_cmds.py,sha256=PcgFzZmO7eoEFmRpgJlhMrBD01y2RRd38IUtHGX0UQU,4713
 awc_cli/cmd/cmds.py,sha256=dn2mhqcABK0qrdvNNz5PRQ9F5wNXW52nia2Ju6_n9Cw,290
 awc_cli/cmd/mgr.py,sha256=FUA5hl2UqKqoR6bKYwZCJTRg6_9163Lh3n17Rol2w7E,3326
-awc_cli/cmd/user_cmds.py,sha256=fLLsZp5dwrdaf9Fi71Vxri9Rh-zrdIAWxuqvjuXYCkM,2532
-awc_cli-1.2.0.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
-awc_cli-1.2.0.dist-info/METADATA,sha256=Dy82gzRawKz4TPMXqODDC6FaLM9f5ycAicYZxU3CT_o,1271
-awc_cli-1.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc_cli-1.2.0.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
-awc_cli-1.2.0.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
-awc_cli-1.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc_cli-1.2.0.dist-info/RECORD,,
+awc_cli/cmd/user_cmds.py,sha256=Xty1ozOFhKYAmfOc2Z3GJGGzbwJs4wRWMkG9cOTkWNk,2875
+awc_cli-1.3.0.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
+awc_cli-1.3.0.dist-info/METADATA,sha256=G2fAGK9Fx8k24s8ZijmxaInfjNicIkqUHdo0VrnVGs8,1291
+awc_cli-1.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc_cli-1.3.0.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
+awc_cli-1.3.0.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
+awc_cli-1.3.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc_cli-1.3.0.dist-info/RECORD,,
```

