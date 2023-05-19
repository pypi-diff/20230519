# Comparing `tmp/pytest-testinfra-7.0.0.tar.gz` & `tmp/pytest-testinfra-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-testinfra-7.0.0.tar", last modified: Thu Dec  1 20:30:48 2022, max compression
+gzip compressed data, was "pytest-testinfra-8.0.0.tar", last modified: Fri May 19 08:31:51 2023, max compression
```

## Comparing `pytest-testinfra-7.0.0.tar` & `pytest-testinfra-8.0.0.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      253 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)    10969 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10143 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      528 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)       54 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       83 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     6783 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     9916 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      592 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/_templates/piwik.html
--rw-r--r--   0 runner    (1001) docker     (122)      664 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7205 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/backends.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9466 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      192 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/invocation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4758 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)      767 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/doc/source/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/alpine/
--rw-r--r--   0 runner    (1001) docker     (122)      931 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/images/alpine/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/archlinux/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/images/archlinux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/centos_7/
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/images/centos_7/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/debian_bullseye/
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/images/debian_bullseye/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/images/ubuntu_xenial/
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/images/ubuntu_xenial/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)      239 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/pytest_testinfra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     8609 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test/ssh_key
--rw-r--r--   0 runner    (1001) docker     (122)    21241 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test/test_invocation.py
--rw-r--r--   0 runner    (1001) docker     (122)    21449 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/testinfra/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/testinfra/backend/
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2822 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     8345 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/chroot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (122)      968 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/openshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/paramiko.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/podman.py
--rw-r--r--   0 runner    (1001) docker     (122)     2377 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/salt.py
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/backend/winrm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5540 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/host.py
--rw-r--r--   0 runner    (1001) docker     (122)      690 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/testinfra/modules/
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4739 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/addr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4180 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/blockdevice.py
--rw-r--r--   0 runner    (1001) docker     (122)      854 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/environment.py
--rw-r--r--   0 runner    (1001) docker     (122)     8228 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/group.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/iptables.py
--rw-r--r--   0 runner    (1001) docker     (122)     4403 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/mountpoint.py
--rw-r--r--   0 runner    (1001) docker     (122)     5941 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/package.py
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/pip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/podman.py
--rw-r--r--   0 runner    (1001) docker     (122)     6296 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     2985 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/puppet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/salt.py
--rw-r--r--   0 runner    (1001) docker     (122)     8328 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/service.py
--rw-r--r--   0 runner    (1001) docker     (122)    12724 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/sudo.py
--rw-r--r--   0 runner    (1001) docker     (122)     5265 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1163 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (122)     5826 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/systeminfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     6524 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/modules/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     6357 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:30:48.000000 pytest-testinfra-7.0.0/testinfra/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/testinfra/utils/ansible_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2022-12-01 20:30:39.000000 pytest-testinfra-7.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.266626 pytest-testinfra-8.0.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/_templates/piwik.html
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/invocation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.254625 pytest-testinfra-8.0.0/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/alpine/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/alpine/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/archlinux/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/archlinux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/debian_bullseye/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/debian_bullseye/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.274627 pytest-testinfra-8.0.0/images/rockylinux8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/rockylinux8/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.274627 pytest-testinfra-8.0.0/images/ubuntu_xenial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/ubuntu_xenial/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.278627 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-19 08:31:51.306628 pytest-testinfra-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.278627 pytest-testinfra-8.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/ssh_key
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.282627 pytest-testinfra-8.0.0/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.290627 pytest-testinfra-8.0.0/testinfra/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/paramiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/winrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/testinfra/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/addr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/blockdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/iptables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/mountpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/puppet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/systeminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/testinfra/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/utils/ansible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-testinfra-7.0.0/CHANGELOG.rst` & `pytest-testinfra-8.0.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 =========
 Changelog
 =========
 
+8.0.0
+=====
+
+* [NEW] Add Group.members attribute
+* [NEW] Add File.inode attribute
+* [NEW] Add Interface.routes() method
+* [NEW] Add Docker.is_restarting attribute
+* [FIX] Fix possible error in Interface.default()
+* [FIX] Fix busybox detection in Process module
+* [FIX] Fix possible KeyError in SysInfo module
+* [BREAKING] Drop support for python 3.7
+
+7.0.1
+=====
+
+* [FIX] Fix `command -v` compatibility with dash shell
+
 7.0.0
 =====
 
 * [NEW] Improved ssh config support in Paramiko backend
 * [NEW] Add chroot backend
 * [NEW] Add support for Manjaro-Linux
 * [NEW] Add support for Cloudlinux
```

### Comparing `pytest-testinfra-7.0.0/CONTRIBUTING.rst` & `pytest-testinfra-8.0.0/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 #########################
 
 First, thanks for contributing to testinfra and make it even more awesome !
 
 Pull requests
 =============
 
-Regardless the review by a developer, a pull request will trigger automatic
-tests on https://travis-ci.org/pytest-dev/pytest-testinfra/
-
 You're encouraged to setup a full test environment, to add tests and check if
 all the tests pass *before* submitting your pull request. To run the complete
 test suite you must install:
 
 - `Docker <https://www.docker.com>`_
 - `tox <https://tox.readthedocs.io/en/latest/>`_
```

### Comparing `pytest-testinfra-7.0.0/LICENSE` & `pytest-testinfra-8.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -169,8 +169,7 @@
       or other liability obligations and/or rights consistent with this
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
-
```

### Comparing `pytest-testinfra-7.0.0/MANIFEST.in` & `pytest-testinfra-8.0.0/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 recursive-include doc *.py *.rst *.svg
 include doc/source/_templates/piwik.html
 include doc/Makefile
 include tox.ini
 include .flake8
 include mypy.ini
 include Makefile
