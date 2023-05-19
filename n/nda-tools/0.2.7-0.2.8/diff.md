# Comparing `tmp/nda_tools-0.2.7.tar.gz` & `tmp/nda_tools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nda_tools-0.2.7.tar", last modified: Tue Jul 20 16:52:43 2021, max compression
+gzip compressed data, was "dist/nda_tools-0.2.8.tar", last modified: Fri Sep  3 14:02:02 2021, max compression
```

## Comparing `nda_tools-0.2.7.tar` & `nda_tools-0.2.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/NDATools/
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/NDATools/clientscripts/
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/NDATools/clientscripts/config/
--rw-r-----   0 bamboo    (1001) bamboo    (1001)      569 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/clientscripts/config/settings.cfg
--rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/clientscripts/__init__.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     4769 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/clientscripts/downloadcmd.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    13824 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/clientscripts/vtcmd.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    16803 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/BuildPackage.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     5539 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/Configuration.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)      881 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/DataManager.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    17399 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/Download.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     4311 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/MultiPartUploads.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     1743 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/S3Authentication.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    32976 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/Submission.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     4413 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/TokenGenerator.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     7584 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/Utils.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    16937 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/Validation.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     1392 2021-07-20 16:52:42.000000 nda_tools-0.2.7/NDATools/__init__.py
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    12290 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/PKG-INFO
--rw-r-----   0 bamboo    (1001) bamboo    (1001)      970 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/SOURCES.txt
--rw-r-----   0 bamboo    (1001) bamboo    (1001)        1 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/dependency_links.txt
--rw-r-----   0 bamboo    (1001) bamboo    (1001)      207 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/entry_points.txt
--rw-r-----   0 bamboo    (1001) bamboo    (1001)       74 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/requires.txt
--rw-r-----   0 bamboo    (1001) bamboo    (1001)       15 2021-07-20 16:52:43.000000 nda_tools-0.2.7/nda_tools.egg-info/top_level.txt
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/
-drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/integration_tests/
--rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:42.000000 nda_tools-0.2.7/tests/integration_tests/__init__.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     1388 2021-07-20 16:52:42.000000 nda_tools-0.2.7/tests/integration_tests/test_build_package.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     6791 2021-07-20 16:52:42.000000 nda_tools-0.2.7/tests/integration_tests/test_configuration.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     2505 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/integration_tests/test_submission.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     3602 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/integration_tests/test_validation.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-07-20 16:52:42.000000 nda_tools-0.2.7/tests/__init__.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     1388 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/test_build_package.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     6791 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/test_configuration.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     2505 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/test_submission.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)     3600 2021-07-20 16:52:43.000000 nda_tools-0.2.7/tests/test_validation.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    10329 2021-07-20 16:52:42.000000 nda_tools-0.2.7/README.md
--rwxr-x--x   0 bamboo    (1001) bamboo    (1001)     1177 2021-07-20 16:52:42.000000 nda_tools-0.2.7/setup.py
--rw-r-----   0 bamboo    (1001) bamboo    (1001)    12290 2021-07-20 16:52:43.000000 nda_tools-0.2.7/PKG-INFO
--rw-r-----   0 bamboo    (1001) bamboo    (1001)       38 2021-07-20 16:52:43.000000 nda_tools-0.2.7/setup.cfg
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/config/
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)      569 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/config/settings.cfg
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/__init__.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     4615 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/downloadcmd.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    13824 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/clientscripts/vtcmd.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    16803 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/BuildPackage.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     5539 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/Configuration.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)      881 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/DataManager.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    21809 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/Download.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     4311 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/MultiPartUploads.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     1743 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/S3Authentication.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    32976 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/Submission.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     4413 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/TokenGenerator.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     8122 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/Utils.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    16937 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/Validation.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     1392 2021-09-03 14:02:02.000000 nda_tools-0.2.8/NDATools/__init__.py
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    12290 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/PKG-INFO
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)      970 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/SOURCES.txt
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)        1 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/dependency_links.txt
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)      207 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/entry_points.txt
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)       74 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/requires.txt
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)       15 2021-09-03 14:02:02.000000 nda_tools-0.2.8/nda_tools.egg-info/top_level.txt
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/
+drwxr-x---   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/__init__.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     1388 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/test_build_package.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     6791 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/test_configuration.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     2505 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/test_submission.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     3602 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/integration_tests/test_validation.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)        0 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/__init__.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     1388 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/test_build_package.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     6791 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/test_configuration.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     2505 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/test_submission.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)     3600 2021-09-03 14:02:02.000000 nda_tools-0.2.8/tests/test_validation.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    10329 2021-09-03 14:02:02.000000 nda_tools-0.2.8/README.md
+-rwxr-x--x   0 bamboo    (1001) bamboo    (1001)     1177 2021-09-03 14:02:02.000000 nda_tools-0.2.8/setup.py
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)    12290 2021-09-03 14:02:02.000000 nda_tools-0.2.8/PKG-INFO
+-rw-r-----   0 bamboo    (1001) bamboo    (1001)       38 2021-09-03 14:02:02.000000 nda_tools-0.2.8/setup.cfg
```

### Comparing `nda_tools-0.2.7/NDATools/clientscripts/config/settings.cfg` & `nda_tools-0.2.8/NDATools/clientscripts/config/settings.cfg`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/clientscripts/downloadcmd.py` & `nda_tools-0.2.8/NDATools/clientscripts/downloadcmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,37 +45,38 @@
 
     parser.add_argument('-d', '--directory', metavar='<arg>', type=str, nargs=1, action='store',
                         help='Enter an alternate full directory path where you would like your files to be saved.')
 
     parser.add_argument('-wt', '--workerThreads', metavar='<arg>', type=int, action='store',
                         help='Number of worker threads')
 
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Option to print out more detailed messages as the program runs.')
+    parser.add_argument('-q', '--quiet', action='store_true',
+                        help='Option to suppress output of detailed messages as the program runs.')
 
     args = parser.parse_args()
 
     return args
 
 
-def configure(username=None, password=None):
+def configure(args):
 
     NDATools.Utils.logging.getLogger().setLevel(logging.INFO)
     if os.path.isfile(os.path.join(os.path.expanduser('~'), '.NDATools/settings.cfg')):
-        config = ClientConfiguration(os.path.join(os.path.expanduser('~'), '.NDATools/settings.cfg'), username, password)
+        config = ClientConfiguration(os.path.join(os.path.expanduser('~'), '.NDATools/settings.cfg'), args.username, args.password)
     else:
-        config = ClientConfiguration('clientscripts/config/settings.cfg', username, password)
+        config = ClientConfiguration('clientscripts/config/settings.cfg', args.username, args.password)
         config.read_user_credentials()
         config.make_config()
+
     return config
 
 
 def main():
     args = parse_args()
-    config = configure(args.username, args.password)
+    config = configure(args)
 
     # directory where files will be downloaded
     if args.directory:
         dir = args.directory[0]
     elif args.resume:
         dir = args.resume[0]
     else:
@@ -97,20 +98,14 @@
         paths = args.datastructure
     elif args.paths:
         links = 'paths'
         paths = args.paths
     else:  # only package provided
         links = 'package'
 
-    s3Download = Download(dir, config, verbose=args.verbose)
+    s3Download = Download(dir, config, quiet=args.quiet)
     s3Download.get_links(links, paths, args.package, filters=None)
-
-    if len(s3Download.s3_links) == 0:
-        return
     s3Download.start_workers(args.resume, dir, args.workerThreads)
 
-    if args.verbose:
-        print('Finished downloading all files.')
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `nda_tools-0.2.7/NDATools/clientscripts/vtcmd.py` & `nda_tools-0.2.8/NDATools/clientscripts/vtcmd.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/BuildPackage.py` & `nda_tools-0.2.8/NDATools/BuildPackage.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/Configuration.py` & `nda_tools-0.2.8/NDATools/Configuration.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/DataManager.py` & `nda_tools-0.2.8/NDATools/DataManager.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/Download.py` & `nda_tools-0.2.8/NDATools/Download.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import absolute_import
 from __future__ import with_statement
 
