# Comparing `tmp/swh.lister-5.3.0.tar.gz` & `tmp/swh.lister-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.lister-5.3.0.tar", last modified: Tue May  2 12:38:55 2023, max compression
+gzip compressed data, was "dist/swh.lister-5.4.0.tar", last modified: Fri May 19 13:48:03 2023, max compression
```

## Comparing `swh.lister-5.3.0.tar` & `swh.lister-5.4.0.tar`

### file list

```diff
@@ -1,607 +1,607 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-02 12:38:53.000000 swh.lister-5.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      113 2023-05-02 12:38:53.000000 swh.lister-5.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-05-02 12:38:53.000000 swh.lister-5.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-02 12:38:53.000000 swh.lister-5.3.0/ACKNOWLEDGEMENTS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-02 12:38:53.000000 swh.lister-5.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)      153 2023-05-02 12:38:53.000000 swh.lister-5.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-02 12:38:53.000000 swh.lister-5.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      218 2023-05-02 12:38:53.000000 swh.lister-5.3.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-02 12:38:53.000000 swh.lister-5.3.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-05-02 12:38:55.000000 swh.lister-5.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3218 2023-05-02 12:38:53.000000 swh.lister-5.3.0/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      554 2023-05-02 12:38:53.000000 swh.lister-5.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)    77777 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/images/new_base.png
--rw-r--r--   0 jenkins    (115) docker     (999)     5612 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/images/new_bitbucket_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)     6675 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/images/new_github_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)    30902 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/images/old_github_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)      677 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4996 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/new_lister_template.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3381 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/run_a_new_lister.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2452 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/save_forge.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    17094 2023-05-02 12:38:53.000000 swh.lister-5.3.0/docs/tutorial.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      952 2023-05-02 12:38:53.000000 swh.lister-5.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 12:38:53.000000 swh.lister-5.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-05-02 12:38:53.000000 swh.lister-5.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-05-02 12:38:53.000000 swh.lister-5.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-05-02 12:38:53.000000 swh.lister-5.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-05-02 12:38:53.000000 swh.lister-5.3.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-02 12:38:55.000000 swh.lister-5.3.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     3962 2023-05-02 12:38:53.000000 swh.lister-5.3.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)     2918 2023-05-02 12:38:53.000000 swh.lister-5.3.0/sql/crawler.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1073 2023-05-02 12:38:53.000000 swh.lister-5.3.0/sql/pimp_db.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/
--rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/arch/
--rw-r--r--   0 jenkins    (115) docker     (999)     8141 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18461 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/arch/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)     1146 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)    43737 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     6401 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog
--rw-r--r--   0 jenkins    (115) docker     (999)     3443 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance
--rw-r--r--   0 jenkins    (115) docker     (999)     1373 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip
--rw-r--r--   0 jenkins    (115) docker     (999)     1034 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns
--rw-r--r--   0 jenkins    (115) docker     (999)    11596 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial
--rw-r--r--   0 jenkins    (115) docker     (999)     1453 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib
--rw-r--r--   0 jenkins    (115) docker     (999)     1958 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1758 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1190 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1128 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)    70402 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/arch/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/aur/
--rw-r--r--   0 jenkins    (115) docker     (999)     4847 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      588 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/aur/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/aur/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2084 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tests/data/fake_aur_packages.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      701 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     5066 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/aur/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bitbucket/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1200 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4213 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6600 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1762 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bitbucket/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bower/
--rw-r--r--   0 jenkins    (115) docker     (999)     2171 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2412 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bower/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bower/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/bower/tests/data/https_registry.bower.io/
--rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/tests/data/https_registry.bower.io/packages
--rw-r--r--   0 jenkins    (115) docker     (999)     1160 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/bower/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8503 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      557 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/
--rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/README
--rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo
--rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary
--rw-r--r--   0 jenkins    (115) docker     (999)     2375 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed
--rw-r--r--   0 jenkins    (115) docker     (999)     5382 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.baserock.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     3213 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.eclipse.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     3377 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/README
--rw-r--r--   0 jenkins    (115) docker     (999)   530004 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     7459 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/
--rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/README
--rw-r--r--   0 jenkins    (115) docker     (999)    11062 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     3157 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100
--rw-r--r--   0 jenkins    (115) docker     (999)    11407 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50
--rw-r--r--   0 jenkins    (115) docker     (999)     2719 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects
--rw-r--r--   0 jenkins    (115) docker     (999)     2656 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users
--rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects
--rw-r--r--   0 jenkins    (115) docker     (999)    15289 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base
--rw-r--r--   0 jenkins    (115) docker     (999)    14966 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2
--rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250
--rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12
--rw-r--r--   0 jenkins    (115) docker     (999)    15849 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp
--rw-r--r--   0 jenkins    (115) docker     (999)    15926 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay
--rw-r--r--   0 jenkins    (115) docker     (999)    12968 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev
--rw-r--r--   0 jenkins    (115) docker     (999)    16116 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv
--rw-r--r--   0 jenkins    (115) docker     (999)     9041 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm
--rw-r--r--   0 jenkins    (115) docker     (999)     6692 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl
--rw-r--r--   0 jenkins    (115) docker     (999)    17765 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc
--rw-r--r--   0 jenkins    (115) docker     (999)    29634 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl
--rw-r--r--   0 jenkins    (115) docker     (999)    28967 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_jff.email/
--rw-r--r--   0 jenkins    (115) docker     (999)     3442 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/data/https_jff.email/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     7243 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/repo_list.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     8757 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1237 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cgit/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cli.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/conda/
--rw-r--r--   0 jenkins    (115) docker     (999)     4336 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4757 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      589 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/conda/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_conda.anaconda.org/
--rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/
--rw-r--r--   0 jenkins    (115) docker     (999)      634 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     1445 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)      770 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     4332 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/conda/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cpan/
--rw-r--r--   0 jenkins    (115) docker     (999)     1990 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7360 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cpan/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     9011 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     1102 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     2458 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3
--rw-r--r--   0 jenkins    (115) docker     (999)     4089 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4
--rw-r--r--   0 jenkins    (115) docker     (999)     9128 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search
--rw-r--r--   0 jenkins    (115) docker     (999)     5367 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cpan/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cran/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/__init__.py
--rwxr-xr-x   0 jenkins    (115) docker     (999)      305 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/list_all_packages.R
--rw-r--r--   0 jenkins    (115) docker     (999)     4959 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cran/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/cran/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      883 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/tests/data/list-r-packages.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4854 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/cran/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/crates/
--rw-r--r--   0 jenkins    (115) docker     (999)     4779 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9337 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      599 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/crates/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      174 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/crates/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     3851 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/crates/tests/data/https_static.crates.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     1358 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1534 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)     7982 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/crates/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/debian/
--rw-r--r--   0 jenkins    (115) docker     (999)      460 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11355 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/debian/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/debian/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     5970 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_bullseye
--rw-r--r--   0 jenkins    (115) docker     (999)     4413 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_buster
--rw-r--r--   0 jenkins    (115) docker     (999)     4893 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_stretch
--rw-r--r--   0 jenkins    (115) docker     (999)     9160 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/debian/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/fedora/
--rw-r--r--   0 jenkins    (115) docker     (999)      400 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10356 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/fedora/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1982 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1172 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     3112 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     4971 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     7582 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1944 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/fedora/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitea/
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      749 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitea/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitea/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitea/tests/data/https_try.gitea.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     5856 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     7652 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     6224 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1838 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitea/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/github/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7559 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1859 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/github/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9015 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)      296 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/github/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/
--rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9848 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/
--rw-r--r--   0 jenkins    (115) docker     (999)    12380 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/
--rw-r--r--   0 jenkins    (115) docker     (999)     1605 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gitlab.com/
--rw-r--r--   0 jenkins    (115) docker     (999)     6065 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    13032 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1492 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gitlab/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gnu/
--rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2663 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gnu/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gnu/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/
--rw-r--r--   0 jenkins    (115) docker     (999)   622168 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     6450 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/data/tree.json
--rw-r--r--   0 jenkins    (115) docker     (999)      982 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/data/tree.min.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1290 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1077 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8690 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tests/test_tree.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9207 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gnu/tree.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gogs/
--rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7202 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gogs/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     2949 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     3072 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3
--rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4
--rw-r--r--   0 jenkins    (115) docker     (999)    11848 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1830 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/gogs/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/golang/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6327 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      756 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/golang/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/golang/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      489 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/data/page-1.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      418 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/data/page-2.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/data/page-3.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     7644 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1743 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/golang/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/
--rw-r--r--   0 jenkins    (115) docker     (999)     2804 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5183 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      621 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23107 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23804 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0
--rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23805 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0
--rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit2
--rw-r--r--   0 jenkins    (115) docker     (999)    23353 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1
--rw-r--r--   0 jenkins    (115) docker     (999)    22764 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2
--rw-r--r--   0 jenkins    (115) docker     (999)     6472 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1159 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hackage/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hex/
--rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4692 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hex/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hex/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/
--rw-r--r--   0 jenkins    (115) docker     (999)     6247 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     7468 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3554 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page3.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5203 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1737 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/hex/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/launchpad/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7518 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1747 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     5814 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_response1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4960 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_response2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     8457 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1793 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/launchpad/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/
--rw-r--r--   0 jenkins    (115) docker     (999)     9772 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16142 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      888 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)    31940 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/
--rw-r--r--   0 jenkins    (115) docker     (999)     2312 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/export_full.fld
--rw-r--r--   0 jenkins    (115) docker     (999)      740 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld
--rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/export_null_mtime.fld
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)     5749 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j
--rw-r--r--   0 jenkins    (115) docker     (999)     7821 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java
--rw-r--r--   0 jenkins    (115) docker     (999)     6110 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     2823 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom
--rwxr-xr-x   0 jenkins    (115) docker     (999)     7586 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     2831 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom
--rw-r--r--   0 jenkins    (115) docker     (999)    13122 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/maven/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nixguix/
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    22153 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     6666 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/data/sources-failure.json
--rw-r--r--   0 jenkins    (115) docker     (999)     9912 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/data/sources-success.json
--rw-r--r--   0 jenkins    (115) docker     (999)    13751 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      933 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nixguix/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/npm/
--rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5999 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      827 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/npm/tests/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/npm/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)    10583 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/data/npm_full_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     7301 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/data/npm_full_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5759 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/data/npm_incremental_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    22638 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/data/npm_incremental_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6441 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1784 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/npm/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nuget/
--rw-r--r--   0 jenkins    (115) docker     (999)     3249 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nuget/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1336 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     2832 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     8037 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5322 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6791 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1519 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1287 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)     2567 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3634 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/nuget/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4737 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1389 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/
--rw-r--r--   0 jenkins    (115) docker     (999)     1176 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/
--rw-r--r--   0 jenkins    (115) docker     (999)     1085 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/
--rw-r--r--   0 jenkins    (115) docker     (999)     1092 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/
--rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/
--rw-r--r--   0 jenkins    (115) docker     (999)     1472 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1004 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/repo
--rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/version
--rw-r--r--   0 jenkins    (115) docker     (999)     5843 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/opam/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/packagist/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7053 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      518 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/packagist/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     2281 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/den1n_contextmenu.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       53 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/repos_gitlky_wx_article
--rw-r--r--   0 jenkins    (115) docker     (999)     6972 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api
--rw-r--r--   0 jenkins    (115) docker     (999)     5394 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main
--rw-r--r--   0 jenkins    (115) docker     (999)     9749 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/idevlab_essential.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2545 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6911 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/lky_wx_article.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4632 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/payrix_payrix-php.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4062 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/with_invalid_url.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/data/ycms_module-main.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6680 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1052 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/packagist/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14169 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pattern.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/phabricator/
--rw-r--r--   0 jenkins    (115) docker     (999)      345 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6039 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      753 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    44289 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    46784 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/phabricator/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pubdev/
--rw-r--r--   0 jenkins    (115) docker     (999)     2064 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3573 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/
--rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/api_package-names
--rw-r--r--   0 jenkins    (115) docker     (999)     1578 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker
--rw-r--r--   0 jenkins    (115) docker     (999)     1557 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon
--rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pubdev/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/puppet/
--rw-r--r--   0 jenkins    (115) docker     (999)     3557 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6203 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/puppet/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/puppet/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/
--rw-r--r--   0 jenkins    (115) docker     (999)    94411 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100
--rw-r--r--   0 jenkins    (115) docker     (999)    10141 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100
--rw-r--r--   0 jenkins    (115) docker     (999)    92818 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26
--rw-r--r--   0 jenkins    (115) docker     (999)     5702 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/puppet/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pypi/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6736 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/pypi/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8171 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/pypi/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/rubygems/
--rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9375 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      894 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     2867 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar
--rw-r--r--   0 jenkins    (115) docker     (999)     1361 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     6208 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/rubygems/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/sourceforge/
--rw-r--r--   0 jenkins    (115) docker     (999)      340 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18526 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      820 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     1632 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/aaron.html
--rw-r--r--   0 jenkins    (115) docker     (999)     6332 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/aaron.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2242 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/adobexmp.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3993 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/backapps-website.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5614 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/backapps.json
--rw-r--r--   0 jenkins    (115) docker     (999)      384 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/main-sitemap.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     3041 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/mojunk.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3938 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/mramm.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2404 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html
--rw-r--r--   0 jenkins    (115) docker     (999)     5477 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3209 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/os3dmodels.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/random-mercurial.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1523 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     7836 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/t12eksandbox.html
--rw-r--r--   0 jenkins    (115) docker     (999)     7904 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/data/t12eksandbox.json
--rw-r--r--   0 jenkins    (115) docker     (999)    19233 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/sourceforge/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2064 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9165 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tests/test_pattern.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1191 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tests/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/tuleap/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4611 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      579 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/
--rw-r--r--   0 jenkins    (115) docker     (999)     4552 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects
--rw-r--r--   0 jenkins    (115) docker     (999)      422 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_1
--rw-r--r--   0 jenkins    (115) docker     (999)      338 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_2
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_3
--rw-r--r--   0 jenkins    (115) docker     (999)     5639 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/tuleap/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2215 2023-05-02 12:38:53.000000 swh.lister-5.3.0/swh/lister/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)    21059 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-02 12:38:55.000000 swh.lister-5.3.0/swh.lister.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1599 2023-05-02 12:38:53.000000 swh.lister-5.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-19 13:48:00.000000 swh.lister-5.4.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      113 2023-05-19 13:48:00.000000 swh.lister-5.4.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-05-19 13:48:00.000000 swh.lister-5.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-19 13:48:00.000000 swh.lister-5.4.0/ACKNOWLEDGEMENTS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-19 13:48:00.000000 swh.lister-5.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      153 2023-05-19 13:48:00.000000 swh.lister-5.4.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-19 13:48:00.000000 swh.lister-5.4.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      218 2023-05-19 13:48:00.000000 swh.lister-5.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-19 13:48:00.000000 swh.lister-5.4.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-05-19 13:48:03.000000 swh.lister-5.4.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3218 2023-05-19 13:48:00.000000 swh.lister-5.4.0/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      554 2023-05-19 13:48:00.000000 swh.lister-5.4.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)    77777 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/images/new_base.png
+-rw-r--r--   0 jenkins    (115) docker     (999)     5612 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/images/new_bitbucket_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)     6675 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/images/new_github_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    30902 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/images/old_github_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)      677 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4996 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/new_lister_template.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3381 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/run_a_new_lister.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2452 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/save_forge.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    17094 2023-05-19 13:48:00.000000 swh.lister-5.4.0/docs/tutorial.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      952 2023-05-19 13:48:00.000000 swh.lister-5.4.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-19 13:48:00.000000 swh.lister-5.4.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-05-19 13:48:00.000000 swh.lister-5.4.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-05-19 13:48:00.000000 swh.lister-5.4.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-05-19 13:48:00.000000 swh.lister-5.4.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-05-19 13:48:00.000000 swh.lister-5.4.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-19 13:48:03.000000 swh.lister-5.4.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     3962 2023-05-19 13:48:00.000000 swh.lister-5.4.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2918 2023-05-19 13:48:00.000000 swh.lister-5.4.0/sql/crawler.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1073 2023-05-19 13:48:00.000000 swh.lister-5.4.0/sql/pimp_db.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/arch/
+-rw-r--r--   0 jenkins    (115) docker     (999)     8141 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18461 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/arch/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1146 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)    43737 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6401 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog
+-rw-r--r--   0 jenkins    (115) docker     (999)     3443 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance
+-rw-r--r--   0 jenkins    (115) docker     (999)     1373 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip
+-rw-r--r--   0 jenkins    (115) docker     (999)     1034 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns
+-rw-r--r--   0 jenkins    (115) docker     (999)    11596 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial
+-rw-r--r--   0 jenkins    (115) docker     (999)     1453 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib
+-rw-r--r--   0 jenkins    (115) docker     (999)     1958 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1758 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1190 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1128 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)    70402 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/arch/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/aur/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4847 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      588 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/aur/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/aur/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2084 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tests/data/fake_aur_packages.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      701 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     5066 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/aur/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bitbucket/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1200 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4213 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6600 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1762 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bitbucket/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bower/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2171 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2412 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bower/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bower/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/bower/tests/data/https_registry.bower.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/tests/data/https_registry.bower.io/packages
+-rw-r--r--   0 jenkins    (115) docker     (999)     1160 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/bower/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8503 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      557 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/README
+-rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo
+-rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary
+-rw-r--r--   0 jenkins    (115) docker     (999)     2375 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed
+-rw-r--r--   0 jenkins    (115) docker     (999)     5382 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.baserock.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3213 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.eclipse.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3377 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/README
+-rw-r--r--   0 jenkins    (115) docker     (999)   530004 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     7459 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/
+-rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/README
+-rw-r--r--   0 jenkins    (115) docker     (999)    11062 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     3157 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    11407 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50
+-rw-r--r--   0 jenkins    (115) docker     (999)     2719 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects
+-rw-r--r--   0 jenkins    (115) docker     (999)     2656 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users
+-rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects
+-rw-r--r--   0 jenkins    (115) docker     (999)    15289 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base
+-rw-r--r--   0 jenkins    (115) docker     (999)    14966 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2
+-rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250
+-rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12
+-rw-r--r--   0 jenkins    (115) docker     (999)    15849 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp
+-rw-r--r--   0 jenkins    (115) docker     (999)    15926 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay
+-rw-r--r--   0 jenkins    (115) docker     (999)    12968 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev
+-rw-r--r--   0 jenkins    (115) docker     (999)    16116 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv
+-rw-r--r--   0 jenkins    (115) docker     (999)     9041 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm
+-rw-r--r--   0 jenkins    (115) docker     (999)     6692 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl
+-rw-r--r--   0 jenkins    (115) docker     (999)    17765 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc
+-rw-r--r--   0 jenkins    (115) docker     (999)    29634 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl
+-rw-r--r--   0 jenkins    (115) docker     (999)    28967 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_jff.email/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3442 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/data/https_jff.email/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     7243 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/repo_list.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     8757 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1237 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cgit/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1877 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cli.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/conda/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4336 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4757 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      589 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/conda/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_conda.anaconda.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)      634 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     1445 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      770 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     4332 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/conda/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cpan/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1990 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7360 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cpan/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     9011 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     1102 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     2458 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3
+-rw-r--r--   0 jenkins    (115) docker     (999)     4089 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4
+-rw-r--r--   0 jenkins    (115) docker     (999)     9128 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search
+-rw-r--r--   0 jenkins    (115) docker     (999)     5367 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cpan/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cran/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/__init__.py
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      305 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/list_all_packages.R
+-rw-r--r--   0 jenkins    (115) docker     (999)     4959 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cran/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/cran/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      883 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/tests/data/list-r-packages.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4854 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/cran/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/crates/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4779 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9337 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      599 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/crates/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      174 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/crates/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     3851 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/crates/tests/data/https_static.crates.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1358 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1534 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)     7982 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/crates/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/debian/
+-rw-r--r--   0 jenkins    (115) docker     (999)      460 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11355 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/debian/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/debian/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5970 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_bullseye
+-rw-r--r--   0 jenkins    (115) docker     (999)     4413 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_buster
+-rw-r--r--   0 jenkins    (115) docker     (999)     4893 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_stretch
+-rw-r--r--   0 jenkins    (115) docker     (999)     9160 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/debian/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/fedora/
+-rw-r--r--   0 jenkins    (115) docker     (999)      400 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10356 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/fedora/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1982 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1172 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     3112 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     4971 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     7582 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1944 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/fedora/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitea/
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      749 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitea/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitea/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitea/tests/data/https_try.gitea.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5856 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     7652 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     6224 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1838 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitea/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/github/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7559 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1859 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/github/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9015 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      296 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/github/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/
+-rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10135 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)    12380 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1605 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gitlab.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6065 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    13570 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1492 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gitlab/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gnu/
+-rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2663 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gnu/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gnu/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)   622168 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     6450 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/data/tree.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      982 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/data/tree.min.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1290 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1077 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8690 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tests/test_tree.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9207 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gnu/tree.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gogs/
+-rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7401 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gogs/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2949 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     3072 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3
+-rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4
+-rw-r--r--   0 jenkins    (115) docker     (999)    12373 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1830 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/gogs/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/golang/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6327 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      756 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/golang/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/golang/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      489 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/data/page-1.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      418 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/data/page-2.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/data/page-3.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     7644 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1743 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/golang/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2804 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5183 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      621 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23107 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23804 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0
+-rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23805 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0
+-rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit2
+-rw-r--r--   0 jenkins    (115) docker     (999)    23353 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1
+-rw-r--r--   0 jenkins    (115) docker     (999)    22764 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2
+-rw-r--r--   0 jenkins    (115) docker     (999)     6472 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1159 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hackage/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hex/
+-rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4692 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hex/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hex/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6247 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     7468 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3554 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page3.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5203 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1737 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/hex/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/launchpad/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7518 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1747 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5814 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_response1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4960 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_response2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     8457 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1793 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/launchpad/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/
+-rw-r--r--   0 jenkins    (115) docker     (999)     9772 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16142 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      888 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)    31940 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2312 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/export_full.fld
+-rw-r--r--   0 jenkins    (115) docker     (999)      740 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld
+-rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/export_null_mtime.fld
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5749 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j
+-rw-r--r--   0 jenkins    (115) docker     (999)     7821 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java
+-rw-r--r--   0 jenkins    (115) docker     (999)     6110 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     2823 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     7586 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     2831 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)    13122 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/maven/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nixguix/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    22153 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6666 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/data/sources-failure.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     9912 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/data/sources-success.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    13751 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      933 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nixguix/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/npm/
+-rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5999 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      827 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/npm/tests/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/npm/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)    10583 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/data/npm_full_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     7301 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/data/npm_full_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5759 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/data/npm_incremental_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    22638 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/data/npm_incremental_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6441 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1784 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/npm/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nuget/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3249 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nuget/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1336 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     2832 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     8037 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5322 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6791 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1519 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1287 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)     2567 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3634 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/nuget/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4737 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1389 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1176 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1085 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1092 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1472 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1004 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/repo
+-rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/version
+-rw-r--r--   0 jenkins    (115) docker     (999)     5843 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/opam/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/packagist/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7053 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      518 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/packagist/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2281 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/den1n_contextmenu.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       53 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/repos_gitlky_wx_article
+-rw-r--r--   0 jenkins    (115) docker     (999)     6972 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api
+-rw-r--r--   0 jenkins    (115) docker     (999)     5394 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main
+-rw-r--r--   0 jenkins    (115) docker     (999)     9749 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/idevlab_essential.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2545 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6911 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/lky_wx_article.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4632 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/payrix_payrix-php.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4062 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/with_invalid_url.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/data/ycms_module-main.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6680 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1052 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/packagist/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15460 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pattern.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/phabricator/
+-rw-r--r--   0 jenkins    (115) docker     (999)      345 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6039 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      753 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    44289 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    46784 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/phabricator/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pubdev/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2064 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3573 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/
+-rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/api_package-names
+-rw-r--r--   0 jenkins    (115) docker     (999)     1578 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker
+-rw-r--r--   0 jenkins    (115) docker     (999)     1557 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon
+-rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pubdev/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/puppet/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3557 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6203 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/puppet/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/puppet/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)    94411 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    10141 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    92818 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26
+-rw-r--r--   0 jenkins    (115) docker     (999)     5702 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/puppet/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pypi/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6736 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/pypi/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8171 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/pypi/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/rubygems/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9375 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      894 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2867 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar
+-rw-r--r--   0 jenkins    (115) docker     (999)     1361 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     6208 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/rubygems/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/sourceforge/
+-rw-r--r--   0 jenkins    (115) docker     (999)      340 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18526 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      820 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1632 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/aaron.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     6332 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/aaron.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2242 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/adobexmp.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3993 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/backapps-website.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5614 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/backapps.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      384 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/main-sitemap.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     3041 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/mojunk.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3938 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/mramm.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2404 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     5477 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3209 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/os3dmodels.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/random-mercurial.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1523 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     7836 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/t12eksandbox.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     7904 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/data/t12eksandbox.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    19233 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/sourceforge/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2012 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9972 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tests/test_pattern.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1191 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tests/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/tuleap/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4611 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      579 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4552 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects
+-rw-r--r--   0 jenkins    (115) docker     (999)      422 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_1
+-rw-r--r--   0 jenkins    (115) docker     (999)      338 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_2
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_3
+-rw-r--r--   0 jenkins    (115) docker     (999)     5639 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/tuleap/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2215 2023-05-19 13:48:00.000000 swh.lister-5.4.0/swh/lister/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)    21059 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-19 13:48:03.000000 swh.lister-5.4.0/swh.lister.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1599 2023-05-19 13:48:00.000000 swh.lister-5.4.0/tox.ini
```

### Comparing `swh.lister-5.3.0/.pre-commit-config.yaml` & `swh.lister-5.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/CODE_OF_CONDUCT.md` & `swh.lister-5.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/LICENSE` & `swh.lister-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/PKG-INFO` & `swh.lister-5.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.lister
-Version: 5.3.0
+Version: 5.4.0
 Summary: Software Heritage lister
 Home-page: https://forge.softwareheritage.org/diffusion/DLSGH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-lister
