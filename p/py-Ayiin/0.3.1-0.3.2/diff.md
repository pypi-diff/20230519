# Comparing `tmp/py-Ayiin-0.3.1.tar.gz` & `tmp/py-Ayiin-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.1.tar", last modified: Thu May 18 14:15:10 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.2.tar", last modified: Fri May 19 07:04:15 2023, max compression
```

## Comparing `py-Ayiin-0.3.1.tar` & `py-Ayiin-0.3.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.571883 py-Ayiin-0.3.1/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.571883 py-Ayiin-0.3.1/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.571883 py-Ayiin-0.3.1/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 14:15:10.000000 py-Ayiin-0.3.1/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-18 14:15:10.000000 py-Ayiin-0.3.1/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:15:10.000000 py-Ayiin-0.3.1/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 14:15:10.000000 py-Ayiin-0.3.1/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 14:15:10.000000 py-Ayiin-0.3.1/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:15:10.575883 py-Ayiin-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 14:14:57.000000 py-Ayiin-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.887915 py-Ayiin-0.3.2/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 07:04:15.000000 py-Ayiin-0.3.2/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 07:04:15.891915 py-Ayiin-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-19 07:04:03.000000 py-Ayiin-0.3.2/setup.py
```

### Comparing `py-Ayiin-0.3.1/LICENSE` & `py-Ayiin-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/NOTICE` & `py-Ayiin-0.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/PKG-INFO` & `py-Ayiin-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.1/README.md` & `py-Ayiin-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.2/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.2/pyAyiin/Clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from fipper import Client
 
 from telethon import TelegramClient
 from telethon.sessions import MemorySession
 
 from . import *
 
-from config import Var
-
-
-
 from ..config import Var as Variable
 
 Var = Variable()
 
 
 hndlr = f"{Var.HNDLR[0]} {Var.HNDLR[1]} {Var.HNDLR[2]} {Var.HNDLR[3]} {Var.HNDLR[4]} {Var.HNDLR[5]}"
```

### Comparing `py-Ayiin-0.3.1/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.3.2/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.2/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/__init__.py` & `py-Ayiin-0.3.2/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.1"
-ayiin_ver = "0.1.0"
+__version__ = "0.3.2"
+ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
```

### Comparing `py-Ayiin-0.3.1/pyAyiin/__main__.py` & `py-Ayiin-0.3.2/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/assistant.py` & `py-Ayiin-0.3.2/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/config.py` & `py-Ayiin-0.3.2/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.2/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.2/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.2/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.2/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.2/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.2/pyAyiin/dB/blacklistgcast.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,18 @@
     return True
 
 
 async def add_blacklist_gcast(chat_id: int):
     is_served = await is_blacklist_gcast(chat_id)
     if is_served:
         return
-    return await chatsdb.insert_one({"chat_id": chat_id})
+    await chatsdb.insert_one({"chat_id": chat_id})
+    await blacklisted()
+    return
 
 
 async def remove_blacklist_gcast(chat_id: int):
     is_served = await is_blacklist_gcast(chat_id)
     if not is_served:
         return
+    BLACKLIST_GCAST.remove(chat_id)
     return await chatsdb.delete_one({"chat_id": chat_id})
```

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.2/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.2/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.2/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.2/pyAyiin/dB/logdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from ._core import mongodb
 
 collection = mongodb.logdb
 
 # pmlogs
 
 
-async def is_pmlogs(on_off: int) -> bool:
+async def is_pm_logs(on_off: int) -> bool:
     onoff = await collection.find_one({"on_off": on_off})
     if not onoff:
         return False
     return True
 
 
-async def add_on(on_off: int):
-    is_on = await is_pmlogs(on_off)
+async def add_pm_on(on_off: int):
+    is_on = await is_pm_logs(on_off)
     if is_on:
         return
     return await collection.insert_one({"on_off": on_off})
 
 
-async def add_off(on_off: int):
-    is_off = await is_pmlogs(on_off)
+async def add_pm_off(on_off: int):
+    is_off = await is_pm_logs(on_off)
     if not is_off:
         return
     return await collection.delete_one({"on_off": on_off})
 
 
-async def is_gruplogs(on_off: int) -> bool:
+async def is_grup_logs(on_off: int) -> bool:
     onoff = await collection.find_one({"on_off": on_off})
     if not onoff:
         return False
     return True
 
 
-async def addg_on(on_off: int):
-    is_on = await is_gruplogs(on_off)
+async def add_grup_on(on_off: int):
+    is_on = await is_grup_logs(on_off)
     if is_on:
         return
     return await collection.insert_one({"on_off": on_off})
 
 
-async def addg_off(on_off: int):
-    is_off = await is_gruplogs(on_off)
+async def add_grup_off(on_off: int):
+    is_off = await is_grup_logs(on_off)
     if not is_off:
         return
     return await collection.delete_one({"on_off": on_off})
```

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.2/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.2/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/start.py` & `py-Ayiin-0.3.2/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.2/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.2/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.2/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.2/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/decorator.py` & `py-Ayiin-0.3.2/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/exceptions.py` & `py-Ayiin-0.3.2/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.2/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.2/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.2/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.2/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/func.py` & `py-Ayiin-0.3.2/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.2/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.2/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.2/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.2/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.2/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.2/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.2/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/pyAyiin/xd.py` & `py-Ayiin-0.3.2/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.2/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.1/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.2/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.1/setup.py` & `py-Ayiin-0.3.2/setup.py`

 * *Files identical despite different names*

