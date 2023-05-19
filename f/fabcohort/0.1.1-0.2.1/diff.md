# Comparing `tmp/fabcohort-0.1.1.tar.gz` & `tmp/fabcohort-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabcohort-0.1.1.tar", last modified: Fri May 19 14:09:34 2023, max compression
+gzip compressed data, was "fabcohort-0.2.1.tar", last modified: Fri May 19 14:27:56 2023, max compression
```

## Comparing `fabcohort-0.1.1.tar` & `fabcohort-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.958796 fabcohort-0.1.1/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:09:34.958633 fabcohort-0.1.1/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      337 2023-05-18 20:13:13.000000 fabcohort-0.1.1/README.md
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.957681 fabcohort-0.1.1/fab_cohort/
--rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.1.1/fab_cohort/__init__.py
--rw-r--r--   0 linliding   (501) staff       (20)     5113 2023-05-19 13:35:30.000000 fabcohort-0.1.1/fab_cohort/cohort.py
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.958438 fabcohort-0.1.1/fabcohort.egg-info/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/SOURCES.txt
--rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/dependency_links.txt
--rw-r--r--   0 linliding   (501) staff       (20)        7 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/requires.txt
--rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/top_level.txt
--rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-19 14:09:34.958855 fabcohort-0.1.1/setup.cfg
--rw-r--r--   0 linliding   (501) staff       (20)     1284 2023-05-19 11:02:52.000000 fabcohort-0.1.1/setup.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:27:56.013893 fabcohort-0.2.1/
+-rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:27:56.013727 fabcohort-0.2.1/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      337 2023-05-18 20:13:13.000000 fabcohort-0.2.1/README.md
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:27:56.012919 fabcohort-0.2.1/fab_cohort/
+-rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.1/fab_cohort/__init__.py
+-rw-r--r--   0 linliding   (501) staff       (20)     5119 2023-05-19 14:26:28.000000 fabcohort-0.2.1/fab_cohort/cohort.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:27:56.013523 fabcohort-0.2.1/fabcohort.egg-info/
+-rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:27:55.000000 fabcohort-0.2.1/fabcohort.egg-info/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-19 14:27:55.000000 fabcohort-0.2.1/fabcohort.egg-info/SOURCES.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-19 14:27:55.000000 fabcohort-0.2.1/fabcohort.egg-info/dependency_links.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       13 2023-05-19 14:27:55.000000 fabcohort-0.2.1/fabcohort.egg-info/requires.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-19 14:27:55.000000 fabcohort-0.2.1/fabcohort.egg-info/top_level.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-19 14:27:56.013946 fabcohort-0.2.1/setup.cfg
+-rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-05-19 14:27:33.000000 fabcohort-0.2.1/setup.py
```

### Comparing `fabcohort-0.1.1/PKG-INFO` & `fabcohort-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.1.1
+Version: 0.2.1
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `fabcohort-0.1.1/fab_cohort/cohort.py` & `fabcohort-0.2.1/fab_cohort/cohort.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         # Get unique segments
         unique_segment = df['segment'].unique()
         unique_segment_df = pd.DataFrame({'segment': unique_segment})
 
         # Perform cross join with time_series_df
         merged = unique_user_ids_df.assign(key=1).merge(time_series_df.assign(key=1)).drop('key', axis=1)
 
-        df_cross_join = merged.assign(key=1).merge(unique_segment.assign(key=1)).drop('key', axis=1)
+        df_cross_join = merged.assign(key=1).merge(unique_segment_df.assign(key=1)).drop('key', axis=1)
 
         df_cont = pd.merge(df_cross_join, df, how='left', on=['user_id', 'date', 'segment'])
         df_cont['count'].fillna(0, inplace=True)
 
         df_created = df.groupby(['user_id', 'segment'])['date'].min().reset_index()
         df_created.columns = ['user_id', 'segment', 'created']
 
@@ -77,15 +77,15 @@
 
         result = df_cont_created.groupby(['created', 'cohort', 'segment']).size().reset_index(name='count')
 
         # refine the results if dataset too sparse
         indexes_df = pd.DataFrame({'cohort': np.arange(len(time_series_df))})
 
         merged = time_series_df.assign(key=1).merge(indexes_df.assign(key=1)).drop('key', axis=1)
-        cross_join_df = merged.assign(key=1).merge(unique_segment.assign(key=1)).drop('key', axis=1)
+        cross_join_df = merged.assign(key=1).merge(unique_segment_df.assign(key=1)).drop('key', axis=1)
         cross_join_df['cohort'] = 't' + cross_join_df['cohort'].astype(int).astype(str)
         cross_join_df.rename(columns={'date': 'created'}, inplace=True)
 
 
         refined_result = pd.merge(cross_join_df, result, how='left', on=['created', 'cohort', 'segment'])
         return refined_result
```

### Comparing `fabcohort-0.1.1/fabcohort.egg-info/PKG-INFO` & `fabcohort-0.2.1/fabcohort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.1.1
+Version: 0.2.1
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `fabcohort-0.1.1/setup.py` & `fabcohort-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="fabcohort",
-    version="0.1.1",
+    version="0.2.1",
     description="for cohort analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linliD/fabcohort/",
     author="Linli Ding",
     author_email="linli@joinbonnet.com",
     license="MIT",
@@ -32,9 +32,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["fab_cohort"],
     include_package_data=True,
-    install_requires=["pandas"]
+    install_requires=["pandas", "numpy"]
 )
```

