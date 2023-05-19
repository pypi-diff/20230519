# Comparing `tmp/skellyai-0.1.4.tar.gz` & `tmp/skellyai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.1.4.tar", last modified: Tue May 16 23:24:36 2023, max compression
+gzip compressed data, was "dist/skellyai-0.1.5.tar", last modified: Fri May 19 20:54:19 2023, max compression
```

## Comparing `skellyai-0.1.4.tar` & `skellyai-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.008228 skellyai-0.1.4/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-16 23:24:36.007565 skellyai-0.1.4/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-05-16 23:24:36.008400 skellyai-0.1.4/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-05-16 23:24:18.000000 skellyai-0.1.4/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.004243 skellyai-0.1.4/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.4/skellyai/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      705 2023-05-16 17:53:34.000000 skellyai-0.1.4/skellyai/label_gen.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.007032 skellyai-0.1.4/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      210 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 20:54:19.861727 skellyai-0.1.5/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-19 20:54:19.861273 skellyai-0.1.5/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-05-19 20:54:19.861944 skellyai-0.1.5/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-05-19 20:53:29.000000 skellyai-0.1.5/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 20:54:19.857874 skellyai-0.1.5/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.5/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-19 20:54:19.860809 skellyai-0.1.5/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-19 20:54:19.000000 skellyai-0.1.5/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      197 2023-05-19 20:54:19.000000 skellyai-0.1.5/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-05-19 20:54:19.000000 skellyai-0.1.5/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-05-19 20:54:19.000000 skellyai-0.1.5/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-05-19 20:54:19.000000 skellyai-0.1.5/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.1.4/setup.py` & `skellyai-0.1.5/setup.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setupsetup(    name='skellyai',    version='0.1.4',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
+from setuptools import setupsetup(    name='skellyai',    version='0.1.5',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
```