```

### Comparing `swh.lister-5.3.0/README.md` & `swh.lister-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/conftest.py` & `swh.lister-5.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/images/new_base.png` & `swh.lister-5.4.0/docs/images/new_base.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/images/new_bitbucket_lister.png` & `swh.lister-5.4.0/docs/images/new_bitbucket_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/images/new_github_lister.png` & `swh.lister-5.4.0/docs/images/new_github_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/images/old_github_lister.png` & `swh.lister-5.4.0/docs/images/old_github_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/index.rst` & `swh.lister-5.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/new_lister_template.py` & `swh.lister-5.4.0/docs/new_lister_template.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/run_a_new_lister.rst` & `swh.lister-5.4.0/docs/run_a_new_lister.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/save_forge.rst` & `swh.lister-5.4.0/docs/save_forge.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/docs/tutorial.rst` & `swh.lister-5.4.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/mypy.ini` & `swh.lister-5.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/setup.py` & `swh.lister-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/sql/crawler.sql` & `swh.lister-5.4.0/sql/crawler.sql`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/sql/pimp_db.sql` & `swh.lister-5.4.0/sql/pimp_db.sql`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/__init__.py` & `swh.lister-5.4.0/swh/lister/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/__init__.py` & `swh.lister-5.4.0/swh/lister/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/lister.py` & `swh.lister-5.4.0/swh/lister/arch/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tasks.py` & `swh.lister-5.4.0/swh/lister/arch/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/__init__.py` & `swh.lister-5.4.0/swh/lister/arch/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh` & `swh.lister-5.4.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz` & `swh.lister-5.4.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/arch/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/arch/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/arch/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/__init__.py` & `swh.lister-5.4.0/swh/lister/aur/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/lister.py` & `swh.lister-5.4.0/swh/lister/aur/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/tasks.py` & `swh.lister-5.4.0/swh/lister/aur/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/tests/data/fake_aur_packages.sh` & `swh.lister-5.4.0/swh/lister/aur/tests/data/fake_aur_packages.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz` & `swh.lister-5.4.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/aur/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/aur/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/aur/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/lister.py` & `swh.lister-5.4.0/swh/lister/bitbucket/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/tasks.py` & `swh.lister-5.4.0/swh/lister/bitbucket/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json` & `swh.lister-5.4.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json` & `swh.lister-5.4.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/bitbucket/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bitbucket/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/bitbucket/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bower/__init__.py` & `swh.lister-5.4.0/swh/lister/bower/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bower/lister.py` & `swh.lister-5.4.0/swh/lister/bower/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bower/tasks.py` & `swh.lister-5.4.0/swh/lister/bower/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bower/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/bower/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/bower/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/bower/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/lister.py` & `swh.lister-5.4.0/swh/lister/cgit/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tasks.py` & `swh.lister-5.4.0/swh/lister/cgit/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/data/https_jff.email/cgit` & `swh.lister-5.4.0/swh/lister/cgit/tests/data/https_jff.email/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/repo_list.txt` & `swh.lister-5.4.0/swh/lister/cgit/tests/repo_list.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/cgit/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cgit/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/cgit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cli.py` & `swh.lister-5.4.0/swh/lister/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     context_settings=CONTEXT_SETTINGS,
     help="Trigger a full listing run for a particular forge "
     "instance. The output of this listing results in "
     '"oneshot" tasks in the scheduler db with a priority '
     "defined by the user",
 )
 @click.option(
-    "--lister", "-l", help="Lister to run", type=click.Choice(SUPPORTED_LISTERS)
+    "--lister",
+    "-l",
+    help="Lister to run",
+    type=click.Choice(SUPPORTED_LISTERS),
+    required=True,
 )
 @click.argument("options", nargs=-1)
 @click.pass_context
 def run(ctx, lister, options):
     from swh.scheduler.cli.utils import parse_options
 
     config = deepcopy(ctx.obj["config"])