+include *.yaml
 include README.rst CONTRIBUTING.rst CHANGELOG.rst
 include MANIFEST.in
 include ansible.cfg
 include dev-requirements.txt
 include test-requirements.txt
 include LICENSE
 exclude .editorconfig
-exclude .travis.yml
 exclude .gitignore
 prune doc/build
 prune .github
```

### Comparing `pytest-testinfra-7.0.0/PKG-INFO` & `pytest-testinfra-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 7.0.0
+Version: 8.0.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: ansible
 Provides-Extra: docker
 Provides-Extra: kubectl
 Provides-Extra: local
 Provides-Extra: lxc
 Provides-Extra: paramiko
@@ -49,28 +48,28 @@
 
 Testinfra aims to be a Serverspec_ equivalent in python and is written as
 a plugin to the powerful Pytest_ test engine
 
 License
 =======
 
-`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/master/LICENSE>`_
+`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/main/LICENSE>`_
 
 The logo is licensed under the `Creative Commons NoDerivatives 4.0 License <https://creativecommons.org/licenses/by-nd/4.0/>`_
 If you have some other use in mind, contact us.
 
 Quick start
 ===========
 
 Install testinfra using pip::
 
     $ pip install pytest-testinfra
 
     # or install the devel version
-    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@master#egg=pytest-testinfra'
+    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@main#egg=pytest-testinfra'
 
 
 Write your first tests file to `test_myinfra.py`:
 
 .. code-block:: python
 
     def test_passwd_file(host):
```

### Comparing `pytest-testinfra-7.0.0/README.rst` & `pytest-testinfra-8.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 Testinfra aims to be a Serverspec_ equivalent in python and is written as
 a plugin to the powerful Pytest_ test engine
 
 License
 =======
 
-`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/master/LICENSE>`_
+`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/main/LICENSE>`_
 
 The logo is licensed under the `Creative Commons NoDerivatives 4.0 License <https://creativecommons.org/licenses/by-nd/4.0/>`_
 If you have some other use in mind, contact us.
 
 Quick start
 ===========
 
 Install testinfra using pip::
 
     $ pip install pytest-testinfra
 
     # or install the devel version
-    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@master#egg=pytest-testinfra'
+    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@main#egg=pytest-testinfra'
 
 
 Write your first tests file to `test_myinfra.py`:
 
 .. code-block:: python
 
     def test_passwd_file(host):
```

### Comparing `pytest-testinfra-7.0.0/doc/Makefile` & `pytest-testinfra-8.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/_static/logo.svg` & `pytest-testinfra-8.0.0/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/_templates/piwik.html` & `pytest-testinfra-8.0.0/doc/source/_templates/piwik.html`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/api.rst` & `pytest-testinfra-8.0.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/backends.rst` & `pytest-testinfra-8.0.0/doc/source/backends.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/conf.py` & `pytest-testinfra-8.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
-
 import datetime
+import os
 import subprocess
+import sys
+from typing import Dict, List
 
 import alabaster
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath("../.."))
@@ -88,15 +88,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = []
+exclude_patterns: List[str] = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -129,15 +129,14 @@
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "logo": "logo.svg",
     "github_user": "pytest-dev",
     "github_repo": "pytest-testinfra",
     "github_button": True,
-    "travis_button": True,
     "extra_nav_links": {
         "View on github": "https://github.com/pytest-dev/pytest-testinfra",
     },
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 html_theme_path = [alabaster.get_path()]
@@ -218,15 +217,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "testinfradoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
+latex_elements: Dict[str, tuple] = {
     # The paper size ('letterpaper' or 'a4paper')
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
```

### Comparing `pytest-testinfra-7.0.0/doc/source/examples.rst` & `pytest-testinfra-8.0.0/doc/source/examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 `NRPE <https://en.wikipedia.org/wiki/Nagios#Nagios_Remote_Plugin_Executor>`_.
 
 
 Integration with KitchenCI
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 KitchenCI (aka Test Kitchen) can use testinfra via its :code:`shell` verifier.
-Add the following to your :code:`.kitchen.yml`, this requires installing `paramiko` 
+Add the following to your :code:`.kitchen.yml`, this requires installing `paramiko`
 additionally (on your host machine, not in the VM handled by kitchen) ::
 
     verifier:
       name: shell
       command: py.test --hosts="paramiko://${KITCHEN_USERNAME}@${KITCHEN_HOSTNAME}:${KITCHEN_PORT}?ssh_identity_file=${KITCHEN_SSH_KEY}" --junit-xml "junit-${KITCHEN_INSTANCE}.xml" "test/integration/${KITCHEN_SUITE}"
```

### Comparing `pytest-testinfra-7.0.0/doc/source/invocation.rst` & `pytest-testinfra-8.0.0/doc/source/invocation.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/modules.rst` & `pytest-testinfra-8.0.0/doc/source/modules.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/doc/source/support.rst` & `pytest-testinfra-8.0.0/doc/source/support.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/images/alpine/Dockerfile` & `pytest-testinfra-8.0.0/images/alpine/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,7 @@
     rc-update add sshd && \
     mkdir -p /root/.ssh && \
     chmod 700 /root/.ssh && \
     echo "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCgDryK4AjJeifuc2N54St13KMNlnGLAtibQSMmvSyrhH7XJ1atnBo1HrJhGZNNBVKM67+zYNc9J3fg3qI1g63vSQAA+nXMsDYwu4BPwupakpwJELcGZJxsUGzjGVotVpqPIX5nW8NBGvkVuObI4UELOleq5mQMTGerJO64KkSVi20FDwPJn3q8GG2zk3pESiDA5ShEyFhYC8vOLfSSYD0LYmShAVGCLEgiNb+OXQL6ZRvzqfFEzL0QvaI/l3mb6b0VFPAO4QWOL0xj3cWzOZXOqht3V85CZvSk8ISdNgwCjXLZsPeaYL/toHNvBF30VMrDZ7w4SDU0ZZLEsc/ezxjb" > /root/.ssh/authorized_keys
 
 EXPOSE 22
 CMD ["/sbin/init"]
