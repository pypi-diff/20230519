# Comparing `tmp/cekit-4.6.0.tar.gz` & `tmp/cekit-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cekit-4.6.0.tar", last modified: Fri Mar 17 12:03:44 2023, max compression
+gzip compressed data, was "cekit-4.7.0.tar", last modified: Fri May 19 09:36:55 2023, max compression
```

## Comparing `cekit-4.6.0.tar` & `cekit-4.7.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.468794 cekit-4.6.0/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-03-17 12:03:43.000000 cekit-4.6.0/LICENSE
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-03-17 12:03:43.000000 cekit-4.6.0/MANIFEST.in
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-03-17 12:03:44.468794 cekit-4.6.0/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-03-17 12:03:43.000000 cekit-4.6.0/README.rst
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.466795 cekit-4.6.0/cekit/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builder.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.467795 cekit-4.6.0/cekit/builders/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builders/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builders/buildah.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     9671 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builders/docker_builder.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    19471 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builders/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/builders/podman.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.467795 cekit-4.6.0/cekit/cache/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/cache/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/cache/artifact.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/cache/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/cekit_types.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    14914 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/cli.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2408 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/config.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/crypto.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.467795 cekit-4.6.0/cekit/descriptor/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     6611 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1336 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/env.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1288 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/execute.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/image.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/label.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/module.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/modules.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/overrides.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     7474 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/packages.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/port.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    24929 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/resource.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/run.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/descriptor/volume.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/errors.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.467795 cekit-4.6.0/cekit/generator/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    27031 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/base.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/behave.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/docker.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/legacy_version.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    13990 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/generator/osbs.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/log.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/template_helper.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.467795 cekit-4.6.0/cekit/templates/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/templates/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/templates/help.jinja
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/templates/template.jinja
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.468794 cekit-4.6.0/cekit/test/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/test/__init__.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/test/behave_runner.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/test/behave_tester.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/test/collector.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)    22048 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/tools.py
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-03-17 12:03:43.000000 cekit-4.6.0/cekit/version.py
-drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-03-17 12:03:44.466795 cekit-4.6.0/cekit.egg-info/
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/PKG-INFO
--rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/entry_points.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/requires.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-03-17 12:03:44.000000 cekit-4.6.0/cekit.egg-info/top_level.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-03-17 12:03:43.000000 cekit-4.6.0/requirements.txt
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      339 2023-03-17 12:03:44.468794 cekit-4.6.0/setup.cfg
--rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-03-17 12:03:43.000000 cekit-4.6.0/setup.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.515787 cekit-4.7.0/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1074 2023-05-19 09:36:54.000000 cekit-4.7.0/LICENSE
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-05-19 09:36:54.000000 cekit-4.7.0/MANIFEST.in
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-05-19 09:36:55.515787 cekit-4.7.0/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      465 2023-05-19 09:36:54.000000 cekit-4.7.0/README.rst
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.513787 cekit-4.7.0/cekit/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3832 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builder.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/builders/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1560 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/buildah.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     9671 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/docker_builder.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    21904 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1711 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/builders/podman.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/cache/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       91 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3601 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/artifact.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5730 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cache/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      354 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cekit_types.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    15244 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/cli.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2408 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/config.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1346 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/crypto.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/descriptor/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      682 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6611 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1367 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/env.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1174 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/execute.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    19410 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/image.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1005 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/label.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1098 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/module.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1588 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/modules.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     4396 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      913 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/overrides.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     6338 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/packages.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1666 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/port.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    24929 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/resource.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1090 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/run.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      677 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/descriptor/volume.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      177 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/errors.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/generator/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    27118 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/base.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      469 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/behave.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      989 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/docker.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3852 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/legacy_version.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    13990 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/generator/osbs.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1639 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/log.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     5123 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/template_helper.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.514787 cekit-4.7.0/cekit/templates/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3420 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/help.jinja
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    10582 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/templates/template.jinja
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.515787 cekit-4.7.0/cekit/test/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/__init__.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2564 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/behave_runner.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     2591 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/behave_tester.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     3200 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/test/collector.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)    22126 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/tools.py
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       41 2023-05-19 09:36:54.000000 cekit-4.7.0/cekit/version.py
+drwxrwxr-x   0 rnc       (1000) rnc       (1000)        0 2023-05-19 09:36:55.513787 cekit-4.7.0/cekit.egg-info/
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      745 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)     1383 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        1 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       74 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/entry_points.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)       99 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/requires.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)        6 2023-05-19 09:36:55.000000 cekit-4.7.0/cekit.egg-info/top_level.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      638 2023-05-19 09:36:54.000000 cekit-4.7.0/requirements.txt
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      339 2023-05-19 09:36:55.515787 cekit-4.7.0/setup.cfg
+-rw-rw-r--   0 rnc       (1000) rnc       (1000)      899 2023-05-19 09:36:54.000000 cekit-4.7.0/setup.py
```

### Comparing `cekit-4.6.0/LICENSE` & `cekit-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/PKG-INFO` & `cekit-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.6.0
+Version: 4.7.0
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.6.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.7.0.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.6.0/cekit/builder.py` & `cekit-4.7.0/cekit/builder.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/builders/buildah.py` & `cekit-4.7.0/cekit/builders/buildah.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/builders/docker_builder.py` & `cekit-4.7.0/cekit/builders/docker_builder.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/builders/osbs.py` & `cekit-4.7.0/cekit/builders/osbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """Class representing OSBS builder."""
 
     def __init__(self, params):
         super(OSBSBuilder, self).__init__("osbs", params)
 
         self._rhpkg_set_url_repos: List[str] = []
         self.artifacts: List[str] = []
