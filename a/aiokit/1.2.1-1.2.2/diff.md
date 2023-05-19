# Comparing `tmp/aiokit-1.2.1-py3-none-any.whl.zip` & `tmp/aiokit-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3930 bytes, number of entries: 7
+Zip file size: 3922 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      176 b- defN 22-Oct-25 09:23 aiokit/__init__.py
 -rw-r--r--  2.0 unx     3121 b- defN 23-May-11 22:09 aiokit/aiothing.py
--rw-r--r--  2.0 unx     4046 b- defN 22-Oct-25 09:23 aiokit/executors.py
+-rw-r--r--  2.0 unx     4077 b- defN 23-May-19 17:46 aiokit/executors.py
 -rw-r--r--  2.0 unx     1226 b- defN 22-Oct-25 09:23 aiokit/utils.py
-?rw-------  2.0 unx       91 b- defN 23-May-11 22:09 aiokit-1.2.1.dist-info/WHEEL
-?rw-------  2.0 unx      326 b- defN 23-May-11 22:09 aiokit-1.2.1.dist-info/METADATA
-?rw-------  2.0 unx      499 b- defN 23-May-11 22:09 aiokit-1.2.1.dist-info/RECORD
-7 files, 9485 bytes uncompressed, 3060 bytes compressed:  67.7%
+?rw-------  2.0 unx       91 b- defN 23-May-19 17:47 aiokit-1.2.2.dist-info/WHEEL
+?rw-------  2.0 unx      294 b- defN 23-May-19 17:47 aiokit-1.2.2.dist-info/METADATA
+?rw-------  2.0 unx      499 b- defN 23-May-19 17:47 aiokit-1.2.2.dist-info/RECORD
+7 files, 9484 bytes uncompressed, 3052 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: aiokit/executors.py
 Comment: 
 
 Filename: aiokit/utils.py
 Comment: 
 
-Filename: aiokit-1.2.1.dist-info/WHEEL
+Filename: aiokit-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: aiokit-1.2.1.dist-info/METADATA
+Filename: aiokit-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: aiokit-1.2.1.dist-info/RECORD
+Filename: aiokit-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiokit/executors.py

```diff
@@ -8,27 +8,26 @@
 from typing import (
     Callable,
     List,
     Optional,
     Union,
 )
 
-import uvloop
-
 from .aiothing import AioThing
 
 logger = logging.getLogger('aiokit.executors')
 
 
 class MultiprocessAsyncExecutor:
     def __init__(
         self,
         create_aiothing: Optional[Union[Callable[[int], AioThing], partial]] = None,
         create_aiothings: Optional[List[Union[Callable[[int], AioThing], partial]]] = None,
         shards: List = None,
+        loop_ctr=asyncio.new_event_loop
     ):
         if create_aiothing and create_aiothings:
             raise RuntimeError('`create_aiothing` and `create_aiothings` cannot be set both')
         if not create_aiothing and not create_aiothings:
             raise RuntimeError('`create_aiothing` or `create_aiothings` should be set')
         if create_aiothings and shards and len(create_aiothings) != len(shards):
             raise RuntimeError('length of `shards` and `create_aiothings` should be the same')
@@ -42,15 +41,15 @@
         self._shutting_down = False
         self.processes = []
 
         if create_aiothing:
             create_aiothings = [create_aiothing] * len(shards)
 
         for create_aiothing, shard in zip(create_aiothings, shards):
-            process = multiprocessing.Process(target=self._run_loop, args=(create_aiothing, shard,))
+            process = multiprocessing.Process(target=self._run_loop, args=(create_aiothing, shard, loop_ctr))
             process.daemon = True
             self.processes.append(process)
 
     def stop_children(self, signum):
         for process in self.processes:
             try:
                 os.kill(process.pid, signum)
@@ -100,17 +99,17 @@
                     logger.debug({
                         'action': 'all_processes_exited',
                         'mode': 'join',
                     })
                     return
             time.sleep(1.0)
 
-    def _run_loop(self, create_aiothing, shard):
+    def _run_loop(self, create_aiothing, shard, loop_ctr):
         try:
-            loop = uvloop.new_event_loop()
+            loop = loop_ctr()
             asyncio.set_event_loop(loop)
             aiothing = create_aiothing(shard)
             loop.run_until_complete(aiothing.start_and_wait())
         except asyncio.CancelledError:
             pass
         except Exception as e:
             logger.error(e)
```

