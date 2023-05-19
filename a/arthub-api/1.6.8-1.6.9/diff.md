# Comparing `tmp/arthub_api-1.6.8.tar.gz` & `tmp/arthub_api-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.8.tar", last modified: Thu May 18 12:09:46 2023, max compression
+gzip compressed data, was "arthub_api-1.6.9.tar", last modified: Fri May 19 06:21:27 2023, max compression
```

## Comparing `arthub_api-1.6.8.tar` & `arthub_api-1.6.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.204836 arthub_api-1.6.8/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.8/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-18 12:09:46.204836 arthub_api-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.181896 arthub_api-1.6.8/arthub_api/
--rw-rw-rw-   0        0        0      645 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.8/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.8/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.8/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.8/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    42964 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2070 2023-05-17 11:50:58.000000 arthub_api-1.6.8/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    26249 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.8/arthub_api/models.py
--rw-rw-rw-   0        0        0    42130 2023-05-17 11:50:58.000000 arthub_api-1.6.8/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.8/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.8/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.192868 arthub_api-1.6.8/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.8/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 12:09:46.204836 arthub_api-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     2973 2023-05-16 11:29:25.000000 arthub_api-1.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.202907 arthub_api-1.6.8/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.8/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.8/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.8/tests/conftest.py
--rw-rw-rw-   0        0        0     6110 2023-05-18 07:59:55.000000 arthub_api-1.6.8/tests/test_open_api.py
--rw-rw-rw-   0        0        0    17906 2023-05-18 12:05:48.000000 arthub_api-1.6.8/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.8/tests/test_storage.py
--rw-rw-rw-   0        0        0     6853 2023-05-18 12:05:48.000000 arthub_api-1.6.8/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.691635 arthub_api-1.6.9/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-19 06:21:27.691131 arthub_api-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.666960 arthub_api-1.6.9/arthub_api/
+-rw-rw-rw-   0        0        0      645 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3483 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.9/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.9/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    42964 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2070 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    26625 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.9/arthub_api/models.py
+-rw-rw-rw-   0        0        0    42130 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.9/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.679145 arthub_api-1.6.9/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.9/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.9/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:21:27.691635 arthub_api-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     3079 2023-05-19 06:20:15.000000 arthub_api-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.689424 arthub_api-1.6.9/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/_utils.py
+-rw-rw-rw-   0        0        0      280 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/conftest.py
+-rw-rw-rw-   0        0        0     6110 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    17906 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3647 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_storage.py
+-rw-rw-rw-   0        0        0     7255 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.8/LICENSE` & `arthub_api-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/PKG-INFO` & `arthub_api-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.8
+Version: 1.6.9
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.8/README.md` & `arthub_api-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/__init__.py` & `arthub_api-1.6.9/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/__main__.py` & `arthub_api-1.6.9/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/_internal_utils.py` & `arthub_api-1.6.9/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/asset_matrix.py` & `arthub_api-1.6.9/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/blade_api.py` & `arthub_api-1.6.9/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/blade_api_instance.py` & `arthub_api-1.6.9/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/blade_storage.py` & `arthub_api-1.6.9/arthub_api/blade_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         pass
     class FileNotFoundError(IOError):
         pass
 
 class SignerError(RuntimeError):
     pass
 
+class COSHttpError(RuntimeError):
+    pass
+
 # signer for blade api
 class RemoteSignerForPackage(object):    
     def __init__(self, blade_backend, force=False):
         self.cli = blade_backend
         self.force = force
         
     @classmethod
@@ -231,16 +234,16 @@
         resumableUploader = ResumableUploader(self.remote_signer, Bucket, Key, LocalFilePath, file_size, part_size, MAXThread, callback)
         if file_size < 20 * 1024 * 1024:
             resumableUploader.simple_upload()
             return
             
         resumableUploader.upload()
 
-    def get_download_url(self, Bucket, Key):
-        return self.remote_signer.get_download_url(Bucket, Key)
+    def get_download_url(self, Bucket, Key, Expired=1200):
+        return self.remote_signer.get_download_url(Bucket, Key, Expired)
 
     # check file exists with http-get method
     def check_exists(self, bucket, key):
         headers = {'Range': 'bytes=0-0'}
         self.download_url = self.remote_signer.get_download_url(bucket, key)
         response = requests.get(self.download_url, headers=headers)
         if response.status_code == 404:
