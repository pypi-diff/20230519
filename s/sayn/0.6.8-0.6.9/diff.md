# Comparing `tmp/sayn-0.6.8.tar.gz` & `tmp/sayn-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayn-0.6.8.tar", max compression
+gzip compressed data, was "sayn-0.6.9.tar", max compression
```

## Comparing `sayn-0.6.8.tar` & `sayn-0.6.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     7744 2023-04-03 17:04:21.765654 sayn-0.6.8/CHANGELOG.md
--rw-r--r--   0        0        0    10089 2021-03-18 12:17:49.585126 sayn-0.6.8/LICENSE.md
--rw-r--r--   0        0        0      544 2021-03-18 12:17:49.585201 sayn-0.6.8/NOTICE.md
--rw-r--r--   0        0        0     3254 2022-01-24 12:35:11.985071 sayn-0.6.8/README.md
--rw-r--r--   0        0        0       67 2021-03-18 12:17:49.585470 sayn-0.6.8/docs/api/database.md
--rw-r--r--   0        0        0       65 2022-07-19 09:36:59.894884 sayn-0.6.8/docs/api/python_task.md
--rw-r--r--   0        0        0     3598 2022-02-24 13:53:08.364628 sayn-0.6.8/docs/cli.md
--rw-r--r--   0        0        0      477 2021-03-18 12:17:49.585773 sayn-0.6.8/docs/css/admonitions.css
--rw-r--r--   0        0        0      689 2021-03-18 12:17:49.585848 sayn-0.6.8/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0    26013 2021-03-18 12:17:49.586118 sayn-0.6.8/docs/dag.png
--rw-r--r--   0        0        0    15035 2022-02-24 13:53:08.364916 sayn-0.6.8/docs/database_objects.md
--rw-r--r--   0        0        0     2725 2023-04-03 17:04:21.766383 sayn-0.6.8/docs/databases/bigquery.md
--rw-r--r--   0        0        0     1358 2021-03-18 12:17:49.586395 sayn-0.6.8/docs/databases/mysql.md
--rw-r--r--   0        0        0     2664 2021-04-29 16:40:55.449583 sayn-0.6.8/docs/databases/overview.md
--rw-r--r--   0        0        0     1372 2021-03-18 12:17:49.586586 sayn-0.6.8/docs/databases/postgresql.md
--rw-r--r--   0        0        0     6514 2023-04-03 17:04:21.766739 sayn-0.6.8/docs/databases/redshift.md
--rw-r--r--   0        0        0     1545 2021-03-18 12:17:49.586767 sayn-0.6.8/docs/databases/snowflake.md
--rw-r--r--   0        0        0      608 2021-03-18 12:17:49.586844 sayn-0.6.8/docs/databases/sqlite.md
--rw-r--r--   0        0        0      960 2022-01-24 12:35:11.987045 sayn-0.6.8/docs/installation.md
--rw-r--r--   0        0        0     6180 2021-04-29 16:40:55.449961 sayn-0.6.8/docs/parameters.md
--rw-r--r--   0        0        0     1609 2021-04-29 16:40:55.450116 sayn-0.6.8/docs/presets.md
--rw-r--r--   0        0        0    19176 2021-11-23 17:13:41.722989 sayn-0.6.8/docs/project_examples/bbc_news_nlp.md
--rw-r--r--   0        0        0  1084434 2021-11-23 17:13:41.729704 sayn-0.6.8/docs/project_examples/chart_race.gif
--rw-r--r--   0        0        0     3195 2021-11-23 17:13:41.730124 sayn-0.6.8/docs/project_examples/facebook_data_project.md
--rw-r--r--   0        0        0    17605 2021-11-23 17:13:41.730422 sayn-0.6.8/docs/project_examples/reddit_news_nlp.md
--rw-r--r--   0        0        0     1781 2021-11-23 17:13:41.730657 sayn-0.6.8/docs/project_examples/simple_etl.md
--rw-r--r--   0        0        0     1235 2021-03-18 12:17:49.587301 sayn-0.6.8/docs/project_structure.md
--rw-r--r--   0        0        0     1635 2022-01-24 12:35:11.987267 sayn-0.6.8/docs/settings/project_yaml.md
--rw-r--r--   0        0        0     4950 2022-02-24 13:53:08.366135 sayn-0.6.8/docs/settings/settings_yaml.md
--rw-r--r--   0        0        0     8177 2022-07-19 09:36:59.895926 sayn-0.6.8/docs/tasks/autosql.md
--rw-r--r--   0        0        0     7467 2022-02-24 13:53:08.366602 sayn-0.6.8/docs/tasks/copy.md
--rw-r--r--   0        0        0     1829 2021-04-29 16:40:55.451169 sayn-0.6.8/docs/tasks/dummy.md
--rw-r--r--   0        0        0     7835 2022-07-19 09:36:59.896330 sayn-0.6.8/docs/tasks/overview.md
--rw-r--r--   0        0        0    11394 2022-07-19 09:36:59.896724 sayn-0.6.8/docs/tasks/python.md
--rw-r--r--   0        0        0     9393 2022-11-08 18:05:17.851969 sayn-0.6.8/docs/tasks/sql.md
--rw-r--r--   0        0        0     1639 2022-08-04 14:21:08.499774 sayn-0.6.8/docs/tests/custom.md
--rw-r--r--   0        0        0     4121 2022-08-04 14:21:08.500832 sayn-0.6.8/docs/tests/overview.md
--rw-r--r--   0        0        0     1832 2022-02-24 13:53:08.367627 sayn-0.6.8/docs/tests/standard.md
--rw-r--r--   0        0        0   325125 2021-03-18 12:17:49.589475 sayn-0.6.8/docs/tutorials/sayn_run1.gif
--rw-r--r--   0        0        0     4520 2022-03-16 14:32:08.023722 sayn-0.6.8/docs/tutorials/tutorial_part1.md
--rw-r--r--   0        0        0     5243 2022-03-16 14:32:08.024011 sayn-0.6.8/docs/tutorials/tutorial_part2.md
--rw-r--r--   0        0        0     8014 2022-03-16 14:32:08.024289 sayn-0.6.8/docs/tutorials/tutorial_part3.md
--rw-r--r--   0        0        0     2326 2022-07-19 09:36:59.902566 sayn-0.6.8/mkdocs.yml
--rw-r--r--   0        0        0     2187 2023-04-03 17:04:21.768805 sayn-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-03 17:04:21.768914 sayn-0.6.8/sayn/__init__.py
--rw-r--r--   0        0        0     7728 2022-02-24 13:53:08.370450 sayn-0.6.8/sayn/cli.py
--rw-r--r--   0        0        0        0 2021-03-18 12:17:49.591152 sayn-0.6.8/sayn/core/__init__.py
--rw-r--r--   0        0        0    23306 2023-04-03 17:04:21.769079 sayn-0.6.8/sayn/core/app.py
--rw-r--r--   0        0        0     5342 2022-01-24 12:35:11.993153 sayn-0.6.8/sayn/core/errors.py
--rw-r--r--   0        0        0    15854 2023-04-03 17:04:21.769669 sayn-0.6.8/sayn/core/project.py
--rw-r--r--   0        0        0    11733 2023-04-03 17:04:21.769868 sayn-0.6.8/sayn/core/settings.py
--rw-r--r--   0        0        0    28266 2023-04-03 17:04:21.770039 sayn-0.6.8/sayn/database/__init__.py
--rw-r--r--   0        0        0    11528 2023-04-03 17:04:21.770667 sayn-0.6.8/sayn/database/bigquery.py
--rw-r--r--   0        0        0     1065 2022-02-24 13:53:08.372369 sayn-0.6.8/sayn/database/creator.py
--rw-r--r--   0        0        0     2101 2023-04-03 17:04:21.771342 sayn-0.6.8/sayn/database/mysql.py
--rw-r--r--   0        0        0     8802 2023-04-03 17:04:21.771461 sayn-0.6.8/sayn/database/objects.py
--rw-r--r--   0        0        0     1505 2023-04-03 17:04:21.771820 sayn-0.6.8/sayn/database/postgresql.py
--rw-r--r--   0        0        0     9191 2023-04-03 17:04:21.772084 sayn-0.6.8/sayn/database/redshift.py
--rw-r--r--   0        0        0     2507 2023-04-03 17:04:21.772736 sayn-0.6.8/sayn/database/snowflake.py
--rw-r--r--   0        0        0     3557 2023-04-03 17:04:21.772868 sayn-0.6.8/sayn/database/sqlite.py
--rw-r--r--   0        0        0     2181 2023-04-03 17:04:21.773646 sayn-0.6.8/sayn/database/templates/create_table.sql
--rw-r--r--   0        0        0      614 2023-04-03 17:04:21.774019 sayn-0.6.8/sayn/database/templates/create_view.sql
--rw-r--r--   0        0        0      349 2021-11-23 17:13:41.734017 sayn-0.6.8/sayn/database/templates/merge_tables.sql
--rw-r--r--   0        0        0     1366 2023-04-03 17:04:21.774115 sayn-0.6.8/sayn/database/templates/move_table.sql
--rw-r--r--   0        0        0      167 2023-04-03 17:04:21.774176 sayn-0.6.8/sayn/database/templates/redshift_load_batch.sql
--rw-r--r--   0        0        0      364 2023-04-03 17:04:21.774239 sayn-0.6.8/sayn/database/templates/redshift_merge_tables.sql
--rw-r--r--   0        0        0      664 2022-07-19 09:36:59.908339 sayn-0.6.8/sayn/database/templates/snowflake_load_batch.sql
--rw-r--r--   0        0        0      171 2022-02-24 13:53:08.373158 sayn-0.6.8/sayn/database/unknown.py
--rw-r--r--   0        0        0      156 2021-03-18 12:17:49.592845 sayn-0.6.8/sayn/logging/__init__.py
--rw-r--r--   0        0        0      714 2021-03-18 12:17:49.592944 sayn-0.6.8/sayn/logging/console_logger.py
--rw-r--r--   0        0        0     2903 2022-01-24 12:35:11.999438 sayn-0.6.8/sayn/logging/event_tracker.py
--rw-r--r--   0        0        0     6206 2022-02-24 13:53:08.373327 sayn-0.6.8/sayn/logging/fancy_logger.py
--rw-r--r--   0        0        0     1484 2022-02-24 13:53:08.373462 sayn-0.6.8/sayn/logging/file_logger.py
--rw-r--r--   0        0        0    20346 2023-04-03 17:04:21.774399 sayn-0.6.8/sayn/logging/log_formatter.py
--rw-r--r--   0        0        0     4039 2022-01-24 12:35:12.000136 sayn-0.6.8/sayn/logging/logger.py
--rw-r--r--   0        0        0     2603 2022-01-24 12:35:12.000317 sayn-0.6.8/sayn/logging/task_event_tracker.py
--rw-r--r--   0        0        0        0 2021-03-18 12:17:49.593666 sayn-0.6.8/sayn/scaffolding/__init__.py
--rw-r--r--   0        0        0     2601 2021-03-18 12:17:49.593825 sayn-0.6.8/sayn/scaffolding/data/init_project/.gitignore
--rw-r--r--   0        0        0      937 2022-02-24 13:53:08.374117 sayn-0.6.8/sayn/scaffolding/data/init_project/README.md
--rw-r--r--   0        0        0   131072 2022-02-24 13:53:08.374508 sayn-0.6.8/sayn/scaffolding/data/init_project/dev.db
--rw-r--r--   0        0        0   131072 2022-02-24 13:53:08.374919 sayn-0.6.8/sayn/scaffolding/data/init_project/prod.db
--rw-r--r--   0        0        0      478 2022-02-24 13:53:08.375101 sayn-0.6.8/sayn/scaffolding/data/init_project/project.yaml
--rw-r--r--   0        0        0        0 2021-03-18 12:17:49.593965 sayn-0.6.8/sayn/scaffolding/data/init_project/python/__init__.py
--rw-r--r--   0        0        0     2795 2022-02-24 13:53:08.375285 sayn-0.6.8/sayn/scaffolding/data/init_project/python/load_data.py
--rw-r--r--   0        0        0       81 2022-02-24 13:53:08.375374 sayn-0.6.8/sayn/scaffolding/data/init_project/python/say_hello.py
--rw-r--r--   0        0        0        5 2021-03-18 12:17:49.594200 sayn-0.6.8/sayn/scaffolding/data/init_project/requirements.txt
--rw-r--r--   0        0        0      785 2022-02-24 13:53:08.375533 sayn-0.6.8/sayn/scaffolding/data/init_project/sample_settings.yaml
--rw-r--r--   0        0        0       59 2021-03-18 12:17:49.594375 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/dim_arenas.sql
--rw-r--r--   0        0        0       65 2021-03-18 12:17:49.594440 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/dim_fighters.sql
--rw-r--r--   0        0        0       74 2021-03-18 12:17:49.594499 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/dim_tournaments.sql
--rw-r--r--   0        0        0      650 2022-02-24 13:53:08.375694 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/f_battles.sql
--rw-r--r--   0        0        0      439 2022-02-24 13:53:08.375851 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/f_fighter_results.sql
--rw-r--r--   0        0        0      223 2022-02-24 13:53:08.375981 sayn-0.6.8/sayn/scaffolding/data/init_project/sql/f_rankings.sql
--rw-r--r--   0        0        0      796 2021-03-18 12:17:49.594887 sayn-0.6.8/sayn/scaffolding/init_project.py
--rw-r--r--   0        0        0        0 2022-01-24 12:35:12.000445 sayn-0.6.8/sayn/tasks/__init__.py
--rw-r--r--   0        0        0    15191 2023-04-03 17:04:21.774599 sayn-0.6.8/sayn/tasks/autosql.py
--rw-r--r--   0        0        0     2355 2022-07-19 09:36:59.909572 sayn-0.6.8/sayn/tasks/builder.py
--rw-r--r--   0        0        0    24790 2023-04-03 17:04:21.774746 sayn-0.6.8/sayn/tasks/copy.py
--rw-r--r--   0        0        0      307 2022-01-24 12:35:12.002196 sayn-0.6.8/sayn/tasks/dummy.py
--rw-r--r--   0        0        0     6282 2022-07-19 09:36:59.910282 sayn-0.6.8/sayn/tasks/python.py
--rw-r--r--   0        0        0    17435 2023-04-03 17:04:21.774939 sayn-0.6.8/sayn/tasks/sql.py
--rw-r--r--   0        0        0    11760 2022-07-19 09:36:59.910974 sayn-0.6.8/sayn/tasks/task.py
--rw-r--r--   0        0        0    15766 2023-04-03 17:04:21.775101 sayn-0.6.8/sayn/tasks/task_wrapper.py
--rw-r--r--   0        0        0     4047 2022-07-19 09:36:59.911594 sayn-0.6.8/sayn/tasks/test.py
--rw-r--r--   0        0        0      451 2022-07-19 09:36:59.911782 sayn-0.6.8/sayn/tasks/tests/standard_test_output.sql
--rw-r--r--   0        0        0      450 2022-07-19 09:36:59.911947 sayn-0.6.8/sayn/tasks/tests/standard_test_output_bigquery.sql
--rw-r--r--   0        0        0      504 2022-02-24 13:53:08.377600 sayn-0.6.8/sayn/tasks/tests/standard_tests.sql
--rw-r--r--   0        0        0      483 2022-02-24 13:53:08.377737 sayn-0.6.8/sayn/tasks/tests/standard_tests_bigquery.sql
--rw-r--r--   0        0        0        0 2021-03-18 12:17:49.595609 sayn-0.6.8/sayn/utils/__init__.py
--rw-r--r--   0        0        0     4220 2022-09-20 15:34:39.546883 sayn-0.6.8/sayn/utils/compiler.py
--rw-r--r--   0        0        0     3741 2022-01-24 12:35:12.003823 sayn-0.6.8/sayn/utils/dag.py
--rw-r--r--   0        0        0      971 2022-02-24 13:53:08.377892 sayn-0.6.8/sayn/utils/graphviz.py
--rw-r--r--   0        0        0     2029 2021-03-18 12:17:49.595859 sayn-0.6.8/sayn/utils/misc.py
--rw-r--r--   0        0        0     3083 2022-01-24 12:35:12.004042 sayn-0.6.8/sayn/utils/python_loader.py
--rw-r--r--   0        0        0      418 2021-03-18 12:17:49.596000 sayn-0.6.8/sayn/utils/singleton.py
--rw-r--r--   0        0        0     4187 2022-02-24 13:53:08.378041 sayn-0.6.8/sayn/utils/task_query.py
--rw-r--r--   0        0        0     1419 2022-01-24 12:35:12.004329 sayn-0.6.8/sayn/utils/yaml.py
--rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 sayn-0.6.8/setup.py
--rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 sayn-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     7923 2023-04-05 14:31:17.155361 sayn-0.6.9/CHANGELOG.md
+-rw-r--r--   0        0        0    10089 2021-03-18 12:17:49.585126 sayn-0.6.9/LICENSE.md
+-rw-r--r--   0        0        0      544 2021-03-18 12:17:49.585201 sayn-0.6.9/NOTICE.md
+-rw-r--r--   0        0        0     3254 2022-01-24 12:35:11.985071 sayn-0.6.9/README.md
+-rw-r--r--   0        0        0       67 2021-03-18 12:17:49.585470 sayn-0.6.9/docs/api/database.md
+-rw-r--r--   0        0        0       65 2022-07-19 09:36:59.894884 sayn-0.6.9/docs/api/python_task.md
+-rw-r--r--   0        0        0     3598 2022-02-24 13:53:08.364628 sayn-0.6.9/docs/cli.md
+-rw-r--r--   0        0        0      477 2021-03-18 12:17:49.585773 sayn-0.6.9/docs/css/admonitions.css
+-rw-r--r--   0        0        0      689 2021-03-18 12:17:49.585848 sayn-0.6.9/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0    26013 2021-03-18 12:17:49.586118 sayn-0.6.9/docs/dag.png
+-rw-r--r--   0        0        0    15035 2022-02-24 13:53:08.364916 sayn-0.6.9/docs/database_objects.md
+-rw-r--r--   0        0        0     2725 2023-04-03 17:04:21.766383 sayn-0.6.9/docs/databases/bigquery.md
+-rw-r--r--   0        0        0     1358 2021-03-18 12:17:49.586395 sayn-0.6.9/docs/databases/mysql.md
+-rw-r--r--   0        0        0     2664 2021-04-29 16:40:55.449583 sayn-0.6.9/docs/databases/overview.md
+-rw-r--r--   0        0        0     1372 2021-03-18 12:17:49.586586 sayn-0.6.9/docs/databases/postgresql.md
+-rw-r--r--   0        0        0     6514 2023-04-03 17:04:21.766739 sayn-0.6.9/docs/databases/redshift.md
+-rw-r--r--   0        0        0     1545 2021-03-18 12:17:49.586767 sayn-0.6.9/docs/databases/snowflake.md
+-rw-r--r--   0        0        0      608 2021-03-18 12:17:49.586844 sayn-0.6.9/docs/databases/sqlite.md
+-rw-r--r--   0        0        0      960 2022-01-24 12:35:11.987045 sayn-0.6.9/docs/installation.md
+-rw-r--r--   0        0        0     6180 2021-04-29 16:40:55.449961 sayn-0.6.9/docs/parameters.md
+-rw-r--r--   0        0        0     1609 2021-04-29 16:40:55.450116 sayn-0.6.9/docs/presets.md
+-rw-r--r--   0        0        0    19176 2021-11-23 17:13:41.722989 sayn-0.6.9/docs/project_examples/bbc_news_nlp.md
+-rw-r--r--   0        0        0  1084434 2021-11-23 17:13:41.729704 sayn-0.6.9/docs/project_examples/chart_race.gif
+-rw-r--r--   0        0        0     3195 2021-11-23 17:13:41.730124 sayn-0.6.9/docs/project_examples/facebook_data_project.md
+-rw-r--r--   0        0        0    17605 2021-11-23 17:13:41.730422 sayn-0.6.9/docs/project_examples/reddit_news_nlp.md
+-rw-r--r--   0        0        0     1781 2021-11-23 17:13:41.730657 sayn-0.6.9/docs/project_examples/simple_etl.md
+-rw-r--r--   0        0        0     1235 2021-03-18 12:17:49.587301 sayn-0.6.9/docs/project_structure.md
+-rw-r--r--   0        0        0     1635 2022-01-24 12:35:11.987267 sayn-0.6.9/docs/settings/project_yaml.md
+-rw-r--r--   0        0        0     4950 2022-02-24 13:53:08.366135 sayn-0.6.9/docs/settings/settings_yaml.md
+-rw-r--r--   0        0        0     8177 2022-07-19 09:36:59.895926 sayn-0.6.9/docs/tasks/autosql.md
+-rw-r--r--   0        0        0     7467 2022-02-24 13:53:08.366602 sayn-0.6.9/docs/tasks/copy.md
+-rw-r--r--   0        0        0     1829 2021-04-29 16:40:55.451169 sayn-0.6.9/docs/tasks/dummy.md
+-rw-r--r--   0        0        0     7835 2022-07-19 09:36:59.896330 sayn-0.6.9/docs/tasks/overview.md
+-rw-r--r--   0        0        0    11394 2022-07-19 09:36:59.896724 sayn-0.6.9/docs/tasks/python.md
+-rw-r--r--   0        0        0     9393 2022-11-08 18:05:17.851969 sayn-0.6.9/docs/tasks/sql.md
+-rw-r--r--   0        0        0     1639 2022-08-04 14:21:08.499774 sayn-0.6.9/docs/tests/custom.md
+-rw-r--r--   0        0        0     4121 2022-08-04 14:21:08.500832 sayn-0.6.9/docs/tests/overview.md
+-rw-r--r--   0        0        0     1832 2022-02-24 13:53:08.367627 sayn-0.6.9/docs/tests/standard.md
+-rw-r--r--   0        0        0   325125 2021-03-18 12:17:49.589475 sayn-0.6.9/docs/tutorials/sayn_run1.gif
+-rw-r--r--   0        0        0     4520 2022-03-16 14:32:08.023722 sayn-0.6.9/docs/tutorials/tutorial_part1.md
+-rw-r--r--   0        0        0     5243 2022-03-16 14:32:08.024011 sayn-0.6.9/docs/tutorials/tutorial_part2.md
+-rw-r--r--   0        0        0     8014 2022-03-16 14:32:08.024289 sayn-0.6.9/docs/tutorials/tutorial_part3.md
+-rw-r--r--   0        0        0     2326 2022-07-19 09:36:59.902566 sayn-0.6.9/mkdocs.yml
+-rw-r--r--   0        0        0     2350 2023-04-05 14:31:17.156511 sayn-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-04-05 14:31:17.157544 sayn-0.6.9/sayn/__init__.py
+-rw-r--r--   0        0        0     7728 2022-02-24 13:53:08.370450 sayn-0.6.9/sayn/cli.py
+-rw-r--r--   0        0        0        0 2021-03-18 12:17:49.591152 sayn-0.6.9/sayn/core/__init__.py
+-rw-r--r--   0        0        0    23306 2023-04-03 17:04:21.769079 sayn-0.6.9/sayn/core/app.py
+-rw-r--r--   0        0        0     5342 2022-01-24 12:35:11.993153 sayn-0.6.9/sayn/core/errors.py
+-rw-r--r--   0        0        0    15854 2023-04-03 17:04:21.769669 sayn-0.6.9/sayn/core/project.py
+-rw-r--r--   0        0        0    11733 2023-04-03 17:04:21.769868 sayn-0.6.9/sayn/core/settings.py
+-rw-r--r--   0        0        0    28264 2023-04-05 14:31:17.158562 sayn-0.6.9/sayn/database/__init__.py
+-rw-r--r--   0        0        0    11580 2023-04-05 14:31:17.159035 sayn-0.6.9/sayn/database/bigquery.py
+-rw-r--r--   0        0        0     1065 2022-02-24 13:53:08.372369 sayn-0.6.9/sayn/database/creator.py
+-rw-r--r--   0        0        0     2101 2023-04-03 17:04:21.771342 sayn-0.6.9/sayn/database/mysql.py
+-rw-r--r--   0        0        0     8802 2023-04-03 17:04:21.771461 sayn-0.6.9/sayn/database/objects.py
+-rw-r--r--   0        0        0     1505 2023-04-03 17:04:21.771820 sayn-0.6.9/sayn/database/postgresql.py
+-rw-r--r--   0        0        0     9013 2023-04-05 14:31:17.159492 sayn-0.6.9/sayn/database/redshift.py
+-rw-r--r--   0        0        0     2507 2023-04-03 17:04:21.772736 sayn-0.6.9/sayn/database/snowflake.py
+-rw-r--r--   0        0        0     3557 2023-04-03 17:04:21.772868 sayn-0.6.9/sayn/database/sqlite.py
+-rw-r--r--   0        0        0     2181 2023-04-03 17:04:21.773646 sayn-0.6.9/sayn/database/templates/create_table.sql
+-rw-r--r--   0        0        0      614 2023-04-03 17:04:21.774019 sayn-0.6.9/sayn/database/templates/create_view.sql
+-rw-r--r--   0        0        0      349 2021-11-23 17:13:41.734017 sayn-0.6.9/sayn/database/templates/merge_tables.sql
+-rw-r--r--   0        0        0     1366 2023-04-03 17:04:21.774115 sayn-0.6.9/sayn/database/templates/move_table.sql
+-rw-r--r--   0        0        0      188 2023-04-05 14:31:17.159703 sayn-0.6.9/sayn/database/templates/redshift_load_batch.sql
+-rw-r--r--   0        0        0      364 2023-04-03 17:04:21.774239 sayn-0.6.9/sayn/database/templates/redshift_merge_tables.sql
+-rw-r--r--   0        0        0      664 2022-07-19 09:36:59.908339 sayn-0.6.9/sayn/database/templates/snowflake_load_batch.sql
+-rw-r--r--   0        0        0      171 2022-02-24 13:53:08.373158 sayn-0.6.9/sayn/database/unknown.py
+-rw-r--r--   0        0        0      156 2021-03-18 12:17:49.592845 sayn-0.6.9/sayn/logging/__init__.py
+-rw-r--r--   0        0        0      714 2021-03-18 12:17:49.592944 sayn-0.6.9/sayn/logging/console_logger.py
+-rw-r--r--   0        0        0     2903 2022-01-24 12:35:11.999438 sayn-0.6.9/sayn/logging/event_tracker.py
+-rw-r--r--   0        0        0     6206 2022-02-24 13:53:08.373327 sayn-0.6.9/sayn/logging/fancy_logger.py
+-rw-r--r--   0        0        0     1484 2022-02-24 13:53:08.373462 sayn-0.6.9/sayn/logging/file_logger.py
+-rw-r--r--   0        0        0    20346 2023-04-03 17:04:21.774399 sayn-0.6.9/sayn/logging/log_formatter.py
+-rw-r--r--   0        0        0     4039 2022-01-24 12:35:12.000136 sayn-0.6.9/sayn/logging/logger.py
+-rw-r--r--   0        0        0     2603 2022-01-24 12:35:12.000317 sayn-0.6.9/sayn/logging/task_event_tracker.py
+-rw-r--r--   0        0        0        0 2021-03-18 12:17:49.593666 sayn-0.6.9/sayn/scaffolding/__init__.py
+-rw-r--r--   0        0        0     2601 2021-03-18 12:17:49.593825 sayn-0.6.9/sayn/scaffolding/data/init_project/.gitignore
+-rw-r--r--   0        0        0      937 2022-02-24 13:53:08.374117 sayn-0.6.9/sayn/scaffolding/data/init_project/README.md
+-rw-r--r--   0        0        0   131072 2022-02-24 13:53:08.374508 sayn-0.6.9/sayn/scaffolding/data/init_project/dev.db
+-rw-r--r--   0        0        0   131072 2022-02-24 13:53:08.374919 sayn-0.6.9/sayn/scaffolding/data/init_project/prod.db
+-rw-r--r--   0        0        0      478 2022-02-24 13:53:08.375101 sayn-0.6.9/sayn/scaffolding/data/init_project/project.yaml
+-rw-r--r--   0        0        0        0 2021-03-18 12:17:49.593965 sayn-0.6.9/sayn/scaffolding/data/init_project/python/__init__.py
+-rw-r--r--   0        0        0     2795 2022-02-24 13:53:08.375285 sayn-0.6.9/sayn/scaffolding/data/init_project/python/load_data.py
+-rw-r--r--   0        0        0       81 2022-02-24 13:53:08.375374 sayn-0.6.9/sayn/scaffolding/data/init_project/python/say_hello.py
+-rw-r--r--   0        0        0        5 2021-03-18 12:17:49.594200 sayn-0.6.9/sayn/scaffolding/data/init_project/requirements.txt
+-rw-r--r--   0        0        0      785 2022-02-24 13:53:08.375533 sayn-0.6.9/sayn/scaffolding/data/init_project/sample_settings.yaml
+-rw-r--r--   0        0        0       59 2021-03-18 12:17:49.594375 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/dim_arenas.sql
+-rw-r--r--   0        0        0       65 2021-03-18 12:17:49.594440 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/dim_fighters.sql
+-rw-r--r--   0        0        0       74 2021-03-18 12:17:49.594499 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/dim_tournaments.sql
+-rw-r--r--   0        0        0      650 2022-02-24 13:53:08.375694 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/f_battles.sql
+-rw-r--r--   0        0        0      439 2022-02-24 13:53:08.375851 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/f_fighter_results.sql
+-rw-r--r--   0        0        0      223 2022-02-24 13:53:08.375981 sayn-0.6.9/sayn/scaffolding/data/init_project/sql/f_rankings.sql
+-rw-r--r--   0        0        0      796 2021-03-18 12:17:49.594887 sayn-0.6.9/sayn/scaffolding/init_project.py
+-rw-r--r--   0        0        0        0 2022-01-24 12:35:12.000445 sayn-0.6.9/sayn/tasks/__init__.py
+-rw-r--r--   0        0        0    15191 2023-04-03 17:04:21.774599 sayn-0.6.9/sayn/tasks/autosql.py
+-rw-r--r--   0        0        0     2355 2022-07-19 09:36:59.909572 sayn-0.6.9/sayn/tasks/builder.py
+-rw-r--r--   0        0        0    24790 2023-04-03 17:04:21.774746 sayn-0.6.9/sayn/tasks/copy.py
+-rw-r--r--   0        0        0      307 2022-01-24 12:35:12.002196 sayn-0.6.9/sayn/tasks/dummy.py
+-rw-r--r--   0        0        0     6282 2022-07-19 09:36:59.910282 sayn-0.6.9/sayn/tasks/python.py
+-rw-r--r--   0        0        0    17435 2023-04-03 17:04:21.774939 sayn-0.6.9/sayn/tasks/sql.py
+-rw-r--r--   0        0        0    11760 2022-07-19 09:36:59.910974 sayn-0.6.9/sayn/tasks/task.py
+-rw-r--r--   0        0        0    15766 2023-04-03 17:04:21.775101 sayn-0.6.9/sayn/tasks/task_wrapper.py
+-rw-r--r--   0        0        0     4047 2022-07-19 09:36:59.911594 sayn-0.6.9/sayn/tasks/test.py
+-rw-r--r--   0        0        0      451 2022-07-19 09:36:59.911782 sayn-0.6.9/sayn/tasks/tests/standard_test_output.sql
+-rw-r--r--   0        0        0      450 2022-07-19 09:36:59.911947 sayn-0.6.9/sayn/tasks/tests/standard_test_output_bigquery.sql
+-rw-r--r--   0        0        0      504 2022-02-24 13:53:08.377600 sayn-0.6.9/sayn/tasks/tests/standard_tests.sql
+-rw-r--r--   0        0        0      483 2022-02-24 13:53:08.377737 sayn-0.6.9/sayn/tasks/tests/standard_tests_bigquery.sql
+-rw-r--r--   0        0        0        0 2021-03-18 12:17:49.595609 sayn-0.6.9/sayn/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2022-09-20 15:34:39.546883 sayn-0.6.9/sayn/utils/compiler.py
+-rw-r--r--   0        0        0     3741 2022-01-24 12:35:12.003823 sayn-0.6.9/sayn/utils/dag.py
+-rw-r--r--   0        0        0      971 2022-02-24 13:53:08.377892 sayn-0.6.9/sayn/utils/graphviz.py
+-rw-r--r--   0        0        0     2029 2021-03-18 12:17:49.595859 sayn-0.6.9/sayn/utils/misc.py
+-rw-r--r--   0        0        0     3083 2022-01-24 12:35:12.004042 sayn-0.6.9/sayn/utils/python_loader.py
+-rw-r--r--   0        0        0      418 2021-03-18 12:17:49.596000 sayn-0.6.9/sayn/utils/singleton.py
+-rw-r--r--   0        0        0     4187 2022-02-24 13:53:08.378041 sayn-0.6.9/sayn/utils/task_query.py
+-rw-r--r--   0        0        0     1419 2022-01-24 12:35:12.004329 sayn-0.6.9/sayn/utils/yaml.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 sayn-0.6.9/setup.py
+-rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 sayn-0.6.9/PKG-INFO
```

### Comparing `sayn-0.6.8/CHANGELOG.md` & `sayn-0.6.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Change Log
 
