# Comparing `tmp/cyberdrop-dl-4.2.31.tar.gz` & `tmp/cyberdrop-dl-4.2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.31.tar", last modified: Thu May 18 19:01:55 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.32.tar", last modified: Fri May 19 05:52:23 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.31.tar` & `cyberdrop-dl-4.2.32.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.703730 cyberdrop-dl-4.2.31/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.707730 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.707730 cyberdrop-dl-4.2.31/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.703730 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 19:01:55.719730 cyberdrop-dl-4.2.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.155469 cyberdrop-dl-4.2.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 05:52:23.155469 cyberdrop-dl-4.2.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.147469 cyberdrop-dl-4.2.32/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.151469 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.151469 cyberdrop-dl-4.2.32/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.151469 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.155469 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.155469 cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:52:23.147469 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 05:52:23.000000 cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-19 05:52:23.155469 cyberdrop-dl-4.2.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 05:52:11.000000 cyberdrop-dl-4.2.32/setup.py
```

### Comparing `cyberdrop-dl-4.2.31/LICENSE` & `cyberdrop-dl-4.2.32/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/PKG-INFO` & `cyberdrop-dl-4.2.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.31
+Version: 4.2.32
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -126,15 +126,16 @@
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
 --config-file                   config file to read arguments from
 --db-file                       history database file to write to
---errored-urls-file             csv file to write failed download information to
+--errored-download-urls-file    csv file to write failed download information to
+--errored-scrape-urls-file      csv file to write failed scrape information to
 --log-file                      log file to write to
 --output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
 --unsupported-urls-file         csv file to output unsupported links into
 
 --exclude-audio         skip downloading of audio files
 --exclude-images        skip downloading of image files
 --exclude-other         skip downloading of images
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.31 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.32 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -113,18 +113,19 @@
 username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 Bulk downloader for multiple file hosts positional arguments: link link to
 content to download (passing multiple links is supported) optional arguments: -
 h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
-database file to write to --errored-urls-file csv file to write failed download
-information to --log-file log file to write to --output-last-forum-post-file
-text file to output last scraped post from a forum thread for re-feeding into
-CDL --unsupported-urls-file csv file to output unsupported links into --
+database file to write to --errored-download-urls-file csv file to write failed
+download information to --errored-scrape-urls-file csv file to write failed
+scrape information to --log-file log file to write to --output-last-forum-post-
+file text file to output last scraped post from a forum thread for re-feeding
+into CDL --unsupported-urls-file csv file to output unsupported links into --
 exclude-audio skip downloading of audio files --exclude-images skip downloading
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
```

### Comparing `cyberdrop-dl-4.2.31/README.md` & `cyberdrop-dl-4.2.32/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
 --config-file                   config file to read arguments from
 --db-file                       history database file to write to
---errored-urls-file             csv file to write failed download information to
+--errored-download-urls-file    csv file to write failed download information to
+--errored-scrape-urls-file      csv file to write failed scrape information to
 --log-file                      log file to write to
 --output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
 --unsupported-urls-file         csv file to output unsupported links into
 
 --exclude-audio         skip downloading of audio files
 --exclude-images        skip downloading of image files
 --exclude-other         skip downloading of images
```

#### html2text {}

```diff
@@ -107,18 +107,19 @@
 username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 Bulk downloader for multiple file hosts positional arguments: link link to
 content to download (passing multiple links is supported) optional arguments: -
 h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
-database file to write to --errored-urls-file csv file to write failed download
-information to --log-file log file to write to --output-last-forum-post-file
-text file to output last scraped post from a forum thread for re-feeding into
-CDL --unsupported-urls-file csv file to output unsupported links into --
+database file to write to --errored-download-urls-file csv file to write failed
+download information to --errored-scrape-urls-file csv file to write failed
+scrape information to --log-file log file to write to --output-last-forum-post-
+file text file to output last scraped post from a forum thread for re-feeding
+into CDL --unsupported-urls-file csv file to output unsupported links into --
 exclude-audio skip downloading of audio files --exclude-images skip downloading
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
             "socialmediagirls_username": "",
             "socialmediagirls_password": "",
             "xbunker_username": "",
             "xbunker_password": "",
         },
         "Files": {
             "db_file": "download_history.sqlite",
-            "errored_urls_file": "Errored_URLs.csv",
+            "errored_download_urls_file": "Errored_Download_URLs.csv",
+            "errored_scrape_urls_file": "Errored_Scrape_URLs.csv",
             "input_file": "URLs.txt",
             "log_file": "downloader.log",
             "output_folder": "Downloads",
             "output_last_forum_post_file": "URLs_last_post.txt",
             "unsupported_urls_file": "Unsupported_URLs.csv",
         },
         "Forum_Options": {
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import get_filename_and_ext, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class AnonfilesCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api_link = URL("https://api.anonfiles.com/v2/file")
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Anonfiles"""
         assert url.host is not None
         if 'cdn' in url.host:
             url = URL("https://anonfiles.com") / url.parts[1]
 
         album_obj = AlbumItem("Loose Anon Files", [])
@@ -44,13 +47,12 @@
                 if not complete:
                     await self.SQL_Helper.insert_media("anonfiles", "", media_item)
             else:
                 log(f"Dead: {url}", quiet=self.quiet, style="red")
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return album_obj
 
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,28 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class BunkrCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, remove_bunkr_id: bool):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, remove_bunkr_id: bool, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
         self.limiter = AsyncLimiter(20, 1)
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if "v" in url.parts or "d" in url.parts:
             media = await self.get_file(session, url)
@@ -124,14 +127,15 @@
             await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
             complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
             return MediaItem(link, url, complete, filename, ext, original_filename)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
+            await self.error_writer.write_errored_scrape(f"{url},{e}")
             logger.debug(e)
             return MediaItem(url, url, False, "", "", "")
 
     async def get_album(self, session: ScrapeSession, url: URL):
         """Iterates through an album and creates the media items"""
 
         ### Temp Fix ###
@@ -177,11 +181,10 @@
                 await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
                 complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
                 media = MediaItem(link, url, complete, filename, ext, original_filename)
                 await album.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return album
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import CascadeItem
 
 if TYPE_CHECKING:
     from bs4 import Tag
 
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
@@ -31,36 +32,38 @@
             self.next_page_selector = 'a[title="Next page"]'
         elif self.domain == "kemono":
             self.posts_selectors = ['article[class="post-card post-card--preview"] a', 'article[class="post-card"] a']
             self.next_page_selector = 'a[class=next]'
 
 
 class CoomenoCrawler:
-    def __init__(self, *, include_id=False, scraping_mapper, separate_posts=False, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, include_id=False, scraping_mapper, separate_posts=False, quiet: bool, SQL_Helper: SQLHelper,
+                 error_writer: ErrorFileWriter):
         self.include_id = include_id
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
         self.limiter = AsyncLimiter(15, 1)
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL):
         """Director for Coomer/Kemono scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
         title = None
         try:
             assert url.host is not None
             domain = next((domain for domain in ("coomer", "kemono") if domain in url.host), None)
             if domain:
                 title = await self.handle_coomeno(session, url, domain, cascade)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         await self.SQL_Helper.insert_cascade(cascade)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def handle_coomeno(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem) -> str:
         """Coomer/Kemono director function"""
@@ -116,16 +119,15 @@
             if next_page:
                 next_page = next_page.get('href')
                 if next_page:
                     await self.parse_profile(session, URL("https://" + url.host + next_page), spec, cascade)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return title
 
     async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
                          title: str = "") -> str:
         """Parses posts with supplied selectors"""
         try:
@@ -163,16 +165,15 @@
             for download in downloads:
                 await self.parse_tag(download, url, domain, title, cascade)
 
             text_content = soup.select('div[class=post__content] a')
             await self.map_links(text_content, title, url)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return title
 
     async def parse_tag(self, tag: Tag, url: URL, domain: str, title: str, cascade: CascadeItem):
         """Convert link from tag to MediaItem and add it to cascade"""
         href: Union[str, List[str], None] = tag.get('href')
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
 
 import contextlib
-from typing import TYPE_CHECKING, Optional, Tuple, List
+from typing import TYPE_CHECKING, Tuple, List
 
 from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class CyberFileCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
         self.file_details = URL('https://cyberfile.me/account/ajax/file_details')
         self.limiter = AsyncLimiter(10, 10)
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for cyberfile scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         domain_obj = DomainItem("cyberfile", {})
 
         download_links = []
         if 'folder' in url.parts:
@@ -62,16 +65,15 @@
             script_func = script_func.split('loadImages(')[-1]
             script_func = script_func.split(';')[0]
             nodeId = int(script_func.split(',')[1].replace("'", ""))
             return nodeId
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return 0
 
     async def get_folder_content(self, session: ScrapeSession, url: URL, nodeId: int, page: int, title=None):
         """Gets the content id's encased in a folder"""
         data = {"pageType": "folder", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
         nodes = []
         contents = []
@@ -112,16 +114,16 @@
             if page < total_pages:
                 contents.extend(await self.get_folder_content(session, url, nodeId, page+1, original_title))
             for node in nodes:
                 contents.extend(await self.get_folder_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return []
 
     async def get_single_contentId(self, session: ScrapeSession, url: URL) -> int:
         """Gets an individual content id"""
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
@@ -134,16 +136,15 @@
                     part_b = part_a.split(");")[0]
                     contentId = int(part_b)
                     return contentId
             return 0
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return 0
 
     async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page: int) -> Tuple[List, List]:
         """Gets folder id's and content id's from shared links"""
         try:
             # Initial page load to tell server, this is what we want.
             async with self.limiter:
@@ -185,16 +186,15 @@
                 nodes_temp, content_temp = await self.get_shared_ids_and_content(session, url, page + 1)
                 nodes.extend(nodes_temp)
                 contents.extend(content_temp)
             return nodes, contents
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return [], []
 
     async def get_shared_content(self, session, url: URL, nodeId: int, page: int, title=None) -> List:
         """Gets content from shared folders"""
         try:
             nodes = []
             contents = []
@@ -232,16 +232,15 @@
                 contents.extend(await self.get_shared_content(session, url, nodeId, page + 1, title))
             for title, node in nodes:
                 contents.extend(await self.get_shared_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return []
 
     async def get_download_links(self, session: ScrapeSession, url: URL, contentIds: List) -> List:
         """Obtains download links from content ids"""
         download_links = []
         try:
             for title, contentId in contentIds:
@@ -267,10 +266,9 @@
                     continue
 
                 download_links.append((title, media))
             return download_links
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return []
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,27 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import InvalidContentTypeFailure, NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class CyberdropCrawler:
-    def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.include_id = include_id
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Cyberdrop scraper"""
         album_obj = AlbumItem("Loose Cyberdrop Files", [])
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
@@ -65,14 +68,13 @@
                     logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 await album_obj.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return album_obj
 
         await self.SQL_Helper.insert_album("cyberdrop", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class EHentaiCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for E-Hentai"""
         album_obj = AlbumItem("Loose EHentai Files", [])
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         if "g" in url.parts:
             await self.get_album(session, url, album_obj)
@@ -52,24 +55,22 @@
             if next_page is not None:
                 next_page = URL(next_page.get('href'))
                 if next_page is not None:
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_image(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets media items from image links"""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("img[id=img]")
             link = URL(image.get('src'))
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "e-hentai")
             await album_obj.add_media(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class EromeCrawler:
-    def __init__(self, *, include_id: bool, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, include_id: bool, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director function for Erome scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if 'a' in url.parts:
             domain_obj = await self.handle_album(session, url)
         else:
@@ -63,16 +66,15 @@
                     logger.debug("Couldn't get extension for %s", link)
                     continue
                 await domain_obj.add_media(title, media)
 
             await self.SQL_Helper.insert_domain("erome", url, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return domain_obj
 
     async def handle_profile(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler for erome profiles, sends albums to handle_album"""
         domain_obj = DomainItem("erome", {})
         try:
@@ -93,11 +95,10 @@
             if next_page:
                 next_page = next_page.get("href").split("page=")[-1]
                 next_page = url.with_query(f"page={next_page}")
                 await domain_obj.extend(await self.handle_profile(session, next_page))
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return domain_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.data_classes import MediaItem
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class FapelloCrawler:
-    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Basic director for fapello"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if not str(url).endswith("/"):
             url = url / ""
 
@@ -60,16 +63,15 @@
                 if next_page:
                     await album_obj.extend(await self.parse_profile(session, URL(next_page)))
             await self.SQL_Helper.insert_album("fapello", url, album_obj)
             return album_obj
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return None
 
     async def parse_post(self, session: ScrapeSession, url: URL) -> list[MediaItem]:
         """Parses posts, returns list of MediaItem"""
         results = []
         try:
             soup = await session.get_BS4(url)
@@ -93,11 +95,10 @@
                     media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", download_link)
                     continue
                 results.append(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return results
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class GfycatCrawler:
-    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic scraper for gfycat"""
         album_obj = AlbumItem("Gfycat", [])
         try:
             log(f"Starting: {url}", quiet=self.quiet, style="green")
             soup = await session.get_BS4(url)
 
@@ -39,11 +42,10 @@
 
             media_item = await create_media_item(video_link, url, self.SQL_Helper, "gfycat")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("gfycat", video_link, album_obj)
             log(f"Finished: {url}", quiet=self.quiet, style="green")
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return album_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from yarl import URL
 
 from ..base_functions.base_functions import log, logger, make_title_safe, get_filename_and_ext
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class GoFileCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.limiter = AsyncLimiter(1, 1)
 
+        self.error_writer = error_writer
+
         self.api_address = URL("https://api.gofile.io")
         self.token = ""
 
     async def get_token(self, session: ScrapeSession, api_token=None):
         """Creates an anon gofile account to use."""
         if self.token:
             return
@@ -65,16 +68,15 @@
             for title, media_item in results:
                 await domain_obj.add_media(title, media_item)
 
             await self.SQL_Helper.insert_domain("gofile", url, domain_obj)
             log(f"Finished: {url}", quiet=self.quiet, style="green")
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return domain_obj
 
     async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None) -> List[List]:
         """Gets links from the given url, creates media_items"""
         results: List[List] = []
         params = {
@@ -83,16 +85,15 @@
             "websiteToken": "fghij",
         }
 
         async with self.limiter:
             content = await session.get_json(self.api_address / "getContent", params)
 
         if content["status"] != "ok":
-            logger.debug("Error encountered while handling %s", url)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
+            await self.error_writer.write_errored_scrape(url, Exception("Does Not Exist"), self.quiet)
             return results
 
         content = content['data']
         if title:
             title = title + "/" + await make_title_safe(content["name"])
         else:
             title = await make_title_safe(content["name"])
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class HGameCGCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic director for HGameCG"""
         album_obj = AlbumItem("Loose HGamesCG Files", [])
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         await self.get_album(session, url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
@@ -50,16 +53,15 @@
                 if next_page is not None:
                     assert url.host is not None
                     next_page = URL("https://" + url.host + next_page)
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_image(self, session: ScrapeSession, url: URL) -> URL:
         """Gets image link from the given url."""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("div[class=hgamecgimage] img")
             return URL(image.get('src'))
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,26 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class ImgBoxCrawler:
-    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director func for ImgBox scraping"""
         album_obj = AlbumItem("Loose ImgBox Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             if await check_direct(url):
@@ -50,16 +53,15 @@
             else:
                 img = await self.singular(session, url)
                 media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
                 await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         await self.SQL_Helper.insert_album("imgbox", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def folder(self, session: ScrapeSession, url: URL):
         """Gets links from a folder"""
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,26 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class LoveFapCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for lovefap scraping"""
         album_obj = AlbumItem("Loose LoveFap Files", [])
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "lovefap")
@@ -40,16 +43,15 @@
             if "video" in url.parts:
                 await self.fetch_video(session, url, album_obj)
             else:
                 await self.fetch_album(session, url, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return album_obj
 
         await self.SQL_Helper.insert_album("lovefap", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class NSFWXXXCrawler:
-    def __init__(self, quiet: bool, separate_posts: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, separate_posts: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for NSFW.XXX scraping"""
         domain_obj = DomainItem("nsfw.xxx", {})
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         if "user" in url.parts:
             await self.get_user(session, url, domain_obj)
@@ -51,16 +54,15 @@
 
                 posts = await self.get_post_hrefs(posts)
                 for post in posts:
                     await self.get_post(session, post, domain_obj, model)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_post_hrefs(self, posts) -> List:
         """Gets links from post objects"""
         posts_links = []
         for post in posts:
             url = URL(post.get("href"))
             if url not in posts_links:
@@ -90,9 +92,8 @@
                     continue
 
                 title = f"{model}/{post_name}" if self.separate_posts else model
                 await domain_obj.add_media(title, media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class PimpAndHostCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for pimpandhost scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
         if url.parts[1] == 'album':
             media_items, title = await self.get_listings(session, url)
@@ -43,29 +46,27 @@
             soup = await session.get_BS4(url)
             title = soup.select_one("div[class=image-header]")
             user_link = title.select_one("span[class=details]")
             user_link.decompose()
             title = await make_title_safe(title.get_text())
 
             for file in soup.select('a[class*="image-wrapper center-cropped im-wr"]'):
-                link = file.get("href")
+                link = URL(file.get("href"))
                 media_items.append(await self.get_singular(session, link))
             return media_items, title
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_singular(self, session: ScrapeSession, url: URL):
         """Handles singular files"""
         try:
             soup = await session.get_BS4(url)
             img = soup.select_one("a img")
             img = img.get("src")
             if img.startswith("//"):
                 img = URL("https:" + img)
             return await create_media_item(img, url, self.SQL_Helper, "pimpandhost")
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from yarl import URL
 
 from ..base_functions.base_functions import get_filename_and_ext, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class PixelDrainCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api = URL('https://pixeldrain.com/api/')
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for pixeldrain scraping"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
         identifier = str(url).split('/')[-1]
         if url.parts[1] == 'l':
@@ -54,16 +57,15 @@
                     logger.debug("Couldn't get extension for %s", link)
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 media_items.append(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         return media_items
 
     async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
         """Gets filename for the given file identifier"""
         content = await session.get_json(self.api / 'file' / identifier / 'info')
         return content['name']
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class PostImgCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for PostImg scraping"""
         album_obj = AlbumItem("Loose PostImg Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             if "gallery" in url.parts:
@@ -32,16 +35,15 @@
                     await album_obj.add_media(media_item)
             else:
                 media_item = await self.get_singular(session, url)
                 await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         await self.SQL_Helper.insert_album("postimg", url, album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_folder(self, session: ScrapeSession, url: URL) -> List:
         """Handles folder scraping"""
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class SaintCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic director for saint scraping"""
         album_obj = AlbumItem("Loose Saint Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one('video[id=main-video] source').get('src'))
             media_item = await create_media_item(link, url, self.SQL_Helper, "saint")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("saint", link, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,28 @@
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class ShareXCrawler:
-    def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.limiter = AsyncLimiter(10, 1)
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for ShareX scraper"""
         assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
@@ -75,16 +78,15 @@
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_albums(session, next_page, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
@@ -92,32 +94,30 @@
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_church_from_fish(link)
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str,
                                   domain_obj: DomainItem) -> None:
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             albums = soup.select("div[class=pad-content-listing] div")
             for album in albums:
                 album_url = album.get('data-url-short')
                 if album_url is not None:
                     album_url = URL(album_url)
                     await self.parse(session=session, url=album_url, og_title=og_title, domain_obj=domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for profiles"""
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             title = soup.select_one("div[class=header] h1 strong").get_text()
@@ -127,16 +127,15 @@
                 titlep2 = url.name
                 title = title + " - " + titlep2
             title = await make_title_safe(title.replace(r"\n", "").strip())
             await self.get_list_links(session, url, title, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem) -> None:
         """Gets final links and adds to domain_obj"""
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             assert url.host is not None
@@ -162,16 +161,15 @@
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_list_links(session, next_page, title, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
     async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem) -> None:
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
 
             title = soup.select_one("a[data-text=album-name]").get_text()
@@ -190,9 +188,8 @@
                 await self.get_sub_album_links(session, sub_albums, title, domain_obj)
             finally:
                 list_recent = URL(soup.select_one("a[id=list-most-recent-link]").get("href"))
                 await self.get_list_links(session, list_recent, title, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class XBunkrCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for XBunkr scraping"""
         album_obj = AlbumItem("Loose XBunkr Files", [])
 
         try:
             assert url.host is not None
             if "media" in url.host:
@@ -41,13 +44,12 @@
                     except NoExtensionFailure:
                         logger.debug("Couldn't get extension for %s", link)
                         continue
                     await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error scraping {url}", quiet=self.quiet)
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
 
         await self.SQL_Helper.insert_album("xbunkr", URL(""), album_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from ..base_functions.data_classes import CascadeItem, MediaItem
 from ..base_functions.error_classes import FailedLoginFailure, NoExtensionFailure
 
 if TYPE_CHECKING:
     import bs4
 
+    from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
@@ -135,15 +136,16 @@
     domains = {
         "nudostar": "NudoStar",
         "simpcity": "SimpCity",
         "socialmediagirls": "SocialMediaGirls",
         "xbunker": "XBunker",
     }
 
-    def __init__(self, *, scraping_mapper, args: Dict, SQL_Helper: SQLHelper, quiet: bool):
+    def __init__(self, *, scraping_mapper, args: Dict, SQL_Helper: SQLHelper, quiet: bool,
+                 error_writer: ErrorFileWriter):
         self.include_id = args["Runtime"]["include_id"]
         self.quiet = quiet
 
         self.scrape_single_post = args["Forum_Options"]["scrape_single_post"]
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.output_last = args["Forum_Options"]["output_last_forum_post"]
         self.output_last_file = args["Files"]["output_last_forum_post_file"]
@@ -153,14 +155,16 @@
                                           auth_args[f"{domain}_username"],
                                           auth_args[f"{domain}_password"])
                        for domain, name in self.domains.items()}
 
         self.scraping_mapper = scraping_mapper
         self.SQL_Helper = SQL_Helper
 
+        self.error_writer = error_writer
+
     async def fetch(self, session: ScrapeSession, url: URL) -> Tuple[CascadeItem, str]:
         """Xenforo forum director"""
         log(f"Starting: {url}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
 
         scrape_url, post_num = await self.get_thread_url_and_post_num(url)
         title = ""
@@ -169,16 +173,15 @@
             domain = next((domain for domain in self.domains if domain in url.host), None)
             if domain:
                 parse_spec = ParseSpec(domain)
                 await self.forums[domain].login(session, url, parse_spec, self.quiet)
                 title = await self.parse_forum(session, scrape_url, parse_spec, cascade, "", post_num)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
-            log(f"Error: {url}", quiet=self.quiet, style="red")
-            logger.debug(e)
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             return cascade, ""
 
         await self.SQL_Helper.insert_cascade(cascade)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def get_thread_url_and_post_num(self, url: URL):
@@ -331,10 +334,11 @@
                 await self.parse_forum(session, next_page, spec, cascade, title, post_number)
         elif self.output_last:
             assert url.raw_name is not None
             if 'page-' in url.raw_name or 'post-' in url.raw_name:
                 last_post_url = url.parent / post_num_str
             else:
                 last_post_url = url / post_num_str
+            await self.error_writer.write_last_post(last_post_url)
             async with aiofiles.open(self.output_last_file, mode='a') as f:
                 await f.write(f'{last_post_url}\n')
         return title
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import contextlib
 import itertools
 import logging
 from http import HTTPStatus
 from random import gauss
 from typing import TYPE_CHECKING, Any, Dict, Tuple, Coroutine, List, Optional
 
-import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
     log,
     logger,
@@ -41,37 +40,40 @@
 from .progress_definitions import (
     OverallFileProgress,
     ProgressMaster,
 )
 
 if TYPE_CHECKING:
     from pathlib import Path
-
     from rich.progress import TaskID
 
+    from cyberdrop_dl.base_functions.base_functions import ErrorFileWriter
+
 
 def _limit_concurrency(coroutines: List[Coroutine], semaphore: Optional[asyncio.Semaphore]) -> List[Coroutine]:
     if not semaphore:
         return coroutines
 
     async def limit_concurrency(coroutine: Coroutine) -> Coroutine:
         async with semaphore:
             return await coroutine
 
     return [limit_concurrency(coroutine) for coroutine in coroutines]
 
 
 class CDLHelper:
-    def __init__(self, args: Dict, client: Client, files: OverallFileProgress, SQL_Helper: SQLHelper):
+    def __init__(self, args: Dict, client: Client, files: OverallFileProgress, SQL_Helper: SQLHelper,
+                 error_writer: ErrorFileWriter):
         self.args = args
 
         # CDL Objects
         self.client = client
         self.files = files
         self.SQL_Helper = SQL_Helper
+        self.error_writer = error_writer
         self.File_Lock = FileLock()
 
         # Limits
         self.delay = {'cyberdrop': 1.0, 'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
 
         # Exclude Args
         self.exclude_audio = args["Ignore"]["exclude_audio"]
@@ -89,18 +91,14 @@
         self.required_free_space = args["Runtime"]["required_free_space"]
 
         # Concurrency Limits
         self.threads_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_threads"]) if args["Runtime"]["max_concurrent_threads"] else None
         self.domains_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_domains"]) if args["Runtime"]["max_concurrent_domains"] else None
         self.albums_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_albums"]) if args["Runtime"]["max_concurrent_albums"] else None
 
-        # Output Args
-        self.errored_output = args['Runtime']['output_errored_urls']
-        self.errored_file = args['Files']['errored_urls_file']
-
         # API Keys
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
     def get_throttle(self, domain: str) -> float:
         """Get the throttle for a domain"""
         if domain in self.delay:
             return self.delay[domain]
@@ -240,17 +238,15 @@
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     def can_retry(self, url_path: str) -> bool:
         return self.CDL_Helper.disable_attempt_limit or self.current_attempt[url_path] < self.CDL_Helper.allowed_attempts - 1
 
     async def handle_failed(self, media: MediaItem, e: Any) -> None:
         self.CDL_Helper.files.add_failed()
-        if self.CDL_Helper.errored_output:
-            async with aiofiles.open(self.CDL_Helper.errored_file, mode='a') as file:
-                await file.write(f"{media.url},{media.referer},{e.message}\n")
+        await self.CDL_Helper.error_writer.write_errored_download(media.url, media.referer, e.message)
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str, current_throttle: float):
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
@@ -316,18 +312,18 @@
     async def get_downloader(self, domain: str):
         if domain not in self.downloaders:
             return await self.create_downloader(domain)
         return self.downloaders[domain]
 
 
 class DownloadDirector:
-    def __init__(self, args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client):
+    def __init__(self, args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client,
+                 error_writer: ErrorFileWriter):
         self.Progress_Master = ProgressMaster(args["Progress_Options"])
-        self.CDL_Helper = CDLHelper(args, client, self.Progress_Master.OverallFileProgress, SQL_Helper)
-
+        self.CDL_Helper = CDLHelper(args, client, self.Progress_Master.OverallFileProgress, SQL_Helper, error_writer)
         self.Download_Manager = DownloadManager(self.CDL_Helper, self.Progress_Master)
 
         self.Forums = Forums
 
     async def start(self):
         self.CDL_Helper.files.update_total(await self.Forums.get_total())
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import itertools
 import logging
 from http import HTTPStatus
 from pathlib import Path
 from random import gauss
 from typing import Dict, Any
 
-import aiofiles
 import aiohttp.client_exceptions
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
+    ErrorFileWriter,
     log,
     logger,
 )
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, DomainItem, FileLock, ForumItem, MediaItem
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper, get_db_path
 from cyberdrop_dl.client.client import Client, DownloadSession
@@ -55,26 +55,24 @@
         self.progress.update(1)
 
 
 class Old_Downloader:
     """Downloader class, directs downloading for domain objects"""
 
     def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper,
-                 domain: str, domain_obj: DomainItem, files: Files):
+                 domain: str, domain_obj: DomainItem, files: Files, error_writer: ErrorFileWriter):
         self.client = client
         self.download_session = DownloadSession(client)
+        self.error_writer = error_writer
         self.File_Lock = FileLock()
         self.SQL_Helper = SQL_Helper
 
         self.domain = domain
         self.domain_obj = domain_obj
 
-        self.errored_output = args['Runtime']['output_errored_urls']
-        self.errored_file = args['Files']['errored_urls_file']
-
         self.files = files
 
         self.current_attempt: Dict[str, int] = {}
         max_workers = get_threads_number(args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.delay = {'cyberfile': 1, 'anonfiles': 1, "coomer": 0.2, "kemono": 0.2}
 
@@ -221,17 +219,15 @@
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     def can_retry(self, url_path: str) -> bool:
         return self.disable_attempt_limit or self.current_attempt[url_path] < self.allowed_attempts - 1
 
     async def handle_failed(self, media: MediaItem, e: Any) -> None:
         self.files.add_failed()
-        if self.errored_output:
-            async with aiofiles.open(self.errored_file, mode='a') as file:
-                await file.write(f"{media.url},{media.referer},{e.message}\n")
+        await self.error_writer.write_errored_download(media.url, media.referer, e.message)
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str,
                                 current_throttle: float) -> tuple[Path, Path, bool]:
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 import re
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import Dict, List
 
-import aiofiles
 from yarl import URL
 
-from cyberdrop_dl.base_functions.base_functions import clear, log, purge_dir
+from cyberdrop_dl.base_functions.base_functions import clear, log, purge_dir, ErrorFileWriter
 from cyberdrop_dl.base_functions.config_manager import document_args, run_args
 from cyberdrop_dl.base_functions.config_schema import config_default
 from cyberdrop_dl.base_functions.sorting_functions import Sorter
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 from cyberdrop_dl.client.client import Client
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
 from cyberdrop_dl.downloader.downloaders import DownloadDirector
 from cyberdrop_dl.downloader.old_downloaders import old_download_forums
 from cyberdrop_dl.scraper.Scraper import ScrapeMapper
 
 from . import __version__ as VERSION
-from .base_functions.data_classes import CascadeItem, ForumItem, SkipData
+from .base_functions.data_classes import ForumItem, SkipData
 
 
 def parse_args() -> argparse.Namespace:
     """Parses the command line arguments passed into the program"""
     parser = argparse.ArgumentParser(description="Bulk downloader for multiple file hosts")
     parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {VERSION}")
 
@@ -35,35 +34,31 @@
     config_group = config_data["Files"]
     path_opts = parser.add_argument_group("Path options")
     path_opts.add_argument("-i", "--input-file", type=Path, help="file containing links to download (default: %(default)s)", default=config_group["input_file"])
     path_opts.add_argument("-o", "--output-folder", type=Path, help="folder to download files to (default: %(default)s)", default=config_group["output_folder"])
 
     path_opts.add_argument("--config-file", type=Path, help="config file to read arguments from (default: %(default)s)", default="config.yaml")
     path_opts.add_argument("--db-file", type=Path, help="history database file to write to (default: %(default)s)", default=config_group["db_file"])
-    path_opts.add_argument("--errored-urls-file", type=Path, default=config_group["errored_urls_file"], 
-                           help="csv file to write failed download information to (default: %(default)s)")
+    path_opts.add_argument("--errored-download-urls-file", type=Path, default=config_group["errored_download_urls_file"], help="csv file to write failed download information to (default: %(default)s)")
+    path_opts.add_argument("--errored-scrape-urls-file", type=Path, default=config_group["errored_scrape_urls_file"], help="csv file to write failed scrape information to (default: %(default)s)")
     path_opts.add_argument("--log-file", type=Path, help="log file to write to (default: %(default)s)", default=config_group["log_file"])
-    path_opts.add_argument("--output-last-forum-post-file", type=Path, default=config_group["output_last_forum_post_file"],
-                           help="the text file to output last scraped post from a forum thread for re-feeding into CDL (default: %(default)s)")
-    path_opts.add_argument("--unsupported-urls-file", type=Path, default=config_group["unsupported_urls_file"],
-                           help="the csv file to output unsupported links into (default: %(default)s)")
+    path_opts.add_argument("--output-last-forum-post-file", type=Path, default=config_group["output_last_forum_post_file"], help="the text file to output last scraped post from a forum thread for re-feeding into CDL (default: %(default)s)")
+    path_opts.add_argument("--unsupported-urls-file", type=Path, default=config_group["unsupported_urls_file"], help="the csv file to output unsupported links into (default: %(default)s)")
 
     # Ignore
     config_group = config_data["Ignore"]
     ignore_opts = parser.add_argument_group("Ignore options")
     ignore_opts.add_argument("--exclude-audio", help="skip downloading of audio files", action="store_true")
     ignore_opts.add_argument("--exclude-images", help="skip downloading of image files", action="store_true")
     ignore_opts.add_argument("--exclude-other", help="skip downloading of images", action="store_true")
     ignore_opts.add_argument("--exclude-videos", help="skip downloading of video files", action="store_true")
     ignore_opts.add_argument("--ignore-cache", help="ignores previous runs cached scrape history", action="store_true")
     ignore_opts.add_argument("--ignore-history", help="ignores previous download history", action="store_true")
-    ignore_opts.add_argument("--skip-hosts", choices=SkipData.supported_hosts, action="append",
-                             help="removes host links from downloads", default=config_group["skip_hosts"])
-    ignore_opts.add_argument("--only-hosts", choices=SkipData.supported_hosts, action="append",
-                             help="only allows downloads from these hosts", default=config_group["only_hosts"])
+    ignore_opts.add_argument("--skip-hosts", choices=SkipData.supported_hosts, action="append", help="removes host links from downloads", default=config_group["skip_hosts"])
+    ignore_opts.add_argument("--only-hosts", choices=SkipData.supported_hosts, action="append", help="only allows downloads from these hosts", default=config_group["only_hosts"])
 
     # Runtime arguments
     config_group = config_data["Runtime"]
     runtime_opts = parser.add_argument_group("Runtime options")
     runtime_opts.add_argument("--allow-insecure-connections", help="allows insecure connections from content hosts", action="store_true")
     runtime_opts.add_argument("--attempts", type=int, help="number of attempts to download each file (default: %(default)s)", default=config_group["attempts"])
     runtime_opts.add_argument("--block-sub-folders", help="block sub folders from being created", action="store_true")
@@ -142,43 +137,54 @@
     progress_opts.add_argument("--visible-rows-files", type=int, help="number of visiblerows to use for the files table (default: %(default)s)", default=config_group["visible_rows_files"])
 
     # Links
     parser.add_argument("links", metavar="link", nargs="*", help="link to content to download (passing multiple links is supported)", default=[])
     return parser.parse_args()
 
 
-async def file_management(args: Dict, links: List) -> None:
+async def file_management(args: Dict, links: List) -> ErrorFileWriter:
     """We handle file defaults here (resetting and creation)"""
     input_file = args['Files']['input_file']
     if not input_file.is_file() and not links:
         input_file.touch()
 
     Path(args['Files']['output_folder']).mkdir(parents=True, exist_ok=True)
 
+    error_writer = ErrorFileWriter(args['Runtime']['output_errored_urls'], args['Runtime']['output_unsupported_urls'],
+                                   args['Forum_Options']['output_last_forum_post'], args['Files']['errored_scrape_urls_file'],
+                                   args['Files']['errored_download_urls_file'], args['Files']['unsupported_urls_file'],
+                                   args['Files']['output_last_forum_post_file'])
+
     if args['Forum_Options']['output_last_forum_post']:
         output_url_file = args['Files']['output_last_forum_post_file']
         if output_url_file.exists():
             output_url_file.unlink()
             output_url_file.touch()
 
     if args['Runtime']['output_unsupported_urls']:
         unsupported_urls = args['Files']['unsupported_urls_file']
         if unsupported_urls.exists():
             unsupported_urls.unlink()
             unsupported_urls.touch()
-            async with aiofiles.open(unsupported_urls, mode='w') as f:
-                await f.write("URL,REFERER,TITLE\n")
+            await error_writer.write_unsupported_header()
 
     if args['Runtime']['output_errored_urls']:
-        errored_urls = args['Files']['errored_urls_file']
+        errored_urls = args['Files']['errored_download_urls_file']
+        if errored_urls.exists():
+            errored_urls.unlink()
+            errored_urls.touch()
+            await error_writer.write_errored_download_header()
+
+        errored_urls = args['Files']['errored_scrape_urls_file']
         if errored_urls.exists():
             errored_urls.unlink()
             errored_urls.touch()
-            async with aiofiles.open(errored_urls, mode='w') as f:
-                await f.write("URL,REFERER,REASON\n")
+            await error_writer.write_errored_scrape_header()
+
+    return error_writer
 
 
 async def regex_links(urls: List) -> List:
     """Regex grab the links from the URLs.txt file"""
     """This allows code blocks or full paragraphs to be copy and pasted into the URLs.txt"""
     yarl_links = []
     for line in urls:
@@ -227,50 +233,50 @@
     return Forums
 
 
 async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
-    await file_management(args, links)
     log(f"We are running version {VERSION} of Cyberdrop Downloader")
+    error_writer = await file_management(args, links)
 
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
         log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
         exit(1)
 
     links = await consolidate_links(args, links)
     client = Client(args['Ratelimiting']['ratelimit'], args['Ratelimiting']['throttle'],
                     args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"],
                     args['Runtime']['user_agent'])
     SQL_Helper = SQLHelper(args['Ignore']['ignore_history'], args['Ignore']['ignore_cache'], args['Files']['db_file'])
-    Scraper = ScrapeMapper(args, client, SQL_Helper, False)
+    Scraper = ScrapeMapper(args, client, SQL_Helper, False, error_writer)
 
     await SQL_Helper.sql_initialize()
 
     if links:
         Forums = await scrape_links(Scraper, links)
         await asyncio.sleep(5)
         await clear()
 
         if args['Progress_Options']['hide_new_progress']:
             if not await Forums.is_empty():
                 await old_download_forums(args, Forums, SQL_Helper, client)
         else:
             if not await Forums.is_empty():
-                download_director = DownloadDirector(args, Forums, SQL_Helper, client)
+                download_director = DownloadDirector(args, Forums, SQL_Helper, client, error_writer)
                 await download_director.start()
 
     if args['Files']['output_folder'].is_dir():
         if args['Sorting']['sort_downloads']:
             log("")
             log("Sorting Downloads")
             sorter = Sorter(args['Files']['output_folder'], args['Sorting']['sort_directory'],
                             args['Sorting']['sorted_audio'], args['Sorting']['sorted_images'],
-                            args['Sorting']['sorted_videos'], args['Sorting']['sorted_others'],)
+                            args['Sorting']['sorted_videos'], args['Sorting']['sorted_others'])
             await sorter.sort()
 
         log("")
         log("Checking for incomplete downloads")
         partial_downloads = any(f.is_file() for f in args['Files']['output_folder'].rglob("*.part"))
         temp_downloads = any(Path(f).is_file() for f in await SQL_Helper.get_temp_names())
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.32/cyberdrop_dl/scraper/Scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Optional, Dict
 
-import aiofiles
-from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.crawlers.Anonfiles_Spider import AnonfilesCrawler
 from cyberdrop_dl.crawlers.Bunkr_Spider import BunkrCrawler
@@ -30,30 +28,30 @@
 from cyberdrop_dl.crawlers.Saint_Spider import SaintCrawler
 from cyberdrop_dl.crawlers.ShareX_Spider import ShareXCrawler
 from cyberdrop_dl.crawlers.XBunkr_Spider import XBunkrCrawler
 from cyberdrop_dl.crawlers.Xenforo_Spider import XenforoCrawler
 from cyberdrop_dl.scraper.JDownloader_Integration import JDownloader
 
 if TYPE_CHECKING:
+    from cyberdrop_dl.base_functions.base_functions import ErrorFileWriter
     from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 
 
 class ScrapeMapper:
     """This class maps links to their respective handlers, or JDownloader if they are unsupported"""
-    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
+    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool, error_writer: ErrorFileWriter):
         self.args = args
         self.client = client
         self.SQL_Helper = SQL_Helper
         self.Cascade = CascadeItem({})
         self.Forums = ForumItem({})
         self.skip_data = SkipData(args['Ignore']['skip_hosts'])
         self.only_data = SkipData(args['Ignore']['only_hosts'])
 
-        self.unsupported_file = args["Files"]["unsupported_urls_file"]
-        self.unsupported_output = args['Runtime']['output_unsupported_urls']
+        self.error_writer = error_writer
 
         self.anonfiles_crawler: Optional[AnonfilesCrawler] = None
         self.bunkr_crawler: Optional[BunkrCrawler] = None
         self.cyberdrop_crawler: Optional[CyberdropCrawler] = None
         self.coomeno_crawler: Optional[CoomenoCrawler] = None
         self.cyberfile_crawler: Optional[CyberFileCrawler] = None
         self.ehentai_crawler: Optional[EHentaiCrawler] = None
@@ -120,181 +118,199 @@
         await self.map_url(url, title)
 
     """Regular file host handling"""
 
     async def Anonfiles(self, url: URL, title=None):
         anonfiles_session = ScrapeSession(self.client)
         if not self.anonfiles_crawler:
-            self.anonfiles_crawler = AnonfilesCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.anonfiles_crawler = AnonfilesCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                      error_writer=self.error_writer)
         album_obj = await self.anonfiles_crawler.fetch(anonfiles_session, url)
         await self._handle_album_additions("anonfiles", album_obj, title)
         await anonfiles_session.exit_handler()
 
     async def Bunkr(self, url: URL, title=None):
         bunkr_session = ScrapeSession(self.client)
         if not self.bunkr_crawler:
             self.bunkr_crawler = BunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
-                                              remove_bunkr_id=self.remove_bunkr_id)
+                                              remove_bunkr_id=self.remove_bunkr_id, error_writer=self.error_writer)
 
         album_obj = await self.bunkr_crawler.fetch(bunkr_session, url)
         if not await album_obj.is_empty():
             await self._handle_album_additions("bunkr", album_obj, title)
         await bunkr_session.exit_handler()
 
     async def Cyberdrop(self, url: URL, title=None):
         cyberdrop_session = ScrapeSession(self.client)
         if not self.cyberdrop_crawler:
-            self.cyberdrop_crawler = CyberdropCrawler(include_id=self.include_id, quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.cyberdrop_crawler = CyberdropCrawler(include_id=self.include_id, quiet=self.quiet,
+                                                      SQL_Helper=self.SQL_Helper, error_writer=self.error_writer)
         album_obj = await self.cyberdrop_crawler.fetch(cyberdrop_session, url)
         await self._handle_album_additions("cyberdrop", album_obj, title)
         await cyberdrop_session.exit_handler()
 
     async def CyberFile(self, url, title=None):
         cyberfile_session = ScrapeSession(self.client)
         if not self.cyberfile_crawler:
-            self.cyberfile_crawler = CyberFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.cyberfile_crawler = CyberFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                      error_writer=self.error_writer)
 
         domain_obj = await self.cyberfile_crawler.fetch(cyberfile_session, url)
         await self._handle_domain_additions("cyberfile", domain_obj, title)
         await cyberfile_session.exit_handler()
 
     async def EHentai(self, url, title=None):
         ehentai_session = ScrapeSession(self.client)
         if not self.ehentai_crawler:
-            self.ehentai_crawler = EHentaiCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.ehentai_crawler = EHentaiCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                  error_writer=self.error_writer)
         album_obj = await self.ehentai_crawler.fetch(ehentai_session, url)
         await self._handle_album_additions("e-hentai", album_obj, title)
         await ehentai_session.exit_handler()
 
     async def Erome(self, url, title=None):
         erome_session = ScrapeSession(self.client)
         if not self.erome_crawler:
-            self.erome_crawler = EromeCrawler(include_id=self.include_id, quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.erome_crawler = EromeCrawler(include_id=self.include_id, quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                              error_writer=self.error_writer)
         domain_obj = await self.erome_crawler.fetch(erome_session, url)
         await self._handle_domain_additions("erome", domain_obj, title)
         await erome_session.exit_handler()
 
     async def Gfycat(self, url, title=None):
         gfycat_session = ScrapeSession(self.client)
         if not self.gfycat_crawler:
-            self.gfycat_crawler = GfycatCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.gfycat_crawler = GfycatCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                error_writer=self.error_writer)
         album_obj = await self.gfycat_crawler.fetch(gfycat_session, url)
         await self._handle_album_additions("gfycat", album_obj, title)
         await gfycat_session.exit_handler()
 
     async def GoFile(self, url, title=None):
         gofile_session = ScrapeSession(self.client)
         if not self.gofile_crawler:
-            self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                error_writer=self.error_writer)
 
         async with self.gofile_semaphore:
             await self.gofile_crawler.get_token(session=gofile_session,
                                                 api_token=self.args['Authentication']['gofile_api_key'])
         domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
         await self._handle_domain_additions("gofile", domain_obj, title)
         await gofile_session.exit_handler()
 
     async def HGameCG(self, url, title=None):
         hgamecg_session = ScrapeSession(self.client)
         if not self.hgamecg_crawler:
