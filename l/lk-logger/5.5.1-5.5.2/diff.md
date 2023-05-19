# Comparing `tmp/lk_logger-5.5.1-py3-none-any.whl.zip` & `tmp/lk_logger-5.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 36983 bytes, number of entries: 25
+Zip file size: 36997 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 lk_logger/_print.py
 -rw-r--r--  2.0 unx     1672 b- defN 80-Jan-01 00:00 lk_logger/cache.py
 -rw-r--r--  2.0 unx     5487 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 lk_logger/control.py
 -rw-r--r--  2.0 unx     6459 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
--rw-r--r--  2.0 unx    13000 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 unx    13051 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 unx    10446 b- defN 80-Jan-01 00:00 lk_logger/markup.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 unx     9899 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
 -rw-r--r--  2.0 unx      769 b- defN 80-Jan-01 00:00 lk_logger/shunt.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     1995 b- defN 16-Jan-01 00:00 lk_logger-5.5.1.dist-info/RECORD
-25 files, 116993 bytes uncompressed, 33803 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.2.dist-info/METADATA
+?rw-r--r--  2.0 unx     1995 b- defN 16-Jan-01 00:00 lk_logger-5.5.2.dist-info/RECORD
+25 files, 117044 bytes uncompressed, 33817 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -60,17 +60,17 @@
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
 Filename: lk_logger/shunt.py
 Comment: 
 
-Filename: lk_logger-5.5.1.dist-info/WHEEL
+Filename: lk_logger-5.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.5.1.dist-info/METADATA
+Filename: lk_logger-5.5.2.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.5.1.dist-info/RECORD
+Filename: lk_logger-5.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -17,8 +17,8 @@
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.5.1'
+__version__ = '5.5.2'
```

## lk_logger/logger.py

```diff
@@ -97,14 +97,15 @@
         
         def consume() -> None:
             msg: t.Union[str, tuple]
             kwargs: dict
             custom_print: t.Optional[t.Callable]
             
             for i in range(len(self._message_queue)):
+                if not self._message_queue: break
                 msg, kwargs, custom_print = self._message_queue.popleft()
                 if custom_print:
                     # debug(custom_print, msg, kwargs)
                     kwargs.pop('file', None)
                     custom_print(*msg, **kwargs)
                 else:
                     con_print(msg, **kwargs)
```

## Comparing `lk_logger-5.5.1.dist-info/METADATA` & `lk_logger-5.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.5.1
+Version: 5.5.2
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.5.1.dist-info/RECORD` & `lk_logger-5.5.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-lk_logger/__init__.py,sha256=rNWWBbG7CjrjrIvcU6S3tWlwu8hD1LDvzjKTEo17kZM,592
+lk_logger/__init__.py,sha256=QurUBVXay6P0mgoM5M1tvAT_4KcB8yAKvJktKevHJds,592
 lk_logger/_print.py,sha256=Q0WdJ-TxOcQy1aKxEgaxaCrixq9GdXqQVF7YTw-jELo,591
 lk_logger/cache.py,sha256=ayisqijEVWmUatnNqrooM8urR0hIAzYkzcJTUt_8248,1672
 lk_logger/config.py,sha256=mmM6x2vlR5setLz_5dhWKHzwL4tvY-oESsNDl5FOLr4,5487
 lk_logger/console.py,sha256=GSoFWXBybfNuF7S7b3_OJL70h52OSlTPnCbpay1pL60,1563
 lk_logger/control.py,sha256=Fk8o5aGjTAAxhJs6G1EvTUZ3ERvlQ13H-cpX_Mn5CSQ,4503
 lk_logger/frame_info.py,sha256=tkraucs-K_hCvtp9IB8dvLkuZ8wG8kAQt0swz8b2mZQ,6459
-lk_logger/logger.py,sha256=H4zRYxiOH0ngig-BoM8MS25yZog4ZDt7Nl6IHPSCkEw,13000
+lk_logger/logger.py,sha256=NvF5IYj1Yq5lR8WPTMoxkZFhC75Ai5NK-sNX4Mp3xL0,13051
 lk_logger/markup.py,sha256=FIDjNJ-q-Fb3T2FDCjhMDwyUrkH1mdY5_nFE1bSze20,10446
 lk_logger/message_builder.py,sha256=Jj6YEmEbwjaiIXndS32vMToXBAfgHKXw3wDGdoqCCgI,6265
 lk_logger/message_formatter.py,sha256=lIdEoMdKDOfdduTq9wfKvL5Q7el9GQRMQeX4p63wu0k,9899
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
 lk_logger/pipeline.py,sha256=bo-Z9367i2TxxJOCS5_Rk_6CFccFyJYgp3-uw9q9LzQ,2559
 lk_logger/scanner/__init__.py,sha256=er6nQAKVaYpdk30878kEDo5vKTSa6CzR-CdxNJiaODo,71
 lk_logger/scanner/analyser.py,sha256=tbI48nDcBPthZoD8jlnpap7S6FIHs4u8pUMQpsmh6r4,6247
 lk_logger/scanner/const.py,sha256=pRfHUK2huF2oLkd-ZpGtGUKQ2T4K3EnlSI0pUGGnp6Q,1128
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=7Ase1WyHD87cBr4k9zYehe9LgL91r0L1_XlgKHg1_Eg,9594
 lk_logger/scanner/symbols.py,sha256=ibW1-n7Xigo9LvowUSn6dIrx-UmiJyuxN321bSCilSg,3238
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=Vr929B1w9UGiLVEMIJJIyE6gULjd_NxmNVpssyZW_JI,491
 lk_logger/shunt.py,sha256=X3wqfprKLsmSUgZifte0Ao9CB7MDh2A45IqC1Gt8f2Y,769
-lk_logger-5.5.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_logger-5.5.1.dist-info/METADATA,sha256=L2BsGbfZ3Y7Z7yfiJommeNb2iJzsvV3JIeav8BLF_KA,4884
-lk_logger-5.5.1.dist-info/RECORD,,
+lk_logger-5.5.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+lk_logger-5.5.2.dist-info/METADATA,sha256=g9Hl7zTksuqHijr3O6tXnfpFY2WH_NGgJEcWmlhlJgU,4884
+lk_logger-5.5.2.dist-info/RECORD,,
```

