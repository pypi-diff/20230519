# Comparing `tmp/1password-secrets-0.0.2.tar.gz` & `tmp/1password-secrets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1password-secrets-0.0.2.tar", last modified: Wed Mar  1 18:01:28 2023, max compression
+gzip compressed data, was "1password-secrets-0.0.3.tar", last modified: Fri May 19 10:50:15 2023, max compression
```

## Comparing `1password-secrets-0.0.2.tar` & `1password-secrets-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:01:28.129314 1password-secrets-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:01:28.129314 1password-secrets-0.0.2/1password_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 18:01:28.000000 1password-secrets-0.0.2/1password_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-01 18:01:28.129314 1password-secrets-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-01 18:01:16.000000 1password-secrets-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-03-01 18:01:16.000000 1password-secrets-0.0.2/onepassword_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-01 18:01:28.129314 1password-secrets-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-01 18:01:16.000000 1password-secrets-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:50:15.175514 1password-secrets-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:50:15.175514 1password-secrets-0.0.3/1password_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 10:50:15.000000 1password-secrets-0.0.3/1password_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-19 10:50:15.175514 1password-secrets-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-19 10:50:05.000000 1password-secrets-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-19 10:50:05.000000 1password-secrets-0.0.3/onepassword_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 10:50:15.175514 1password-secrets-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 10:50:05.000000 1password-secrets-0.0.3/setup.py
```

### Comparing `1password-secrets-0.0.2/1password_secrets.egg-info/PKG-INFO` & `1password-secrets-0.0.3/1password_secrets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password-secrets
-Version: 0.0.2
+Version: 0.0.3
 Summary: 1password-secrets is a set of utilities to sync 1Password secrets.
 Home-page: https://github.com/significa/fly-1password-secrets
 Author: Significa
 License: MIT
 Keywords: fly.io,1password,secrets
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -59,18 +59,18 @@
 
 `pip install 1password-secrets`
 
 ## Usage
 
 ### Local
 
-From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `get` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
+From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
 
 To get secrets from 1Password, run:
-`1password-secrets local get`
+`1password-secrets local pull`
 
 To push the local changes to 1Password, run:
 `1password-secrets local push`
 
 ### Fly
 
 Make sure you have a Secure Note in 1Password with `fly:<fly-app-name>` in the title. `fly-app-name` is the name of your fly application.
```

### Comparing `1password-secrets-0.0.2/PKG-INFO` & `1password-secrets-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1password-secrets
-Version: 0.0.2
+Version: 0.0.3
 Summary: 1password-secrets is a set of utilities to sync 1Password secrets.
 Home-page: https://github.com/significa/fly-1password-secrets
 Author: Significa
 License: MIT
 Keywords: fly.io,1password,secrets
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -59,18 +59,18 @@
 
 `pip install 1password-secrets`
 
 ## Usage
 
 ### Local
 
-From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `get` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
+From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
 
 To get secrets from 1Password, run:
-`1password-secrets local get`
+`1password-secrets local pull`
 
 To push the local changes to 1Password, run:
 `1password-secrets local push`
 
 ### Fly
 
 Make sure you have a Secure Note in 1Password with `fly:<fly-app-name>` in the title. `fly-app-name` is the name of your fly application.
```

### Comparing `1password-secrets-0.0.2/README.md` & `1password-secrets-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 
 `pip install 1password-secrets`
 
 ## Usage
 
 ### Local
 
-From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `get` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
+From within a valid git repository with remote "origin" ending in `<owner>/<repo>.git`, 1password-secrets will be able to `pull` and `push` secrets to a 1password secure note containing `repo:<owner>/<repo>` in its name. By default it syncs to `./.env` file, this can overridden with a `file_name` field containing the desired relative file path.
 
 To get secrets from 1Password, run:
-`1password-secrets local get`
+`1password-secrets local pull`
 
 To push the local changes to 1Password, run:
 `1password-secrets local push`
 
 ### Fly
 
 Make sure you have a Secure Note in 1Password with `fly:<fly-app-name>` in the title. `fly-app-name` is the name of your fly application.
```

### Comparing `1password-secrets-0.0.2/onepassword_secrets.py` & `1password-secrets-0.0.3/onepassword_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
             f'do you wish to import secrets to the fly app {app_id} (y/n)?\n'
         )
 
     if user_input.lower() == 'y':
         import_1password_secrets_to_fly(app_id)
 
 
-def get_local_secrets():
+def pull_local_secrets():
     repository = get_git_repository_name_from_current_directory()
     item_id = get_1password_env_file_item_id(f'repo:{repository}')
 
     secrets = get_envs_from_1password(item_id)
 
     env_file_name = get_filename_from_1password(item_id) or DEFAULT_ENV_FILE_NAME
 
@@ -295,27 +295,27 @@
     subparsers = parser.add_subparsers(dest="subcommand", required=True)
 
     fly_parser = subparsers.add_parser('fly', help='manage fly secrets')
     fly_parser.add_argument('action', type=str, choices=['import', 'edit'])
     fly_parser.add_argument('app_name', type=str, help='fly application name')
 
     local_parser = subparsers.add_parser('local', help='manage local secrets')
-    local_parser.add_argument('action', type=str, choices=['get', 'push'])
+    local_parser.add_argument('action', type=str, choices=['pull', 'push'])
 
     args = parser.parse_args()
 
     try:
         if args.subcommand == 'fly':
             if args.action == 'import':
                 import_1password_secrets_to_fly(args.app_name)
             elif args.action == 'edit':
                 edit_1password_secrets(args.app_name)
         elif args.subcommand == 'local':
-            if args.action == 'get':
-                get_local_secrets()
+            if args.action == 'pull':
+                pull_local_secrets()
             elif args.action == 'push':
                 push_local_secrets()
     except Exception:
         sys.exit(1)
 
 
 if __name__ == '__main__':
```

### Comparing `1password-secrets-0.0.2/setup.py` & `1password-secrets-0.0.3/setup.py`

 * *Files identical despite different names*