-            self.hgamecg_crawler = HGameCGCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.hgamecg_crawler = HGameCGCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                  error_writer=self.error_writer)
         album_obj = await self.hgamecg_crawler.fetch(hgamecg_session, url)
         await self._handle_album_additions("hgamecg", album_obj, title)
         await hgamecg_session.exit_handler()
 
     async def ImgBox(self, url, title=None):
         imgbox_session = ScrapeSession(self.client)
         if not self.imgbox_crawler:
-            self.imgbox_crawler = ImgBoxCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.imgbox_crawler = ImgBoxCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                error_writer=self.error_writer)
         album_obj = await self.imgbox_crawler.fetch(imgbox_session, url)
         await self._handle_album_additions("imgbox", album_obj, title)
         await imgbox_session.exit_handler()
 
     async def LoveFap(self, url: URL, title=None):
         lovefap_session = ScrapeSession(self.client)
         if not self.lovefap_crawler:
-            self.lovefap_crawler = LoveFapCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.lovefap_crawler = LoveFapCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                  error_writer=self.error_writer)
         album_obj = await self.lovefap_crawler.fetch(lovefap_session, url)
         await self._handle_album_additions("lovefap", album_obj, title)
         await lovefap_session.exit_handler()
 
     async def PimpAndHost(self, url, title=None):
         pimpandhost_session = ScrapeSession(self.client)
         if not self.pimpandhost_crawler:
-            self.pimpandhost_crawler = PimpAndHostCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.pimpandhost_crawler = PimpAndHostCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                          error_writer=self.error_writer)
         album_obj = await self.pimpandhost_crawler.fetch(pimpandhost_session, url)
         await self._handle_album_additions("pimpandhost", album_obj, title)
         await pimpandhost_session.exit_handler()
 
     async def PixelDrain(self, url, title=None):
         pixeldrain_session = ScrapeSession(self.client)
         if not self.pixeldrain_crawler:
-            self.pixeldrain_crawler = PixelDrainCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.pixeldrain_crawler = PixelDrainCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                        error_writer=self.error_writer)
         album_obj = await self.pixeldrain_crawler.fetch(pixeldrain_session, url)
         await self._handle_album_additions("pixeldrain", album_obj, title)
         await pixeldrain_session.exit_handler()
 
     async def PostImg(self, url, title=None):
         postimg_session = ScrapeSession(self.client)
         if not self.postimg_crawler:
-            self.postimg_crawler = PostImgCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.postimg_crawler = PostImgCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                  error_writer=self.error_writer)
         album_obj = await self.postimg_crawler.fetch(postimg_session, url)
         await self._handle_album_additions("postimg", album_obj, title)
         await postimg_session.exit_handler()
 
     async def Saint(self, url, title=None):
         saint_session = ScrapeSession(self.client)
         if not self.saint_crawler:
-            self.saint_crawler = SaintCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.saint_crawler = SaintCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                              error_writer=self.error_writer)
         album_obj = await self.saint_crawler.fetch(saint_session, url)
         await self._handle_album_additions("saint", album_obj, title)
         await saint_session.exit_handler()
 
     async def ShareX(self, url, title=None):
         sharex_session = ScrapeSession(self.client)
         if not self.sharex_crawler:
-            self.sharex_crawler = ShareXCrawler(include_id=self.include_id, quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.sharex_crawler = ShareXCrawler(include_id=self.include_id, quiet=self.quiet,
+                                                SQL_Helper=self.SQL_Helper, error_writer=self.error_writer)
 
         domain_obj = await self.sharex_crawler.fetch(sharex_session, url)
         await self._handle_domain_additions("sharex", domain_obj, title)
         await sharex_session.exit_handler()
 
     async def XBunkr(self, url, title=None):
         xbunkr_session = ScrapeSession(self.client)
         if not self.xbunkr_crawler:
-            self.xbunkr_crawler = XBunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.xbunkr_crawler = XBunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                error_writer=self.error_writer)
         album_obj = await self.xbunkr_crawler.fetch(xbunkr_session, url)
         await self._handle_album_additions("xbunkr", album_obj, title)
         await xbunkr_session.exit_handler()
 
     """Archive Sites"""
 
     async def Fapello(self, url, title=None):
         fapello_session = ScrapeSession(self.client)
         if not self.fapello_crawler:
-            self.fapello_crawler = FapelloCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.fapello_crawler = FapelloCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
+                                                  error_writer=self.error_writer)
         album_obj = await self.fapello_crawler.fetch(fapello_session, url)
         if album_obj:
             await self._handle_album_additions("fapello", album_obj, title)
         await fapello_session.exit_handler()
 
     async def NSFW_XXX(self, url, title=None):
         nsfwxxx_session = ScrapeSession(self.client)
         if not self.nsfwxxx_crawler:
-            self.nsfwxxx_crawler = NSFWXXXCrawler(separate_posts=self.separate_posts, quiet=self.quiet, SQL_Helper=self.SQL_Helper)
+            self.nsfwxxx_crawler = NSFWXXXCrawler(separate_posts=self.separate_posts, quiet=self.quiet,
+                                                  SQL_Helper=self.SQL_Helper, error_writer=self.error_writer)
         domain_obj = await self.nsfwxxx_crawler.fetch(nsfwxxx_session, url)
         await self._handle_domain_additions("nsfw.xxx", domain_obj, title)
         await nsfwxxx_session.exit_handler()
 
     async def Coomeno(self, url: URL, title=None):
         coomeno_session = ScrapeSession(self.client)
         if not self.coomeno_crawler:
             self.coomeno_crawler = CoomenoCrawler(include_id=self.include_id, scraping_mapper=self,
                                                   separate_posts=self.separate_posts, SQL_Helper=self.SQL_Helper,
-                                                  quiet=self.quiet)
+                                                  quiet=self.quiet, error_writer=self.error_writer)
         assert url.host is not None
         async with self.coomero_semaphore:
             cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
 
         if not new_title or await cascade.is_empty():
             await coomeno_session.exit_handler()
             return
