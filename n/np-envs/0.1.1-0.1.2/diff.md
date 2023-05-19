# Comparing `tmp/np_envs-0.1.1.tar.gz` & `tmp/np_envs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_envs-0.1.1.tar", last modified: Fri May 19 01:11:21 2023, max compression
+gzip compressed data, was "np_envs-0.1.2.tar", last modified: Fri May 19 04:36:22 2023, max compression
```

## Comparing `np_envs-0.1.1.tar` & `np_envs-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.1/README.md
--rw-r--r--   0        0        0      472 2023-05-19 01:11:21.691843 np_envs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.1/src/np_envs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.1/src/np_envs/__main__.py
--rw-r--r--   0        0        0     1220 2023-05-19 01:01:20.125885 np_envs-0.1.1/src/np_envs/config.py
--rw-r--r--   0        0        0     6736 2023-05-19 01:09:52.002710 np_envs-0.1.1/src/np_envs/env.py
--rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.1/src/np_envs/pip.ini
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.2/README.md
+-rw-r--r--   0        0        0      472 2023-05-19 04:36:22.047697 np_envs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.2/src/np_envs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.2/src/np_envs/__main__.py
+-rw-r--r--   0        0        0     1246 2023-05-19 04:35:25.235779 np_envs-0.1.2/src/np_envs/config.py
+-rw-r--r--   0        0        0     6732 2023-05-19 04:34:42.478746 np_envs-0.1.2/src/np_envs/env.py
+-rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.2/src/np_envs/pip.ini
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.2/PKG-INFO
```

### Comparing `np_envs-0.1.1/src/np_envs/config.py` & `np_envs-0.1.2/src/np_envs/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from typing import Any
 
 import np_config
 import np_logging
 
 logger = np_logging.getLogger(__name__)
 
-ZK_CONFIG_NODE = '/projects/np_envs'
+ZK_CONFIG_NODE = '/projects/np_envs' 
 CONFIG = np_config.fetch(ZK_CONFIG_NODE)
-ROOT = pathlib.Path(CONFIG['root']) / ('win' if sys.platform == 'win32' else 'unix')
+
+ROOT = pathlib.Path(CONFIG['root'])
+PLATFORM_ROOT = ROOT / ('win' if sys.platform == 'win32' else 'unix')
+REQUIREMENTS_TXT_ROOT = PLATFORM_ROOT / CONFIG['requirements_txt_dir_relative_to_root']
+"""Where pip requirements are stored. Might not be possible to store in yaml
+for ZooKeeper, so we just use txt files"""
+
 PROJECT_TO_PIP_CONFIG: dict[str, dict] = CONFIG['pip_ini']
 PROJECT_TO_PYTHON_VERSION: dict[str, str] = CONFIG['python_versions']
 DEFAULT_PYTHON_VERSION = PROJECT_TO_PYTHON_VERSION['default']
 """Should be compatible with the most common `np_*` packages in use."""
-REQUIREMENTS_TXT_ROOT = ROOT.parent / CONFIG['requirements_txt_dir_relative_to_root']
-"""Where pip requirements are stored. Might not be possible to store in yaml
-for ZooKeeper, so we just use txt files"""
 
 def add_or_update_config(new_config: dict[str, Any]) -> None:
     logger.debug('Adding or updating %s in ZooKeeper node %s', new_config, ZK_CONFIG_NODE)
     np_config.to_zk(np_config.merge(CONFIG, new_config), ZK_CONFIG_NODE)
     logger.info('Updated ZooKeeper config')
     
 def add_default_python_version(env_name: str, python_version: str) -> None:
```

### Comparing `np_envs-0.1.1/src/np_envs/env.py` & `np_envs-0.1.2/src/np_envs/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     @property
     def pip_ini(self) -> pathlib.Path:
         return self.root / 'pip.ini'
 
     @property
     def pip_cache(self) -> pathlib.Path:
         """Shared cache, across versions and across env types (not platforms)."""
-        return self.project_root.parent / 'pip_cache'
+        return config.ROOT / 'pip_cache'
     
     @property 
     def pip_ini_config(self) -> configparser.ConfigParser:
         pip_ini_config = configparser.ConfigParser()
         pip_ini_config.read_dict(
             config.PROJECT_TO_PIP_CONFIG.get(self.name),
             config.PROJECT_TO_PIP_CONFIG['default'],
@@ -170,15 +170,15 @@
     >>> env = EnvPath('np_pipeline_qc')
     """
 
     version: str
     """Python version to used for any envs, e.g. '3.8.5' or '3.8.*'."""
     
     def __new__(cls, env_name: str, **kwargs):
-        path = config.ROOT / env_name
+        path = config.PLATFORM_ROOT / env_name
         return super().__new__(cls, path, **kwargs)
     
     def __init__(self, *args, python_version: str | None = None, **kwargs):
         if python_version is None:
             python_version = config.PROJECT_TO_PYTHON_VERSION[self.name]
         self.version = python_version
```