-        self.dist_git: DistGit
+        self.git: Git
         self.dist_git_dir: pathlib.Path
 
         if CONFIG.get("common", "redhat"):
             if self.params.get("stage"):
                 self._fedpkg = "rhpkg-stage"
                 self._koji = "brew-stage"
                 self._koji_url = "https://brewweb.stage.engineering.redhat.com/brew"
@@ -150,41 +150,41 @@
             os.path.expanduser(CONFIG.get("common", "work_dir")), osbs_dir, repository
         )
         if not os.path.exists(os.path.dirname(self.dist_git_dir)):
             os.makedirs(os.path.dirname(self.dist_git_dir))
 
         LOGGER.debug("Using dist-git directory of {}".format(self.dist_git_dir))
 
-        self.dist_git = DistGit(
+        self.git = Git(
             self.dist_git_dir,
             self.target,
             repository,
             branch,
             # TODO: default result, dict, doesn't have attribute `extra_dir`
             self.generator.image.get("osbs", {}).extra_dir,
             self.params.assume_yes,
         )
 
-        self.dist_git.prepare(self.params.stage, self.params.user)
-        self.dist_git.clean(self.artifacts)
+        self.git.prepare(self.params.stage, self.params.user)
+        self.git.clean(self.artifacts)
 
     def _copy_to_dist_git(self):
         LOGGER.debug(
             "Copying files to dist-git '{}' directory".format(self.dist_git_dir)
         )
         copy_recursively(os.path.join(self.target, "image"), self.dist_git_dir)
 
     def _sync_with_dist_git(self):
         with Chdir(self.dist_git_dir):
-            self.dist_git.add(self.artifacts)
+            self.git.add(self.artifacts)
             self.update_lookaside_cache()
 
-            if self.dist_git.stage_modified():
-                self.dist_git.commit(self.params.commit_message)
-                self.dist_git.push()
+            if self.git.stage_modified():
+                self.git.commit(self.params.commit_message)
+                self.git.push()
             else:
                 LOGGER.info("No changes made to the code, committing skipped")
 
     def _wait_for_osbs_task(
         self, task_id: str, current_time: int = 0, timeout: int = 7200
     ):
         """Default timeout is 2hrs"""
@@ -242,15 +242,14 @@
             )
         )
 
     def update_lookaside_cache(self):
         LOGGER.info("Updating lookaside cache...")
 
         cache_artifacts = []
-
         for artifact in self.artifacts:
             # In case the artifact is a directory, we don't want to add it.
             # Instead, it will be staged.
             if os.path.isdir(artifact):
                 continue
 
             cache_artifacts.append(artifact)
@@ -271,15 +270,17 @@
     def run(self):
         if self.params.sync_only:
             LOGGER.info(
                 "The --sync-only parameter was specified, build will not be executed, exiting"
             )
             return
 
-        cmd = [self._koji]
+        build_id: str = ""
+        git_tag: str = ""
+        cmd: List[str] = [self._koji]
 
         if self.params.user:
             cmd += ["--user", self.params.user]
 
         cmd += ["call", "--python", "buildContainer", "--kwargs"]
 
         with Chdir(self.dist_git_dir):
@@ -297,23 +298,23 @@
             src = "git://{}{}#{}".format(url.hostname, url.path, commit)
 
             target = self.generator.image.get("osbs", {}).get("koji_target")
 
             # If target was not specified in the image descriptor
             if not target:
                 # Default to computed target based on branch