-
-
```

### Comparing `pytest-testinfra-7.0.0/images/centos_7/Dockerfile` & `pytest-testinfra-8.0.0/images/rockylinux8/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-FROM centos:7
+FROM rockylinux:8
 
-RUN yum -y install openssh-server && yum clean all &&\
+RUN dnf -y install openssh-server procps python39 && dnf clean all &&\
     (cd /lib/systemd/system/sysinit.target.wants/; for i in *; do if ! test $i = systemd-tmpfiles-setup.service; then rm -f $i; fi; done) && \
     rm -f /lib/systemd/system/multi-user.target.wants/* && \
     rm -f /etc/systemd/system/*.wants/* && \
     rm -f /lib/systemd/system/local-fs.target.wants/* && \
     rm -f /lib/systemd/system/sockets.target.wants/*udev* && \
     rm -f /lib/systemd/system/sockets.target.wants/*initctl* && \
     rm -f /lib/systemd/system/basic.target.wants/* && \
@@ -13,10 +13,9 @@
     ssh-keygen -q -N "" -t dsa -f /etc/ssh/ssh_host_ecdsa_key && \
     ssh-keygen -q -N "" -t rsa -f /etc/ssh/ssh_host_rsa_key && \
     sed -i "s/#UsePrivilegeSeparation.*/UsePrivilegeSeparation no/g" /etc/ssh/sshd_config && \
     systemctl enable sshd.service && \
     mkdir -p /root/.ssh && \
     echo "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCgDryK4AjJeifuc2N54St13KMNlnGLAtibQSMmvSyrhH7XJ1atnBo1HrJhGZNNBVKM67+zYNc9J3fg3qI1g63vSQAA+nXMsDYwu4BPwupakpwJELcGZJxsUGzjGVotVpqPIX5nW8NBGvkVuObI4UELOleq5mQMTGerJO64KkSVi20FDwPJn3q8GG2zk3pESiDA5ShEyFhYC8vOLfSSYD0LYmShAVGCLEgiNb+OXQL6ZRvzqfFEzL0QvaI/l3mb6b0VFPAO4QWOL0xj3cWzOZXOqht3V85CZvSk8ISdNgwCjXLZsPeaYL/toHNvBF30VMrDZ7w4SDU0ZZLEsc/ezxjb" > /root/.ssh/authorized_keys
 
-VOLUME ["/sys/fs/cgroup"]
 EXPOSE 22
 CMD ["/usr/sbin/init"]
```

### Comparing `pytest-testinfra-7.0.0/images/debian_bullseye/Dockerfile` & `pytest-testinfra-8.0.0/images/debian_bullseye/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/images/ubuntu_xenial/Dockerfile` & `pytest-testinfra-8.0.0/images/ubuntu_xenial/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,7 @@
     systemctl disable ssh.service && \
     mkdir -p /var/run/sshd && \
     mkdir -p /root/.ssh && \
     echo "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCgDryK4AjJeifuc2N54St13KMNlnGLAtibQSMmvSyrhH7XJ1atnBo1HrJhGZNNBVKM67+zYNc9J3fg3qI1g63vSQAA+nXMsDYwu4BPwupakpwJELcGZJxsUGzjGVotVpqPIX5nW8NBGvkVuObI4UELOleq5mQMTGerJO64KkSVi20FDwPJn3q8GG2zk3pESiDA5ShEyFhYC8vOLfSSYD0LYmShAVGCLEgiNb+OXQL6ZRvzqfFEzL0QvaI/l3mb6b0VFPAO4QWOL0xj3cWzOZXOqht3V85CZvSk8ISdNgwCjXLZsPeaYL/toHNvBF30VMrDZ7w4SDU0ZZLEsc/ezxjb" > /root/.ssh/authorized_keys
 
 EXPOSE 22
 CMD ["/sbin/init"]
-
```

### Comparing `pytest-testinfra-7.0.0/pytest_testinfra.egg-info/PKG-INFO` & `pytest-testinfra-8.0.0/pytest_testinfra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 7.0.0
+Version: 8.0.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: ansible
 Provides-Extra: docker
 Provides-Extra: kubectl
 Provides-Extra: local
 Provides-Extra: lxc
 Provides-Extra: paramiko
@@ -49,28 +48,28 @@
 
 Testinfra aims to be a Serverspec_ equivalent in python and is written as
 a plugin to the powerful Pytest_ test engine
 
 License
 =======
 
-`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/master/LICENSE>`_
+`Apache License 2.0 <https://github.com/pytest-dev/pytest-testinfra/blob/main/LICENSE>`_
 
 The logo is licensed under the `Creative Commons NoDerivatives 4.0 License <https://creativecommons.org/licenses/by-nd/4.0/>`_
 If you have some other use in mind, contact us.
 
 Quick start
 ===========
 
 Install testinfra using pip::
 
     $ pip install pytest-testinfra
 
     # or install the devel version
-    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@master#egg=pytest-testinfra'
+    $ pip install 'git+https://github.com/pytest-dev/pytest-testinfra@main#egg=pytest-testinfra'
 
 
 Write your first tests file to `test_myinfra.py`:
 
 .. code-block:: python
 
     def test_passwd_file(host):