+## [0.6.9] - 2023-04-05
+
+### Fixed
+
+- Colon (:) in SQL is not interpreted as bind parameters
+- Update Redshift dependencies
+- Fixes to Redshift load_data when using an S3 bucket
+
 ## [0.6.8] - 2023-04-03
 
 ### Changed
 
 - Add support for 3rd level (eg: projects in BigQuery or databases in Snowflake)
   when referencing database objects with `src` and `out`
 - Add support for python 3.11
```

### Comparing `sayn-0.6.8/LICENSE.md` & `sayn-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/NOTICE.md` & `sayn-0.6.9/NOTICE.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/README.md` & `sayn-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/cli.md` & `sayn-0.6.9/docs/cli.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/css/mkdocstrings.css` & `sayn-0.6.9/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/dag.png` & `sayn-0.6.9/docs/dag.png`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/database_objects.md` & `sayn-0.6.9/docs/database_objects.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/bigquery.md` & `sayn-0.6.9/docs/databases/bigquery.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/mysql.md` & `sayn-0.6.9/docs/databases/mysql.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/overview.md` & `sayn-0.6.9/docs/databases/overview.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/postgresql.md` & `sayn-0.6.9/docs/databases/postgresql.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/redshift.md` & `sayn-0.6.9/docs/databases/redshift.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/snowflake.md` & `sayn-0.6.9/docs/databases/snowflake.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/databases/sqlite.md` & `sayn-0.6.9/docs/databases/sqlite.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/installation.md` & `sayn-0.6.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/parameters.md` & `sayn-0.6.9/docs/parameters.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/presets.md` & `sayn-0.6.9/docs/presets.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_examples/bbc_news_nlp.md` & `sayn-0.6.9/docs/project_examples/bbc_news_nlp.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_examples/chart_race.gif` & `sayn-0.6.9/docs/project_examples/chart_race.gif`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_examples/facebook_data_project.md` & `sayn-0.6.9/docs/project_examples/facebook_data_project.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_examples/reddit_news_nlp.md` & `sayn-0.6.9/docs/project_examples/reddit_news_nlp.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_examples/simple_etl.md` & `sayn-0.6.9/docs/project_examples/simple_etl.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/project_structure.md` & `sayn-0.6.9/docs/project_structure.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/settings/project_yaml.md` & `sayn-0.6.9/docs/settings/project_yaml.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/settings/settings_yaml.md` & `sayn-0.6.9/docs/settings/settings_yaml.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/autosql.md` & `sayn-0.6.9/docs/tasks/autosql.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/copy.md` & `sayn-0.6.9/docs/tasks/copy.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/dummy.md` & `sayn-0.6.9/docs/tasks/dummy.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/overview.md` & `sayn-0.6.9/docs/tasks/overview.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/python.md` & `sayn-0.6.9/docs/tasks/python.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tasks/sql.md` & `sayn-0.6.9/docs/tasks/sql.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tests/custom.md` & `sayn-0.6.9/docs/tests/custom.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tests/overview.md` & `sayn-0.6.9/docs/tests/overview.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tests/standard.md` & `sayn-0.6.9/docs/tests/standard.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tutorials/sayn_run1.gif` & `sayn-0.6.9/docs/tutorials/sayn_run1.gif`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tutorials/tutorial_part1.md` & `sayn-0.6.9/docs/tutorials/tutorial_part1.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tutorials/tutorial_part2.md` & `sayn-0.6.9/docs/tutorials/tutorial_part2.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/docs/tutorials/tutorial_part3.md` & `sayn-0.6.9/docs/tutorials/tutorial_part3.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/mkdocs.yml` & `sayn-0.6.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/pyproject.toml` & `sayn-0.6.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sayn"
-version = "0.6.8"
+version = "0.6.9"
 description = "Data-modelling and processing framework for automating Python and SQL tasks"
 authors = ["Robin Watteaux <robin@173tech.com>", "Adrian Macias <adrian@173tech.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/173TECH/sayn"
 homepage = "https://173tech.github.io/sayn"
@@ -30,14 +30,15 @@
 
 halo = "0.0.31"
 colorama = ">=0.4.4"
 
 # DB drivers (optional)
 # Postgresql
 psycopg2 = { version = ">=2.9.3", optional = true }
+psycopg2-binary = { version = ">=2.9.3", optional = true }
 
 # MySQL
 PyMySQL = { version = ">=1.0.2", optional = true }
 
 # Snowflake
 snowflake-sqlalchemy = { version = ">=1.4.4", optional = true }
 
@@ -45,23 +46,24 @@
 # BigQuery doesn't work with 3.11 at the moment: https://github.com/googleapis/python-bigquery-sqlalchemy/issues/500
 sqlalchemy-bigquery = { version = ">=1.6.0", python = ">=3.8.1,<3.12", optional = true }
 
 # BigQuery dependencies for the storage client
 google-cloud-bigquery-storage = { version = ">=2.0.0,<3.0.0dev", optional = true }
 
 # Redshift
-redshift-connector = "^2.0.910"
-sqlalchemy-redshift = "^0.8.12"
+redshift-connector = { version = ">=2.0.909", optional = true }
+sqlalchemy-redshift = { version = ">=0.8.12", optional = true }
 
 # DAG visualisation
 graphviz = { version = ">=0.19.1", optional = true }
 
 [tool.poetry.extras]
 all = ["graphviz", "psycopg2", "pymysql", "snowflake-sqlalchemy", "sqlalchemy-bigquery", "graphviz"]
 postgresql = ["psycopg2"]
+postgresql-binary = ["psycopg2-binary"]
 redshift = ["redshift-connector", "sqlalchemy-redshift"]
 mysql = ["pymysql"]
 snowflake = ["snowflake-sqlalchemy"]
 bigquery = ["sqlalchemy-bigquery", "google-cloud-bigquery-storage"]
 graphviz = ["graphviz"]
 
 [tool.poetry.scripts]
@@ -74,12 +76,12 @@
 flake8 = "^6.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.11"
 mkdocstrings = "^0.19.1"
 livereload = "^2.6.3"
 
 [build-system]
-requires = ["poetry>=1.3.1"]
+requires = ["poetry>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests" ]
```