-                target = "{}-containers-candidate".format(self.dist_git.branch)
+                target = "{}-containers-candidate".format(self.git.branch)
 
             scratch = True
 
             if self.params.release:
                 scratch = False
 
             kwargs = "{{'src': '{}', 'target': '{}', 'opts': {{'scratch': {}, 'git_branch': '{}', 'yum_repourls': {}}}}}".format(
-                src, target, scratch, self.dist_git.branch, self._rhpkg_set_url_repos
+                src, target, scratch, self.git.branch, self._rhpkg_set_url_repos
             )
 
             cmd.append(kwargs)
 
             LOGGER.info("About to execute '{}'.".format(" ".join(cmd)))
 
             if self.params.assume_yes or tools.decision(
@@ -336,23 +337,71 @@
                     return
 
                 self._wait_for_osbs_task(task_id)
 
                 LOGGER.info("Image was built successfully in OSBS!")
 
                 if self.params.tag:
-                    tag = Template(self.params.tag).render(self.generator.image)
-                    if "/" in tag:
-                        LOGGER.debug(f"Replacing / in tag with - for {tag}")
-                        tag = tag.replace("/", "-")
-                    self.dist_git.tag(tag)
-                    self.dist_git.push(True)
+                    git_tag, build_id = self._establish_tag_name(task_id)
+                    if git_tag:
+                        self.git.tag(src, git_tag, build_id)
+                        self.git.push(git_tag)
+        if self.params.tag:
+            # This is a bit of code reuse cheat - if tagging is enabled this will also tag
+            # the image source repository (while the above block handles the dist-git source)
+            url = run_wrapper(
+                ["git", "config", "--get", "remote.origin.url"],
+                capture_output=True,
+                check=False,
+            ).stdout
+            if git_tag:
+                self.git.tag(url, git_tag, build_id)
+                self.git.push(git_tag)
+
+    def _establish_tag_name(self, task_id: str) -> Tuple[str, str]:
+        """This calls Brew to establish the NVR from the completed build in order to use that to tag the repositories
 
+        :param task_id: A task_id to use to look up the NVR
+        :returns a Tuple containing a tag and build_id. Maybe blank if the task was a scratch build.
+        """
+        tag: str = ""
+        build_id: str = ""
 
-class DistGit(object):
+        task_result = run_wrapper(
+            # Don't need to handle raise_fault as OSBS build must have completed successfully to get to here.
+            [self._koji, "call", "--json-output", "getTaskResult", task_id],
+            True,
+            f"Could not check the task {task_id} result",
+        )
+
+        koji_builds = json.loads(task_result.stdout)["koji_builds"]
+        if koji_builds:
+            build_id = koji_builds[0]
+            build_result = run_wrapper(
+                [self._koji, "call", "--json-output", "getBuild", build_id],
+                True,
+                f"Could not check the build {build_id} result",
+            )
+            nvr: str = json.loads(build_result.stdout)["nvr"]
+            release: str = nvr.rpartition("-")[2]
+            # The default rendered tag (name-version) with release equates to a NVR.
+            tag: str = Template(self.params.tag).render(self.generator.image)
+            if "/" in tag:
+                LOGGER.debug(f"Replacing / in tag with - for {tag}")
+                tag = tag.replace("/", "-")
+            tag = tag + "-" + release
+            LOGGER.info(f"Retrieved NVR {nvr} and generated {tag}")
+        else:
+            LOGGER.warning(
+                f"No koji build found - maybe {task_id} was a scratch build?"
+            )
+        return tag, build_id
+
+
+class Git(object):
     """Git support for osbs repositories"""
 
     @staticmethod
     def repo_info(path) -> Tuple[str, str, str]:
         with Chdir(path):
             if (
                 run_wrapper(["git", "rev-parse", "--is-inside-work-tree"], True).stdout
@@ -389,15 +438,15 @@
         self.osbs_extra: PathType = osbs_extra
         self.noninteractive: bool = noninteractive
 
         (
             self.source_repo_name,
             self.source_repo_branch,
             self.source_repo_commit,
-        ) = DistGit.repo_info(source)
+        ) = Git.repo_info(source)
 
     def stage_modified(self) -> bool:
         # Check if there are any files in stage (return code 1). If there are no files
         # (return code 0) it means that this is a rebuild, so skip committing
         if run_wrapper(
             ["git", "diff-index", "--quiet", "--cached", "HEAD"], False, check=False
         ).returncode:
@@ -535,24 +584,35 @@
                 env={
                     "PS1": "cekit $ ",
                     "TERM": os.getenv("TERM", "xterm"),
                     "HOME": os.getenv("HOME", ""),
                 },
             )
 