```

### Comparing `pytest-testinfra-7.0.0/pytest_testinfra.egg-info/SOURCES.txt` & `pytest-testinfra-8.0.0/pytest_testinfra.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .flake8
+.pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 ansible.cfg
@@ -23,16 +24,16 @@
 doc/source/invocation.rst
 doc/source/modules.rst
 doc/source/support.rst
 doc/source/_static/logo.svg
 doc/source/_templates/piwik.html
 images/alpine/Dockerfile
 images/archlinux/Dockerfile
-images/centos_7/Dockerfile
 images/debian_bullseye/Dockerfile
+images/rockylinux8/Dockerfile
 images/ubuntu_xenial/Dockerfile
 pytest_testinfra.egg-info/PKG-INFO
 pytest_testinfra.egg-info/SOURCES.txt
 pytest_testinfra.egg-info/dependency_links.txt
 pytest_testinfra.egg-info/entry_points.txt
 pytest_testinfra.egg-info/requires.txt
 pytest_testinfra.egg-info/top_level.txt
```

### Comparing `pytest-testinfra-7.0.0/setup.cfg` & `pytest-testinfra-8.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Testing
 	Topic :: System :: Systems Administration
 	Framework :: Pytest
 
 [options]
 use_scm_version = True
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	pytest!=3.0.2
 extras_require =
