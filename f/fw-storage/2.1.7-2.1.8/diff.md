# Comparing `tmp/fw_storage-2.1.7-py3-none-any.whl.zip` & `tmp/fw_storage-2.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 37976 bytes, number of entries: 24
+Zip file size: 37981 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      511 b- defN 80-Jan-01 00:00 fw_storage/__init__.py
 -rw-r--r--  2.0 unx    18182 b- defN 80-Jan-01 00:00 fw_storage/config.py
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 fw_storage/errors.py
 -rw-r--r--  2.0 unx     1676 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
 -rw-r--r--  2.0 unx     1016 b- defN 80-Jan-01 00:00 fw_storage/filters.py
 -rw-r--r--  2.0 unx     1013 b- defN 80-Jan-01 00:00 fw_storage/future/__init__.py
 -rw-r--r--  2.0 unx    11816 b- defN 80-Jan-01 00:00 fw_storage/future/base.py
 -rw-r--r--  2.0 unx     4652 b- defN 80-Jan-01 00:00 fw_storage/future/errors.py
 -rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 fw_storage/future/types/__init__.py
 -rw-r--r--  2.0 unx    12755 b- defN 80-Jan-01 00:00 fw_storage/future/types/fs.py
 -rw-r--r--  2.0 unx     3934 b- defN 80-Jan-01 00:00 fw_storage/future/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_storage/py.typed
--rw-r--r--  2.0 unx     7677 b- defN 80-Jan-01 00:00 fw_storage/storage.py
+-rw-r--r--  2.0 unx     7611 b- defN 80-Jan-01 00:00 fw_storage/storage.py
 -rw-r--r--  2.0 unx       28 b- defN 80-Jan-01 00:00 fw_storage/types/__init__.py
--rw-r--r--  2.0 unx     6844 b- defN 80-Jan-01 00:00 fw_storage/types/az.py
+-rw-r--r--  2.0 unx     6900 b- defN 80-Jan-01 00:00 fw_storage/types/az.py
 -rw-r--r--  2.0 unx    13338 b- defN 80-Jan-01 00:00 fw_storage/types/dicom.py
 -rw-r--r--  2.0 unx     7996 b- defN 80-Jan-01 00:00 fw_storage/types/dicomweb.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 fw_storage/types/fs.py
--rw-r--r--  2.0 unx     4861 b- defN 80-Jan-01 00:00 fw_storage/types/gs.py
--rw-r--r--  2.0 unx     6374 b- defN 80-Jan-01 00:00 fw_storage/types/s3.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1925 b- defN 16-Jan-01 00:00 fw_storage-2.1.7.dist-info/RECORD
-24 files, 110066 bytes uncompressed, 34892 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     4937 b- defN 80-Jan-01 00:00 fw_storage/types/gs.py
+-rw-r--r--  2.0 unx     6450 b- defN 80-Jan-01 00:00 fw_storage/types/s3.py
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1925 b- defN 16-Jan-01 00:00 fw_storage-2.1.8.dist-info/RECORD
+24 files, 110208 bytes uncompressed, 34897 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: fw_storage/types/gs.py
 Comment: 
 
 Filename: fw_storage/types/s3.py
 Comment: 
 
-Filename: fw_storage-2.1.7.dist-info/LICENSE
+Filename: fw_storage-2.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: fw_storage-2.1.7.dist-info/METADATA
+Filename: fw_storage-2.1.8.dist-info/METADATA
 Comment: 
 
-Filename: fw_storage-2.1.7.dist-info/WHEEL
+Filename: fw_storage-2.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: fw_storage-2.1.7.dist-info/RECORD
+Filename: fw_storage-2.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_storage/storage.py