+import datetime
 import sys
 
 from requests import HTTPError
 
 IS_PY2 = sys.version_info < (3, 0)
 
 if IS_PY2:
@@ -15,14 +16,15 @@
 import csv
 from threading import Thread
 import botocore
 import multiprocessing
 from NDATools.Utils import *
 import requests
 
+
 class Worker(Thread):
     """ Thread executing tasks from a given tasks queue """
 
     def __init__(self, tasks):
         Thread.__init__(self)
         self.tasks = tasks
         self.daemon = True
@@ -41,15 +43,15 @@
                 self.tasks.task_done()
 
 
 class ThreadPool:
     """ Pool of threads consuming tasks from a queue """
 
     def __init__(self, num_threads):
-        self.tasks = Queue(num_threads)
+        self.tasks = Queue(num_threads * 100)
         for _ in range(num_threads):
             Worker(self.tasks)
 
     def add_task(self, func, *args, **kargs):
         """ Add a task to the queue """
         self.tasks.put((func, args, kargs))
 
@@ -61,145 +63,120 @@
     def wait_completion(self):
         """ Wait for completion of all the tasks in the queue """
         self.tasks.join()
 
 
 class Download(Protocol):
 
-    def __init__(self, directory, config=None, verbose=False):
+    def __init__(self, directory, config=None, quiet=False):
         if config:
             self.config = config
         else:
             self.config = ClientConfiguration()
         self.url = self.config.datamanager_api  # todo: delete me
         self.package_url = self.config.package_api
         self.datadictionary_url = self.config.datadictionary_api
         self.username = config.username
         self.password = config.password
         self.directory = directory
         self.download_queue = Queue()