-    def tag(self, tag: str) -> None:
-        LOGGER.info(f"Tagging dist-git repository with {tag}")
-        run_wrapper(["git", "tag", tag], False)
+    def tag(self, url: str, tag: str, build_id) -> None:
+        LOGGER.info(f"Tagging git repository ({url}) with {tag} from build {build_id}")
+        # cgit requires annotated tags.
+        run_wrapper(
+            [
+                "git",
+                "tag",
+                "-a",
+                "-m",
+                f"CEKit automated tag from build {build_id}",
+                tag,
+            ],
+            False,
+        )
 
-    def push(self, tag: bool = False) -> None:
+    def push(self, tag: str = None) -> None:
         if self.noninteractive or tools.decision("Do you want to push the commit?"):
             print("")
             LOGGER.info("Pushing change to the upstream repository...")
             if tag:
-                cmd = ["git", "push", "--tags"]
+                cmd = ["git", "push", "origin", tag]
             else:
                 cmd = ["git", "push", "-q", "origin", self.branch]
             run_wrapper(cmd, False)
             LOGGER.info("Change pushed.")
         else:
             LOGGER.info("Changes are not pushed, exiting")
             sys.exit(0)
```

### Comparing `cekit-4.6.0/cekit/builders/podman.py` & `cekit-4.7.0/cekit/builders/podman.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/cache/artifact.py` & `cekit-4.7.0/cekit/cache/artifact.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/cache/cli.py` & `cekit-4.7.0/cekit/cache/cli.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/cli.py` & `cekit-4.7.0/cekit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 if TYPE_CHECKING:
     from cekit.builder import Command
 
 LOGGER = logging.getLogger("cekit")
 CONFIG = Config()
 
 
