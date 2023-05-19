# Comparing `tmp/RecruitPlotEasy-3.2.2.tar.gz` & `tmp/RecruitPlotEasy-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecruitPlotEasy-3.2.2.tar", last modified: Fri May 19 20:06:41 2023, max compression
+gzip compressed data, was "RecruitPlotEasy-3.2.3.tar", last modified: Fri May 19 20:07:52 2023, max compression
```

## Comparing `RecruitPlotEasy-3.2.2.tar` & `RecruitPlotEasy-3.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:06:41.586219 RecruitPlotEasy-3.2.2/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:06:41.585224 RecruitPlotEasy-3.2.2/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.2.2/README.md
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:06:41.492595 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/PKG-INFO
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      767 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/SOURCES.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/dependency_links.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/entry_points.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/requires.txt
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-05-19 20:06:41.000000 RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/top_level.txt
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:06:41.542316 RecruitPlotEasy-3.2.2/rpe2_code/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.2.2/rpe2_code/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_database.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     7135 2023-05-19 20:06:08.000000 RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_describe.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    38578 2023-05-19 20:05:55.000000 RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_plot.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      903 2023-05-19 20:03:23.000000 RecruitPlotEasy-3.2.2/rpe2_code/rpe2_main.py
-drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:06:41.583229 RecruitPlotEasy-3.2.2/rpe2_code/supports/
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/__init__.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/agnostic_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/bam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/blast_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/cig_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/fasta_reader.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/file_checker.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/mdz_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/protein_predictor.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.2.2/rpe2_code/supports/sam_parser.py
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-05-19 20:06:41.586219 RecruitPlotEasy-3.2.2/setup.cfg
--rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-05-19 20:06:23.000000 RecruitPlotEasy-3.2.2/setup.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:07:52.597772 RecruitPlotEasy-3.2.3/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:07:52.595765 RecruitPlotEasy-3.2.3/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 15:17:49.000000 RecruitPlotEasy-3.2.3/README.md
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:07:52.503493 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      243 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/PKG-INFO
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      767 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        1 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       92 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/entry_points.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       28 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/requires.txt
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       10 2023-05-19 20:07:52.000000 RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/top_level.txt
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:07:52.555354 RecruitPlotEasy-3.2.3/rpe2_code/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       24 2022-11-02 16:46:51.000000 RecruitPlotEasy-3.2.3/rpe2_code/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    11443 2023-04-12 17:52:46.000000 RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_database.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     7160 2023-05-19 20:07:22.000000 RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_describe.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    38600 2023-05-19 20:07:32.000000 RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_plot.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      903 2023-05-19 20:03:23.000000 RecruitPlotEasy-3.2.3/rpe2_code/rpe2_main.py
+drwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2023-05-19 20:07:52.593771 RecruitPlotEasy-3.2.3/rpe2_code/supports/
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)        0 2022-11-02 16:51:28.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/__init__.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      996 2022-09-28 14:43:48.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/agnostic_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    42852 2023-04-11 18:28:56.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/bam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2169 2023-04-11 18:27:57.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/blast_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     1033 2022-09-28 19:11:20.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/cig_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      991 2022-09-30 16:44:49.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/fasta_reader.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2425 2023-04-12 16:58:55.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/file_checker.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      418 2022-09-28 16:56:11.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/mdz_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)    12522 2022-11-02 20:26:01.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/protein_predictor.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)     2597 2023-04-11 18:30:05.000000 RecruitPlotEasy-3.2.3/rpe2_code/supports/sam_parser.py
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)       38 2023-05-19 20:07:52.598758 RecruitPlotEasy-3.2.3/setup.cfg
+-rwxrwxrwx   0 kenji     (1000) kenji     (1000)      682 2023-05-19 20:07:40.000000 RecruitPlotEasy-3.2.3/setup.py
```

### Comparing `RecruitPlotEasy-3.2.2/RecruitPlotEasy.egg-info/SOURCES.txt` & `RecruitPlotEasy-3.2.3/RecruitPlotEasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_database.py` & `RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_database.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_describe.py` & `RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_describe.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,16 @@
 	if db is None:
 		print("You must supply a database. Quitting.")
 		parser.print_help()
 		sys.exit()
 	else:
 		if not os.path.exists(db):
 			print("Database", db, "could not be found.")
-			print("Have you created one with RecruitPlotEasy build yet?")
+			print("Have you created one with RecruitPlotEasy build yet? Quitting.")
+			sys.exit()
 	
 	mf = opts.mags_file
 	sf = opts.samps_file
 	hm = opts.heatmap
 	
 	if mf is None and sf is None and hm is None:
 		print("You must supply at least one output file. Quitting.")
```

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/recruit_plot_easy_2_plot.py` & `RecruitPlotEasy-3.2.3/rpe2_code/recruit_plot_easy_2_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1157,17 +1157,17 @@
 	if db is None:
 		print("You must supply a database. Quitting.")
 		parser.print_help()
 		sys.exit()
 	else:
 		if not os.path.exists(db):
 			print("Database", db, "could not be found.")
-			print("Have you created one with RecruitPlotEasy build yet?")
+			print("Have you created one with RecruitPlotEasy build yet?  Quitting.")
+			sys.exit()
 	
-		
 	do_proteins = opts.prot
 	
 	width = opts.width
 	height = opts.height
 	
 	out = opts.outdir
```

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/rpe2_main.py` & `RecruitPlotEasy-3.2.3/rpe2_code/rpe2_main.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/agnostic_reader.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/agnostic_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/bam_parser.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/bam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/blast_parser.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/blast_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/cig_parser.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/cig_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/fasta_reader.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/file_checker.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/file_checker.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/protein_predictor.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/protein_predictor.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/rpe2_code/supports/sam_parser.py` & `RecruitPlotEasy-3.2.3/rpe2_code/supports/sam_parser.py`

 * *Files identical despite different names*

### Comparing `RecruitPlotEasy-3.2.2/setup.py` & `RecruitPlotEasy-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="RecruitPlotEasy",
-	version="3.2.2",
+	version="3.2.3",
 	author="Kenji Gerhardt",
 	author_email="kenji.gerhardt@gmail.com",
 	description="A tool for visualizing short read mapping efforts",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	include_package_data=True,
```

