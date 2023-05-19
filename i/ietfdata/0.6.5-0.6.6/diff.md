# Comparing `tmp/ietfdata-0.6.5.tar.gz` & `tmp/ietfdata-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietfdata-0.6.5.tar", last modified: Wed Apr 19 18:48:12 2023, max compression
+gzip compressed data, was "ietfdata-0.6.6.tar", last modified: Fri May 19 14:15:00 2023, max compression
```

## Comparing `ietfdata-0.6.5.tar` & `ietfdata-0.6.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-04-19 18:48:12.869054 ietfdata-0.6.5/
--rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.6.5/LICENSE
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-04-19 18:48:12.868734 ietfdata-0.6.5/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     2529 2022-02-21 17:42:14.000000 ietfdata-0.6.5/README.md
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-04-19 18:48:12.862876 ietfdata-0.6.5/examples/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.6.5/examples/__init__.py
--rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.6.5/examples/bluesheets.py
--rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.6.5/examples/draft-authors.py
--rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.6.5/examples/draft-references.py
--rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.6.5/examples/draft-submissions-by-date.py
--rw-rw----   0 csp        (502) staff       (20)     1695 2022-11-03 14:42:34.000000 ietfdata-0.6.5/examples/draft-submissions.py
--rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.6.5/examples/drafts-for-person.py
--rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.6.5/examples/drafts-for-rfc.py
--rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.6.5/examples/drafts-for-wg.py
--rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.6.5/examples/emails-per-person.py
--rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.6.5/examples/non-wg-standards-track-rfcs.py
--rw-r--r--   0 csp        (502) staff       (20)     2084 2021-04-14 11:17:29.000000 ietfdata-0.6.5/examples/org-chart.py
--rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.6.5/examples/person-attendance.py
--rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.6.5/examples/person-emails.py
--rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.6.5/examples/person.py
--rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.6.5/examples/recent-pubreq.py
--rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.6.5/examples/rfc-data.py
--rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.6.5/examples/rfc-streams.py
--rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.6.5/examples/role-names.py
--rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.6.5/examples/wg-chairs.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-04-19 18:48:12.866724 ietfdata-0.6.5/ietfdata/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.5/ietfdata/__init__.py
--rw-rw----   0 csp        (502) staff       (20)   160702 2023-04-19 18:37:31.000000 ietfdata-0.6.5/ietfdata/datatracker.py
--rw-rw----   0 csp        (502) staff       (20)    16240 2022-04-28 14:40:41.000000 ietfdata-0.6.5/ietfdata/datatracker_ext.py
--rw-rw----   0 csp        (502) staff       (20)    25946 2022-10-28 08:25:24.000000 ietfdata-0.6.5/ietfdata/mailarchive.py
--rw-rw----   0 csp        (502) staff       (20)    22261 2022-08-29 10:29:34.000000 ietfdata-0.6.5/ietfdata/mailarchive2.py
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.5/ietfdata/py.typed
--rw-rw----   0 csp        (502) staff       (20)    24747 2022-02-13 18:30:57.000000 ietfdata-0.6.5/ietfdata/rfcindex.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-04-19 18:48:12.868367 ietfdata-0.6.5/ietfdata.egg-info/
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-04-19 18:48:12.000000 ietfdata-0.6.5/ietfdata.egg-info/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)      894 2023-04-19 18:48:12.000000 ietfdata-0.6.5/ietfdata.egg-info/SOURCES.txt
--rw-rw----   0 csp        (502) staff       (20)        1 2023-04-19 18:48:12.000000 ietfdata-0.6.5/ietfdata.egg-info/dependency_links.txt
--rw-rw----   0 csp        (502) staff       (20)      110 2023-04-19 18:48:12.000000 ietfdata-0.6.5/ietfdata.egg-info/requires.txt
--rw-rw----   0 csp        (502) staff       (20)       18 2023-04-19 18:48:12.000000 ietfdata-0.6.5/ietfdata.egg-info/top_level.txt
--rw-rw----   0 csp        (502) staff       (20)      100 2021-05-19 10:27:44.000000 ietfdata-0.6.5/pyproject.toml
--rw-rw----   0 csp        (502) staff       (20)       38 2023-04-19 18:48:12.869163 ietfdata-0.6.5/setup.cfg
--rw-rw----   0 csp        (502) staff       (20)      783 2023-04-19 18:07:13.000000 ietfdata-0.6.5/setup.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.240742 ietfdata-0.6.6/
+-rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.6.6/LICENSE
+-rw-rw----   0 csp        (502) staff       (20)     2970 2023-05-19 14:15:00.240053 ietfdata-0.6.6/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     2529 2022-02-21 17:42:14.000000 ietfdata-0.6.6/README.md
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.227342 ietfdata-0.6.6/examples/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.6.6/examples/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.6.6/examples/bluesheets.py
+-rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/draft-authors.py
+-rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.6.6/examples/draft-references.py
+-rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.6.6/examples/draft-submissions-by-date.py
+-rw-rw----   0 csp        (502) staff       (20)     1695 2022-11-03 14:42:34.000000 ietfdata-0.6.6/examples/draft-submissions.py
+-rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.6.6/examples/drafts-for-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.6.6/examples/drafts-for-rfc.py
+-rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/drafts-for-wg.py
+-rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.6.6/examples/emails-per-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/ietf-leadership.py
+-rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.6.6/examples/non-wg-standards-track-rfcs.py
+-rw-r--r--   0 csp        (502) staff       (20)     2084 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/org-chart.py
+-rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.6.6/examples/person-attendance.py
+-rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.6.6/examples/person-emails.py
+-rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.6.6/examples/person.py
+-rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.6.6/examples/recent-pubreq.py
+-rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.6.6/examples/rfc-data.py
+-rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.6.6/examples/rfc-streams.py
+-rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/role-names.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.235009 ietfdata-0.6.6/ietfdata/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.6/ietfdata/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)   160704 2023-05-19 14:12:42.000000 ietfdata-0.6.6/ietfdata/datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)    16240 2022-04-28 14:40:41.000000 ietfdata-0.6.6/ietfdata/datatracker_ext.py
+-rw-rw----   0 csp        (502) staff       (20)    25946 2022-10-28 08:25:24.000000 ietfdata-0.6.6/ietfdata/mailarchive.py
+-rw-rw----   0 csp        (502) staff       (20)    22261 2022-08-29 10:29:34.000000 ietfdata-0.6.6/ietfdata/mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.6/ietfdata/py.typed
+-rw-rw----   0 csp        (502) staff       (20)    24747 2022-02-13 18:30:57.000000 ietfdata-0.6.6/ietfdata/rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.239137 ietfdata-0.6.6/ietfdata.egg-info/
+-rw-rw----   0 csp        (502) staff       (20)     2970 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)      900 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/SOURCES.txt
+-rw-rw----   0 csp        (502) staff       (20)        1 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/dependency_links.txt
+-rw-rw----   0 csp        (502) staff       (20)      110 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/requires.txt
+-rw-rw----   0 csp        (502) staff       (20)       18 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/top_level.txt
+-rw-rw----   0 csp        (502) staff       (20)      100 2021-05-19 10:27:44.000000 ietfdata-0.6.6/pyproject.toml
+-rw-rw----   0 csp        (502) staff       (20)       38 2023-05-19 14:15:00.240954 ietfdata-0.6.6/setup.cfg
+-rw-rw----   0 csp        (502) staff       (20)      783 2023-05-19 14:12:49.000000 ietfdata-0.6.6/setup.py
```

### Comparing `ietfdata-0.6.5/LICENSE` & `ietfdata-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/PKG-INFO` & `ietfdata-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.6.5
+Version: 0.6.6
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: csp@csperkins.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.6.5/README.md` & `ietfdata-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/bluesheets.py` & `ietfdata-0.6.6/examples/bluesheets.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/draft-authors.py` & `ietfdata-0.6.6/examples/draft-authors.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/draft-references.py` & `ietfdata-0.6.6/examples/draft-references.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/draft-submissions-by-date.py` & `ietfdata-0.6.6/examples/draft-submissions-by-date.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/draft-submissions.py` & `ietfdata-0.6.6/examples/draft-submissions.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/drafts-for-person.py` & `ietfdata-0.6.6/examples/drafts-for-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/drafts-for-rfc.py` & `ietfdata-0.6.6/examples/drafts-for-rfc.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/drafts-for-wg.py` & `ietfdata-0.6.6/examples/drafts-for-wg.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/emails-per-person.py` & `ietfdata-0.6.6/examples/emails-per-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/non-wg-standards-track-rfcs.py` & `ietfdata-0.6.6/examples/non-wg-standards-track-rfcs.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/org-chart.py` & `ietfdata-0.6.6/examples/org-chart.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/person-attendance.py` & `ietfdata-0.6.6/examples/person-attendance.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/person-emails.py` & `ietfdata-0.6.6/examples/person-emails.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/person.py` & `ietfdata-0.6.6/examples/person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/recent-pubreq.py` & `ietfdata-0.6.6/examples/recent-pubreq.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/rfc-data.py` & `ietfdata-0.6.6/examples/rfc-data.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/rfc-streams.py` & `ietfdata-0.6.6/examples/rfc-streams.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/role-names.py` & `ietfdata-0.6.6/examples/role-names.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/examples/wg-chairs.py` & `ietfdata-0.6.6/examples/ietf-leadership.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/ietfdata/datatracker.py` & `ietfdata-0.6.6/ietfdata/datatracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,14 @@
     notify             : str
     expires            : Optional[str]
     type               : DocumentTypeURI
     rfc                : Optional[int]
     rev                : str           # If `rfc` is not None, `rev` will point to the RFC publication notice
     abstract           : str
     internal_comments  : str
