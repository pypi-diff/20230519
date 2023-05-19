# Comparing `tmp/jellyfishlights-py-0.6.0.tar.gz` & `tmp/jellyfishlights-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyfishlights-py-0.6.0.tar", last modified: Thu Feb 16 03:27:08 2023, max compression
+gzip compressed data, was "jellyfishlights-py-0.7.0.tar", last modified: Fri May 19 03:35:47 2023, max compression
```

## Comparing `jellyfishlights-py-0.6.0.tar` & `jellyfishlights-py-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-02-16 03:27:08.206483 jellyfishlights-py-0.6.0/
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      196 2023-02-16 03:27:08.205482 jellyfishlights-py-0.6.0/PKG-INFO
-drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-02-16 03:27:08.178904 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      196 2023-02-16 03:27:08.000000 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/PKG-INFO
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      379 2023-02-16 03:27:08.000000 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        1 2023-02-16 03:27:08.000000 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       17 2023-02-16 03:27:08.000000 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/requires.txt
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       18 2023-02-16 03:27:08.000000 jellyfishlights-py-0.6.0/jellyfishlights_py.egg-info/top_level.txt
-drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-02-16 03:27:08.200489 jellyfishlights-py-0.6.0/jellyfishlightspy/
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       45 2022-12-21 05:47:47.000000 jellyfishlights-py-0.6.0/jellyfishlightspy/__init__.py
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     1306 2022-12-21 05:47:47.000000 jellyfishlights-py-0.6.0/jellyfishlightspy/getData.py
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     9155 2023-02-16 03:24:09.000000 jellyfishlights-py-0.6.0/jellyfishlightspy/jellyfishmain.py
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     2822 2022-12-27 03:28:58.000000 jellyfishlights-py-0.6.0/jellyfishlightspy/runPattern.py
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     5643 2022-12-21 07:21:32.000000 jellyfishlights-py-0.6.0/jellyfishlightspy/runPatternData.py
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       38 2023-02-16 03:27:08.206483 jellyfishlights-py-0.6.0/setup.cfg
--rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      461 2023-02-16 03:25:30.000000 jellyfishlights-py-0.6.0/setup.py
+drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-05-19 03:35:47.775517 jellyfishlights-py-0.7.0/
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      269 2023-05-19 03:35:47.774516 jellyfishlights-py-0.7.0/PKG-INFO
+drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-05-19 03:35:47.722786 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      269 2023-05-19 03:35:47.000000 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      480 2023-05-19 03:35:47.000000 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        1 2023-05-19 03:35:47.000000 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       17 2023-05-19 03:35:47.000000 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/requires.txt
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       18 2023-05-19 03:35:47.000000 jellyfishlights-py-0.7.0/jellyfishlights_py.egg-info/top_level.txt
+drwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)        0 2023-05-19 03:35:47.767030 jellyfishlights-py-0.7.0/jellyfishlightspy/
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      282 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/__init__.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     5564 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/cache.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      932 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/const.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)    28063 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/controller.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     4813 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/helpers.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     3908 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/model.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     5591 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/monitor.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)     3323 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/requests.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)    10916 2023-05-19 03:25:51.000000 jellyfishlights-py-0.7.0/jellyfishlightspy/validators.py
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)       38 2023-05-19 03:35:47.776517 jellyfishlights-py-0.7.0/setup.cfg
+-rwxrwxrwx   0 vinenoob  (1000) vinenoob  (1000)      461 2023-05-19 03:34:37.000000 jellyfishlights-py-0.7.0/setup.py
```