-        self.path_list = set()
         self.local_file_names = {}
         self.access_key = None
         self.secret_key = None
         self.session = None
         self.associated_files = False
         self.dsList = []
-        self.verbose = verbose
+        self.quiet = quiet
         self.s3_links = {}
         self.package_file_id_list = set()
         self.package_file_download_errors = set()
+        self.download_all_files_flg = False
+        self.auth = requests.auth.HTTPBasicAuth(self.config.username, self.config.password)
 
     @staticmethod
     def get_protocol(cls):
         return cls.XML
 
+    @staticmethod
+    def request_header():
+        return {'content-type': 'application/json'}
+
     def verbose_print(self, *args):
-        if self.verbose:
+        if not self.quiet:
             print(' '.join(list(args)))
 
-    def get_presigned_urls(self):
-        """ Download package files (not associated files) """
-        auth = requests.auth.HTTPBasicAuth(self.config.username, self.config.password)
-        headers = {'content-type': 'application/json'}
-        url = self.package_url + '/{}/files?page=1&size=all'.format(self.package)
-        tmp = requests.get(url, headers, auth=auth)
-        tmp.raise_for_status()
-        response = json.loads(tmp.text)
-
-        for element in response['results']:
-            associated = element['associatedFile']
-            # if not associated:  # Does not loaded associated files
-            alias = element['download_alias']
-            package_file_id = element['package_file_id']
-            self.package_file_id_list.add(package_file_id)
-            self.local_file_names[package_file_id] = alias
-
-        logging.debug("Generating download links...")
-        self.__chunk_file_id_list()
-
-    def __chunk_file_id_list(self):
-        """
-        Chunk requests due to max batch size 0f 50,000. Subsequently calls __post_for_s3_links to get presigned urls.
-        """
-        self.package_file_id_list = list(self.package_file_id_list)  # Convert set to list
-        auth = requests.auth.HTTPBasicAuth(self.config.username, self.config.password)
-        headers = {'content-type': 'application/json'}
-        max_batch_size = 50000
-        if len(self.package_file_id_list) > max_batch_size:
-            chunks = [self.package_file_id_list[i:i + max_batch_size] for i in
-                      range(0, len(self.package_file_id_list), max_batch_size)]
-            for chunk in chunks:
-                self.__post_for_s3_links(chunk, auth, headers)
-        else:
-            self.__post_for_s3_links(self.package_file_id_list, auth, headers)
-
-        self.verbose_print('Downloading package files for package {}.'.format(self.package))
-
-    def __post_for_s3_links(self, id_list, auth, headers):
+    def get_presigned_urls(self, id_list):
         """
         Stores key-value pairs of (key: package_file_id, value: presigned URL)
         :param id_list: List of package file IDs with max size of 50,000
         """
-        url = self.package_url + '/{}/files/batchGeneratePresignedUrls'.format(self.package)
-        tmp = requests.post(url, headers=headers, json=id_list, auth=auth)
-        tmp.raise_for_status()
-        response = json.loads(tmp.text)
+        if len(id_list) == 1:
+            file_id = id_list[0]
+            url = self.package_url + '/{}/files/{}/download_url'.format(self.package, file_id)
+            tmp = requests.get(url, headers=self.request_header(), json=id_list, auth=self.auth)
+            tmp.raise_for_status()
+            response = json.loads(tmp.text)
+            return response['downloadURL']
+        else:
+            # Use the batchGeneratePresignedUrls when retrieving multiple files
+            self.verbose_print('Retrieving credentials for {} files'.format(len(id_list)))
+            url = self.package_url + '/{}/files/batchGeneratePresignedUrls'.format(self.package)
+            tmp = requests.post(url, headers=self.request_header(), json=id_list, auth=self.auth)
+            tmp.raise_for_status()
+            response = json.loads(tmp.text)
+
+            creds = {e['package_file_id']: e['downloadURL'] for e in response['presignedUrls']}
+            self.verbose_print('Finished retrieving credentials')
+            return creds
 