-    order              : int
     note               : str
     ad                 : Optional[PersonURI]
     shepherd           : Optional[EmailURI]
     group              : Optional[GroupURI]
     stream             : Optional[StreamURI]
     intended_std_level : Optional[str]  # FIXME: should be a URI subtype?
     std_level          : Optional[str]  # FIXME: should be a URI subtype?
@@ -1042,14 +1041,15 @@
     remote_instructions : str
     short               : str
     attendees           : Optional[int]
     modified            : datetime
     comments            : str
     on_agenda           : bool
     purpose             : SessionPurposeURI
+    has_onsite_tool     : bool
 
 
 @dataclass(frozen=True)
 class SessionStatusNameURI(URI):
     root : str = "/api/v1/name/sessionstatusname/"
 
 
@@ -1727,15 +1727,15 @@
                 mongodb_pass = cache_pass
 
         logging.getLogger('requests_cache').setLevel('WARN')
 
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
         self.log = logging.getLogger("ietfdata")
 
-        self.ua        = "glasgow-ietfdata/0.6.5"          # Update when making a new relaase
+        self.ua        = "glasgow-ietfdata/0.6.6"          # Update when making a new relaase
         self.base_url  = os.environ.get("IETFDATA_DT_URL", "https://datatracker.ietf.org")
         self.http_req  = 0
         self.get_count = 0
 
         if use_cache:
             self.log.info(f"mongodb host = {mongodb_host}")
             self.log.info(f"mongodb port = {mongodb_port}")
