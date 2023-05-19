# Comparing `tmp/chat-downloader-0.2.5.tar.gz` & `tmp/chat-downloader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-downloader-0.2.5.tar", last modified: Fri May  5 21:15:16 2023, max compression
+gzip compressed data, was "chat-downloader-0.2.6.tar", last modified: Fri May 19 11:06:22 2023, max compression
```

## Comparing `chat-downloader-0.2.5.tar` & `chat-downloader-0.2.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.627220 chat-downloader-0.2.5/chat_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/custom_formats.json
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/output/continuous_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.635220 chat-downloader-0.2.5/chat_downloader/sites/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    57721 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.635220 chat-downloader-0.2.5/chat_downloader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/timed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.639220 chat-downloader-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/items.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/options.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.639220 chat-downloader-0.2.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/chat_downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/sites.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 21:15:16.647220 chat-downloader-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/other youtube actions
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_init_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/youtube_actions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/custom_formats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/formatting/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/output/continuous_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57794 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/sites/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/chat_downloader/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/chat_downloader/utils/timed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.501308 chat-downloader-0.2.6/chat_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:06:22.000000 chat-downloader-0.2.6/chat_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/items.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/options.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/chat_downloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/docs/source/sites.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:06:22.505308 chat-downloader-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/other youtube actions
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_init_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-05-19 11:06:07.000000 chat-downloader-0.2.6/tests/youtube_actions.json
```

### Comparing `chat-downloader-0.2.5/LICENSE` & `chat-downloader-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/PKG-INFO` & `chat-downloader-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.5/README.rst` & `chat-downloader-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/chat_downloader.py` & `chat-downloader-0.2.6/chat_downloader/chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/cli.py` & `chat-downloader-0.2.6/chat_downloader/cli.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/debugging.py` & `chat-downloader-0.2.6/chat_downloader/debugging.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/errors.py` & `chat-downloader-0.2.6/chat_downloader/errors.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/formatting/custom_formats.json` & `chat-downloader-0.2.6/chat_downloader/formatting/custom_formats.json`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/formatting/format.py` & `chat-downloader-0.2.6/chat_downloader/formatting/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
                         pass   # TODO add others
 
                 # Apply separator
                 separator = formatting_info.get('separator')
                 if separator:
                     if index == 'author.badges':
                         value = separator.join(
-                            map(lambda key: key.get('title'), value))
+                            filter(None, map(lambda key: key.get('title'), value))
+                        )
                     elif isinstance(value, (tuple, list)):
                         value = separator.join(
                             map(lambda x: str(x), value))
                     else:
                         pass
             else:
                 pass
```

### Comparing `chat-downloader-0.2.5/chat_downloader/output/continuous_write.py` & `chat-downloader-0.2.6/chat_downloader/output/continuous_write.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/__init__.py` & `chat-downloader-0.2.6/chat_downloader/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/common.py` & `chat-downloader-0.2.6/chat_downloader/sites/common.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/facebook.py` & `chat-downloader-0.2.6/chat_downloader/sites/facebook.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/twitch.py` & `chat-downloader-0.2.6/chat_downloader/sites/twitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,16 +815,19 @@
 
         if 'time_in_seconds' in info:
             info['time_in_seconds'] -= offset
             info['time_text'] = seconds_to_time(int(info['time_in_seconds']))
 
         badges = info.pop('author_badges', None)
         if badges:
-            info['author']['badges'] = list(map(lambda x: TwitchChatDownloader._parse_badge_info(
-                x.get('setID'), x.get('version'), channel_id), badges))
+            info['author']['badges'] = [
+                TwitchChatDownloader._parse_badge_info(x.get('setID'), x.get('version'), channel_id)
+                for x in badges
+                if x.get('setID') and x.get('version')
+            ]
 
         BaseChatDownloader._move_to_dict(info, 'author')
 
         original_message_type = info.get('message_type')
         if original_message_type:
             TwitchChatDownloader._set_message_type(
                 info, original_message_type)
```

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/youtube.py` & `chat-downloader-0.2.6/chat_downloader/sites/youtube.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/sites/zoom.py` & `chat-downloader-0.2.6/chat_downloader/sites/zoom.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/utils/core.py` & `chat-downloader-0.2.6/chat_downloader/utils/core.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader/utils/timed_utils.py` & `chat-downloader-0.2.6/chat_downloader/utils/timed_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/chat_downloader.egg-info/PKG-INFO` & `chat-downloader-0.2.6/chat_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.5/chat_downloader.egg-info/SOURCES.txt` & `chat-downloader-0.2.6/chat_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/Makefile` & `chat-downloader-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/README.rst` & `chat-downloader-0.2.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/changelog.rst` & `chat-downloader-0.2.6/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/cli.rst` & `chat-downloader-0.2.6/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/conf.py` & `chat-downloader-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/contributing.rst` & `chat-downloader-0.2.6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/items.rst` & `chat-downloader-0.2.6/docs/items.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/options.rst` & `chat-downloader-0.2.6/docs/options.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/source/chat_downloader.rst` & `chat-downloader-0.2.6/docs/source/chat_downloader.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/docs/source/sites.rst` & `chat-downloader-0.2.6/docs/source/sites.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/setup.py` & `chat-downloader-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/other youtube actions` & `chat-downloader-0.2.6/tests/other youtube actions`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_chat_downloader.py` & `chat-downloader-0.2.6/tests/test_chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_formatting.py` & `chat-downloader-0.2.6/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_generators.py` & `chat-downloader-0.2.6/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_init_params.py` & `chat-downloader-0.2.6/tests/test_init_params.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_sites.py` & `chat-downloader-0.2.6/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_utils.py` & `chat-downloader-0.2.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/test_writers.py` & `chat-downloader-0.2.6/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.5/tests/youtube_actions.json` & `chat-downloader-0.2.6/tests/youtube_actions.json`

 * *Files identical despite different names*

