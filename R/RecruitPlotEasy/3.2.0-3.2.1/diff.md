# Comparing `tmp/RecruitPlotEasy-3.2.0.tar.gz` & `tmp/RecruitPlotEasy-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecruitPlotEasy-3.2.0.tar", last modified: Fri May 19 20:02:24 2023, max compression
+gzip compressed data, was "RecruitPlotEasy-3.2.1.tar", last modified: Fri May 19 20:03:41 2023, max compression
```

## Comparing `RecruitPlotEasy-3.2.0.tar` & `RecruitPlotEasy-3.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.443920 RecruitPlotEasy-3.2.0/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:02:24.442922 RecruitPlotEasy-3.2.0/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.2.0/README.md
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.267882 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      767 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/SOURCES.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/dependency_links.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/entry_points.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/requires.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-05-19 20:02:23.000000 RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/top_level.txt
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.333576 RecruitPlotEasy-3.2.0/rpe2_code/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.2.0/rpe2_code/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_database.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     6982 2023-05-19 19:59:39.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_describe.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    38422 2023-05-19 19:59:26.000000 RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_plot.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      889 2023-05-19 20:00:42.000000 RecruitPlotEasy-3.2.0/rpe2_code/rpe2_main.py
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:02:24.440928 RecruitPlotEasy-3.2.0/rpe2_code/supports/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/agnostic_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/bam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/blast_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/cig_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/fasta_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/file_checker.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/mdz_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/protein_predictor.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.2.0/rpe2_code/supports/sam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-05-19 20:02:24.443920 RecruitPlotEasy-3.2.0/setup.cfg
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-05-19 20:02:12.000000 RecruitPlotEasy-3.2.0/setup.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:03:41.046563 RecruitPlotEasy-3.2.1/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:03:41.045149 RecruitPlotEasy-3.2.1/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.2.1/README.md
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:03:40.963487 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      767 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/entry_points.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/requires.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-05-19 20:03:40.000000 RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/top_level.txt
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:03:41.001786 RecruitPlotEasy-3.2.1/rpe2_code/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.2.1/rpe2_code/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_database.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     6982 2023-05-19 19:59:39.000000 RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_describe.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    38422 2023-05-19 19:59:26.000000 RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_plot.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      903 2023-05-19 20:03:23.000000 RecruitPlotEasy-3.2.1/rpe2_code/rpe2_main.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:03:41.043161 RecruitPlotEasy-3.2.1/rpe2_code/supports/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/agnostic_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/bam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/blast_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/cig_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/fasta_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/file_checker.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/mdz_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/protein_predictor.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.2.1/rpe2_code/supports/sam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-05-19 20:03:41.046563 RecruitPlotEasy-3.2.1/setup.cfg
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-05-19 20:02:54.000000 RecruitPlotEasy-3.2.1/setup.py
```

### Comparing `RecruitPlotEasy-3.2.0/RecruitPlotEasy.egg-info/SOURCES.txt` & `RecruitPlotEasy-3.2.1/RecruitPlotEasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_database.py` & `RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_database.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_describe.py` & `RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_describe.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/recruit_plot_easy_2_plot.py` & `RecruitPlotEasy-3.2.1/rpe2_code/recruit_plot_easy_2_plot.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/rpe2_main.py` & `RecruitPlotEasy-3.2.1/rpe2_code/rpe2_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 def main():
 	if len(sys.argv) < 2:
-		sys.exit("Please choose a module: either 'build' or 'plot'")
+		sys.exit("Please choose a module: either 'build' or 'plot' or 'describe'")
 	else:
 		action = sys.argv[1]
 		if action not in ["build", "plot", "describe"]:
 			print("I could not recognize your module:", action+".", "Please try again.")
 			sys.exit()
 		
 		if action == "build":
```

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/agnostic_reader.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/agnostic_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/bam_parser.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/bam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/blast_parser.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/blast_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/cig_parser.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/cig_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/fasta_reader.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/file_checker.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/file_checker.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/protein_predictor.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/protein_predictor.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/rpe2_code/supports/sam_parser.py` & `RecruitPlotEasy-3.2.1/rpe2_code/supports/sam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.0/setup.py` & `RecruitPlotEasy-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="RecruitPlotEasy",
-	version="3.2.0",
+	version="3.2.1",
 	author="Kenji Gerhardt",
 	author_email="kenji.gerhardt@gmail.com",
 	description="A tool for visualizing short read mapping efforts",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	include_package_data=True,
```