```

### Comparing `swh.lister-5.3.0/swh/lister/conda/__init__.py` & `swh.lister-5.4.0/swh/lister/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/lister.py` & `swh.lister-5.4.0/swh/lister/conda/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tasks.py` & `swh.lister-5.4.0/swh/lister/conda/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2` & `swh.lister-5.4.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/conda/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/conda/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/conda/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/__init__.py` & `swh.lister-5.4.0/swh/lister/cpan/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/lister.py` & `swh.lister-5.4.0/swh/lister/cpan/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tasks.py` & `swh.lister-5.4.0/swh/lister/cpan/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1` & `swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2` & `swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3` & `swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4` & `swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search` & `swh.lister-5.4.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/cpan/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cpan/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/cpan/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cran/lister.py` & `swh.lister-5.4.0/swh/lister/cran/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cran/tasks.py` & `swh.lister-5.4.0/swh/lister/cran/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cran/tests/data/list-r-packages.json` & `swh.lister-5.4.0/swh/lister/cran/tests/data/list-r-packages.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cran/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/cran/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/cran/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/cran/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/__init__.py` & `swh.lister-5.4.0/swh/lister/crates/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/lister.py` & `swh.lister-5.4.0/swh/lister/crates/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tasks.py` & `swh.lister-5.4.0/swh/lister/crates/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh` & `swh.lister-5.4.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz` & `swh.lister-5.4.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1` & `swh.lister-5.4.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/crates/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/crates/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/crates/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/lister.py` & `swh.lister-5.4.0/swh/lister/debian/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tasks.py` & `swh.lister-5.4.0/swh/lister/debian/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_bullseye` & `swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_bullseye`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_buster` & `swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_buster`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tests/data/Sources_stretch` & `swh.lister-5.4.0/swh/lister/debian/tests/data/Sources_stretch`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/debian/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/debian/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/debian/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/lister.py` & `swh.lister-5.4.0/swh/lister/fedora/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tasks.py` & `swh.lister-5.4.0/swh/lister/fedora/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz` & `swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz` & `swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz` & `swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml` & `swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml` & `swh.lister-5.4.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/fedora/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/fedora/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/fedora/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/lister.py` & `swh.lister-5.4.0/swh/lister/gitea/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/tasks.py` & `swh.lister-5.4.0/swh/lister/gitea/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1` & `swh.lister-5.4.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2` & `swh.lister-5.4.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/gitea/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitea/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/gitea/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/github/lister.py` & `swh.lister-5.4.0/swh/lister/github/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/github/tasks.py` & `swh.lister-5.4.0/swh/lister/github/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/github/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/github/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/github/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/github/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/lister.py` & `swh.lister-5.4.0/swh/lister/gitlab/lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,30 @@
         ignored_project_prefixes: List of prefixes of project paths to ignore
 
     """
 
     def __init__(
         self,
         scheduler,
-        url: str,
+        url: Optional[str] = None,
         name: Optional[str] = "gitlab",
         instance: Optional[str] = None,
         credentials: Optional[CredentialsType] = None,
         max_origins_per_page: Optional[int] = None,
         max_pages: Optional[int] = None,
         enable_origins: bool = True,
         incremental: bool = False,
         ignored_project_prefixes: Optional[List[str]] = None,
     ):
         if name is not None:
             self.LISTER_NAME = name
         super().__init__(
             scheduler=scheduler,
-            url=url.rstrip("/"),
+            # if url is not provided, url will be built in the `build_url` method
+            url=url.rstrip("/") if url else None,
             instance=instance,
             credentials=credentials,
             max_origins_per_page=max_origins_per_page,
             max_pages=max_pages,
             enable_origins=enable_origins,
         )
         self.incremental = incremental
@@ -134,14 +135,19 @@
             logger.info(
                 "Using %s credentials from user %s", self.instance, cred["username"]
             )
             api_token = cred["password"]
             if api_token:
                 self.session.headers["Authorization"] = f"Bearer {api_token}"
 
+    def build_url(self, instance: str) -> str:
+        """Build gitlab api url."""
+        prefix_url = super().build_url(instance)
+        return f"{prefix_url}/api/v4"
+
     def state_from_dict(self, d: Dict[str, Any]) -> GitLabListerState:
         return GitLabListerState(**d)
 
     def state_to_dict(self, state: GitLabListerState) -> Dict[str, Any]:
         return asdict(state)
 
     @http_retry(
```

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tasks.py` & `swh.lister-5.4.0/swh/lister/gitlab/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json` & `swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json` & `swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json` & `swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json` & `swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json` & `swh.lister-5.4.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/gitlab/tests/test_lister.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,25 +18,38 @@
 from swh.lister.pattern import ListerStats
 from swh.lister.tests.utils import assert_sleep_calls
 
 logger = logging.getLogger(__name__)
 
 
 def api_url(instance: str) -> str:
-    return f"https://{instance}/api/v4/"
+    return f"https://{instance}/api/v4"
 
 
 def _match_request(request, lister_name="gitlab"):
     return request.headers.get("User-Agent") == USER_AGENT_TEMPLATE % lister_name
 
 
+def test_lister_gitlab_fail_to_instantiate(swh_scheduler):
+    """Build a lister without its url nor its instance should raise"""
+    # while instantiating a gitlab lister is fine with the url or the instance...
+    assert GitLabLister(swh_scheduler, url="https://gitlab.com/api/v4") is not None
+    assert GitLabLister(swh_scheduler, instance="gitlab.fr") is not None
+
+    # ... It will raise without any of those
+    with pytest.raises(ValueError, match="'url' or 'instance'"):
+        GitLabLister(swh_scheduler)
+
+
 def test_lister_gitlab(datadir, swh_scheduler, requests_mock):
     """Gitlab lister supports full listing"""
     instance = "gitlab.com"
-    lister = GitLabLister(swh_scheduler, url=api_url(instance), instance=instance)
+    lister = GitLabLister(swh_scheduler, instance=instance)
+
+    assert lister.url == api_url(instance)
 
     response = gitlab_page_response(datadir, instance, 1)
 
     requests_mock.get(
         lister.page_url(),
         [{"json": response}],
         additional_matcher=_match_request,
```

### Comparing `swh.lister-5.3.0/swh/lister/gitlab/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/gitlab/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/lister.py` & `swh.lister-5.4.0/swh/lister/gnu/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tasks.py` & `swh.lister-5.4.0/swh/lister/gnu/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz` & `swh.lister-5.4.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/data/tree.json` & `swh.lister-5.4.0/swh/lister/gnu/tests/data/tree.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/data/tree.min.json` & `swh.lister-5.4.0/swh/lister/gnu/tests/data/tree.min.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/gnu/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/gnu/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tests/test_tree.py` & `swh.lister-5.4.0/swh/lister/gnu/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gnu/tree.py` & `swh.lister-5.4.0/swh/lister/gnu/tree.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/lister.py` & `swh.lister-5.4.0/swh/lister/gogs/lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from dataclasses import asdict, dataclass
 import logging
 import random
@@ -66,15 +66,15 @@
     VISIT_TYPE = "git"
 
     REPO_LIST_PATH = "repos/search"
 
     def __init__(
         self,
         scheduler: SchedulerInterface,
-        url: str,
+        url: Optional[str] = None,
         instance: Optional[str] = None,
         api_token: Optional[str] = None,
         page_size: int = 50,
         credentials: CredentialsType = None,
         max_origins_per_page: Optional[int] = None,
         max_pages: Optional[int] = None,
         enable_origins: bool = True,
@@ -107,14 +107,19 @@
         if self.api_token:
             self.session.headers["Authorization"] = f"token {self.api_token}"
         else:
             logger.warning(
                 "No authentication token set in configuration, using anonymous mode"
             )
 
+    def build_url(self, instance: str) -> str:
+        "Build gogs url out of the instance."
+        prefix_url = super().build_url(instance)
+        return f"{prefix_url}/api/v1/"
+
     def state_from_dict(self, d: Dict[str, Any]) -> GogsListerState:
         return GogsListerState(**d)
 
     def state_to_dict(self, state: GogsListerState) -> Dict[str, Any]:
         return asdict(state)
 
     def page_request(
```

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tasks.py` & `swh.lister-5.4.0/swh/lister/gogs/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1` & `swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2` & `swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3` & `swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4` & `swh.lister-5.4.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/gogs/tests/test_lister.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2022-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import json
 from pathlib import Path
 from typing import List
@@ -95,21 +95,31 @@
 def check_listed_origins(lister_urls: List[str], scheduler_origins: List[ListedOrigin]):
     """Asserts that the two collections have the same origin URLs.
 
     Does not test last_update."""
     assert set(lister_urls) == {origin.url for origin in scheduler_origins}
 
 
+def test_lister_gogs_fail_to_instantiate(swh_scheduler):
+    """Build a lister without its url nor its instance should raise"""
+    # while instantiating a gogs lister is fine with the url or the instance...
+    assert GogsLister(swh_scheduler, url="https://try.gogs.io/api/v1") is not None
+    assert GogsLister(swh_scheduler, instance="try.gogs.io") is not None
+
+    # ... It will raise without any of those
+    with pytest.raises(ValueError, match="'url' or 'instance'"):
+        GogsLister(swh_scheduler)
+
+
 def test_gogs_full_listing(
     swh_scheduler, requests_mock, mocker, trygogs_p1, trygogs_p2, trygogs_p3_last
 ):
-    kwargs = dict(
-        url=TRY_GOGS_URL, instance="try_gogs", page_size=3, api_token="secret"
-    )
+    kwargs = dict(instance="try.gogs.io", page_size=3, api_token="secret")
     lister = GogsLister(scheduler=swh_scheduler, **kwargs)
+    assert lister.url == TRY_GOGS_URL
 
     lister.get_origins_from_page: Mock = mocker.spy(lister, "get_origins_from_page")
 
     p1_text, p1_headers, p1_result, p1_origin_urls = trygogs_p1
     p2_text, p2_headers, p2_result, p2_origin_urls = trygogs_p2
     p3_text, p3_headers, p3_result, p3_origin_urls = trygogs_p3_last
```

### Comparing `swh.lister-5.3.0/swh/lister/gogs/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/gogs/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/golang/lister.py` & `swh.lister-5.4.0/swh/lister/golang/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/golang/tasks.py` & `swh.lister-5.4.0/swh/lister/golang/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/golang/tests/data/page-3.txt` & `swh.lister-5.4.0/swh/lister/golang/tests/data/page-3.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/golang/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/golang/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/golang/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/golang/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/__init__.py` & `swh.lister-5.4.0/swh/lister/hackage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/lister.py` & `swh.lister-5.4.0/swh/lister/hackage/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tasks.py` & `swh.lister-5.4.0/swh/lister/hackage/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2` & `swh.lister-5.4.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/hackage/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hackage/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/hackage/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/lister.py` & `swh.lister-5.4.0/swh/lister/hex/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tasks.py` & `swh.lister-5.4.0/swh/lister/hex/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page1.json` & `swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page2.json` & `swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tests/data/https_hex.pm/page3.json` & `swh.lister-5.4.0/swh/lister/hex/tests/data/https_hex.pm/page3.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/hex/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/hex/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/hex/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/lister.py` & `swh.lister-5.4.0/swh/lister/launchpad/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tasks.py` & `swh.lister-5.4.0/swh/lister/launchpad/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/conftest.py` & `swh.lister-5.4.0/swh/lister/launchpad/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json` & `swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_response1.json` & `swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_response1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/data/launchpad_response2.json` & `swh.lister-5.4.0/swh/lister/launchpad/tests/data/launchpad_response2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/launchpad/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/launchpad/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/launchpad/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/README.md` & `swh.lister-5.4.0/swh/lister/maven/README.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/lister.py` & `swh.lister-5.4.0/swh/lister/maven/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tasks.py` & `swh.lister-5.4.0/swh/lister/maven/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/export_full.fld` & `swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/export_full.fld`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld` & `swh.lister-5.4.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom` & `swh.lister-5.4.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/maven/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/maven/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/maven/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/__init__.py` & `swh.lister-5.4.0/swh/lister/nixguix/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/lister.py` & `swh.lister-5.4.0/swh/lister/nixguix/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/tasks.py` & `swh.lister-5.4.0/swh/lister/nixguix/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/tests/data/sources-failure.json` & `swh.lister-5.4.0/swh/lister/nixguix/tests/data/sources-failure.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/tests/data/sources-success.json` & `swh.lister-5.4.0/swh/lister/nixguix/tests/data/sources-success.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/nixguix/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nixguix/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/nixguix/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/__init__.py` & `swh.lister-5.4.0/swh/lister/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/lister.py` & `swh.lister-5.4.0/swh/lister/npm/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tasks.py` & `swh.lister-5.4.0/swh/lister/npm/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/data/npm_full_page1.json` & `swh.lister-5.4.0/swh/lister/npm/tests/data/npm_full_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/data/npm_full_page2.json` & `swh.lister-5.4.0/swh/lister/npm/tests/data/npm_full_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/data/npm_incremental_page1.json` & `swh.lister-5.4.0/swh/lister/npm/tests/data/npm_incremental_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/data/npm_incremental_page2.json` & `swh.lister-5.4.0/swh/lister/npm/tests/data/npm_incremental_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/npm/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/npm/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/npm/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/__init__.py` & `swh.lister-5.4.0/swh/lister/nuget/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/lister.py` & `swh.lister-5.4.0/swh/lister/nuget/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tasks.py` & `swh.lister-5.4.0/swh/lister/nuget/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json` & `swh.lister-5.4.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/nuget/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/nuget/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/nuget/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/lister.py` & `swh.lister-5.4.0/swh/lister/opam/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tasks.py` & `swh.lister-5.4.0/swh/lister/opam/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam` & `swh.lister-5.4.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/opam/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/opam/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/opam/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/lister.py` & `swh.lister-5.4.0/swh/lister/packagist/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tasks.py` & `swh.lister-5.4.0/swh/lister/packagist/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/den1n_contextmenu.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/den1n_contextmenu.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/idevlab_essential.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/idevlab_essential.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/lky_wx_article.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/lky_wx_article.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/payrix_payrix-php.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/payrix_payrix-php.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/with_invalid_url.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/with_invalid_url.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/data/ycms_module-main.json` & `swh.lister-5.4.0/swh/lister/packagist/tests/data/ycms_module-main.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/packagist/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/packagist/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/packagist/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pattern.py` & `swh.lister-5.4.0/swh/lister/pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,30 +100,42 @@
 
     LISTER_NAME: str = ""
     github_session: Optional[GitHubSession] = None
 
     def __init__(
         self,
         scheduler: SchedulerInterface,
-        url: str,
+        url: Optional[str] = None,
         instance: Optional[str] = None,
         credentials: CredentialsType = None,
         max_origins_per_page: Optional[int] = None,
         max_pages: Optional[int] = None,
         enable_origins: bool = True,
         with_github_session: bool = False,
     ):
         if not self.LISTER_NAME:
             raise ValueError("Must set the LISTER_NAME attribute on Lister classes")
 
-        self.url = url
+        self.url: str
+        if url is not None:
+            # Retro-compability with lister already instantiated out of a provided url
+            self.url = url
+        elif url is None and instance is not None:
+            # Allow lister to be instantiated simply with their type and instance
+            # (as in their domain like "gitlab.com", "git.garbaye.fr", ...)
+            self.url = self.build_url(instance)
+        else:
+            raise ValueError(
+                "Either 'url' or 'instance' parameter should be provided for listing."
+            )
+
         if instance is not None:
             self.instance = instance
         else:
-            self.instance = urlparse(url).netloc
+            self.instance = urlparse(self.url).netloc
 
         self.scheduler = scheduler
 
         if not credentials:
             credentials = {}
         self.credentials = list(
             credentials.get(self.LISTER_NAME, {}).get(self.instance, [])
@@ -148,14 +160,33 @@
         )
 
         self.recorded_origins: Set[str] = set()
         self.max_pages = max_pages
         self.max_origins_per_page = max_origins_per_page
         self.enable_origins = enable_origins
 
+    def build_url(self, instance: str) -> str:
+        """Optionally build the forge url to list. When the url is not provided in the
+        constructor, this method is called. This should compute the actual url to use to
+        list the forge.
+
+        This is particularly useful for forges which uses an api. This simplifies the
+        cli calls to use. They should then only provide the instance (its domain).
+
+        For example:
+        - gitlab: https://{instance}/api/v4
+        - gitea: https://{instance}/api/v1
+        - ...
+
+        """
+        scheme = urlparse(instance).scheme
+        if scheme:
+            raise ValueError("Instance should only be a net location.")
+        return f"https://{instance}"
+
     @http_retry(before_sleep=before_sleep_log(logger, logging.WARNING))
     def http_request(self, url: str, method="GET", **kwargs) -> requests.Response:
         logger.debug("Fetching URL %s with params %s", url, kwargs.get("params"))
 
         response = self.session.request(method, url, **kwargs)
         if response.status_code not in (200, 304):
             logger.warning(
```

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/lister.py` & `swh.lister-5.4.0/swh/lister/phabricator/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/tasks.py` & `swh.lister-5.4.0/swh/lister/phabricator/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json` & `swh.lister-5.4.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json` & `swh.lister-5.4.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/phabricator/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/phabricator/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/phabricator/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/__init__.py` & `swh.lister-5.4.0/swh/lister/pubdev/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/lister.py` & `swh.lister-5.4.0/swh/lister/pubdev/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/tasks.py` & `swh.lister-5.4.0/swh/lister/pubdev/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker` & `swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon` & `swh.lister-5.4.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/pubdev/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pubdev/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/pubdev/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/__init__.py` & `swh.lister-5.4.0/swh/lister/puppet/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/lister.py` & `swh.lister-5.4.0/swh/lister/puppet/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tasks.py` & `swh.lister-5.4.0/swh/lister/puppet/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100` & `swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100` & `swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26` & `swh.lister-5.4.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/puppet/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/puppet/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/puppet/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pypi/lister.py` & `swh.lister-5.4.0/swh/lister/pypi/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pypi/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/pypi/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/pypi/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/pypi/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/__init__.py` & `swh.lister-5.4.0/swh/lister/rubygems/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/lister.py` & `swh.lister-5.4.0/swh/lister/rubygems/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tasks.py` & `swh.lister-5.4.0/swh/lister/rubygems/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml` & `swh.lister-5.4.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar` & `swh.lister-5.4.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh` & `swh.lister-5.4.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/rubygems/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/rubygems/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/rubygems/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/lister.py` & `swh.lister-5.4.0/swh/lister/sourceforge/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tasks.py` & `swh.lister-5.4.0/swh/lister/sourceforge/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/aaron.html` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/aaron.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/aaron.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/aaron.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/adobexmp.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/adobexmp.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/backapps-website.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/backapps-website.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/backapps.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/backapps.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/mojunk.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/mojunk.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/mramm.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/mramm.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/os3dmodels.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/os3dmodels.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/random-mercurial.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/random-mercurial.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/t12eksandbox.html` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/t12eksandbox.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/data/t12eksandbox.json` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/data/t12eksandbox.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/sourceforge/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/sourceforge/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tests/test_cli.py` & `swh.lister-5.4.0/swh/lister/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2021  The Software Heritage developers
+# Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
 
 from swh.lister.cli import SUPPORTED_LISTERS, get_lister
@@ -13,30 +13,29 @@
     },
     "phabricator": {
         "instance": "softwareheritage",
         "url": "https://forge.softwareheritage.org/api/diffusion.repository.search",
         "api_token": "bogus",
     },
     "gitea": {
-        "url": "https://try.gitea.io/api/v1/",
+        "instance": "try.gitea.io",
     },
     "tuleap": {
         "url": "https://tuleap.net",
     },
     "gitlab": {
-        "url": "https://gitlab.ow2.org/api/v4",
-        "instance": "ow2",
+        "instance": "gitlab.ow2.org",
     },
     "opam": {"url": "https://opam.ocaml.org", "instance": "opam"},
     "maven": {
         "url": "https://repo1.maven.org/maven2/",
         "index_url": "http://indexes/export.fld",
     },
     "gogs": {
-        "url": "https://try.gogs.io/",
+        "instance": "try.gogs.io",
         "api_token": "secret",
     },
     "nixguix": {
         "url": "https://guix.gnu.org/sources.json",
         "origin_upstream": "https://git.savannah.gnu.org/cgit/guix.git/",
     },
     "fedora": {
```

### Comparing `swh.lister-5.3.0/swh/lister/tests/test_pattern.py` & `swh.lister-5.4.0/swh/lister/tests/test_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,32 @@
 
     LISTER_NAME = "test-pattern-lister"
 
     def state_from_dict(self, d: Dict[str, str]) -> StateType:
         return d
 
 
+def test_instantiation_fail_to_instantiate(swh_scheduler):
+    """Instantiation without proper url or instance will raise."""
+    # While instantiating with either a url or instance is fine...
+    InstantiableLister(scheduler=swh_scheduler, url="https://example.com")
+    InstantiableLister(scheduler=swh_scheduler, instance="example.com")
+
+    # ... Instantiating will fail when:
+    # - no instance nor url parameters are provided to the constructor
+    with pytest.raises(ValueError, match="'url' or 'instance"):
+        InstantiableLister(
+            scheduler=swh_scheduler,
+        )
+
+    # - an instance, which is not in a net location format, is provided
+    with pytest.raises(ValueError, match="net location"):
+        InstantiableLister(scheduler=swh_scheduler, instance="http://example.com")
+
+
 def test_instantiation(swh_scheduler):
     lister = InstantiableLister(
         scheduler=swh_scheduler, url="https://example.com", instance="example.com"
     )
 
     # check the lister was registered in the scheduler backend
     stored_lister = swh_scheduler.get_or_create_lister(
```

### Comparing `swh.lister-5.3.0/swh/lister/tests/test_utils.py` & `swh.lister-5.4.0/swh/lister/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tuleap/lister.py` & `swh.lister-5.4.0/swh/lister/tuleap/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tuleap/tasks.py` & `swh.lister-5.4.0/swh/lister/tuleap/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects` & `swh.lister-5.4.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tuleap/tests/test_lister.py` & `swh.lister-5.4.0/swh/lister/tuleap/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/tuleap/tests/test_tasks.py` & `swh.lister-5.4.0/swh/lister/tuleap/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh/lister/utils.py` & `swh.lister-5.4.0/swh/lister/utils.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh.lister.egg-info/PKG-INFO` & `swh.lister-5.4.0/swh.lister.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.lister
-Version: 5.3.0
+Version: 5.4.0
 Summary: Software Heritage lister
 Home-page: https://forge.softwareheritage.org/diffusion/DLSGH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-lister
```

### Comparing `swh.lister-5.3.0/swh.lister.egg-info/SOURCES.txt` & `swh.lister-5.4.0/swh.lister.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/swh.lister.egg-info/entry_points.txt` & `swh.lister-5.4.0/swh.lister.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.3.0/tox.ini` & `swh.lister-5.4.0/tox.ini`

 * *Files identical despite different names*

