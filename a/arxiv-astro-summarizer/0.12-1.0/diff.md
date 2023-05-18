# Comparing `tmp/arxiv-astro-summarizer-0.12.tar.gz` & `tmp/arxiv-astro-summarizer-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-astro-summarizer-0.12.tar", last modified: Thu May 18 22:07:01 2023, max compression
+gzip compressed data, was "arxiv-astro-summarizer-1.0.tar", last modified: Thu May 18 23:01:54 2023, max compression
```

## Comparing `arxiv-astro-summarizer-0.12.tar` & `arxiv-astro-summarizer-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 22:07:00.998601 arxiv-astro-summarizer-0.12/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)      664 2023-05-18 22:07:00.998325 arxiv-astro-summarizer-0.12/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 22:07:00.995323 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer/
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    19473 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer/astroph_summarizer.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 22:07:00.997871 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      664 2023-05-18 22:07:00.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-18 22:07:00.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-18 22:07:00.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      104 2023-05-18 22:07:00.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-18 22:07:00.000000 arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      304 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-0.12/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-18 22:07:00.998685 arxiv-astro-summarizer-0.12/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1079 2023-05-18 22:04:37.000000 arxiv-astro-summarizer-0.12/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.789044 arxiv-astro-summarizer-1.0/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 23:01:54.788773 arxiv-astro-summarizer-1.0/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.786685 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19473 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/astroph_summarizer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.788283 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      110 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      320 2023-05-18 22:35:31.000000 arxiv-astro-summarizer-1.0/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-18 23:01:54.789130 arxiv-astro-summarizer-1.0/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1087 2023-05-18 22:59:09.000000 arxiv-astro-summarizer-1.0/setup.py
```

### Comparing `arxiv-astro-summarizer-0.12/LICENSE.txt` & `arxiv-astro-summarizer-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-0.12/PKG-INFO` & `arxiv-astro-summarizer-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 0.12
+Version: 1.0
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-0.12/README.md` & `arxiv-astro-summarizer-1.0/README.md`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-0.12/arxiv_astro_summarizer/astroph_summarizer.py` & `arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/astroph_summarizer.py`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-0.12/arxiv_astro_summarizer.egg-info/PKG-INFO` & `arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 0.12
+Version: 1.0
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-0.12/setup.py` & `arxiv-astro-summarizer-1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="arxiv-astro-summarizer",
-    version="0.12",
+    version="1.0",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/arxiv-astro-summarizer",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Intended Audience :: Developers',
 		'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 		'Programming Language :: Python :: 3',	   
 ],
     packages=find_packages('.'),
-    install_requires = ['numpy', 'requests', 'arxivscraper', 'pandas', 'PyPDF2', 'transformers', 'scikit-learn', 'nltk', 'textract', 'datefinder', 'tensorflow'],
+    install_requires = ['numpy', 'requests', 'arxivscraper', 'pandas', 'PyPDF2', 'transformers', 'scikit-learn', 'nltk', 'textract', 'datefinder', 'tensorflow', 'torch'],
     python_requires='>=3.7,<4',
     include_package_data=True,
     test_suite="nose.collector",
 )
```

