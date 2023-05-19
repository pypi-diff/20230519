# Comparing `tmp/copyright_claim-0.0.2.tar.gz` & `tmp/copyright_claim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyright_claim-0.0.2.tar", max compression
+gzip compressed data, was "copyright_claim-0.0.3.tar", max compression
```

## Comparing `copyright_claim-0.0.2.tar` & `copyright_claim-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2553 2023-05-19 18:02:58.062746 copyright_claim-0.0.2/README.md
--rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.2/copyright_claim/__init__.py
--rw-r--r--   0        0        0     8128 2023-05-19 17:36:55.654300 copyright_claim-0.0.2/copyright_claim/copyright_claim.py
--rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.2/copyright_claim/dummy_copyright_claim.txt
--rw-r--r--   0        0        0      535 2023-05-19 18:04:07.114981 copyright_claim-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 copyright_claim-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3738 2023-05-19 18:13:40.488333 copyright_claim-0.0.3/README.md
+-rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.3/copyright_claim/__init__.py
+-rw-r--r--   0        0        0     8128 2023-05-19 17:36:55.654300 copyright_claim-0.0.3/copyright_claim/copyright_claim.py
+-rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.3/copyright_claim/dummy_copyright_claim.txt
+-rw-r--r--   0        0        0      535 2023-05-19 18:19:52.664903 copyright_claim-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 copyright_claim-0.0.3/PKG-INFO
```

### Comparing `copyright_claim-0.0.2/README.md` & `copyright_claim-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -36,31 +36,56 @@
 
 you can run 
 ```
 $ copyright-claim -h
 ```
 in your terminal and observe
 ```
-usage: copyright_claim [-h] [--claim_path CLAIM_PATH] [-r] [--extension EXTENSION] [--comment_symbol COMMENT_SYMBOL] {add,remove} project_path
+usage: copyright_claim [-h] [--project_path PROJECT_PATH]
+                       [--claim_path CLAIM_PATH] [-r] [--ext EXT]
+                       [--comment_symbol COMMENT_SYMBOL]
+                       [--start_string START_STRING] [--end_string END_STRING]
+                       {add,remove,dummy}
 
 Adds and removes copyright claims at the beginning of text files.
 
 positional arguments:
-  {add,remove}          Choose "add" if you want to add the claim, "remove" if you want to remove it.
-  project_path          The path to the file or directory to be treated.
+  {add,remove,dummy}    Choose "add" if you want to add the claim, "remove" if
+                        you want to remove it. The "dummy" option simply
+                        outputs our dummy example of a copyright claim.
 
 options:
   -h, --help            show this help message and exit
+  --project_path PROJECT_PATH, -p PROJECT_PATH
+                        The path to the file or directory to be treated. It is
+                        a compulsory argument, unless the 'dummy' option is
+                        being used
   --claim_path CLAIM_PATH, -c CLAIM_PATH
-                        In case the add option is used, this argument is necessary. Useless otherwise.
-  -r                    This flag must be used when treating a directory is desired. In this case all the file within the directory and its subdirectories will be affected, provided they have the chosen extension.
-  --extension EXTENSION, -e EXTENSION
-                        The extension that characterizes the file(s) to be treated. Defaults to ".py". When processing a single file, this argument is ignored.
+                        The path to the text of your copyright claim. In case
+                        the add option is used, this argument is necessary.
+                        Useless otherwise. For testing purposes you can use
+                        the special value 'dummy' which allows to use our
+                        dummy copyright claim.
+  -r                    This flag must be used when treating a directory is
+                        desired. In this case all the file within the
+                        directory and its subdirectories will be affected,
+                        provided they have the chosen extension.
+  --ext EXT             The extension that characterizes the file(s) to be
+                        treated. Defaults to ".py". When processing a single
+                        file, this argument is ignored.
   --comment_symbol COMMENT_SYMBOL
-                        The string to be used to comment out the lines of the claim block. Defaults to '# '.
+                        The string to be used to comment out the lines of the
+                        claim block. Defaults to '# '.
+  --start_string START_STRING, -s START_STRING
+                        The string that marks the beginning of the copyright
+                        claim block. Defaults to "COPYRIGHT CLAIM".
+  --end_string END_STRING, -e END_STRING
+                        The string that marks the beginning of the copyright
+                        claim block. Defaults to "END OF COPYRIGHT CLAIM".
+
 ```
 
 
 
 ## Further developments of the project
 
 Feel free to open the discussion through issues and pull requests on the [GitHub repository](https://github.com/completementgaga/copyright-claim).
```

### Comparing `copyright_claim-0.0.2/copyright_claim/copyright_claim.py` & `copyright_claim-0.0.3/copyright_claim/copyright_claim.py`

 * *Files identical despite different names*

### Comparing `copyright_claim-0.0.2/pyproject.toml` & `copyright_claim-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copyright-claim"
-version = "0.0.2"
+version = "0.0.3"
 description = "Adds and removes copyright claims at the beginning of text files."
 authors = ["Gaël Cousin <gcousin333@gmail.com>"]
 license = "BSD-2-Clause License"
 readme = "README.md"
 packages = [{include = "copyright_claim"}]
 
 [tool.poetry.dependencies]
```

### Comparing `copyright_claim-0.0.2/PKG-INFO` & `copyright_claim-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyright-claim
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adds and removes copyright claims at the beginning of text files.
 License: BSD-2-Clause License
 Author: Gaël Cousin
 Author-email: gcousin333@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -53,31 +53,56 @@
 
 you can run 
 ```
 $ copyright-claim -h
 ```
 in your terminal and observe
 ```
-usage: copyright_claim [-h] [--claim_path CLAIM_PATH] [-r] [--extension EXTENSION] [--comment_symbol COMMENT_SYMBOL] {add,remove} project_path
+usage: copyright_claim [-h] [--project_path PROJECT_PATH]
+                       [--claim_path CLAIM_PATH] [-r] [--ext EXT]
+                       [--comment_symbol COMMENT_SYMBOL]
+                       [--start_string START_STRING] [--end_string END_STRING]
+                       {add,remove,dummy}
 
 Adds and removes copyright claims at the beginning of text files.
 
 positional arguments:
-  {add,remove}          Choose "add" if you want to add the claim, "remove" if you want to remove it.
-  project_path          The path to the file or directory to be treated.
+  {add,remove,dummy}    Choose "add" if you want to add the claim, "remove" if
+                        you want to remove it. The "dummy" option simply
+                        outputs our dummy example of a copyright claim.
 
 options:
   -h, --help            show this help message and exit
+  --project_path PROJECT_PATH, -p PROJECT_PATH
+                        The path to the file or directory to be treated. It is
+                        a compulsory argument, unless the 'dummy' option is
+                        being used
   --claim_path CLAIM_PATH, -c CLAIM_PATH
-                        In case the add option is used, this argument is necessary. Useless otherwise.
-  -r                    This flag must be used when treating a directory is desired. In this case all the file within the directory and its subdirectories will be affected, provided they have the chosen extension.
-  --extension EXTENSION, -e EXTENSION
-                        The extension that characterizes the file(s) to be treated. Defaults to ".py". When processing a single file, this argument is ignored.
+                        The path to the text of your copyright claim. In case
+                        the add option is used, this argument is necessary.
+                        Useless otherwise. For testing purposes you can use
+                        the special value 'dummy' which allows to use our
+                        dummy copyright claim.
+  -r                    This flag must be used when treating a directory is
+                        desired. In this case all the file within the
+                        directory and its subdirectories will be affected,
+                        provided they have the chosen extension.
+  --ext EXT             The extension that characterizes the file(s) to be
+                        treated. Defaults to ".py". When processing a single
+                        file, this argument is ignored.
   --comment_symbol COMMENT_SYMBOL
-                        The string to be used to comment out the lines of the claim block. Defaults to '# '.
+                        The string to be used to comment out the lines of the
+                        claim block. Defaults to '# '.
+  --start_string START_STRING, -s START_STRING
+                        The string that marks the beginning of the copyright
+                        claim block. Defaults to "COPYRIGHT CLAIM".
+  --end_string END_STRING, -e END_STRING
+                        The string that marks the beginning of the copyright
+                        claim block. Defaults to "END OF COPYRIGHT CLAIM".
+
 ```
 
 
 
 ## Further developments of the project
 
 Feel free to open the discussion through issues and pull requests on the [GitHub repository](https://github.com/completementgaga/copyright-claim).
```

