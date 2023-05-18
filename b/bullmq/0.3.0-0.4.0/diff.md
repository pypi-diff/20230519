# Comparing `tmp/bullmq-0.3.0.tar.gz` & `tmp/bullmq-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.3.0.tar", last modified: Tue Apr 18 08:58:58 2023, max compression
+gzip compressed data, was "bullmq-0.4.0.tar", last modified: Thu May 18 22:19:58 2023, max compression
```

## Comparing `bullmq-0.3.0.tar` & `bullmq-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.060057 bullmq-0.3.0/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-04-18 08:58:58.059681 bullmq-0.3.0/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-03-29 08:17:29.000000 bullmq-0.3.0/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.036847 bullmq-0.3.0/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      268 2023-02-16 14:21:48.000000 bullmq-0.3.0/bullmq/__init__.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.058868 bullmq-0.3.0/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5277 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5285 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      676 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    10209 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/timer.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8492 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.038537 bullmq-0.3.0/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1333 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-04-18 08:58:58.060205 bullmq-0.3.0/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1183 2023-04-18 08:57:31.000000 bullmq-0.3.0/setup.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.659998 bullmq-0.4.0/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-18 22:19:58.659561 bullmq-0.4.0/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.0/README.md
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.629815 bullmq-0.4.0/bullmq/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/backoffs.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.658790 bullmq-0.4.0/bullmq/commands/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getState-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveJobFromActiveToWait-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/pause-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/promote-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/reprocessJob-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/takeLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/error_code.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/event_emitter.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7277 2023-05-18 22:16:17.000000 bullmq-0.4.0/bullmq/job.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4852 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/queue.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      833 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/redis_connection.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    14763 2023-05-18 22:16:17.000000 bullmq-0.4.0/bullmq/scripts.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/timer.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7481 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/worker.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.632254 bullmq-0.4.0/bullmq.egg-info/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1352 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-05-18 22:19:58.660251 bullmq-0.4.0/setup.cfg
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1183 2023-05-18 22:18:20.000000 bullmq-0.4.0/setup.py
```

### Comparing `bullmq-0.3.0/PKG-INFO` & `bullmq-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.3.0
+Version: 0.4.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
   - [x] Regular jobs.
   - [ ] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
-- [ ] Job progress.
+- [x] Job progress.
 - [ ] Job retries.
 - [ ] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
```

### Comparing `bullmq-0.3.0/README.md` & `bullmq-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - [x] Regular jobs.
   - [ ] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
-- [ ] Job progress.
+- [x] Job progress.
 - [ ] Job retries.
 - [ ] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
```

### Comparing `bullmq-0.3.0/bullmq/commands/addJob-8.lua` & `bullmq-0.4.0/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/changeDelay-3.lua` & `bullmq-0.4.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.4.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/drain-4.lua` & `bullmq-0.4.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/getCounts-1.lua` & `bullmq-0.4.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/getRanges-1.lua` & `bullmq-0.4.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/getState-7.lua` & `bullmq-0.4.0/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/getStateV2-7.lua` & `bullmq-0.4.0/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/isFinished-3.lua` & `bullmq-0.4.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveJobFromActiveToWait-4.lua` & `bullmq-0.4.0/bullmq/commands/moveJobFromActiveToWait-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.4.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveToActive-9.lua` & `bullmq-0.4.0/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.4.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.4.0/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.4.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/obliterate-2.lua` & `bullmq-0.4.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/pause-4.lua` & `bullmq-0.4.0/bullmq/commands/pause-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/promote-6.lua` & `bullmq-0.4.0/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/removeJob-1.lua` & `bullmq-0.4.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.4.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/reprocessJob-4.lua` & `bullmq-0.4.0/bullmq/commands/reprocessJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/retryJob-8.lua` & `bullmq-0.4.0/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/commands/retryJobs-6.lua` & `bullmq-0.4.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/event_emitter.py` & `bullmq-0.4.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/queue.py` & `bullmq-0.4.0/bullmq/queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-from bullmq.scripts import Scripts
-from bullmq.job import Job, JobOptions
 from bullmq.redis_connection import RedisConnection