-        for element in response['presignedUrls']:
-            download_url = element['downloadURL']
-            package_file_id = element['package_file_id']
-            self.s3_links[package_file_id] = download_url
 
     def use_s3_links_file(self):
         """
         Reads a text file line by line, collects all S3 URLs, and requests the package file ids
         from the package service for those files.
         """
+        path_list = set()
         try:
             with open(self.dataStructure, 'r', encoding='utf-8') as s3_links_file:
                 for line in s3_links_file:
                     if line.startswith('s3://'):
-                        self.path_list.add(line.strip())
-            self.get_package_file_ids()
+                        path_list.add(line.strip())
+            self.get_package_file_ids(path_list)
         except IOError as e:
             self.verbose_print(
                 '{} not found. Please enter the correct path to your file and try again.'.format(self.dataStructure))
             raise e
 
+
     def use_data_structure(self):
         """
         Downloads a data structure file from the package, the data_structure_manifest file,
         parses both files to identify all associated files for the data structure, and then
         requests the package file ids for those files from the package service
         """
         data_structure_name = self.dataStructure.split(os.path.sep)[-1].split('.txt')[0]
-        auth = requests.auth.HTTPBasicAuth(self.config.username, self.config.password)
-        headers = {'content-type': 'application/json'}
-        url = self.package_url + '/{}/files?page=1&size=all&types=Data'.format(self.package)
-        tmp = requests.get(url, headers, auth=auth)
+        url = self.package_url + '/{}/files?page=1&size=all&types=Package%20Metadata&types=Data'.format(self.package)
+        tmp = requests.get(url, self.request_header(), auth=self.auth)
         tmp.raise_for_status()
         response = json.loads(tmp.text)
         has_data_structure = False
         has_data_structure_manifest = False
         for element in response['results']:
             # api response is always lower-case
             if data_structure_name.lower() == element['download_alias'].split('.txt')[0]:
                 pfi = list()
                 pfi.append(element['package_file_id'])
-                self.__post_for_s3_links(pfi, auth, headers)
                 self.local_file_names[element['package_file_id']] = element['download_alias']
-                self.download_from_s3link(element['package_file_id'], True, self.directory)
+                self.download_from_s3link(element['package_file_id'], True, self.directory, err_if_exists=True)
                 has_data_structure = True
             if element['download_alias'] == 'datastructure_manifest.txt':
                 pfi = list()
                 pfi.append(element['package_file_id'])
-                self.__post_for_s3_links(pfi, auth, headers)
                 self.local_file_names[element['package_file_id']] = element['download_alias']
-                self.download_from_s3link(element['package_file_id'], True, self.directory)
+                self.download_from_s3link(element['package_file_id'], True, self.directory, err_if_exists=True)
                 has_data_structure_manifest = True
             if has_data_structure_manifest and has_data_structure:
                 break
         if not has_data_structure:
             structures = [f['download_alias'].replace('.txt', '') for f in response['results'] if
                           f['nda_file_type'] == 'Data']
             structures.sort()
@@ -246,147 +223,265 @@
             with open(os.path.normpath(os.path.join(self.directory, 'datastructure_manifest.txt'))) as \
                     data_structure_manifest:
                 reader = csv.DictReader(data_structure_manifest, dialect='excel-tab')
                 for row in reader:
                     if row['dataset_id'] in manifest_names:
                         if row['manifest_name'] in manifest_names[row['dataset_id']]:
                             data_structure_manifest_file_links.add(row['associated_file'])
+        path_list = set()
+        path_list.update(data_structure_file_links)
+        path_list.update(data_structure_manifest_file_links)
+        if len(path_list) > 0:
+            self.get_package_file_ids(path_list)
 
-        self.path_list.update(data_structure_file_links)
-        self.path_list.update(data_structure_manifest_file_links)
-        if len(self.path_list) > 0:
-            self.get_package_file_ids()
-
-    def get_package_file_ids(self):
-        self.verbose_print('Requesting files from package: {}'.format(self.package))
-        auth = requests.auth.HTTPBasicAuth(self.config.username, self.config.password)
+    def get_package_file_ids(self, path_list):
         url = self.package_url + '/{}/files'.format(self.package)
         try:
