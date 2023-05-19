# Comparing `tmp/neulabs-cdk-constructs-0.3.6.tar.gz` & `tmp/neulabs-cdk-constructs-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.3.6.tar", last modified: Tue May 16 16:38:36 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.3.7.tar", last modified: Fri May 19 10:39:16 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.3.6.tar` & `neulabs-cdk-constructs-0.3.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.914210 neulabs-cdk-constructs-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   327267 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.6.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-16 16:38:25.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:38:36.918210 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-16 16:38:36.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-16 16:38:36.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:38:36.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-16 16:38:36.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 16:38:36.000000 neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.613455 neulabs-cdk-constructs-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100739 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.7.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 10:39:04.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:39:16.617455 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-19 10:39:16.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-19 10:39:16.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:39:16.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 10:39:16.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 10:39:16.000000 neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.3.6/LICENSE` & `neulabs-cdk-constructs-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/PKG-INFO` & `neulabs-cdk-constructs-0.3.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 756c  : 2.1.Name: neul
 00000020: 6162 732d 6364 6b2d 636f 6e73 7472 7563  abs-cdk-construc
 00000030: 7473 0a56 6572 7369 6f6e 3a20 302e 332e  ts.Version: 0.3.
-00000040: 360a 5375 6d6d 6172 793a 206e 6575 6c61  6.Summary: neula
+00000040: 370a 5375 6d6d 6172 793a 206e 6575 6c61  7.Summary: neula
 00000050: 6273 2d63 646b 2d63 6f6e 7374 7275 6374  bs-cdk-construct
 00000060: 730a 486f 6d65 2d70 6167 653a 2068 7474  s.Home-page: htt
 00000070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000080: 6e65 756c 6162 7363 6f6d 2f6e 6575 6c61  neulabscom/neula
 00000090: 6273 2d63 646b 2d63 6f6e 7374 7275 6374  bs-cdk-construct
 000000a0: 732e 6769 740a 4175 7468 6f72 3a20 4e65  s.git.Author: Ne
 000000b0: 756c 6162 733c 7465 6368 406e 6575 6c61  ulabs<tech@neula
@@ -144,90 +144,144 @@
 000008f0: 6c20 6e65 756c 6162 732d 6364 6b2d 636f  l neulabs-cdk-co
 00000900: 6e73 7472 7563 7473 0a60 6060 0a0a 2a2a  nstructs.```..**
 00000910: 5061 636b 6167 6520 496e 7374 616c 6c61  Package Installa
 00000920: 7469 6f6e 2028 7079 7468 6f6e 292a 2a3a  tion (python)**:
 00000930: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
 00000940: 6c20 6e65 756c 6162 732d 6364 6b2d 636f  l neulabs-cdk-co
 00000950: 6e73 7472 7563 7473 0a60 6060 0a0a 2a2a  nstructs.```..**
