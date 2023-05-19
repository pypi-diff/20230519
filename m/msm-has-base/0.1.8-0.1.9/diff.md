# Comparing `tmp/msm_has_base-0.1.8.tar.gz` & `tmp/msm_has_base-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msm_has_base-0.1.8.tar", max compression
+gzip compressed data, was "msm_has_base-0.1.9.tar", max compression
```

## Comparing `msm_has_base-0.1.8.tar` & `msm_has_base-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-01-14 02:56:07.609280 msm_has_base-0.1.8/msm_has_base/__init__.py
--rw-r--r--   0        0        0     1414 2023-02-01 08:46:31.558851 msm_has_base-0.1.8/msm_has_base/apdu.py
--rw-r--r--   0        0        0     3797 2023-02-01 08:46:53.526561 msm_has_base-0.1.8/msm_has_base/bc_reader.py
--rw-r--r--   0        0        0      803 2023-02-01 08:47:16.917563 msm_has_base-0.1.8/msm_has_base/card_reader.py
--rw-r--r--   0        0        0     1596 2023-01-14 02:56:16.497879 msm_has_base-0.1.8/msm_has_base/epp.py
--rw-r--r--   0        0        0     4989 2023-02-01 08:57:21.525373 msm_has_base-0.1.8/msm_has_base/pboc.py
--rw-r--r--   0        0        0     1758 2023-02-06 06:49:11.076872 msm_has_base-0.1.8/msm_has_base/pos.py
--rw-r--r--   0        0        0     3495 2023-02-01 08:47:38.900189 msm_has_base-0.1.8/msm_has_base/pos_ccb.py
--rw-r--r--   0        0        0    12829 2023-01-14 02:56:25.321004 msm_has_base-0.1.8/msm_has_base/tlv.py
--rw-r--r--   0        0        0      218 2023-02-01 08:47:57.556821 msm_has_base-0.1.8/msm_has_base/utils.py
--rw-r--r--   0        0        0      626 2023-02-06 06:49:23.860752 msm_has_base-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-07 09:19:20.201822 msm_has_base-0.1.8/README.md
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 msm_has_base-0.1.8/setup.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 msm_has_base-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-14 02:56:07.609280 msm_has_base-0.1.9/msm_has_base/__init__.py
+-rw-r--r--   0        0        0     1414 2023-02-01 08:46:31.558851 msm_has_base-0.1.9/msm_has_base/apdu.py
+-rw-r--r--   0        0        0     3797 2023-02-01 08:46:53.526561 msm_has_base-0.1.9/msm_has_base/bc_reader.py
+-rw-r--r--   0        0        0      803 2023-02-01 08:47:16.917563 msm_has_base-0.1.9/msm_has_base/card_reader.py
+-rw-r--r--   0        0        0     1596 2023-01-14 02:56:16.497879 msm_has_base-0.1.9/msm_has_base/epp.py
+-rw-r--r--   0        0        0     4989 2023-02-01 08:57:21.525373 msm_has_base-0.1.9/msm_has_base/pboc.py
+-rw-r--r--   0        0        0     1754 2023-02-07 07:46:44.410367 msm_has_base-0.1.9/msm_has_base/pos.py
+-rw-r--r--   0        0        0     3576 2023-02-13 01:29:24.830127 msm_has_base-0.1.9/msm_has_base/pos_ccb.py
+-rw-r--r--   0        0        0    12829 2023-01-14 02:56:25.321004 msm_has_base-0.1.9/msm_has_base/tlv.py
+-rw-r--r--   0        0        0      218 2023-02-01 08:47:57.556821 msm_has_base-0.1.9/msm_has_base/utils.py
+-rw-r--r--   0        0        0      697 2023-02-13 01:29:30.557285 msm_has_base-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-07 09:19:20.201822 msm_has_base-0.1.9/README.md
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 msm_has_base-0.1.9/setup.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 msm_has_base-0.1.9/PKG-INFO
```

### Comparing `msm_has_base-0.1.8/msm_has_base/apdu.py` & `msm_has_base-0.1.9/msm_has_base/apdu.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/msm_has_base/bc_reader.py` & `msm_has_base-0.1.9/msm_has_base/bc_reader.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/msm_has_base/card_reader.py` & `msm_has_base-0.1.9/msm_has_base/card_reader.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/msm_has_base/epp.py` & `msm_has_base-0.1.9/msm_has_base/epp.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/msm_has_base/pboc.py` & `msm_has_base-0.1.9/msm_has_base/pboc.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/msm_has_base/pos.py` & `msm_has_base-0.1.9/msm_has_base/pos.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .epp import EPP
 
 __TOKEN__ = '696939654e404e293635284634453324596a427a574938624e7056532b2c36'
 
 
 class POSAPI(object):
 
