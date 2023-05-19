# Comparing `tmp/nvosscript-1.3.0.7.tar.gz` & `tmp/nvosscript-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.0.7.tar", last modified: Thu May 18 09:53:11 2023, max compression
+gzip compressed data, was "nvosscript-1.3.1.tar", last modified: Fri May 19 01:33:14 2023, max compression
```

## Comparing `nvosscript-1.3.0.7.tar` & `nvosscript-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.672206 nvosscript-1.3.0.7/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0.7/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 09:53:11.672070 nvosscript-1.3.0.7/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0.7/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.669299 nvosscript-1.3.0.7/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0.7/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13680 2023-05-18 09:52:52.000000 nvosscript-1.3.0.7/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0.7/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0.7/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0.7/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.670153 nvosscript-1.3.0.7/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-18 09:53:11.000000 nvosscript-1.3.0.7/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-18 09:53:11.672243 nvosscript-1.3.0.7/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      807 2023-05-18 09:53:09.000000 nvosscript-1.3.0.7/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.670809 nvosscript-1.3.0.7/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/skyeye/datahandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/skyeye/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/skyeye/skyeyecommand.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.671335 nvosscript-1.3.0.7/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0.7/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0.7/start/commonUtil.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4527 2023-05-18 09:53:09.000000 nvosscript-1.3.0.7/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.667430 nvosscript-1.3.0.7/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.671499 nvosscript-1.3.0.7/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0.7/venv/bin/activate_this.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:53:11.671779 nvosscript-1.3.0.7/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0.7/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.907871 nvosscript-1.3.1/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.1/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-19 01:33:14.907712 nvosscript-1.3.1/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.1/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.902673 nvosscript-1.3.1/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.1/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13416 2023-05-19 01:32:59.000000 nvosscript-1.3.1/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.1/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.1/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.1/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.1/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.904828 nvosscript-1.3.1/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-19 01:33:14.907981 nvosscript-1.3.1/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-05-19 01:32:59.000000 nvosscript-1.3.1/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.905890 nvosscript-1.3.1/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/datahandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/skyeyecommand.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.906519 nvosscript-1.3.1/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.1/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.1/start/commonUtil.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4525 2023-05-19 01:33:05.000000 nvosscript-1.3.1/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.899806 nvosscript-1.3.1/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.906692 nvosscript-1.3.1/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.1/venv/bin/activate_this.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.907256 nvosscript-1.3.1/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.1/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.0.7/LICENSE` & `nvosscript-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/nvos/file.py` & `nvosscript-1.3.1/nvos/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,17 +164,14 @@
             if os.path.isdir(os.path.join(workspace_path, file_path)):
                 temp = {"project_space": os.path.join(workspace_path, file_path),
                         "fileDirectory": os.path.join(workspace_path, file_path),
                         "git_branch": "nvos_default", "gitBranch": "nvos_default"}
                 result_list.append(temp)
         return result_list
 
-    print(f"not_exit_git_data ps: {os.path.join(os.getcwd(), '.ndtc')} : {not_exit_git_data}")
-    print(f"exit_git_data ps: {os.path.join(os.getcwd(), '.ndtc')} : {exit_git_data}")
-
     filter_exit_data = []
     for project_space in not_exit_git_data:
         max_prefix = ""
         max_public_str = ""
 
         for item in exit_git_data:
             prefix = item["project_space"][:item["project_space"].rfind(os.path.sep)]
@@ -213,15 +210,14 @@
     git_path = os.path.join(workspace_path, ".git")
     if not os.path.exists(git_path):
         return ""
 
     try:
         completed_process = subprocess.run(['git', 'branch'], stdout=subprocess.PIPE)
         git_branch_val = completed_process.stdout.decode().splitlines()
-        print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {git_branch_val}")
         if len(git_branch_val) == 0:
             return "(no branch)"
         git_branch_data = ""
         for line in git_branch_val:
             if "*" in line:
                 git_branch_data = line.split("*")[1].strip()
         return git_branch_data
```

### Comparing `nvosscript-1.3.0.7/nvos/login.py` & `nvosscript-1.3.1/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/nvos/remote.py` & `nvosscript-1.3.1/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/nvos/run.py` & `nvosscript-1.3.1/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/nvos/utils.py` & `nvosscript-1.3.1/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/setup.py` & `nvosscript-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.0.7',
+    version='1.3.1',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.0.7/skyeye/datahandler.py` & `nvosscript-1.3.1/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/skyeye/remote.py` & `nvosscript-1.3.1/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/start/main.py` & `nvosscript-1.3.1/start/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.0.7")
+        print("1.3.1")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.0.7/venv/bin/activate_this.py` & `nvosscript-1.3.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.7/win/win_auto_script.py` & `nvosscript-1.3.1/win/win_auto_script.py`

 * *Files identical despite different names*

