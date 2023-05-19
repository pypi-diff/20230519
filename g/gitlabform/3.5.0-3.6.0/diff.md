# Comparing `tmp/gitlabform-3.5.0.tar.gz` & `tmp/gitlabform-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.5.0.tar", last modified: Fri Mar 17 21:58:39 2023, max compression
+gzip compressed data, was "gitlabform-3.6.0.tar", last modified: Fri May 19 08:44:55 2023, max compression
```

## Comparing `gitlabform-3.5.0.tar` & `gitlabform-3.6.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.932217 gitlabform-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-17 21:58:36.000000 gitlabform-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-17 21:58:39.932217 gitlabform-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-17 21:58:36.000000 gitlabform-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.924217 gitlabform-3.5.0/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.924217 gitlabform-3.5.0/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.924217 gitlabform-3.5.0/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-17 21:58:36.000000 gitlabform-3.5.0/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.924217 gitlabform-3.5.0/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-17 21:58:39.000000 gitlabform-3.5.0/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-17 21:58:39.932217 gitlabform-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-17 21:58:36.000000 gitlabform-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.928217 gitlabform-3.5.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.932217 gitlabform-3.5.0/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2859 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6034 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3334 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8325 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1476 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11049 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1909 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2947 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4202 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8153 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5784 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10968 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2428 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7723 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5396 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_token_from_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5642 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.932217 gitlabform-3.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.932217 gitlabform-3.5.0/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:39.932217 gitlabform-3.5.0/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-17 21:58:36.000000 gitlabform-3.5.0/tests/unit/test_non_empty_configs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 08:44:49.000000 gitlabform-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-19 08:44:55.935792 gitlabform-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-19 08:44:49.000000 gitlabform-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 08:44:55.935792 gitlabform-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 08:44:49.000000 gitlabform-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8047 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4136 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9639 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10353 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7264 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5045 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_token_from_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5559 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/test_non_empty_configs_provider.py
```

### Comparing `gitlabform-3.5.0/LICENSE` & `gitlabform-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/PKG-INFO` & `gitlabform-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.5.0
+Version: 3.6.0
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.5.0 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.6.0 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.5.0/README.md` & `gitlabform-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/__init__.py` & `gitlabform-3.6.0/gitlabform/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/configuration/common.py` & `gitlabform-3.6.0/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/configuration/core.py` & `gitlabform-3.6.0/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/configuration/groups.py` & `gitlabform-3.6.0/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/configuration/projects.py` & `gitlabform-3.6.0/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/configuration/transform.py` & `gitlabform-3.6.0/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/__init__.py` & `gitlabform-3.6.0/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/commits.py` & `gitlabform-3.6.0/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/core.py` & `gitlabform-3.6.0/gitlabform/gitlab/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,14 @@
 
     @functools.lru_cache()
     def _get_project_id(self, project_and_group):
         # This is a NEW workaround for https://github.com/gitlabhq/gitlabhq/issues/8290
         result = self.get_project(project_and_group)
         return str(result["id"])
 
-    def has_no_license(self):
-        license = self._make_requests_to_api("license")
-        return not license or license["expired"]
-
     def _make_requests_to_api(
         self,
         path_as_format_string,
         args=None,
         method="GET",
         data=None,
         expected_codes=200,
```

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/group_badges.py` & `gitlabform-3.6.0/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.6.0/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/group_variables.py` & `gitlabform-3.6.0/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/groups.py` & `gitlabform-3.6.0/gitlabform/gitlab/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,19 +132,14 @@
         #     'setting2': value2,
         # }
         # ..as documented at: https://docs.gitlab.com/ee/api/groups.html#update-group
         self._make_requests_to_api(
             "groups/%s", project_and_group_name, "PUT", group_settings
         )
 
-    def get_group_shared_with(self, group):
-        group = self.get_group_case_insensitive(group)
-
-        return group["shared_with_groups"]
-
     def add_share_to_group(
         self, group, share_with_group_name, group_access, expires_at=None
     ):
         share_with_group_id = self.get_group_id_case_insensitive(share_with_group_name)
         data = {"group_id": share_with_group_id, "expires_at": expires_at}
         if group_access is not None:
             data["group_access"] = group_access
```

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/integrations.py` & `gitlabform-3.6.0/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/members.py` & `gitlabform-3.6.0/gitlabform/gitlab/members.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,14 @@
     def get_project_members(self, project_and_group_name, all=False):
         url_template = "projects/%s/members"
         if all:
             url_template += "/all"
 
         return self._make_requests_to_api(url_template, project_and_group_name)
 
-    def get_shared_with_groups(self, project_and_group_name):
-        # a dict with groups that this project has been shared with
-        return self._make_requests_to_api("projects/%s", project_and_group_name)[
-            "shared_with_groups"
-        ]
-
     def add_member_to_project(
         self,
         project_and_group_name,
         username,
         access_level,
         expires_at=None,
     ):
```

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.6.0/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/pipelines.py` & `gitlabform-3.6.0/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/project_badges.py` & `gitlabform-3.6.0/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.6.0/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.6.0/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.6.0/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/projects.py` & `gitlabform-3.6.0/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/repositories.py` & `gitlabform-3.6.0/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.6.0/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/schedules.py` & `gitlabform-3.6.0/gitlabform/gitlab/schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/tags.py` & `gitlabform-3.6.0/gitlabform/gitlab/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,14 @@
 
 class GitLabTags(GitLabCore):
     def get_tags(self, project_and_group_name):
         return self._make_requests_to_api(
             "projects/%s/repository/tags", project_and_group_name
         )
 
-    def create_tag(self, project_and_group_name, tag_name, ref, message=None):
-        data = {
-            "tag_name": tag_name,
-            "ref": ref,
-            "message": message,
-        }
-        return self._make_requests_to_api(
-            "projects/%s/repository/tags",
-            project_and_group_name,
-            method="POST",
-            data=data,
-            expected_codes=201,
-        )
-
     def delete_tag(self, project_and_group_name, tag_name):
         self._make_requests_to_api(
             "projects/%s/repository/tags/%s",
             (project_and_group_name, tag_name),
             method="DELETE",
             expected_codes=[200, 204],
         )
```

### Comparing `gitlabform-3.5.0/gitlabform/gitlab/variables.py` & `gitlabform-3.6.0/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/lists/__init__.py` & `gitlabform-3.6.0/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/lists/filter.py` & `gitlabform-3.6.0/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/lists/groups.py` & `gitlabform-3.6.0/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/lists/projects.py` & `gitlabform-3.6.0/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/output.py` & `gitlabform-3.6.0/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/__init__.py` & `gitlabform-3.6.0/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/abstract_processor.py` & `gitlabform-3.6.0/gitlabform/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/defining_keys.py` & `gitlabform-3.6.0/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/group/__init__.py` & `gitlabform-3.6.0/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.6.0/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.6.0/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.6.0/gitlabform/processors/group/group_members_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 class GroupMembersProcessor(AbstractProcessor):
     def __init__(self, gitlab: GitLab):
         super().__init__("group_members", gitlab)
 
     def _process_configuration(self, group: str, configuration: dict):
+        keep_bots = configuration.get("group_members|keep_bots", False)
+
         enforce_group_members = configuration.get("group_members|enforce", False)
 
         (
             groups_to_set_by_group_path,
             users_to_set_by_username,
         ) = self._get_groups_and_users_to_set(configuration)
 
@@ -30,15 +32,17 @@
                 " some 'users' or 'groups' defined as Owners,"
                 " if you want to enforce them (GitLab requires it).",
                 exit_code=EXIT_INVALID_INPUT,
             )
 
         self._process_groups(group, groups_to_set_by_group_path, enforce_group_members)
 
-        self._process_users(group, users_to_set_by_username, enforce_group_members)
+        self._process_users(
+            group, users_to_set_by_username, enforce_group_members, keep_bots
+        )
 
     @staticmethod
     def _get_groups_and_users_to_set(configuration: dict) -> Tuple[dict, dict]:
         groups_to_set_by_group_path = configuration.get("group_members|groups", {})
 
         users_to_set_by_username = configuration.get("group_members", {})
         if users_to_set_by_username:
@@ -133,15 +137,19 @@
                 self.gitlab.remove_share_from_group(group, group_path)
         else:
             debug("Not enforcing group members.")
 
         debug("Group shared with AFTER: %s", self.gitlab.get_group_members(group))
 
     def _process_users(
-        self, group: str, users_to_set_by_username: dict, enforce_group_members: bool
+        self,
+        group: str,
+        users_to_set_by_username: dict,
+        enforce_group_members: bool,
+        keep_bots: bool,
     ):
         # group users before by username
         # (note: we DON'T get inherited users as we don't manage them at this level anyway)
         users_before = self.gitlab.get_group_members(group, with_inherited=False)
         debug("Group members BEFORE: %s", users_before)
         users_before_by_username = dict()
         for user in users_before:
@@ -203,13 +211,18 @@
         if enforce_group_members:
             # remove users not configured explicitly
             # note: only direct members are removed - inherited are left
             users_not_configured = set(
                 [user["username"] for user in users_before]
             ) - set(users_to_set_by_username.keys())
             for user in users_not_configured:
+                if keep_bots and self.gitlab.get_user_by_name(user)["bot"]:
+                    debug(
+                        f"Will not remove bot user '{user}' as the 'keep_bots' option is true."
+                    )
+                    continue
                 debug("Removing user '%s' who is not configured to be a member.", user)
                 self.gitlab.remove_member_from_group(group, user)
         else:
             debug("Not enforcing group members.")
 
         debug("Group members AFTER: %s", self.gitlab.get_group_members(group))
```

### Comparing `gitlabform-3.5.0/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.6.0/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.6.0/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/__init__.py` & `gitlabform-3.6.0/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/files_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/members_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/members_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 
 class MembersProcessor(AbstractProcessor):
     def __init__(self, gitlab: GitLab):
         super().__init__("members", gitlab)
 
     def _process_configuration(self, project_and_group: str, configuration: dict):
+        keep_bots = configuration.get("members|keep_bots", False)
+
         enforce_members = configuration.get("members|enforce", False)
 
         groups = configuration.get("members|groups", {})
 
         users = configuration.get("members|users", {})
 
         if not groups and not users and not enforce_members:
@@ -23,15 +25,15 @@
                 "Project members configuration section has to contain"
                 " either 'users' or 'groups' non-empty keys"
                 " (unless you want to enforce no direct members).",
                 exit_code=EXIT_INVALID_INPUT,
             )
 
         self._process_groups(project_and_group, groups, enforce_members)
-        self._process_users(project_and_group, users, enforce_members)
+        self._process_users(project_and_group, users, enforce_members, keep_bots)
 
     def _process_groups(
         self, project_and_group: str, groups: dict, enforce_members: bool
     ):
         if groups:
             verbose("Processing groups as members...")
 