```diff
@@ -121,36 +121,34 @@
         *_args,
         **_kwargs,
     ):
         """Initialize cloud storage, check permission and setup cache."""
         self.delete_keys: t.Set[str] = set()
 
     @abc.abstractmethod
-    def download_file(self, path: str, dst: t.IO[bytes]) -> None:
+    def download_file(self, path: AnyPath, dst: t.IO[bytes]) -> None:
         """Download file and it opened for reading in binary mode."""
 
     @abc.abstractmethod
-    def upload_file(self, path: str, file: AnyFile) -> None:
+    def upload_file(self, path: AnyPath, file: AnyFile) -> None:
         """Upload file to the given path."""
 
     @abc.abstractmethod
     def flush_delete(self):
         """Flush pending remove operations."""
 
     def get(self, path: AnyPath, **_kwargs) -> BinFile:
         """Return a file opened for reading in binary mode."""
-        abspath = self.abspath(path)
         file = TempFile()
-        self.download_file(abspath, file)
+        self.download_file(path, file)
         file.seek(0)
         return BinFile(t.cast(t.BinaryIO, file), metapath=self.relpath(path))
 
     def set(self, path: AnyPath, file: AnyFile) -> None:
         """Write a file at the given path in storage."""
-        path = self.abspath(path)
         file = str(file) if isinstance(file, Path) else file
         self.upload_file(path, file)
 
     def rm(self, path: AnyPath, recurse: bool = False, flush: bool = False) -> None:
         """Remove file from storage.
 
         Removing objects is delayed and performed in batches (see 'flush_delete').
```

## fw_storage/types/az.py

```diff
@@ -163,22 +163,23 @@
             size=blob.size,
             hash=blob.etag,
             created=blob.creation_time.timestamp(),
             modified=blob.last_modified.timestamp(),
         )
 
     @errmap
-    def download_file(self, path: str, dst: t.IO[bytes]) -> None:
+    def download_file(self, path: AnyPath, dst: t.IO[bytes]) -> None:
         """Download file and it is opened for reading in binary mode."""
-        blob_stream = self.client.download_blob(path)
+        blob_stream = self.client.download_blob(self.abspath(path))
         blob_stream.readinto(dst)
 
     @errmap
-    def upload_file(self, path: str, file: AnyFile) -> None:
+    def upload_file(self, path: AnyPath, file: AnyFile) -> None:
         """Write source file to the given path."""
+        path = self.abspath(path)
         # upload_blob uses automatic chunking stated by Azure documentation
         with open_any(file, mode="rb") as r_file:
             self.client.upload_blob(name=path, data=r_file, overwrite=True)
 
     @errmap
     def flush_delete(self) -> None:
         """Remove a file at the given path."""
```

## fw_storage/types/gs.py

```diff
@@ -102,21 +102,23 @@
             size=blob.size,
             hash=blob.etag,
             created=blob.time_created.timestamp(),
             modified=blob.updated.timestamp(),
         )
 
     @errmap
-    def download_file(self, path: str, dst: t.IO[bytes]) -> None:
+    def download_file(self, path: AnyPath, dst: t.IO[bytes]) -> None:
         """Download file and it opened for reading in binary mode."""
+        path = self.abspath(path)
         self.client.bucket(self.config.bucket).blob(path).download_to_file(dst)
 
     @errmap
-    def upload_file(self, path: str, file: AnyFile) -> None:
+    def upload_file(self, path: AnyPath, file: AnyFile) -> None:
         """Upload file to the given path."""
+        path = self.abspath(path)
         blob = self.client.bucket(self.config.bucket).blob(path)
         if isinstance(file, bytes):
             upload_func = blob.upload_from_string
         elif isinstance(file, str):
             upload_func = blob.upload_from_filename
         else:
             upload_func = blob.upload_from_file
```

## fw_storage/types/s3.py

```diff
@@ -129,22 +129,24 @@
             size=meta["ContentLength"],
             hash=meta["ETag"][1:-1],
             created=meta["LastModified"].timestamp(),  # TODO consider None
             modified=meta["LastModified"].timestamp(),
         )
 
     @errmap
-    def download_file(self, path: str, dst: t.IO[bytes]) -> None:
+    def download_file(self, path: AnyPath, dst: t.IO[bytes]) -> None:
         """Download file and it opened for reading in binary mode."""
         bucket = self.config.bucket
+        path = self.abspath(path)
         self.client.download_fileobj(bucket, path, dst, Config=TRANSFER_CONFIG)
 
     @errmap
-    def upload_file(self, path: str, file: AnyFile) -> None:
+    def upload_file(self, path: AnyPath, file: AnyFile) -> None:
         """Upload file to the given path."""
+        path = self.abspath(path)
         upload_args: list = []
         upload_kwargs: dict = {"Bucket": self.config.bucket, "Key": path}
         acl = "bucket-owner-full-control"
         if isinstance(file, bytes):
             upload_func = self.client.put_object
             upload_kwargs.update(Body=file, ACL=acl)
         elif isinstance(file, str):
```