-            response = requests.post(url, auth=auth, json=list(self.path_list))
+            response = requests.post(url, auth=self.auth, json=list(path_list))
             response.raise_for_status()
             for package_file in response.json():
                 self.package_file_id_list.add(package_file['package_file_id'])
                 self.local_file_names[package_file['package_file_id']] = package_file['download_alias']
         except HTTPError as e:
             if e.response.status_code == 404:
                 message = e.response.text
                 invalid_s3_links = set(map(lambda x: x.rstrip(), message.split('\n')[1:]))
                 print('WARNING: The following associated files were not found in the package '
                       'and will not be downloaded\n{}'.format('\n'.join(invalid_s3_links)))
                 print()
                 for i in invalid_s3_links:
-                    self.path_list.remove(i)
+                    path_list.remove(i)
 
-                if not self.path_list:
-                    print('Error detected in package config. Please contact NDAHelp@mail.nih.gov for assistance in resolving this error.')
-                    print('Please note - this error may be encountered if you did not select the "include associated files" '
+                if not path_list:
+                    print('All files requested for download were invalid.')
+                    print('This error may be encountered if you did not select the "include associated files" '
                           'option when before your data package. If you wish to download associated files, you will need to create a new '
                           'package')
+                    print(
+                        'If you are sure you created your package with this option selected, please contact NDAHelp@mail.nih.gov '
+                        'for assistance in resolving this error.')
                     sys.exit(1)
                 else:
-                    self.get_package_file_ids() # retry request after excluding the invalid s3links
+                    self.get_package_file_ids(path_list)  # retry request after excluding the invalid s3links
                     return
             else:
                 raise e
 
-        self.__chunk_file_id_list()
 
     def get_links(self, links, files, package, filters=None):
         self.package = package
         if links == 'datastructure':
-            self.verbose_print('Downloading S3 links from a data structure (i.e., image03): {}'.format(files))
+            self.verbose_print('Downloading S3 links from data structure: {}'.format(files))
             self.dataStructure = files
-            self.use_data_structure()
+            self.use_data_structure()  # path list to package-file-ids+file-paths to presigned-urls
         elif links == 'text':
             self.verbose_print('Downloading S3 links from text file: {}'.format(files))
             self.dataStructure = files
             self.use_s3_links_file()
         elif links == 'package':
             self.verbose_print('Downloading all files from package with id: {}'.format(package))
-            self.get_presigned_urls()
+            self.download_all_files_flg = True
+            # self.get_all_files_in_package() # package-ids+file-paths directly to presigned-urls
         else:
-            self.path_list = files
-            self.get_package_file_ids()
+            self.get_package_file_ids(files)
+
 
-    def download_from_s3link(self, package_file_id, resume, prev_directory):
+    def download_from_s3link(self, package_file_id, resume, prev_directory, err_if_exists=False):
 
         # use this instead of exists_ok in order to work with python v.2
         def mk_dir_ignore_err(dir):
             try:
                 os.makedirs(os.path.normpath(dir))
+            except FileExistsError as e:
+                pass
             except OSError as e:
                 # Raise exception for any errors other than FileExists error
-                # Using OSError over FileExistsError for version compatibility
+                # Using OSError for version compatibility
                 if e.errno != 17:
                     raise
                 pass
 
-        s3_link = self.s3_links[package_file_id]
         alias = self.local_file_names[package_file_id]
         completed_download = os.path.normpath(os.path.join(self.directory, alias))
         partial_download = os.path.normpath(
             os.path.join(prev_directory, alias + '.partial'))
         downloaded = False
         resume_header = None
+        bytes_written = 0
 
         if os.path.isfile(completed_download):
-            return
+            if err_if_exists:
+                msg= "File {} already exists. Move or rename the file before re-running the command to continue".format(completed_download)
+                print(msg)
+                print('Exiting...')
+                sys.exit(1)
+
+            self.verbose_print('Skipping download (already exists): {}'.format(completed_download))
+            return bytes_written
 
         if os.path.isfile(partial_download):
             downloaded = True
             downloaded_size = os.path.getsize(partial_download)
             resume_header = {'Range': 'bytes={}-'.format(downloaded_size)}
-            download_file = open(partial_download, "ab")
             self.verbose_print('Resuming download: {}'.
                                format(partial_download))
-        if not downloaded:
+        else:
             mk_dir_ignore_err(os.path.dirname(partial_download))
-            download_file = open(partial_download, "wb")
             self.verbose_print('Starting download: {}'.format(partial_download))
 
+        s3_link = self.get_presigned_urls([package_file_id])
+
         try:
             s = requests.session()
             if resume_header:
                 s.headers.update(resume_header)
-            with s.get(s3_link, stream=True) as response:
-                for chunk in response.iter_content(chunk_size=512 * 1024):
-                    if chunk:
-                        download_file.write(chunk)
-            download_file.close()
-            try:
-                os.rename(partial_download, completed_download)
-            except WindowsError:
-                os.remove(completed_download)
-                os.rename(partial_download, completed_download)
+            with open(partial_download, "ab" if downloaded else "wb") as download_file:
+                with s.get(s3_link, stream=True) as response:
+                    for chunk in response.iter_content(chunk_size=512 * 1024):
+                        if chunk:
+                            bytes_written += download_file.write(chunk)
+            os.rename(partial_download, completed_download)
             self.verbose_print('Completed download {}'.format(completed_download))
-        # except botocore.exceptions.ClientError as e:
+            return bytes_written
         except Exception as e:
             # If a client error is thrown, then check that it was a 404 error.
             # If it was a 404 error, then the bucket does not exist.
             self.package_file_download_errors.add(package_file_id)
-            error_code = int(e.response['Error']['Code'])
+            error_code = -1 if not isinstance(e, HTTPError) else int(e.response['Error']['Code'])
             if error_code == 404:
                 message = 'This path is incorrect: {}. Please try again.'.format(s3_link)
                 self.verbose_print(message)
                 raise Exception(e)
-            if error_code == 403:
+            elif error_code == 403:
                 message = '\nThis is a private bucket. Please contact NDAR for help: {}'.format(s3_link)
                 self.verbose_print(message)
                 raise Exception(e)
+            else:
+                self.verbose_print(str(e))
+                self.verbose_print(get_traceback())
+            return 0
+
 
     def start_workers(self, resume, prev_directory, thread_num=None):
+        success_files = set()
+        download_request_count = 0
+        download_start_date = datetime.datetime.now()
+
+        # These are all arrays just so that the print_download_progress_report method can update the variables inside them
+        trailing_50_file_bytes = []
+        trailing_50_timestamp = [datetime.datetime.now()]
+
+        def print_download_progress_report(num_downloaded):
+            self.verbose_print()
+            byte_total = sum(trailing_50_file_bytes)
+            download_progress_message = 'Download Progress Report [{}] - {}/{} files downloaded so far. ' \
+                .format(datetime.datetime.now().strftime('%b %d %Y %H:%M:%S'), num_downloaded, download_request_count)
+            download_progress_message += 'Last 50 files contained ~ {} bytes and finished in {} (Hours:Minutes:Seconds). ' \
+                .format(byte_total, str(datetime.datetime.now() - trailing_50_timestamp[0]).split('.')[0])
+
+            seconds_last_50_files = (datetime.datetime.now() - trailing_50_timestamp[0]).seconds
+            if seconds_last_50_files == 0:
+                seconds_last_50_files = 1 # avoid a 'division by 0' error
+            download_progress_message += ' Avg download rate for the last 50 files is ~ {} bytes/sec.' \
+                .format(byte_total // seconds_last_50_files)
+
+            download_progress_message += ' Download has been in progress for {} (Hours:Minutes:Seconds).' \
+                .format(str(datetime.datetime.now() - download_start_date).split('.')[0])
+
+            self.verbose_print(download_progress_message)
+            trailing_50_file_bytes.clear()
+            trailing_50_timestamp[0] = datetime.datetime.now()
+            self.verbose_print()
+
         def download(package_file_id):
-            self.download_from_s3link(package_file_id, resume, prev_directory)
+            # check if  these exist, and if not, get and set:
+            trailing_50_file_bytes.append(self.download_from_s3link(package_file_id, resume, prev_directory))
+            success_files.add(package_file_id)
+            num_downloaded = len(success_files)
+
+            if num_downloaded % 50 == 0:
+                print_download_progress_report(num_downloaded)
+
 
         # Instantiate a thread pool with i worker threads
         self.thread_num = max([1, multiprocessing.cpu_count() - 1])
         if thread_num:
             self.thread_num = thread_num
+        else:
+            self.verbose_print()
+            self.verbose_print('WARNING: No value specified for --workerThreads. Using the default option of {}'.format(
+                self.thread_num))
+            self.verbose_print(
+                'You should configure the thread count setting using the --workerThreads argument to maximize your download speed.')
+            self.verbose_print()
 
         pool = ThreadPool(self.thread_num)
 
-        # Add the jobs in bulk to the thread pool
-        pool.map(download, self.package_file_id_list)
-        print('Beginning download of {} files to {}'.format(len(self.package_file_id_list), self.directory))
+        print('Beginning download of files to {} using {} threads'.format(self.directory, self.thread_num))
+
+        for package_file_id_list in self.generate_download_batch_file_ids():
+            additional_file_ct = len(package_file_id_list)
+            download_request_count += additional_file_ct
+            self.verbose_print('Adding {} files to download queue. Queue contains {} files'.format(additional_file_ct,
+                                                                                                   download_request_count))
+            pool.map(download, package_file_id_list)
+
         pool.wait_completion()
-        print('Finished processing download requests for {} files. Total errors encountered: {}'
-              .format(len(self.package_file_id_list), len(self.package_file_download_errors)))
+
+        print()
+
+        print('Finished processing all download requests @ {}.'.format(datetime.datetime.now()))
+        print('     Total download requests {}'
+              .format(download_request_count))
+        print('     Total errors encountered: {}'.format(len(self.package_file_download_errors)))
+        print(' Exiting Program...')
+
+    def get_package_files_by_page(self, page, batch_size):
+
+        url = self.package_url + '/{}/files?page={}&size={}'.format(self.package, page, batch_size)
+        aliases = {}
+        package_file_ids = set()
+        try:
+            tmp = requests.get(url, self.request_header(), auth=self.auth)
+            tmp.raise_for_status()
+            response = json.loads(tmp.text)
+
+            for element in response['results']:
+                associated = element['associatedFile']
+                # if not associated:  # Does not loaded associated files
+                alias = element['download_alias']
+                package_file_id = element['package_file_id']
+                package_file_ids.add(package_file_id)
+                aliases[package_file_id] = alias
+            return aliases, package_file_ids
+
+        except HTTPError as e:
+            if 'Cannot navigate past last page' in e.response.text:
+                # empty alias and package-file return means there are no files for given page parameter
+                return aliases, package_file_ids
+            else:
+                raise e
+        except Exception as e:
+            raise e
+
+    def generate_download_batch_file_ids(self):
+        batch_size = 50  # arbitrary number of files to add to job queue at once.
+
+        if self.download_all_files_flg:
+            #  write generator function that goes through each page in file listing
+            #  and yields file-ids for files in package. Before returning, self.local_file_path must be set
+            page = 1
+            while True:
+                aliases, package_file_ids = self.get_package_files_by_page(page, batch_size)
+                self.local_file_names.update(aliases)
+                self.package_file_id_list.update(package_file_ids)
+                page += 1
+                if not package_file_ids:
+                    break
+
+                yield package_file_ids
+
+        else:
+            package_file_list = list(self.package_file_id_list)
+            batches = [package_file_list[i:i + batch_size] for i in range(0, len(package_file_list), batch_size)]
+            for batch in batches:
+                yield batch
```

### Comparing `nda_tools-0.2.7/NDATools/MultiPartUploads.py` & `nda_tools-0.2.8/NDATools/MultiPartUploads.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/S3Authentication.py` & `nda_tools-0.2.8/NDATools/S3Authentication.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/Submission.py` & `nda_tools-0.2.8/NDATools/Submission.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/TokenGenerator.py` & `nda_tools-0.2.8/NDATools/TokenGenerator.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/Utils.py` & `nda_tools-0.2.8/NDATools/Utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from __future__ import absolute_import
 import re
 import signal
 import sys
 import getpass
 import time
 import threading
+import traceback
+
 import requests
 from requests.adapters import HTTPAdapter
 import requests.packages.urllib3.util
 import json
 import signal
 import os
 import logging
@@ -34,25 +36,26 @@
     import thread
 else:
     import configparser
     import _thread as thread
 
 import xml.etree.ElementTree as ET
 
+
 class Protocol(object):
     CSV = "csv"
     XML = "xml"
     JSON = "json"
 
     @staticmethod
     def get_protocol(cls):
         return cls.JSON
 
-def api_request(api, verb, endpoint, data=None, session=None):
 
+def api_request(api, verb, endpoint, data=None, session=None):
     retry = requests.packages.urllib3.util.retry.Retry(
         total=20,
         read=20,
         connect=20,
         backoff_factor=3,
         status_forcelist=(400, 403, 404, 500, 502, 504)
     )
@@ -150,19 +153,19 @@
     :param no_match: Stores list of invalid paths
     :param full_file_path: Dictionary of tuples that store full filepath and file size
     :param no_read_access: List of files that user does not have access to
     :return: Modifies references to no_match, full_file_path, no_read_access
     """
     files_to_match = len(no_match)
     logging.debug('Starting local directory search for {} files'.format(str(files_to_match)))
-    progress_counter = int(files_to_match*0.05)
+    progress_counter = int(files_to_match * 0.05)
     for file in no_match[:]:
         if progress_counter == 0:
             logging.debug('Found {} files out of {}'.format(str(files_to_match - len(no_match)), str(files_to_match)))
-            progress_counter = int(files_to_match*0.05)
+            progress_counter = int(files_to_match * 0.05)
         file_key = sanitize_file_path(file)
         for d in directory_list:
             if skip_local_file_check:
                 file_name = os.path.join(d, file)
                 try:
                     full_file_path[file_key] = (file_name, os.path.getsize(file_name))
                     no_match.remove(file)
@@ -180,15 +183,17 @@
                 else:
                     continue
                 if not check_read_permissions(file_name):
                     no_read_access.add(file_name)
                 full_file_path[file_key] = (file_name, os.path.getsize(file_name))
                 no_match.remove(file)
                 break
-    logging.debug('Local directory search complete, found {} files out of {}'.format(str(files_to_match - len(no_match)), str(files_to_match)))
+    logging.debug(
+        'Local directory search complete, found {} files out of {}'.format(str(files_to_match - len(no_match)),
+                                                                           str(files_to_match)))
 
 
 def sanitize_file_path(file):
     """
     Replaces backslashes with forward slashes and removes leading / or drive:/.
 
     :param file: Relative or absolute filepath
@@ -209,7 +214,25 @@
     try:
         open(file)
         return True
     except (OSError, IOError) as err:
         if err.errno == 13:
             print('Permission Denied: {}'.format(file))
     return False
+
+
+def get_error():
+    exc_type, exc_value, exc_tb = sys.exc_info()
+    tbe = traceback.TracebackException(
+        exc_type, exc_value, exc_tb,
+    )
+    ex = ''.join(tbe.format_exception_only())
+    return 'Error: {}'.format(ex)
+
+
+def get_traceback():
+    exc_type, exc_value, exc_tb = sys.exc_info()
+    tbe = traceback.TracebackException(
+        exc_type, exc_value, exc_tb,
+    )
+    tb = ''.join(tbe.format())
+    return tb
```

### Comparing `nda_tools-0.2.7/NDATools/Validation.py` & `nda_tools-0.2.8/NDATools/Validation.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/NDATools/__init__.py` & `nda_tools-0.2.8/NDATools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import NDATools
 import requests
 import json
 import sys
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 pypi_version = None
 version_checked = False
 
 def check_version():
     try:
         from packaging.version import parse
     except ImportError:
```

### Comparing `nda_tools-0.2.7/nda_tools.egg-info/PKG-INFO` & `nda_tools-0.2.8/nda_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nda-tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: NIMH Data Archive Python Client
 Home-page: https://github.com/NDAR/nda-tools/tree/master/NDATools
 Author: NDA
 Author-email: NDAHelp@mail.nih.gov
 License: MIT
 Description: # nda-tools
```

### Comparing `nda_tools-0.2.7/nda_tools.egg-info/SOURCES.txt` & `nda_tools-0.2.8/nda_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/integration_tests/test_build_package.py` & `nda_tools-0.2.8/tests/integration_tests/test_build_package.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/integration_tests/test_configuration.py` & `nda_tools-0.2.8/tests/integration_tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/integration_tests/test_submission.py` & `nda_tools-0.2.8/tests/integration_tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/integration_tests/test_validation.py` & `nda_tools-0.2.8/tests/integration_tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/test_build_package.py` & `nda_tools-0.2.8/tests/test_build_package.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/test_configuration.py` & `nda_tools-0.2.8/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/test_submission.py` & `nda_tools-0.2.8/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/tests/test_validation.py` & `nda_tools-0.2.8/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/README.md` & `nda_tools-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/setup.py` & `nda_tools-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `nda_tools-0.2.7/PKG-INFO` & `nda_tools-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nda_tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: NIMH Data Archive Python Client
 Home-page: https://github.com/NDAR/nda-tools/tree/master/NDATools
 Author: NDA
 Author-email: NDAHelp@mail.nih.gov
 License: MIT
 Description: # nda-tools
```

