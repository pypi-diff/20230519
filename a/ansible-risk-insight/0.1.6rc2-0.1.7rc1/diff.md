# Comparing `tmp/ansible-risk-insight-0.1.6rc2.tar.gz` & `tmp/ansible-risk-insight-0.1.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.6rc2.tar", last modified: Fri Apr 28 07:49:26 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.7rc1.tar", last modified: Fri May 19 04:27:07 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.6rc2.tar` & `ansible-risk-insight-0.1.7rc1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.109335 ansible-risk-insight-0.1.6rc2/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.047314 ansible-risk-insight-0.1.6rc2/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.054451 ansible-risk-insight-0.1.6rc2/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.6rc2/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 07:49:26.109140 ansible-risk-insight-0.1.6rc2/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.064592 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-28 07:49:19.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.067284 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.072013 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.072186 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.073875 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    75964 2023-04-28 05:12:53.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    43989 2023-04-28 05:12:52.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.092936 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-04-28 04:49:11.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     3050 2023-04-28 06:29:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-04-28 04:13:42.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.065569 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-28 07:49:26.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-28 07:49:25.000000 ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.6rc2/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.048139 ansible-risk-insight-0.1.6rc2/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.096663 ansible-risk-insight-0.1.6rc2/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.6rc2/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.099954 ansible-risk-insight-0.1.6rc2/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.6rc2/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.6rc2/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.103668 ansible-risk-insight-0.1.6rc2/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.6rc2/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104259 ansible-risk-insight-0.1.6rc2/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104538 ansible-risk-insight-0.1.6rc2/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.104962 ansible-risk-insight-0.1.6rc2/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.6rc2/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.6rc2/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.6rc2/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.6rc2/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-28 07:49:26.109397 ansible-risk-insight-0.1.6rc2/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.6rc2/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.105331 ansible-risk-insight-0.1.6rc2/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.6rc2/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049686 ansible-risk-insight-0.1.6rc2/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049164 ansible-risk-insight-0.1.6rc2/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106230 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049325 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049586 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106668 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.106919 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107426 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.049747 ansible-risk-insight-0.1.6rc2/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.050002 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107667 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.107968 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-28 07:49:26.108771 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.6rc2/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.6rc2/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.434586 ansible-risk-insight-0.1.7rc1/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.353750 ansible-risk-insight-0.1.7rc1/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.361087 ansible-risk-insight-0.1.7rc1/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.7rc1/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-19 04:27:07.434394 ansible-risk-insight-0.1.7rc1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.376534 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      662 2023-05-19 04:27:02.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.385656 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.398935 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.399162 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.401846 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-05-19 01:44:23.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46758 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8612 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2508 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-05-19 01:44:42.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    76012 2023-05-19 01:43:47.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-05-19 01:44:34.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    44597 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8504 2023-05-19 00:55:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.418563 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3036 2023-04-28 09:03:05.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-05-19 01:44:44.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-05-19 01:44:37.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24619 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.378393 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       91 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.354738 ansible-risk-insight-0.1.7rc1/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.422724 ansible-risk-insight-0.1.7rc1/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.425052 ansible-risk-insight-0.1.7rc1/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.7rc1/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.7rc1/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.429698 ansible-risk-insight-0.1.7rc1/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430217 ansible-risk-insight-0.1.7rc1/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430577 ansible-risk-insight-0.1.7rc1/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430869 ansible-risk-insight-0.1.7rc1/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.7rc1/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      993 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-19 04:27:07.434650 ansible-risk-insight-0.1.7rc1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.431234 ansible-risk-insight-0.1.7rc1/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc1/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356301 ansible-risk-insight-0.1.7rc1/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.355609 ansible-risk-insight-0.1.7rc1/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432069 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.355813 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356139 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432447 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432810 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433149 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356389 ansible-risk-insight-0.1.7rc1/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356761 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433457 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433727 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.434037 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.7rc1/tox.ini
```

### Comparing `ansible-risk-insight-0.1.6rc2/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.7rc1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/.github/workflows/test.yml` & `ansible-risk-insight-0.1.7rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/.gitignore` & `ansible-risk-insight-0.1.7rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/CONTRIBUTING.md` & `ansible-risk-insight-0.1.7rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/LICENSE` & `ansible-risk-insight-0.1.7rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/README.md` & `ansible-risk-insight-0.1.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "0.1.6-rc2"
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,15 @@
         target_version = target
         if version:
             target_version = "{}:{}".format(target, version)
         logger.debug("downloading: {}".format("ansible-galaxy collection download '{}' {} -p {}".format(target_version, server_option, output_dir)))
         proc = subprocess.run(
             "ansible-galaxy collection download '{}' {} -p {}".format(target_version, server_option, output_dir),
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         install_msg = proc.stdout
         logger.debug("STDOUT: {}".format(install_msg))
         return install_msg
@@ -551,27 +552,29 @@
     def download_galaxy_collection_from_reqfile(self, requirements, output_dir, source_repository=""):
         server_option = ""
         if source_repository:
             server_option = "--server {}".format(source_repository)
         proc = subprocess.run(
             "ansible-galaxy collection download -r {} {} -p {}".format(requirements, server_option, output_dir),
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         install_msg = proc.stdout
         logger.debug("STDOUT: {}".format(install_msg))
         # return proc.stdout
 
     def install_galaxy_collection_from_targz(self, tarfile, output_dir):
         logger.debug("install collection from {}".format(tarfile))
         proc = subprocess.run(
             "ansible-galaxy collection install {} -p {}".format(tarfile, output_dir),
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         install_msg = proc.stdout
         logger.debug("STDOUT: {}".format(install_msg))
         # return proc.stdout
@@ -585,14 +588,15 @@
                 logger.warning("requirements file not found: {}".format(requirements))
                 return
         logger.debug("install collection from {}".format(requirements))
         src_dir = requirements.replace(requirements_yml, "")
         proc = subprocess.run(
             "cd {} && ansible-galaxy collection install -r {} -p {}".format(src_dir, requirements, output_dir),
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         try:
             proc.check_returncode()
         except Exception as exc:
@@ -621,14 +625,15 @@
                         filename = file
         return is_exist, filename
 
     def install_galaxy_role_from_reqfile(self, file, output_dir):
         proc = subprocess.run(
             "ansible-galaxy role install -r {} -p {}".format(file, output_dir),
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         install_msg = proc.stdout
         logger.debug("STDOUT: {}".format(install_msg))
 
@@ -782,14 +787,15 @@
         # we use cp command here because shutil module is slow,
         # but the behavior of cp command is slightly different between Mac and Linux
         # we use a command like `cp -r <src>/* <dst>/` so the behavior will be the same
         dirs = os.listdir(src)
         proc = subprocess.run(
             f"cp -r {src}/* {dst}/",
             shell=True,
+            stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             text=True,
         )
         # raise if copy failed
         try:
             proc.check_returncode()
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
     return requirements, paths, metadata
 
 
 def install_github_target(target, output_dir):
     proc = subprocess.run(
         "git clone {} {}".format(target, output_dir),
         shell=True,
+        stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         text=True,
     )
     install_msg = proc.stdout
     logger.debug("STDOUT: {}".format(install_msg))
     return proc.stdout
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/findings.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from copy import deepcopy
 from dataclasses import dataclass, field
 import jsonpickle
 from .utils import (
     lock_file,
     unlock_file,
+    remove_lock_file,
 )
 
 
 @dataclass
 class Findings:
     metadata: dict = field(default_factory=dict)
     dependencies: list = field(default_factory=list)
@@ -49,18 +50,21 @@
         f = deepcopy(self)
         # omit report and summary_txt when the findings are saved
         # to reduce unnecessary file write
         f.report = {}
         f.summary_txt = ""
         json_str = jsonpickle.encode(f, make_refs=False)
         if fpath:
-            with open(fpath, "w") as file:
-                lock_file(file)
-                file.write(json_str)
-                unlock_file(file)
+            lock = lock_file(fpath)
+            try:
+                with open(fpath, "w") as file:
+                    file.write(json_str)
+            finally:
+                unlock_file(lock)
+                remove_lock_file(lock)
         return json_str
 
     def save_rule_result(self, fpath=""):
         json_str = jsonpickle.encode(self.report.get("ari_result", {}), make_refs=False, unpicklable=False)
         if fpath:
             with open(fpath, "w") as file:
                 file.write(json_str)
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/model_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     pass
 
 
 class TaskFormatError(Exception):
     pass
 
 
+class FatalRuleResultError(Exception):
+    pass
+
+
 class JSONSerializable(object):
     def dump(self):
         return self.to_json()
 
     def to_json(self):
         return jsonpickle.encode(self, make_refs=False)
 
@@ -1503,15 +1507,15 @@
         return False
 
     def get_annotation_by_condition(self, cond: AnnotationCondition):
         _annotations = self.annotations
         if cond.type:
             _annotations = [an for an in _annotations if an.type == RiskAnnotation.type and an.risk_type == cond.type]
         if cond.attr_conditions:
-            for (key, val) in cond.attr_conditions:
+            for key, val in cond.attr_conditions:
                 _annotations = [an for an in _annotations if hasattr(an, key) and getattr(an, key) == val]
         if _annotations:
             return _annotations[0]
         return None
 
     def file_info(self):
         file = self.spec.defined_in
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_assessment_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from .utils import (
     escape_url,
     version_to_num,
     diff_files_data,
     is_test_object,
     lock_file,
     unlock_file,
+    remove_lock_file,
 )
 from .safe_glob import safe_glob
 from .keyutil import get_obj_info_by_key, make_imported_taskfile_key
 from .model_loader import load_builtin_modules
 
 
 module_index_name = "module_index.json"
@@ -189,20 +190,22 @@
                         current.append(m_meta)
                         new_data_found = True
                     modules.update({short_name: current})
         if new_data_found:
             self.save_module_index(modules)
         return
 
-    def register_role_index_to_ram(self, findings: Findings):
+    def register_role_index_to_ram(self, findings: Findings, include_test_contents: bool = False):
         new_data_found = False
         roles = self.load_role_index()
         for role in findings.root_definitions.get("definitions", {}).get("roles", []):
             if not isinstance(role, Role):
                 continue
+            if include_test_contents and is_test_object(role.defined_in):
+                continue
             r_meta = RoleMetadata.from_role(role, findings.metadata)
             current = roles.get(r_meta.fqcn, [])
             exists = False
             for r_dict in current:
                 r = None
                 if isinstance(r_dict, dict):
                     r = RoleMetadata.from_dict(r_dict)
@@ -416,15 +419,22 @@
         if "." in name:
             short_name = name.split(".")[-1]
 
         from_indices = False
         found_index = None
         if short_name in self.module_index and self.module_index[short_name]:
             from_indices = True
-            found_index = self.module_index[short_name][0]
+            # look for the module index with FQCN
+            for possible_index in self.module_index[short_name]:
+                if possible_index["fqcn"] == name:
+                    found_index = possible_index
+                    break
+            # if any candidates don't match with FQCN, use the first index
+            if not found_index:
+                found_index = self.module_index[short_name][0]
 
         modules_json_list = []
         if from_indices:
             _type = found_index.get("type", "")
             _name = found_index.get("name", "")
             _version = found_index.get("version", "")
             _hash = found_index.get("hash", "")
@@ -908,15 +918,14 @@
         if os.path.exists(latest_findings_path):
             findings = self.load_findings(latest_findings_path)
 
         self.findings_search_cache[args_str] = findings
         return findings
 
     def load_findings(self, path: str):
-
         basename = os.path.basename(path)
         dir_path = path
         if basename == "findings.json":
             dir_path = os.path.dirname(path)
 
         findings = Findings.load(fpath=os.path.join(dir_path, "findings.json"))
         return findings
@@ -931,18 +940,22 @@
         findings.dump(fpath=os.path.join(out_dir, "findings.json"))
 
     def save_index(self, index_objects, filename):
         out_dir = os.path.join(self.root_dir, "indices")
         if not os.path.exists(out_dir):
             os.makedirs(out_dir, exist_ok=True)
         index_objects_str = jsonpickle.encode(index_objects, make_refs=False, unpicklable=False)
-        with open(os.path.join(out_dir, filename), "w") as file:
-            lock_file(file)
-            file.write(index_objects_str)
-            unlock_file(file)
+        fpath = os.path.join(out_dir, filename)
+        lock = lock_file(fpath)
+        try:
+            with open(fpath, "w") as file:
+                file.write(index_objects_str)
+        finally:
+            unlock_file(lock)
+            remove_lock_file(lock)
 
     def load_index(self, filename=""):
         path = os.path.join(self.root_dir, "indices", filename)
         index_objects = {}
         if os.path.exists(path):
             with open(path, "r") as file:
                 index_objects = json.load(file)
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 import json
 import traceback
 from typing import List
 import time
 
 import ansible_risk_insight.logger as logger
-from .models import AnsibleRunContext, ARIResult, TargetResult, NodeResult, RuleResult, Rule, SpecMutation
+from .models import AnsibleRunContext, ARIResult, TargetResult, NodeResult, RuleResult, Rule, SpecMutation, FatalRuleResultError
 from .keyutil import detect_type, key_delimiter
 from .analyzer import load_taskcalls_in_trees
 from .utils import load_classes_in_dir
 
 
 rule_versions_filename = "rule_versions.json"
 
@@ -174,30 +174,38 @@
             ctx.current = t
             n_result = NodeResult(node=t)
             for rule in loaded_rules:
                 if not rule.enabled:
                     continue
                 start_time = time.time()
                 r_result = RuleResult(file=t.file_info(), rule=rule.get_metadata())
+                detail = {}
                 try:
                     matched = rule.match(ctx)
                     if matched:
                         tmp_result = rule.process(ctx)
                         if tmp_result:
                             r_result = tmp_result
                         r_result.matched = matched
                     r_result.duration = round((time.time() - start_time) * 1000, 6)
+                    detail = r_result.get_detail()
+                    fatal = detail.get("fatal", False)
+                    if fatal:
+                        error = r_result.error or "unknown error"
+                        error = f"ARI rule evaluation threw fatal exception: {error}"
+                        raise FatalRuleResultError(error)
                     if rule.spec_mutation:
-                        detail = r_result.get_detail()
                         if isinstance(detail, dict):
                             s_mutations = detail.get("spec_mutations", [])
                             for s_mutation in s_mutations:
                                 if not isinstance(s_mutation, SpecMutation):
                                     continue
                                 spec_mutations[s_mutation.key] = s_mutation
+                except FatalRuleResultError:
+                    raise
                 except Exception:
                     exc = traceback.format_exc()
                     r_result.error = f"failed to execute the rule `{rule.rule_id}`: {exc}"
                 n_result.rules.append(r_result)
             t_result.nodes.append(n_result)
         ari_result.targets.append(t_result)
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from ansible_risk_insight.models import (
     AnsibleRunContext,
     RunTargetType,
     Rule,
     Severity,
     RuleTag as Tag,
-    Variable,
     VariableType,
     ArgumentsType,
 )
 
 
 def is_loop_var(value, task):
     # `item` or alternative loop variable (if any) should not be replaced to avoid breaking loop
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/tree.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,72 +17,81 @@
 import os
 import traceback
 import subprocess
 import requests
 import hashlib
 import yaml
 import json
+from filelock import FileLock
 from copy import deepcopy
 from tabulate import tabulate
 from inspect import isclass
 from importlib.util import spec_from_file_location, module_from_spec
 
 import ansible_risk_insight.logger as logger
 
 
-try:
-    # Posix based file locking (Linux, Ubuntu, MacOS, etc.)
-    #   Only allows locking on writable files, might cause
-    #   strange results for reading.
-    import fcntl
-
-    def lock_file(f):
-        if f.writable():
-            fcntl.lockf(f, fcntl.LOCK_EX)
-
-    def unlock_file(f):
-        if f.writable():
-            fcntl.lockf(f, fcntl.LOCK_UN)
-
-except ModuleNotFoundError:
-    # Windows file locking
-    import msvcrt
+def lock_file(fpath, timeout=10):
+    if not fpath:
+        return
+    lockfile = get_lock_file_name(fpath)
+    lock = FileLock(lockfile, timeout=timeout)
+    lock.acquire()
+    return lock
+
+
+def unlock_file(lock):
+    if not lock:
+        return
+    if not isinstance(lock, FileLock):
+        return
+    lock.release()
+
+
+def remove_lock_file(lock):
+    if not lock:
+        return
+    if not isinstance(lock, FileLock):
+        return
+    lockfile = lock.lock_file
+    if not lockfile:
+        return
+    if not os.path.exists(lockfile):
+        return
+    os.remove(lockfile)
 
-    def file_size(f):
-        return os.path.getsize(os.path.realpath(f.name))
 
-    def lock_file(f):
-        msvcrt.locking(f.fileno(), msvcrt.LK_RLCK, file_size(f))
-
-    def unlock_file(f):
-        msvcrt.locking(f.fileno(), msvcrt.LK_UNLCK, file_size(f))
+def get_lock_file_name(fpath):
+    return fpath + ".lock"
 
 
 def install_galaxy_target(target, target_type, output_dir, source_repository="", target_version=""):
     server_option = ""
     if source_repository:
         server_option = "--server {}".format(source_repository)
     target_name = target
     if target_version:
         target_name = f"{target}:{target_version}"
     logger.debug("exec ansible-galaxy cmd: ansible-galaxy {} install {} {} -p {}".format(target_type, target_name, server_option, output_dir))
     proc = subprocess.run(
         "ansible-galaxy {} install {} {} -p {}".format(target_type, target_name, server_option, output_dir),
         shell=True,
+        stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         text=True,
     )
     return proc.stdout
 
 
 def install_github_target(target, output_dir):
     proc = subprocess.run(
         "git clone {} {}".format(target, output_dir),
         shell=True,
+        stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         text=True,
     )
     return proc.stdout
 
 
@@ -551,15 +560,15 @@
         fqcn_list.append(fqcn)
     if not fqcn_list:
         return {}
     fqcn_list_str = " ".join(fqcn_list)
     cmd_args = [f"ansible-doc {fqcn_list_str} --json"]
     _env = os.environ.copy()
     _env["ANSIBLE_COLLECTIONS_PATH"] = search_path
-    proc = subprocess.run(cmd_args, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=_env)
+    proc = subprocess.run(args=cmd_args, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=_env)
     if proc.stderr and not proc.stdout:
         logger.debug(f"error while getting the documentation for modules `{fqcn_list_str}`: {proc.stderr}")
         return ""
     wrapper_dict = json.loads(proc.stdout)
     specs = {}
     for fqcn in wrapper_dict:
         doc_dict = wrapper_dict[fqcn].get("doc", {})
```

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/data-struct.txt` & `ansible-risk-insight-0.1.7rc1/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.7rc1/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.7rc1/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.7rc1/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.7rc1/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/annotation.md` & `ansible-risk-insight-0.1.7rc1/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/customize_rules.md` & `ansible-risk-insight-0.1.7rc1/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.7rc1/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.7rc1/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.7rc1/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.7rc1/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/example/readme.md` & `ansible-risk-insight-0.1.7rc1/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.7rc1/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/example/sample.py` & `ansible-risk-insight-0.1.7rc1/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/mkdocs.yml` & `ansible-risk-insight-0.1.7rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/pyproject.toml` & `ansible-risk-insight-0.1.7rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "jsonpickle",
     "PyYAML",
     "smmap",
     "tabulate",
     "requests",
     "ansible",
     "ruamel.yaml",
+    "filelock",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ansible_risk_insight._version.__version__"}
 
 [project.scripts]
```

### Comparing `ansible-risk-insight-0.1.6rc2/test/test_scanner.py` & `ansible-risk-insight-0.1.7rc1/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.6rc2/tox.ini` & `ansible-risk-insight-0.1.7rc1/tox.ini`

 * *Files identical despite different names*