### Comparing `sayn-0.6.8/sayn/cli.py` & `sayn-0.6.9/sayn/cli.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/core/app.py` & `sayn-0.6.9/sayn/core/app.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/core/errors.py` & `sayn-0.6.9/sayn/core/errors.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/core/project.py` & `sayn-0.6.9/sayn/core/project.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/core/settings.py` & `sayn-0.6.9/sayn/core/settings.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/__init__.py` & `sayn-0.6.9/sayn/database/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from itertools import groupby
 from pathlib import Path
 from typing import List, Optional, Union
 
 from jinja2 import Environment, FileSystemLoader, StrictUndefined
 from pydantic import BaseModel, validator, Extra
 from sqlalchemy import MetaData, Table
-from sqlalchemy.sql import sqltypes
-from sqlalchemy import text
+from sqlalchemy.sql import sqltypes, text
 
 from ..core.errors import DBError, Exc, Ok
 
 
 class Hook(BaseModel):
     sql: str
 
@@ -442,15 +441,15 @@
     def execute(self, script):
         """Executes a script in the database. Multiple statements are supported.
 
         Args:
             script (sql): The SQL script to execute
         """
         with self.engine.connect().execution_options(autocommit=True) as connection:
-            connection.execute(text(script))
+            connection.execute(text(script.replace(":", "\\:")))
 
     def read_data(self, query, **params):
         """Executes the query and returns a list of dictionaries with the data.
 
         Args:
             query (str): The SELECT query to execute
             params (dict): sqlalchemy parameters to use when building the final query as per
```

### Comparing `sayn-0.6.8/sayn/database/bigquery.py` & `sayn-0.6.9/sayn/database/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,19 @@
         dst_schema=None,
         src_db=None,
         dst_db=None,
         **ddl,
     ):
         # ddl = self._format_properties(ddl).value
 
-        full_src_table = f"{src_db + '.' if src_schema is not None else ''}{src_schema + '.' if src_schema is not None else ''}{src_table}"
+        full_src_table = (
+            f"{src_db + '.' if src_db is not None else ''}"
+            f"{src_schema + '.' if src_schema is not None else ''}"
+            f"{src_table}"
+        )
         select = f"SELECT * FROM {full_src_table}"
         create_or_replace = self.create_table(
             dst_table, dst_schema, dst_db, select=select, replace=True, **ddl
         )
 
         return "\n\n".join((create_or_replace, f"DROP TABLE {full_src_table}"))
```

### Comparing `sayn-0.6.8/sayn/database/creator.py` & `sayn-0.6.9/sayn/database/creator.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/mysql.py` & `sayn-0.6.9/sayn/database/mysql.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/objects.py` & `sayn-0.6.9/sayn/database/objects.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/postgresql.py` & `sayn-0.6.9/sayn/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/redshift.py` & `sayn-0.6.9/sayn/database/redshift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections import Counter
 import csv
+from io import BytesIO
+import gzip
 from pathlib import Path
-import tempfile
 from typing import List, Optional, Union
 
+import orjson
 from pydantic import BaseModel, constr, validator, Extra
 from sqlalchemy import create_engine
 
 from ..core.errors import DBError
 from . import Database, Columns, Hook, BaseDDL
 
 
@@ -216,38 +218,33 @@
         """
         # if no bucket is supplied, the old _load_data_batch function is used
         if self.bucket is None:
             return super(Database, self)._load_data_batch(table, data, schema, db)
 
         full_table_name = f"{'' if db is None else db + '.'}{'' if schema is None else schema + '.'}{table}"
         template = self._jinja_env.get_template("redshift_load_batch.sql")
