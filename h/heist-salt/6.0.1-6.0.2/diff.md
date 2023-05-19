# Comparing `tmp/heist-salt-6.0.1.tar.gz` & `tmp/heist-salt-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heist-salt-6.0.1.tar", last modified: Mon May  8 17:04:31 2023, max compression
+gzip compressed data, was "heist-salt-6.0.2.tar", last modified: Fri May 19 17:43:53 2023, max compression
```

## Comparing `heist-salt-6.0.1.tar` & `heist-salt-6.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.529930 heist-salt-6.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-08 17:04:01.000000 heist-salt-6.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2417 2023-05-08 17:04:31.529930 heist-salt-6.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-05-08 17:04:01.000000 heist-salt-6.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.518929 heist-salt-6.0.1/heist_salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.521929 heist-salt-6.0.1/heist_salt/artifact/
--rw-rw-rw-   0 root         (0) root         (0)    20587 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/artifact/salt.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.513928 heist-salt-6.0.1/heist_salt/heist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.522929 heist-salt-6.0.1/heist_salt/heist/salt/
--rw-rw-rw-   0 root         (0) root         (0)    17322 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/init.py
--rw-rw-rw-   0 root         (0) root         (0)     4684 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/master.py
--rw-rw-rw-   0 root         (0) root         (0)     5991 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/minion.py
--rw-rw-rw-   0 root         (0) root         (0)     5729 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/heist/salt/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.523929 heist-salt-6.0.1/heist_salt/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.523929 heist-salt-6.0.1/heist_salt/salt/call/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.524929 heist-salt-6.0.1/heist_salt/salt/call/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/call/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/call/init.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.525929 heist-salt-6.0.1/heist_salt/salt/key/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/salt/key/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/init.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/local_master.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/key/raas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/salt/pillar/
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/salt/pillar/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.526929 heist-salt-6.0.1/heist_salt/service/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/service/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.527929 heist-salt-6.0.1/heist_salt/service/salt/
--rw-rw-rw-   0 root         (0) root         (0)     5702 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/service/salt/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.528930 heist-salt-6.0.1/heist_salt/tool/
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/tool/service.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-08 17:04:01.000000 heist-salt-6.0.1/heist_salt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:04:31.520929 heist-salt-6.0.1/heist_salt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2417 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-08 17:04:31.000000 heist-salt-6.0.1/heist_salt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-08 17:04:01.000000 heist-salt-6.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:04:31.529930 heist-salt-6.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-08 17:04:01.000000 heist-salt-6.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.769801 heist-salt-6.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-19 17:43:30.000000 heist-salt-6.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-19 17:43:53.768801 heist-salt-6.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-05-19 17:43:30.000000 heist-salt-6.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.762801 heist-salt-6.0.2/heist_salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.764801 heist-salt-6.0.2/heist_salt/artifact/
+-rw-rw-rw-   0 root         (0) root         (0)    20587 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/artifact/salt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.759801 heist-salt-6.0.2/heist_salt/heist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.765801 heist-salt-6.0.2/heist_salt/heist/salt/
+-rw-rw-rw-   0 root         (0) root         (0)    17322 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/heist/salt/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/heist/salt/master.py
+-rw-rw-rw-   0 root         (0) root         (0)     6054 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/heist/salt/minion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5792 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/heist/salt/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.765801 heist-salt-6.0.2/heist_salt/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.765801 heist-salt-6.0.2/heist_salt/salt/call/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.765801 heist-salt-6.0.2/heist_salt/salt/call/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/call/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/call/init.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.766800 heist-salt-6.0.2/heist_salt/salt/key/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/key/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.766800 heist-salt-6.0.2/heist_salt/salt/key/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/key/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/key/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/key/local_master.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/key/raas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.767801 heist-salt-6.0.2/heist_salt/salt/pillar/
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/salt/pillar/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.767801 heist-salt-6.0.2/heist_salt/service/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/service/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.767801 heist-salt-6.0.2/heist_salt/service/salt/
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/service/salt/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.768801 heist-salt-6.0.2/heist_salt/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/tool/artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/tool/config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/tool/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/tool/service.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-19 17:43:30.000000 heist-salt-6.0.2/heist_salt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:43:53.763801 heist-salt-6.0.2/heist_salt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-19 17:43:53.000000 heist-salt-6.0.2/heist_salt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-19 17:43:53.000000 heist-salt-6.0.2/heist_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:43:53.000000 heist-salt-6.0.2/heist_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-19 17:43:53.000000 heist-salt-6.0.2/heist_salt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-19 17:43:53.000000 heist-salt-6.0.2/heist_salt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-19 17:43:30.000000 heist-salt-6.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 17:43:53.769801 heist-salt-6.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-19 17:43:30.000000 heist-salt-6.0.2/setup.py
```

### Comparing `heist-salt-6.0.1/LICENSE` & `heist-salt-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/PKG-INFO` & `heist-salt-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist-salt
-Version: 6.0.1
+Version: 6.0.2
 Summary: Vertical app-merge components for salt into heist
 Home-page: 
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heist-salt-6.0.1/README.rst` & `heist-salt-6.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/artifact/salt.py` & `heist-salt-6.0.2/heist_salt/artifact/salt.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/conf.py` & `heist-salt-6.0.2/heist_salt/conf.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/heist/salt/init.py` & `heist-salt-6.0.2/heist_salt/heist/salt/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/heist/salt/master.py` & `heist-salt-6.0.2/heist_salt/heist/salt/master.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,8 +151,10 @@
             hub.tool.artifacts.get_salt_path(
                 run_dir, run_dir_root=run_dir_root, target_os=target_os
             )
         )
         + f"/{service_name}"
         + f" -c {hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
     )