-from typing import TypedDict
-
-
-class RetryJobsOpts(TypedDict):
-    state: str
-    count: int
-    timestamp: int
-
-
-class QueueOptions(TypedDict, total=False):
-    """
-    Options for the Queue class.
-    """
-
-    prefix: str
-    """
-    Prefix for all queue keys.
-    """
+from bullmq.types import QueueOptions, RetryJobsOptions, JobOptions
+from bullmq.scripts import Scripts
+from bullmq.job import Job
 
 
 class Queue:
     """
     Instantiate a Queue object
     """
 
-    def __init__(self, name: str, redisOpts: dict = {}, opts: QueueOptions = {}):
+    def __init__(self, name: str, redisOpts: dict | str = {}, opts: QueueOptions = {}):
         """
         Initialize a connection
         """
         self.name = name
         self.redisConnection = RedisConnection(redisOpts)
         self.client = self.redisConnection.conn
         self.opts = opts
         self.prefix = opts.get("prefix", "bull")
-        self.scripts = Scripts(self.prefix, name, self.redisConnection.conn)
+        self.scripts = Scripts(
+            self.prefix, name, self.redisConnection.conn)
 
     async def add(self, name: str, data, opts: JobOptions = {}):
         """
         Adds a new job to the queue.
 
         @param name: Name of the job to be added to the queue,.
         @param data: Arbitrary data to append to the job.
         @param opts: Job options that affects how the job is going to be processed.
         """
-        job = Job(self.client, name, data, opts)
+        job = Job(self, name, data, opts)
         job_id = await self.scripts.addJob(job)
         job.id = job_id
         return job
 
     def pause(self):
         """
         Pauses the processing of this queue globally.
@@ -94,15 +78,15 @@
         """
         await self.pause()
         while True:
             cursor = await self.scripts.obliterate(1000, force)
             if cursor is None or cursor == 0 or cursor == "0":
                 break
 
-    async def retryJobs(self, opts: RetryJobsOpts = {}):
+    async def retryJobs(self, opts: RetryJobsOptions = {}):
         """
         Retry all the failed jobs.
         """
         while True:
             cursor = await self.scripts.retryJobs(
                 opts.get("state"),
                 opts.get("count"),
@@ -133,15 +117,15 @@
         for index, val in enumerate(responses):
             counts[current_types[index]] = val or 0
         return counts
 
     def sanitizeJobTypes(self, types):
         current_types = list(types)
 
-        if len(types) > 0 :
+        if len(types) > 0:
             sanitized_types = current_types.copy()
 
             try:
                 sanitized_types.index('waiting')
                 sanitized_types.append('paused')
             except ValueError:
                 pass
@@ -160,15 +144,7 @@
         ]
 
     def close(self):
         """
         Close the queue instance.
         """
         return self.redisConnection.close()
-
-
-async def fromId(queue: Queue, jobId: str):
-    key = f"{queue.prefix}:{queue.name}:{jobId}"
-    raw_data = await queue.client.hgetall(key)
-    return Job.fromJSON(queue.client, raw_data, jobId)
-
-Job.fromId = staticmethod(fromId)
```

### Comparing `bullmq-0.3.0/bullmq/redis_connection.py` & `bullmq-0.4.0/bullmq/redis_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 
 class RedisConnection:
     """
     RedisConnection class
     """
 
-    def __init__(self, redisOpts: dict = {}):
-        host = redisOpts.get("host") or "localhost"
-        port = redisOpts.get("port") or 6379
-        db = redisOpts.get("db") or 0
-        password = redisOpts.get("password") or None
-
-        self.conn = redis.Redis(
-            host=host, port=port, db=db, password=password, decode_responses=True)
+    def __init__(self, redisOpts: dict | str = {}):
+        if isinstance(redisOpts, dict):
+            host = redisOpts.get("host") or "localhost"
+            port = redisOpts.get("port") or 6379
+            db = redisOpts.get("db") or 0
+            password = redisOpts.get("password") or None
+
+            self.conn = redis.Redis(
+                host=host, port=port, db=db, password=password, decode_responses=True)
+        else:
+            self.conn = redis.from_url(redisOpts, decode_responses=True)
 
     def disconnect(self):
         """
         Disconnect from Redis
         """
         return self.conn.disconnect()