@@ -83,15 +85,19 @@
                     f"Removing group '{group_not_in_config}' that is not configured to be a member."
                 )
                 self.gitlab.unshare_with_group(project_and_group, group_not_in_config)
         else:
             debug("Not enforcing group members.")
 
     def _process_users(
-        self, project_and_group: str, users: dict, enforce_members: bool
+        self,
+        project_and_group: str,
+        users: dict,
+        enforce_members: bool,
+        keep_bots: bool,
     ):
         if users:
             verbose("Processing users as members...")
 
             current_members = self.gitlab.get_members_from_project(project_and_group)
             for user in users:
                 expires_at = (
@@ -136,14 +142,23 @@
             current_members = self.gitlab.get_members_from_project(project_and_group)
 
             users_in_config = users.keys()
             users_in_gitlab = current_members.keys()
             users_not_in_config = set(users_in_gitlab) - set(users_in_config)
 
             for user_not_in_config in users_not_in_config:
+                if (
+                    keep_bots
+                    and self.gitlab.get_user_by_name(user_not_in_config)["bot"]
+                ):
+                    debug(
+                        f"Will not remove bot user '{user_not_in_config}' as the 'keep_bots' option is true."
+                    )
+                    continue
+
                 debug(
                     f"Removing user '{user_not_in_config}' that is not configured to be a member."
                 )
                 self.gitlab.remove_member_from_project(
                     project_and_group, user_not_in_config
                 )
         else:
```

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/project_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/schedules_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/schedules_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.6.0/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.6.0/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.6.0/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.6.0/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/util/decorators.py` & `gitlabform-3.6.0/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.6.0/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.6.0/gitlabform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.5.0
+Version: 3.6.0
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.5.0 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.6.0 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.5.0/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.6.0/gitlabform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/setup.py` & `gitlabform-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,35 +42,36 @@
     packages=find_packages(),
     package_data={"": ["LICENSE", "version", "*.md", "config.yml"]},
     include_package_data=True,
     python_requires=">=3.7.0",
     install_requires=[
         "certifi",  # we want the latest root certs for security
         "requests==2.28.2",
-        "types-requests==2.28.11.15",
+        "types-requests==2.28.11.17",
         "Jinja2==3.1.2",
         "MarkupSafe==2.1.2",
         "ruamel.yaml==0.17.21",
         "luddite==1.0.2",
         "cli-ui==0.17.2",
         "packaging==23.0",
         "mergedeep==1.3.4",
-        "yamlpath==3.7.0",
+        "yamlpath==3.8.0",
         "ez-yaml==1.2.0",
     ],
     extras_require={
         "test": [
-            "pytest==7.2.2",
+            "python-gitlab==3.13.0",
+            "pytest==7.3.1",
             "xkcdpass==1.19.3",
             "pre-commit==2.21.0",  # not really for tests, but for development
             "coverage==7.2.1",
             "pytest-cov==4.0.0",
             "deepdiff==6.2.3",
             "pytest-rerunfailures==11.1.2",
-            "cryptography==39.0.2",
+            "cryptography==40.0.1",
             "mypy==1.1.1",
             "mypy-extensions==1.0.0",
         ],
         "docs": [
             "mkdocs",
             "mkdocs-material",
         ],
```

### Comparing `gitlabform-3.5.0/tests/acceptance/__init__.py` & `gitlabform-3.6.0/tests/acceptance/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import random
 import string
 import textwrap
+from contextlib import contextmanager
+from typing import List, Union, TYPE_CHECKING
+
+import gitlab
+from gitlab.v4.objects import Group, Project
 from xkcdpass import xkcd_password as xp
 
 from gitlabform import GitLabForm
-from gitlabform.gitlab import GitLab, AccessLevel
-from gitlabform.gitlab.core import NotFoundException, UnexpectedResponseException
 
 CONFIG = """
 config_version: 3
 """
 
 DEFAULT_README = "Default README content."
 
@@ -35,15 +38,33 @@
                         print(f"{env_var} set!")
                         break
                 except Exception as e:
                     print(f"Failed to read {file_path}: {e}")
             else:
                 print(f"{file_path} doesn't exist.")
 
-gl = GitLab(config_string=CONFIG)
+gl = gitlab.Gitlab(
+    os.getenv("GITLAB_URL"), private_token=os.getenv("GITLAB_TOKEN"), per_page=100
+)
+
+
+@contextmanager
+def allowed_codes(codes: Union[int, List[int]]):
+    """
+    A context manager that allows failures on specific response status codes
+    when gitlab.Gitlab objects.
+    """
+    if isinstance(codes, int):
+        codes = [codes]
+
+    try:
+        yield
+    except (gitlab.GitlabHttpError, gitlab.GitlabOperationError) as e:
+        if e.response_code not in codes:
+            raise e
 
 
 def get_random_name(entity: str) -> str:
     random_suffix = get_random_suffix()
     return f"gitlabform_{entity}_{random_suffix}"
 
 
@@ -62,127 +83,149 @@
     length = 16
     all_chars = string.ascii_letters + string.digits
     password = "".join(random.sample(all_chars, length))
 
     return password
 
 
-def get_gitlab():
-    return gl
-
-
-def create_group(group_name, parent_id=None):
-    gl.create_group(group_name, group_name, parent_id=parent_id, visibility="internal")
+def create_group(group_name, parent_id=None) -> Group:
+    with allowed_codes(404):
+        group = gl.groups.create(
+            {
+                "name": group_name,
+                "path": group_name,
+                "parent_id": parent_id,
+                "visibility": "internal",
+            }
+        )
+    if TYPE_CHECKING:
+        assert isinstance(group, Group)
+    return group
 
 
 def create_groups(group_base_name, no_of_groups):
     groups = []
     for group_no in range(1, no_of_groups + 1):
         group_name = group_base_name + str(group_no)
         try:
-            gl.get_group_case_insensitive(group_name)
-        except NotFoundException:
-            gl.create_group(group_name, group_name)
-        groups.append(group_name)
+            group = gl.groups.get(group_name)
+        except gitlab.GitlabGetError:
+            group = create_group(group_name)
+        groups.append(group)
     return groups
 
 
 def delete_groups(group_base_name, no_of_groups):
     for group_no in range(1, no_of_groups + 1):
         group_name = group_base_name + str(group_no)
-        gl.delete_group(group_name)
+        with allowed_codes(404):
+            gl.groups.delete(group_name)
 
 
-def create_project(group_name, project_name):
-    group = gl.get_group(group_name)
-    gl.create_project(
-        project_name,
-        project_name,
-        group["id"],
-        default_branch="main",
-        wait_if_still_being_deleted=True,
+def create_project(group: Group, project_name) -> Project:
+    project = gl.projects.create(
+        {
+            "name": project_name,
+            "path": project_name,
+            "namespace_id": group.id,
+            "default_branch": "main",
+        }
     )
 
-    gl.add_file(
-        f"{group_name}/{project_name}",
-        "main",
-        "README.md",
-        DEFAULT_README,
-        "Create README",
+    project.files.create(
+        {
+            "branch": "main",
+            "file_path": "README.md",
+            "content": DEFAULT_README,
+            "commit_message": "Create README",
+        }
     )
+    if TYPE_CHECKING:
+        assert isinstance(project, Project)
+    return project
 
 
 def create_users(user_base_name, no_of_users):
     users = []
     for user_no in range(1, no_of_users + 1):
         username = user_base_name + str(user_no)
+        existing = gl.users.list(username=username)
         try:
-            gl.get_user_by_name(username)
-        except NotFoundException:
-            gl.create_user(
-                username + "@example.com",
-                username + " Example",
-                username,
-                get_random_password(),
+            user = existing[0]
+        except IndexError:
+            user = gl.users.create(
+                {
+                    "username": username,
+                    "email": username + "@example.com",
+                    "name": username + " Example",
+                    "password": get_random_password(),
+                }
             )
-        users.append(username)
+        users.append(user)
     return users
 
 
-def delete_users(user_base_name, no_of_users):
-    for user_no in range(1, no_of_users + 1):
-        username = user_base_name + str(user_no)
-        gl.delete_user(username)
-
-
-def remove_users_from_project(user_base_name, no_of_users, project_and_group):
-    for user_no in range(1, no_of_users + 1):
-        username = user_base_name + str(user_no)
-        gl.remove_member_from_project(project_and_group, username)
+def get_only_branch_access_levels(project: Project, branch):
+    protected_branch = None
 
+    with allowed_codes(404):
+        protected_branch = project.protectedbranches.get(branch)
 
-def add_users_to_group(group_name, usernames, access_level=AccessLevel.DEVELOPER.value):
-    for username in usernames:
-        try:
-            gl.add_member_to_group(group_name, username, access_level)
-        except UnexpectedResponseException:
-            # this is fine - user is already in the group
-            pass
+    if not protected_branch:
+        return None, None, None, None, None
 
+    push_access_levels = set()
+    merge_access_levels = set()
+    push_access_user_ids = set()
+    merge_access_user_ids = set()
+    unprotect_access_level = None
+
+    if "push_access_levels" in protected_branch.attributes:
+        for push_access in protected_branch.push_access_levels:
+            if not push_access["user_id"]:
+                push_access_levels.add(push_access["access_level"])
+            else:
+                push_access_user_ids.add(push_access["user_id"])
 
-def remove_users_from_group(group_name, usernames):
-    for username in usernames:
-        try:
-            gl.remove_member_from_group(group_name, username)
-        except NotFoundException:
-            # this is fine - user is removed from group
-            pass
-
-
-def delete_variables_from_group(group_name, variables):
-    for variable in variables:
-        try:
-            gl.delete_group_variable(group_name, variable)
-        except NotFoundException:
-            # this is fine - variable is removed from group
-            pass
-
+    if "merge_access_levels" in protected_branch.attributes:
+        for merge_access in protected_branch.merge_access_levels:
+            if not merge_access["user_id"]:
+                merge_access_levels.add(merge_access["access_level"])
+            else:
+                merge_access_user_ids.add(merge_access["user_id"])
 
-def delete_pipeline_schedules_from_project(project_and_group):
-    schedules = gl.get_all_pipeline_schedules(project_and_group)
-    for schedule in schedules:
-        gl.delete_pipeline_schedule(project_and_group, schedule["id"])
+    if (
+        "unprotect_access_levels" in protected_branch.attributes
+        and len(protected_branch.unprotect_access_levels) == 1
+    ):
+        unprotect_access_level = protected_branch.unprotect_access_levels[0][
+            "access_level"
+        ]
+
+    return (
+        sorted(push_access_levels),
+        sorted(merge_access_levels),
+        sorted(push_access_user_ids),
+        sorted(merge_access_user_ids),
+        unprotect_access_level,
+    )
 
 
 def run_gitlabform(config, target, include_archived_projects=True):
     # f-strings with """ used as configs have the disadvantage of having indentation in them - let's remove it here
     config = textwrap.dedent(config)
 
     # we don't want to repeat ourselves in the tests, so prefix the configs with this mandatory part here
     config = CONFIG + config
 
+    # allow passing in gitlab RESTObjects. assume full path string otherwise
+    if isinstance(target, Group):
+        target = target.full_path
+    elif isinstance(target, Project):
+        target = target.path_with_namespace
+
     gf = GitLabForm(
         include_archived_projects=include_archived_projects,
         config_string=config,
         target=target,
     )
     gf.run()
```

### Comparing `gitlabform-3.5.0/tests/acceptance/conftest.py` & `gitlabform-3.6.0/tests/acceptance/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,146 @@
 import os
 from typing import Callable, Optional, Generator, List
 
 import pytest
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
+from gitlab import Gitlab
+from gitlab.v4.objects import Group, Project, User, ProjectAccessToken, GroupAccessToken
 
 from gitlabform.gitlab import AccessLevel, GitLab
 from tests.acceptance import (
-    get_gitlab,
+    allowed_codes,
     create_group,
     create_groups,
     delete_groups,
     create_project,
     get_random_name,
     create_users,
-    delete_users,
     get_random_password,
 )
 
 
 @pytest.fixture(scope="session")
-def gitlab() -> Generator[GitLab, None, None]:
-    gl = get_gitlab()
-    yield gl  # provide fixture value
+def gl():
+    return Gitlab(os.getenv("GITLAB_URL"), private_token=os.getenv("GITLAB_TOKEN"))
 
 
-@pytest.fixture(scope="class")
-def group_and_project(group, project) -> str:
-    return f"{group}/{project}"
+@pytest.fixture(autouse=True)
+def requires_license(gl: Gitlab, request):
+    if not request.node.get_closest_marker("requires_license"):
+        return
+
+    gitlab_license = gl.get_license()
+    if not gitlab_license or gitlab_license["expired"]:
+        pytest.skip("this test requires a GitLab license (Paid/Trial)")
 
 
-@pytest.fixture(scope="function")
-def group_and_project_for_function(group, project_for_function) -> str:
-    return f"{group}/{project_for_function}"
+@pytest.fixture(scope="session")
+def root_user(gl):
+    return gl.users.list(username="root")[0]
 
 
 @pytest.fixture(scope="class")
-def group() -> Generator[str, None, None]:
+def group(gl: Gitlab) -> Generator[Optional[Group], None, None]:
     group_name = get_random_name("group")
-    create_group(group_name)
+    gitlab_group = create_group(group_name)
 
-    yield group_name
+    yield gitlab_group
 
-    gl = get_gitlab()
-    gl.delete_group(group_name)
+    with allowed_codes(404):
+        gl.groups.delete(group_name)
 
 
 @pytest.fixture(scope="function")
-def group_for_function():
+def group_for_function(gl: Gitlab):
     group_name = get_random_name("group")
-    create_group(group_name)
+    gitlab_group = create_group(group_name)
 
-    yield group_name
+    yield gitlab_group
 
-    gl = get_gitlab()
-    gl.delete_group(group_name)
+    with allowed_codes(404):
+        gl.groups.delete(group_name)
 
 
 @pytest.fixture(scope="class")
-def other_group():
+def other_group(gl: Gitlab):
     # TODO: deduplicate this - it's a copy and paste from the above fixture
     group_name = get_random_name("group")
-    create_group(group_name)
+    group = create_group(group_name)
 
-    yield group_name
+    yield group
 
-    gl = get_gitlab()
-    gl.delete_group(group_name)
+    with allowed_codes(404):
+        gl.groups.delete(group_name)
 
 
 @pytest.fixture(scope="class")
-def third_group():
+def third_group(gl: Gitlab):
     # TODO: deduplicate this - it's a copy and paste from the above fixture
     group_name = get_random_name("group")
-    create_group(group_name)
+    group = create_group(group_name)
 
-    yield group_name
+    yield group
 
-    gl = get_gitlab()
-    gl.delete_group(group_name)
+    with allowed_codes(404):
+        gl.groups.delete(group_name)
 
 
 @pytest.fixture(scope="class")
-def subgroup(group):
-    gl = get_gitlab()
-    parent_id = gl.get_group_id_case_insensitive(group)
-    group_name = get_random_name("subgroup")
-    create_group(group_name, parent_id)
+def subgroup(gl: Gitlab, group: Group):
+    subgroup_name = get_random_name("subgroup")
+    gitlab_subgroup = create_group(subgroup_name, group.id)
 
-    yield group + "/" + group_name
+    yield gitlab_subgroup
 
-    gl = get_gitlab()
-    gl.delete_group(group + "/" + group_name)
+    with allowed_codes(404):
+        gl.groups.delete(f"{group.full_path}/{subgroup_name}")
 
 
 @pytest.fixture(scope="class")
-def project_in_subgroup(subgroup):
+def project(gl: Gitlab, group: Group):
     project_name = get_random_name("project")
-    create_project(subgroup, project_name)
+    gitlab_project = create_project(group, project_name)
 
-    yield f"{subgroup}/{project_name}"
+    yield gitlab_project
 
-    gl = get_gitlab()
-    gl.delete_project(f"{subgroup}/{project_name}")
+    gitlab_project.delete()
 
 
 @pytest.fixture(scope="class")
-def project(group):
+def project_in_subgroup(gl: Gitlab, subgroup: Group):
     project_name = get_random_name("project")
-    create_project(group, project_name)
+    gitlab_project = create_project(subgroup, project_name)
 
-    yield project_name
+    yield gitlab_project
 
-    gl = get_gitlab()
-    gl.delete_project(f"{group}/{project_name}")
+    gitlab_project.delete()
 
 
 @pytest.fixture(scope="function")
-def project_for_function(group):
+def project_for_function(gl: Gitlab, group: Group):
     project_name = get_random_name("project")
-    create_project(group, project_name)
+    gitlab_project = create_project(group, project_name)
 
-    yield project_name
+    yield gitlab_project
 
-    gl = get_gitlab()
-    gl.delete_project(f"{group}/{project_name}")
+    gitlab_project.delete()
 
 
 @pytest.fixture(scope="class")
-def other_project(group):
+def other_project(gl: Gitlab, group):
     # TODO: deduplicate this - it's a copy and paste from the above fixture
     project_name = get_random_name("project")
-    create_project(group, project_name)
+    gitlab_project = create_project(group, project_name)
 
-    yield project_name
+    yield gitlab_project
 
-    gl = get_gitlab()
-    gl.delete_project(f"{group}/{project_name}")
+    gitlab_project.delete()
 
 
 @pytest.fixture(scope="class")
 def groups(users):
     no_of_groups = 4
 
     group_name_base = get_random_name("group")
@@ -157,129 +156,184 @@
     no_of_users = 4
 
     username_base = get_random_name("user")
     users = create_users(username_base, no_of_users)
 
     yield users
 
-    delete_users(username_base, no_of_users)
+    for user in users:
+        user.delete()
 
 
 @pytest.fixture(scope="class")
 def other_users():
     # TODO: deduplicate this - it's a copy and paste from the above fixture
     no_of_users = 4
 
     username_base = get_random_name("user")
     users = create_users(username_base, no_of_users)
 
     yield users
 
-    delete_users(username_base, no_of_users)
+    for user in users:
+        user.delete()
 
 
 @pytest.fixture(scope="class")
-def branch(gitlab, group_and_project):
+def branch(project):
     name = get_random_name("branch")
-    gitlab.create_branch(group_and_project, name, "main")
+    branch = project.branches.create({"branch": name, "ref": "main"})
 
     yield name
 
-    gitlab.delete_branch(group_and_project, name)
+    branch.delete()
 
 
 @pytest.fixture(scope="class")
-def other_branch(gitlab, group_and_project):
+def other_branch(project):
     # TODO: deduplicate
     name = get_random_name("other_branch")
-    gitlab.create_branch(group_and_project, name, "main")
+    branch = project.branches.create({"branch": name, "ref": "main"})
 
     yield name
 
-    gitlab.delete_branch(group_and_project, name)
-
-
-class User:
-    def __init__(self, name, id):
-        self.name = name
-        self.id = id
+    branch.delete()
 
 
 @pytest.fixture(scope="class")
 def make_user(
-    gitlab, group_and_project
+    gl, project
 ) -> Generator[Callable[[AccessLevel, bool], User], None, None]:
     username_base = get_random_name("user")
     created_users: List[User] = []
 
     def _make_user(
         level: AccessLevel = AccessLevel.DEVELOPER, add_to_project: bool = True
     ) -> User:
         last_id = len(created_users) + 1
         username = f"{username_base}_{last_id}"
-        user = gitlab.create_user(
-            username + "@example.com",
-            username + " Example",
-            username,
-            get_random_password(),
+        user = gl.users.create(
+            {
+                "username": username,
+                "email": username + "@example.com",
+                "name": username + " Example",
+                "password": get_random_password(),
+            }
         )
-
         if add_to_project:
-            gitlab.add_member_to_project(group_and_project, username, level.value)
-
-        user_obj = User(username, user["id"])
-        created_users.append(user_obj)
-        return user_obj
+            project.members.create({"user_id": user.id, "access_level": level.value})
+        created_users.append(user)
+        return user
 
     yield _make_user
 
     for user in created_users:
-        gitlab.delete_user(None, user_id=user.id)
+        with allowed_codes(404):
+            gl.users.delete(user.id)
+
+
+@pytest.fixture(scope="class")
+def make_project_access_token(
+    project,
+) -> Generator[Callable[[AccessLevel, List[str]], ProjectAccessToken], None, None]:
+    token_name_base = get_random_name("user")
+    created_tokens: List[ProjectAccessToken] = []
+
+    def _make_project_access_token(
+        level: AccessLevel = AccessLevel.DEVELOPER, scopes: List[str] = ["api"]
+    ) -> ProjectAccessToken:
+        last_id = len(created_tokens) + 1
+        token_name = f"{token_name_base}_{last_id}_bot"
+        token = project.access_tokens.create(
+            {
+                "access_level": level,
+                "name": token_name,
+                "scopes": scopes,
+            }
+        )
+        created_tokens.append(token)
+        return token
+
+    yield _make_project_access_token
+
+    for token in created_tokens:
+        with allowed_codes(404):
+            project.access_tokens.delete(token.id)
+
+
+@pytest.fixture(scope="class")
+def make_group_access_token(
+    group,
+) -> Generator[Callable[[AccessLevel, List[str]], GroupAccessToken], None, None]:
+    token_name_base = get_random_name("user")
+    created_tokens: List[GroupAccessToken] = []
+
+    def _make_group_access_token(
+        level: AccessLevel = AccessLevel.DEVELOPER, scopes: List[str] = ["api"]
+    ) -> GroupAccessToken:
+        last_id = len(created_tokens) + 1
+        token_name = f"{token_name_base}_{last_id}_bot"
+        token = group.access_tokens.create(
+            {
+                "access_level": level,
+                "name": token_name,
+                "scopes": scopes,
+            }
+        )
+        created_tokens.append(token)
+        return token
+
+    yield _make_group_access_token
+
+    for token in created_tokens:
+        with allowed_codes(404):
+            group.access_tokens.delete(token.id)
 
 
 @pytest.fixture(scope="class")
-def three_members(gitlab, group_and_project, make_user):
+def three_members(make_user):
     member1 = make_user()
     member2 = make_user()
     member3 = make_user()
 
     yield [member1.name, member2.name, member3.name]
 
 
 @pytest.fixture(scope="function")
-def outsider_user(gitlab, group_and_project):
+def outsider_user(gl):
     username = get_random_name("outsider_user")
-    user = gitlab.create_user(
-        username + "@example.com",
-        username + " Example",
-        username,
-        get_random_password(),
+    user = gl.users.create(
+        {
+            "username": username,
+            "email": username + "@example.com",
+            "name": username + " Example",
+            "password": get_random_password(),
+        }
     )
-    user_obj = User(username, user["id"])
 
-    yield user_obj.name
+    yield user
 
-    gitlab.delete_user(None, user_id=user_obj.id)
+    gl.users.delete(user.id)
 
 
 @pytest.fixture(scope="function")
-def public_ssh_key(gitlab):
+def public_ssh_key():
     key = rsa.generate_private_key(
         backend=crypto_default_backend(), public_exponent=65537, key_size=2048
     )
 
     public_key = key.public_key().public_bytes(
         crypto_serialization.Encoding.OpenSSH, crypto_serialization.PublicFormat.OpenSSH
     )
 
     yield public_key.decode("UTF-8")
 
 
 @pytest.fixture(scope="function")
-def other_public_ssh_key(gitlab):
+def other_public_ssh_key():
     # TODO: deduplicate this - it's a copy and paste from the above fixture
     key = rsa.generate_private_key(
         backend=crypto_default_backend(), public_exponent=65537, key_size=2048
     )
 
     public_key = key.public_key().public_bytes(
         crypto_serialization.Encoding.OpenSSH, crypto_serialization.PublicFormat.OpenSSH
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_archive_project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,86 @@
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestArchiveProject:
-    def test__archive_project(self, gitlab, group_and_project):
+    def test__archive_project(self, gl, project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project:
               archive: true
         """
 
-        run_gitlabform(config, group_and_project)
-        project = gitlab.get_project(group_and_project)
-        assert project["archived"] is True
-
-    def test__unarchive_project(
-        self, gitlab, group_and_project, other_group, other_project
-    ):
+        run_gitlabform(config, project)
+        project = gl.projects.get(project.id)
+        assert project.archived is True
+
+    def test__unarchive_project(self, gl, project, other_group, other_project):
         archive_project = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project:
               archive: true
         """
 
-        run_gitlabform(archive_project, group_and_project)
-        project = gitlab.get_project(group_and_project)
-        assert project["archived"] is True
+        run_gitlabform(archive_project, project)
+        project = gl.projects.get(project.id)
+        assert project.archived is True
 
         unarchive_project = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project:
               archive: false
         """
 
         # 1. if you run gitlabform ALL, but without '--include-archived-projects',
         # then nothing will happen here as the archived project will be omitted when in
         # the effective list of groups and projects
 
         run_gitlabform(unarchive_project, "ALL", False)
-        project = gitlab.get_project(group_and_project)
-        assert project["archived"] is True
+        project = gl.projects.get(project.id)
+        assert project.archived is True
 
         # 2. only after you run gitlabform ALL, with '--include-archived-projects'
         # (OR pointing to it that project)
         # the target project will be unarchived
         run_gitlabform(unarchive_project, "ALL")
-        project = gitlab.get_project(group_and_project)
-        assert project["archived"] is False
-
-    def test__dont_edit_archived_project(self, gitlab, group, project):
-        group_and_project = f"{group}/{project}"
+        project = gl.projects.get(project.id)
+        assert project.archived is False
 
+    def test__dont_edit_archived_project(self, gl, group, project):
         archive_project = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project:
               archive: true
         """
 
-        run_gitlabform(archive_project, group_and_project)
-        project = gitlab.get_project(group_and_project)
-        assert project["archived"] is True
+        run_gitlabform(archive_project, project)
+        project = gl.projects.get(project.id)
+        assert project.archived is True
 
         edit_archived_project = f"""
         # the project has to be configured as archived
         # for other configs for it to be ignored
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project:
               archive: true
 
-          {group}/*:
+          {group.full_path}/*:
             files:
               README.md:
                 overwrite: true
                 branches:
                   - main
                 content: |
                   Some other content that the default one
         """
 
-        run_gitlabform(edit_archived_project, group_and_project)
+        run_gitlabform(edit_archived_project, project.path_with_namespace)
 
         # the fact that we are not getting an exception because of trying to edit
         # an archived project means that the test is passing
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_badges.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_badges.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,164 @@
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
+def get_project_badges(project):
+    badges = project.badges.list(iterator=True)
+    return [badge for badge in badges if badge.kind == "project"]
+
+
 class TestBadges:
-    def test__badges_add(self, gitlab, group_and_project):
+    def test__badges_add(self, project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             badges:
               pipeline-status:
                 name: "Project Badge"
                 link_url: "https://gitlab.example.com/%{{project_path}}/-/commits/%{{default_branch}}/foo"
                 image_url: "https://gitlab.example.com/%{{project_path}}/badges/%{{default_branch}}/pipeline.svg"
         """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 1
-        assert badges[0]["name"] == "Project Badge"
+        assert badges[0].name == "Project Badge"
 
-    def test__badges_delete(self, gitlab, group_and_project):
+    def test__badges_delete(self, project):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     link_url: "https://gitlab.example.com/%{{project_path}}/-/commits/%{{default_branch}}/foo"
                     image_url: "https://gitlab.example.com/%{{project_path}}/badges/%{{default_branch}}/pipeline.svg"
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 1
-        assert badges[0]["name"] == "Project Badge"
+        assert badges[0].name == "Project Badge"
 
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     delete: true
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 0
 
-    def test__badges_update(self, gitlab, group_and_project):
+    def test__badges_update(self, project):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     link_url: "https://gitlab.example.com/foo"
                     image_url: "https://gitlab.example.com/pipeline.svg"
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 1
-        assert badges[0]["link_url"].endswith("foo")
+        assert badges[0].link_url.endswith("foo")
 
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     link_url: "https://gitlab.example.com/bar"
                     image_url: "https://gitlab.example.com/pipeline.svg"
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 1
-        assert badges[0]["link_url"].endswith("bar")
+        assert badges[0].link_url.endswith("bar")
 
-    def test__badges_update_choose_the_right_one(self, gitlab, group_and_project):
+    def test__badges_update_choose_the_right_one(self, project):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     link_url: "https://gitlab.example.com/first"
                     image_url: "https://gitlab.example.com/first"
                   another:
                     name: "Project Badge 2"
                     link_url: "https://gitlab.example.com/second"
                     image_url: "https://gitlab.example.com/second" 
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 2
 
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 badges:
                   a_different_key:
                     name: "Project Badge 2"
                     link_url: "https://gitlab.example.com/foobar"
                     image_url: "https://gitlab.example.com/foobar"
                   and_also_different_than_before:
                     name: "Project Badge"
                     delete: true
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project)
         assert len(badges) == 1
 
         for badge in badges:
-            if badge["name"] == "Project Badge 2":
-                assert badge["link_url"].endswith("foobar")
-                assert badge["image_url"].endswith("foobar")
+            if badge.name == "Project Badge 2":
+                assert badge.link_url.endswith("foobar")
+                assert badge.image_url.endswith("foobar")
             else:
-                assert not badge["link_url"].endswith("foobar")
-                assert not badge["image_url"].endswith("foobar")
-
-    def test__badges_enforce(self, gitlab, group_and_project_for_function):
-        group_and_project = group_and_project_for_function
+                assert not badge.link_url.endswith("foobar")
+                assert not badge.image_url.endswith("foobar")
 
+    def test__badges_enforce(self, project_for_function):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project_for_function.path_with_namespace}:
                 badges:
                   pipeline-status:
                     name: "Project Badge"
                     link_url: "https://gitlab.example.com/first"
                     image_url: "https://gitlab.example.com/first"
                   another:
                     name: "Project Badge 2"
                     link_url: "https://gitlab.example.com/second"
                     image_url: "https://gitlab.example.com/second" 
             """
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project_for_function.path_with_namespace)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project_for_function)
         assert len(badges) == 2
 
         config2 = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project_for_function.path_with_namespace}:
                 badges:
                   another:
                     name: "Project Badge 2"
                     link_url: "https://gitlab.example.com/foobar"
                     image_url: "https://gitlab.example.com/foobar"
                   enforce: true
             """
-        run_gitlabform(config2, group_and_project)
+        run_gitlabform(config2, project_for_function.path_with_namespace)
 
-        badges = gitlab.get_project_badges(group_and_project)
+        badges = get_project_badges(project_for_function)
         assert len(badges) == 1
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_branches.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_branches.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,84 @@
 from gitlabform.gitlab import AccessLevel
-from tests.acceptance import (
-    run_gitlabform,
-    get_gitlab,
-)
-
-
-gl = get_gitlab()
+from tests.acceptance import get_only_branch_access_levels, run_gitlabform
 
 
 class TestBranches:
-    def test__protect_and_unprotect(self, gitlab, group_and_project, branch):
+    def test__protect_and_unprotect(self, project, branch):
         config_protect_branch = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: true
                 push_access_level: {AccessLevel.NO_ACCESS.value}
                 merge_access_level: {AccessLevel.MAINTAINER.value}
                 unprotect_access_level: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(config_protect_branch, group_and_project)
+        run_gitlabform(config_protect_branch, project.path_with_namespace)
 
         (
             push_access_levels,
             merge_access_levels,
             push_access_user_ids,
             merge_access_user_ids,
             unprotect_access_level,
-        ) = gitlab.get_only_branch_access_levels(group_and_project, branch)
+        ) = get_only_branch_access_levels(project, branch)
         assert push_access_levels == [AccessLevel.NO_ACCESS.value]
         assert merge_access_levels == [AccessLevel.MAINTAINER.value]
         assert push_access_user_ids == []
         assert merge_access_user_ids == []
         assert unprotect_access_level is AccessLevel.MAINTAINER.value
 
         config_unprotect_branch = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: false
                 push_access_level: {AccessLevel.NO_ACCESS.value}
                 merge_access_level: {AccessLevel.MAINTAINER.value}
                 unprotect_access_level: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(config_unprotect_branch, group_and_project)
+        run_gitlabform(config_unprotect_branch, project.path_with_namespace)
 
         (
             push_access_levels,
             merge_access_levels,
             push_access_user_ids,
             merge_access_user_ids,
             unprotect_access_level,
-        ) = gitlab.get_only_branch_access_levels(group_and_project, branch)
+        ) = get_only_branch_access_levels(project, branch)
         assert push_access_levels is None
         assert merge_access_levels is None
         assert push_access_user_ids is None
         assert merge_access_user_ids is None
         assert unprotect_access_level is None
 
-    def test__config_with_access_level_names(self, gitlab, group_and_project, branch):
+    def test__config_with_access_level_names(self, project, branch):
         config_with_access_levels_names = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: true
                 push_access_level: no_access        # note "_" or " " and the various
                 merge_access_level: Developer       # case in each line. it should not
                 unprotect_access_level: MAINTAINER  # matter as we allow any case.
         """
 
-        run_gitlabform(config_with_access_levels_names, group_and_project)
+        run_gitlabform(config_with_access_levels_names, project.path_with_namespace)
 
         (
             push_access_level,
             merge_access_level,
             push_access_user_ids,
             merge_access_user_ids,
             unprotect_access_level,
-        ) = gitlab.get_only_branch_access_levels(group_and_project, branch)
+        ) = get_only_branch_access_levels(project, branch)
         assert push_access_level == [AccessLevel.NO_ACCESS.value]
         assert merge_access_level == [AccessLevel.DEVELOPER.value]
         assert push_access_user_ids == []
         assert merge_access_user_ids == []
         assert unprotect_access_level is AccessLevel.MAINTAINER.value
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestDeployKeysAllProjects:
     def test__deploy_key_to_all_projects(
-        self, gitlab, group, project, other_project, public_ssh_key
+        self, group, project, other_project, public_ssh_key
     ):
         deploy_key_to_all_projects = f"""
         projects_and_groups:
           "*":
             deploy_keys:
               foobar:
                 key: {public_ssh_key}
                 title: common_key
                 can_push: false
         """
-        run_gitlabform(deploy_key_to_all_projects, group)
-
-        deploy_keys1 = gitlab.get_deploy_keys(f"{group}/{project}")
-        assert len(deploy_keys1) == 1
+        run_gitlabform(deploy_key_to_all_projects, group.full_path)
 
-        deploy_keys2 = gitlab.get_deploy_keys(f"{group}/{other_project}")
-        assert len(deploy_keys2) == 1
+        assert len(project.keys.list()) == 1
+        assert len(other_project.keys.list()) == 1
 
     def test__deploy_key_with_spaces_in_comment_to_all_projects(
-        self, gitlab, group, project, other_project, public_ssh_key
+        self, group, project, other_project, public_ssh_key
     ):
         public_ssh_key = f"{public_ssh_key} this is a comment with spaces"
 
         deploy_key_to_all_projects = f"""
         projects_and_groups:
           "*":
             deploy_keys:
               foobar:
                 key: {public_ssh_key}
                 title: common_key
                 can_push: false
         """
         run_gitlabform(deploy_key_to_all_projects, group)
 
-        deploy_keys1 = gitlab.get_deploy_keys(f"{group}/{project}")
-        assert len(deploy_keys1) == 1
-
-        deploy_keys2 = gitlab.get_deploy_keys(f"{group}/{other_project}")
-        assert len(deploy_keys2) == 1
+        assert len(project.keys.list()) == 1
+        assert len(other_project.keys.list()) == 1
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_files.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_files.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import os
 import pytest
-import re
+
+from gitlab import GitlabGetError
 
 from gitlabform.gitlab import AccessLevel
-from gitlabform.gitlab.core import NotFoundException
-from tests.acceptance import run_gitlabform, DEFAULT_README
+from tests.acceptance import (
+    get_only_branch_access_levels,
+    run_gitlabform,
+    DEFAULT_README,
+)
 
 
 @pytest.fixture(scope="function")
-def no_access_branch(request, gitlab, group_and_project):
-    gitlab.create_branch(group_and_project, "no_access_branch", "main")
-    gitlab.protect_branch(
-        group_and_project,
-        "no_access_branch",
+def no_access_branch(project):
+    branch = project.branches.create({"branch": "no_access_branch", "ref": "main"})
+    protected_branch = project.protectedbranches.create(
         {
+            "name": "no_access_branch",
             "push_access_level": AccessLevel.NO_ACCESS.value,
             "merge_access_level": AccessLevel.NO_ACCESS.value,
             "unprotect_access_level": AccessLevel.MAINTAINER.value,
         },
     )
 
-    def fin():
-        gitlab.unprotect_branch(group_and_project, "no_access_branch")
-        gitlab.delete_branch(group_and_project, "no_access_branch")
+    yield branch
 
-    request.addfinalizer(fin)
+    protected_branch.delete()
+    branch.delete()
 
 
 @pytest.fixture(scope="class")
 def file(request):
     f = open("file.txt", "a")
     f.write("Hanzi (Simplified): 丏丅丙两\nHanzi (Traditional): 丕不丈丁")
     f.close()
@@ -48,145 +50,140 @@
     def fin():
         os.remove("file2.txt")
 
     request.addfinalizer(fin)
 
 
 class TestFiles:
-    def test__set_file_specific_branch(self, gitlab, group_and_project, branch):
+    def test__set_file_specific_branch(self, project, branch):
         set_file_specific_branch = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: true
                 push_access_level: maintainer
                 merge_access_level: developer
                 unprotect_access_level: maintainer
             files:
               "README.md":
                 overwrite: true
                 branches:
                   - {branch}
                 content: "Content for {branch} only"
         """
 
-        run_gitlabform(set_file_specific_branch, group_and_project)
+        run_gitlabform(set_file_specific_branch, project.path_with_namespace)
 
-        commit = gitlab.get_last_commit(group_and_project, branch)
+        the_branch = project.branches.get(branch)
         assert all(
-            [text in commit["message"] for text in ["Automated", "made by gitlabform"]]
+            [
+                text in the_branch.commit["message"]
+                for text in ["Automated", "made by gitlabform"]
+            ]
         )
 
-        file_content = gitlab.get_file(group_and_project, branch, "README.md")
-        assert file_content == f"Content for {branch} only"
+        project_file = project.files.get(ref=branch, file_path="README.md")
+        assert project_file.decode().decode("utf-8") == f"Content for {branch} only"
 
-        other_branch_file_content = gitlab.get_file(
-            group_and_project, "main", "README.md"
-        )
-        assert other_branch_file_content == DEFAULT_README
+        project_file = project.files.get(ref="main", file_path="README.md")
+        assert project_file.decode().decode("utf-8") == DEFAULT_README
 
         # check if main stays protected after the file update
-        the_branch = gitlab.get_branch(group_and_project, branch)
-        assert the_branch["protected"] is True
+        assert the_branch.protected is True
 
-    def test__set_file_strongly_protected_branch(
-        self, gitlab, group_and_project, no_access_branch
-    ):
+    def test__set_file_strongly_protected_branch(self, project, no_access_branch):
         set_file_specific_branch = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 branches:
                   no_access_branch:
                     protected: true
                     push_access_level: no access
                     merge_access_level: no access
                     unprotect_access_level: maintainer
                 files:
                   "README.md":
                     overwrite: true
                     branches:
                       - no_access_branch
                     content: "Content for no_access_branch only"
             """
 
-        run_gitlabform(set_file_specific_branch, group_and_project)
+        run_gitlabform(set_file_specific_branch, project)
 
-        commit = gitlab.get_last_commit(group_and_project, "no_access_branch")
-        assert commit["message"] == "Automated change made by gitlabform"
+        branch = project.branches.get(no_access_branch.name)
+        assert branch.commit["message"] == "Automated change made by gitlabform"
 
-        file_content = gitlab.get_file(
-            group_and_project, "no_access_branch", "README.md"
+        project_file = project.files.get(ref="no_access_branch", file_path="README.md")
+        assert (
+            project_file.decode().decode("utf-8") == "Content for no_access_branch only"
         )
-        assert file_content == "Content for no_access_branch only"
 
-        other_branch_file_content = gitlab.get_file(
-            group_and_project, "main", "README.md"
-        )
-        assert other_branch_file_content == DEFAULT_README
+        project_file = project.files.get(ref="main", file_path="README.md")
+        assert project_file.decode().decode("utf-8") == DEFAULT_README
 
         # check if no_access_branch stays protected after the file update
-        branch = gitlab.get_branch(group_and_project, "no_access_branch")
-        assert branch["protected"] is True
+        assert branch.protected is True
 
-    def test__delete_file_specific_branch(self, gitlab, group_and_project, branch):
+    def test__delete_file_specific_branch(self, project, branch):
         set_file_specific_branch = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 branches:
                   {branch}:
                     protected: true
                     push_access_level: maintainer
                     merge_access_level: developer
                     unprotect_access_level: maintainer
                 files:
                   "README.md":
                     branches:
                       - {branch}
                     delete: true
             """
 
-        run_gitlabform(set_file_specific_branch, group_and_project)
+        run_gitlabform(set_file_specific_branch, project)
 
-        commit = gitlab.get_last_commit(group_and_project, branch)
-        assert commit["message"] == "Automated delete made by gitlabform"
+        the_branch = project.branches.get(branch)
+        assert the_branch.commit["message"] == "Automated delete made by gitlabform"
 
-        with pytest.raises(NotFoundException):
-            gitlab.get_file(group_and_project, branch, "README.md")
+        with pytest.raises(GitlabGetError):
+            project.files.get(ref=branch, file_path="README.md")
 
         # check if main stays protected after the file delete
-        the_branch = gitlab.get_branch(group_and_project, branch)
-        assert the_branch["protected"] is True
+        the_branch = project.branches.get(the_branch.name)
+        assert the_branch.protected is True
 
-    def test__custom_commit_message(self, gitlab, group_and_project, branch):
+    def test__custom_commit_message(self, project, branch):
         set_file_specific_branch = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: false
             files:
               "README.md":
                 overwrite: true
                 branches:
                   - {branch}
                 skip_ci: true
                 content: "Hello world!"
                 commit_message: "Preconfigured commit message"
         """
 
-        run_gitlabform(set_file_specific_branch, group_and_project)
+        run_gitlabform(set_file_specific_branch, project)
 
-        commit = gitlab.get_last_commit(group_and_project, branch)
-        assert commit["message"] == "Preconfigured commit message [skip ci]"
+        branch = project.branches.get(branch)
+        assert branch.commit["message"] == "Preconfigured commit message [skip ci]"
 
-    def test__set_file_protected_branches(self, gitlab, group_and_project, branch):
+    def test__set_file_protected_branches(self, project, branch):
         test_config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               {branch}:
                 protected: true
                 push_access_level: {AccessLevel.MAINTAINER.value}
                 merge_access_level: {AccessLevel.MAINTAINER.value}
                 unprotect_access_level: {AccessLevel.MAINTAINER.value}
             files:
@@ -194,38 +191,36 @@
                 overwrite: true
                 branches:
                   - {branch}
                 skip_ci: true
                 content: foobar
         """
 
-        run_gitlabform(test_config, group_and_project)
+        run_gitlabform(test_config, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, branch, "anyfile1")
-        assert file_content == "foobar"
+        project_file = project.files.get(ref=branch, file_path="anyfile1")
+        assert project_file.decode().decode("utf-8") == "foobar"
 
         (
             push_access_levels,
             merge_access_levels,
             push_access_user_ids,
             merge_access_user_ids,
             unprotect_access_level,
-        ) = gitlab.get_only_branch_access_levels(group_and_project, branch)
+        ) = get_only_branch_access_levels(project, branch)
         assert push_access_levels == [AccessLevel.MAINTAINER.value]
         assert merge_access_levels == [AccessLevel.MAINTAINER.value]
         assert push_access_user_ids == []
         assert merge_access_user_ids == []
         assert unprotect_access_level is AccessLevel.MAINTAINER.value
 
-    def test__set_file_protected_branches_not_all_levels(
-        self, gitlab, group_and_project, branch
-    ):
+    def test__set_file_protected_branches_not_all_levels(self, project, branch):
         test_config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 branches:
                   {branch}:
                     protected: true
                     # use a level that will require unprotecting the branch
                     # to change the file value
                     push_access_level: {AccessLevel.MAINTAINER.value}
                     merge_access_level: {AccessLevel.MAINTAINER.value}
@@ -233,83 +228,88 @@
                   anyfile2:
                     overwrite: true
                     branches:
                       - {branch}
                     content: barfoo
             """
 
-        run_gitlabform(test_config, group_and_project)
+        run_gitlabform(test_config, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, branch, "anyfile2")
-        assert file_content == "barfoo"
+        project_file = project.files.get(ref=branch, file_path="anyfile2")
+        assert project_file.decode().decode("utf-8") == "barfoo"
 
         (
             push_access_levels,
             merge_access_levels,
             push_access_user_ids,
             merge_access_user_ids,
             unprotect_access_level,
-        ) = gitlab.get_only_branch_access_levels(group_and_project, branch)
+        ) = get_only_branch_access_levels(project, branch)
         assert push_access_levels == [AccessLevel.MAINTAINER.value]
         assert merge_access_levels == [AccessLevel.MAINTAINER.value]
         assert push_access_user_ids == []
         assert merge_access_user_ids == []
         # the default value
         # according to https://docs.gitlab.com/ee/api/protected_branches.html#protect-repository-branches
         assert unprotect_access_level is AccessLevel.MAINTAINER.value
 
-    def test__set_file_with_chinese_characters(self, gitlab, group_and_project, branch):
+    def test__set_file_with_chinese_characters(self, project, branch):
         set_file_chinese_characters = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches:
                   - {branch}
                 content: |
                     Hanzi (Traditional): 丕不丈丁
                     Hanzi (Simplified): 丏丅丙两
         """
 
-        run_gitlabform(set_file_chinese_characters, group_and_project)
+        run_gitlabform(set_file_chinese_characters, project)
 
-        file_content = gitlab.get_file(group_and_project, branch, "README.md")
-        assert file_content == "Hanzi (Traditional): 丕不丈丁\nHanzi (Simplified): 丏丅丙两\n"
+        file_content = project.files.get(ref=branch, file_path="README.md")
+        assert (
+            file_content.decode().decode("utf-8")
+            == "Hanzi (Traditional): 丕不丈丁\nHanzi (Simplified): 丏丅丙两\n"
+        )
 
-    def test__set_external_file_with_chinese_characters(
-        self, gitlab, group_and_project, branch, file
-    ):
+    def test__set_external_file_with_chinese_characters(self, project, branch, file):
         set_file_chinese_characters = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches:
                   - {branch}
                 file: file.txt
         """
 
-        run_gitlabform(set_file_chinese_characters, group_and_project)
+        run_gitlabform(set_file_chinese_characters, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, branch, "README.md")
-        assert file_content == "Hanzi (Simplified): 丏丅丙两\nHanzi (Traditional): 丕不丈丁"
+        project_file = project.files.get(ref=branch, file_path="README.md")
+        assert (
+            project_file.decode().decode("utf-8")
+            == "Hanzi (Simplified): 丏丅丙两\nHanzi (Traditional): 丕不丈丁"
+        )
 
-    def test__set_external_file_with_utf8_characters(
-        self, gitlab, group_and_project, branch, file2
-    ):
+    def test__set_external_file_with_utf8_characters(self, project, branch, file2):
         set_file_chinese_characters = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches:
                   - {branch}
                 file: file2.txt
         """
 
-        run_gitlabform(set_file_chinese_characters, group_and_project)
+        run_gitlabform(set_file_chinese_characters, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, branch, "README.md")
-        assert file_content == "LICENSE\n\n“This is a license file”\n"
+        project_file = project.files.get(ref=branch, file_path="README.md")
+        assert (
+            project_file.decode().decode("utf-8")
+            == "LICENSE\n\n“This is a license file”\n"
+        )
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_files_protected.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from tests.acceptance import run_gitlabform, DEFAULT_README
 
 
 class TestFilesProtected:
     # this test should be in a separate class than other test files as it changes too
     # much for a reasonable setup and cleanup using fixtures
-    def test__set_file_protected_branches(
-        self, gitlab, group_and_project, branch, other_branch
-    ):
+    def test__set_file_protected_branches(self, project, branch, other_branch):
         set_file_protected_branches = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             branches:
               main:
                 protected: true
                 push_access_level: maintainer
                 merge_access_level: developer
                 unprotect_access_level: maintainer
               {branch}:
@@ -26,23 +24,26 @@
             files:
               "README.md":
                 overwrite: true
                 branches: protected
                 content: "Content for protected branches only"
         """
 
-        run_gitlabform(set_file_protected_branches, group_and_project)
+        run_gitlabform(set_file_protected_branches, project.path_with_namespace)
 
         for some_branch in [
             "main",  # main branch is protected by default
             other_branch,
         ]:
-            file_content = gitlab.get_file(group_and_project, some_branch, "README.md")
-            assert file_content == "Content for protected branches only"
-            some_branch = gitlab.get_branch(group_and_project, some_branch)
-            assert some_branch["protected"] is True
+            project_file = project.files.get(ref=some_branch, file_path="README.md")
+            assert (
+                project_file.decode().decode("utf-8")
+                == "Content for protected branches only"
+            )
+            some_branch = project.branches.get(some_branch)
+            assert some_branch.protected is True
 
         for some_branch in [branch]:
-            file_content = gitlab.get_file(group_and_project, some_branch, "README.md")
-            assert file_content == DEFAULT_README
-            some_branch = gitlab.get_branch(group_and_project, some_branch)
-            assert some_branch["protected"] is False
+            project_file = project.files.get(ref=some_branch, file_path="README.md")
+            assert project_file.decode().decode("utf-8") == DEFAULT_README
+            some_branch = project.branches.get(some_branch)
+            assert some_branch.protected is False
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_files_templates.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,86 +13,89 @@
     def fin():
         os.remove("file3.txt")
 
     request.addfinalizer(fin)
 
 
 class TestFilesTemplates:
-    def test__default_variables(self, gitlab, group_and_project):
+    def test__default_variables(self, project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches: all
                 content: |
                   This is a text that contains the default variables: {{{{ group }}}}/{{{{ project }}}}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        file_content = gitlab.get_file(group_and_project, "main", "README.md")
+        project_file = project.files.get(ref="main", file_path="README.md")
         assert (
-            file_content
-            == f"This is a text that contains the default variables: {group_and_project}\n"
+            project_file.decode().decode("utf-8")
+            == f"This is a text that contains the default variables: {project.path_with_namespace}\n"
         )
 
-    def test__custom_variables(self, gitlab, group_and_project):
+    def test__custom_variables(self, project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches: all
                 jinja_env:
                   foo: "fooz"
                   bar: "barz"
                 content: |
                   This is a text that contains custom variables: {{{{ foo }}}}, {{{{ bar }}}}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        file_content = gitlab.get_file(group_and_project, "main", "README.md")
+        project_file = project.files.get(ref="main", file_path="README.md")
         assert (
-            file_content
+            project_file.decode().decode("utf-8")
             == "This is a text that contains custom variables: fooz, barz\n"
         )
 
-    def test__trailing_new_lines(self, gitlab, group_and_project, file3):
+    def test__trailing_new_lines(self, project, file3):
         set_file_chinese_characters = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches: all
                 file: file3.txt
         """
 
-        run_gitlabform(set_file_chinese_characters, group_and_project)
+        run_gitlabform(set_file_chinese_characters, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, "main", "README.md")
-        assert file_content == f"{group_and_project}\n\n"
+        project_file = project.files.get(ref="main", file_path="README.md")
+        assert (
+            project_file.decode().decode("utf-8")
+            == f"{project.path_with_namespace}\n\n"
+        )
 
-    def test__disabled_templating(self, gitlab, group_and_project):
+    def test__disabled_templating(self, project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             files:
               "README.md":
                 overwrite: true
                 branches: all
                 template: no
                 content: |
                   This is a text containing literals: {{{{ group }}}}/{{{{ project }}}}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project.path_with_namespace)
 
-        file_content = gitlab.get_file(group_and_project, "main", "README.md")
+        project_file = project.files.get(ref="main", file_path="README.md")
         assert (
-            file_content
+            project_file.decode().decode("utf-8")
             == "This is a text containing literals: {{ group }}/{{ project }}\n"
         )
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_group_badges.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestGroupBadges:
-    def test__badges_add(self, gitlab, group):
+    def test__badges_add(self, group):
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 link_url: "https://gitlab.example.com/%{{project_path}}/-/commits/%{{default_branch}}/foo"
                 image_url: "https://gitlab.example.com/%{{project_path}}/badges/%{{default_branch}}/pipeline.svg"
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 1
-        assert badges[0]["name"] == "Group Badge"
+        assert badges[0].name == "Group Badge"
 
-    def test__badges_delete(self, gitlab, group):
+    def test__badges_delete(self, group):
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 link_url: "https://gitlab.example.com/%{{project_path}}/-/commits/%{{default_branch}}/foo"
                 image_url: "https://gitlab.example.com/%{{project_path}}/badges/%{{default_branch}}/pipeline.svg"
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 1
-        assert badges[0]["name"] == "Group Badge"
+        assert badges[0].name == "Group Badge"
 
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 delete: true
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 0
 
-    def test__badges_update(self, gitlab, group):
+    def test__badges_update(self, group):
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 link_url: "https://gitlab.example.com/foo"
                 image_url: "https://gitlab.example.com/pipeline.svg"
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 1
-        assert badges[0]["link_url"].endswith("foo")
+        assert badges[0].link_url.endswith("foo")
 
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 link_url: "https://gitlab.example.com/bar"
                 image_url: "https://gitlab.example.com/pipeline.svg"
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 1
-        assert badges[0]["link_url"].endswith("bar")
+        assert badges[0].link_url.endswith("bar")
 
-    def test__badges_update_choose_the_right_one(self, gitlab, group):
+    def test__badges_update_choose_the_right_one(self, group):
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               pipeline-status:
                 name: "Group Badge"
                 link_url: "https://gitlab.example.com/first"
                 image_url: "https://gitlab.example.com/first"
               another:
                 name: "Group Badge 2"
                 link_url: "https://gitlab.example.com/second"
                 image_url: "https://gitlab.example.com/second" 
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 2
 
         config = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_badges:
               a_different_key:
                 name: "Group Badge 2"
                 link_url: "https://gitlab.example.com/foobar"
                 image_url: "https://gitlab.example.com/foobar"
               and_also_different_than_before:
                 name: "Group Badge"
                 delete: true
         """
         run_gitlabform(config, group)
 
-        badges = gitlab.get_group_badges(group)
+        badges = group.badges.list()
         assert len(badges) == 1
 
         for badge in badges:
-            if badge["name"] == "Group Badge 2":
-                assert badge["link_url"].endswith("foobar")
-                assert badge["image_url"].endswith("foobar")
+            if badge.name == "Group Badge 2":
+                assert badge.link_url.endswith("foobar")
+                assert badge.image_url.endswith("foobar")
             else:
-                assert not badge["link_url"].endswith("foobar")
-                assert not badge["image_url"].endswith("foobar")
+                assert not badge.link_url.endswith("foobar")
+                assert not badge.image_url.endswith("foobar")
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_group_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from tests.acceptance import run_gitlabform
 
 
 class TestGroupSettings:
-    def test__edit_settings(self, gitlab, group):
-        settings = gitlab.get_group_settings(group)
-        assert settings["description"] != "foobar"
+    def test__edit_settings(self, gl, group):
+        assert group.description != "foobar"
 
         edit_group_settings = f"""
         projects_and_groups:
-          {group}/*:
+          {group.full_path}/*:
             group_settings:
               description: foobar
         """
 
         run_gitlabform(edit_group_settings, group)
 
-        settings = gitlab.get_group_settings(group)
-        assert settings["visibility"] == "internal"
+        group = gl.groups.get(group.id)
+        assert group.visibility == "internal"
 
-    def test__no_edit_needed(self, gitlab, group):
-        settings = gitlab.get_group_settings(group)
-        current_value = settings["path"]
+    def test__no_edit_needed(self, gl, group):
+        current_value = group.path
 
         edit_group_settings = f"""
             projects_and_groups:
-              {group}/*:
+              {group.full_path}/*:
                 group_settings:
                   path: {current_value}
             """
 
         run_gitlabform(edit_group_settings, group)
 
-        settings = gitlab.get_group_settings(group)
-        assert settings["path"] == current_value
+        group = gl.groups.get(group.id)
+        assert group.path == current_value
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_group_variables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 from tests.acceptance import run_gitlabform
 
 
 class TestGroupVariables:
-    def test__single_variable(self, gitlab, group_for_function):
+    def test__single_variable(self, group_for_function):
         config_single_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
         """
 
         run_gitlabform(config_single_variable, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
+        variables = group_for_function.variables.list()
         assert len(variables) == 1
 
-    def test__delete_variable(self, gitlab, group_for_function):
+    def test__delete_variable(self, group_for_function):
         config_single_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
         """
 
         run_gitlabform(config_single_variable, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
+        variables = group_for_function.variables.list()
         assert len(variables) == 1
-        assert variables[0]["value"] == "123"
+        assert variables[0].value == "123"
 
         config_delete_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
                 delete: true
         """
 
         run_gitlabform(config_delete_variable, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
+        variables = group_for_function.variables.list()
         assert len(variables) == 0
 
-    def test__reset_single_variable(self, gitlab, group_for_function):
+    def test__reset_single_variable(self, group_for_function):
         config_single_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
         """
 
         run_gitlabform(config_single_variable, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
+        variables = group_for_function.variables.list()
         assert len(variables) == 1
-        assert variables[0]["value"] == "123"
+        assert variables[0].value == "123"
 
         config_single_variable2 = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123456
         """
 
         run_gitlabform(config_single_variable2, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
+        variables = group_for_function.variables.list()
         assert len(variables) == 1
-        assert variables[0]["value"] == "123456"
+        assert variables[0].value == "123456"
 
-    def test__more_variables(self, gitlab, group_for_function):
+    def test__more_variables(self, group_for_function):
         config_more_variables = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123456
               bar:
                 key: BAR
                 value: bleble
         """
 
         run_gitlabform(config_more_variables, group_for_function)
 
-        variables = gitlab.get_group_variables(group_for_function)
-        variables_keys = {variable["key"] for variable in variables}
+        variables = group_for_function.variables.list()
+        variables_keys = {variable.key for variable in variables}
         assert len(variables) == 2
         assert variables_keys == {"FOO", "BAR"}
 
-    def test__masked_variables(self, gitlab, group_for_function):
+    def test__masked_variables(self, group_for_function):
         masked_variables = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 # https://docs.gitlab.com/ee/ci/variables/#masked-variable-requirements
                 value: 12345678
                 masked: true
         """
 
         run_gitlabform(masked_variables, group_for_function)
 
-        variable = gitlab.get_group_variable_object(group_for_function, "FOO")
-        assert variable["value"] == "12345678"
-        assert variable["masked"]
+        variable = group_for_function.variables.get("FOO")
+        assert variable.value == "12345678"
+        assert variable.masked
 
-    def test__protected_variables(self, gitlab, group_for_function):
+    def test__protected_variables(self, group_for_function):
         protected_variables = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
                 protected: true
         """
 
         run_gitlabform(protected_variables, group_for_function)
 
-        variable = gitlab.get_group_variable_object(group_for_function, "FOO")
-        assert variable["value"] == "123"
-        assert variable["protected"]
+        variable = group_for_function.variables.get("FOO")
+        assert variable.value == "123"
+        assert variable.protected
 
-    def test__protected_change_variables(self, gitlab, group_for_function):
+    def test__protected_change_variables(self, group_for_function):
         config_single_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
         """
 
         run_gitlabform(config_single_variable, group_for_function)
 
-        variable = gitlab.get_group_variable_object(group_for_function, "FOO")
-        assert variable["value"] == "123"
-        assert variable["protected"] is False
+        variable = group_for_function.variables.get("FOO")
+        assert variable.value == "123"
+        assert variable.protected is False
 
         protected_variables = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: FOO
                 value: 123
                 protected: true
         """
 
         run_gitlabform(protected_variables, group_for_function)
 
-        variable = gitlab.get_group_variable_object(group_for_function, "FOO")
-        assert variable["value"] == "123"
-        assert variable["protected"] is True
+        variable = group_for_function.variables.get("FOO")
+        assert variable.value == "123"
+        assert variable.protected is True
 
-    def test__not_masked_and_not_protected_variable(self, gitlab, group_for_function):
+    def test__not_masked_and_not_protected_variable(self, group_for_function):
         config_single_variable = f"""
         projects_and_groups:
-          {group_for_function}/*:
+          {group_for_function.full_path}/*:
             group_variables:
               foo:
                 key: DOUBLE_NOT
                 value: 123
                 masked: false
                 protected: false
         """
 
         run_gitlabform(config_single_variable, group_for_function)
 
-        variable = gitlab.get_group_variable_object(group_for_function, "DOUBLE_NOT")
-        assert variable["masked"] is False
-        assert variable["protected"] is False
+        variable = group_for_function.variables.get("DOUBLE_NOT")
+        assert variable.masked is False
+        assert variable.protected is False
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_integrations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import pytest
 
-from gitlabform.gitlab.core import NotFoundException
-from tests.acceptance import run_gitlabform
+from gitlab import GitlabGetError
+from tests.acceptance import allowed_codes, run_gitlabform
 
 
 @pytest.fixture(scope="function")
-def integrations(request, gitlab, group_and_project):
+def integrations(project):
     integrations = ["asana", "slack", "redmine", "jira", "mattermost"]
 
-    def fin():
-        # disable test integrations
-        for integration in integrations:
-            gitlab.delete_integration(group_and_project, integration)
+    yield integrations
 
-    request.addfinalizer(fin)
-    return integrations  # provide fixture value
+    # disable test integrations
+    for integration in integrations:
+        with allowed_codes(404):
+            project.integrations.delete(integration)
 
 
 class TestIntegrations:
     # we use "other_project" here on purpose because if we would reuse the "project"
     # then we could end up with running this test after another, and a integration created
     # and then deleted is a different entity in GitLab than a never created one (!).
     # the first one exists but has "active" field set to False, the other throws 404
-    def test__if_they_are_not_set_by_default(self, gitlab, group, other_project):
-        group_and_project = f"{group}/{other_project}"
-
+    def test__if_they_are_not_set_by_default(self, other_project):
         for integration_name in ["asana", "slack", "redmine", "jira"]:
-            with pytest.raises(NotFoundException):
-                gitlab.get_integration(group_and_project, integration_name)
+            with pytest.raises(GitlabGetError):
+                other_project.integrations.get(integration_name)
 
-    def test__if_delete_works(self, gitlab, group_and_project):
+    def test__if_delete_works(self, project):
         config_integrations = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 url: http://foo.bar.com
                 username: foo
                 password: bar
                 active: true
                 commit_events: true
@@ -49,230 +46,226 @@
               redmine:
                 new_issue_url: http://foo.bar.com
                 project_url: http://foo.bar.com
                 issues_url: http://foo.bar.com
                 push_events: true
         """
 
-        run_gitlabform(config_integrations, group_and_project)
+        run_gitlabform(config_integrations, project)
 
         for integration_name in ["jira", "asana", "slack", "redmine"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
-            assert integration["active"] is True
+            integration = project.integrations.get(integration_name)
+            assert integration.active is True
 
         config_integrations_delete = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 delete: true
               slack:
                 delete: true
         """
 
-        run_gitlabform(config_integrations_delete, group_and_project)
+        run_gitlabform(config_integrations_delete, project)
 
         for integration_name in ["jira", "slack"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
-            assert integration["active"] is False
+            integration = project.integrations.get(integration_name)
+            assert integration.active is False
 
-    def test__if_push_events_true_works(self, gitlab, group_and_project):
+    def test__if_push_events_true_works(self, project):
         config_integration_push_events_true = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               asana:
                 api_key: foo
                 push_events: true
               slack:
                 webhook: http://foo.bar.com
                 push_events: true
               redmine:
                 new_issue_url: http://foo.bar.com
                 project_url: http://foo.bar.com
                 issues_url: http://foo.bar.com
                 push_events: true
         """
 
-        run_gitlabform(config_integration_push_events_true, group_and_project)
+        run_gitlabform(config_integration_push_events_true, project)
 
         integrations = []
         for integration_name in ["asana", "slack", "redmine"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
+            integration = project.integrations.get(integration_name)
             integrations.append(integration)
 
-        assert all([integration["active"] for integration in integrations]) is True
-        assert all([integration["push_events"] for integration in integrations]) is True
+        assert all([integration.active for integration in integrations]) is True
+        assert all([integration.push_events for integration in integrations]) is True
 
-    def test__if_push_events_false_works(self, gitlab, group_and_project):
+    def test__if_push_events_false_works(self, project):
         config_integration_push_events_false = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               asana:
                 api_key: foo
                 push_events: false # changed
               slack:
                 webhook: http://foo.bar.com
                 push_events: false # changed
               redmine:
                 new_issue_url: http://foo.bar.com
                 project_url: http://foo.bar.com
                 issues_url: http://foo.bar.com
                 push_events: false # changed
         """
 
-        run_gitlabform(config_integration_push_events_false, group_and_project)
+        run_gitlabform(config_integration_push_events_false, project)
 
         integrations = []
         for integration_name in ["asana", "slack", "redmine"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
+            integration = project.integrations.get(integration_name)
             integrations.append(integration)
 
-        assert all([integration["active"] for integration in integrations]) is True
-        assert (
-            all([integration["push_events"] for integration in integrations]) is False
-        )
+        assert all([integration.active for integration in integrations]) is True
+        assert all([integration.push_events for integration in integrations]) is False
 
-    def test__if_push_events_change_works(self, gitlab, group_and_project):
+    def test__if_push_events_change_works(self, project):
         config_integration_push_events_true = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               asana:
                 api_key: foo
                 push_events: true
               slack:
                 webhook: http://foo.bar.com
                 push_events: true
               redmine:
                 new_issue_url: http://foo.bar.com
                 project_url: http://foo.bar.com
                 issues_url: http://foo.bar.com
                 push_events: true
         """
 
-        run_gitlabform(config_integration_push_events_true, group_and_project)
+        run_gitlabform(config_integration_push_events_true, project)
 
         integrations = []
         for integration_name in ["asana", "slack", "redmine"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
+            integration = project.integrations.get(integration_name)
             integrations.append(integration)
 
-        assert all([integration["active"] for integration in integrations]) is True
-        assert all([integration["push_events"] for integration in integrations]) is True
+        assert all([integration.active for integration in integrations]) is True
+        assert all([integration.push_events for integration in integrations]) is True
 
         config_integration_push_events_false = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               asana:
                 api_key: foo
                 push_events: false # changed
               slack:
                 webhook: http://foo.bar.com
                 push_events: false # changed
               redmine:
                 new_issue_url: http://foo.bar.com
                 project_url: http://foo.bar.com
                 issues_url: http://foo.bar.com
                 push_events: false # changed
         """
 
-        run_gitlabform(config_integration_push_events_false, group_and_project)
+        run_gitlabform(config_integration_push_events_false, project)
 
         integrations = []
         for integration_name in ["asana", "slack", "redmine"]:
-            integration = gitlab.get_integration(group_and_project, integration_name)
+            integration = project.integrations.get(integration_name)
             integrations.append(integration)
 
-        assert all([integration["active"] for integration in integrations]) is True
-        assert (
-            all([integration["push_events"] for integration in integrations]) is False
-        )
+        assert all([integration.active for integration in integrations]) is True
+        assert all([integration.push_events for integration in integrations]) is False
 
-    def test__if_jira_commit_events_true_works(self, gitlab, group_and_project):
+    def test__if_jira_commit_events_true_works(self, project):
         config_integration_jira_commit_events_true = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 url: http://foo.bar.com
                 username: foo
                 password: bar
                 active: true
                 commit_events: true
         """
 
-        run_gitlabform(config_integration_jira_commit_events_true, group_and_project)
+        run_gitlabform(config_integration_jira_commit_events_true, project)
 
-        integration = gitlab.get_integration(group_and_project, "jira")
-        assert integration["active"] is True
-        assert integration["commit_events"] is True
+        integration = project.integrations.get("jira")
+        assert integration.active is True
+        assert integration.commit_events is True
 
-    def test__if_jira_commit_events_false_works(self, gitlab, group_and_project):
+    def test__if_jira_commit_events_false_works(self, project):
         config_integration_jira_commit_events_false = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 url: http://foo.bar.com
                 username: foo
                 password: bar
                 active: true
                 commit_events: false
         """
 
-        run_gitlabform(config_integration_jira_commit_events_false, group_and_project)
+        run_gitlabform(config_integration_jira_commit_events_false, project)
 
-        integration = gitlab.get_integration(group_and_project, "jira")
-        assert integration["active"] is True
-        assert integration["commit_events"] is False
+        integration = project.integrations.get("jira")
+        assert integration.active is True
+        assert integration.commit_events is False
 
-    def test__if_change_works(self, gitlab, group_and_project):
+    def test__if_change_works(self, project):
         config_integration_jira_commit_events_true = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 url: http://foo.bar.com
                 username: foo
                 password: bar
                 active: true
                 commit_events: true
         """
 
-        run_gitlabform(config_integration_jira_commit_events_true, group_and_project)
+        run_gitlabform(config_integration_jira_commit_events_true, project)
 
-        integration = gitlab.get_integration(group_and_project, "jira")
-        assert integration["active"] is True
-        assert integration["commit_events"] is True
+        integration = project.integrations.get("jira")
+        assert integration.active is True
+        assert integration.commit_events is True
 
         config_integration_jira_commit_events_false = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               jira:
                 url: http://foo.bar.com
                 username: foo
                 password: bar
                 active: true
                 commit_events: false
         """
 
-        run_gitlabform(config_integration_jira_commit_events_false, group_and_project)
+        run_gitlabform(config_integration_jira_commit_events_false, project)
 
-        integration = gitlab.get_integration(group_and_project, "jira")
-        assert integration["active"] is True
-        assert integration["commit_events"] is False
+        integration = project.integrations.get("jira")
+        assert integration.active is True
+        assert integration.commit_events is False
 
-    def test__mattermost_confidential_issues_events(self, gitlab, group_and_project):
+    def test__mattermost_confidential_issues_events(self, project):
         config_integration_mattermost_confidential_issues_events = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             integrations:
               mattermost:
                 active: true
                 webhook: https://mattermost.com/hooks/xxx
                 username: gitlab
                 merge_requests_events: true
                 merge_request_channel: "merge-requests"
@@ -284,12 +277,12 @@
                 confidential_note_events: false
                 pipeline_events: false
                 wiki_page_events: false
                 branches_to_be_notified: "all"
         """
 
         run_gitlabform(
-            config_integration_mattermost_confidential_issues_events, group_and_project
+            config_integration_mattermost_confidential_issues_events, project
         )
 
-        integration = gitlab.get_integration(group_and_project, "mattermost")
-        assert integration["confidential_issues_events"] is False
+        integration = project.integrations.get("mattermost")
+        assert integration.confidential_issues_events is False
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_members.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_members.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 from gitlabform.gitlab import AccessLevel
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestMembers:
-    def test__add_user(self, gitlab, group_and_project, three_members, outsider_user):
-        members_before = gitlab.get_project_members(group_and_project)
+    def test__add_user(self, project, three_members, outsider_user):
+        members_before = project.members.list()
         assert len(members_before) > 0
 
-        members_usernames_before = [member["username"] for member in members_before]
-        assert outsider_user not in members_usernames_before
+        members_usernames_before = [member.username for member in members_before]
+        assert outsider_user.username not in members_usernames_before
 
         add_users = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             members:
               users:
-                {outsider_user}: # new user
+                {outsider_user.username}: # new user
                   access_level: {AccessLevel.DEVELOPER.value}
         """
 
-        run_gitlabform(add_users, group_and_project)
+        run_gitlabform(add_users, project)
 
-        members = gitlab.get_project_members(group_and_project)
+        members = project.members.list()
         assert len(members) == len(members_before) + 1
 
-        members_usernames = [member["username"] for member in members]
-        assert outsider_user in members_usernames
+        members_usernames = [member.username for member in members]
+        assert outsider_user.username in members_usernames
 
-    def test__no_groups_and_no_users(self, gitlab, group_and_project):
+    def test__no_groups_and_no_users(self, project):
         config_with_error = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             members:
               # there should be a sub-key 'users' here, not directly a user
               some_user1: 
                 access_level: {AccessLevel.DEVELOPER.value}
         """
 
         with pytest.raises(SystemExit):
-            run_gitlabform(config_with_error, group_and_project)
+            run_gitlabform(config_with_error, project)
 
     def test__add_user_with_access_level_names(
-        self, gitlab, group_and_project, three_members, outsider_user
+        self, project, three_members, outsider_user
     ):
-        members_before = gitlab.get_project_members(group_and_project)
+        members_before = project.members.list()
         assert len(members_before) > 0
 
-        members_usernames_before = [member["username"] for member in members_before]
-        assert outsider_user not in members_usernames_before
+        members_usernames_before = [member.username for member in members_before]
+        assert outsider_user.username not in members_usernames_before
 
         add_users = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 members:
                   users:
-                    {outsider_user}: # new user
+                    {outsider_user.username}: # new user
                       access_level: maintainer
             """
 
-        run_gitlabform(add_users, group_and_project)
+        run_gitlabform(add_users, project)
 
-        members = gitlab.get_project_members(group_and_project)
+        members = project.members.list()
         assert len(members) == len(members_usernames_before) + 1
 
-        members_usernames = [member["username"] for member in members]
-        assert outsider_user in members_usernames
+        members_usernames = [member.username for member in members]
+        assert outsider_user.username in members_usernames
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_members_add_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,63 +3,61 @@
 from gitlabform.gitlab import AccessLevel
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 @pytest.fixture(scope="class")
-def two_members_in_other_group(gitlab, other_group, make_user):
+def two_members_in_other_group(other_group, make_user):
     outsider_user1 = make_user(add_to_project=False)
     outsider_user2 = make_user(add_to_project=False)
 
-    gitlab.add_member_to_group(
-        other_group, outsider_user1.name, AccessLevel.OWNER.value
+    other_group.members.create(
+        {"access_level": AccessLevel.OWNER.value, "user_id": outsider_user1.id}
     )
-    gitlab.add_member_to_group(
-        other_group, outsider_user2.name, AccessLevel.DEVELOPER.value
+    other_group.members.create(
+        {"access_level": AccessLevel.DEVELOPER.value, "user_id": outsider_user2.id}
     )
 
-    yield [outsider_user1.name, outsider_user2.name]
+    yield [outsider_user1, outsider_user2]
 
 
 class TestMembersAddGroup:
     # this test should be in a separate class than other test files as it changes too
     # much for a reasonable setup and cleanup using fixtures
     def test__add_group(
         self,
-        gitlab,
-        group_and_project,
+        gl,
+        project,
         three_members,
         other_group,
         two_members_in_other_group,
     ):
-        no_of_members_before = len(gitlab.get_project_members(group_and_project))
-        no_of_members_of_other_group = len(gitlab.get_group_members(other_group))
+        no_of_members_before = len(project.members.list())
+        no_of_members_of_other_group = len(project.members.list())
 
-        no_of_groups_shared_before = len(
-            gitlab.get_shared_with_groups(group_and_project)
-        )
+        no_of_groups_shared_before = len(project.shared_with_groups)
         assert no_of_groups_shared_before == 0
 
         add_group = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             members:
               groups:
-                {other_group}:
+                {other_group.full_path}:
                   group_access: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(add_group, group_and_project)
+        run_gitlabform(add_group, project)
 
-        members = gitlab.get_project_members(group_and_project, all=True)
+        members = project.members_all.list()
 
         assert len(members) == no_of_members_before + no_of_members_of_other_group
 
         for member in members:
-            if member["username"] in two_members_in_other_group:
+            if member.username in two_members_in_other_group:
                 # "group_access" is the *maximum* access level, see
                 # https://docs.gitlab.com/ee/user/project/members/share_project_with_groups.html#maximum-access-level
-                assert member["access_level"] <= AccessLevel.MAINTAINER.value
+                assert member.access_level <= AccessLevel.MAINTAINER.value
 
-        no_of_groups_shared = len(gitlab.get_shared_with_groups(group_and_project))
+        no_of_groups_shared = len(gl.projects.get(project.id).shared_with_groups)
         assert no_of_groups_shared == 1
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_resource_groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 from tests.acceptance import run_gitlabform
 import time
 
 
 @pytest.fixture(scope="function")
-def add_gitlab_ci_config(group_and_project):
+def add_gitlab_ci_config(project):
     add_gitlab_ci_config = f"""
     projects_and_groups:
-      {group_and_project}:
+      {project.path_with_namespace}:
         files:
           ".gitlab-ci.yml":
             branches: 
               - main
             overwrite: true
             content: |
               stages:
@@ -20,31 +20,27 @@
               deploy:
                 stage: deploy
                 script:
                   - echo deploy
                 environment: production
                 resource_group: production
         """
-    run_gitlabform(add_gitlab_ci_config, group_and_project)
-    return group_and_project
+    run_gitlabform(add_gitlab_ci_config, project)
+    return project
 
 
 class TestResourceGroups:
-    def test__update_resource_group_process_mode(
-        self, gitlab, group_and_project, add_gitlab_ci_config
-    ):
+    def test__update_resource_group_process_mode(self, project, add_gitlab_ci_config):
         update_resource_group_config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             resource_groups:
               production:
                 process_mode: newest_first
             """
 
         time.sleep(5)
-        run_gitlabform(update_resource_group_config, group_and_project)
+        run_gitlabform(update_resource_group_config, project)
 
-        resource_group = gitlab.get_specific_resource_group(
-            group_and_project, "production"
-        )
-        assert resource_group["key"] == "production"
-        assert resource_group["process_mode"] == "newest_first"
+        resource_group = project.resource_groups.get("production")
+        assert resource_group.key == "production"
+        assert resource_group.process_mode == "newest_first"
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_running.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_running.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,49 +2,46 @@
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestRunning:
     # noinspection PyPep8Naming
-    def test__ALL(self, gitlab, group, project, other_project):
+    def test__ALL(self, gl, project, other_project):
         config = f"""
         projects_and_groups:
           '*':
             project_settings:
               request_access_enabled: true
         """
 
         run_gitlabform(config, "ALL")
 
-        project = gitlab.get_project(f"{group}/{project}")
-        assert project["request_access_enabled"] is True
+        project = gl.projects.get(project.id)
+        assert project.request_access_enabled is True
 
-        other_project = gitlab.get_project(f"{group}/{other_project}")
-        assert other_project["request_access_enabled"] is True
+        other_project = gl.projects.get(other_project.id)
+        assert other_project.request_access_enabled is True
 
     # noinspection PyPep8Naming
-    def test__ALL_DEFINED(self, gitlab, group, project, other_project):
-        group_and_project = f"{group}/{project}"
-
+    def test__ALL_DEFINED(self, gl, project, other_project):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             project_settings:
               suggestion_commit_message: 'foobar'
         """
 
         run_gitlabform(config, "ALL_DEFINED")
 
-        project = gitlab.get_project(group_and_project)
-        assert project["suggestion_commit_message"] == "foobar"
+        project = gl.projects.get(project.id)
+        assert project.suggestion_commit_message == "foobar"
 
-        group_and_other_project = f"{group}/{other_project}"
-        project = gitlab.get_project(group_and_other_project)
-        assert project["suggestion_commit_message"] != "foobar"
+        project = gl.projects.get(other_project.id)
+        assert project.suggestion_commit_message != "foobar"
 
         config = f"""
         projects_and_groups:
           non/existent_project:
             project_settings:
               suggestion_commit_message: 'foobar'
         """
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_schedules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,217 +1,217 @@
 import pytest
 
 
 from tests.acceptance import run_gitlabform
 
 
 @pytest.fixture(scope="class")
-def schedules(gitlab, group_and_project):
+def schedules(project):
     another_branch = "scheduled/new-feature"
-    gitlab.create_branch(group_and_project, another_branch, "main")
+    project.branches.create({"branch": another_branch, "ref": "main"})
 
     # fmt: off
     schedules = [
-        ("Existing schedule", "main", "0 * * * *", {"active": "true"}),
-        ("Existing schedule with vars", "main", "30 * * * *", {}),
-        ("Existing schedule to replace", "main", "30 1 * * *", {}),
-        ("Existing schedule to replace", another_branch, "30 2 * * *", {}),
+        ("Existing schedule", "main", "0 * * * *", True),
+        ("Existing schedule with vars", "main", "30 * * * *", False),
+        ("Existing schedule to replace", "main", "30 1 * * *", False),
+        ("Existing schedule to replace", another_branch, "30 2 * * *", False),
     ]
     # fmt: on
 
-    for schedule in schedules:
-        gitlab.create_pipeline_schedule(
-            group_and_project,
-            *schedule,
-        )
+    gitlab_schedules = []
 
-    redundant_schedule = gitlab.create_pipeline_schedule(
-        group_and_project,
-        "Redundant schedule",
-        "main",
-        "0 * * * *",
-    )
-    gitlab.create_pipeline_schedule_variable(
-        group_and_project, redundant_schedule["id"], "test_variable", "test_value"
+    for schedule in schedules:
+        gitlab_schedule = project.pipelineschedules.create(
+            {
+                "description": schedule[0],
+                "ref": schedule[1],
+                "cron": schedule[2],
+                "active": schedule[3],
+            }
+        )
+        gitlab_schedules.append(gitlab_schedule)
+
+    redundant_schedule = project.pipelineschedules.create(
+        {
+            "description": "Redundant schedule",
+            "ref": "main",
+            "cron": "0 * * * *",
+        }
     )
+    redundant_schedule.variables.create({"key": "test_variable", "value": "test_value"})
 
-    schedules.append(("Redundant schedule", "main", "0 * * * *"))
+    schedules.append(redundant_schedule)
 
     return schedules  # provide fixture value
 
 
 class TestSchedules:
-    def test__add_new_schedule(self, gitlab, group_and_project, schedules):
+    def test__add_new_schedule(self, project, schedules):
         add_schedule = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "New schedule":
                 ref: main
                 cron: "0 * * * *"
                 cron_timezone: "London"
                 active: true
         """
 
-        run_gitlabform(add_schedule, group_and_project)
+        run_gitlabform(add_schedule, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
-            gitlab, group_and_project, "New schedule"
+            project, "New schedule"
         )
         assert schedule is not None
-        assert schedule["description"] == "New schedule"
-        assert schedule["ref"] == "main"
-        assert schedule["cron"] == "0 * * * *"
-        assert schedule["cron_timezone"] == "London"
-        assert schedule["active"] is True
+        assert schedule.description == "New schedule"
+        assert schedule.ref == "main"
+        assert schedule.cron == "0 * * * *"
+        assert schedule.cron_timezone == "London"
+        assert schedule.active is True
 
-    def test__add_new_schedule_with_mandatory_fields_only(
-        self, gitlab, group_and_project, schedules
-    ):
+    def test__add_new_schedule_with_mandatory_fields_only(self, project, schedules):
         add_schedule_mandatory_fields_only = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "New schedule with mandatory fields":
                 ref: main
                 cron: "30 1 * * *"
         """
 
-        run_gitlabform(add_schedule_mandatory_fields_only, group_and_project)
+        run_gitlabform(add_schedule_mandatory_fields_only, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
-            gitlab, group_and_project, "New schedule with mandatory fields"
+            project, "New schedule with mandatory fields"
         )
         assert schedule is not None
-        assert schedule["description"] == "New schedule with mandatory fields"
-        assert schedule["ref"] == "main"
-        assert schedule["cron"] == "30 1 * * *"
-        assert schedule["cron_timezone"] == "UTC"
-        assert schedule["active"] is True
+        assert schedule.description == "New schedule with mandatory fields"
+        assert schedule.ref == "main"
+        assert schedule.cron == "30 1 * * *"
+        assert schedule.cron_timezone == "UTC"
+        assert schedule.active is True
 
-    def test__set_schedule_variables(self, gitlab, group_and_project, schedules):
+    def test__set_schedule_variables(self, project, schedules):
         add_schedule_with_variables = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "New schedule with variables":
                 ref: main
                 cron: "30 1 * * *"
                 variables:
                     var1:
                         value: value123
                     var2:
                         value: value987
                         variable_type: file
         """
 
-        run_gitlabform(add_schedule_with_variables, group_and_project)
+        run_gitlabform(add_schedule_with_variables, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
-            gitlab, group_and_project, "New schedule with variables"
+            project, "New schedule with variables"
         )
         assert schedule is not None
-        assert schedule["description"] == "New schedule with variables"
-        assert schedule["ref"] == "main"
-        assert schedule["cron"] == "30 1 * * *"
-        assert schedule["cron_timezone"] == "UTC"
-        assert schedule["active"] is True
-        assert schedule["variables"] is not None
-        assert len(schedule["variables"]) == 2
-
-        assert schedule["variables"][0]["variable_type"] == "env_var"
-        assert schedule["variables"][0]["key"] == "var1"
-        assert schedule["variables"][0]["value"] == "value123"
-
-        assert schedule["variables"][1]["variable_type"] == "file"
-        assert schedule["variables"][1]["key"] == "var2"
-        assert schedule["variables"][1]["value"] == "value987"
+        assert schedule.description == "New schedule with variables"
+        assert schedule.ref == "main"
+        assert schedule.cron == "30 1 * * *"
+        assert schedule.cron_timezone == "UTC"
+        assert schedule.active is True
+
+        variables = schedule.attributes["variables"]
+        assert variables is not None
+        assert len(variables) == 2
+
+        assert variables[0]["variable_type"] == "env_var"
+        assert variables[0]["key"] == "var1"
+        assert variables[0]["value"] == "value123"
+
+        assert variables[1]["variable_type"] == "file"
+        assert variables[1]["key"] == "var2"
+        assert variables[1]["value"] == "value987"
 
-    def test__update_existing_schedule(self, gitlab, group_and_project, schedules):
+    def test__update_existing_schedule(self, project, schedules):
         edit_schedule = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "Existing schedule":
                 ref: scheduled/new-feature
                 cron: "0 */4 * * *"
                 cron_timezone: "Stockholm"
                 active: false
         """
 
-        run_gitlabform(edit_schedule, group_and_project)
+        run_gitlabform(edit_schedule, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
-            gitlab, group_and_project, "Existing schedule"
+            project, "Existing schedule"
         )
         assert schedule is not None
-        assert schedule["description"] == "Existing schedule"
-        assert schedule["ref"] == "scheduled/new-feature"
-        assert schedule["cron"] == "0 */4 * * *"
-        assert schedule["cron_timezone"] == "Stockholm"
-        assert schedule["active"] is False
+        assert schedule.description == "Existing schedule"
+        assert schedule.ref == "scheduled/new-feature"
+        assert schedule.cron == "0 */4 * * *"
+        assert schedule.cron_timezone == "Stockholm"
+        assert schedule.active is False
 
-    def test__replace_existing_schedules(self, gitlab, group_and_project, schedules):
+    def test__replace_existing_schedules(self, project, schedules):
         replace_schedules = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "Existing schedule to replace":
                 ref: scheduled/new-feature
                 cron: "0 */3 * * *"
                 cron_timezone: "London"
                 active: true
         """
 
-        run_gitlabform(replace_schedules, group_and_project)
+        run_gitlabform(replace_schedules, project)
 
-        schedules = self.__find_pipeline_schedules_by_description(
-            gitlab, group_and_project, "Existing schedule to replace"
+        existing_schedules = self.__find_pipeline_schedules_by_description(
+            project, "Existing schedule to replace"
         )
-        assert schedules is not None
-        assert len(schedules) == 1
-        assert schedules[0]["description"] == "Existing schedule to replace"
-        assert schedules[0]["ref"] == "scheduled/new-feature"
-        assert schedules[0]["cron"] == "0 */3 * * *"
-        assert schedules[0]["cron_timezone"] == "London"
-        assert schedules[0]["active"] is True
+        assert existing_schedules is not None
+        assert len(existing_schedules) == 1
 
-    def test__delete_schedule(self, gitlab, group_and_project, schedules):
+        schedule = existing_schedules[0]
+        assert schedule.description == "Existing schedule to replace"
+        assert schedule.ref == "scheduled/new-feature"
+        assert schedule.cron == "0 */3 * * *"
+        assert schedule.cron_timezone == "London"
+        assert schedule.active is True
+
+    def test__delete_schedule(self, project, schedules):
         delete_schedule = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             schedules:
               "Redundant schedule":
                 delete: True
         """
 
-        run_gitlabform(delete_schedule, group_and_project)
+        run_gitlabform(delete_schedule, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
-            gitlab, group_and_project, "Redundant schedule"
+            project, "Redundant schedule"
         )
         assert schedule is None
 
-    @staticmethod
+    @classmethod
     def __find_pipeline_schedule_by_description_and_get_first(
-        gitlab, group_and_project, description
+        cls, project, description
     ):
-        for schedule in gitlab.get_all_pipeline_schedules(group_and_project):
-            if schedule["description"] == description:
-                return gitlab.get_pipeline_schedule(group_and_project, schedule["id"])
-        return None
+        try:
+            return cls.__find_pipeline_schedules_by_description(project, description)[0]
+        except IndexError:
+            return None
 
     @staticmethod
-    def __find_pipeline_schedules_by_description(
-        gitlab, group_and_project, description
-    ):
-        return list(
-            map(
-                lambda schedule: gitlab.get_pipeline_schedule(
-                    group_and_project, schedule["id"]
-                ),
-                filter(
-                    lambda schedule: schedule["description"] == description,
-                    gitlab.get_all_pipeline_schedules(group_and_project),
-                ),
-            )
-        )
+    def __find_pipeline_schedules_by_description(project, description):
+        return [
+            project.pipelineschedules.get(schedule.id)
+            for schedule in project.pipelineschedules.list()
+            if schedule.description == description
+        ]
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_tags.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,174 +3,175 @@
 from gitlabform.gitlab import AccessLevel
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 @pytest.fixture(scope="function")
-def tags(request, gitlab, group_and_project):
-    tags = [
+def tags(project):
+    tag_names = [
         "tag1",
         "tag2",
         "tag3",
     ]
-    for tag in tags:
-        gitlab.create_tag(group_and_project, tag, "main")
+    tags = []
+
+    for tag_name in tag_names:
+        tag = project.tags.create({"tag_name": tag_name, "ref": "main"})
+        tags.append(tag)
 
-    def fin():
-        protected_tags = gitlab.get_protected_tags(group_and_project)
-        for protected_tag in protected_tags:
-            gitlab.unprotect_tag(group_and_project, protected_tag["name"])
-        for tag in tags:
-            gitlab.delete_tag(group_and_project, tag)
+    yield tags
 
-    request.addfinalizer(fin)
+    protected_tags = project.protectedtags.list()
+    for protected_tag in protected_tags:
+        protected_tag.delete()
+
+    for tag in tags:
+        tag.delete()
 
 
 class TestTags:
-    def test__protect_single_tag(self, gitlab, group_and_project, tags):
+    def test__protect_single_tag(self, project, tags):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             tags:
               tag1:
                 protected: true
                 create_access_level: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            if tag["name"] == "tag1":
-                assert tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            if tag.name == "tag1":
+                assert tag.protected
             else:
-                assert not tag["protected"]
+                assert not tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 1
-        assert protected_tags[0]["name"] == "tag1"
+        assert protected_tags[0].name == "tag1"
         assert (
-            protected_tags[0]["create_access_levels"][0]["access_level"]
+            protected_tags[0].create_access_levels[0]["access_level"]
             == AccessLevel.MAINTAINER.value
         )
 
-    def test__protect_wildcard_tag(self, gitlab, group_and_project, tags):
+    def test__protect_wildcard_tag(self, project, tags):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             tags:
               "tag*":
                 protected: true
                 create_access_level: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            assert tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            assert tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 1
-        assert protected_tags[0]["name"] == "tag*"
+        assert protected_tags[0].name == "tag*"
         assert (
-            protected_tags[0]["create_access_levels"][0]["access_level"]
+            protected_tags[0].create_access_levels[0]["access_level"]
             == AccessLevel.MAINTAINER.value
         )
 
-    def test__unprotect_the_same_tag(self, gitlab, group_and_project, tags):
+    def test__unprotect_the_same_tag(self, project, tags):
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             tags:
               "tag*":
                 protected: true
                 create_access_level: {AccessLevel.MAINTAINER.value}
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            assert tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            assert tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 1
-        assert protected_tags[0]["name"] == "tag*"
+        assert protected_tags[0].name == "tag*"
         assert (
-            protected_tags[0]["create_access_levels"][0]["access_level"]
+            protected_tags[0].create_access_levels[0]["access_level"]
             == AccessLevel.MAINTAINER.value
         )
 
         config = f"""
         projects_and_groups:
-          {group_and_project}:
+          {project.path_with_namespace}:
             tags:
               "tag*":
                 protected: false
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            assert not tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            assert not tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 0
 
-    def test__protect_single_tag_no_access(self, gitlab, group_and_project, tags):
+    def test__protect_single_tag_no_access(self, project, tags):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 tags:
                   tag1:
                     protected: true
                     create_access_level: {AccessLevel.NO_ACCESS.value}
             """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            if tag["name"] == "tag1":
-                assert tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            if tag.name == "tag1":
+                assert tag.protected
             else:
-                assert not tag["protected"]
+                assert not tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 1
-        assert protected_tags[0]["name"] == "tag1"
+        assert protected_tags[0].name == "tag1"
         assert (
-            protected_tags[0]["create_access_levels"][0]["access_level"]
+            protected_tags[0].create_access_levels[0]["access_level"]
             == AccessLevel.NO_ACCESS.value
         )
 
-    def test__protect_single_tag_with_access_level_names(
-        self, gitlab, group_and_project, tags
-    ):
+    def test__protect_single_tag_with_access_level_names(self, project, tags):
         config = f"""
             projects_and_groups:
-              {group_and_project}:
+              {project.path_with_namespace}:
                 tags:
                   tag1:
                     protected: true
                     create_access_level: maintainer
             """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-        tags = gitlab.get_tags(group_and_project)
-        for tag in tags:
-            if tag["name"] == "tag1":
-                assert tag["protected"]
+        project_tags = project.tags.list()
+        for tag in project_tags:
+            if tag.name == "tag1":
+                assert tag.protected
             else:
-                assert not tag["protected"]
+                assert not tag.protected
 
-        protected_tags = gitlab.get_protected_tags(group_and_project)
+        protected_tags = project.protectedtags.list()
         assert len(protected_tags) == 1
-        assert protected_tags[0]["name"] == "tag1"
+        assert protected_tags[0].name == "tag1"
         assert (
-            protected_tags[0]["create_access_levels"][0]["access_level"]
+            protected_tags[0].create_access_levels[0]["access_level"]
             == AccessLevel.MAINTAINER.value
         )
```

### Comparing `gitlabform-3.5.0/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.6.0/tests/acceptance/standard/test_token_from_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 from tests.acceptance import (
     run_gitlabform,
 )
 
 
 class TestTokenFromConfig:
-    def test__token_no_quotes(self, gitlab, group_and_project, token_from_env_var):
+    def test__token_no_quotes(self, project, token_from_env_var):
         config = f"""
         gitlab:
           token: {token_from_env_var}
           
         projects_and_groups:
           placeholder:
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-    def test__token_single_quotes(self, gitlab, group_and_project, token_from_env_var):
+    def test__token_single_quotes(self, project, token_from_env_var):
         config = f"""
         gitlab:
           token: '{token_from_env_var}'
           
         projects_and_groups:
           placeholder:
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
 
-    def test__token_double_quotes(self, gitlab, group_and_project, token_from_env_var):
+    def test__token_double_quotes(self, project, token_from_env_var):
         config = f"""
         gitlab:
           token: "{token_from_env_var}"
 
         projects_and_groups:
           placeholder:
         """
 
-        run_gitlabform(config, group_and_project)
+        run_gitlabform(config, project)
```

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.6.0/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.6.0/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.6.0/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.6.0/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.6.0/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.6.0/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.6.0/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.6.0/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/test_access_levels.py` & `gitlabform-3.6.0/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.5.0/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.6.0/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

