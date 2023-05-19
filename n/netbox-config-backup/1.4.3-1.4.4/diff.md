# Comparing `tmp/netbox_config_backup-1.4.3.tar.gz` & `tmp/netbox_config_backup-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_config_backup-1.4.3.tar", last modified: Tue May  9 15:10:55 2023, max compression
+gzip compressed data, was "netbox_config_backup-1.4.4.tar", last modified: Fri May 19 19:39:07 2023, max compression
```

## Comparing `netbox_config_backup-1.4.3.tar` & `netbox_config_backup-1.4.4.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/enqueue_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/fix_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/runbackup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0002_git_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0004_custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0005_commit_add_time_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0010_backup_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0011_alter_backup_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0012_backup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/models/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.260462 netbox_config_backup-1.4.3/netbox_config_backup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backups.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/diff.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/repository.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/ncb_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/rq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/enqueue_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/fix_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/runbackup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0002_git_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0004_custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0005_commit_add_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0010_backup_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0011_alter_backup_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0012_backup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.869653 netbox_config_backup-1.4.4/netbox_config_backup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/diff.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/repository.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/ncb_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/setup.py
```

### Comparing `netbox_config_backup-1.4.3/LICENSE` & `netbox_config_backup-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/PKG-INFO` & `netbox_config_backup-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_config_backup
-Version: 1.4.3
+Version: 1.4.4
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.3/README.md` & `netbox_config_backup-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/__init__.py` & `netbox_config_backup-1.4.4/netbox_config_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/choices.py` & `netbox_config_backup-1.4.4/netbox_config_backup/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/filtersets.py` & `netbox_config_backup-1.4.4/netbox_config_backup/filtersets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import django_filters
+import netaddr
 from django.core.exceptions import ValidationError
 from django.db.models import Q
 from django.utils.translation import gettext as _
+from netaddr import AddrFormatError
 
 from ipam.models import IPAddress
 from netbox.filtersets import NetBoxModelFilterSet, BaseFilterSet
 from dcim.models import Device
 from netbox_config_backup import models
 from netbox_config_backup.choices import FileTypeChoices
 from utilities.filters import MultiValueCharFilter
@@ -38,18 +40,28 @@
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         qs_filter = (
             Q(name__icontains=value) |
             Q(device__name__icontains=value) |
-            Q(device__primary_ip4__address__net_host_contained=value) |
-            Q(device__primary_ip6__address__net_host_contained=value) |
-            Q(ip__address__net_host_contained=value)
+            Q(device__primary_ip4__address__contains=value.strip()) |
+            Q(device__primary_ip6__address__contains=value.strip()) |
+            Q(ip__address__contains=value.strip())
         )
+
+        try:
+            prefix = str(netaddr.IPNetwork(value.strip()).cidr)
+            qs_filter |= Q(device__primary_ip4__address__net_host_contained=prefix)
+            qs_filter |= Q(device__primary_ip6__address__net_host_contained=prefix)
+            qs_filter |= Q(ip__address__net_host_contained=prefix)
+
+        except (AddrFormatError, ValueError):
+            pass
+
         return queryset.filter(qs_filter)
 
     def filter_address(self, queryset, name, value):
         try:
             return queryset.filter(ip__address__net_host_contained=value)
         except ValidationError:
             return queryset.none()
```

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/forms.py` & `netbox_config_backup-1.4.4/netbox_config_backup/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/git.py` & `netbox_config_backup-1.4.4/netbox_config_backup/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/fix_missing.py` & `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/fix_missing.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/rebuild.py` & `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/rebuild.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/runbackup.py` & `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/runbackup.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0001_initial.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0002_git_models.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0002_git_models.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0003_primary_model_to_bigid.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0010_backup_ip.py` & `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0010_backup_ip.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/models/backups.py` & `netbox_config_backup-1.4.4/netbox_config_backup/models/backups.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .abstract import BigIDModel
 from netbox_config_backup.utils.rq import remove_queued
 from ..utils import Differ
 
 logger = logging.getLogger(f"netbox_config_backup")
 
 
-class Backup(BigIDModel):
+class Backup(NetBoxModel):
     name = models.CharField(max_length=255, unique=True)
     uuid = models.UUIDField(default=uuid.uuid4, editable=False)
     status = models.CharField(
         max_length=50,
         choices=StatusChoices,
         default=StatusChoices.STATUS_ACTIVE
     )
```

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/models/jobs.py` & `netbox_config_backup-1.4.4/netbox_config_backup/models/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/navigation.py` & `netbox_config_backup-1.4.4/netbox_config_backup/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/tables.py` & `netbox_config_backup-1.4.4/netbox_config_backup/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/tasks.py` & `netbox_config_backup-1.4.4/netbox_config_backup/tasks.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/template_content.py` & `netbox_config_backup-1.4.4/netbox_config_backup/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backup.html` & `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backup.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backups.html` & `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backups.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/diff.html` & `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/diff.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/urls.py` & `netbox_config_backup-1.4.4/netbox_config_backup/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/utils/backups.py` & `netbox_config_backup-1.4.4/netbox_config_backup/utils/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/utils/git.py` & `netbox_config_backup-1.4.4/netbox_config_backup/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/utils/rq.py` & `netbox_config_backup-1.4.4/netbox_config_backup/utils/rq.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup/views.py` & `netbox_config_backup-1.4.4/netbox_config_backup/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     actions = ['config', 'diff']
     action_perms = {
         'config': {'view'},
         'diff': {'view'},
     }
     tab = ViewTab(
         label='View Backups',
+        badge=lambda obj: BackupCommitTreeChange.objects.filter(backup=obj, file__isnull=False).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(backup=parent, file__isnull=False)
 
     def get_extra_context(self, request, instance):
         return {
```

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup.egg-info/PKG-INFO` & `netbox_config_backup-1.4.4/netbox_config_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-backup
-Version: 1.4.3
+Version: 1.4.4
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.3/netbox_config_backup.egg-info/SOURCES.txt` & `netbox_config_backup-1.4.4/netbox_config_backup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 netbox_config_backup/views.py
 netbox_config_backup.egg-info/PKG-INFO
 netbox_config_backup.egg-info/SOURCES.txt
 netbox_config_backup.egg-info/dependency_links.txt
 netbox_config_backup.egg-info/not-zip-safe
 netbox_config_backup.egg-info/requires.txt
 netbox_config_backup.egg-info/top_level.txt
+netbox_config_backup/api/__init__.py
+netbox_config_backup/api/nested_serializers.py
+netbox_config_backup/api/serializers.py
 netbox_config_backup/management/__init__.py
 netbox_config_backup/management/commands/__init__.py
 netbox_config_backup/management/commands/enqueue_if_needed.py
 netbox_config_backup/management/commands/fix_missing.py
 netbox_config_backup/management/commands/rebuild.py
 netbox_config_backup/management/commands/runbackup.py
 netbox_config_backup/migrations/0001_initial.py
```

### Comparing `netbox_config_backup-1.4.3/setup.py` & `netbox_config_backup-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_config_backup',
-    version='1.4.3',
+    version='1.4.4',
     description='NetBox Configuration Backup',
     long_description='Plugin to backup device configuration',
     url='https://github.com/dansheps/netbox-config-backup/',
     download_url='https://github.com/dansheps/netbox-config-backup/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

