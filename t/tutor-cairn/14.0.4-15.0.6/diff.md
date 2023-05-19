# Comparing `tmp/tutor-cairn-14.0.4.tar.gz` & `tmp/tutor-cairn-15.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-cairn-14.0.4.tar", last modified: Fri May 19 08:15:49 2023, max compression
+gzip compressed data, was "tutor-cairn-15.0.6.tar", last modified: Fri May 19 08:15:29 2023, max compression
```

## Comparing `tutor-cairn-14.0.4.tar` & `tutor-cairn-15.0.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/
--rw-rw-r--   0 regis     (1000) regis     (1000)       80 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/MANIFEST.in
--rw-rw-r--   0 regis     (1000) regis     (1000)    16703 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)    15889 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/README.rst
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/setup.cfg
--rw-rw-r--   0 regis     (1000) regis     (1000)     1610 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/setup.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.613566 tutor-cairn-14.0.4/tutor_cairn.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)    16703 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     2500 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       45 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       22 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       11 2023-05-19 08:15:49.000000 tutor-cairn-14.0.4/tutor_cairn.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.613566 tutor-cairn-14.0.4/tutorcairn/
--rw-rw-r--   0 regis     (1000) regis     (1000)       24 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/__about__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/patches/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/patches/.gitignore
--rw-rw-r--   0 regis     (1000) regis     (1000)       87 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/patches/caddyfile
--rw-rw-r--   0 regis     (1000) regis     (1000)     9124 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/patches/k8s-deployments
--rw-rw-r--   0 regis     (1000) regis     (1000)     2625 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/patches/k8s-jobs
--rw-rw-r--   0 regis     (1000) regis     (1000)      759 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/patches/k8s-services
--rw-rw-r--   0 regis     (1000) regis     (1000)      868 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/patches/k8s-volumes
--rw-rw-r--   0 regis     (1000) regis     (1000)      981 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/patches/kustomization-configmapgenerator
--rw-rw-r--   0 regis     (1000) regis     (1000)     1703 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/patches/local-docker-compose-jobs-services
--rw-rw-r--   0 regis     (1000) regis     (1000)     3256 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/patches/local-docker-compose-services
--rw-rw-r--   0 regis     (1000) regis     (1000)     2008 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/plugin.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.613566 tutor-cairn-14.0.4/tutorcairn/templates/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.613566 tutor-cairn-14.0.4/tutorcairn/templates/cairn/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)      350 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/auth.json
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
--rw-rw-r--   0 regis     (1000) regis     (1000)      734 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      430 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     2121 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     2250 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      343 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     1093 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)      985 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
--rw-rw-r--   0 regis     (1000) regis     (1000)     1277 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/users.d/
--rw-rw-r--   0 regis     (1000) regis     (1000)      269 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.613566 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/openedx/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/openedx/scripts/
--rw-rw-r--   0 regis     (1000) regis     (1000)     3245 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/bootstrap/
--rw-rw-r--   0 regis     (1000) regis     (1000)   115036 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
--rw-rw-r--   0 regis     (1000) regis     (1000)     3896 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/superset_config.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/
--rw-rw-r--   0 regis     (1000) regis     (1000)      405 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/file.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      413 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/k8s.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      367 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/local.toml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/partials/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1929 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      112 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)      224 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
--rwxrwxr-x   0 regis     (1000) regis     (1000)     4981 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
--rwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/clickhouse-auth.json
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/
--rw-rw-r--   0 regis     (1000) regis     (1000)      902 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/scripts/
--rw-rw-r--   0 regis     (1000) regis     (1000)     9775 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/.gitignore
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-clickhouse/
--rw-rw-r--   0 regis     (1000) regis     (1000)       57 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-clickhouse/init
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-openedx/
--rw-rw-r--   0 regis     (1000) regis     (1000)       44 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-openedx/init
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:49.617567 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-superset/
--rw-rw-r--   0 regis     (1000) regis     (1000)      390 2023-05-19 08:15:46.000000 tutor-cairn-14.0.4/tutorcairn/templates/cairn/hooks/cairn-superset/init
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       80 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/MANIFEST.in
+-rw-rw-r--   0 regis     (1000) regis     (1000)    16700 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)    15886 2023-05-19 08:15:25.000000 tutor-cairn-15.0.6/README.rst
+-rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/setup.cfg
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1610 2023-05-19 08:15:25.000000 tutor-cairn-15.0.6/setup.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutor_cairn.egg-info/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    16700 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2500 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/SOURCES.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/dependency_links.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       45 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/entry_points.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       22 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/requires.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       11 2023-05-19 08:15:29.000000 tutor-cairn-15.0.6/tutor_cairn.egg-info/top_level.txt
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       24 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/__about__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/patches/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/.gitignore
+-rw-rw-r--   0 regis     (1000) regis     (1000)       87 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/caddyfile
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9124 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-deployments
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3003 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-jobs
+-rw-rw-r--   0 regis     (1000) regis     (1000)      759 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)      868 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/k8s-volumes
+-rw-rw-r--   0 regis     (1000) regis     (1000)      981 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/kustomization-configmapgenerator
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1858 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-jobs-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3256 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4838 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/plugin.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      350 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/auth.json
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      734 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)      430 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2121 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2250 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)      343 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1093 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)      985 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1277 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/users.d/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      269 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.912021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3245 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/
+-rw-rw-r--   0 regis     (1000) regis     (1000)   115036 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4316 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/superset_config.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      405 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/file.toml
+-rw-rw-r--   0 regis     (1000) regis     (1000)      413 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/k8s.toml
+-rw-rw-r--   0 regis     (1000) regis     (1000)      367 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/local.toml
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1929 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
+-rw-rw-r--   0 regis     (1000) regis     (1000)      112 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      554 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
+-rwxrwxr-x   0 regis     (1000) regis     (1000)     5017 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
+-rwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/clickhouse-auth.json
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1209 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9638 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-clickhouse/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       57 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-openedx/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       44 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-openedx/init
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-19 08:15:29.916021 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-superset/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      390 2023-05-19 07:41:10.000000 tutor-cairn-15.0.6/tutorcairn/templates/cairn/tasks/cairn-superset/init
```

### Comparing `tutor-cairn-14.0.4/PKG-INFO` & `tutor-cairn-15.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 14.0.4
+Version: 15.0.6
 Summary: cairn plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
 Platform: UNKNOWN