-00000960: 4578 616d 706c 6573 2a2a 0a0a 5374 6163  Examples**..Stac
-00000970: 6b20 666f 7220 696e 7465 6772 6174 696f  k for integratio
-00000980: 6e20 6265 7477 6565 6e20 4157 5320 616e  n between AWS an
-00000990: 6420 4e65 7720 5265 6c69 632e 0a0a 4669  d New Relic...Fi
-000009a0: 6c65 2060 6170 702e 7079 600a 0a60 6060  le `app.py`..```
-000009b0: 0a69 6d70 6f72 7420 6177 735f 6364 6b20  .import aws_cdk 
-000009c0: 6173 2063 646b 0a0a 6672 6f6d 206e 6575  as cdk..from neu
-000009d0: 6c61 6273 5f63 646b 5f63 6f6e 7374 7275  labs_cdk_constru
-000009e0: 6374 732e 7374 6163 6b73 2e6d 6f6e 6974  cts.stacks.monit
-000009f0: 6f72 696e 672e 6e65 7772 656c 6963 2069  oring.newrelic i
-00000a00: 6d70 6f72 7420 456e 6470 6f69 6e74 5572  mport EndpointUr
-00000a10: 6c4c 6f67 730a 6672 6f6d 206e 6575 6c61  lLogs.from neula
-00000a20: 6273 5f63 646b 5f63 6f6e 7374 7275 6374  bs_cdk_construct
-00000a30: 732e 7374 6163 6b73 2e6d 6f6e 6974 6f72  s.stacks.monitor
-00000a40: 696e 672e 6e65 7772 656c 6963 2069 6d70  ing.newrelic imp
-00000a50: 6f72 7420 456e 6470 6f69 6e74 5572 6c4d  ort EndpointUrlM
-00000a60: 6574 7269 6373 0a66 726f 6d20 6e65 756c  etrics.from neul
-00000a70: 6162 735f 6364 6b5f 636f 6e73 7472 7563  abs_cdk_construc
-00000a80: 7473 2e73 7461 636b 732e 6d6f 6e69 746f  ts.stacks.monito
-00000a90: 7269 6e67 2e6e 6577 7265 6c69 6320 696d  ring.newrelic im
-00000aa0: 706f 7274 204e 6577 5265 6c69 6353 7461  port NewRelicSta
-00000ab0: 636b 0a0a 6170 7020 3d20 6364 6b2e 4170  ck..app = cdk.Ap
-00000ac0: 7028 290a 0a65 6e76 6972 6f6e 6d65 6e74  p()..environment
-00000ad0: 203d 2063 646b 2e45 6e76 6972 6f6e 6d65   = cdk.Environme
-00000ae0: 6e74 280a 2020 2020 6163 636f 756e 743d  nt(.    account=
-00000af0: 6f73 2e67 6574 656e 7628 2743 444b 5f44  os.getenv('CDK_D
-00000b00: 4546 4155 4c54 5f41 4343 4f55 4e54 2729  EFAULT_ACCOUNT')
-00000b10: 2c0a 2020 2020 7265 6769 6f6e 3d6f 732e  ,.    region=os.
-00000b20: 6765 7465 6e76 2827 4344 4b5f 4445 4641  getenv('CDK_DEFA
-00000b30: 554c 545f 5245 4749 4f4e 2729 2c0a 290a  ULT_REGION'),.).
-00000b40: 0a73 7461 6765 203d 206f 732e 6765 7465  .stage = os.gete
-00000b50: 6e76 2827 454e 5649 524f 4e4d 454e 5427  nv('ENVIRONMENT'
-00000b60: 2c20 2764 6576 656c 6f70 2729 0a6e 6577  , 'develop').new
-00000b70: 5f72 656c 6963 5f61 6363 6f75 6e74 5f69  _relic_account_i
-00000b80: 6420 3d20 6f73 2e67 6574 656e 7628 274e  d = os.getenv('N
-00000b90: 4557 5f52 454c 4943 5f41 4343 4f55 4e54  EW_RELIC_ACCOUNT
-00000ba0: 5f49 4427 290a 6e65 775f 7265 6c69 635f  _ID').new_relic_
-00000bb0: 6c69 6365 6e73 655f 6b65 7920 3d20 6f73  license_key = os
-00000bc0: 2e67 6574 656e 7628 274e 4557 5f52 454c  .getenv('NEW_REL
-00000bd0: 4943 5f4c 4943 454e 5345 5f4b 4559 2729  IC_LICENSE_KEY')
-00000be0: 0a0a 6e65 775f 7265 6c69 635f 7374 6163  ..new_relic_stac
-00000bf0: 6b20 3d20 4e65 7752 656c 6963 5374 6163  k = NewRelicStac
-00000c00: 6b28 0a20 2020 2061 7070 2c0a 2020 2020  k(.    app,.    
-00000c10: 274e 6577 5265 6c69 6353 7461 636b 272c  'NewRelicStack',
-00000c20: 0a20 2020 2065 6e76 3d65 6e76 6972 6f6e  .    env=environ
-00000c30: 6d65 6e74 2c0a 2020 2020 7374 6167 653d  ment,.    stage=
-00000c40: 7374 6167 652c 0a20 2020 206e 6577 5f72  stage,.    new_r
-00000c50: 656c 6963 5f62 7563 6b65 745f 6e61 6d65  elic_bucket_name
-00000c60: 3d66 276e 6575 6c61 6273 2d6e 6577 7265  =f'neulabs-newre
-00000c70: 6c69 632d 7b73 7461 6765 7d27 2c0a 2020  lic-{stage}',.  
-00000c80: 2020 6e65 775f 7265 6c69 635f 6163 636f    new_relic_acco
-00000c90: 756e 745f 6964 3d6e 6577 5f72 656c 6963  unt_id=new_relic
-00000ca0: 5f61 6363 6f75 6e74 5f69 642c 0a20 2020  _account_id,.   
-00000cb0: 206e 6577 5f72 656c 6963 5f6c 6963 656e   new_relic_licen
-00000cc0: 7365 5f6b 6579 3d6e 6577 5f72 656c 6963  se_key=new_relic
-00000cd0: 5f6c 6963 656e 7365 5f6b 6579 2c0a 2020  _license_key,.  
-00000ce0: 2020 6e65 775f 7265 6c69 635f 6170 695f    new_relic_api_
-00000cf0: 7572 6c5f 6d65 7472 6963 733d 456e 6470  url_metrics=Endp
-00000d00: 6f69 6e74 5572 6c4d 6574 7269 6373 2e45  ointUrlMetrics.E
-00000d10: 555f 4d45 5452 4943 532c 0a20 2020 206e  U_METRICS,.    n
-00000d20: 6577 5f72 656c 6963 5f61 7069 5f75 726c  ew_relic_api_url
-00000d30: 5f6c 6f67 733d 456e 6470 6f69 6e74 5572  _logs=EndpointUr
-00000d40: 6c4c 6f67 732e 4555 5f4c 4f47 532c 0a29  lLogs.EU_LOGS,.)
-00000d50: 0a60 6060 0a0a 2323 2320 4465 7620 6d6f  .```..### Dev mo
-00000d60: 6465 0a0a 5275 6e20 696e 2073 6865 6c6c  de..Run in shell
-00000d70: 0a0a 6060 600a 6e70 7820 7072 6f6a 656e  ..```.npx projen
-00000d80: 2064 6566 6175 6c74 0a60 6060 0a0a 2323   default.```..##
-00000d90: 2320 436f 6e74 7269 6275 746f 7273 0a0a  # Contributors..
-00000da0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000db0: 2f67 6974 6875 622e 636f 6d2f 6e65 756c  /github.com/neul
-00000dc0: 6162 7363 6f6d 2f6e 6575 6c61 6273 2d63  abscom/neulabs-c
-00000dd0: 646b 2d63 6f6e 7374 7275 6374 732f 6772  dk-constructs/gr
-00000de0: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
-00000df0: 7322 3e20 3c69 6d67 2073 7263 3d22 6874  s"> <img src="ht
-00000e00: 7470 733a 2f2f 636f 6e74 7269 622e 726f  tps://contrib.ro
-00000e10: 636b 732f 696d 6167 653f 7265 706f 3d6e  cks/image?repo=n
-00000e20: 6575 6c61 6273 636f 6d2f 6e65 756c 6162  eulabscom/neulab
-00000e30: 732d 6364 6b2d 636f 6e73 7472 7563 7473  s-cdk-constructs
-00000e40: 2220 2f3e 203c 2f61 3e0a 0a23 2323 204c  " /> </a>..### L
-00000e50: 6963 656e 7365 0a0a 5365 6520 7468 6520  icense..See the 
-00000e60: 604c 4943 454e 5345 6020 6669 6c65 2066  `LICENSE` file f
-00000e70: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00000e80: 696f 6e2e 0a                             ion..
+00000960: 4372 6561 7465 2047 6974 6875 6220 4f49  Create Github OI
+00000970: 4443 2a2a 0a0a 5468 6520 6372 6561 7469  DC**..The creati
+00000980: 6f6e 206f 6620 4769 7468 7562 204f 4944  on of Github OID
+00000990: 4320 616c 6c6f 7773 2061 2072 6f6c 6520  C allows a role 
+000009a0: 7769 7468 696e 2077 6f72 6b66 6c6f 7773  within workflows
+000009b0: 2074 6f20 6265 2075 7365 6420 746f 206c   to be used to l
+000009c0: 6f67 2069 6e20 746f 2061 7773 2e0a 496e  og in to aws..In
+000009d0: 2074 6869 7320 7374 6163 6b2c 2074 6865   this stack, the
+000009e0: 3a0a 0a2a 2067 6974 6875 622d 6f69 6463  :..* github-oidc
+000009f0: 2d77 6f72 6b66 6c6f 772d 726f 6c65 2075  -workflow-role u
+00000a00: 7365 7220 7573 6564 2066 6f72 2061 7574  ser used for aut
+00000a10: 6865 6e74 6963 6174 696f 6e0a 2a20 6364  hentication.* cd
+00000a20: 6b2d 6f69 6463 2d64 6570 6c6f 792d 726f  k-oidc-deploy-ro
+00000a30: 6c65 2072 6f6c 6520 7573 6564 2066 6f72  le role used for
+00000a40: 2064 6570 6c6f 7969 6e67 0a2a 2063 646b   deploying.* cdk
+00000a50: 2d6f 6964 632d 626f 6f74 7372 6170 2d72  -oidc-bootsrap-r
+00000a60: 6f6c 6520 726f 6c65 2075 7365 6420 666f  ole role used fo
+00000a70: 7220 626f 6f74 7374 7261 700a 0a60 6060  r bootstrap..```
+00000a80: 0a65 6e76 6972 6f6e 6d65 6e74 203d 2070  .environment = p
+00000a90: 726f 6365 7373 2e65 6e76 2e45 4e56 4952  rocess.env.ENVIR
+00000aa0: 4f4e 4d45 4e54 2120 7c7c 2027 7374 6167  ONMENT! || 'stag
+00000ab0: 696e 6727 3b0a 0a6e 6577 2047 6974 6875  ing';..new Githu
+00000ac0: 624f 4944 4353 7461 636b 2861 7070 2c20  bOIDCStack(app, 
+00000ad0: 274f 6964 6353 7461 636b 272c 207b 0a20  'OidcStack', {. 
+00000ae0: 2065 6e76 3a20 7b0a 2020 2020 6163 636f   env: {.    acco
+00000af0: 756e 743a 2070 726f 6365 7373 2e65 6e76  unt: process.env
+00000b00: 2e43 444b 5f44 4546 4155 4c54 5f41 4343  .CDK_DEFAULT_ACC
+00000b10: 4f55 4e54 2c0a 2020 2020 7265 6769 6f6e  OUNT,.    region
+00000b20: 3a20 7072 6f63 6573 732e 656e 762e 4344  : process.env.CD
+00000b30: 4b5f 4445 4641 554c 545f 5245 4749 4f4e  K_DEFAULT_REGION
+00000b40: 2c0a 2020 7d2c 0a20 2073 7461 6765 3a20  ,.  },.  stage: 
+00000b50: 656e 7669 726f 6e6d 656e 742c 0a20 2067  environment,.  g
+00000b60: 6974 6875 6255 7365 723a 2027 7573 6572  ithubUser: 'user
+00000b70: 6e61 6d65 272c 0a20 2067 6974 6875 6252  name',.  githubR
+00000b80: 6570 6f73 6974 6f72 793a 2027 7265 706f  epository: 'repo
+00000b90: 7369 746f 7279 4e61 6d65 272c 2023 2059  sitoryName', # Y
+00000ba0: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00000bb0: 272a 270a 2020 746f 6b65 6e41 6374 696f  '*'.  tokenActio
+00000bc0: 6e3a 2054 6f6b 656e 4163 7469 6f6e 732e  n: TokenActions.
+00000bd0: 414c 4c2c 0a20 2063 646b 4465 706c 6f79  ALL,.  cdkDeploy
+00000be0: 526f 6c65 4d61 6e61 6765 6450 6f6c 6963  RoleManagedPolic
+00000bf0: 6965 733a 205b 2741 646d 696e 6973 7472  ies: ['Administr
+00000c00: 6174 6f72 4163 6365 7373 275d 2c0a 7d29  atorAccess'],.})
+00000c10: 3b0a 6060 600a 0a47 6974 6875 6220 776f  ;.```..Github wo
+00000c20: 726b 666c 6f77 0a0a 6060 600a 2e2e 2e0a  rkflow..```.....
+00000c30: 0a23 2070 6572 6d69 7373 696f 6e20 6361  .# permission ca
+00000c40: 6e20 6265 2061 6464 6564 2061 7420 6a6f  n be added at jo
+00000c50: 6220 6c65 7665 6c20 6f72 2077 6f72 6b66  b level or workf
+00000c60: 6c6f 7720 6c65 7665 6c0a 7065 726d 6973  low level.permis
+00000c70: 7369 6f6e 733a 0a20 2069 642d 746f 6b65  sions:.  id-toke
+00000c80: 6e3a 2077 7269 7465 0a20 2063 6f6e 7465  n: write.  conte
+00000c90: 6e74 733a 2072 6561 6420 2020 2023 2054  nts: read    # T
+00000ca0: 6869 7320 6973 2072 6571 7569 7265 6420  his is required 
+00000cb0: 666f 7220 6163 7469 6f6e 732f 6368 6563  for actions/chec
+00000cc0: 6b6f 7574 0a0a 6a6f 6273 3a0a 2020 2e2e  kout..jobs:.  ..
+00000cd0: 2e0a 0a20 206f 6964 633a 0a20 2020 206e  ...  oidc:.    n
+00000ce0: 616d 653a 2041 7574 680a 2020 2020 7275  ame: Auth.    ru
+00000cf0: 6e73 2d6f 6e3a 2075 6275 6e74 752d 3230  ns-on: ubuntu-20
+00000d00: 2e30 340a 2020 2020 7374 6570 733a 0a20  .04.    steps:. 
+00000d10: 2020 2020 202d 206e 616d 653a 2043 6f6e       - name: Con
+00000d20: 6669 6775 7265 2061 7773 2063 7265 6465  figure aws crede
+00000d30: 6e74 6961 6c73 0a20 2020 2020 2020 2075  ntials.        u
+00000d40: 7365 733a 2061 7773 2d61 6374 696f 6e73  ses: aws-actions
+00000d50: 2f63 6f6e 6669 6775 7265 2d61 7773 2d63  /configure-aws-c
+00000d60: 7265 6465 6e74 6961 6c73 4076 310a 2020  redentials@v1.  
+00000d70: 2020 2020 2020 7769 7468 3a0a 2020 2020        with:.    
+00000d80: 2020 2020 2020 726f 6c65 2d74 6f2d 6173        role-to-as
+00000d90: 7375 6d65 3a20 6172 6e3a 6177 733a 6961  sume: arn:aws:ia
+00000da0: 6d3a 3a7b 4143 434f 554e 5420 4944 7d3a  m::{ACCOUNT ID}:
+00000db0: 726f 6c65 2f67 6974 6875 622d 6f69 6463  role/github-oidc
+00000dc0: 2d77 6f72 6b66 6c6f 772d 726f 6c65 0a20  -workflow-role. 
+00000dd0: 2020 2020 2020 2020 2061 7773 2d72 6567           aws-reg
+00000de0: 696f 6e3a 207b 5245 4749 4f4e 7d0a 2020  ion: {REGION}.  
+00000df0: 2020 2020 2020 2020 6d61 736b 2d61 7773          mask-aws
+00000e00: 2d61 6363 6f75 6e74 2d69 643a 206e 6f0a  -account-id: no.
+00000e10: 0a20 202e 2e2e 0a60 6060 0a0a 2a2a 4372  .  ....```..**Cr
+00000e20: 6561 7465 204e 6577 5265 6c69 6320 436f  eate NewRelic Co
+00000e30: 6e6e 6563 7469 6f6e 2a2a 0a0a 5468 6520  nnection**..The 
+00000e40: 4e65 7752 656c 6963 5374 6163 6b20 696d  NewRelicStack im
+00000e50: 706c 656d 656e 7473 2074 6865 2069 6e66  plements the inf
+00000e60: 7261 7374 7275 6374 7572 6520 746f 2073  rastructure to s
+00000e70: 656e 6420 6d65 7472 6963 7320 616e 6420  end metrics and 
+00000e80: 6c6f 6773 2074 6f20 4e65 7772 656c 6963  logs to Newrelic
+00000e90: 2074 6872 6f75 6768 204b 696e 6573 6973   through Kinesis
+00000ea0: 2061 6e64 2043 6c6f 7564 7761 7463 6820   and Cloudwatch 
+00000eb0: 5374 7265 616d 2e0a 4f6e 6365 2064 6570  Stream..Once dep
+00000ec0: 6c6f 7965 6420 796f 7520 6361 6e20 636f  loyed you can co
+00000ed0: 7079 2074 6865 2041 524e 206f 6620 7468  py the ARN of th
+00000ee0: 6520 274e 6577 5265 6c69 6349 6e66 7261  e 'NewRelicInfra
+00000ef0: 7374 7275 6374 7572 652d 496e 7465 6772  structure-Integr
+00000f00: 6174 696f 6e73 2720 726f 6c65 2061 6e64  ations' role and
+00000f10: 2075 7365 2069 7420 746f 2063 6f6e 6669   use it to confi
+00000f20: 6775 7265 204e 6577 7265 6c69 632e 0a0a  gure Newrelic...
+00000f30: 6060 600a 2020 6e65 7720 4e65 7752 656c  ```.  new NewRel
+00000f40: 6963 5374 6163 6b28 6170 702c 2027 4e65  icStack(app, 'Ne
+00000f50: 7772 656c 6963 5374 6163 6b27 2c20 7b0a  wrelicStack', {.
+00000f60: 2020 2020 656e 763a 2063 6f6e 7374 616e      env: constan
+00000f70: 7473 2e65 6e76 2c0a 2020 2020 7374 6167  ts.env,.    stag
+00000f80: 653a 2063 6f6e 7374 616e 7473 2e65 6e76  e: constants.env
+00000f90: 6972 6f6e 6d65 6e74 2c0a 2020 2020 6e65  ironment,.    ne
+00000fa0: 7752 656c 6963 4275 636b 6574 4e61 6d65  wRelicBucketName
+00000fb0: 3a20 606e 6577 7265 6c69 632d 247b 636f  : `newrelic-${co
+00000fc0: 6e73 7461 6e74 732e 6177 7341 6363 6f75  nstants.awsAccou
+00000fd0: 6e74 4964 7d2d 247b 636f 6e73 7461 6e74  ntId}-${constant
+00000fe0: 732e 656e 7669 726f 6e6d 656e 747d 602c  s.environment}`,
+00000ff0: 0a20 2020 206e 6577 5265 6c69 6341 6363  .    newRelicAcc
+00001000: 6f75 6e74 4964 3a20 6e65 7752 656c 6963  ountId: newRelic
+00001010: 4163 636f 756e 7449 642c 0a20 2020 206e  AccountId,.    n
+00001020: 6577 5265 6c69 634c 6963 656e 7365 4b65  ewRelicLicenseKe
+00001030: 793a 206e 6577 5265 6c69 634c 6963 656e  y: newRelicLicen
+00001040: 7365 4b65 792c 0a20 2020 206e 6577 5265  seKey,.    newRe
+00001050: 6c69 6341 7069 5572 6c4d 6574 7269 6373  licApiUrlMetrics
+00001060: 3a20 456e 6470 6f69 6e74 5572 6c4d 6574  : EndpointUrlMet
+00001070: 7269 6373 2e45 555f 4d45 5452 4943 532c  rics.EU_METRICS,
+00001080: 0a20 2020 206e 6577 5265 6c69 6341 7069  .    newRelicApi
+00001090: 5572 6c4c 6f67 733a 2045 6e64 706f 696e  UrlLogs: Endpoin
+000010a0: 7455 726c 4c6f 6773 2e45 555f 4c4f 4753  tUrlLogs.EU_LOGS
+000010b0: 2c0a 2020 7d29 3b0a 6060 600a 0a23 2323  ,.  });.```..###
+000010c0: 2044 6576 206d 6f64 650a 0a52 756e 2069   Dev mode..Run i
+000010d0: 6e20 7368 656c 6c0a 0a60 6060 0a6e 7078  n shell..```.npx
+000010e0: 2070 726f 6a65 6e20 6465 6661 756c 740a   projen default.
+000010f0: 6060 600a 0a23 2323 2043 6f6e 7472 6962  ```..### Contrib
+00001100: 7574 6f72 730a 0a3c 6120 6872 6566 3d22  utors..<a href="
+00001110: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001120: 6f6d 2f6e 6575 6c61 6273 636f 6d2f 6e65  om/neulabscom/ne
+00001130: 756c 6162 732d 6364 6b2d 636f 6e73 7472  ulabs-cdk-constr
+00001140: 7563 7473 2f67 7261 7068 732f 636f 6e74  ucts/graphs/cont
+00001150: 7269 6275 746f 7273 223e 203c 696d 6720  ributors"> <img 
+00001160: 7372 633d 2268 7474 7073 3a2f 2f63 6f6e  src="https://con
+00001170: 7472 6962 2e72 6f63 6b73 2f69 6d61 6765  trib.rocks/image
+00001180: 3f72 6570 6f3d 6e65 756c 6162 7363 6f6d  ?repo=neulabscom
+00001190: 2f6e 6575 6c61 6273 2d63 646b 2d63 6f6e  /neulabs-cdk-con
+000011a0: 7374 7275 6374 7322 202f 3e20 3c2f 613e  structs" /> </a>
+000011b0: 0a0a 2323 2320 4c69 6365 6e73 650a 0a53  ..### License..S
+000011c0: 6565 2074 6865 2060 4c49 4345 4e53 4560  ee the `LICENSE`
+000011d0: 2066 696c 6520 666f 7220 6d6f 7265 2069   file for more i
+000011e0: 6e66 6f72 6d61 7469 6f6e 2e0a            nformation..
```

### Comparing `neulabs-cdk-constructs-0.3.6/setup.py` & `neulabs-cdk-constructs-0.3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.3.6",
+    "version": "0.3.7",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.3.6.jsii.tgz"
+            "neulabs-cdk-constructs@0.3.7.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.3.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-'''
 # Neulabs CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/neulabs-cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-cdk-constructs)
 [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-constructs/)
 [![PyPI](https://img.shields.io/github/last-commit/neulabscom/neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-constructs/commits/main)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/main/LICENSE)
 
@@ -26,49 +25,81 @@
 
 **Package Installation (python)**:
 
 ```
 pip install neulabs-cdk-constructs
 ```
 
-**Examples**
+**Create Github OIDC**
 
-Stack for integration between AWS and New Relic.
+The creation of Github OIDC allows a role within workflows to be used to log in to aws.
+In this stack, the:
 
-File `app.py`
+* github-oidc-workflow-role user used for authentication
+* cdk-oidc-deploy-role role used for deploying
+* cdk-oidc-bootsrap-role role used for bootstrap
 
 ```
-import aws_cdk as cdk
+environment = process.env.ENVIRONMENT! || 'staging';
 
-from neulabs_cdk_constructs.stacks.monitoring.newrelic import EndpointUrlLogs
-from neulabs_cdk_constructs.stacks.monitoring.newrelic import EndpointUrlMetrics
-from neulabs_cdk_constructs.stacks.monitoring.newrelic import NewRelicStack
+new GithubOIDCStack(app, 'OidcStack', {
+  env: {
+    account: process.env.CDK_DEFAULT_ACCOUNT,
+    region: process.env.CDK_DEFAULT_REGION,
+  },
+  stage: environment,
+  githubUser: 'username',
+  githubRepository: 'repositoryName', # You can also use '*'
+  tokenAction: TokenActions.ALL,
+  cdkDeployRoleManagedPolicies: ['AdministratorAccess'],
+});
+```
+
+Github workflow
 
-app = cdk.App()
+```
+...
 
-environment = cdk.Environment(
-    account=os.getenv('CDK_DEFAULT_ACCOUNT'),
-    region=os.getenv('CDK_DEFAULT_REGION'),
-)
+# permission can be added at job level or workflow level
+permissions:
+  id-token: write
+  contents: read    # This is required for actions/checkout
 
-stage = os.getenv('ENVIRONMENT', 'develop')
-new_relic_account_id = os.getenv('NEW_RELIC_ACCOUNT_ID')
-new_relic_license_key = os.getenv('NEW_RELIC_LICENSE_KEY')
+jobs:
+  ...
 
-new_relic_stack = NewRelicStack(
-    app,
-    'NewRelicStack',
-    env=environment,
-    stage=stage,
-    new_relic_bucket_name=f'neulabs-newrelic-{stage}',
-    new_relic_account_id=new_relic_account_id,
-    new_relic_license_key=new_relic_license_key,
-    new_relic_api_url_metrics=EndpointUrlMetrics.EU_METRICS,
-    new_relic_api_url_logs=EndpointUrlLogs.EU_LOGS,
-)
+  oidc:
+    name: Auth
+    runs-on: ubuntu-20.04
+    steps:
+      - name: Configure aws credentials
+        uses: aws-actions/configure-aws-credentials@v1
+        with:
+          role-to-assume: arn:aws:iam::{ACCOUNT ID}:role/github-oidc-workflow-role
+          aws-region: {REGION}
+          mask-aws-account-id: no
+
+  ...
+```
+
+**Create NewRelic Connection**
+
+The NewRelicStack implements the infrastructure to send metrics and logs to Newrelic through Kinesis and Cloudwatch Stream.
+Once deployed you can copy the ARN of the 'NewRelicInfrastructure-Integrations' role and use it to configure Newrelic.
+
+```
+  new NewRelicStack(app, 'NewrelicStack', {
+    env: constants.env,
+    stage: constants.environment,
+    newRelicBucketName: `newrelic-${constants.awsAccountId}-${constants.environment}`,
+    newRelicAccountId: newRelicAccountId,
+    newRelicLicenseKey: newRelicLicenseKey,
+    newRelicApiUrlMetrics: EndpointUrlMetrics.EU_METRICS,
+    newRelicApiUrlLogs: EndpointUrlLogs.EU_LOGS,
+  });
 ```
 
 ### Dev mode
 
 Run in shell
 
 ```
@@ -78,38 +109,7 @@
 ### Contributors
 
 <a href="https://github.com/neulabscom/neulabs-cdk-constructs/graphs/contributors"> <img src="https://contrib.rocks/image?repo=neulabscom/neulabs-cdk-constructs" /> </a>
 
 ### License
 
 See the `LICENSE` file for more information.
-'''
-import abc
-import builtins
-import datetime
-import enum
-import typing
-
-import jsii
-import publication
-import typing_extensions
-
-from typeguard import check_type
-
-from ._jsii import *
-
-__all__ = [
-    "aws_lambda",
-    "newrelic",
-    "oidc",
-    "stack",
-    "utils",
-]
-
-publication.publish()
-
-# Loading modules to ensure their types are registered with the jsii runtime library
-from . import aws_lambda
-from . import newrelic
-from . import oidc
-from . import stack
-from . import utils
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-''' # Neulabs CDK Constructs [![NPM](https://img.shields.io/npm/v/neulabs-cdk-
+# Neulabs CDK Constructs [![NPM](https://img.shields.io/npm/v/neulabs-cdk-
 constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-
 cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
 constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-
 constructs/) [![PyPI](https://img.shields.io/github/last-commit/neulabscom/
 neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-
 constructs/commits/main) [![License](https://img.shields.io/badge/license-
 Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/
@@ -13,31 +13,34 @@
 that allow the creation of services by simply instantiating a class, or
 constructs that implement logic to facilitate the developer and many other
 aspects. We decided to develop it in Typescript, using projen for repository
 management, and the JSII library to be able to compile the neulabs-cdk-
 constructs package into multiple languages. ## Usage **Package Installation
 (npm)**: ``` yarn add neulabs-cdk-constructs # or npm install neulabs-cdk-
 constructs ``` **Package Installation (python)**: ``` pip install neulabs-cdk-
-constructs ``` **Examples** Stack for integration between AWS and New Relic.
-File `app.py` ``` import aws_cdk as cdk from
-neulabs_cdk_constructs.stacks.monitoring.newrelic import EndpointUrlLogs from
-neulabs_cdk_constructs.stacks.monitoring.newrelic import EndpointUrlMetrics
-from neulabs_cdk_constructs.stacks.monitoring.newrelic import NewRelicStack app
-= cdk.App() environment = cdk.Environment( account=os.getenv
-('CDK_DEFAULT_ACCOUNT'), region=os.getenv('CDK_DEFAULT_REGION'), ) stage =
-os.getenv('ENVIRONMENT', 'develop') new_relic_account_id = os.getenv
-('NEW_RELIC_ACCOUNT_ID') new_relic_license_key = os.getenv
-('NEW_RELIC_LICENSE_KEY') new_relic_stack = NewRelicStack( app,
-'NewRelicStack', env=environment, stage=stage, new_relic_bucket_name=f'neulabs-
-newrelic-{stage}', new_relic_account_id=new_relic_account_id,
-new_relic_license_key=new_relic_license_key,
-new_relic_api_url_metrics=EndpointUrlMetrics.EU_METRICS,
-new_relic_api_url_logs=EndpointUrlLogs.EU_LOGS, ) ``` ### Dev mode Run in shell
-``` npx projen default ``` ### Contributors [https://contrib.rocks/
-image?repo=neulabscom/neulabs-cdk-constructs] ### License See the `LICENSE`
-file for more information. ''' import abc import builtins import datetime
-import enum import typing import jsii import publication import
-typing_extensions from typeguard import check_type from ._jsii import * __all__
-= [ "aws_lambda", "newrelic", "oidc", "stack", "utils", ] publication.publish()
-# Loading modules to ensure their types are registered with the jsii runtime
-library from . import aws_lambda from . import newrelic from . import oidc from
-. import stack from . import utils
+constructs ``` **Create Github OIDC** The creation of Github OIDC allows a role
+within workflows to be used to log in to aws. In this stack, the: * github-
+oidc-workflow-role user used for authentication * cdk-oidc-deploy-role role
+used for deploying * cdk-oidc-bootsrap-role role used for bootstrap ```
+environment = process.env.ENVIRONMENT! || 'staging'; new GithubOIDCStack(app,
+'OidcStack', { env: { account: process.env.CDK_DEFAULT_ACCOUNT, region:
+process.env.CDK_DEFAULT_REGION, }, stage: environment, githubUser: 'username',
+githubRepository: 'repositoryName', # You can also use '*' tokenAction:
+TokenActions.ALL, cdkDeployRoleManagedPolicies: ['AdministratorAccess'], });
+``` Github workflow ``` ... # permission can be added at job level or workflow
+level permissions: id-token: write contents: read # This is required for
+actions/checkout jobs: ... oidc: name: Auth runs-on: ubuntu-20.04 steps: -
+name: Configure aws credentials uses: aws-actions/configure-aws-credentials@v1
+with: role-to-assume: arn:aws:iam::{ACCOUNT ID}:role/github-oidc-workflow-role
+aws-region: {REGION} mask-aws-account-id: no ... ``` **Create NewRelic
+Connection** The NewRelicStack implements the infrastructure to send metrics
+and logs to Newrelic through Kinesis and Cloudwatch Stream. Once deployed you
+can copy the ARN of the 'NewRelicInfrastructure-Integrations' role and use it
+to configure Newrelic. ``` new NewRelicStack(app, 'NewrelicStack', { env:
+constants.env, stage: constants.environment, newRelicBucketName: `newrelic-$
+{constants.awsAccountId}-${constants.environment}`, newRelicAccountId:
+newRelicAccountId, newRelicLicenseKey: newRelicLicenseKey,
+newRelicApiUrlMetrics: EndpointUrlMetrics.EU_METRICS, newRelicApiUrlLogs:
+EndpointUrlLogs.EU_LOGS, }); ``` ### Dev mode Run in shell ``` npx projen
+default ``` ### Contributors [https://contrib.rocks/image?repo=neulabscom/
+neulabs-cdk-constructs] ### License See the `LICENSE` file for more
+information.
```

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.3.6",
+    "0.3.7",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.3.6.jsii.tgz",
+    "neulabs-cdk-constructs@0.3.7.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 756c  : 2.1.Name: neul
 00000020: 6162 732d 6364 6b2d 636f 6e73 7472 7563  abs-cdk-construc
 00000030: 7473 0a56 6572 7369 6f6e 3a20 302e 332e  ts.Version: 0.3.
-00000040: 360a 5375 6d6d 6172 793a 206e 6575 6c61  6.Summary: neula
+00000040: 370a 5375 6d6d 6172 793a 206e 6575 6c61  7.Summary: neula
 00000050: 6273 2d63 646b 2d63 6f6e 7374 7275 6374  bs-cdk-construct
 00000060: 730a 486f 6d65 2d70 6167 653a 2068 7474  s.Home-page: htt
 00000070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000080: 6e65 756c 6162 7363 6f6d 2f6e 6575 6c61  neulabscom/neula
 00000090: 6273 2d63 646b 2d63 6f6e 7374 7275 6374  bs-cdk-construct
 000000a0: 732e 6769 740a 4175 7468 6f72 3a20 4e65  s.git.Author: Ne
 000000b0: 756c 6162 733c 7465 6368 406e 6575 6c61  ulabs<tech@neula
@@ -144,90 +144,144 @@
 000008f0: 6c20 6e65 756c 6162 732d 6364 6b2d 636f  l neulabs-cdk-co
 00000900: 6e73 7472 7563 7473 0a60 6060 0a0a 2a2a  nstructs.```..**
 00000910: 5061 636b 6167 6520 496e 7374 616c 6c61  Package Installa
 00000920: 7469 6f6e 2028 7079 7468 6f6e 292a 2a3a  tion (python)**:
 00000930: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
 00000940: 6c20 6e65 756c 6162 732d 6364 6b2d 636f  l neulabs-cdk-co
 00000950: 6e73 7472 7563 7473 0a60 6060 0a0a 2a2a  nstructs.```..**
-00000960: 4578 616d 706c 6573 2a2a 0a0a 5374 6163  Examples**..Stac
-00000970: 6b20 666f 7220 696e 7465 6772 6174 696f  k for integratio
-00000980: 6e20 6265 7477 6565 6e20 4157 5320 616e  n between AWS an
-00000990: 6420 4e65 7720 5265 6c69 632e 0a0a 4669  d New Relic...Fi
-000009a0: 6c65 2060 6170 702e 7079 600a 0a60 6060  le `app.py`..```
-000009b0: 0a69 6d70 6f72 7420 6177 735f 6364 6b20  .import aws_cdk 
-000009c0: 6173 2063 646b 0a0a 6672 6f6d 206e 6575  as cdk..from neu
-000009d0: 6c61 6273 5f63 646b 5f63 6f6e 7374 7275  labs_cdk_constru
-000009e0: 6374 732e 7374 6163 6b73 2e6d 6f6e 6974  cts.stacks.monit
-000009f0: 6f72 696e 672e 6e65 7772 656c 6963 2069  oring.newrelic i
-00000a00: 6d70 6f72 7420 456e 6470 6f69 6e74 5572  mport EndpointUr
-00000a10: 6c4c 6f67 730a 6672 6f6d 206e 6575 6c61  lLogs.from neula
-00000a20: 6273 5f63 646b 5f63 6f6e 7374 7275 6374  bs_cdk_construct
-00000a30: 732e 7374 6163 6b73 2e6d 6f6e 6974 6f72  s.stacks.monitor
-00000a40: 696e 672e 6e65 7772 656c 6963 2069 6d70  ing.newrelic imp
-00000a50: 6f72 7420 456e 6470 6f69 6e74 5572 6c4d  ort EndpointUrlM
-00000a60: 6574 7269 6373 0a66 726f 6d20 6e65 756c  etrics.from neul
-00000a70: 6162 735f 6364 6b5f 636f 6e73 7472 7563  abs_cdk_construc
-00000a80: 7473 2e73 7461 636b 732e 6d6f 6e69 746f  ts.stacks.monito
-00000a90: 7269 6e67 2e6e 6577 7265 6c69 6320 696d  ring.newrelic im
-00000aa0: 706f 7274 204e 6577 5265 6c69 6353 7461  port NewRelicSta
-00000ab0: 636b 0a0a 6170 7020 3d20 6364 6b2e 4170  ck..app = cdk.Ap
-00000ac0: 7028 290a 0a65 6e76 6972 6f6e 6d65 6e74  p()..environment
-00000ad0: 203d 2063 646b 2e45 6e76 6972 6f6e 6d65   = cdk.Environme
-00000ae0: 6e74 280a 2020 2020 6163 636f 756e 743d  nt(.    account=
-00000af0: 6f73 2e67 6574 656e 7628 2743 444b 5f44  os.getenv('CDK_D
-00000b00: 4546 4155 4c54 5f41 4343 4f55 4e54 2729  EFAULT_ACCOUNT')
-00000b10: 2c0a 2020 2020 7265 6769 6f6e 3d6f 732e  ,.    region=os.
-00000b20: 6765 7465 6e76 2827 4344 4b5f 4445 4641  getenv('CDK_DEFA
-00000b30: 554c 545f 5245 4749 4f4e 2729 2c0a 290a  ULT_REGION'),.).
-00000b40: 0a73 7461 6765 203d 206f 732e 6765 7465  .stage = os.gete
-00000b50: 6e76 2827 454e 5649 524f 4e4d 454e 5427  nv('ENVIRONMENT'
-00000b60: 2c20 2764 6576 656c 6f70 2729 0a6e 6577  , 'develop').new
-00000b70: 5f72 656c 6963 5f61 6363 6f75 6e74 5f69  _relic_account_i
-00000b80: 6420 3d20 6f73 2e67 6574 656e 7628 274e  d = os.getenv('N
-00000b90: 4557 5f52 454c 4943 5f41 4343 4f55 4e54  EW_RELIC_ACCOUNT
-00000ba0: 5f49 4427 290a 6e65 775f 7265 6c69 635f  _ID').new_relic_
-00000bb0: 6c69 6365 6e73 655f 6b65 7920 3d20 6f73  license_key = os
-00000bc0: 2e67 6574 656e 7628 274e 4557 5f52 454c  .getenv('NEW_REL
-00000bd0: 4943 5f4c 4943 454e 5345 5f4b 4559 2729  IC_LICENSE_KEY')
-00000be0: 0a0a 6e65 775f 7265 6c69 635f 7374 6163  ..new_relic_stac
-00000bf0: 6b20 3d20 4e65 7752 656c 6963 5374 6163  k = NewRelicStac
-00000c00: 6b28 0a20 2020 2061 7070 2c0a 2020 2020  k(.    app,.    
-00000c10: 274e 6577 5265 6c69 6353 7461 636b 272c  'NewRelicStack',
-00000c20: 0a20 2020 2065 6e76 3d65 6e76 6972 6f6e  .    env=environ
-00000c30: 6d65 6e74 2c0a 2020 2020 7374 6167 653d  ment,.    stage=
-00000c40: 7374 6167 652c 0a20 2020 206e 6577 5f72  stage,.    new_r
-00000c50: 656c 6963 5f62 7563 6b65 745f 6e61 6d65  elic_bucket_name
-00000c60: 3d66 276e 6575 6c61 6273 2d6e 6577 7265  =f'neulabs-newre
-00000c70: 6c69 632d 7b73 7461 6765 7d27 2c0a 2020  lic-{stage}',.  
-00000c80: 2020 6e65 775f 7265 6c69 635f 6163 636f    new_relic_acco
-00000c90: 756e 745f 6964 3d6e 6577 5f72 656c 6963  unt_id=new_relic
-00000ca0: 5f61 6363 6f75 6e74 5f69 642c 0a20 2020  _account_id,.   
-00000cb0: 206e 6577 5f72 656c 6963 5f6c 6963 656e   new_relic_licen
-00000cc0: 7365 5f6b 6579 3d6e 6577 5f72 656c 6963  se_key=new_relic
-00000cd0: 5f6c 6963 656e 7365 5f6b 6579 2c0a 2020  _license_key,.  
-00000ce0: 2020 6e65 775f 7265 6c69 635f 6170 695f    new_relic_api_
-00000cf0: 7572 6c5f 6d65 7472 6963 733d 456e 6470  url_metrics=Endp
-00000d00: 6f69 6e74 5572 6c4d 6574 7269 6373 2e45  ointUrlMetrics.E
-00000d10: 555f 4d45 5452 4943 532c 0a20 2020 206e  U_METRICS,.    n
-00000d20: 6577 5f72 656c 6963 5f61 7069 5f75 726c  ew_relic_api_url
-00000d30: 5f6c 6f67 733d 456e 6470 6f69 6e74 5572  _logs=EndpointUr
-00000d40: 6c4c 6f67 732e 4555 5f4c 4f47 532c 0a29  lLogs.EU_LOGS,.)
-00000d50: 0a60 6060 0a0a 2323 2320 4465 7620 6d6f  .```..### Dev mo
-00000d60: 6465 0a0a 5275 6e20 696e 2073 6865 6c6c  de..Run in shell
-00000d70: 0a0a 6060 600a 6e70 7820 7072 6f6a 656e  ..```.npx projen
-00000d80: 2064 6566 6175 6c74 0a60 6060 0a0a 2323   default.```..##
-00000d90: 2320 436f 6e74 7269 6275 746f 7273 0a0a  # Contributors..
-00000da0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000db0: 2f67 6974 6875 622e 636f 6d2f 6e65 756c  /github.com/neul
-00000dc0: 6162 7363 6f6d 2f6e 6575 6c61 6273 2d63  abscom/neulabs-c
-00000dd0: 646b 2d63 6f6e 7374 7275 6374 732f 6772  dk-constructs/gr
-00000de0: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
-00000df0: 7322 3e20 3c69 6d67 2073 7263 3d22 6874  s"> <img src="ht
-00000e00: 7470 733a 2f2f 636f 6e74 7269 622e 726f  tps://contrib.ro
-00000e10: 636b 732f 696d 6167 653f 7265 706f 3d6e  cks/image?repo=n
-00000e20: 6575 6c61 6273 636f 6d2f 6e65 756c 6162  eulabscom/neulab
-00000e30: 732d 6364 6b2d 636f 6e73 7472 7563 7473  s-cdk-constructs
-00000e40: 2220 2f3e 203c 2f61 3e0a 0a23 2323 204c  " /> </a>..### L
-00000e50: 6963 656e 7365 0a0a 5365 6520 7468 6520  icense..See the 
-00000e60: 604c 4943 454e 5345 6020 6669 6c65 2066  `LICENSE` file f
-00000e70: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00000e80: 696f 6e2e 0a                             ion..
+00000960: 4372 6561 7465 2047 6974 6875 6220 4f49  Create Github OI
+00000970: 4443 2a2a 0a0a 5468 6520 6372 6561 7469  DC**..The creati
+00000980: 6f6e 206f 6620 4769 7468 7562 204f 4944  on of Github OID
+00000990: 4320 616c 6c6f 7773 2061 2072 6f6c 6520  C allows a role 
+000009a0: 7769 7468 696e 2077 6f72 6b66 6c6f 7773  within workflows
+000009b0: 2074 6f20 6265 2075 7365 6420 746f 206c   to be used to l
+000009c0: 6f67 2069 6e20 746f 2061 7773 2e0a 496e  og in to aws..In
+000009d0: 2074 6869 7320 7374 6163 6b2c 2074 6865   this stack, the
+000009e0: 3a0a 0a2a 2067 6974 6875 622d 6f69 6463  :..* github-oidc
+000009f0: 2d77 6f72 6b66 6c6f 772d 726f 6c65 2075  -workflow-role u
+00000a00: 7365 7220 7573 6564 2066 6f72 2061 7574  ser used for aut
+00000a10: 6865 6e74 6963 6174 696f 6e0a 2a20 6364  hentication.* cd
+00000a20: 6b2d 6f69 6463 2d64 6570 6c6f 792d 726f  k-oidc-deploy-ro
+00000a30: 6c65 2072 6f6c 6520 7573 6564 2066 6f72  le role used for
+00000a40: 2064 6570 6c6f 7969 6e67 0a2a 2063 646b   deploying.* cdk
+00000a50: 2d6f 6964 632d 626f 6f74 7372 6170 2d72  -oidc-bootsrap-r
+00000a60: 6f6c 6520 726f 6c65 2075 7365 6420 666f  ole role used fo
+00000a70: 7220 626f 6f74 7374 7261 700a 0a60 6060  r bootstrap..```
+00000a80: 0a65 6e76 6972 6f6e 6d65 6e74 203d 2070  .environment = p
+00000a90: 726f 6365 7373 2e65 6e76 2e45 4e56 4952  rocess.env.ENVIR
+00000aa0: 4f4e 4d45 4e54 2120 7c7c 2027 7374 6167  ONMENT! || 'stag
+00000ab0: 696e 6727 3b0a 0a6e 6577 2047 6974 6875  ing';..new Githu
+00000ac0: 624f 4944 4353 7461 636b 2861 7070 2c20  bOIDCStack(app, 
+00000ad0: 274f 6964 6353 7461 636b 272c 207b 0a20  'OidcStack', {. 
+00000ae0: 2065 6e76 3a20 7b0a 2020 2020 6163 636f   env: {.    acco
+00000af0: 756e 743a 2070 726f 6365 7373 2e65 6e76  unt: process.env
+00000b00: 2e43 444b 5f44 4546 4155 4c54 5f41 4343  .CDK_DEFAULT_ACC
+00000b10: 4f55 4e54 2c0a 2020 2020 7265 6769 6f6e  OUNT,.    region
+00000b20: 3a20 7072 6f63 6573 732e 656e 762e 4344  : process.env.CD
+00000b30: 4b5f 4445 4641 554c 545f 5245 4749 4f4e  K_DEFAULT_REGION
+00000b40: 2c0a 2020 7d2c 0a20 2073 7461 6765 3a20  ,.  },.  stage: 
+00000b50: 656e 7669 726f 6e6d 656e 742c 0a20 2067  environment,.  g
+00000b60: 6974 6875 6255 7365 723a 2027 7573 6572  ithubUser: 'user
+00000b70: 6e61 6d65 272c 0a20 2067 6974 6875 6252  name',.  githubR
+00000b80: 6570 6f73 6974 6f72 793a 2027 7265 706f  epository: 'repo
+00000b90: 7369 746f 7279 4e61 6d65 272c 2023 2059  sitoryName', # Y
+00000ba0: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00000bb0: 272a 270a 2020 746f 6b65 6e41 6374 696f  '*'.  tokenActio
+00000bc0: 6e3a 2054 6f6b 656e 4163 7469 6f6e 732e  n: TokenActions.
+00000bd0: 414c 4c2c 0a20 2063 646b 4465 706c 6f79  ALL,.  cdkDeploy
+00000be0: 526f 6c65 4d61 6e61 6765 6450 6f6c 6963  RoleManagedPolic
+00000bf0: 6965 733a 205b 2741 646d 696e 6973 7472  ies: ['Administr
+00000c00: 6174 6f72 4163 6365 7373 275d 2c0a 7d29  atorAccess'],.})
+00000c10: 3b0a 6060 600a 0a47 6974 6875 6220 776f  ;.```..Github wo
+00000c20: 726b 666c 6f77 0a0a 6060 600a 2e2e 2e0a  rkflow..```.....
+00000c30: 0a23 2070 6572 6d69 7373 696f 6e20 6361  .# permission ca
+00000c40: 6e20 6265 2061 6464 6564 2061 7420 6a6f  n be added at jo
+00000c50: 6220 6c65 7665 6c20 6f72 2077 6f72 6b66  b level or workf
+00000c60: 6c6f 7720 6c65 7665 6c0a 7065 726d 6973  low level.permis
+00000c70: 7369 6f6e 733a 0a20 2069 642d 746f 6b65  sions:.  id-toke
+00000c80: 6e3a 2077 7269 7465 0a20 2063 6f6e 7465  n: write.  conte
+00000c90: 6e74 733a 2072 6561 6420 2020 2023 2054  nts: read    # T
+00000ca0: 6869 7320 6973 2072 6571 7569 7265 6420  his is required 
+00000cb0: 666f 7220 6163 7469 6f6e 732f 6368 6563  for actions/chec
+00000cc0: 6b6f 7574 0a0a 6a6f 6273 3a0a 2020 2e2e  kout..jobs:.  ..
+00000cd0: 2e0a 0a20 206f 6964 633a 0a20 2020 206e  ...  oidc:.    n
+00000ce0: 616d 653a 2041 7574 680a 2020 2020 7275  ame: Auth.    ru
+00000cf0: 6e73 2d6f 6e3a 2075 6275 6e74 752d 3230  ns-on: ubuntu-20
+00000d00: 2e30 340a 2020 2020 7374 6570 733a 0a20  .04.    steps:. 
+00000d10: 2020 2020 202d 206e 616d 653a 2043 6f6e       - name: Con
+00000d20: 6669 6775 7265 2061 7773 2063 7265 6465  figure aws crede
+00000d30: 6e74 6961 6c73 0a20 2020 2020 2020 2075  ntials.        u
+00000d40: 7365 733a 2061 7773 2d61 6374 696f 6e73  ses: aws-actions
+00000d50: 2f63 6f6e 6669 6775 7265 2d61 7773 2d63  /configure-aws-c
+00000d60: 7265 6465 6e74 6961 6c73 4076 310a 2020  redentials@v1.  
+00000d70: 2020 2020 2020 7769 7468 3a0a 2020 2020        with:.    
+00000d80: 2020 2020 2020 726f 6c65 2d74 6f2d 6173        role-to-as
+00000d90: 7375 6d65 3a20 6172 6e3a 6177 733a 6961  sume: arn:aws:ia
+00000da0: 6d3a 3a7b 4143 434f 554e 5420 4944 7d3a  m::{ACCOUNT ID}:
+00000db0: 726f 6c65 2f67 6974 6875 622d 6f69 6463  role/github-oidc
+00000dc0: 2d77 6f72 6b66 6c6f 772d 726f 6c65 0a20  -workflow-role. 
+00000dd0: 2020 2020 2020 2020 2061 7773 2d72 6567           aws-reg
+00000de0: 696f 6e3a 207b 5245 4749 4f4e 7d0a 2020  ion: {REGION}.  
+00000df0: 2020 2020 2020 2020 6d61 736b 2d61 7773          mask-aws
+00000e00: 2d61 6363 6f75 6e74 2d69 643a 206e 6f0a  -account-id: no.
+00000e10: 0a20 202e 2e2e 0a60 6060 0a0a 2a2a 4372  .  ....```..**Cr
+00000e20: 6561 7465 204e 6577 5265 6c69 6320 436f  eate NewRelic Co
+00000e30: 6e6e 6563 7469 6f6e 2a2a 0a0a 5468 6520  nnection**..The 
+00000e40: 4e65 7752 656c 6963 5374 6163 6b20 696d  NewRelicStack im
+00000e50: 706c 656d 656e 7473 2074 6865 2069 6e66  plements the inf
+00000e60: 7261 7374 7275 6374 7572 6520 746f 2073  rastructure to s
+00000e70: 656e 6420 6d65 7472 6963 7320 616e 6420  end metrics and 
+00000e80: 6c6f 6773 2074 6f20 4e65 7772 656c 6963  logs to Newrelic
+00000e90: 2074 6872 6f75 6768 204b 696e 6573 6973   through Kinesis
+00000ea0: 2061 6e64 2043 6c6f 7564 7761 7463 6820   and Cloudwatch 
+00000eb0: 5374 7265 616d 2e0a 4f6e 6365 2064 6570  Stream..Once dep
+00000ec0: 6c6f 7965 6420 796f 7520 6361 6e20 636f  loyed you can co
+00000ed0: 7079 2074 6865 2041 524e 206f 6620 7468  py the ARN of th
+00000ee0: 6520 274e 6577 5265 6c69 6349 6e66 7261  e 'NewRelicInfra
+00000ef0: 7374 7275 6374 7572 652d 496e 7465 6772  structure-Integr
+00000f00: 6174 696f 6e73 2720 726f 6c65 2061 6e64  ations' role and
+00000f10: 2075 7365 2069 7420 746f 2063 6f6e 6669   use it to confi
+00000f20: 6775 7265 204e 6577 7265 6c69 632e 0a0a  gure Newrelic...
+00000f30: 6060 600a 2020 6e65 7720 4e65 7752 656c  ```.  new NewRel
+00000f40: 6963 5374 6163 6b28 6170 702c 2027 4e65  icStack(app, 'Ne
+00000f50: 7772 656c 6963 5374 6163 6b27 2c20 7b0a  wrelicStack', {.
+00000f60: 2020 2020 656e 763a 2063 6f6e 7374 616e      env: constan
+00000f70: 7473 2e65 6e76 2c0a 2020 2020 7374 6167  ts.env,.    stag
+00000f80: 653a 2063 6f6e 7374 616e 7473 2e65 6e76  e: constants.env
+00000f90: 6972 6f6e 6d65 6e74 2c0a 2020 2020 6e65  ironment,.    ne
+00000fa0: 7752 656c 6963 4275 636b 6574 4e61 6d65  wRelicBucketName
+00000fb0: 3a20 606e 6577 7265 6c69 632d 247b 636f  : `newrelic-${co
+00000fc0: 6e73 7461 6e74 732e 6177 7341 6363 6f75  nstants.awsAccou
+00000fd0: 6e74 4964 7d2d 247b 636f 6e73 7461 6e74  ntId}-${constant
+00000fe0: 732e 656e 7669 726f 6e6d 656e 747d 602c  s.environment}`,
+00000ff0: 0a20 2020 206e 6577 5265 6c69 6341 6363  .    newRelicAcc
+00001000: 6f75 6e74 4964 3a20 6e65 7752 656c 6963  ountId: newRelic
+00001010: 4163 636f 756e 7449 642c 0a20 2020 206e  AccountId,.    n
+00001020: 6577 5265 6c69 634c 6963 656e 7365 4b65  ewRelicLicenseKe
+00001030: 793a 206e 6577 5265 6c69 634c 6963 656e  y: newRelicLicen
+00001040: 7365 4b65 792c 0a20 2020 206e 6577 5265  seKey,.    newRe
+00001050: 6c69 6341 7069 5572 6c4d 6574 7269 6373  licApiUrlMetrics
+00001060: 3a20 456e 6470 6f69 6e74 5572 6c4d 6574  : EndpointUrlMet
+00001070: 7269 6373 2e45 555f 4d45 5452 4943 532c  rics.EU_METRICS,
+00001080: 0a20 2020 206e 6577 5265 6c69 6341 7069  .    newRelicApi
+00001090: 5572 6c4c 6f67 733a 2045 6e64 706f 696e  UrlLogs: Endpoin
+000010a0: 7455 726c 4c6f 6773 2e45 555f 4c4f 4753  tUrlLogs.EU_LOGS
+000010b0: 2c0a 2020 7d29 3b0a 6060 600a 0a23 2323  ,.  });.```..###
+000010c0: 2044 6576 206d 6f64 650a 0a52 756e 2069   Dev mode..Run i
+000010d0: 6e20 7368 656c 6c0a 0a60 6060 0a6e 7078  n shell..```.npx
+000010e0: 2070 726f 6a65 6e20 6465 6661 756c 740a   projen default.
+000010f0: 6060 600a 0a23 2323 2043 6f6e 7472 6962  ```..### Contrib
+00001100: 7574 6f72 730a 0a3c 6120 6872 6566 3d22  utors..<a href="
+00001110: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001120: 6f6d 2f6e 6575 6c61 6273 636f 6d2f 6e65  om/neulabscom/ne
+00001130: 756c 6162 732d 6364 6b2d 636f 6e73 7472  ulabs-cdk-constr
+00001140: 7563 7473 2f67 7261 7068 732f 636f 6e74  ucts/graphs/cont
+00001150: 7269 6275 746f 7273 223e 203c 696d 6720  ributors"> <img 
+00001160: 7372 633d 2268 7474 7073 3a2f 2f63 6f6e  src="https://con
+00001170: 7472 6962 2e72 6f63 6b73 2f69 6d61 6765  trib.rocks/image
+00001180: 3f72 6570 6f3d 6e65 756c 6162 7363 6f6d  ?repo=neulabscom
+00001190: 2f6e 6575 6c61 6273 2d63 646b 2d63 6f6e  /neulabs-cdk-con
+000011a0: 7374 7275 6374 7322 202f 3e20 3c2f 613e  structs" /> </a>
+000011b0: 0a0a 2323 2320 4c69 6365 6e73 650a 0a53  ..### License..S
+000011c0: 6565 2074 6865 2060 4c49 4345 4e53 4560  ee the `LICENSE`
+000011d0: 2066 696c 6520 666f 7220 6d6f 7265 2069   file for more i
+000011e0: 6e66 6f72 6d61 7469 6f6e 2e0a            nformation..
```

### Comparing `neulabs-cdk-constructs-0.3.6/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.3.7/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.6.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.7.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