@@ -307,15 +323,15 @@
 
     """Forum handling"""
 
     async def Xenforo(self, url: URL, title=None):
         xenforo_session = ScrapeSession(self.client)
         if not self.xenforo_crawler:
             self.xenforo_crawler = XenforoCrawler(scraping_mapper=self, args=self.args, SQL_Helper=self.SQL_Helper,
-                                                  quiet=self.quiet)
+                                                  quiet=self.quiet, error_writer=self.error_writer)
         title = None
         cascade = None
 
         assert self.xenforo_crawler is not None and url.host is not None
         if "simpcity" in url.host:
             async with self.simpcity_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
@@ -361,12 +377,10 @@
             return
 
         if self.jdownloader.jdownloader_enable:
             await self.jdownloader.direct_unsupported_to_jdownloader(url_to_map, title)
 
         else:
             log(f"Not Supported: {url_to_map}", quiet=self.quiet, style="yellow")
-            if self.unsupported_output:
-                title = title.encode("ascii", "ignore")
-                title = title.decode().strip()
-                async with aiofiles.open(self.unsupported_file, mode='a') as f:
-                    await f.write(f"{url_to_map},{referer},{title}\n")
+            title = title.encode("ascii", "ignore")
+            title = title.decode().strip()
+            await self.error_writer.write_unsupported(f"{url_to_map},{referer},{title}")
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.31
+Version: 4.2.32
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -126,15 +126,16 @@
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
 --config-file                   config file to read arguments from
 --db-file                       history database file to write to