@@ -78,30 +78,31 @@
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
     tutor local quickstart
 
-Create credentials to access the Clickhouse database::
+Create a user to access both in the Clickhouse database and the Superset frontend::
 
-    tutor local run cairn-clickhouse cairn createuser YOURUSERNAME
+    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Create an admin user to access the frontend::
+You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
 
-    # You will be prompted for a new password
-    tutor local run cairn-superset cairn createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+To make this user an administrator, add the ``--admin`` option::
 
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
 
-At this point, your user should have access to Cairn but its account will not include any dashboard. To import the "Course overview" dashboard that comes with Cairn, run::
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-    tutor local run cairn-superset cairn bootstrap-dashboards YOURUSERNAME /app/bootstrap/courseoverview.json
+You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
 
-Some event data will be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
+Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
     :alt: Course overview dashboard part 1
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
     :alt: Course overview dashboard part 2
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
     :alt: Course overview dashboard part 3
```

### Comparing `tutor-cairn-14.0.4/README.rst` & `tutor-cairn-15.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,31 @@
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
     tutor local quickstart
 
-Create credentials to access the Clickhouse database::
+Create a user to access both in the Clickhouse database and the Superset frontend::
 
-    tutor local run cairn-clickhouse cairn createuser YOURUSERNAME
+    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Create an admin user to access the frontend::
+You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
 
-    # You will be prompted for a new password
-    tutor local run cairn-superset cairn createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+To make this user an administrator, add the ``--admin`` option::
 
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
 
-At this point, your user should have access to Cairn but its account will not include any dashboard. To import the "Course overview" dashboard that comes with Cairn, run::
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-    tutor local run cairn-superset cairn bootstrap-dashboards YOURUSERNAME /app/bootstrap/courseoverview.json
+You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
 
