# Comparing `tmp/edman_web-2023.5.19.tar.gz` & `tmp/edman_web-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2023.5.19.tar", last modified: Fri May 19 01:25:22 2023, max compression
+gzip compressed data, was "edman_web-2023.5.8.tar", last modified: Mon May  8 04:41:52 2023, max compression
```

## Comparing `edman_web-2023.5.19.tar` & `edman_web-2023.5.8.tar`

### file list

```diff
@@ -1,34 +1,20 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.5.19/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-19 01:25:22.710404 edman_web-2023.5.19/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.5.19/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.5.19/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7090 2023-05-16 07:35:37.000000 edman_web-2023.5.19/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.5.19/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-19 01:25:22.000000 edman_web-2023.5.19/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      617 2023-05-19 01:25:22.000000 edman_web-2023.5.19/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-19 01:25:22.000000 edman_web-2023.5.19/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       64 2023-05-19 01:25:22.000000 edman_web-2023.5.19/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2023-05-19 01:25:22.000000 edman_web-2023.5.19/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      948 2023-05-19 01:23:44.000000 edman_web-2023.5.19/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-19 01:25:22.710404 edman_web-2023.5.19/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    15283 2023-05-16 07:35:37.000000 edman_web-2023.5.19/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.5.19/tests/test_search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-19 01:25:22.710404 edman_web-2023.5.19/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2023.5.19/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 00:15:38.000000 edman_web-2023.5.19/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.696269 edman_web-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.5.8/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6477 2023-05-08 04:40:18.000000 edman_web-2023.5.8/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.5.8/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       61 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-05-08 04:41:52.696269 edman_web-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13863 2023-04-25 08:38:11.000000 edman_web-2023.5.8/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.5.8/tests/test_search_manager.py
```

### Comparing `edman_web-2023.5.19/LICENSE.txt` & `edman_web-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.19/README.rst` & `edman_web-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.19/edman_web/file_manager.py` & `edman_web-2023.5.8/edman_web/file_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import base64
-import gridfs
-import mimetypes
+import gzip
 from typing import Union, List, Tuple, Any
 from io import BytesIO
 from werkzeug.datastructures import FileStorage
 from bson import ObjectId
 from PIL import Image as PILImage
 from gridfs.errors import GridFSError
 from edman import File, Config
@@ -51,61 +50,45 @@
             except Exception as e:
                 # 途中で例外が起きた場合、gridfsからデータを削除する
                 self.fs_delete(inserted_file_oids)
                 raise EdmanDbProcessError(str(e))
 
     def web_grid_in(self, file: FileStorage, compress: bool) -> list[Any]:
         """
-        Gridfsへデータをアップロード
+        Gridfsへデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
 
         :param FileStorage file:
         :param bool compress:
         :return: inserted
         :rtype: list
         """
         inserted = []
+
         try:
             f = file.stream.read()
-            metadata = {'filename': file.filename}
+            if compress:
+                f = gzip.compress(f, compresslevel=self.comp_level)
+                compress_type = 'gzip'
+            else:
+                compress_type = None
+
+            metadata = {'filename': file.filename, 'compress': compress_type}
+
         except OSError:
             raise EdmanDbProcessError('DBにファイルをアップロード出来ませんでした')
         except Exception:
             raise
+
         try:
             inserted.append(self.fs.put(f, **metadata))
         except GridFSError as e:
             raise EdmanDbProcessError(e)
         return inserted
 
