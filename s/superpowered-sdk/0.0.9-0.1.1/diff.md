# Comparing `tmp/superpowered-sdk-0.0.9.tar.gz` & `tmp/superpowered-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.0.9.tar", last modified: Thu Feb  2 08:52:20 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.1.tar", last modified: Fri May 19 07:14:53 2023, max compression
```

## Comparing `superpowered-sdk-0.0.9.tar` & `superpowered-sdk-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/superpowered/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.175529 superpowered-sdk-0.1.1/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6509 2023-05-19 07:14:53.174927 superpowered-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)     5009 2023-05-19 06:21:14.000000 superpowered-sdk-0.1.1/README.md
+-rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-19 07:14:53.175851 superpowered-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 justinclark   (501) staff       (20)     2040 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/setup.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.169304 superpowered-sdk-0.1.1/superpowered/
+-rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/__init__.py
+-rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/exceptions.py
+-rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.1/superpowered/superpowered.py
+drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-19 07:14:53.174078 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/
+-rw-r--r--   0 justinclark   (501) staff       (20)     6509 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 justinclark   (501) staff       (20)      298 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-19 07:14:53.000000 superpowered-sdk-0.1.1/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.0.9/setup.py` & `superpowered-sdk-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,42 @@
-#!/usr/bin/env python
-#
-# Copyright (c) 2023 Superpowered AI All right reserved.
-#
-
 import os
-
 import setuptools
 
 long_desc = """# Superpowered AI
-Create Collaborative AI Agents with memory, tools, and knowledge bases.
+Knowledge base as a service for LLM applications
 """
 
+
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setuptools.setup(
     name="superpowered-sdk",
-    version="0.0.9",
+    version=read("VERSION"),
     description="Superpowered AI SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://superpowered.ai",
     project_urls={
         "Homepage": "https://superpowered.ai",
         "Documentation": "https://superpowered.ai/docs",
         "Contact": "https://superpowered.ai/contact/",
         "End-User License Agreement": "https://superpowered.ai/api-user-agreement/"
     },
     author="superpowered",
     author_email="justin@superpowered.ai",
-    keywords="Superpowered AI LLM Chat Agents",
-    packages=setuptools.find_packages(),
-    # install_requires=read("requirements.txt"),
+    keywords="Superpowered AI Knowledge base as a service for LLM applications",
+    packages=["superpowered"],
+    # package_dir={"": "superpowered"},
+    install_requires=read("requirements.txt"),
     include_package_data=True,
     python_requires=">=3.6",
-    # entry_points={
-    #     'console_scripts': ['pinecone=pinecone.cli:main'],
-    # },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
@@ -55,9 +48,9 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Database",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules"
-    ]
+    ],
 )
```