@@ -258,23 +261,24 @@
         self.key = key
         self.local_path = local_path
         self.part_size = part_size
         self.thread_num = thread_num
         self.progress_callback = progress_callback
         self.file_size = file_size
         self.download_url = None
+        self.expired = 600
         self.url_expire_time = None
         self.tmp_file = '{0}_ahtmp'.format(local_path)
         self.record_file = '{0}_dl_ahrecord'.format(local_path)
 
     def _refresh_download_url(self):
         current_time = time.time()
         if self.download_url is None or current_time >= self.url_expire_time:
-            self.download_url = self.remote_signer.get_download_url(self.bucket, self.key)
-            self.url_expire_time = current_time + 10 * 60  # 10 minutes expiry time
+            self.download_url = self.remote_signer.get_download_url(self.bucket, self.key, self.expired)
+            self.url_expire_time = current_time + self.expired - 20  # 10 minutes expiry time
 
     def _load_progress(self):
         if os.path.exists(self.record_file):
             with open(self.record_file, 'r') as f:
                 return [tuple(map(int, line.strip().split('-'))) for line in f]
         return []
 
@@ -384,33 +388,33 @@
         except Exception as e:
             error_message = "request S3 multipart by url %s upload id exception: %s" % (begin_url, e)
             logging.error("[API] %s" % error_message)
             raise
         if not res or not res.ok:
             error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (begin_url, res.status_code)
             logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
+            raise COSHttpError(error_message)
         # parse
         try:
             xml_tree = ElementTree.fromstring(res.content)
             upload_id = xml_tree.find("UploadId").text
             logging.info("[API] get multipart upload id: %s" % upload_id)
             return upload_id
         except Exception as e:
             error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
             logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
+            raise COSHttpError(error_message)
         
     def _upload_part(self, bucket, key, start, end, upload_id, part_number, disable_record=False):
         upload_url = self.remote_signer.get_upload_part_url(bucket, key, upload_id, part_number)
         res = utils.upload_part_of_file(upload_url, self.local_path, start, end-start+1, self._report)
         if not res.is_succeeded():
             err = "upload \"{0}\"th part failed, {1}".format(part_number, res.error_message())
             logging.error("[API] %s" % err)
-            raise RuntimeError(err)
+            raise COSHttpError(err)
         etag = res.data.headers.get("etag").strip('"')
         if not disable_record:
             self._save_progress(start, end, upload_id, part_number, etag)  # Save progress after part is uploaded
         return (part_number, etag)
     
     def _complete_multipart_upload(self, bucket, key, upload_id, etags):
         complete_url = self.remote_signer.get_complete_multipart_upload_url(bucket, key, upload_id)
@@ -422,24 +426,24 @@
         except Exception as e:
             error_message = "request complete S3 multipart by url %s upload id exception: %s" % (complete_url, e)
             logging.error("[API] %s" % error_message)
             raise
         if not res or not res.ok:
             error_message = "request complete S3 multipart upload id failed, url: %s, code: %d" % (complete_url, res.status_code)
             logging.error("[API] %s" % error_message)
-            raise RuntimeError(error_message)
+            raise COSHttpError(error_message)
         return
         
     def _upload(self, bucket, key):
         upload_url = self.remote_signer.get_upload_url(bucket, key)
         res = utils.upload_file(upload_url, self.local_path, self._report)
         if not res.is_succeeded():
             err = "upload failed, {0}".format(res.error_message())
             logging.error("[API] %s" % err)
-            raise RuntimeError(err)
+            raise COSHttpError(err)
         return 
         
     def _report(self, new_read_size):
         if self.progress_callback:
             self.progress_callback.report(new_read_size)
 
     def _load_progress(self):
@@ -556,28 +560,31 @@
 
     def check_file_exist(self, server_path):
         try:
             return self.cli.check_exists("", server_path)
         except ValueError:
             return False
 
