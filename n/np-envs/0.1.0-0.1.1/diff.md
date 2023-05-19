# Comparing `tmp/np_envs-0.1.0.tar.gz` & `tmp/np_envs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_envs-0.1.0.tar", last modified: Thu May 18 08:44:15 2023, max compression
+gzip compressed data, was "np_envs-0.1.1.tar", last modified: Fri May 19 01:11:21 2023, max compression
```

## Comparing `np_envs-0.1.0.tar` & `np_envs-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.0/README.md
--rw-r--r--   0        0        0      447 2023-05-18 08:44:15.088773 np_envs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.0/src/np_envs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.0/src/np_envs/__main__.py
--rw-r--r--   0        0        0      466 2023-05-18 08:28:24.713740 np_envs-0.1.0/src/np_envs/config.py
--rw-r--r--   0        0        0     3419 2023-05-18 08:27:13.424169 np_envs-0.1.0/src/np_envs/env.py
--rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.0/src/np_envs/pip.ini
--rw-r--r--   0        0        0       14 2023-05-18 06:56:35.295952 np_envs-0.1.0/src/np_envs/requirements/np_pipeline_qc.requirements.txt
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 np_envs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.1/README.md
+-rw-r--r--   0        0        0      472 2023-05-19 01:11:21.691843 np_envs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.1/src/np_envs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.1/src/np_envs/__main__.py
+-rw-r--r--   0        0        0     1220 2023-05-19 01:01:20.125885 np_envs-0.1.1/src/np_envs/config.py
+-rw-r--r--   0        0        0     6736 2023-05-19 01:09:52.002710 np_envs-0.1.1/src/np_envs/env.py
+-rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.1/src/np_envs/pip.ini
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.1/PKG-INFO
```

