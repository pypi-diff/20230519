# Comparing `tmp/angeltools-0.2.8.tar.gz` & `tmp/angeltools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angeltools-0.2.8.tar", last modified: Wed May 17 08:38:33 2023, max compression
+gzip compressed data, was "angeltools-0.2.9.tar", last modified: Fri May 19 08:24:27 2023, max compression
```

## Comparing `angeltools-0.2.8.tar` & `angeltools-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.8/LICENSE
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-17 08:38:33.271493 angeltools-0.2.8/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.8/README.md
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools/
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools/Db/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.8/angeltools/Db/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3289 2022-04-21 02:57:31.000000 angeltools-0.2.8/angeltools/Db/redis_connector.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.8/angeltools/ImageTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.8/angeltools/MathTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.8/angeltools/Slavers.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    15430 2023-05-17 08:36:58.000000 angeltools-0.2.8/angeltools/StrTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.8/angeltools/TimeTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.8/angeltools/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.8/angeltools/commands.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/angeltools/fdfs/
--rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.8/angeltools/fdfs/__init__.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/angeltools/fdfs/fdfs_client/
--rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/connection.py
--rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/exceptions.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_protol.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_test.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/storage_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/tracker_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/utils.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_operator.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools.egg-info/
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/SOURCES.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/dependency_links.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/entry_points.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.8/angeltools.egg-info/not-zip-safe
--rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/requires.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/top_level.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-17 08:38:33.271493 angeltools-0.2.8/setup.cfg
--rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-17 08:38:28.000000 angeltools-0.2.8/setup.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.9/LICENSE
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-19 08:24:27.987460 angeltools-0.2.9/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.9/README.md
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.983460 angeltools-0.2.9/angeltools/
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/Db/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.9/angeltools/Db/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3297 2023-05-19 07:03:17.000000 angeltools-0.2.9/angeltools/Db/redis_connector.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.9/angeltools/ImageTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.9/angeltools/MathTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.9/angeltools/Slavers.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    15912 2023-05-19 08:23:24.000000 angeltools-0.2.9/angeltools/StrTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.9/angeltools/TimeTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.9/angeltools/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.9/angeltools/commands.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/fdfs/
+-rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.9/angeltools/fdfs/__init__.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/fdfs/fdfs_client/
+-rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/connection.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/exceptions.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_protol.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_test.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/storage_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/tracker_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/utils.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_operator.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools.egg-info/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/entry_points.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.9/angeltools.egg-info/not-zip-safe
+-rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/requires.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/top_level.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-19 08:24:27.987460 angeltools-0.2.9/setup.cfg
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-19 08:24:14.000000 angeltools-0.2.9/setup.py
```

### Comparing `angeltools-0.2.8/LICENSE` & `angeltools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/PKG-INFO` & `angeltools-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.8
+Version: 0.2.9
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.8/README.md` & `angeltools-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/Db/__init__.py` & `angeltools-0.2.9/angeltools/Db/__init__.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/Db/redis_connector.py` & `angeltools-0.2.9/angeltools/Db/redis_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,23 @@
 
     def del_hkeys(self, name, key_list: list):
         if not name or not key_list:
             return
         cli = self.cli()
         cli.hdel(name, *key_list)
 
-    def keys(self, pattern):
+    def get_keys(self, pattern):
         if not pattern:
             return
         return redis.Redis(**self.params).keys(pattern)
 
     def set_values(self, key_pattern, return_dic=True):
         if not key_pattern:
             return
-        keys = self.keys(key_pattern)
+        keys = self.get_keys(key_pattern)
 
         values = list()
         values_dic = dict()
         pipe = self.cli().pipeline()
         for key in keys:
             value = pipe.get(key)
             values.append(value)
```

### Comparing `angeltools-0.2.8/angeltools/ImageTool.py` & `angeltools-0.2.9/angeltools/ImageTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/MathTool.py` & `angeltools-0.2.9/angeltools/MathTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/Slavers.py` & `angeltools-0.2.9/angeltools/Slavers.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/StrTool.py` & `angeltools-0.2.9/angeltools/StrTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,15 @@
 
     使用方式：
     with FileLock(lock_id='xxxx', timeout=xx.xx):
         do_the_jobs()
 
     """
     def __init__(self, lock_id=None, timeout: float or int = None):
+        self.lock_id = lock_id
         self.timeout = float(timeout) if timeout else 3600 * 24 * 30 * 12
         self.__lock_dir()
         self.__get_lock_prefix()
         self.__init_lock(lock_id)
         self.fps = self.fp.absolute()
         self.enter_with_acquire = False
 
@@ -282,16 +283,23 @@
             lock_id = gen_uid1()
         lock_id_hash = hash_str(str(lock_id))
         self.fp = Path(f'{str(self.fp_prefix.absolute())}{lock_id_hash}.lock')
 
     def __acquire_lock(self):
         expire_time = time.time() + self.timeout
         try:
-            while self.__get_size() and time.time() - expire_time < 0:
-                self.__wait()
+            while True:
+                try:
+                    if self.__get_size() and time.time() - expire_time < 0:
+                        self.__wait()
+                    else:
+                        break
+                except Exception as E:
+                    print(f"acquire_lock error; lock id: {self.lock_id}: \n{E}")
+                    break
         except KeyboardInterrupt:
             sys.exit()
         self.__add_num()
         return self
 
     def __read_num(self):
         num = "0"
@@ -445,20 +453,24 @@
     #     for i in range(100):
     #         print(i)
     #         time.sleep(0.5)
     #     # print(lock.lock_time(format_time=True))
 
     def do_job(job_name):
         time.sleep(random.randint(1, 10) / 10)
-        with FileLock(f'test-lock', timeout=12):
+        with FileLock(f'test-lock_s1', timeout=12):
             for i in range(10):
-                print(f"{job_name}: {i}")
+                print(f"s1-{job_name}: {i}")
                 time.sleep(0.5)
-                # if i == 5:
-                #     raise ValueError("进程出错了")
+            with FileLock(f'test-lock_s2', timeout=12):
+                for i in range(10):
+                    print(f"s2-{job_name}: {i}")
+                    time.sleep(0.5)
+                    # if i == 5:
+                    #     raise ValueError("进程出错了")
 
 
     # do_job("进程1")
     from angeltools.Slavers import BigSlaves
     BigSlaves(7).work(do_job, ["进程1", "进程2", "进程3"])
 
     # FileLock().clear(lock_id='test-lock')
```

### Comparing `angeltools-0.2.8/angeltools/TimeTool.py` & `angeltools-0.2.9/angeltools/TimeTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/commands.py` & `angeltools-0.2.9/angeltools/commands.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/client.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/connection.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_protol.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_test.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/storage_client.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/tracker_client.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_client/utils.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools/fdfs/fdfs_operator.py` & `angeltools-0.2.9/angeltools/fdfs/fdfs_operator.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/angeltools.egg-info/PKG-INFO` & `angeltools-0.2.9/angeltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.8
+Version: 0.2.9
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.8/angeltools.egg-info/SOURCES.txt` & `angeltools-0.2.9/angeltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.8/setup.py` & `angeltools-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 using_setuptools = True
 
 setup_args = {
     "name": "angeltools",
-    "version": "0.2.8",
+    "version": "0.2.9",
     "url": "https://github.com/ga1008/angeltools",
     "description": "personal python small tools collection",
     "long_description": long_description,
     "author": "Guardian",
     "author_email": "zhling2012@live.com",
     "maintainer": "Guardian",
     "maintainer_email": "zhling2012@live.com",
```

