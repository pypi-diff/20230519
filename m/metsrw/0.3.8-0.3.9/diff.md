# Comparing `tmp/metsrw-0.3.8.tar.gz` & `tmp/metsrw-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metsrw-0.3.8.tar", last modified: Wed Apr 17 17:54:17 2019, max compression
+gzip compressed data, was "dist/metsrw-0.3.9.tar", last modified: Fri Jun 21 17:23:24 2019, max compression
```

## Comparing `metsrw-0.3.8.tar` & `metsrw-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/
--rw-r--r--   0 jesus     (1000) jesus     (1000)    34520 2019-03-19 23:59:42.000000 metsrw-0.3.8/LICENSE
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw/
--rw-r--r--   0 jesus     (1000) jesus     (1000)     5652 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/validate.py
--rwxr-xr-x   0 jesus     (1000) jesus     (1000)    21931 2019-04-17 17:54:07.000000 metsrw-0.3.8/metsrw/mets.py
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw/resources/
--rw-r--r--   0 jesus     (1000) jesus     (1000)    12087 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/resources/archivematica_mets_schematron.xml
--rw-r--r--   0 jesus     (1000) jesus     (1000)   155309 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/resources/mets.xsd
--rw-r--r--   0 jesus     (1000) jesus     (1000)    12177 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/resources/archivematica_mets_pointer_file_schematron.xml
--rw-r--r--   0 jesus     (1000) jesus     (1000)     7050 2019-03-24 14:15:54.000000 metsrw-0.3.8/metsrw/di.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)    19007 2019-04-17 17:54:07.000000 metsrw-0.3.8/metsrw/fsentry.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)    20702 2019-04-17 17:54:07.000000 metsrw-0.3.8/metsrw/metadata.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)     1730 2019-04-17 17:54:07.000000 metsrw-0.3.8/metsrw/__init__.py
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw/plugins/
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw/plugins/premisrw/
--rw-r--r--   0 jesus     (1000) jesus     (1000)     2054 2019-03-24 14:15:54.000000 metsrw-0.3.8/metsrw/plugins/premisrw/__init__.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)     2866 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/plugins/premisrw/utils.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)    35038 2019-04-01 19:22:02.000000 metsrw-0.3.8/metsrw/plugins/premisrw/premis.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)       26 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/plugins/__init__.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)      348 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/exceptions.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)     1785 2019-03-19 23:59:42.000000 metsrw-0.3.8/metsrw/utils.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)     1810 2019-03-19 23:59:42.000000 metsrw-0.3.8/setup.py
--rw-r--r--   0 jesus     (1000) jesus     (1000)     2651 2019-04-17 17:54:17.000000 metsrw-0.3.8/PKG-INFO
--rw-r--r--   0 jesus     (1000) jesus     (1000)     1649 2019-03-19 23:59:42.000000 metsrw-0.3.8/README.md
--rw-r--r--   0 jesus     (1000) jesus     (1000)       42 2019-03-19 23:59:42.000000 metsrw-0.3.8/MANIFEST.in
-drwxr-xr-x   0 jesus     (1000) jesus     (1000)        0 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/
--rw-r--r--   0 jesus     (1000) jesus     (1000)     2651 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/PKG-INFO
--rw-r--r--   0 jesus     (1000) jesus     (1000)      598 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/SOURCES.txt
--rw-r--r--   0 jesus     (1000) jesus     (1000)       16 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/requires.txt
--rw-r--r--   0 jesus     (1000) jesus     (1000)        7 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/top_level.txt
--rw-r--r--   0 jesus     (1000) jesus     (1000)        1 2019-04-17 17:54:17.000000 metsrw-0.3.8/metsrw.egg-info/dependency_links.txt
--rw-r--r--   0 jesus     (1000) jesus     (1000)       38 2019-04-17 17:54:17.000000 metsrw-0.3.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2651 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      598 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1810 2019-04-08 18:55:47.000000 metsrw-0.3.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)    34520 2018-08-26 17:08:43.000000 metsrw-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       42 2018-08-26 17:08:43.000000 metsrw-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1649 2018-08-26 17:08:43.000000 metsrw-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/
+-rw-r--r--   0 root         (0) root         (0)     1730 2019-06-21 14:47:14.000000 metsrw-0.3.9/metsrw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20702 2019-06-07 12:48:19.000000 metsrw-0.3.9/metsrw/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/plugins/
+-rw-r--r--   0 root         (0) root         (0)       26 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/plugins/premisrw/
+-rw-r--r--   0 root         (0) root         (0)     2054 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35038 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/premis.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/utils.py
+-rw-r--r--   0 root         (0) root         (0)      348 2018-09-25 23:11:23.000000 metsrw-0.3.9/metsrw/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)    21931 2019-06-07 12:48:19.000000 metsrw-0.3.9/metsrw/mets.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/resources/
+-rw-r--r--   0 root         (0) root         (0)   155309 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/mets.xsd
+-rw-r--r--   0 root         (0) root         (0)    12087 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/archivematica_mets_schematron.xml
+-rw-r--r--   0 root         (0) root         (0)    12177 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/archivematica_mets_pointer_file_schematron.xml
+-rw-r--r--   0 root         (0) root         (0)    19559 2019-06-21 14:47:14.000000 metsrw-0.3.9/metsrw/fsentry.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/validate.py
+-rw-r--r--   0 root         (0) root         (0)     7050 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/di.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-06-21 17:23:24.000000 metsrw-0.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2019-06-21 17:23:24.000000 metsrw-0.3.9/PKG-INFO
```

### Comparing `metsrw-0.3.8/LICENSE` & `metsrw-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/validate.py` & `metsrw-0.3.9/metsrw/validate.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/mets.py` & `metsrw-0.3.9/metsrw/mets.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/resources/archivematica_mets_schematron.xml` & `metsrw-0.3.9/metsrw/resources/archivematica_mets_schematron.xml`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/resources/mets.xsd` & `metsrw-0.3.9/metsrw/resources/mets.xsd`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/resources/archivematica_mets_pointer_file_schematron.xml` & `metsrw-0.3.9/metsrw/resources/archivematica_mets_pointer_file_schematron.xml`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/di.py` & `metsrw-0.3.9/metsrw/di.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/fsentry.py` & `metsrw-0.3.9/metsrw/fsentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,20 @@
     wrapped copies of those XML files, which should be wrapped in
     MDWrap objects.
 
     :param str path: Path to the file on disk, as a bytestring. This will
         populate FLocat @xlink:href
     :param str label: Label in the structMap. If not provided, will be populated
         with the basename of path
+    :param str fileid: Provides a mechanism to assign a FILEID to an FSENTRY
+        when a pointer file is being created, so when a METS file is being
+        written for an package-file-type, i.e. an AIP. The FILE ID is an XML
+        NC (Non-colonized) name and so callers must understand the restricted
+        character-set of that type to use it properly. There is currently no
+        validation on this attribute on generation.
     :param str use: Use for the fileGrp.  Items with identical uses will be
         grouped together.
     :param str type: Type of FSEntry this is. This will appear in the structMap.
     :param list children: List of :class:`metsrw.fsentry.FSEntry` that are
         direct children of this element in the structMap.  Only allowed if type
         is 'Directory'
     :param str file_uuid: UUID of this entry. Will be used to construct the
@@ -108,14 +114,15 @@
     PREMIS_EVENT = "PREMIS:EVENT"
     PREMIS_AGENT = "PREMIS:AGENT"
     PREMIS_RIGHTS = "PREMIS:RIGHTS"
 
     def __init__(
         self,
         path=None,
+        fileid=None,
         label=None,
         use="original",
         type=u"Item",
         children=None,
         file_uuid=None,
         derived_from=None,
         checksum=None,
@@ -134,14 +141,15 @@
         else:  # TODO: Py3 is still using Unicode.
             if isinstance(path, six.binary_type):
                 self.path = path.decode("utf-8", errors="strict")
             else:
                 self.path = path
         if label is None and path is not None:
             label = os.path.basename(path)
+        self._fileid = fileid
         self.label = label
         self.use = use
         self.type = six.text_type(type)
         self.parent = None
         self._children = []
         if not transform_files:
             transform_files = []
@@ -200,14 +208,16 @@
         if self.type.lower() == "directory":
             return None
         if self.file_uuid is None:
             raise exceptions.MetsError(
                 "No FILEID: File %s does not have file_uuid set" % self.path
             )
         if self.is_aip:
+            if self._fileid:
+                return self._fileid
             return os.path.splitext(os.path.basename(self.path))[0]
         return utils.FILE_ID_PREFIX + self.file_uuid
 
     def group_id(self):
         """
         Returns the @GROUPID.
```