-        fname = "batch.csv"
 
-        s3_client = self._boto_session.client("s3")
+        s3_client = self._boto_session.client("s3", region_name=self.bucket["region"])
 
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            with (Path(tmpdirname) / fname).open("w") as f:
-                writer = csv.DictWriter(
-                    f, fieldnames=data[0].keys(), delimiter="|", escapechar="\\"
-                )
-
-                writer.writerows(data)
-
-            with (Path(tmpdirname) / fname).open("rb") as f:
-                s3_client.upload_fileobj(f, self.bucket, fname)
-
-            self.execute(
-                template.render(
-                    full_table_name=full_table_name,
-                    temp_file_directory=tmpdirname,
-                    temp_file_name=fname,
-                    bucket=self.bucket,
-                    region=self.bucket_region,
-                )
+        buf = BytesIO()
+        with gzip.GzipFile(fileobj=buf, mode="w") as gf:
+            gf.write(b"\n".join([orjson.dumps(r, default=str) for r in data]))
+
+        buf.seek(0)
+        fname = "batch.json.gz"
+        s3_client.upload_fileobj(buf, self.bucket["name"], fname)
+
+        self.execute(
+            template.render(
+                full_table_name=full_table_name,
+                temp_file_name=fname,
+                bucket=self.bucket["name"],
+                region=self.bucket["region"],
             )
+        )
 
     def merge_tables(
         self,
         src_table,
         dst_table,
         delete_key,
         cleanup=True,
```

### Comparing `sayn-0.6.8/sayn/database/snowflake.py` & `sayn-0.6.9/sayn/database/snowflake.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/sqlite.py` & `sayn-0.6.9/sayn/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/templates/create_table.sql` & `sayn-0.6.9/sayn/database/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/templates/create_view.sql` & `sayn-0.6.9/sayn/database/templates/create_view.sql`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/templates/move_table.sql` & `sayn-0.6.9/sayn/database/templates/move_table.sql`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/database/templates/snowflake_load_batch.sql` & `sayn-0.6.9/sayn/database/templates/snowflake_load_batch.sql`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/console_logger.py` & `sayn-0.6.9/sayn/logging/console_logger.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/event_tracker.py` & `sayn-0.6.9/sayn/logging/event_tracker.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/fancy_logger.py` & `sayn-0.6.9/sayn/logging/fancy_logger.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/file_logger.py` & `sayn-0.6.9/sayn/logging/file_logger.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/log_formatter.py` & `sayn-0.6.9/sayn/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/logger.py` & `sayn-0.6.9/sayn/logging/logger.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/logging/task_event_tracker.py` & `sayn-0.6.9/sayn/logging/task_event_tracker.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/.gitignore` & `sayn-0.6.9/sayn/scaffolding/data/init_project/.gitignore`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/README.md` & `sayn-0.6.9/sayn/scaffolding/data/init_project/README.md`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/dev.db` & `sayn-0.6.9/sayn/scaffolding/data/init_project/dev.db`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/prod.db` & `sayn-0.6.9/sayn/scaffolding/data/init_project/prod.db`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/python/load_data.py` & `sayn-0.6.9/sayn/scaffolding/data/init_project/python/load_data.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/sample_settings.yaml` & `sayn-0.6.9/sayn/scaffolding/data/init_project/sample_settings.yaml`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/data/init_project/sql/f_battles.sql` & `sayn-0.6.9/sayn/scaffolding/data/init_project/sql/f_battles.sql`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/scaffolding/init_project.py` & `sayn-0.6.9/sayn/scaffolding/init_project.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/autosql.py` & `sayn-0.6.9/sayn/tasks/autosql.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/builder.py` & `sayn-0.6.9/sayn/tasks/builder.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/copy.py` & `sayn-0.6.9/sayn/tasks/copy.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/python.py` & `sayn-0.6.9/sayn/tasks/python.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/sql.py` & `sayn-0.6.9/sayn/tasks/sql.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/task.py` & `sayn-0.6.9/sayn/tasks/task.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/task_wrapper.py` & `sayn-0.6.9/sayn/tasks/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/tasks/test.py` & `sayn-0.6.9/sayn/tasks/test.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/compiler.py` & `sayn-0.6.9/sayn/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/dag.py` & `sayn-0.6.9/sayn/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/graphviz.py` & `sayn-0.6.9/sayn/utils/graphviz.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/misc.py` & `sayn-0.6.9/sayn/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/python_loader.py` & `sayn-0.6.9/sayn/utils/python_loader.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/task_query.py` & `sayn-0.6.9/sayn/utils/task_query.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/sayn/utils/yaml.py` & `sayn-0.6.9/sayn/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sayn-0.6.8/setup.py` & `sayn-0.6.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,35 @@
  'halo==0.0.31',
  'orjson>=3.7.7',
  'pydantic>=1.9.0,<1.10.0',
  'ruamel.yaml.clib==0.2.7',
  'ruamel.yaml==0.17.21']
 
 extras_require = \
-{':extra == "redshift"': ['redshift-connector>=2.0.910,<3.0.0',
-                          'sqlalchemy-redshift>=0.8.12,<0.9.0'],
- 'all': ['psycopg2>=2.9.3',
+{'all': ['psycopg2>=2.9.3',
          'PyMySQL>=1.0.2',
          'snowflake-sqlalchemy>=1.4.4',
          'graphviz>=0.19.1',
          'graphviz>=0.19.1'],
  'all:python_full_version >= "3.8.1" and python_version < "3.12"': ['sqlalchemy-bigquery>=1.6.0'],
  'bigquery': ['google-cloud-bigquery-storage>=2.0.0,<3.0.0dev'],
  'bigquery:python_full_version >= "3.8.1" and python_version < "3.12"': ['sqlalchemy-bigquery>=1.6.0'],
  'graphviz': ['graphviz>=0.19.1'],
  'mysql': ['PyMySQL>=1.0.2'],
  'postgresql': ['psycopg2>=2.9.3'],
+ 'postgresql-binary': ['psycopg2-binary>=2.9.3'],
+ 'redshift': ['redshift-connector>=2.0.909', 'sqlalchemy-redshift>=0.8.12'],
  'snowflake': ['snowflake-sqlalchemy>=1.4.4']}
 
 entry_points = \
 {'console_scripts': ['sayn = sayn.cli:cli']}
 
 setup_kwargs = {
     'name': 'sayn',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': 'Data-modelling and processing framework for automating Python and SQL tasks',
     'long_description': '<img\n  src="https://173-static-files.s3.eu-west-2.amazonaws.com/sayn_docs/logos/sayn_logo.png"\n  alt="SAYN logo"\n  style="width: 50%; height: 50%;"\n/>\n\n#\n\nSAYN is a modern data processing and modelling framework. Users define tasks (incl. Python, automated SQL transformations and more) and their relationships, SAYN takes care of the rest. It is designed for simplicity, flexibility and centralisation in order to bring significant efficiency gains to the data engineering workflow.\n\n## Use Cases\n\nSAYN can be used for multiple purposes across the data engineering and analytics workflows:\n\n* Data extraction: complement tools such as Fivetran or Stitch with customised extraction processes.\n* Data modelling: transform raw data in your data warehouse (e.g. aggregate activity or sessions, calculate marketing campaign ROI, etc.).\n* Data science: integrate and execute data science models.\n\n## Key Features\n\nSAYN has the following key features:\n\n* YAML based DAG (Direct Acyclic Graph) creation. This means all analysts, including non Python proficient ones, can easily add tasks to ETL processes with SAYN.\n* [Automated SQL transformations](https://173tech.github.io/sayn/tasks/autosql/): write your SELECT statement. SAYN turns it into a table/view and manages everything for you.\n* [Jinja parameters](https://173tech.github.io/sayn/parameters/): switch easily between development and product environment and other tricks with Jinja templating.\n* [Python tasks](https://173tech.github.io/sayn/tasks/python/): use Python scripts to complement your extraction and loading layer and build data science models.\n* Multiple [databases](https://173tech.github.io/sayn/databases/overview/) supported.\n* and much more... See the [Documentation](https://173tech.github.io/sayn/).\n\n## Design Principles\n\nSAYN aims to empower data engineers and analysts through its  three core design principles:\n\n* **Simplicity**: data processes should be easy to create, scale and maintain. So your team can focus on data transformation instead of writing processes. SAYN orchestrates all your tasks systematically and provides a lot of automation features.\n* **Flexibility**: the power of data is unlimited and so should your tooling. SAYN supports both SQL and Python so your analysts can choose the most optimal solution for each process.\n* **Centralisation**: all analytics code should live in one place, making your life easier and allowing dependencies throughout the whole analytics process.\n\n## Quick Start\n\nSAYN supports Python 3.7 to 3.10.\n\n```bash\n$ pip install sayn\n$ sayn init test_sayn\n$ cd test_sayn\n$ sayn run\n```\n\nThis is it! You completed your first SAYN run on the example project. Continue with the [Tutorial: Part 1](https://173tech.github.io/sayn/tutorials/tutorial_part1/) which will give you a good overview of SAYN\'s true power!\n\n## Release Updates\n\nIf you want to receive update emails about SAYN releases, you can sign up [here](http://eepurl.com/hnfJIr).\n\n## Support\n\nIf you need any help with SAYN, or simply want to know more, please contact the team at <sayn@173tech.com>.\n\n## License\n\nSAYN is open source under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license.\n\n---\n\nMade with :heart: by [173tech](https://www.173tech.com).\n',
     'author': 'Robin Watteaux',
     'author_email': 'robin@173tech.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://173tech.github.io/sayn',
```

### Comparing `sayn-0.6.8/PKG-INFO` & `sayn-0.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayn
-Version: 0.6.8
+Version: 0.6.9
 Summary: Data-modelling and processing framework for automating Python and SQL tasks
 Home-page: https://173tech.github.io/sayn
 License: Apache-2.0
 Author: Robin Watteaux
 Author-email: robin@173tech.com
 Requires-Python: >=3.8.1,<=4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,33 +13,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: bigquery
 Provides-Extra: graphviz
 Provides-Extra: mysql
 Provides-Extra: postgresql
+Provides-Extra: postgresql-binary
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Requires-Dist: Click (==8.0.4)
 Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: PyMySQL (>=1.0.2) ; extra == "all" or extra == "mysql"
 Requires-Dist: SQLAlchemy (>=1.4.25,<2.0.0)
 Requires-Dist: colorama (>=0.4.4)
 Requires-Dist: google-cloud-bigquery-storage (>=2.0.0,<3.0.0dev) ; extra == "bigquery"
 Requires-Dist: graphviz (>=0.19.1) ; extra == "all" or extra == "all" or extra == "graphviz"
 Requires-Dist: halo (==0.0.31)
 Requires-Dist: orjson (>=3.7.7)
 Requires-Dist: psycopg2 (>=2.9.3) ; extra == "all" or extra == "postgresql"
+Requires-Dist: psycopg2-binary (>=2.9.3) ; extra == "postgresql-binary"
 Requires-Dist: pydantic (>=1.9.0,<1.10.0)
-Requires-Dist: redshift-connector (>=2.0.910,<3.0.0) ; extra == "redshift"
+Requires-Dist: redshift-connector (>=2.0.909) ; extra == "redshift"
 Requires-Dist: ruamel.yaml (==0.17.21)
 Requires-Dist: ruamel.yaml.clib (==0.2.7)
 Requires-Dist: snowflake-sqlalchemy (>=1.4.4) ; extra == "all" or extra == "snowflake"
 Requires-Dist: sqlalchemy-bigquery (>=1.6.0) ; (python_full_version >= "3.8.1" and python_version < "3.12") and (extra == "all" or extra == "bigquery")
-Requires-Dist: sqlalchemy-redshift (>=0.8.12,<0.9.0) ; extra == "redshift"
+Requires-Dist: sqlalchemy-redshift (>=0.8.12) ; extra == "redshift"
 Project-URL: Repository, https://github.com/173TECH/sayn
 Description-Content-Type: text/markdown
 
 <img
   src="https://173-static-files.s3.eu-west-2.amazonaws.com/sayn_docs/logos/sayn_logo.png"
   alt="SAYN logo"
   style="width: 50%; height: 50%;"
```