+def verify_release_passed(ctx, param, value):
+    if not ctx.params.get("release") and value:
+        raise click.UsageError(
+            "--tag requires --release as scratch builds cannot be tagged"
+        )
+    return value
+
+
 @click.group(context_settings=dict(max_content_width=100))
 @click.option(
     "--descriptor",
     metavar="PATH",
     help="Path to image descriptor file.",
     default="image.yaml",
     show_default=True,
@@ -229,15 +237,15 @@
 
         https://podman.io/
     """
     run_build(ctx, "podman")
 
 
 @build.command(name="osbs", short_help="Build using OSBS engine")
-@click.option("--release", help="Execute a release build.", is_flag=True)
+@click.option("--release", help="Execute a release build.", is_flag=True, is_eager=True)
 @click.option("--user", metavar="USER", help="User used to kick the build as.")
 @click.option("--nowait", help="Do not wait for the task to finish.", is_flag=True)
 @click.option("--stage", help="Use stage environment.", is_flag=True)
 @click.option(
     "--sync-only",
     help="Generate files and sync with dist-git, but do not execute build.",
     is_flag=True,
@@ -245,16 +253,17 @@
 @click.option(
     "--commit-message", metavar="MESSAGE", help="Custom dist-git commit message."
 )
 @click.option(
     "--tag",
     is_flag=False,
     flag_value="{{name}}-{{version}}",
-    metavar="TAG",
-    help="Use specified tag to tag the dist-git repository after build",
+    metavar="<TAG>",
+    help="Tag the source and dist-git repositories after build. Default format if not supplied is {{name}}-{{version}}",
+    callback=verify_release_passed,
 )
 @click.option(
     "--assume-yes", "-y", help="Execute build in non-interactive mode.", is_flag=True
 )
 @click.pass_context
 def build_osbs(
     ctx, release, user, nowait, stage, sync_only, commit_message, assume_yes, tag
```

### Comparing `cekit-4.6.0/cekit/config.py` & `cekit-4.7.0/cekit/config.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/crypto.py` & `cekit-4.7.0/cekit/crypto.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/__init__.py` & `cekit-4.7.0/cekit/descriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/base.py` & `cekit-4.7.0/cekit/descriptor/base.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/env.py` & `cekit-4.7.0/cekit/descriptor/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import yaml
 
 from cekit.descriptor import Descriptor
 
 env_schema = yaml.safe_load(
     """
-map:
+type: map
+allowempty: True
+mapping:
   name: {type: str, required: True}
   value: {type: any}
   example: {type: any}
   description: {type: str}"""
 )
```

### Comparing `cekit-4.6.0/cekit/descriptor/execute.py` & `cekit-4.7.0/cekit/descriptor/execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,14 @@
     """
         map:
           name: {type: str}
           script: {type: str}
           user: {type: text}"""
 )
 
-# TODO: This seems unused?
-container_schemas = yaml.safe_load(
-    """
-        seq:
-          - {type: any}"""
-)
-
 logger = logging.getLogger("cekit")
 
 
 class Execute(Descriptor):
     def __init__(self, descriptor, module_name):
         self.schema = execute_schemas
         super(Execute, self).__init__(descriptor)
```

### Comparing `cekit-4.6.0/cekit/descriptor/image.py` & `cekit-4.7.0/cekit/descriptor/image.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/label.py` & `cekit-4.7.0/cekit/descriptor/label.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/module.py` & `cekit-4.7.0/cekit/descriptor/module.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/modules.py` & `cekit-4.7.0/cekit/descriptor/modules.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/osbs.py` & `cekit-4.7.0/cekit/descriptor/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/overrides.py` & `cekit-4.7.0/cekit/descriptor/overrides.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/port.py` & `cekit-4.7.0/cekit/descriptor/port.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/resource.py` & `cekit-4.7.0/cekit/descriptor/resource.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/run.py` & `cekit-4.7.0/cekit/descriptor/run.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/descriptor/volume.py` & `cekit-4.7.0/cekit/descriptor/volume.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/generator/base.py` & `cekit-4.7.0/cekit/generator/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,14 +472,20 @@
         else:
             self.image["packages"]["set_url"] = injected_repos
 
     def _prepare_content_sets(self, content_sets: Repository):
         if not content_sets:
             return False
 
+        from cekit.generator.behave import BehaveGenerator
+
+        if isinstance(self, BehaveGenerator):
+            LOGGER.warning("Running via Behave so not requesting ODCS compose")
+            return False
+
         arch = platform.machine()
 
         if arch not in content_sets:
             raise CekitError(
                 "There are no content_sets defined for platform '{}'!".format(arch)
             )
 
@@ -581,18 +587,14 @@
         if "id" in repo:
             LOGGER.warning(
                 "Repository '{}' is defined as plain. It must be available "
                 "inside the image as Cekit will not inject it.".format(repo["name"])
             )
             return False
 
-        if "content_sets" in repo:
-            self._fetch_repos = True
-            return self._prepare_content_sets(repo)
-
         elif "rpm" in repo:
             self._prepare_repository_rpm(repo)
             return False
 
         elif "url" in repo:
             return True
```

### Comparing `cekit-4.6.0/cekit/generator/docker.py` & `cekit-4.7.0/cekit/generator/docker.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/generator/legacy_version.py` & `cekit-4.7.0/cekit/generator/legacy_version.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/generator/osbs.py` & `cekit-4.7.0/cekit/generator/osbs.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/log.py` & `cekit-4.7.0/cekit/log.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/template_helper.py` & `cekit-4.7.0/cekit/template_helper.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/templates/help.jinja` & `cekit-4.7.0/cekit/templates/help.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/templates/template.jinja` & `cekit-4.7.0/cekit/templates/template.jinja`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/test/behave_runner.py` & `cekit-4.7.0/cekit/test/behave_runner.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/test/behave_tester.py` & `cekit-4.7.0/cekit/test/behave_tester.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/test/collector.py` & `cekit-4.7.0/cekit/test/collector.py`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/cekit/tools.py` & `cekit-4.7.0/cekit/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,19 @@
 
     :param cmd: The command to execute
     :param capture_output: Whether to capture the output or not
     :param exception_message: An optional detailed exception message
     :param check: Whether to check the return code (defaults to True)
     :return: a CompletedProcess object
     """
-    logger.debug("Executing '{}'.".format(" ".join(cmd)))
+    logger.debug(
+        "Executing '{}'.".format(
+            " ".join("'" + w + "'" if " " in w else w for w in cmd)
+        )
+    )
     try:
         # While it would be nicer to use
         #   result = subprocess.run(
         #        cmd, capture_output=capture_output, check=check, text=True
         #   )
         # capture_output and text are not available on Python 3.6
         stdout_capture = None
```

### Comparing `cekit-4.6.0/cekit.egg-info/PKG-INFO` & `cekit-4.7.0/cekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cekit
-Version: 4.6.0
+Version: 4.7.0
 Summary: Container image creation tool
 Home-page: https://github.com/cekit/cekit
-Download-URL: https://github.com/cekit/cekit/archive/4.6.0.tar.gz
+Download-URL: https://github.com/cekit/cekit/archive/4.7.0.tar.gz
 Author: CEKit team
 Author-email: cekit@cekit.io
 License: MIT
 License-File: LICENSE
 
 CEKit
 =====
```

### Comparing `cekit-4.6.0/cekit.egg-info/SOURCES.txt` & `cekit-4.7.0/cekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/requirements.txt` & `cekit-4.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cekit-4.6.0/setup.py` & `cekit-4.7.0/setup.py`

 * *Files identical despite different names*

