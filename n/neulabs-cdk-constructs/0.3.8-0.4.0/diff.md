# Comparing `tmp/neulabs-cdk-constructs-0.3.8.tar.gz` & `tmp/neulabs-cdk-constructs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.3.8.tar", last modified: Fri May 19 12:42:52 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.4.0.tar", last modified: Fri May 19 14:10:33 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.3.8.tar` & `neulabs-cdk-constructs-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.136985 neulabs-cdk-constructs-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.136985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100741 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.140985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 12:42:40.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:52.136985 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-19 12:42:52.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-19 12:42:52.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:42:52.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 12:42:52.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 12:42:52.000000 neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100996 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 14:10:20.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:10:33.025831 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-19 14:10:33.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:10:32.000000 neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.3.8/LICENSE` & `neulabs-cdk-constructs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/PKG-INFO` & `neulabs-cdk-constructs-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.3.8
+Version: 0.4.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 
 # Neulabs CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/neulabs-cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-cdk-constructs)
 [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-constructs/)
 [![PyPI](https://img.shields.io/github/last-commit/neulabscom/neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-constructs/commits/main)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/main/LICENSE)
+[![View on Construct Hub](https://constructs.dev/badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-cdk-constructs)
 
 The neulabs-cdk-constructs library contains CDK-based constructs and stacks to allow the creation of cloud infrastructure on AWS.
 
 The purpose of the library is to expose modules that can facilitate the creation and maintenance of the infrastructure as code.
 
 Inside you will find generic stacks that allow the creation of services by simply instantiating a class, or constructs that implement logic to facilitate the developer and many other aspects.
```

### Comparing `neulabs-cdk-constructs-0.3.8/README.md` & `neulabs-cdk-constructs-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Neulabs CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/neulabs-cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-cdk-constructs)
 [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-constructs/)
 [![PyPI](https://img.shields.io/github/last-commit/neulabscom/neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-constructs/commits/main)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/main/LICENSE)
+[![View on Construct Hub](https://constructs.dev/badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-cdk-constructs)
 
 The neulabs-cdk-constructs library contains CDK-based constructs and stacks to allow the creation of cloud infrastructure on AWS.
 
 The purpose of the library is to expose modules that can facilitate the creation and maintenance of the infrastructure as code.
 
 Inside you will find generic stacks that allow the creation of services by simply instantiating a class, or constructs that implement logic to facilitate the developer and many other aspects.
```

#### html2text {}

```diff
@@ -2,19 +2,21 @@
 constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-
 cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
 constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-
 constructs/) [![PyPI](https://img.shields.io/github/last-commit/neulabscom/
 neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-
 constructs/commits/main) [![License](https://img.shields.io/badge/license-
 Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/
-main/LICENSE) The neulabs-cdk-constructs library contains CDK-based constructs
-and stacks to allow the creation of cloud infrastructure on AWS. The purpose of
-the library is to expose modules that can facilitate the creation and
-maintenance of the infrastructure as code. Inside you will find generic stacks
-that allow the creation of services by simply instantiating a class, or
+main/LICENSE) [![View on Construct Hub](https://constructs.dev/
+badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-
+cdk-constructs) The neulabs-cdk-constructs library contains CDK-based
+constructs and stacks to allow the creation of cloud infrastructure on AWS. The
+purpose of the library is to expose modules that can facilitate the creation
+and maintenance of the infrastructure as code. Inside you will find generic
+stacks that allow the creation of services by simply instantiating a class, or
 constructs that implement logic to facilitate the developer and many other
 aspects. We decided to develop it in Typescript, using projen for repository
 management, and the JSII library to be able to compile the neulabs-cdk-
 constructs package into multiple languages. ## Usage **Package Installation
 (npm)**: ``` yarn add neulabs-cdk-constructs # or npm install neulabs-cdk-
 constructs ``` **Package Installation (python)**: ``` pip install neulabs-cdk-
 constructs ``` **Create Github OIDC** The creation of Github OIDC allows a role
```

### Comparing `neulabs-cdk-constructs-0.3.8/setup.py` & `neulabs-cdk-constructs-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.3.8",
+    "version": "0.4.0",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.3.8.jsii.tgz"
+            "neulabs-cdk-constructs@0.4.0.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 # Neulabs CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/neulabs-cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-cdk-constructs)
 [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-constructs/)
 [![PyPI](https://img.shields.io/github/last-commit/neulabscom/neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-constructs/commits/main)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/main/LICENSE)
+[![View on Construct Hub](https://constructs.dev/badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-cdk-constructs)
 
 The neulabs-cdk-constructs library contains CDK-based constructs and stacks to allow the creation of cloud infrastructure on AWS.
 
 The purpose of the library is to expose modules that can facilitate the creation and maintenance of the infrastructure as code.
 
 Inside you will find generic stacks that allow the creation of services by simply instantiating a class, or constructs that implement logic to facilitate the developer and many other aspects.
```

#### html2text {}

```diff
@@ -2,19 +2,21 @@
 constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-
 cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
 constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-
 constructs/) [![PyPI](https://img.shields.io/github/last-commit/neulabscom/
 neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-
 constructs/commits/main) [![License](https://img.shields.io/badge/license-
 Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/
-main/LICENSE) The neulabs-cdk-constructs library contains CDK-based constructs
-and stacks to allow the creation of cloud infrastructure on AWS. The purpose of
-the library is to expose modules that can facilitate the creation and
-maintenance of the infrastructure as code. Inside you will find generic stacks
-that allow the creation of services by simply instantiating a class, or
+main/LICENSE) [![View on Construct Hub](https://constructs.dev/
+badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-
+cdk-constructs) The neulabs-cdk-constructs library contains CDK-based
+constructs and stacks to allow the creation of cloud infrastructure on AWS. The
+purpose of the library is to expose modules that can facilitate the creation
+and maintenance of the infrastructure as code. Inside you will find generic
+stacks that allow the creation of services by simply instantiating a class, or
 constructs that implement logic to facilitate the developer and many other
 aspects. We decided to develop it in Typescript, using projen for repository
 management, and the JSII library to be able to compile the neulabs-cdk-
 constructs package into multiple languages. ## Usage **Package Installation
 (npm)**: ``` yarn add neulabs-cdk-constructs # or npm install neulabs-cdk-
 constructs ``` **Package Installation (python)**: ``` pip install neulabs-cdk-
 constructs ``` **Create Github OIDC** The creation of Github OIDC allows a role
```

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.3.8",
+    "0.4.0",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.3.8.jsii.tgz",
+    "neulabs-cdk-constructs@0.4.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.3.8
+Version: 0.4.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 
 # Neulabs CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/neulabs-cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-cdk-constructs)
 [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-constructs/)
 [![PyPI](https://img.shields.io/github/last-commit/neulabscom/neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-constructs/commits/main)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/main/LICENSE)
+[![View on Construct Hub](https://constructs.dev/badge?package=neulabs-cdk-constructs)](https://constructs.dev/packages/neulabs-cdk-constructs)
 
 The neulabs-cdk-constructs library contains CDK-based constructs and stacks to allow the creation of cloud infrastructure on AWS.
 
 The purpose of the library is to expose modules that can facilitate the creation and maintenance of the infrastructure as code.
 
 Inside you will find generic stacks that allow the creation of services by simply instantiating a class, or constructs that implement logic to facilitate the developer and many other aspects.
```

### Comparing `neulabs-cdk-constructs-0.3.8/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.4.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.8.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.0.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

