# Comparing `tmp/makim-1.7.1.tar.gz` & `tmp/makim-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makim-1.7.1.tar", max compression
+gzip compressed data, was "makim-1.8.0.tar", max compression
```

## Comparing `makim-1.7.1.tar` & `makim-1.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       88 2023-05-19 01:41:27.435666 makim-1.7.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      316 2023-05-19 01:41:27.435666 makim-1.7.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1395 2023-05-19 01:41:27.435666 makim-1.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     3893 2023-05-19 01:41:27.435666 makim-1.7.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1781 2023-05-19 01:41:27.435666 makim-1.7.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1886 2023-05-19 01:41:27.439666 makim-1.7.1/.gitignore
--rw-r--r--   0        0        0     8018 2023-05-19 01:41:27.439666 makim-1.7.1/.makim.yaml
--rw-r--r--   0        0        0     1095 2023-05-19 01:41:27.439666 makim-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1854 2023-05-19 01:41:27.439666 makim-1.7.1/.releaserc.json
--rw-r--r--   0        0        0     1514 2023-05-19 01:41:27.439666 makim-1.7.1/LICENSE
--rw-r--r--   0        0        0     3409 2023-05-19 01:41:27.439666 makim-1.7.1/README.md
--rw-r--r--   0        0        0      253 2023-05-19 01:41:27.439666 makim-1.7.1/conda/dev.yaml
--rw-r--r--   0        0        0     5772 2023-05-19 01:44:56.814768 makim-1.7.1/docs/changelog.md
--rw-r--r--   0        0        0     5253 2023-05-19 01:41:27.439666 makim-1.7.1/docs/contributing.md
--rw-r--r--   0        0        0    72342 2023-05-19 01:41:27.439666 makim-1.7.1/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-05-19 01:41:27.439666 makim-1.7.1/docs/images/logo.png
--rw-r--r--   0        0        0     1083 2023-05-19 01:41:27.439666 makim-1.7.1/docs/installation.md
--rw-r--r--   0        0        0     3832 2023-05-19 01:41:27.439666 makim-1.7.1/docs/mkdocs.yaml
--rw-r--r--   0        0        0      194 2023-05-19 01:44:56.802768 makim-1.7.1/makim/__init__.py
--rw-r--r--   0        0        0     4746 2023-05-19 01:41:27.439666 makim-1.7.1/makim/__main__.py
--rw-r--r--   0        0        0      343 2023-05-19 01:41:27.439666 makim-1.7.1/makim/error.py
--rw-r--r--   0        0        0    12787 2023-05-19 01:41:27.439666 makim-1.7.1/makim/makim.py
--rw-r--r--   0        0        0   153976 2023-05-19 01:44:21.710267 makim-1.7.1/poetry.lock
--rw-r--r--   0        0        0     1676 2023-05-19 01:44:56.802768 makim-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 makim-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0       88 2023-05-19 14:33:34.440946 makim-1.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      316 2023-05-19 14:33:34.440946 makim-1.8.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1395 2023-05-19 14:33:34.440946 makim-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     3893 2023-05-19 14:33:34.440946 makim-1.8.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1781 2023-05-19 14:33:34.440946 makim-1.8.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1886 2023-05-19 14:33:34.440946 makim-1.8.0/.gitignore
+-rw-r--r--   0        0        0     8018 2023-05-19 14:33:34.440946 makim-1.8.0/.makim.yaml
+-rw-r--r--   0        0        0     1095 2023-05-19 14:33:34.440946 makim-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1854 2023-05-19 14:33:34.440946 makim-1.8.0/.releaserc.json
+-rw-r--r--   0        0        0     1514 2023-05-19 14:33:34.440946 makim-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3409 2023-05-19 14:33:34.440946 makim-1.8.0/README.md
+-rw-r--r--   0        0        0      253 2023-05-19 14:33:34.440946 makim-1.8.0/conda/dev.yaml
+-rw-r--r--   0        0        0     6113 2023-05-19 14:37:02.635891 makim-1.8.0/docs/changelog.md
+-rw-r--r--   0        0        0     5253 2023-05-19 14:33:34.440946 makim-1.8.0/docs/contributing.md
+-rw-r--r--   0        0        0    72342 2023-05-19 14:33:34.440946 makim-1.8.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-05-19 14:33:34.440946 makim-1.8.0/docs/images/logo.png
+-rw-r--r--   0        0        0     1083 2023-05-19 14:33:34.440946 makim-1.8.0/docs/installation.md
+-rw-r--r--   0        0        0     3832 2023-05-19 14:33:34.440946 makim-1.8.0/docs/mkdocs.yaml
+-rw-r--r--   0        0        0      194 2023-05-19 14:37:02.623890 makim-1.8.0/makim/__init__.py
+-rw-r--r--   0        0        0     4746 2023-05-19 14:33:34.440946 makim-1.8.0/makim/__main__.py
+-rw-r--r--   0        0        0      343 2023-05-19 14:33:34.440946 makim-1.8.0/makim/error.py
+-rw-r--r--   0        0        0    12919 2023-05-19 14:33:34.440946 makim-1.8.0/makim/makim.py
+-rw-r--r--   0        0        0   153976 2023-05-19 14:36:29.467381 makim-1.8.0/poetry.lock
+-rw-r--r--   0        0        0     1676 2023-05-19 14:37:02.627890 makim-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 makim-1.8.0/PKG-INFO
```

### Comparing `makim-1.7.1/.github/PULL_REQUEST_TEMPLATE.md` & `makim-1.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.github/workflows/main.yaml` & `makim-1.8.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.github/workflows/release.yaml` & `makim-1.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.gitignore` & `makim-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.makim.yaml` & `makim-1.8.0/.makim.yaml`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.pre-commit-config.yaml` & `makim-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/.releaserc.json` & `makim-1.8.0/.releaserc.json`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/LICENSE` & `makim-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/README.md` & `makim-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/docs/changelog.md` & `makim-1.8.0/docs/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Release Notes
 ---
 