```

### Comparing `bullmq-0.3.0/bullmq/scripts.py` & `bullmq-0.4.0/bullmq/scripts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
     This class is used to load and execute Lua scripts.
     It is a wrapper around the Redis client.
 """
-from typing import Any
+
+from __future__ import annotations
 from redis import Redis
-from bullmq.job import Job
 from bullmq.error_code import ErrorCode
+from typing import Any, TYPE_CHECKING
+if TYPE_CHECKING:
+    from bullmq.job import Job
 
 import time
 import json
 import msgpack
 import os
 
 
@@ -21,22 +24,28 @@
     def __init__(self, prefix: str, queueName: str, redisClient: Redis):
         self.prefix = prefix
         self.queueName = queueName
         self.keys = {}
         self.redisClient = redisClient
         self.commands = {
             "addJob": redisClient.register_script(self.getScript("addJob-8.lua")),
+            "extendLock": redisClient.register_script(self.getScript("extendLock-2.lua")),
             "getCounts": redisClient.register_script(self.getScript("getCounts-1.lua")),
-            "obliterate": redisClient.register_script(self.getScript("obliterate-2.lua")),
-            "pause": redisClient.register_script(self.getScript("pause-4.lua")),
             "moveToActive": redisClient.register_script(self.getScript("moveToActive-9.lua")),
+            "moveToDelayed": redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": redisClient.register_script(self.getScript("moveToFinished-12.lua")),
-            "extendLock": redisClient.register_script(self.getScript("extendLock-2.lua")),
             "moveStalledJobsToWait": redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
+            "pause": redisClient.register_script(self.getScript("pause-4.lua")),
+            "obliterate": redisClient.register_script(self.getScript("obliterate-2.lua")),
+            "reprocessJob": redisClient.register_script(self.getScript("reprocessJob-6.lua")),
+            "retryJob": redisClient.register_script(self.getScript("retryJob-8.lua")),
             "retryJobs": redisClient.register_script(self.getScript("retryJobs-6.lua")),
+            "saveStacktrace": redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
+            "updateData": redisClient.register_script(self.getScript("updateData-1.lua")),
+            "updateProgress": redisClient.register_script(self.getScript("updateProgress-2.lua")),
         }
 
         # loop all the names and add them to the keys object
         names = ["", "active", "wait", "paused", "completed", "failed", "delayed",
                  "stalled", "limiter", "priority", "id", "stalled-check", "meta", "events"]
         for name in names:
             self.keys[name] = self.toKey(name)
@@ -80,20 +89,103 @@
         packedOpts = msgpack.packb(job.opts)
 
         keys = self.getKeys(['wait', 'paused', 'meta', 'id',
                             'delayed', 'priority', 'completed', 'events'])
 
         return self.commands["addJob"](keys=keys, args=[packedArgs, jsonData, packedOpts])
 
+    def saveStacktraceArgs(self, job_id: str, stacktrace: str, failedReason: str):
+        keys = [self.toKey(job_id)]
+        args = [stacktrace, failedReason]
+
+        return (keys, args)
+
+    def retryJobArgs(self, job_id: str, lifo: bool, token: str):
+        keys = self.getKeys(['active', 'wait', 'paused'])
+        keys.append(self.toKey(job_id))
+        keys.append(self.keys['meta'])
+        keys.append(self.keys['events'])
+        keys.append(self.keys['delayed'])
+        keys.append(self.keys['priority'])
+
+        push_cmd = "R" if lifo else "L"
+
+        args = [self.keys[''], round(time.time() * 1000), push_cmd,
+            job_id, token]
+
+        return (keys, args)
+
+    def moveToDelayedArgs(self, job_id: str, timestamp: int, token: str):
+        max_timestamp = max(0, timestamp or 0)
+
+        if timestamp > 0:
+            max_timestamp = max_timestamp * 0x1000 + (convert_to_int(job_id) & 0xfff)
+
+        keys = self.getKeys(['wait', 'active', 'priority', 'delayed'])
+        keys.append(self.toKey(job_id))
+        keys.append(self.keys['events'])
+        keys.append(self.keys['paused'])
+        keys.append(self.keys['meta'])
+
+        args = [self.keys[''], round(time.time() * 1000), str(max_timestamp),
+            job_id, token]
+
+        return (keys, args)
+
+    async def moveToDelayed(self, job_id: str, timestamp: int, token: str = "0"):
+        keys, args = self.moveToDelayedArgs(job_id, timestamp, token)
+
+        result = await self.commands["moveToDelayed"](keys=keys, args=args)
+
+        if result is not None:
+            if result < 0:
+                raise self.finishedErrors(result, job_id, 'moveToDelayed', 'active')
+        return None
+
     def getCounts(self, types):
         keys = self.getKeys([''])
-        transformed_types = list(map(lambda type: 'wait' if type == 'waiting' else type, types))
+        transformed_types = list(
+            map(lambda type: 'wait' if type == 'waiting' else type, types))
 
         return self.commands["getCounts"](keys=keys, args=transformed_types)
 
+    async def updateData(self, job_id: str, data):
+        keys = [self.toKey(job_id)]
+        data_json = json.dumps(data, separators=(',', ':'))
+        args = [data_json]
+
+        result = await self.commands["updateData"](keys=keys, args=args)
+
+        if result is not None:
+            if result < 0:
+                raise self.finishedErrors(result, job_id, 'updateData')
+        return None
+
+    async def reprocessJob(self, job: Job, state: str):
+        keys = [self.toKey(job.id)]
+        keys.append(self.keys['events'])
+        keys.append(self.keys[state])
+        keys.append(self.keys['wait'])
+        keys.append(self.keys['meta'])
+        keys.append(self.keys['paused'])
+        
+        args = [
+            job.id,
+            ("R" if job.opts.get("lifo") else "L") + "PUSH",
+            "failedReason" if state == "failed" else "returnvalue",
+            state
+            ]
+
+        result = await self.commands["reprocessJob"](keys=keys, args=args)
+
+        if result is not None:
+            if result < 0:
+                raise self.finishedErrors(result, job.id, 'reprocessJob', state)
+        return None
+
     def pause(self, pause: bool = True):
         """
         Pause or resume a queue
         """
         src = "wait" if pause else "paused"
         dst = "paused" if pause else "wait"
         keys = self.getKeys([src, dst, 'meta', 'events'])
@@ -113,15 +205,16 @@
         return result
 
     async def retryJobs(self, state: str, count: int, timestamp: int):
         """
         Remove a queue completely
         """
         current_state = state or 'failed'
-        keys = self.getKeys(['', 'events', current_state, 'wait', 'paused', 'meta'])
+        keys = self.getKeys(
+            ['', 'events', current_state, 'wait', 'paused', 'meta'])
         result = await self.commands["retryJobs"](keys=keys, args=[count or 1000, timestamp or round(time.time()*1000), current_state])
         return result
 
     async def moveToActive(self, token: str, opts: dict, jobId: str = "") -> list[Any]:
         """
         Add an item to the queue
         """
@@ -133,24 +226,34 @@
                             'stalled', 'limiter', 'delayed', 'paused', 'meta'])
         packedOpts = msgpack.packb(
             {"token": token, "lockDuration": lockDuration, "limiter": limiter}, use_bin_type=True)
         args = [self.keys[''], timestamp, jobId or "", packedOpts]
 
         result = await self.commands["moveToActive"](keys=keys, args=args)
 
-        # Todo: up to 4 results in tuple (only 2 now)
         return raw2NextJobData(result)
 
     def moveToCompleted(self, job: Job, val: Any, removeOnComplete, token: str, opts: dict, fetchNext=True):
         return self.moveToFinished(job, val, "returnvalue", removeOnComplete, "completed", token, opts, fetchNext)
 
     def moveToFailed(self, job: Job, failedReason: str, removeOnFailed, token: str, opts: dict, fetchNext=True):
         return self.moveToFinished(job, failedReason, "failedReason", removeOnFailed, "failed", token, opts, fetchNext)
 
-    async def moveToFinished(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext=True) -> list[Any] | None:
+    async def updateProgress(self, job_id: str, progress):
+        keys = [self.toKey(job_id), self.keys['events']]
+        progress_json = json.dumps(progress, separators=(',', ':'))
+        args = [job_id, progress_json]
+        result = await self.commands["updateProgress"](keys=keys, args=args)
+
+        if result is not None:
+            if result < 0:
+                raise self.finishedErrors(result, job_id, 'updateProgress')
+        return None
+
+    def moveToFinishedArgs(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext=True) -> list[Any] | None:
         timestamp = round(time.time() * 1000)
         metricsKey = self.toKey('metrics:' + target)
 
         keys = self.getKeys(['wait', 'active', 'priority', 'events',
                             'stalled', 'limiter', 'delayed', 'paused', target])
         keys.append(self.toKey(job.id))
         keys.append(self.keys['meta'])
@@ -191,22 +294,30 @@
             "attemptsMade": job.attemptsMade,
             "maxMetricsSize": getMetricsSize(opts),
             "fpof": getFailParentOnFailure(job),
         }, use_bin_type=True)
 
         args = [job.id, timestamp, propVal, val or "", target, "",
                 fetchNext and "fetch" or "", self.keys[''], packedOpts]
+        return (keys, args)
+
+    def moveToFailedArgs(self, job: Job, failed_reason: str, shouldRemove, token: str, opts: dict, fetchNext=True):
+        return self.moveToFinishedArgs(
+            job, failed_reason, 'failedReason', shouldRemove, 'failed',
+            token, opts, fetchNext
+        )
+
+    async def moveToFinished(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext=True) -> list[Any] | None:
+        keys, args = self.moveToFinishedArgs(job, val, propVal, shouldRemove, target, token, opts, fetchNext)
+
         result = await self.commands["moveToFinished"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
-                raise finishedErrors(result, job.id, 'finished', 'active')
-            else:
-                # I do not like this as it is using a sideeffect
-                job.finishedOn = timestamp
+                raise self.finishedErrors(result, job.id, 'finished', 'active')
             return raw2NextJobData(result)
         return None
 
     def extendLock(self, jobId: str, token: str, duration: int, client: Redis = None):
         keys = [self.toKey(jobId) + ":lock", self.keys['stalled']]
         args = [token, duration, jobId]
         return self.commands["extendLock"](keys, args, client)
@@ -215,39 +326,46 @@
         keys = self.getKeys(['stalled', 'wait', 'active', 'failed',
                             'stalled-check', 'meta', 'paused', 'events'])
         args = [maxStalledCount, self.keys[''], round(
             time.time() * 1000), stalledInterval]
         return self.commands["moveStalledJobsToWait"](keys, args)
 
 
-def finishedErrors(code: int, jobId: str, command: str, state: str) -> TypeError:
-    if code == ErrorCode.JobNotExist.value:
-        return TypeError(f"Missing key for job {jobId}.{command}")
-    elif code == ErrorCode.JobLockNotExist.value:
-        return TypeError(f"Missing lock for job {jobId}.{command}")
-    elif code == ErrorCode.JobNotInState.value:
-        return TypeError(f"Job {jobId} is not in the state {state}.{command}")
-    elif code == ErrorCode.JobPendingDependencies.value:
-        return TypeError(f"Job {jobId} has pending dependencies.{command}")
-    elif code == ErrorCode.ParentJobNotExist.value:
-        return TypeError(f"Missing key for parent job {jobId}.{command}")
-    elif code == ErrorCode.JobLockMismatch.value:
-        return TypeError(f"Lock mismatch for job {jobId}. Cmd {command} from {state}")
-    else:
-        return TypeError(f"Unknown code {str(code)} error for {jobId}.{command}")
+    def finishedErrors(code: int, jobId: str, command: str, state: str) -> TypeError:
+        if code == ErrorCode.JobNotExist.value:
+            return TypeError(f"Missing key for job {jobId}.{command}")
+        elif code == ErrorCode.JobLockNotExist.value:
+            return TypeError(f"Missing lock for job {jobId}.{command}")
+        elif code == ErrorCode.JobNotInState.value:
+            return TypeError(f"Job {jobId} is not in the state {state}.{command}")
+        elif code == ErrorCode.JobPendingDependencies.value:
+            return TypeError(f"Job {jobId} has pending dependencies.{command}")
+        elif code == ErrorCode.ParentJobNotExist.value:
+            return TypeError(f"Missing key for parent job {jobId}.{command}")
+        elif code == ErrorCode.JobLockMismatch.value:
+            return TypeError(f"Lock mismatch for job {jobId}. Cmd {command} from {state}")
+        else:
+            return TypeError(f"Unknown code {str(code)} error for {jobId}.{command}")
 
 
 def raw2NextJobData(raw: list[Any]) -> list[Any] | None:
     if raw:
-        # TODO: return all the raw datas (up to 4)
+        result = [None, raw[1], None, None] if len(raw) == 2 else [None, raw[1], raw[2], raw[3]]
         if raw[0]:
-            return (array2obj(raw[0]), raw[1])
-        else:
-            return (None, raw[1])
-    return None
+            result[0]= array2obj(raw[0])
+        return result
+    return [None, None, None, None]
 
 
 def array2obj(arr: list[str]) -> dict[str, str]:
     obj = {}
     for i in range(0, len(arr), 2):
         obj[arr[i]] = arr[i + 1]
     return obj
+
+
+def convert_to_int(text: str):
+    try:
+        result = int(text)
+        return result
+    except ValueError:
+        return 0
```

### Comparing `bullmq-0.3.0/bullmq/timer.py` & `bullmq-0.4.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.3.0/bullmq/worker.py` & `bullmq-0.4.0/bullmq/worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,39 @@
-from typing import Callable, TypedDict, Any, List
+from typing import Callable
 from uuid import uuid4
 from bullmq.scripts import Scripts
 from bullmq.redis_connection import RedisConnection
 from bullmq.event_emitter import EventEmitter
 from bullmq.job import Job
 from bullmq.timer import Timer
+from bullmq.types import WorkerOptions
 
 import asyncio
 import traceback
 import time
 
-
-class WorkerOptions(TypedDict, total=False):
-    autorun: bool
-    """
-    Condition to start processor at instance creation
-
-    @default true
-    """
-
-    concurrency: int
-    """
-    Amount of jobs that a single worker is allowed to work on
-    in parallel.
-
-    @default 1
-    @see https://docs.bullmq.io/guide/workers/concurrency
-    """
-
-    maxStalledCount: int
-    """
-    Amount of times a job can be recovered from a stalled state
-    to the `wait` state. If this is exceeded, the job is moved
-    to `failed`.
-
-    @default 1
-    """
-
-    stalledInterval: int
-    """
-    Number of milliseconds between stallness checks.
-
-    @default 30000
-    """
-
-    lockDuration: int
-    """
-    Duration of the lock for the job in milliseconds. The lock represents that
-    a worker is processing the job. If the lock is lost, the job will be eventually
-    be picked up by the stalled checker and move back to wait so that another worker
-    can process it again.
-
-    @default 30000
-    """
-
-    prefix: str
-    """
-    Prefix for all queue keys.
-    """
-
-    connection: dict[str, Any]
-    """
-    Options for connecting to a Redis instance.
-    """
-
-
 class Worker(EventEmitter):
     def __init__(self, name: str, processor: Callable[[Job, str], asyncio.Future], opts: WorkerOptions = {}):
         super().__init__()
         self.name = name
         self.processor = processor
-        self.opts = {
-            "concurrency": opts.get("concurrency", 1),
-            "lockDuration": opts.get("lockDuration", 30000),
-            "maxStalledCount": opts.get("maxStalledCount", 1),
-            "stalledInterval": opts.get("stalledInterval", 30000),
+        final_opts = {
+            "concurrency": 1,
+            "lockDuration": 30000,
+            "maxStalledCount": 1,
+            "stalledInterval": 30000,
         }
+        final_opts.update(opts or {})
+        self.opts = final_opts
         redis_opts = opts.get("connection", {})
         self.redisConnection = RedisConnection(redis_opts)
         self.blockingRedisConnection = RedisConnection(redis_opts)
         self.client = self.redisConnection.conn
         self.bclient = self.blockingRedisConnection.conn
+        self.prefix = opts.get("prefix", "bull")
         self.scripts = Scripts(opts.get("prefix", "bull"), name, self.client)
         self.closing = False
         self.forceClosing = False
         self.closed = False
         self.running = False
         self.processing = set()
         self.jobs = set()
@@ -141,45 +90,43 @@
         @param token: worker token to be assigned to retrieved job
         @returns a Job or undefined if no job was available in the queue.
         """
         # First try to move a job from the waiting list to the active list
         result = await self.scripts.moveToActive(token, self.opts)
         job = None
         job_id = None