---errored-urls-file             csv file to write failed download information to
+--errored-download-urls-file    csv file to write failed download information to
+--errored-scrape-urls-file      csv file to write failed scrape information to
 --log-file                      log file to write to
 --output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
 --unsupported-urls-file         csv file to output unsupported links into
 
 --exclude-audio         skip downloading of audio files
 --exclude-images        skip downloading of image files
 --exclude-other         skip downloading of images
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.31 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.32 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -113,18 +113,19 @@
 username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 Bulk downloader for multiple file hosts positional arguments: link link to
 content to download (passing multiple links is supported) optional arguments: -
 h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
-database file to write to --errored-urls-file csv file to write failed download
-information to --log-file log file to write to --output-last-forum-post-file
-text file to output last scraped post from a forum thread for re-feeding into
-CDL --unsupported-urls-file csv file to output unsupported links into --
+database file to write to --errored-download-urls-file csv file to write failed
+download information to --errored-scrape-urls-file csv file to write failed
+scrape information to --log-file log file to write to --output-last-forum-post-
+file text file to output last scraped post from a forum thread for re-feeding
+into CDL --unsupported-urls-file csv file to output unsupported links into --
 exclude-audio skip downloading of audio files --exclude-images skip downloading
 of image files --exclude-other skip downloading of images --exclude-videos skip
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
```

### Comparing `cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.32/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.31/setup.cfg` & `cyberdrop-dl-4.2.32/setup.cfg`

 * *Files identical despite different names*