```

### Comparing `pytest-testinfra-7.0.0/setup.py` & `pytest-testinfra-8.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/test/conftest.py` & `pytest-testinfra-8.0.0/test/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 3235393661656230350a326264356530326432393832353064363439393330616634633761393838
 3261
 """
 
 DOCKER_IMAGES = [
     "alpine",
     "archlinux",
-    "centos_7",
+    "rockylinux8",
     "debian_bullseye",
     "ubuntu_xenial",
 ]
 
 
 def setup_ansible_config(tmpdir, name, host, user, port, key):
     items = [
@@ -109,15 +109,21 @@
 
         def teardown():
             check_output("docker rm -f %s", docker_id)
 
         request.addfinalizer(teardown)
 
         port = check_output("docker port %s 22", docker_id)
-        port = int(port.rsplit(":", 1)[-1])
+        # IPv4 addresses seem to be reported consistently
+        # in the first line of the output.
+        # To workaround https://github.com/moby/moby/issues/42442
+        # use only the values of the first line of the command
+        # output
+        port = int(port.splitlines()[0].rsplit(":", 1)[-1])
+
         return docker_id, docker_host, port
 
     fname = "_docker_container_{}_{}".format(image, scope)
     mod = sys.modules[__name__]
     setattr(mod, fname, func)
 
 
@@ -177,15 +183,15 @@
                 ).format(hostname, docker_host, port, str(key))
             )
             kw["ssh_config"] = str(ssh_config)
 
         # Wait ssh to be up
         service = testinfra.get_host(docker_id, connection="docker").service
 
-        images_with_sshd = ("centos_7", "alpine", "archlinux")
+        images_with_sshd = ("rockylinux8", "alpine", "archlinux")
 
         if image in images_with_sshd:
             service_name = "sshd"
         else:
             service_name = "ssh"
 
         while not service(service_name).is_running:
```

### Comparing `pytest-testinfra-7.0.0/test/ssh_key` & `pytest-testinfra-8.0.0/test/ssh_key`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/test/test_backends.py` & `pytest-testinfra-8.0.0/test/test_backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,75 +125,75 @@
     with tempfile.NamedTemporaryFile() as f:
         f.write(
             (
                 b"ungrp\n"
                 b"[g1]\n"
                 b"debian\n"
                 b"[g2]\n"
-                b"centos\n"
+                b"rockylinux\n"
                 b"[g3:children]\n"
                 b"g1\n"
                 b"g2\n"
                 b"[g4:children]\n"
                 b"g3"
             )
         )
         f.flush()
 
         def get_hosts(spec):
             return AnsibleRunner(f.name).get_hosts(spec)
 
-        assert get_hosts("all") == ["centos", "debian", "ungrp"]
-        assert get_hosts("*") == ["centos", "debian", "ungrp"]
+        assert get_hosts("all") == ["debian", "rockylinux", "ungrp"]
+        assert get_hosts("*") == ["debian", "rockylinux", "ungrp"]
         assert get_hosts("g1") == ["debian"]
-        assert get_hosts("*2") == ["centos"]
+        assert get_hosts("*2") == ["rockylinux"]
         assert get_hosts("*ia*") == ["debian"]
-        assert get_hosts("*3") == ["centos", "debian"]
-        assert get_hosts("*4") == ["centos", "debian"]
+        assert get_hosts("*3") == ["debian", "rockylinux"]
+        assert get_hosts("*4") == ["debian", "rockylinux"]
         assert get_hosts("ungrouped") == ["ungrp"]
         assert get_hosts("un*") == ["ungrp"]
         assert get_hosts("nope") == []
 
 
 def test_ansible_get_variables():
     with tempfile.NamedTemporaryFile() as f:
         f.write(
             (
                 b"debian a=b c=d\n"
-                b"centos e=f\n"
+                b"rockylinux e=f\n"
                 b"[all:vars]\n"
                 b"a=a\n"
                 b"[g]\n"
                 b"debian\n"
                 b"[g:vars]\n"
                 b"x=z\n"
             )
         )
         f.flush()
 
         def get_vars(host):
             return AnsibleRunner(f.name).get_variables(host)
 
         groups = {
-            "all": ["centos", "debian"],
+            "all": ["debian", "rockylinux"],
             "g": ["debian"],
-            "ungrouped": ["centos"],
+            "ungrouped": ["rockylinux"],
         }
         assert get_vars("debian") == {
             "a": "b",
             "c": "d",
             "x": "z",
             "inventory_hostname": "debian",
             "group_names": ["g"],
             "groups": groups,
         }
-        assert get_vars("centos") == {
+        assert get_vars("rockylinux") == {
             "a": "a",
             "e": "f",
-            "inventory_hostname": "centos",
+            "inventory_hostname": "rockylinux",
             "group_names": ["ungrouped"],
             "groups": groups,
         }
 
 
 @pytest.mark.parametrize(
     "kwargs,inventory,expected",
@@ -481,20 +481,20 @@
     # just check that all declared backend are importable and NAME is set
     # correctly
     for connection_type in testinfra.backend.BACKENDS:
         obj = testinfra.backend.get_backend_class(connection_type)
         assert obj.get_connection_type() == connection_type
 
 
-@pytest.mark.testinfra_hosts("docker://centos_7", "ssh://centos_7")
+@pytest.mark.testinfra_hosts("docker://rockylinux8", "ssh://rockylinux8")
 def test_docker_encoding(host):
     encoding = host.check_output(
-        "python -c 'import locale;print(locale.getpreferredencoding())'"
+        "python3 -c 'import locale;print(locale.getpreferredencoding())'"
     )
-    assert encoding == "ANSI_X3.4-1968"
+    assert encoding == "UTF-8"
     string = "ťēꞩƫìṇḟřặ ṧꝕèȃǩ ửƫᵮ8"
     assert host.check_output("echo %s | tee /tmp/s.txt", string) == string
     assert host.file("/tmp/s.txt").content_string.strip() == string
 
 
 @pytest.mark.parametrize(
     "hostspec,expected",
```

### Comparing `pytest-testinfra-7.0.0/test/test_invocation.py` & `pytest-testinfra-8.0.0/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/test/test_modules.py` & `pytest-testinfra-8.0.0/test/test_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 all_images = pytest.mark.testinfra_hosts(
     *[
         "docker://{}".format(image)
         for image in (
             "alpine",
             "archlinux",
-            "centos_7",
+            "rockylinux8",
             "debian_bullseye",
             "ubuntu_xenial",
         )
     ]
 )
 
 
@@ -43,24 +43,24 @@
     else:
         name = "openssh-server"
 
     ssh = host.package(name)
     version = {
         "alpine": "8.",
         "archlinux": "9.",
-        "centos_7": "7.",
+        "rockylinux8": "8.",
         "debian_bullseye": "1:8.4",
         "ubuntu_xenial": "1:7.2",
     }[docker_image]
     assert ssh.is_installed
     assert ssh.version.startswith(version)
     release = {
         "alpine": "r3",
         "archlinux": None,
-        "centos_7": ".el7",
+        "rockylinux8": ".el8",
         "debian_bullseye": None,
         "ubuntu_xenial": None,
     }[docker_image]
     if release is None:
         with pytest.raises(NotImplementedError):
             ssh.release
     else:
@@ -69,15 +69,15 @@
 
 def test_held_package(host):
     python = host.package("python3")
     assert python.is_installed
     assert python.version.startswith("3.9.")
 
 
-@pytest.mark.testinfra_hosts("docker://centos_7")
+@pytest.mark.testinfra_hosts("docker://rockylinux8")
 def test_non_default_package_tool(host):
     # Make non default pkg tool binary present
     host.run("install -m a+rx /bin/true /usr/bin/dpkg-query")
     assert host.package("openssh").is_installed
 
 
 @pytest.mark.destructive
@@ -99,27 +99,27 @@
 @all_images
 def test_systeminfo(host, docker_image):
     assert host.system_info.type == "linux"
 
     release, distribution, codename, arch = {
         "alpine": (r"^3\.14\.", "alpine", None, "x86_64"),
         "archlinux": ("rolling", "arch", None, "x86_64"),
-        "centos_7": (r"^7$", "centos", None, "x86_64"),
+        "rockylinux8": (r"^8.\d+$", "rocky", None, "x86_64"),
         "debian_bullseye": (r"^11", "debian", "bullseye", "x86_64"),
         "ubuntu_xenial": (r"^16\.04$", "ubuntu", "xenial", "x86_64"),
     }[docker_image]
 
     assert host.system_info.distribution == distribution
     assert host.system_info.codename == codename
     assert re.match(release, host.system_info.release)
 
 
 @all_images
 def test_ssh_service(host, docker_image):
-    if docker_image in ("centos_7", "alpine", "archlinux"):
+    if docker_image in ("rockylinux8", "alpine", "archlinux"):
         name = "sshd"
     else:
         name = "ssh"
 
     ssh = host.service(name)
     if docker_image == "ubuntu_xenial":
         assert not ssh.is_running
@@ -184,14 +184,15 @@
 
 
 def test_facter(host):
     assert host.facter()["os"]["distro"]["codename"] == "bullseye"
     assert host.facter("virtual") in (
         {"virtual": "docker"},
         {"virtual": "hyperv"},  # github action uses hyperv
+        {"virtual": "physical"},  # I've this on my machine...
     )
 
 
 def test_sysctl(host):
     assert host.sysctl("kernel.hostname") == host.check_output("hostname")
     assert isinstance(host.sysctl("kernel.panic"), int)
 
@@ -245,15 +246,15 @@
         # busybox ps doesn't have a euid equivalent
         assert init.euid == 0
     assert init.user == "root"
 
     args, comm = {
         "alpine": ("/sbin/init", "init"),
         "archlinux": ("/usr/sbin/init", "systemd"),
-        "centos_7": ("/usr/sbin/init", "systemd"),
+        "rockylinux8": ("/usr/sbin/init", "systemd"),
         "debian_bullseye": ("/sbin/init", "systemd"),
         "ubuntu_xenial": ("/sbin/init", "systemd"),
     }[docker_image]
     assert init.args == args
     assert init.comm == comm
 
 
@@ -345,14 +346,24 @@
     assert link.is_symlink
     assert link.is_file
     assert link.linked_to == "/d/f"
     assert link.linked_to == f
     assert f == host.file("/d/f")
     assert not d == f
 
+    host.check_output("ln /d/f /d/h")
+    hardlink = host.file("/d/h")
+    assert hardlink.is_file
+    assert not hardlink.is_symlink
+    assert isinstance(hardlink.inode, int)
+    assert isinstance(f.inode, int)
+    assert hardlink.inode == f.inode
+    assert f == host.file("/d/f")
+    assert not d == f
+
     host.check_output("rm -f /d/p && mkfifo /d/p")
     assert host.file("/d/p").is_pipe
 
 
 def test_ansible_unavailable(host):
     expected = "Ansible module is only available with " "ansible connection backend"
     with pytest.raises(RuntimeError) as excinfo:
```

### Comparing `pytest-testinfra-7.0.0/testinfra/__init__.py` & `pytest-testinfra-8.0.0/testinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/__init__.py` & `pytest-testinfra-8.0.0/testinfra/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/ansible.py` & `pytest-testinfra-8.0.0/testinfra/backend/ansible.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/base.py` & `pytest-testinfra-8.0.0/testinfra/backend/base.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/chroot.py` & `pytest-testinfra-8.0.0/testinfra/backend/chroot.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/docker.py` & `pytest-testinfra-8.0.0/testinfra/backend/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/kubectl.py` & `pytest-testinfra-8.0.0/testinfra/backend/kubectl.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/local.py` & `pytest-testinfra-8.0.0/testinfra/backend/local.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/lxc.py` & `pytest-testinfra-8.0.0/testinfra/backend/lxc.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/openshift.py` & `pytest-testinfra-8.0.0/testinfra/backend/openshift.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/paramiko.py` & `pytest-testinfra-8.0.0/testinfra/backend/paramiko.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/podman.py` & `pytest-testinfra-8.0.0/testinfra/backend/podman.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/salt.py` & `pytest-testinfra-8.0.0/testinfra/backend/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/ssh.py` & `pytest-testinfra-8.0.0/testinfra/backend/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/backend/winrm.py` & `pytest-testinfra-8.0.0/testinfra/backend/winrm.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/host.py` & `pytest-testinfra-8.0.0/testinfra/host.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,52 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import testinfra.backend
 import testinfra.modules
+from testinfra.utils import cached_property
 
 
 class Host:
     _host_cache = {}  # type: ignore[var-annotated]
     _hosts_cache = {}  # type: ignore[var-annotated]
 
     def __init__(self, backend):
         self.backend = backend
         super().__init__()
 
     def __repr__(self):
         return "<testinfra.host.Host {}>".format(self.backend.get_pytest_id())
 
+    @cached_property
+    def has_command_v(self):
+        """Return True if `command -v` is available"""
+        return self.run("command -v command").rc == 0
+
     def exists(self, command):
         """Return True if given command exist in $PATH"""
-        rc = self.run_expect([0, 1, 127], "command -v %s", command).rc
-        if rc == 127:
-            return self.run_expect([0, 1], "which %s", command).rc == 0
+        if self.has_command_v:
+            out = self.run("command -v %s", command)
         else:
-            return rc == 0
+            out = self.run_expect([0, 1], "which %s", command)
+        return out.rc == 0
 
     def find_command(self, command, extrapaths=("/sbin", "/usr/sbin")):
         """Return path of given command
 
         raise ValueError if command cannot be found
         """
-        out = self.run_expect([0, 1, 127], "command -v %s", command)
+        if self.has_command_v:
+            out = self.run("command -v %s", command)
+        else:
+            out = self.run_expect([0, 1], "which %s", command)
         if out.rc == 0:
             return out.stdout.rstrip("\r\n")
-        if out.rc == 127:
-            out = self.run_expect([0, 1], "which %s", command)
-            if out.rc == 0:
-                return out.stdout.rstrip("\r\n")
         for basedir in extrapaths:
             path = os.path.join(basedir, command)
             if self.exists(path):
                 return path
         raise ValueError('cannot find "{}" command'.format(command))
 
     def run(self, command, *args, **kwargs):
```

### Comparing `pytest-testinfra-7.0.0/testinfra/main.py` & `pytest-testinfra-8.0.0/testinfra/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 
 import warnings
 
 import pytest
 
 
 def main():
-    warnings.warn("calling testinfra is deprecated, call py.test instead")
+    warnings.warn("calling testinfra is deprecated, call py.test instead", stacklevel=1)
     return pytest.main()
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/__init__.py` & `pytest-testinfra-8.0.0/testinfra/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/addr.py` & `pytest-testinfra-8.0.0/testinfra/modules/addr.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/ansible.py` & `pytest-testinfra-8.0.0/testinfra/modules/ansible.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/base.py` & `pytest-testinfra-8.0.0/testinfra/modules/base.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/blockdevice.py` & `pytest-testinfra-8.0.0/testinfra/modules/blockdevice.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/command.py` & `pytest-testinfra-8.0.0/testinfra/modules/command.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/docker.py` & `pytest-testinfra-8.0.0/testinfra/modules/docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         return json.loads(output)[0]
 
     @property
     def is_running(self):
         return self.inspect()["State"]["Running"]
 
     @property
+    def is_restarting(self):
+        return self.inspect()["State"]["Restarting"]
+
+    @property
     def id(self):
         return self.inspect()["Id"]
 
     @property
     def name(self):
         return self.inspect()["Name"][1:]  # get rid of slash in front
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/environment.py` & `pytest-testinfra-8.0.0/testinfra/modules/environment.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/file.py` & `pytest-testinfra-8.0.0/testinfra/modules/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,18 @@
 
         .. _oct(x): https://docs.python.org/3/library/functions.html#oct
         .. _stat: https://docs.python.org/3/library/stat.html
         """  # noqa
         raise NotImplementedError
 
     def contains(self, pattern):
