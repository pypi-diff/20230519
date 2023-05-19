# Comparing `tmp/np_envs-0.1.2.tar.gz` & `tmp/np_envs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_envs-0.1.2.tar", last modified: Fri May 19 04:36:22 2023, max compression
+gzip compressed data, was "np_envs-0.1.3.tar", last modified: Fri May 19 05:24:31 2023, max compression
```

## Comparing `np_envs-0.1.2.tar` & `np_envs-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.2/README.md
--rw-r--r--   0        0        0      472 2023-05-19 04:36:22.047697 np_envs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.2/src/np_envs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.2/src/np_envs/__main__.py
--rw-r--r--   0        0        0     1246 2023-05-19 04:35:25.235779 np_envs-0.1.2/src/np_envs/config.py
--rw-r--r--   0        0        0     6732 2023-05-19 04:34:42.478746 np_envs-0.1.2/src/np_envs/env.py
--rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.2/src/np_envs/pip.ini
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-05-18 06:03:05.768579 np_envs-0.1.3/README.md
+-rw-r--r--   0        0        0      541 2023-05-19 05:24:31.705913 np_envs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-18 07:49:42.185517 np_envs-0.1.3/src/np_envs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 06:08:40.452037 np_envs-0.1.3/src/np_envs/__main__.py
+-rw-r--r--   0        0        0     1246 2023-05-19 04:35:25.235779 np_envs-0.1.3/src/np_envs/config.py
+-rw-r--r--   0        0        0     6915 2023-05-19 05:15:50.702210 np_envs-0.1.3/src/np_envs/env.py
+-rw-r--r--   0        0        0       87 2023-05-18 05:48:25.501423 np_envs-0.1.3/src/np_envs/pip.ini
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 np_envs-0.1.3/PKG-INFO
```

### Comparing `np_envs-0.1.2/src/np_envs/config.py` & `np_envs-0.1.3/src/np_envs/config.py`

 * *Files identical despite different names*

### Comparing `np_envs-0.1.2/src/np_envs/env.py` & `np_envs-0.1.3/src/np_envs/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,23 +82,22 @@
     @property
     def pip_ini(self) -> pathlib.Path:
         return self.root / 'pip.ini'
 
     @property
     def pip_cache(self) -> pathlib.Path:
         """Shared cache, across versions and across env types (not platforms)."""
-        return config.ROOT / 'pip_cache'
+        return config.ROOT / '.pip-cache'
     
     @property 
     def pip_ini_config(self) -> configparser.ConfigParser:
         pip_ini_config = configparser.ConfigParser()
         pip_ini_config.read_dict(
-            config.PROJECT_TO_PIP_CONFIG.get(self.name),
-            config.PROJECT_TO_PIP_CONFIG['default'],
-        )
+                config.PROJECT_TO_PIP_CONFIG.get(self.name, config.PROJECT_TO_PIP_CONFIG['default'])
+            )
         pip_ini_config.set('global', 'cache-dir', np_config.normalize_path(self.pip_cache).as_posix())
         return pip_ini_config
     
     def add_pip_config(self):
         if not self.root.exists():
             raise FileNotFoundError(f'Cannot add pip config: {self.root} does not exist')
         if not self.pip_ini.parent.exists():
@@ -160,14 +159,17 @@
         if not conda_env.python.exists():
             conda_env.create('--no-default-packages')
         subprocess.run(
             f'{conda_env.python} -m venv --copies {self.root} {" ".join(args)}',
             check=True,
             )
 
+    def activate(self):
+        activate_file = self.root / ('Scripts' if ON_WINDOWS else 'bin') / 'activate_this.py'
+        exec(activate_file.read_text(), {'__file__': activate_file})
     
 class EnvPath(pathlib.WindowsPath if ON_WINDOWS else pathlib.PosixPath): # type: ignore
     """
     >>> env = EnvPath('np_pipeline_qc')
     """
 
     version: str
```