### Comparing `metsrw-0.3.8/metsrw/metadata.py` & `metsrw-0.3.9/metsrw/metadata.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/__init__.py` & `metsrw-0.3.9/metsrw/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     has_methods,
     is_class,
 )
 from . import plugins
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 __all__ = [
     "Agent",
     "AltRecordID",
     "AMDSec",
     "AM_PNTR_SCT_PATH",
     "AM_SCT_PATH",
```

### Comparing `metsrw-0.3.8/metsrw/plugins/premisrw/__init__.py` & `metsrw-0.3.9/metsrw/plugins/premisrw/__init__.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/plugins/premisrw/utils.py` & `metsrw-0.3.9/metsrw/plugins/premisrw/utils.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/plugins/premisrw/premis.py` & `metsrw-0.3.9/metsrw/plugins/premisrw/premis.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw/utils.py` & `metsrw-0.3.9/metsrw/utils.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/setup.py` & `metsrw-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/PKG-INFO` & `metsrw-0.3.9/metsrw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metsrw
-Version: 0.3.8
+Version: 0.3.9
 Summary: Library for dealing with METS files.
 Home-page: https://github.com/artefactual-labs/mets-reader-writer/
 Author: Artefactual
 Author-email: info@artefactual.com
 License: AGPL
 Description: [![PyPI version](https://badge.fury.io/py/metsrw.svg)](https://badge.fury.io/py/metsrw) [![Travis CI](https://travis-ci.org/artefactual-labs/mets-reader-writer.svg?branch=master)](https://travis-ci.org/artefactual-labs/mets-reader-writer) [![Coverage status](https://img.shields.io/coveralls/artefactual-labs/mets-reader-writer/master.svg)](https://coveralls.io/r/artefactual-labs/mets-reader-writer)
```

### Comparing `metsrw-0.3.8/README.md` & `metsrw-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.8/metsrw.egg-info/PKG-INFO` & `metsrw-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metsrw
-Version: 0.3.8
+Version: 0.3.9
 Summary: Library for dealing with METS files.
 Home-page: https://github.com/artefactual-labs/mets-reader-writer/
 Author: Artefactual
 Author-email: info@artefactual.com
 License: AGPL
 Description: [![PyPI version](https://badge.fury.io/py/metsrw.svg)](https://badge.fury.io/py/metsrw) [![Travis CI](https://travis-ci.org/artefactual-labs/mets-reader-writer.svg?branch=master)](https://travis-ci.org/artefactual-labs/mets-reader-writer) [![Coverage status](https://img.shields.io/coveralls/artefactual-labs/mets-reader-writer/master.svg)](https://coveralls.io/r/artefactual-labs/mets-reader-writer)
```

### Comparing `metsrw-0.3.8/metsrw.egg-info/SOURCES.txt` & `metsrw-0.3.9/metsrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