+        """Checks content of file for pattern
+
+        This uses grep and thus follows the grep regex syntax.
+        """
         return self.run_test("grep -qs -- %s %s", pattern, self.path).rc == 0
 
     @property
     def md5sum(self):
         raise NotImplementedError
 
     @property
@@ -229,14 +233,18 @@
         return datetime.datetime.fromtimestamp(float(ts))
 
     @property
     def size(self):
         return int(self.check_output("stat -c %%s %s", self.path))
 
     @property
+    def inode(self):
+        return int(self.check_output("stat -c %%i %s", self.path))
+
+    @property
     def md5sum(self):
         return self.check_output("md5sum %s | cut -d' ' -f1", self.path)
 
     @property
     def sha256sum(self):
         return self.check_output("sha256sum %s | cut -d ' ' -f 1", self.path)
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/group.py` & `pytest-testinfra-8.0.0/testinfra/modules/group.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,9 +33,17 @@
 
         return self.run_expect([0, 2], "getent group %s", self.name).rc == 0
 
     @property
     def gid(self):
         return int(self.check_output("getent group %s | cut -d':' -f3", self.name))
 
+    @property
+    def members(self):
+        """Return all users that are members of this group."""
+        users = self.check_output("getent group %s | cut -d':' -f4", self.name)
+        if users:
+            return users.split(",")
+        return []
+
     def __repr__(self):
         return "<group {}>".format(self.name)
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/interface.py` & `pytest-testinfra-8.0.0/testinfra/modules/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import re
+
 from testinfra.modules.base import Module
 from testinfra.utils import cached_property
 
 
 class Interface(Module):
     """Test network interfaces
 
@@ -44,14 +47,34 @@
         """Return ipv4 and ipv6 addresses on the interface
 
         >>> host.interface("eth0").addresses
         ['192.168.31.254', '192.168.31.252', 'fe80::e291:f5ff:fe98:6b8c']
         """
         raise NotImplementedError
 
+    def routes(self, scope=None):
+        """Return the routes associated with the interface, optionally filtered by scope
+        ("host", "link" or "global").
+
+        >>> host.interface("eth0").routes()
+        [{'dst': 'default',
+        'flags': [],
+        'gateway': '192.0.2.1',
+        'metric': 3003,
+        'prefsrc': '192.0.2.5',
+        'protocol': 'dhcp'},
+        {'dst': '192.0.2.0/24',
+        'flags': [],
+        'metric': 3003,
+        'prefsrc': '192.0.2.5',
+        'protocol': 'dhcp',
+        'scope': 'link'}]
+        """
+        raise NotImplementedError
+
     def __repr__(self):
         return "<interface {}>".format(self.name)
 
     @classmethod
     def get_module_class(cls, host):
         if host.system_info.type == "linux":
             return LinuxInterface
@@ -105,21 +128,33 @@
         addrs = []
         for line in stdout.splitlines():
             splitted = [e.strip() for e in line.split(" ") if e]
             if splitted and splitted[0] in ("inet", "inet6"):
                 addrs.append(splitted[1].split("/", 1)[0])
         return addrs
 
+    def routes(self, scope=None):
+        cmd = f"{self._ip} --json route list dev %s"
+
+        if scope is None:
+            out = self.check_output(cmd, self.name)
+        else:
+            out = self.check_output(cmd + " scope %s", self.name, scope)
+
+        return json.loads(out)
+
     @classmethod
     def default(cls, family=None):
         _default = cls(None, family=family)
         out = cls.check_output("{} route ls".format(_default._ip))
         for line in out.splitlines():
             if "default" in line:
-                _default.name = line.strip().rsplit(" ", 1)[-1]
+                match = re.search(r"dev\s(\S+)", line)
+                if match:
+                    _default.name = match.group(1)
         return _default
 
     @classmethod
     def names(cls):
         # -o is to tell the ip command to return 1 line per interface
         out = cls.check_output("{} -o link show".format(cls(None)._ip))
         interfaces = []
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/iptables.py` & `pytest-testinfra-8.0.0/testinfra/modules/iptables.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/mountpoint.py` & `pytest-testinfra-8.0.0/testinfra/modules/mountpoint.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/package.py` & `pytest-testinfra-8.0.0/testinfra/modules/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         - apk (Alpine)
         - apt (Debian, Ubuntu, ...)
         - pacman (Arch, Manjaro )
         - pkg (FreeBSD)
         - pkg_info (NetBSD)
         - pkg_info (OpenBSD)
-        - rpm (RHEL, Centos, Fedora, ...)
+        - rpm (RHEL, RockyLinux, Fedora, ...)
         """
         raise NotImplementedError
 
     @property
     def release(self):
         """Return the release specific info from the package version
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/pip.py` & `pytest-testinfra-8.0.0/testinfra/modules/pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,16 @@
     """
 
     @staticmethod
     def _deprecated():
         """Raise a `DeprecationWarning`"""
         warnings.warn(
             "Calling host.pip_package is deprecated, call host.pip instead",
-            DeprecationWarning,
+            category=DeprecationWarning,
+            stacklevel=2,
         )
 
     @classmethod
     def check(cls, pip_path="pip"):
         PipPackage._deprecated()
         return super().check(pip_path=pip_path)
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/podman.py` & `pytest-testinfra-8.0.0/testinfra/modules/podman.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/process.py` & `pytest-testinfra-8.0.0/testinfra/modules/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,17 @@
     def _get_process_attribute_by_pid(self, pid, name):
         raise NotImplementedError
 
     @classmethod
     def get_module_class(cls, host):
         if host.file("/bin/ps").linked_to == "/bin/busybox":
             return BusyboxProcess