-    def file_download(self, oid: Union[ObjectId, str]) -> tuple[
-        gridfs.grid_file.GridOut, str, str]:
-        """
-        GridFsからファイルをダウンロードする
-
-        :param str or ObjectId oid:
-        :rtype: tuple
-        :return:
-        """
-        if not isinstance(oid, ObjectId):
-            if ObjectId.is_valid(oid):
-                oid = ObjectId(oid)
-            else:
-                raise ValueError('ObjectIdに合致しません')
-
-        # ファイル情報を取得
-        try:
-            content = self.fs.get(oid)
-        except gridfs.errors.NoFile:
-            raise ValueError('ファイルが存在しません')
-        except gridfs.errors.GridFSError:
-            raise
-        file_name = content.filename
-        mimetype = mimetypes.guess_type(file_name)[0]
-        return content, file_name, mimetype
-
     def file_delete(self, collection: str, oid: Union[str, ObjectId],
                     delete_list: List[str]):
         """
         edmanからファイルを削除する
 
         :param str collection:
         :param str or ObjectId oid:
```

### Comparing `edman_web-2023.5.19/edman_web/search_manager.py` & `edman_web-2023.5.8/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.19/tests/test_file_manager.py` & `edman_web-2023.5.8/tests/test_file_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 from pathlib import Path
 import tempfile
 import base64
 import os
-import mimetypes
+import gzip
 from io import BytesIO
 from unittest import TestCase
 from PIL import Image
 from pymongo import errors as py_errors, MongoClient
 from bson import ObjectId, DBRef
 import gridfs
 from werkzeug.datastructures import FileStorage
@@ -352,53 +352,20 @@
             inserted = self.file_manager.web_grid_in(st, compress=False)
             a = self.fs.get(inserted[0])
             actual = a.read().decode()
             expected = content.decode()
             self.assertEqual(expected, actual)
 
             # 圧縮が効いているか否か
-            # with files[1].open('rb') as f:
-            #     content = f.read()
-            #     st = FileStorage(stream=BytesIO(content),
-            #                      filename=f.name)
-            # inserted = self.file_manager.web_grid_in(st, compress=True)
-            # b = self.fs.get(inserted[0])
-            # if b.compress == 'gzip':
-            #     actual = gzip.decompress(b.read()).decode()
-            # else:  # 現状compress指定は"gzip"かNoneのみ
-            #     actual = None
-            # self.assertIsNotNone(b.compress)
-            # expected = content.decode()
-            # self.assertEqual(expected, actual)
-
-    def test_file_download(self):
-
-        if not self.db_server_connect:
-            return
-
-        # gridfsにファイルを入れる
-        with tempfile.TemporaryDirectory() as tmp_dl_dir:
-            # ファイルを作成
-            files = self.make_txt_files(tmp_dl_dir, 'file_download', qty=2)
-            # ファイルをgridfsに入れる
-            inserted_oids = []
-            self.fs = gridfs.GridFS(self.testdb)
-            expected = []
-            for file in files:
-                with file.open('rb') as f:
-                    content = f.read()
-                    metadata = {'filename': os.path.basename(f.name)}
-                    inserted_oids.append(self.fs.put(content, **metadata))
-                    # 比較用データ作成
-                    expected.append([os.path.basename(f.name), content.decode(), mimetypes.guess_type(f.name)[0]])
-
-            actual = []
-            # データをダウンロード
-            for oid in inserted_oids:
-                content, file_name, mimetype = self.file_manager.file_download(oid)
-                actual.append([file_name, content.read().decode() , mimetype])
-                # print(file_name, mimetype, content.read().decode())
-
-            # テスト
-            self.assertListEqual(expected, actual)
-            # print(expected)
-            # print(actual)
+            with files[1].open('rb') as f:
+                content = f.read()
+                st = FileStorage(stream=BytesIO(content),
+                                 filename=f.name)
+            inserted = self.file_manager.web_grid_in(st, compress=True)
+            b = self.fs.get(inserted[0])
+            if b.compress == 'gzip':
+                actual = gzip.decompress(b.read()).decode()
+            else:  # 現状compress指定は"gzip"かNoneのみ
+                actual = None
+            self.assertIsNotNone(b.compress)
+            expected = content.decode()
+            self.assertEqual(expected, actual)
```

### Comparing `edman_web-2023.5.19/tests/test_search_manager.py` & `edman_web-2023.5.8/tests/test_search_manager.py`

 * *Files identical despite different names*