-    def get_download_url(self, server_path):
-        """Get current download URL by given server_path.
-
-        Args:
-            server_path: Relative path on COS.
-            expired_time: Expired timestamps.
-
-        Returns:
-            - Current download URL.
+    def get_file_object(self, server_path):
+        url = self.get_download_url(server_path)
+        r = requests.get(url, stream=True)
+        if r.status_code >= 400:
+            msg = r.text
+            if msg == u'':
+                msg = r.headers
+            raise COSHttpError("message: {0}, status code: {1}".format(msg, r.status_code))
+        obj = dict(r.headers)
+        obj.update({"Response": r})
+        return obj
 
-        """
+    def get_download_url(self, server_path, expired_time=1200):
         return self.cli.get_download_url(
             Bucket="",
             Key=server_path,
+            Expired=expired_time,
         )
 
     @tenacity_retry(
         stop=stop_after_attempt(5),
         wait=wait_fixed(0.5),
         retry=retry_if_exception_type(OSError)
         | retry_if_exception_type(PermissionError)
```

### Comparing `arthub_api-1.6.8/arthub_api/config.py` & `arthub_api-1.6.9/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/exception.py` & `arthub_api-1.6.9/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/models.py` & `arthub_api-1.6.9/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/open_api.py` & `arthub_api-1.6.9/arthub_api/open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/storage.py` & `arthub_api-1.6.9/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api/utils.py` & `arthub_api-1.6.9/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.9/arthub_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.8
+Version: 1.6.9
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.8/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.9/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/setup.py` & `arthub_api-1.6.9/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-#!/usr/bin/env python
-import os
-import sys
-from codecs import open
-
-from setuptools import setup, find_packages
-from setuptools.command.test import test as TestCommand
-
-
-# CURRENT_PYTHON = sys.version_info[:2]
-# REQUIRED_PYTHON = (3, 7)
-
-# if CURRENT_PYTHON < REQUIRED_PYTHON:
-#     sys.stderr.write("""
-# ==========================
-# Unsupported Python version
-# ==========================
-# This version of arthub_api requires at least Python {}.{}, but
-# you're trying to install it on Python {}.{}. To resolve this,
-# consider upgrading to a supported Python version.
-# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
-#     sys.exit(1)
-
-
-class PyTest(TestCommand):
-    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
-
-    def initialize_options(self):
-        TestCommand.initialize_options(self)
-        try:
-            from multiprocessing import cpu_count
-
-            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
-        except (ImportError, NotImplementedError):
-            self.pytest_args = ["-n", "1", "--boxed"]
-
-    def finalize_options(self):
-        TestCommand.finalize_options(self)
-        self.test_args = []
-        self.test_suite = True
-
-    def run_tests(self):
-        import pytest
-
-        errno = pytest.main(self.pytest_args)
-        sys.exit(errno)
-
-
-# 'setup.py publish' shortcut.
-if sys.argv[-1] == "publish":
-    os.system("python setup.py sdist bdist_wheel")
-    os.system("twine upload dist/*")
-    sys.exit()
-
-requires = [
-    "requests",
-    "platformdirs==2.0.2",
-    "tenacity>=5.0",
-    "six==1.16",
-    "environ_config>=21",
-]
-
-test_requirements = [
-    "pytest",
-]
-
-about = {}
-here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
-          "utf-8") as f:
-    exec(f.read(), about)
-
-with open("README.md", "r", "utf-8") as f:
-    readme = f.read()
-
-setup(name=about["__title__"],
-      version=about["__version__"],
-      description=about["__description__"],
-      long_description=readme,
-      long_description_content_type="text/markdown",
-      author=about["__author__"],
-      author_email=about["__author_email__"],
-      url=about["__url__"],
-      package_dir={'arthub_api': 'arthub_api'},
-      packages=['arthub_api'],
-      package_data={"": ["LICENSE", "NOTICE"]},
-      include_package_data=True,
-      install_requires=requires,
-      license=about["__license__"],
-      zip_safe=False,
-      classifiers=[
-          "Development Status :: 5 - Production/Stable",
-          "Environment :: Web Environment",
-          "Intended Audience :: Developers",
-          "Natural Language :: English",
-          "Operating System :: OS Independent"],
-      cmdclass={"test": PyTest},
-      tests_require=test_requirements,
-      entry_points={
-          "console_scripts": [
-              "aha = arthub_api.__main__:main",
-          ]
-      },
-      extras_require={
-        ':python_version == "2.7"': ['futures']
-    })
+#!/usr/bin/env python
+import os
+import sys
+from codecs import open
+
+from setuptools import setup, find_packages
+from setuptools.command.test import test as TestCommand
+
+
+# CURRENT_PYTHON = sys.version_info[:2]
+# REQUIRED_PYTHON = (3, 7)
+
+# if CURRENT_PYTHON < REQUIRED_PYTHON:
+#     sys.stderr.write("""
+# ==========================
+# Unsupported Python version
+# ==========================
+# This version of arthub_api requires at least Python {}.{}, but
+# you're trying to install it on Python {}.{}. To resolve this,
+# consider upgrading to a supported Python version.
+# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
+#     sys.exit(1)
+
+
+class PyTest(TestCommand):
+    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
+
+    def initialize_options(self):
+        TestCommand.initialize_options(self)
+        try:
+            from multiprocessing import cpu_count
+
+            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
+        except (ImportError, NotImplementedError):
+            self.pytest_args = ["-n", "1", "--boxed"]
+
+    def finalize_options(self):
+        TestCommand.finalize_options(self)
+        self.test_args = []
+        self.test_suite = True
+
+    def run_tests(self):
+        import pytest
+
+        errno = pytest.main(self.pytest_args)
+        sys.exit(errno)
+
+
+# 'setup.py publish' shortcut.
+if sys.argv[-1] == "publish":
+    os.system("python setup.py sdist bdist_wheel")
+    os.system("twine upload dist/*")
+    sys.exit()
+
+requires = [
+    "requests",
+    "platformdirs==2.0.2",
+    "tenacity>=5.0",
+    "six==1.16",
+    "environ_config>=21",
+]
+
+test_requirements = [
+    "pytest",
+]
+
+about = {}
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
+          "utf-8") as f:
+    exec(f.read(), about)
+
+with open("README.md", "r", "utf-8") as f:
+    readme = f.read()
+
+setup(name=about["__title__"],
+      version=about["__version__"],
+      description=about["__description__"],
+      long_description=readme,
+      long_description_content_type="text/markdown",
+      author=about["__author__"],
+      author_email=about["__author_email__"],
+      url=about["__url__"],
+      package_dir={'arthub_api': 'arthub_api'},
+      packages=['arthub_api'],
+      package_data={"": ["LICENSE", "NOTICE"]},
+      include_package_data=True,
+      install_requires=requires,
+      license=about["__license__"],
+      zip_safe=False,
+      classifiers=[
+          "Development Status :: 5 - Production/Stable",
+          "Environment :: Web Environment",
+          "Intended Audience :: Developers",
+          "Natural Language :: English",
+          "Operating System :: OS Independent"],
+      cmdclass={"test": PyTest},
+      tests_require=test_requirements,
+      entry_points={
+          "console_scripts": [
+              "aha = arthub_api.__main__:main",
+          ]
+      },
+      extras_require={
+        ':python_version == "2.7"': ['futures']
+    })
```

### Comparing `arthub_api-1.6.8/tests/test_open_api.py` & `arthub_api-1.6.9/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/tests/test_open_api_blade.py` & `arthub_api-1.6.9/tests/test_open_api_blade.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.8/tests/test_storage_blade.py` & `arthub_api-1.6.9/tests/test_storage_blade.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     print("\rProgress: |{bar}| {progress:.2f}% Complete".format(bar=bar, progress=progress), end="")
     if six.PY2:
         sys.stdout.flush()
     
     
 def network_downloader(target, local):
     class TmpSigner(object):    