+        if host.file("/bin/busybox").exists:
+            if host.file("/bin/ps").inode == host.file("/bin/busybox").inode:
+                return BusyboxProcess
         if host.system_info.type == "linux" or host.system_info.type.endswith("bsd"):
             return PosixProcess
         raise NotImplementedError
 
     def __repr__(self):
         return "<process>"
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/puppet.py` & `pytest-testinfra-8.0.0/testinfra/modules/puppet.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/salt.py` & `pytest-testinfra-8.0.0/testinfra/modules/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/service.py` & `pytest-testinfra-8.0.0/testinfra/modules/service.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/socket.py` & `pytest-testinfra-8.0.0/testinfra/modules/socket.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/sudo.py` & `pytest-testinfra-8.0.0/testinfra/modules/sudo.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/supervisor.py` & `pytest-testinfra-8.0.0/testinfra/modules/supervisor.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/sysctl.py` & `pytest-testinfra-8.0.0/testinfra/modules/sysctl.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/systeminfo.py` & `pytest-testinfra-8.0.0/testinfra/modules/systeminfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     ("VERSION_CODENAME=", "codename"),
                 ):
                     if line.startswith(key):
                         sysinfo[attname] = (
                             line[len(key) :].replace('"', "").replace("'", "").strip()
                         )
             # Arch doesn't have releases
