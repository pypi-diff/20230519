# Comparing `tmp/iboxstacksops-0.7.7.tar.gz` & `tmp/iboxstacksops-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.7.tar", last modified: Thu May 18 19:43:16 2023, max compression
+gzip compressed data, was "iboxstacksops-0.7.8.tar", last modified: Thu May 18 19:55:12 2023, max compression
```

## Comparing `iboxstacksops-0.7.7.tar` & `iboxstacksops-0.7.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.7/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.651079 iboxstacksops-0.7.7/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.651079 iboxstacksops-0.7.7/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.655079 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.7/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.7/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.7/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4077 2023-05-11 16:41:05.000000 iboxstacksops-0.7.7/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5474 2023-05-18 16:13:00.000000 iboxstacksops-0.7.7/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4234 2023-05-18 19:15:17.000000 iboxstacksops-0.7.7/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.7/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.7/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.7/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.7/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6428 2023-05-18 19:31:13.000000 iboxstacksops-0.7.7/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.7/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1349 2023-05-18 19:03:13.000000 iboxstacksops-0.7.7/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8715 2023-05-18 19:03:44.000000 iboxstacksops-0.7.7/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.7/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.7/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.7/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.7/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.7/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.7/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.7/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.7/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.7/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.7/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.7/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.7/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-18 19:42:22.000000 iboxstacksops-0.7.7/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.395010 iboxstacksops-0.7.8/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:55:12.395010 iboxstacksops-0.7.8/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.8/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.383010 iboxstacksops-0.7.8/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.383010 iboxstacksops-0.7.8/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.387010 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:55:12.000000 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-18 19:55:12.000000 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-18 19:55:12.000000 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-18 19:55:12.000000 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-18 19:55:12.000000 iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.395010 iboxstacksops-0.7.8/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.8/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.8/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.8/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4096 2023-05-18 19:50:43.000000 iboxstacksops-0.7.8/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5474 2023-05-18 16:13:00.000000 iboxstacksops-0.7.8/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4204 2023-05-18 19:47:19.000000 iboxstacksops-0.7.8/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.8/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.8/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.8/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.8/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6390 2023-05-18 19:46:59.000000 iboxstacksops-0.7.8/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.8/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1354 2023-05-18 19:52:27.000000 iboxstacksops-0.7.8/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8720 2023-05-18 19:52:16.000000 iboxstacksops-0.7.8/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.8/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.8/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.8/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.8/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.8/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.8/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.8/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.8/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.8/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.8/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.8/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:55:12.395010 iboxstacksops-0.7.8/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.8/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-18 19:55:12.395010 iboxstacksops-0.7.8/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-18 19:54:34.000000 iboxstacksops-0.7.8/setup.py
```

### Comparing `iboxstacksops-0.7.7/PKG-INFO` & `iboxstacksops-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.7
+Version: 0.7.8
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.7
+Version: 0.7.8
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.7.8/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/actions.py` & `iboxstacksops-0.7.8/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/aws.py` & `iboxstacksops-0.7.8/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/cfg.py` & `iboxstacksops-0.7.8/iboxstacksops/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 statisticresponse = "p95"
 silent = True
 vertical = False
 profile = False
 output = "text"
 disable_rollback = False
 changeset_original = False
+print_mylog = True
 #
 
 OUT_WIDTH = 1000000
 
 SLACK_CHANNEL = "_cf_deploy"
 
 MAX_SINGLE_STACKS = 5
```

### Comparing `iboxstacksops-0.7.7/iboxstacksops/changeset.py` & `iboxstacksops-0.7.8/iboxstacksops/changeset.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/commands.py` & `iboxstacksops-0.7.8/iboxstacksops/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,19 +72,19 @@
 
 def parameters():
     w_stacks = stacks.get()
     cfg.exports = get_exports()
     result = concurrent_exec("parameters", w_stacks, i_stack)
 
 
-def info(mylog=True):
+def info():
     if not cfg.compact:
         cfg.OUT_WIDTH = 80
     w_stacks = stacks.get()