+# [1.8.0](https://github.com/osl-incubator/makim/compare/1.7.1...1.8.0) (2023-05-19)
+
+
+### Features
+
+* by default, for Xonsh shell, stop the target process if any command line fails ([#19](https://github.com/osl-incubator/makim/issues/19)) ([8fa4c1d](https://github.com/osl-incubator/makim/commit/8fa4c1ddb19af2ef215509feff2dd4055ca47561))
+
 ## [1.7.1](https://github.com/osl-incubator/makim/compare/1.7.0...1.7.1) (2023-05-19)
 
 
 ### Bug Fixes
 
 * Fix release workflow and broken dependencies ([#40](https://github.com/osl-incubator/makim/issues/40)) ([c77c6f9](https://github.com/osl-incubator/makim/commit/c77c6f96f4b550e8bafe6d877719bb137d40aa11)), closes [/github.com/ionrock/cachecontrol/issues/292#issuecomment-1536120527](https://github.com//github.com/ionrock/cachecontrol/issues/292/issues/issuecomment-1536120527)
```

### Comparing `makim-1.7.1/docs/contributing.md` & `makim-1.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/docs/images/favicon.ico` & `makim-1.8.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/docs/images/logo.png` & `makim-1.8.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/docs/installation.md` & `makim-1.8.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/docs/mkdocs.yaml` & `makim-1.8.0/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/makim/__main__.py` & `makim-1.8.0/makim/__main__.py`

 * *Files identical despite different names*

### Comparing `makim-1.7.1/makim/makim.py` & `makim-1.8.0/makim/makim.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from colorama import Fore
 from jinja2 import Template
 
 from makim.error import MakimError
 
 
 def escape_template_tag(v: str) -> str:
-    return str(v).replace('{{', r'\{\{').replace('}}', r'\}\}')
+    return v.replace('{{', r'\{\{').replace('}}', r'\}\}')
 
 
 def unescape_template_tag(v: str) -> str:
-    return str(v).replace(r'\{\{', '{{').replace(r'\}\}', '}}')
+    return v.replace(r'\{\{', '{{').replace(r'\}\}', '}}')
 
 
 class PrintPlugin:
     def _print_error(self, message: str):
         print(Fore.RED, message, Fore.RESET, file=sys.stderr)
 
     def _print_info(self, message: str):
@@ -46,14 +46,18 @@
     env: dict = {}
     args: Optional[object] = None
     group_name: str = 'default'
     group_data: dict = {}
     target_name: str = ''
     target_data: dict = {}
 
+    def __init__(self):
+        os.environ['RAISE_SUBPROC_ERROR'] = '1'
+        os.environ['XONSH_SHOW_TRACEBACK'] = '0'
+
     def _call_shell_app(self, cmd):
         fd, filepath = tempfile.mkstemp(suffix='.makim', text=True)
 
         with open(filepath, 'w') as f:
             f.write(cmd)
 
         p = self.shell_app(
@@ -198,30 +202,30 @@
 
         for dep_data in self.target_data['dependencies']:
             args_dep = {}
 
             # update the arguments
             for arg_name, arg_value in dep_data.get('args', {}).items():
                 unescaped_value = (
-                    unescape_template_tag(arg_value)
+                    unescape_template_tag(str(arg_value))
                     if isinstance(arg_value, str)
                     else str(arg_value)
                 )
 
                 args_dep[f'--{arg_name}'] = yaml.safe_load(
                     Template(unescaped_value).render(args=original_args_clean)
                 )
 
             args_dep['target'] = dep_data['target']
             args_dep.update(args_dep_original)
 
             # checking for the conditional statement
             if_stmt = dep_data.get('if')
             if if_stmt:
-                result = Template(unescape_template_tag(if_stmt)).render(
+                result = Template(unescape_template_tag(str(if_stmt))).render(
                     args=original_args_clean
                 )
                 if not yaml.safe_load(result):
                     if args.get('verbose'):
                         self._print_info(
                             '[II] Skipping dependency: '
                             f'{dep_data.get("target")}'
@@ -293,21 +297,21 @@
             (
                 self.target_data.get('env', {}),
                 self._load_dotenv(self.target_data),
             ),
         ]:
             env.update(env_file)
             for k, v in env_user.items():
-                env[k] = Template(unescape_template_tag(v)).render(
+                env[k] = Template(unescape_template_tag(str(v))).render(
                     args=args_input, env=env, vars=variables
                 )
         for k, v in env.items():
             os.environ[k] = v
 
-        cmd = unescape_template_tag(cmd)
+        cmd = unescape_template_tag(str(cmd))
         cmd = Template(cmd).render(args=args_input, env=env, vars=variables)
         if args.get('verbose'):
             self._print_info('=' * 80)
             self._print_info(
                 'TARGET: ' + f'{self.group_name}.{self.target_name}'
             )
             self._print_info('ARGS:')
```

### Comparing `makim-1.7.1/poetry.lock` & `makim-1.8.0/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -9457,63 +9457,63 @@
 00024f00: 6134 3665 3466 3536 3536 6362 6565 3737  a46e4f5656cbee77
 00024f10: 3338 3837 3322 7d2c 0a5d 0a0a 5b70 6163  38873"},.]..[pac
 00024f20: 6b61 6765 2e65 7874 7261 735d 0a74 6573  kage.extras].tes
 00024f30: 7420 3d20 5b22 7079 7465 7374 2028 3e3d  t = ["pytest (>=
 00024f40: 362e 302e 3029 225d 0a0a 5b5b 7061 636b  6.0.0)"]..[[pack
 00024f50: 6167 655d 5d0a 6e61 6d65 203d 2022 786f  age]].name = "xo
 00024f60: 6e73 6822 0a76 6572 7369 6f6e 203d 2022  nsh".version = "
-00024f70: 302e 3133 2e34 220a 6465 7363 7269 7074  0.13.4".descript
+00024f70: 302e 3134 2e30 220a 6465 7363 7269 7074  0.14.0".descript
 00024f80: 696f 6e20 3d20 2250 7974 686f 6e2d 706f  ion = "Python-po
 00024f90: 7765 7265 642c 2063 726f 7373 2d70 6c61  wered, cross-pla
 00024fa0: 7466 6f72 6d2c 2055 6e69 782d 6761 7a69  tform, Unix-gazi
 00024fb0: 6e67 2073 6865 6c6c 220a 6361 7465 676f  ng shell".catego
 00024fc0: 7279 203d 2022 6d61 696e 220a 6f70 7469  ry = "main".opti
 00024fd0: 6f6e 616c 203d 2066 616c 7365 0a70 7974  onal = false.pyt
 00024fe0: 686f 6e2d 7665 7273 696f 6e73 203d 2022  hon-versions = "
 00024ff0: 3e3d 332e 3822 0a66 696c 6573 203d 205b  >=3.8".files = [
 00025000: 0a20 2020 207b 6669 6c65 203d 2022 786f  .    {file = "xo
-00025010: 6e73 682d 302e 3133 2e34 2d70 7933 3130  nsh-0.13.4-py310
+00025010: 6e73 682d 302e 3134 2e30 2d70 7933 3130  nsh-0.14.0-py310
 00025020: 2d6e 6f6e 652d 616e 792e 7768 6c22 2c20  -none-any.whl", 
-00025030: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
-00025040: 6134 3566 3631 3736 3832 6364 3163 6338  a45f617682cd1cc8
-00025050: 6232 3063 6337 6361 3061 6437 3133 6637  b20cc7ca0ad713f7
-00025060: 3666 3863 6131 3264 3537 3833 6566 3434  6f8ca12d5783ef44
-00025070: 3235 6434 6363 6134 3061 3631 3962 3322  25d4cca40a619b3"
+00025030: 6861 7368 203d 2022 7368 6132 3536 3a37  hash = "sha256:7
+00025040: 3235 3036 6336 6463 3439 3431 3033 6466  2506c6dc494103df
+00025050: 3664 3034 3436 3765 3132 3761 6264 6462  6d04467e127abddb
+00025060: 3163 3663 6265 3035 6363 3539 3033 6236  1c6cbe05cc5903b6
+00025070: 6134 6362 6662 6164 3231 3766 6635 6422  a4cbfbad217ff5d"
 00025080: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00025090: 786f 6e73 682d 302e 3133 2e34 2d70 7933  xonsh-0.13.4-py3
+00025090: 786f 6e73 682d 302e 3134 2e30 2d70 7933  xonsh-0.14.0-py3
 000250a0: 3131 2d6e 6f6e 652d 616e 792e 7768 6c22  11-none-any.whl"
 000250b0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-000250c0: 3a38 3334 6463 6331 3535 3031 3236 3634  :834dcc155012664
-000250d0: 3732 6137 3638 3538 3262 3538 3864 3765  72a768582b588d7e
-000250e0: 3636 3239 6666 3533 6339 3134 3634 3937  6629ff53c9146497
-000250f0: 3930 3635 3539 3434 3937 3739 6532 3238  906559449779e228
-00025100: 3222 7d2c 0a20 2020 207b 6669 6c65 203d  2"},.    {file =
-00025110: 2022 786f 6e73 682d 302e 3133 2e34 2d70   "xonsh-0.13.4-p
+000250c0: 3a36 3738 6136 3536 3731 6264 3061 3632  :678a65671bd0a62
+000250d0: 6364 6334 3365 3933 3264 3661 6563 6338  cdc43e932d6aecc8
+000250e0: 6231 3632 3261 6131 3839 3432 6530 6166  b1622aa18942e0af
+000250f0: 6233 3838 6238 6238 6165 3032 6636 3761  b388b8b8ae02f67a
+00025100: 3522 7d2c 0a20 2020 207b 6669 6c65 203d  5"},.    {file =
+00025110: 2022 786f 6e73 682d 302e 3134 2e30 2d70   "xonsh-0.14.0-p
 00025120: 7933 382d 6e6f 6e65 2d61 6e79 2e77 686c  y38-none-any.whl
 00025130: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-00025140: 363a 3761 3433 3164 3432 3939 6231 6536  6:7a431d4299b1e6
-00025150: 6261 3934 3231 3432 3139 3934 6333 3533  ba9421421994c353
-00025160: 3265 3261 6438 3933 6266 3336 6538 3435  2e2ad893bf36e845
-00025170: 3562 3439 6133 6361 3261 6235 6362 3339  5b49a3ca2ab5cb39
-00025180: 6461 227d 2c0a 2020 2020 7b66 696c 6520  da"},.    {file 
-00025190: 3d20 2278 6f6e 7368 2d30 2e31 332e 342d  = "xonsh-0.13.4-
+00025140: 363a 3235 3937 3665 6463 3536 3935 6662  6:25976edc5695fb
+00025150: 3538 3036 6238 6232 3366 3338 3466 6634  5806b8b23f384ff4
+00025160: 3865 3631 3865 3037 6634 3539 3665 6330  8e618e07f4596ec0
+00025170: 3830 3630 3037 6636 3331 3232 3931 3761  806007f63122917a
+00025180: 3833 227d 2c0a 2020 2020 7b66 696c 6520  83"},.    {file 
+00025190: 3d20 2278 6f6e 7368 2d30 2e31 342e 302d  = "xonsh-0.14.0-
 000251a0: 7079 3339 2d6e 6f6e 652d 616e 792e 7768  py39-none-any.wh
 000251b0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-000251c0: 3536 3a34 6165 3137 6261 6362 3731 3664  56:4ae17bacb716d
-000251d0: 3833 3234 3266 6331 6134 6362 6462 3531  83242fc1a4cbdb51
-000251e0: 3966 3161 6434 3366 3361 3339 3430 6130  9f1ad43f3a3940a0
-000251f0: 3239 3663 3462 3966 3130 3834 3130 6335  296c4b9f108410c5
-00025200: 6130 6322 7d2c 0a20 2020 207b 6669 6c65  a0c"},.    {file
-00025210: 203d 2022 786f 6e73 682d 302e 3133 2e34   = "xonsh-0.13.4
+000251c0: 3536 3a37 3531 6236 3135 3732 3664 3233  56:751b615726d23
+000251d0: 3232 6434 3363 3831 3636 6164 3462 6335  22d43c8166ad4bc5
+000251e0: 6362 6536 3564 3033 6133 3732 3866 3138  cbe65d03a3728f18
+000251f0: 3337 6161 3032 3338 3066 6139 6661 6462  37aa02380fa9fadb
+00025200: 3138 3922 7d2c 0a20 2020 207b 6669 6c65  189"},.    {file
+00025210: 203d 2022 786f 6e73 682d 302e 3134 2e30   = "xonsh-0.14.0
 00025220: 2e74 6172 2e67 7a22 2c20 6861 7368 203d  .tar.gz", hash =
-00025230: 2022 7368 6132 3536 3a31 3037 3534 3532   "sha256:1075452
-00025240: 6536 6561 6339 6635 3863 3361 6266 3461  e6eac9f58c3abf4a
-00025250: 6439 6633 3866 3962 3035 3435 3265 3734  d9f38f9b05452e74
-00025260: 3630 3533 3662 6339 3933 6462 6139 3938  60536bc993dba998
-00025270: 3932 3237 6132 3161 3722 7d2c 0a5d 0a0a  9227a21a7"},.]..
+00025230: 2022 7368 6132 3536 3a34 3561 3861 6161   "sha256:45a8aaa
+00025240: 6262 3137 6365 3064 3664 3465 6361 3962  bb17ce0d6d4eca9b
+00025250: 3730 3965 6366 6437 6365 3163 3866 6239  709ecfd7ce1c8fb9
+00025260: 3231 3632 6465 6364 3239 6134 3562 6638  2162decd29a45bf8
+00025270: 3861 3630 6539 6266 3122 7d2c 0a5d 0a0a  8a60e9bf1"},.]..
 00025280: 5b70 6163 6b61 6765 2e65 7874 7261 735d  [package.extras]
 00025290: 0a62 6573 7473 6865 6c6c 203d 205b 2270  .bestshell = ["p
 000252a0: 726f 6d70 742d 746f 6f6c 6b69 7420 283e  rompt-toolkit (>
 000252b0: 3d33 2e30 2e32 3929 222c 2022 7079 676d  =3.0.29)", "pygm
 000252c0: 656e 7473 2028 3e3d 322e 3229 225d 0a64  ents (>=2.2)"].d
 000252d0: 6576 203d 205b 2270 7265 2d63 6f6d 6d69  ev = ["pre-commi
 000252e0: 7422 2c20 2272 652d 7665 7222 2c20 2274  t", "re-ver", "t
@@ -9613,12 +9613,12 @@
 000258c0: 2270 7974 6573 742d 666c 616b 6538 222c  "pytest-flake8",
 000258d0: 2022 7079 7465 7374 2d6d 7970 7920 283e   "pytest-mypy (>
 000258e0: 3d30 2e39 2e31 2922 5d0a 0a5b 6d65 7461  =0.9.1)"]..[meta
 000258f0: 6461 7461 5d0a 6c6f 636b 2d76 6572 7369  data].lock-versi
 00025900: 6f6e 203d 2022 322e 3022 0a70 7974 686f  on = "2.0".pytho
 00025910: 6e2d 7665 7273 696f 6e73 203d 2022 5e33  n-versions = "^3
 00025920: 2e38 2e31 220a 636f 6e74 656e 742d 6861  .8.1".content-ha
-00025930: 7368 203d 2022 3237 6337 6239 6566 6534  sh = "27c7b9efe4
-00025940: 3362 3732 3535 6532 6535 3862 6435 3563  3b7255e2e58bd55c
-00025950: 6135 3336 3335 3061 6637 3864 6466 6661  a536350af78ddffa
-00025960: 3465 3434 3336 3035 3637 3662 6436 6438  4e443605676bd6d8
-00025970: 3432 3166 3266 220a                      421f2f".
+00025930: 7368 203d 2022 3863 3363 6632 3263 3962  sh = "8c3cf22c9b
+00025940: 6464 3930 3934 6236 6636 6235 3530 3839  dd9094b6f6b55089
+00025950: 3263 3432 6339 6364 6636 3362 3363 3634  2c42c9cdf63b3c64
+00025960: 3939 3265 3731 3238 3934 3166 3035 3836  992e7128941f0586
+00025970: 6364 6137 6466 220a                      cda7df".
```

### Comparing `makim-1.7.1/pyproject.toml` & `makim-1.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makim"
-version = "1.7.1"  # semantic-release
+version = "1.8.0"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 repository = "https://github.com/osl-incubator/makim"
 homepage = "https://github.com/osl-incubator/makim"
 readme = "README.md"
 include = [
@@ -40,15 +40,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 sh = "^2.0.0"
 pyyaml = "<6.0"
 jinja2 = "<3.0.3"
-xonsh = "^0.13.4"
+xonsh = "^0.14.0"
 python-dotenv = "^0.21.1"
 colorama = "^0.4.6"
 urllib3 = "<2"
 
 [tool.poetry.dev-dependencies]
 containers-sugar = "1.5.0"
 pytest = "^7"
```

### Comparing `makim-1.7.1/PKG-INFO` & `makim-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makim
-Version: 1.7.1
+Version: 1.8.0
 Summary: Simplify the usage of containers
 Home-page: https://github.com/osl-incubator/makim
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: jinja2 (<3.0.3)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: pyyaml (<6.0)
 Requires-Dist: sh (>=2.0.0,<3.0.0)
 Requires-Dist: urllib3 (<2)
-Requires-Dist: xonsh (>=0.13.4,<0.14.0)
+Requires-Dist: xonsh (>=0.14.0,<0.15.0)
 Project-URL: Repository, https://github.com/osl-incubator/makim
 Description-Content-Type: text/markdown
 
 # MakIm
 
 `MakIm` or just `makim` is based on `make` and focus on improve
 the way to define targets and dependencies. Instead of using the
```