-            if sysinfo["distribution"] == "arch":
+            if "distribution" in sysinfo and sysinfo["distribution"] == "arch":
                 sysinfo["release"] = "rolling"
             return sysinfo
 
         # RedHat / CentOS 6 haven't /etc/os-release
         redhat_release = self.run("cat /etc/redhat-release")
         if redhat_release.rc == 0:
             match = re.match(
```

### Comparing `pytest-testinfra-7.0.0/testinfra/modules/user.py` & `pytest-testinfra-8.0.0/testinfra/modules/user.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/plugin.py` & `pytest-testinfra-8.0.0/testinfra/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         # avoid traceback in py.io.terminalwriter.write_out
         # TypeError: a bytes-like object is required, not 'str'
         if isinstance(s, str):
             s = s.encode(self._out_encoding)
         return super().write(s)
 
 
-@pytest.mark.trylast
+@pytest.hookimpl(trylast=True)
 def pytest_configure(config):
     if config.getoption("--verbose", 0) > 1:
         root = logging.getLogger()
         if not root.handlers:
             root.addHandler(logging.NullHandler())
         logging.getLogger("testinfra").setLevel(logging.DEBUG)
     if config.getoption("--nagios"):
@@ -203,12 +203,12 @@
             out = SpooledTemporaryFile(encoding=sys.stdout.encoding)
             config.pluginmanager.unregister(reporter)
             reporter = reporter.__class__(config, out)
             config.pluginmanager.register(reporter, "terminalreporter")
             config.pluginmanager.register(NagiosReporter(out), "nagiosreporter")
 
 
-@pytest.mark.trylast
+@pytest.hookimpl(trylast=True)
 def pytest_sessionfinish(session, exitstatus):
     reporter = session.config.pluginmanager.getplugin("nagiosreporter")
     if reporter:
         session.exitstatus = reporter.report()
```

### Comparing `pytest-testinfra-7.0.0/testinfra/utils/__init__.py` & `pytest-testinfra-8.0.0/testinfra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/testinfra/utils/ansible_runner.py` & `pytest-testinfra-8.0.0/testinfra/utils/ansible_runner.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-7.0.0/tox.ini` & `pytest-testinfra-8.0.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 [tox]
+minversion = 4.0.16
 envlist=
   lint
-  py{36,37,38,39,310}
-  doc
+  py
+  docs
   packaging
 
 [testenv]
 description = Runs unittests
 deps=
     -rtest-requirements.txt
 commands=
-    {envpython} -m mypy testinfra test
     {envpython} -m pytest {posargs:-v -n 4 --cov testinfra --cov-report xml --cov-report term test}
 usedevelop=True
-passenv=HOME TRAVIS DOCKER_CERT_PATH DOCKER_HOST DOCKER_TLS_VERIFY WSL_DISTRO_NAME
+passenv=
+    HOME
+    TRAVIS
+    DOCKER_CERT_PATH
+    DOCKER_HOST
+    DOCKER_TLS_VERIFY
+    WSL_DISTRO_NAME
 
 [testenv:lint]
 description = Performs linting tasks
-deps=
-  flake8
-  hacking>=4.0
-  flake8-bugbear
-  flake8-comprehensions
-  flake8-debugger
-  flake8-logging-format
-  flake8-pep3101
-  flake8-print
-  black
-  isort
+deps =
+    pre-commit>=2.6.0
 commands=
-  black --check --diff {toxinidir}
-  isort --check --diff testinfra test setup.py
-  flake8 {posargs}
+  pre-commit run -a
 
 [testenv:docs]
 deps=-rdev-requirements.txt
 commands=sphinx-build -W -b html doc/source doc/build
 
 [testenv:packaging]
 description = Validate project packaging
```