+        limit_until = None
         delay_until = None
+
         if result:
-            job, job_id = result
+            job, job_id, limit_until, delay_until = result
 
         # If there are no jobs in the waiting list we keep waiting with BRPOPLPUSH
         if job is None:
             timeout = min(delay_until - int(time.time() * 1000)
                           if delay_until else 5000, 5000) / 1000
             job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
             if job_id:
-                job, job_id = await self.scripts.moveToActive(token, self.opts, job_id)
+                job, job_id, limit_until, delay_until = await self.scripts.moveToActive(token, self.opts, job_id)
 
         if job and job_id:
-            return Job.fromJSON(self.client, job, job_id)
+            return Job.fromJSON(self, job, job_id)
 
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
                 await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", False), token, self.opts, fetchNext=not self.closing)
             self.emit("completed", job, result)
         except Exception as err:
             try:
                 print("Error processing job", err)
-                stacktrace = traceback.format_exc()
-
                 if not self.forceClosing:
-                    await self.scripts.moveToFailed(job, str(err), job.opts.get("removeOnFail", False), token, self.opts, fetchNext=not self.closing)
-
-                # TODO: Store the stacktrace in the job
+                    await job.moveToFailed(err, token)
 
                 self.emit("failed", job, err)
             except Exception as err:
                 print("Error moving job to failed", err)
                 self.emit("error", err, job)
         finally:
             self.jobs.remove((job, token))
