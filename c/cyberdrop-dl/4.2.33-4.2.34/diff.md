# Comparing `tmp/cyberdrop-dl-4.2.33.tar.gz` & `tmp/cyberdrop-dl-4.2.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.33.tar", last modified: Fri May 19 14:10:14 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.34.tar", last modified: Fri May 19 14:12:22 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.33.tar` & `cyberdrop-dl-4.2.34.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.208771 cyberdrop-dl-4.2.33/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 14:10:14.208771 cyberdrop-dl-4.2.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.192771 cyberdrop-dl-4.2.33/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.196771 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.196771 cyberdrop-dl-4.2.33/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.204771 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.204771 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.208771 cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:14.192771 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 14:10:14.000000 cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-19 14:10:14.208771 cyberdrop-dl-4.2.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 14:10:00.000000 cyberdrop-dl-4.2.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.890464 cyberdrop-dl-4.2.34/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 14:12:22.890464 cyberdrop-dl-4.2.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.886464 cyberdrop-dl-4.2.34/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.886464 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.886464 cyberdrop-dl-4.2.34/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.890464 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.890464 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.890464 cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:12:22.886464 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 14:12:22.000000 cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-19 14:12:22.894464 cyberdrop-dl-4.2.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 14:12:13.000000 cyberdrop-dl-4.2.34/setup.py
```

### Comparing `cyberdrop-dl-4.2.33/LICENSE` & `cyberdrop-dl-4.2.34/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/PKG-INFO` & `cyberdrop-dl-4.2.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.33
+Version: 4.2.34
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.33 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.34 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.33/README.md` & `cyberdrop-dl-4.2.34/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.34/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.33
+Version: 4.2.34
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.33 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.34 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.33/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.34/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.33/setup.cfg` & `cyberdrop-dl-4.2.34/setup.cfg`

 * *Files identical despite different names*