-    def __init__(self, url: str, token: str = None, pwd: str = None):
+    def __init__(self, url: str, token: str = '', pwd: str = ''):
         super(POSAPI, self).__init__()
         self.url = url
         self.token = token
         self.pwd = pwd
 
     @property
     def certificate(self):
```

### Comparing `msm_has_base-0.1.8/msm_has_base/pos_ccb.py` & `msm_has_base-0.1.9/msm_has_base/pos_ccb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,30 @@
                 raise RuntimeError('Failed to write PIN key')
 
             r = self.epp.write_mac_key(resp['mkey'])
             logger.debug('write_mac_key {}, {}', r, resp['msum'])
             if r.lower() != resp['msum']:
                 raise RuntimeError('Failed to write MAC key')
 
+        logger.info('Sign in success.')
         return resp['batch']
 
     def sign_out(self) -> None:
         self.api.exec({
             "tranCode": "0820",
             "device": self.device
         })
+        logger.info('Sign out success.')
 
     def pay(self, amount: int) -> dict:
         if amount < 1:
             raise RuntimeError('The amount must be greater than zero')
 
         bci = self.bcr.read_info(amount, '00')
-        logger.debug("bci: {}", bci)
+        logger.info("bci: {}", bci)
 
         if not bci:
             raise RuntimeError('Failed to read card information')
 
         pin = None
         with self.epp:
             pin = self.epp.read_pin(bci.pin_pan)
@@ -83,15 +85,15 @@
         return result
 
     def write_off(self, amount: int, order_no: str, batch: str, auth_code: str) -> dict:
         if amount < 1:
             raise RuntimeError('The amount must be greater than zero')
 
         bci = self.bcr.read_info(amount, '00')
-        logger.debug("bci: {}", bci)
+        logger.info("bci: {}", bci)
 
         if not bci:
             raise RuntimeError('Failed to read card information')
 
         resp = self.api.exec({
             "tranCode": "04001",
             "device": self.device,
```

### Comparing `msm_has_base-0.1.8/msm_has_base/tlv.py` & `msm_has_base-0.1.9/msm_has_base/tlv.py`

 * *Files identical despite different names*

### Comparing `msm_has_base-0.1.8/pyproject.toml` & `msm_has_base-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+[tool.pyright]
+exclude = [".venv"]
+venvPath = '.'
+venv = '.venv'
+
 [tool.poetry]
 name = "msm-has-base"
-version = "0.1.8"
+version = "0.1.9"
 description = "Hardware Access Services Base Foundation"
 authors = ["袁首京 <yuanshoujing@gmail.com>"]
 readme = "README.md"
 packages = [{include = "msm_has_base"}]
 
 [tool.poetry.dependencies]
 python = "^3.7.9"
```

### Comparing `msm_has_base-0.1.8/setup.py` & `msm_has_base-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['loguru>=0.6.0,<0.7.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'msm-has-base',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Hardware Access Services Base Foundation',
     'long_description': '',
     'author': '袁首京',
     'author_email': 'yuanshoujing@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `msm_has_base-0.1.8/PKG-INFO` & `msm_has_base-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msm-has-base
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hardware Access Services Base Foundation
 Author: 袁首京
 Author-email: yuanshoujing@gmail.com
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