-Some event data will be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
+Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
     :alt: Course overview dashboard part 1
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
     :alt: Course overview dashboard part 2
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
     :alt: Course overview dashboard part 3
```

### Comparing `tutor-cairn-14.0.4/setup.py` & `tutor-cairn-15.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     license="AGPLv3",
     author="Overhang.IO",
     description="cairn plugin for Tutor",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
-    install_requires=["tutor>=14.0.0,<15.0.0"],
-    entry_points={"tutor.plugin.v0": ["cairn = tutorcairn.plugin"]},
+    install_requires=["tutor>=15.0.0,<16.0.0"],
+    entry_points={"tutor.plugin.v1": ["cairn = tutorcairn.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
```

### Comparing `tutor-cairn-14.0.4/tutor_cairn.egg-info/PKG-INFO` & `tutor-cairn-15.0.6/tutor_cairn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 14.0.4
+Version: 15.0.6
 Summary: cairn plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
 Platform: UNKNOWN
@@ -78,30 +78,31 @@
 
     tutor plugins enable cairn
 
 Then, restart your platform and run the initialization scripts::
 
     tutor local quickstart
 
-Create credentials to access the Clickhouse database::
+Create a user to access both in the Clickhouse database and the Superset frontend::
 
-    tutor local run cairn-clickhouse cairn createuser YOURUSERNAME
+    tutor local do cairn-createuser YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-Create an admin user to access the frontend::
+You can use the ``--password=<PASSWORD>`` option to provide a password on the command line.
 
-    # You will be prompted for a new password
-    tutor local run cairn-superset cairn createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+To make this user an administrator, add the ``--admin`` option::
 
-You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
+    tutor local do cairn-createuser --admin YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
+
+To add the default dashboards to the new user, add the ``--bootstrap-dashboards`` option::
 
-At this point, your user should have access to Cairn but its account will not include any dashboard. To import the "Course overview" dashboard that comes with Cairn, run::
+    tutor local do cairn-createuser --bootstrap-dashboards YOURUSERNAME YOURUSERNAME@YOUREMAIL.COM
 
-    tutor local run cairn-superset cairn bootstrap-dashboards YOURUSERNAME /app/bootstrap/courseoverview.json
+You can then access the frontend with the user credentials you just created. Open http(s)://data.<YOUR_LMS_HOST> in your browser. When running locally, this will be http://data.local.overhang.io. The admin user will automatically be granted access to the "openedx" database in Superset and will be able to query all tables.
 
-Some event data will be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
+Some event data might be missing from your dashboards: just start using your LMS and refresh your dashboard. The new events should appear immediately.
 
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-01.png
     :alt: Course overview dashboard part 1
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-02.png
     :alt: Course overview dashboard part 2
 .. image:: https://overhang.io/static/catalog/img/cairn/courseoverview-03.png
     :alt: Course overview dashboard part 3
```

### Comparing `tutor-cairn-14.0.4/tutor_cairn.egg-info/SOURCES.txt` & `tutor-cairn-15.0.6/tutor_cairn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
 tutorcairn/templates/cairn/build/.gitignore
 tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
 tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
 tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/clickhouse-auth.json
 tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
 tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn
-tutorcairn/templates/cairn/hooks/.gitignore
-tutorcairn/templates/cairn/hooks/cairn-clickhouse/init
-tutorcairn/templates/cairn/hooks/cairn-openedx/init
-tutorcairn/templates/cairn/hooks/cairn-superset/init
+tutorcairn/templates/cairn/tasks/.gitignore
+tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
+tutorcairn/templates/cairn/tasks/cairn-openedx/init
+tutorcairn/templates/cairn/tasks/cairn-superset/init
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/k8s-deployments` & `tutor-cairn-15.0.6/tutorcairn/patches/k8s-deployments`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     spec:
       securityContext:
         runAsUser: 1000
         runAsGroup: 1000
       containers:
         - name: cairn-superset-worker
           image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
-          args: ["celery", "worker", "--app=superset.tasks.celery_app:app", "-Ofair", "-l", "INFO"]
+          args: ["celery", "--app=superset.tasks.celery_app:app", "worker", "-Ofair", "-l", "INFO"]
           volumeMounts:
             - mountPath: /app/superset_config.py
               name: config
               subPath: superset_config.py
           securityContext:
             allowPrivilegeEscalation: false
       volumes:
@@ -264,15 +264,15 @@
     spec:
       securityContext:
         runAsUser: 1000
         runAsGroup: 1000
       containers:
         - name: cairn-superset-worker-beat
           image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
-          args: ["celery", "beat", "--app=superset.tasks.celery_app:app", "--pidfile", "/tmp/celerybeat.pid", "-l", "INFO", "--schedule=/tmp/celerybeat-schedule"]
+          args: ["celery", "--app=superset.tasks.celery_app:app", "beat", "--pidfile", "/tmp/celerybeat.pid", "-l", "INFO", "--schedule=/tmp/celerybeat-schedule"]
           volumeMounts:
             - mountPath: /app/superset_config.py
               name: config
               subPath: superset_config.py
           securityContext:
             allowPrivilegeEscalation: false
       volumes:
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/k8s-jobs` & `tutor-cairn-15.0.6/tutorcairn/patches/k8s-jobs`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,29 @@
       containers:
         - name: cairn-superset
           image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
           volumeMounts:
             - mountPath: /app/superset_config.py
               name: config
               subPath: superset_config.py
+            - mountPath: /app/bootstrap/
+              name: bootstrap
+            - mountPath: /scripts/clickhouse-auth.json
+              name: clickhouse-auth
+              subPath: auth.json
       volumes:
         - name: config
           configMap:
             name: cairn-superset-config
+        - name: bootstrap
+          configMap:
+            name: cairn-superset-bootstrap
+        - name: clickhouse-auth
+          configMap:
+            name: cairn-clickhouse-auth
 ---
 apiVersion: batch/v1
 kind: Job
 metadata:
   name: cairn-openedx-job
   labels:
     app.kubernetes.io/component: job
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/k8s-services` & `tutor-cairn-15.0.6/tutorcairn/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/k8s-volumes` & `tutor-cairn-15.0.6/tutorcairn/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/kustomization-configmapgenerator` & `tutor-cairn-15.0.6/tutorcairn/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/local-docker-compose-jobs-services` & `tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-jobs-services`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         {%- endfor %}
     environment:
         CLICKHOUSE_DO_NOT_CHOWN: "1"
 cairn-superset-job:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
+        - ../plugins/cairn/apps/clickhouse/auth.json:/scripts/clickhouse-auth.json:ro
+        - ../plugins/cairn/apps/superset/bootstrap:/app/bootstrap:ro
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-openedx-job:
     image: {{ DOCKER_IMAGE_OPENEDX }}
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/patches/local-docker-compose-services` & `tutor-cairn-15.0.6/tutorcairn/patches/local-docker-compose-services`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,26 @@
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-superset-worker:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
-    command: celery worker --app=superset.tasks.celery_app:app -Ofair -l INFO
+    command: celery --app=superset.tasks.celery_app:app worker -Ofair -l INFO
     restart: unless-stopped
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 cairn-superset-worker-beat:
     image: {{ CAIRN_SUPERSET_DOCKER_IMAGE }}
     volumes:
         - ../plugins/cairn/apps/superset/superset_config.py:/app/superset_config.py:ro
-    command: celery beat --app=superset.tasks.celery_app:app --pidfile /tmp/celerybeat.pid -l INFO --schedule=/tmp/celerybeat-schedule
+    command: celery --app=superset.tasks.celery_app:app beat --pidfile /tmp/celerybeat.pid -l INFO --schedule=/tmp/celerybeat-schedule
     restart: unless-stopped
     healthcheck:
         disable: true
     depends_on:
         {% if RUN_REDIS %}- redis{% endif %}
         - cairn-postgresql
 {% if CAIRN_RUN_POSTGRESQL %}
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999800701530612%*

 * *Differences: {"'dashboards'": "{0: {'__Dashboard__': {'slices': {14: {'__Slice__': {'params': "*

 * *                 '\'{"adhoc_filters": [], "bar_stacked": false, "bottom_margin": "auto", '*

 * *                 '"color_scheme": "supersetColors", "columns": ["course_id"], "datasource": '*

 * *                 '"38__table", "extra_form_data": {}, "groupby": ["display_name"], "label_colors": '*

 * *                 '{}, "metrics": [{"aggregate": "COUNT_DISTINCT", "column": {"column_name": '*

 * *                 '"user_id", "description": null, […]*

```diff
@@ -164,15 +164,15 @@
                     },
                     {
                         "__Slice__": {
                             "cache_timeout": null,
                             "datasource_name": "openedx.Course block completions",
                             "datasource_type": "table",
                             "id": 110,
-                            "params": "{\"adhoc_filters\": [], \"bar_stacked\": false, \"bottom_margin\": \"auto\", \"color_scheme\": \"supersetColors\", \"columns\": [\"course_id\"], \"datasource\": \"38__table\", \"extra_form_data\": {}, \"groupby\": [\"display_name\"], \"label_colors\": {}, \"metrics\": [{\"aggregate\": \"COUNT_DISTINCT\", \"column\": {\"column_name\": \"user_id\", \"description\": null, \"expression\": \"\", \"filterable\": true, \"groupby\": true, \"id\": 321, \"is_dttm\": false, \"python_date_format\": null, \"type\": \"UINT64\", \"type_generic\": null, \"verbose_name\": null}, \"expressionType\": \"SIMPLE\", \"hasCustomLabel\": false, \"isNew\": false, \"label\": \"COUNT_DISTINCT(user_id)\", \"optionName\": \"metric_g9cvvlpke9h_z8bnkxr8axa\", \"sqlExpression\": null}], \"order_desc\": false, \"row_limit\": 10000, \"show_bar_value\": false, \"show_legend\": false, \"slice_id\": 110, \"time_range\": \"No filter\", \"time_range_endpoints\": [\"inclusive\", \"exclusive\"], \"url_params\": {}, \"viz_type\": \"dist_bar\", \"x_axis_label\": \"Course block\", \"x_ticks_layout\": \"auto\", \"y_axis_bounds\": [null, null], \"y_axis_format\": \"SMART_NUMBER\", \"y_axis_label\": \"Number of students\", \"remote_id\": 110, \"datasource_name\": \"Course block completions\", \"schema\": \"openedx\", \"database_name\": \"admin\"}",
+                            "params": "{\"adhoc_filters\": [], \"bar_stacked\": false, \"bottom_margin\": \"auto\", \"color_scheme\": \"supersetColors\", \"columns\": [\"course_id\"], \"datasource\": \"38__table\", \"extra_form_data\": {}, \"groupby\": [\"display_name\"], \"label_colors\": {}, \"metrics\": [{\"aggregate\": \"COUNT_DISTINCT\", \"column\": {\"column_name\": \"user_id\", \"description\": null, \"expression\": \"\", \"filterable\": true, \"groupby\": true, \"id\": 321, \"is_dttm\": false, \"python_date_format\": null, \"type\": \"UINT64\", \"type_generic\": null, \"verbose_name\": null}, \"expressionType\": \"SIMPLE\", \"hasCustomLabel\": false, \"isNew\": false, \"label\": \"COUNT_DISTINCT(user_id)\", \"optionName\": \"metric_g9cvvlpke9h_z8bnkxr8axa\", \"sqlExpression\": null}], \"order_desc\": false, \"row_limit\": 1000, \"show_bar_value\": false, \"show_legend\": false, \"slice_id\": 110, \"time_range\": \"No filter\", \"time_range_endpoints\": [\"inclusive\", \"exclusive\"], \"url_params\": {}, \"viz_type\": \"dist_bar\", \"x_axis_label\": \"Course block\", \"x_ticks_layout\": \"auto\", \"y_axis_bounds\": [null, null], \"y_axis_format\": \"SMART_NUMBER\", \"y_axis_label\": \"Number of students\", \"remote_id\": 110, \"datasource_name\": \"Course block completions\", \"schema\": \"openedx\", \"database_name\": \"admin\"}",
                             "slice_name": "Course completion",
                             "viz_type": "dist_bar"
                         }
                     },
                     {
                         "__Slice__": {
                             "cache_timeout": null,
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/superset/superset_config.py` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/superset/superset_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 from cachelib.redis import RedisCache
 from celery.schedules import crontab
 
 # https://superset.apache.org/docs/installation/configuring-superset
 SECRET_KEY = "{{ CAIRN_SUPERSET_SECRET_KEY }}"
 SQLALCHEMY_DATABASE_URI = "postgresql+psycopg2://{{ CAIRN_POSTGRESQL_USERNAME }}:{{ CAIRN_POSTGRESQL_PASSWORD }}@cairn-postgresql/{{ CAIRN_POSTGRESQL_DATABASE }}"
 
+{% if not ENABLE_WEB_PROXY %}
+# Caddy is running behind a proxy: Superset needs to handle x-forwarded-* headers
+# https://flask.palletsprojects.com/en/latest/deploying/proxy_fix/
+ENABLE_PROXY_FIX = True
+{% endif %}
+
 # Languages
 # https://github.com/apache/superset/blob/dc575080d7e43d40b1734bb8f44fdc291cb95b11/superset/config.py#L324
 available_languages = {
     "en": {"flag": "us", "name": "English"},
     "es": {"flag": "es", "name": "Spanish"},
     "it": {"flag": "it", "name": "Italian"},
     "fr": {"flag": "fr", "name": "French"},
@@ -53,14 +59,16 @@
 RESULTS_BACKEND = RedisCache(
     host=REDIS_HOST,
     port=REDIS_PORT,
     db=REDIS_CACHE_DB,
     key_prefix="superset_results",
 )
 
+# TODO implement FILTER_STATE_CACHE_CONFIG and EXPLORE_FORM_DATA_CACHE_CONFIG such that we get rid of the warning messages
+
 class CeleryConfig:  # pylint: disable=too-few-public-methods
     BROKER_URL = f"redis://{REDIS_HOST}:{REDIS_PORT}/{REDIS_CELERY_DB}"
     CELERY_IMPORTS = ("superset.sql_lab", "superset.tasks")
     CELERYD_LOG_LEVEL = "DEBUG"
     CELERYD_PREFETCH_MULTIPLIER = 1
     CELERY_ACKS_LATE = False
     CELERY_ANNOTATIONS = {
@@ -89,14 +97,19 @@
 
 
 CELERY_CONFIG = CeleryConfig
 
 # Avoid duplicate logging because of propagation to root logger
 logging.getLogger("superset").propagate = False
 
+# Enable dashboard embedding
+FEATURE_FLAGS = {
+    "EMBEDDED_SUPERSET": True
+}
+
 # Enable some custom feature flags
 # Do this once native filters are fully functional https://github.com/apache/superset/projects/15+
 # def get_cairn_feature_flags(flags):
 #     flags["DASHBOARD_NATIVE_FILTERS"] = True
 #     return flags
 # GET_FEATURE_FLAGS_FUNC = get_cairn_feature_flags
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,15 @@
         "CREATE TABLE IF NOT EXISTS _migrations (name String) ENGINE = MergeTree PRIMARY KEY(name) ORDER BY name"
     )
 
     # Apply migrations
     migrations = sorted(glob(os.path.join(args.path, "*")))
     for path in migrations:
         migration_name = os.path.basename(path)
-        print(
-            f"Applying migration {migration_name}... ", end=" "
-        )
+        print(f"Applying migration {migration_name}... ", end=" ")
         query = f"SELECT 'applied' FROM _migrations WHERE name='{migration_name}'"
         is_applied = run_query(query)
         if is_applied == "applied":
             print("SKIP")
         else:
             if not args.dry_run and not args.fake:
                 run_command("--queries-file", path)
@@ -146,14 +144,15 @@
         str(CLICKHOUSE_AUTH["port"]),
         "--user",
         CLICKHOUSE_AUTH["username"],
         "--password",
         CLICKHOUSE_AUTH["password"],
         "--multiline",
         "--multiquery",
+        "--history_file=/tmp/.clickhouse-client-history",
     ]
     if CLICKHOUSE_AUTH["http_scheme"] == "https":
         command.append("--secure")
     command += args
     return command
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # Superset image with additional database drivers
 # https://hub.docker.com/r/apache/superset
+# https://github.com/apache/superset/releases
+# https://github.com/apache/superset/blob/master/Dockerfile
 # https://superset.apache.org/docs/databases/installing-database-drivers
-FROM docker.io/apache/superset:1.3.2
+FROM docker.io/apache/superset:2.0.0
 
 USER root
 
 # https://pypi.org/project/clickhouse-driver/
-# https://pypi.org/project/clickhouse-sqlalchemy/
 # https://pypi.org/project/mysqlclient/
-RUN pip install clickhouse-driver==0.2.2 mysqlclient==2.1.0
-RUN pip install clickhouse-sqlalchemy==0.1.7
+# https://pypi.org/project/clickhouse-sqlalchemy/
+RUN pip install clickhouse-driver==0.2.4 mysqlclient==2.1.1
+# Later versions of clickhouse-sqlalchemy will not work.
+# Note that this connector be replaced by clickhouse-connect in v2.0.1:
+# https://github.com/apache/superset/pull/22039
+RUN pip install clickhouse-sqlalchemy==0.1.10
 
 COPY --chown=superset:superset ./scripts /scripts
 RUN chmod a+x /scripts/*
 ENV PATH /scripts:${PATH}
 
 USER superset
 
-HEALTHCHECK CMD curl -f "http://localhost:8000"
+# This is required to have a proper healthcheck
+ENV SUPERSET_PORT=8000
 
 ENTRYPOINT []
 CMD gunicorn \
     --bind  "0.0.0.0:8000" \
     --access-logfile '-' \
     --error-logfile '-' \
     --workers 2 \
```

### Comparing `tutor-cairn-14.0.4/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn` & `tutor-cairn-15.0.6/tutorcairn/templates/cairn/build/cairn-superset/scripts/cairn`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 app.app_context().push()
 
 from superset.connectors.sqla.models import SqlaTable
 from superset.models.core import Database
 from superset.models.slice import Slice
 from superset.extensions import db, security_manager
 import superset.dashboards.commands.importers.v0 as importers
-from superset.utils.core import get_or_create_db
+from superset.utils.database import get_or_create_db
 from werkzeug.security import generate_password_hash
 
 
 now = time()
 
 
 def main():
@@ -86,14 +86,16 @@
     parser_dashboards.add_argument("path", nargs="+")
     parser_dashboards.set_defaults(func=bootstrap_dashboards)
 
     args = parser.parse_args()
     args.func(args)
 
 
+# Note: we'd like to get rid of this command by relying on `superset fab create-user`
+# but the "create-user" command fails if the user already exists.
 def bootstrap_user(args):
     # Bootstrap database
     database_name = args.db or args.username
     bootstrap_database(args.username, database_name)
 
     # Get or create user
     user = security_manager.find_user(args.username)
@@ -117,15 +119,17 @@
             args.email,
             security_manager.find_role(base_role_name),
             password=password,
         )
         if user is None or user is False:
             # This may happen for instance when the email address is already associated
             # to a different username
-            raise RuntimeError(f"Failed to create user '{args.username}' email='{args.email}'")
+            raise RuntimeError(
+                f"Failed to create user '{args.username}' email='{args.email}'"
+            )
 
     # Associate role with the same name to user, if it exists
     role_name = args.role or args.username
 
     def check_permission(permission_view):
         permission_name = str(permission_view)
         if permission_name in [
@@ -151,45 +155,40 @@
         user.roles.append(role)
         db.session.add(user)
         db.session.commit()
     print("Done.")
 
 
 def bootstrap_database(username, database_name):
-    with open(os.path.join(os.path.dirname(__file__), "clickhouse-auth.json")) as f:
+    with open(
+        os.path.join(os.path.dirname(__file__), "clickhouse-auth.json"),
+        encoding="utf-8",
+    ) as f:
         CLICKHOUSE_AUTH = json.load(f)
 
     host = CLICKHOUSE_AUTH["host"]
     port = CLICKHOUSE_AUTH["port"]
     database = CLICKHOUSE_AUTH["database"]
     uri = f"clickhouse+native://{username}:@{host}:{port}/{database}"
     database = get_or_create_db(database_name, uri, always_create=True)
 
-    # TODO get rid of the following once we upgrade clickhouse-sqlalchemy and we
-    # can disable reflection from the DSN
-    # https://github.com/xzkostyan/clickhouse-sqlalchemy/issues/151
-    # https://github.com/xzkostyan/clickhouse-sqlalchemy/issues/140
-    # This is preventing us from creating datasets from physical tables.
-    database_extra = json.loads(database.extra)
-    database_extra["engine_params"] = {"connect_args": {"server_version": "18.12.14"}}
-    database.extra = json.dumps(database_extra)
     db.session.add(database)
     db.session.commit()
 
 
+# Note: we would like to start using superset's native export/import-dashboards command
+# but we failed to get it to work.
 def bootstrap_dashboards(args):
     database_name = args.db or args.username
     database = load_database(database_name)
     user = load_user(args.username)
 
     for path in args.path:
         print(
-            "importing dashboard {} for user='{}' db='{}'... ".format(
-                path, user.username, database.database_name
-            )
+            f"importing dashboard {path} for user='{user.username}' db='{database.database_name}'... "
         )
         dashboard = load_dashboard_file(path)
         import_dashboard(dashboard, user, database)
 
 
 def load_database(database_name):
     return (
@@ -202,15 +201,15 @@
         db.session.query(security_manager.user_model)
         .filter(security_manager.user_model.username == username)
         .one()
     )
 
 
 def load_dashboard_file(path):
-    with open(path) as f:
+    with open(path, encoding="utf-8") as f:
         return json.load(f, object_hook=importers.decode_dashboards)
 
 
 def import_dashboard(data, user, database):
     # Load datasets
     for dataset in data["datasources"]:
         dataset.params = "{}"
@@ -223,24 +222,24 @@
 
     for dashboard in data["dashboards"]:
         # Load slices
         new_slices = []
         slices = dashboard.slices[:]
         old_to_new_slice_id_map = {}
 
-        for slice in slices:
+        for dashboard_slice in slices:
             # Make sure the new slice does not point to the old slice
-            params_dict = slice.params_dict
+            params_dict = dashboard_slice.params_dict
             params_dict["database_name"] = database.name
             params_dict.pop("remote_id")
-            slice.params = json.dumps(params_dict)
-            old_slice_id = slice.id
-            slice.id = None
+            dashboard_slice.params = json.dumps(params_dict)
+            old_slice_id = dashboard_slice.id
+            dashboard_slice.id = None
             # Create new slice
-            new_slice_id = importers.import_chart(slice, None, now)
+            new_slice_id = importers.import_chart(dashboard_slice, None, now)
             new_slice = db.session.query(Slice).get(new_slice_id)
             old_to_new_slice_id_map[old_slice_id] = new_slice_id
             # Make current user the new owner
             new_slice.owners.append(user)
             new_slices.append(new_slice)
             db.session.add(new_slice)
 
@@ -258,27 +257,28 @@
             ):
                 chart["meta"]["chartId"] = old_to_new_slice_id_map[
                     chart["meta"]["chartId"]
                 ]
         dashboard.position_json = json.dumps(position)
 
         # Update filter mapping
-        # import pdb; pdb.set_trace()
         metadata = json.loads(dashboard.json_metadata)
         new_filter_scopes = {}
         for old_slice_id, filter_scope in metadata["filter_scopes"].items():
             new_filter_scope = {}
             for filter_name, properties in filter_scope.items():
                 properties["immune"] = [
                     old_to_new_slice_id_map[old_immune_id]
                     for old_immune_id in properties["immune"]
                 ]
                 new_filter_scope[filter_name] = properties
             # Note that filter scope keys are str, not int
-            new_filter_scopes[str(old_to_new_slice_id_map[int(old_slice_id)])] = new_filter_scope
+            new_filter_scopes[
+                str(old_to_new_slice_id_map[int(old_slice_id)])
+            ] = new_filter_scope
         metadata["filter_scopes"] = new_filter_scopes
         dashboard.json_metadata = json.dumps(metadata)
 
         # Load dashboard
         db.session.add(dashboard)
 
         # Commit changes
```