-    result = concurrent_exec("info", w_stacks, i_stack, **{"mylog": mylog})
+    result = concurrent_exec("info", w_stacks, i_stack)
 
     return result
 
 def show_resources():
     w_stacks = stacks.get()
     result = concurrent_exec("show_resources", w_stacks, i_stack)
```

### Comparing `iboxstacksops-0.7.7/iboxstacksops/common.py` & `iboxstacksops-0.7.8/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/dashboard.py` & `iboxstacksops-0.7.8/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/events.py` & `iboxstacksops-0.7.8/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/i_region.py` & `iboxstacksops-0.7.8/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/i_stack.py` & `iboxstacksops-0.7.8/iboxstacksops/i_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,19 +95,19 @@
         if check:
             parameters.add_stack_params_as_args(self, parser)
             return self.stack_parsed_args, self.parameters
         else:
             logger.info(f"{self.name} Parameters:")
             parser.print_help()
 
-    def info(self, mylog=True):
+    def info(self):
         self.stack = self.cloudformation.Stack(self.name)
         self.template = template.get_template(self)
-        outputs_out = outputs.show(self, "before", mylog=mylog)
-        parameters_out = parameters.show_override(self, mylog=mylog)
+        outputs_out = outputs.show(self, "before")
+        parameters_out = parameters.show_override(self)
 
         return {
             "OUTPUTS": outputs_out,
             "PARAMETERS NOT DEFAULT": parameters_out,
         }
 
     def show_resources(self):
```

### Comparing `iboxstacksops-0.7.7/iboxstacksops/msg.py` & `iboxstacksops-0.7.8/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/outputs.py` & `iboxstacksops-0.7.8/iboxstacksops/outputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
     istack.changed["outputs"] = changed
     istack.cfg.OUT_WIDTH = 80
     show(istack, "changed")
 
 
 # show stack current outputs as dict
-def show(istack, when, mylog=True):
+def show(istack, when):
     outputs = getattr(istack, when)["outputs"]
 
     out = pformat(outputs, width=istack.cfg.OUT_WIDTH)
 
-    if mylog:
+    if istack.cfg.print_mylog:
         istack.mylog(f"{when.upper()} - STACK OUTPUTS\n{out}\n")
 
     return outputs
 
 
 def get(stack):
     outputs = {}
```

### Comparing `iboxstacksops-0.7.7/iboxstacksops/parameters.py` & `iboxstacksops-0.7.8/iboxstacksops/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,30 +154,30 @@
     istack.stack_parsed_args = args
 
     for n, v in vars(args).items():
         if not hasattr(istack.cfg, n):
             setattr(istack.cfg, n, v)
 
 
-def show_override(istack, mylog=True):
+def show_override(istack):
     params = {}
     for name, value in istack.c_parameters.items():
         if (
             not name.startswith("Env")
             and any(name not in n for n in ["UpdateMode"])
             and any(
                 name == t_name and (value != t_value.get("Default"))
                 for t_name, t_value in istack.parameters.items()
             )
         ):
             params[name] = value
 
     out = pformat(params, width=istack.cfg.OUT_WIDTH)
 
-    if mylog:
+    if istack.cfg.print_mylog:
         istack.mylog(f"CURRENT NOT DEFAULT - STACK PARAMETERS\n{out}\n")
 
     return params
 
 
 def process(istack, show=True):
     logger.info("Processing Parameters")
```

### Comparing `iboxstacksops-0.7.7/iboxstacksops/parser.py` & `iboxstacksops-0.7.8/iboxstacksops/parser.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/replica.py` & `iboxstacksops-0.7.8/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/resolve.py` & `iboxstacksops-0.7.8/iboxstacksops/resolve.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/resources.py` & `iboxstacksops-0.7.8/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/route53.py` & `iboxstacksops-0.7.8/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/ssm.py` & `iboxstacksops-0.7.8/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/stacks.py` & `iboxstacksops-0.7.8/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/table.py` & `iboxstacksops-0.7.8/iboxstacksops/table.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/tags.py` & `iboxstacksops-0.7.8/iboxstacksops/tags.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/template.py` & `iboxstacksops-0.7.8/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/iboxstacksops/tools.py` & `iboxstacksops-0.7.8/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.7/setup.py` & `iboxstacksops-0.7.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.7",
+    version="0.7.8",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