-        def get_download_url(self, bucket, key):
+        def get_download_url(self, bucket, key, expired=600):
             # this will returns a url expires in 10 minutes
             return target
         def get_file_size(self, bucket, key):
             # this will returns a url expires in 10 minutes
             with requests.get(target, stream=True) as r:
                 return int(r.headers["Content-length"])
         
@@ -90,14 +90,23 @@
 
 def test_blade_check_exists(env, tmp_path):
     blade_api = init_api(env)
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.2/arthub_test_pkg.7z"
     cli = BladeCOSApi(api=blade_api, force=True)
     assert cli.check_file_exist(target)
 
+def test_blade_get_file_object(env, tmp_path):
+    blade_api = init_api(env)
+    target = "pkg_distribution/7z/portable_photoshop/2023.24.0.1-thm.1/portable_photoshop.7z"
+    cli = BladeCOSApi(api=blade_api, force=True)
+    o = cli.get_file_object(target)
+    assert o
+    assert o.get("Content-Type") == 'application/octet-stream'
+    assert int(o.get("Content-Length")) > 1024*1024*1024
+
 def test_blade_get_download_url(env, tmp_path):
     blade_api = init_api(env)
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.2/arthub_test_pkg.7z"
     cli = BladeCOSApi(api=blade_api, force=True)
     assert cli.get_download_url(target)
     
 def test_blade_uploader(env, tmp_path):
@@ -182,9 +191,8 @@
     
     target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
     def print_percent1(a, b):
         print_percent(a, b)
         if a > b/2:
             import os
             os.exit(1)
-    cli.upload_file(target, source, print_percent)
-        
+    cli.upload_file(target, source, print_percent)
```