+    if target_os == "linux":
+        run_cmd = run_cmd + " -d"
     return run_cmd
```

### Comparing `heist-salt-6.0.1/heist_salt/heist/salt/minion.py` & `heist-salt-6.0.2/heist_salt/heist/salt/minion.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,8 +189,10 @@
             hub.tool.artifacts.get_salt_path(
                 run_dir, run_dir_root=run_dir_root, target_os=target_os
             )
             / service_name
         )
         + f" -c {hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
     )
+    if target_os == "linux":
+        run_cmd = run_cmd + " -d"
     return run_cmd
```

### Comparing `heist-salt-6.0.1/heist_salt/heist/salt/proxy.py` & `heist-salt-6.0.2/heist_salt/heist/salt/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,8 +190,10 @@
                 run_dir, run_dir_root=run_dir_root, target_os=target_os
             )
         )
         + f"/{service_name}"
         + f" -c {hub.tool.artifacts.target_conf(run_dir, run_dir_root=run_dir_root, target_os=target_os)}"
         + f" --proxyid={target_id}"
     )
+    if target_os == "linux":
+        run_cmd = run_cmd + " -d"
     return run_cmd
```

### Comparing `heist-salt-6.0.1/heist_salt/salt/call/init.py` & `heist-salt-6.0.2/heist_salt/salt/call/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/salt/key/init.py` & `heist-salt-6.0.2/heist_salt/salt/key/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/salt/key/local_master.py` & `heist-salt-6.0.2/heist_salt/salt/key/local_master.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/salt/pillar/init.py` & `heist-salt-6.0.2/heist_salt/salt/pillar/init.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/service/salt/init.py` & `heist-salt-6.0.2/heist_salt/service/salt/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     )
     if not await hub.service[service_plugin].status(
         target_name,
         tunnel_plugin,
         service_name,
         block=False,
         target_os=target_os,
+        sudo=False,
     ):
         await hub.service.salt.init.apply_service_config(
             target_name,
             tunnel_plugin,
             run_dir,
             service_plugin,
             target_os=target_os,
```

### Comparing `heist-salt-6.0.1/heist_salt/tool/artifacts.py` & `heist-salt-6.0.2/heist_salt/tool/artifacts.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/tool/config.py` & `heist-salt-6.0.2/heist_salt/tool/config.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt/tool/service.py` & `heist-salt-6.0.2/heist_salt/tool/service.py`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/heist_salt.egg-info/PKG-INFO` & `heist-salt-6.0.2/heist_salt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist-salt
-Version: 6.0.1
+Version: 6.0.2
 Summary: Vertical app-merge components for salt into heist
 Home-page: 
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heist-salt-6.0.1/heist_salt.egg-info/SOURCES.txt` & `heist-salt-6.0.2/heist_salt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/pyproject.toml` & `heist-salt-6.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heist-salt-6.0.1/setup.py` & `heist-salt-6.0.2/setup.py`

 * *Files identical despite different names*

