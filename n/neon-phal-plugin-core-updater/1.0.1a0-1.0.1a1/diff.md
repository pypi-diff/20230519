# Comparing `tmp/neon_phal_plugin_core_updater-1.0.1a0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.0.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6569 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7833 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2327 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-May-18 16:19 neon_phal_plugin_core_updater-1.0.1a0.dist-info/RECORD
-7 files, 12740 bytes uncompressed, 5241 bytes compressed:  58.9%
+Zip file size: 6574 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7869 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2327 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-May-19 16:51 neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD
+7 files, 12776 bytes uncompressed, 5246 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a0.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_core_updater/__init__.py

```diff
@@ -68,15 +68,16 @@
         Get GitHub release names in reverse-chronological order (newest first).
         """
         default_time = "2000-01-01T00:00:00Z"
         url = f'https://api.github.com/repos/{self.github_ref}/releases'
         releases: list = requests.get(url).json()
         releases.sort(key=lambda r: datetime.strptime(r.get('created_at',
                                                             default_time),
-                                                      "%Y-%m-%dT%H:%M:%SZ"))
+                                                      "%Y-%m-%dT%H:%M:%SZ"),
+                      reverse=True)
         return [r.get('name') for r in releases]
 
     def _get_pypi_releases(self):
         # TODO: Implement package release checks
         return []
 
     def check_core_updates(self, message: Message):
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a0.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.0.1a0.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.0.1a0
+Version: 1.0.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a0.dist-info/RECORD` & `neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-neon_phal_plugin_core_updater/__init__.py,sha256=RlWRgRPhknqktnK4FH06FeDi1RCxWHoGPJ2miYB_ils,7833
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/METADATA,sha256=wfXYULar3uggiPRJCXTrnBDvn5fS67dyDUzhTCBGpXU,2327
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/entry_points.txt,sha256=3UhJ0b7cF_TxJwAPWiEGnlMncHuI8nOvh9dzyeokMf0,98
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
-neon_phal_plugin_core_updater-1.0.1a0.dist-info/RECORD,,
+neon_phal_plugin_core_updater/__init__.py,sha256=wRzyxoFnSGqIg7x_kjqGz8aAqTE0fYpuW4TxeD7_v64,7869
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/METADATA,sha256=r8XCQqM3CJxetThX586Edq0vOuXRy6V90cbHID0Yvcs,2327
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/entry_points.txt,sha256=3UhJ0b7cF_TxJwAPWiEGnlMncHuI8nOvh9dzyeokMf0,98
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
+neon_phal_plugin_core_updater-1.0.1a1.dist-info/RECORD,,
```