@@ -216,20 +163,26 @@
 
     async def close(self, force: bool = False):
         """
         Close the worker
         """
         if force:
             self.forceClosing = True
+            self.cancelProcessing()
 
         self.closing = True
 
         await self.blockingRedisConnection.close()
         await self.redisConnection.close()
 
+    def cancelProcessing(self):
+        for job in self.processing:
+            if not job.done():
+                job.cancel()
+
 
 async def getCompleted(task_set: set) -> tuple[list[Job], list]:
     job_set, pending = await asyncio.wait(task_set, return_when=asyncio.FIRST_COMPLETED)
     jobs = [extract_result(job_task) for job_task in job_set]
     # we filter `None` out to remove:
     # a) an empty 'completed jobs' list; and
     # b) a failed extract_result
@@ -237,11 +190,12 @@
     return jobs, pending
 
 
 def extract_result(job_task):
     try:
         return job_task.result()
     except Exception as e:
-        # lets use a simple-but-effective error handling:
-        # print error message and ignore the job
-        print("ERROR:", e)
-        traceback.print_exc()
+        if not str(e).startswith('Connection closed by server'):
+            # lets use a simple-but-effective error handling:
+            # print error message and ignore the job
+            print("ERROR:", e)
+            traceback.print_exc()
```

### Comparing `bullmq-0.3.0/bullmq.egg-info/PKG-INFO` & `bullmq-0.4.0/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.3.0
+Version: 0.4.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
   - [x] Regular jobs.
   - [ ] Delayed jobs.
   - [ ] Job priority.
   - [ ] Repeatable.
 
 - [x] Workers
 - [ ] Job events.
-- [ ] Job progress.
+- [x] Job progress.
 - [ ] Job retries.
 - [ ] Job backoff.
 - [x] Getters.
 
 ## Installation
 
 ```bash
```

### Comparing `bullmq-0.3.0/bullmq.egg-info/SOURCES.txt` & `bullmq-0.4.0/bullmq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 bullmq/__init__.py
+bullmq/backoffs.py
 bullmq/error_code.py
 bullmq/event_emitter.py
 bullmq/job.py
 bullmq/queue.py
 bullmq/redis_connection.py
 bullmq/scripts.py
 bullmq/timer.py
```

### Comparing `bullmq-0.3.0/setup.py` & `bullmq-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(".", 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bullmq',
-    version='0.3.0',    
+    version='0.4.0',    
     description='BullMQ for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bullmq.io',
     author='Taskforce.sh Inc.',
     author_email='manast@taskforce.sh',
     license='MIT',
```

