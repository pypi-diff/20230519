# Comparing `tmp/beets_oldestdate-1.1.3.tar.gz` & `tmp/beets_oldestdate-1.1.4.tar.gz`

## Comparing `beets_oldestdate-1.1.3.tar` & `beets_oldestdate-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/.github/workflows/python-test.yml
--rw-r--r--   0        0        0    18564 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/beetsplug/oldestdate.py
--rw-r--r--   0        0        0    18787 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/beetsplug/test_oldestdate.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/LICENSE
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/beetsplug/oldestdate.py
+-rw-r--r--   0        0        0    19236 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/beetsplug/test_oldestdate.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/LICENSE
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/README.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 beets_oldestdate-1.1.4/PKG-INFO
```

### Comparing `beets_oldestdate-1.1.3/.github/workflows/python-test.yml` & `beets_oldestdate-1.1.4/.github/workflows/python-test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
-      - name: Install dependencies
+      - name: Install package and dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flake8
-          if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+          pip install .
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
       - name: Test with unittest
         run: |
-          python beetsplug/test_oldestdate.py
+          python beetsplug/test_oldestdate.py
```

### Comparing `beets_oldestdate-1.1.3/beetsplug/oldestdate.py` & `beets_oldestdate-1.1.4/beetsplug/oldestdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from beets import ui, config
 from beets.autotag import hooks
 from beets.importer import action
 from beets.plugins import BeetsPlugin
 
 musicbrainzngs.set_useragent(
     "Beets oldestdate plugin",
-    "1.1.2",
+    "1.1.4",
     "https://github.com/kernitus/beets-oldestdate"
 )
 
 
 # Extract first valid work_id from recording
 def _get_work_id_from_recording(recording):
     work_id = None
@@ -69,25 +69,25 @@
 class DateWrapper(datetime.datetime):
     """
     Wrapper class for datetime objects.
     Allows comparison between dates taking into
     account the month and day being optional.
     """
 
-    def __new__(cls, y=None, m=None, d=None, iso_string=None):
+    def __new__(cls, y: int = None, m: int = None, d: int = None, iso_string: str = None):
         """
         Create a new datetime object using a convenience wrapper.
         Must specify at least one of either year or iso_string.
         :param y: The year, as an integer
         :param m: The month, as an integer (optional)
         :param d: The day, as an integer (optional)
         :param iso_string: A string representing the date in the format YYYYMMDD. Month and day are optional.
         """
         if y is not None:
-            year = y
+            year = min(max(y, datetime.MINYEAR), datetime.MAXYEAR)
             month = m if (m is not None and 0 < m <= 12) else 1
             day = d if (d is not None and 0 < d <= 31) else 1
         elif iso_string is not None:
             parsed = parser.isoparse(iso_string)
             return datetime.datetime.__new__(cls, parsed.year, parsed.month, parsed.day)
         else:
             raise TypeError("Must specify a value for year or a date string")
@@ -97,15 +97,15 @@
     @classmethod
     def today(cls):
         today = datetime.date.today()
         return DateWrapper(today.year, today.month, today.day)
 
     def __init__(self, y=None, m=None, d=None, iso_string=None):
         if y is not None:
-            self.y = y
+            self.y = min(max(y, datetime.MINYEAR), datetime.MAXYEAR)
             self.m = m if (m is None or 0 < m <= 12) else 1
             self.d = d if (d is None or 0 < d <= 31) else 1
         elif iso_string is not None:
             # Remove any hyphen separators
             iso_string = iso_string.replace("-", "")
             length = len(iso_string)
 
@@ -176,22 +176,23 @@
             'overwrite_date': False,  # Overwrite date field in tags
             'filter_recordings': True,  # Skip recordings with attributes before fetching them
             'approach': 'releases',  # recordings, releases, hybrid, both
             'release_types': None,  # Filter by release type, e.g. ['Official']
             'use_file_date': False  # Also use file's embedded date when looking for oldest date
         })
 
-        if self.config['ignore_track_id']:
-            self.register_listener('import_task_created', self._import_task_created)
-        if self.config['prompt_missing_work_id']:
-            self.register_listener('import_task_choice', self._import_task_choice)
-        if self.config['filter_on_import']:
-            self.register_listener('trackinfo_received', self._import_trackinfo)
-            # Add heavy weight for missing work_id from a track
-            config['match']['distance_weights'].add({'work_id': 4})
+        if self.config['auto']:
+            if self.config['ignore_track_id']:
+                self.register_listener('import_task_created', self._import_task_created)
+            if self.config['prompt_missing_work_id']:
+                self.register_listener('import_task_choice', self._import_task_choice)
+            if self.config['filter_on_import']:
+                self.register_listener('trackinfo_received', self._import_trackinfo)
+                # Add heavy weight for missing work_id from a track
+                config['match']['distance_weights'].add({'work_id': 4})
 
         # Get global MusicBrainz host setting
         musicbrainzngs.set_hostname(config['musicbrainz']['host'].get())
         musicbrainzngs.set_rate_limit(1, config['musicbrainz']['ratelimit'].get())
 
         for recording_field in (
                 'recording_year',
```

### Comparing `beets_oldestdate-1.1.3/beetsplug/test_oldestdate.py` & `beets_oldestdate-1.1.4/beetsplug/test_oldestdate.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,27 @@
         self.assertEqual(1, result.m)
         self.assertEqual(10, result.d)
         result = oldestdate.DateWrapper(2022, 10, 0)
         self.assertEqual(2022, result.y)
         self.assertEqual(10, result.m)
         self.assertEqual(1, result.d)
 
+    # Force year to be within range 1 - 9999
+    def test_year_zero(self):
+        result = oldestdate.DateWrapper(0, 12, 10)
+        self.assertEqual(1, result.y)
+        self.assertEqual(12, result.m)
+        self.assertEqual(10, result.d)
+
+    def test_year_10000(self):
+        result = oldestdate.DateWrapper(10000, 12, 10)
+        self.assertEqual(9999, result.y)
+        self.assertEqual(12, result.m)
+        self.assertEqual(10, result.d)
+
     def test_less_than_year(self):
         first_date = oldestdate.DateWrapper(2021, 12, 10)
         second_date = oldestdate.DateWrapper(2022, 12, 10)
         self.assertTrue(first_date < second_date)
 
     def test_less_than_month(self):
         first_date = oldestdate.DateWrapper(2022, 11, 10)
```

### Comparing `beets_oldestdate-1.1.3/.gitignore` & `beets_oldestdate-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `beets_oldestdate-1.1.3/LICENSE` & `beets_oldestdate-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_oldestdate-1.1.3/README.md` & `beets_oldestdate-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `beets_oldestdate-1.1.3/pyproject.toml` & `beets_oldestdate-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "beets-oldestdate"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     { name="kernitus" },
 ]
 description = "Beets plugin that finds oldest possible track recording or release date"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `beets_oldestdate-1.1.3/PKG-INFO` & `beets_oldestdate-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-oldestdate
-Version: 1.1.3
+Version: 1.1.4
 Summary: Beets plugin that finds oldest possible track recording or release date
 Project-URL: Homepage, https://github.com/kernitus/beets-oldestdate
 Project-URL: Bug Tracker, https://github.com/kernitus/beets-oldestdate/issues
 Author: kernitus
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