```

### Comparing `ietfdata-0.6.5/ietfdata/datatracker_ext.py` & `ietfdata-0.6.6/ietfdata/datatracker_ext.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/ietfdata/mailarchive.py` & `ietfdata-0.6.6/ietfdata/mailarchive.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/ietfdata/mailarchive2.py` & `ietfdata-0.6.6/ietfdata/mailarchive2.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/ietfdata/rfcindex.py` & `ietfdata-0.6.6/ietfdata/rfcindex.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.5/ietfdata.egg-info/PKG-INFO` & `ietfdata-0.6.6/ietfdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.6.5
+Version: 0.6.6
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: csp@csperkins.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.6.5/ietfdata.egg-info/SOURCES.txt` & `ietfdata-0.6.6/ietfdata.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 examples/draft-references.py
 examples/draft-submissions-by-date.py
 examples/draft-submissions.py
 examples/drafts-for-person.py
 examples/drafts-for-rfc.py
 examples/drafts-for-wg.py
 examples/emails-per-person.py
+examples/ietf-leadership.py
 examples/non-wg-standards-track-rfcs.py
 examples/org-chart.py
 examples/person-attendance.py
 examples/person-emails.py
 examples/person.py
 examples/recent-pubreq.py
 examples/rfc-data.py
 examples/rfc-streams.py
 examples/role-names.py
-examples/wg-chairs.py
 ietfdata/__init__.py
 ietfdata/datatracker.py
 ietfdata/datatracker_ext.py
 ietfdata/mailarchive.py
 ietfdata/mailarchive2.py
 ietfdata/py.typed
 ietfdata/rfcindex.py
```

### Comparing `ietfdata-0.6.5/setup.py` & `ietfdata-0.6.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ietfdata",
-    version="0.6.5",
+    version="0.6.6",
     author="Colin Perkins",
     author_email="csp@csperkins.org",
     description="Access the IETF Data Tracker and RFC Index",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/glasgow-ipl/ietfdata",
     packages=setuptools.find_packages(),
```