## Comparing `fw_storage-2.1.7.dist-info/LICENSE` & `fw_storage-2.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_storage-2.1.7.dist-info/METADATA` & `fw_storage-2.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-storage
-Version: 2.1.7
+Version: 2.1.8
 Summary: Unified storage interface.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-storage
 License: MIT
 Keywords: Flywheel,file,object,storage
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_storage-2.1.7.dist-info/RECORD` & `fw_storage-2.1.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 fw_storage/future/__init__.py,sha256=TWyZ7CFeCDO4_uiiT6gLJhE-SP8Ie7bNsCB3vUSbv2U,1013
 fw_storage/future/base.py,sha256=GsXb5vvvmm1iSn9ErM_djNjSKEbsIeqzCxw39m96lDo,11816
 fw_storage/future/errors.py,sha256=tE-wb4n_X8-v2zaU5KpoPlQVfDaDhazOpjLmNU45cw0,4652
 fw_storage/future/types/__init__.py,sha256=zOnfjDtMpINsVdYFikGbvjIf_FVnfPpm-DanhqDrLjo,36
 fw_storage/future/types/fs.py,sha256=xxs7p7Q6AQRwPALAg5Ds386yHh9k2cDe1HFtLKKrUWo,12755
 fw_storage/future/utils.py,sha256=JLVhxqSsA0uyNMbhPKyEQoJ3FVYoqLyjyO3bfeO4OOk,3934
 fw_storage/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fw_storage/storage.py,sha256=WgEySgS8f4Mjlx1lthDwtpfQ5XWVgTutQGCXPz1e-b8,7677
+fw_storage/storage.py,sha256=1_KqVCRUzINhERpSygBNvZhdvIzYBw7V6FWk13DKJqA,7611
 fw_storage/types/__init__.py,sha256=TT2pfyY-AMuKb4FZduNbVbmWTBRyEC3autb1QbdHE24,28
-fw_storage/types/az.py,sha256=J2KbT9ugvTpLfAZg4BX0lDLK4i2lM8EYisyAnj9tVG4,6844
+fw_storage/types/az.py,sha256=hRSvvPZQlVkBGMNtgKNJfcnrEDVDgXUah-aAZKzD6Aw,6900
 fw_storage/types/dicom.py,sha256=XUSFsdSGTyNb8a6-K2H0jvztzj5lT5FmuGHt8pi_SCI,13338
 fw_storage/types/dicomweb.py,sha256=NR9E-csPgznASouwIdokukAxGPKCPRobhz80e4-z_v0,7996
 fw_storage/types/fs.py,sha256=Cz_GGrS_e11m9SvDgdjJkMf-VMI0s5DKUJZp0bWSegM,140
-fw_storage/types/gs.py,sha256=lQRo9qz0EHf3YmPO7LzLBFYEGkwqhmlVtxwF2T9EISI,4861
-fw_storage/types/s3.py,sha256=MMelCfrbaNZbZqGPBj9mt_Cdyhrbeq-ObYmmC4bM1G4,6374
-fw_storage-2.1.7.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_storage-2.1.7.dist-info/METADATA,sha256=M4SGrmNECRk6Bcp758GIF6dxnoAy5xx0lQsniBpyt80,4013
-fw_storage-2.1.7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_storage-2.1.7.dist-info/RECORD,,
+fw_storage/types/gs.py,sha256=9J0QOH_Ty7QoMeZ6BkaZNGQw3f8LNgdKjz9DmBg8PsU,4937
+fw_storage/types/s3.py,sha256=RomRY4TFZzcvwuF5hemxsQfODuHFDAQcensmocy_0sc,6450
+fw_storage-2.1.8.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_storage-2.1.8.dist-info/METADATA,sha256=xvsGrHg1cxAG2r3BwekK3OQJiTdYLeVCm--V1YRyOK0,4013
+fw_storage-2.1.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_storage-2.1.8.dist-info/RECORD,,
```

