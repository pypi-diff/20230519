# Comparing `tmp/alibabacloud_oceanbasepro20190901-1.0.7.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.7.tar", last modified: Mon Apr 10 03:09:53 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.8.tar", last modified: Fri May 19 10:09:54 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901-1.0.7.tar` & `alibabacloud_oceanbasepro20190901-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265912 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   791228 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   268062 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)   828724 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/LICENSE` & `alibabacloud_oceanbasepro20190901-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/README-CN.md` & `alibabacloud_oceanbasepro20190901-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/README.md` & `alibabacloud_oceanbasepro20190901-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,16 @@
 
     def create_oms_mysql_data_source_with_options(
         self,
         request: ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceResponse:
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
         @param request: CreateOmsMysqlDataSourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateOmsMysqlDataSourceResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -310,15 +311,16 @@
 
     async def create_oms_mysql_data_source_with_options_async(
         self,
         request: ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceResponse:
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
         @param request: CreateOmsMysqlDataSourceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateOmsMysqlDataSourceResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -364,28 +366,30 @@
         )
 
     def create_oms_mysql_data_source(
         self,
         request: ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceRequest,
     ) -> ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceResponse:
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
         @param request: CreateOmsMysqlDataSourceRequest
         @return: CreateOmsMysqlDataSourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_oms_mysql_data_source_with_options(request, runtime)
 
     async def create_oms_mysql_data_source_async(
         self,
         request: ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceRequest,
     ) -> ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceResponse:
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
         @param request: CreateOmsMysqlDataSourceRequest
         @return: CreateOmsMysqlDataSourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_oms_mysql_data_source_with_options_async(request, runtime)
 
@@ -967,17 +971,15 @@
 
     def delete_instances_with_options(
         self,
         request: ocean_base_pro_20190901_models.DeleteInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DeleteInstancesResponse:
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
         @param request: DeleteInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteInstancesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1006,17 +1008,15 @@
 
     async def delete_instances_with_options_async(
         self,
         request: ocean_base_pro_20190901_models.DeleteInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DeleteInstancesResponse:
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
         @param request: DeleteInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteInstancesResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1044,32 +1044,28 @@
         )
 
     def delete_instances(
         self,
         request: ocean_base_pro_20190901_models.DeleteInstancesRequest,
     ) -> ocean_base_pro_20190901_models.DeleteInstancesResponse:
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
         @param request: DeleteInstancesRequest
         @return: DeleteInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_instances_with_options(request, runtime)
 
     async def delete_instances_async(
         self,
         request: ocean_base_pro_20190901_models.DeleteInstancesRequest,
     ) -> ocean_base_pro_20190901_models.DeleteInstancesResponse:
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
         @param request: DeleteInstancesRequest
         @return: DeleteInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_instances_with_options_async(request, runtime)
 
@@ -1682,14 +1678,16 @@
     def describe_charset_with_options(
         self,
         request: ocean_base_pro_20190901_models.DescribeCharsetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DescribeCharsetResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.series):
+            body['Series'] = request.series
         if not UtilClient.is_unset(request.tenant_mode):
             body['TenantMode'] = request.tenant_mode
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCharset',
@@ -1710,14 +1708,16 @@
     async def describe_charset_with_options_async(
         self,
         request: ocean_base_pro_20190901_models.DescribeCharsetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DescribeCharsetResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.series):
+            body['Series'] = request.series
         if not UtilClient.is_unset(request.tenant_mode):
             body['TenantMode'] = request.tenant_mode
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeCharset',
@@ -4381,14 +4381,92 @@
     async def describe_zones_async(
         self,
         request: ocean_base_pro_20190901_models.DescribeZonesRequest,
     ) -> ocean_base_pro_20190901_models.DescribeZonesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_zones_with_options_async(request, runtime)
 
+    def kill_process_list_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.KillProcessListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.KillProcessListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.session_list):
+            body['SessionList'] = request.session_list
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='KillProcessList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.KillProcessListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def kill_process_list_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.KillProcessListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.KillProcessListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.session_list):
+            body['SessionList'] = request.session_list
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='KillProcessList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.KillProcessListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def kill_process_list(
+        self,
+        request: ocean_base_pro_20190901_models.KillProcessListRequest,
+    ) -> ocean_base_pro_20190901_models.KillProcessListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.kill_process_list_with_options(request, runtime)
+
+    async def kill_process_list_async(
+        self,
+        request: ocean_base_pro_20190901_models.KillProcessListRequest,
+    ) -> ocean_base_pro_20190901_models.KillProcessListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.kill_process_list_with_options_async(request, runtime)
+
     def modify_database_description_with_options(
         self,
         request: ocean_base_pro_20190901_models.ModifyDatabaseDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.ModifyDatabaseDescriptionResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -5348,14 +5426,16 @@
     def modify_tenant_user_password_with_options(
         self,
         request: ocean_base_pro_20190901_models.ModifyTenantUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.ModifyTenantUserPasswordResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.encryption_type):
+            body['EncryptionType'] = request.encryption_type
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_name):
             body['UserName'] = request.user_name
         if not UtilClient.is_unset(request.user_password):
@@ -5382,14 +5462,16 @@
     async def modify_tenant_user_password_with_options_async(
         self,
         request: ocean_base_pro_20190901_models.ModifyTenantUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.ModifyTenantUserPasswordResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.encryption_type):
+            body['EncryptionType'] = request.encryption_type
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_name):
             body['UserName'] = request.user_name
         if not UtilClient.is_unset(request.user_password):
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,32 +11,30 @@
         collation: str = None,
         database_name: str = None,
         description: str = None,
         encoding: str = None,
         instance_id: str = None,
         tenant_id: str = None,
     ):
-        # The token used to ensure idempotence.  
-        # The value of this parameter is generated by the client and is unique among different requests.   
-        # 
-        # > <br>ClientToken can contain only ASCII characters, and cannot exceed 64 characters in length.
+        # The name of the database.
         self.client_token = client_token
-        # The collation.
+        # The encoding standard of the database.
+        # For more information, see the Charset field returned by the DescribeCharset operation.
         self.collation = collation
-        # The name of the database.   
-        # You cannot use reserved keywords, such as test and mysql.
+        # Alibaba Cloud CLI
         self.database_name = database_name
-        # The description of the database.
+        # The operation that you want to perform.   
+        # Set the value to **CreateDatabase**.
         self.description = description
-        # The encoding standard of the database.
-        # For more information, see the Charset field returned by the DescribeCharset operation.
+        # The ID of the tenant.
         self.encoding = encoding
-        # The ID of the OceanBase cluster.
+        # The collation.
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # The name of the database.   
+        # You cannot use reserved keywords, such as test and mysql.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -81,17 +79,16 @@
 
 class CreateDatabaseResponseBody(TeaModel):
     def __init__(
         self,
         database_name: str = None,
         request_id: str = None,
     ):
-        # The name of the database.
+        # CreateDatabase
         self.database_name = database_name
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -177,60 +174,63 @@
     ):
         # Specifies whether to enable automatic renewal.   
         # This parameter is valid only when the ChargeType parameter is set to PrePaid. Valid values: 
         # - true: enables automatic renewal for the instance.   
         # - false: disables automatic renewal for the instance. This is the default value.
         self.auto_renew = auto_renew
         # The automatic renewal period of the instance. This parameter is required when the AutoRenew parameter is set to true. Valid values:  
-        # - If the PeriodUnit parameter is set to Week: 1, 2, and 3.   
-        # - If the PeriodUnit parameter is set to Month: 1, 2, 3, 6, and 12.
+        # - If the PeriodUnit parameter is set to Year: "1", "2", and "3".   
+        # - If the PeriodUnit parameter is set to Month: "1", "2", "3", "6", and "12".
         self.auto_renew_period = auto_renew_period
         # The billing method of the instance. Valid values:  
-        # -PrePay: the subscription billing method. You must ensure that the remaining balance or credit balance of your account can cover the cost of the subscription. Otherwise, you will receive an InvalidPayMethod error. 
+        # - PrePay: the subscription billing method. You must ensure that the remaining balance or credit balance of your account can cover the cost of the subscription. Otherwise, you will receive an InvalidPayMethod error. 
         # - PostPay: the pay-as-you-go billing method. This is the default value. By default, fees are charged on an hourly basis.
         self.charge_type = charge_type
-        # The size of the storage space, in GB.    
+        # The size of the storage space,in GB.    
         # The limits on the storage space vary with the cluster specifications:   
         # - 8C32GB: 100 GB to 10000 GB   
         # - 14C70GB: 200 GB to 10000 GB   
         # - 30C180GB: 400 GB to 10000 GB   
         # - 62C400GB: 800 GB to 10000 GB    
         # The preceding minimum storage space sizes are the default storage space sizes of the corresponding cluster specification plans.
         self.disk_size = disk_size
+        # The return result of the request.
         self.disk_type = disk_type
         # The specifications of the cluster.     
         # You can specify one of the following four plans:   
         #  - 8C32GB: indicates 8 CPU cores and 32 GB of memory.    
-        #  - 14C70GB: indicates 14 CPU cores and 70 GB of memory. This is the default value.     
+        #  - 14C70GB: indicates 14 CPU cores and 70 GB of memory. This is the default value.
         # - 30C180GB: indicates 30 CPU cores and 180 GB of memory.     
         # - 62C400GB: indicates 62 CPU cores and 400 GB of memory.
         self.instance_class = instance_class
         # The name of the OceanBase cluster.    
         # It must be 1 to 20 characters in length.   
         # If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.instance_name = instance_name
+        # OceanBase Server version number.
         self.ob_version = ob_version
         # The valid duration of the purchased resources. The unit is specified by the PeriodUnit parameter.   
-        # This parameter is valid and required only when the InstanceChargeType parameter is set to PrePaid.   
-        # If the DedicatedHostId parameter is specified, the subscription period of the instance must be shorter than that of the dedicated host.   
-        # Valid values:    
-        # - If the PeriodUnit parameter is set to Week: 1, 2, 3, and 4.   
-        # - If the PeriodUnit parameter is set to Month: 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36, 48, and 60.
+        # This parameter is valid and required only when the InstanceChargeType parameter is set to PrePaid.      
+        # Valid values:     
+        # - When the PeriodUnit parameter is set to Month: "1", "2", "3", "4", "5", "6", "7", "8", "9". 
+        # - When the PeriodUnit parameter is set to Year: "1", "2", "3".
         self.period = period
         # The unit of the valid duration of the purchased resources.     
-        # Valid value for subscription: Month.   
+        # Valid value for subscription: Month or Year.
         # Default value: Month for subscription, and Hour for pay-as-you-go.
         self.period_unit = period_unit
         # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id
         # The series of the OceanBase cluster. Valid values:    
-        # normal: the high availability edition. This is the default value.
+        # - normal: Standard Cluster Edition (Cloud Disk). This is the default value.
+        # - normal_ssd: Standard Cluster Edition (Local Disk).
+        # - history: History Database Cluster Edition.
         self.series = series
         # The ID of the zone to which the instance belongs.   
-        # For more information about how to obtain the list of zones, see [DescribeZones](https://www.alibabacloud.com/help/zh/doc-detail/25610.htm).
+        # For more information about how to obtain the list of zones, see [DescribeZones](~~25610~~).
         self.zones = zones
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -300,15 +300,17 @@
 class CreateInstanceResponseBodyData(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         order_id: str = None,
         resource_group_id: str = None,
     ):
+        # 订单ID。该参数只有创建包年包月ECS实例（请求参数InstanceChargeType=PrePaid）时有返回值。
         self.instance_id = instance_id
+        # 资源组ID
         self.order_id = order_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -338,16 +340,17 @@
 
 class CreateInstanceResponseBody(TeaModel):
     def __init__(
         self,
         data: CreateInstanceResponseBodyData = None,
         request_id: str = None,
     ):
+        # 实例ID
         self.data = data
-        # The request ID.
+        # Response parameters
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -427,53 +430,39 @@
         password: str = None,
         port: str = None,
         schema: str = None,
         type: str = None,
         username: str = None,
         vpc_id: str = None,
     ):
-        # The description of the data source.   
-        # It must be 2 to 256 characters in length. The default value is null.
         self.description = description
-        # The ID of the database gateway instance.   
-        # 
-        # > <br>If Type is set to DG, this parameter is required.
         self.dg_database_id = dg_database_id
-        # The ID of the ECS instance of the data source.   
-        # 
-        # > <br>If Type is set to RDS, POLARDB, or DG, this parameter is required.
         self.instance_id = instance_id
-        # The IP address of the data source.   
-        # 
-        # > <br>If Type is set to INTERNET or VPC, this parameter is required.
         self.ip = ip
-        # The name of the data source.   
-        # It must be 2 to 128 characters in length and can contain letters, digits, underscores (_), periods (.), and hyphens (-).   
-        # 
-        # > <br>Invalid characters, such as slashes (/), are not allowed.
+        # ```
+        # http(s)://[Endpoint]/?Action=CreateOmsMysqlDataSource
+        # &Name=oms-mysql
+        # &Type=INTERNET
+        # &VpcId=vpc-12345abcde*******\
+        # &InstanceId=pc-12ab34cd56******\
+        # &DgDatabaseId=dg-yhss6sdlaff****\
+        # &Ip=10.0.****\
+        # &Port=3306
+        # &Schema=test
+        # &Username=omsTestUser
+        # &Password=YWJjZDEyM0Ah
+        # &Description=MySQL data source for OMS testing
+        # &Common request parameters
+        # ```
         self.name = name
-        # The password of the username that is used to access the database. It must be Base64 encoded.   
-        # For example, for the password abcd123@!, the Base64-encoded value is YWJjZDEyM0Ah.
         self.password = password
-        # The port number of the data source.   
-        # 
-        # > <br>If Type is set to INTERNET or VPC, this parameter is required.
         self.port = port
-        # The name of the database.   
-        # 
-        # > <br>If you specify this parameter, subsequent migration or synchronization operations will take effect on this database only.
         self.schema = schema
-        # The type of the MySQL data source.   
-        # Valid values: INTERNET, VPC, RDS, POLARDB, and DG.
         self.type = type
-        # The username that is used to access the database.
         self.username = username
-        # The ID of the VPC to which the data source belongs.   
-        # 
-        # > <br>If Type is set to VPC, this parameter is required.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -533,15 +522,14 @@
 
 
 class CreateOmsMysqlDataSourceResponseBodyData(TeaModel):
     def __init__(
         self,
         endpoint_id: str = None,
     ):
-        # The ID of the data source record.
         self.endpoint_id = endpoint_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -562,17 +550,15 @@
 
 class CreateOmsMysqlDataSourceResponseBody(TeaModel):
     def __init__(
         self,
         data: CreateOmsMysqlDataSourceResponseBodyData = None,
         request_id: str = None,
     ):
-        # The return result of the request.
         self.data = data
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -653,37 +639,25 @@
         producer_group: str = None,
         send_msg_timeout: int = None,
         sequence_enable: bool = None,
         sequence_start_timestamp: int = None,
         serializer_type: str = None,
         topic_type: str = None,
     ):
-        # Specifies whether to enable message tracing when the destination data source is RocketMQ.
         self.enable_msg_trace = enable_msg_trace
-        # The ID of the data source.
         self.endpoint_id = endpoint_id
-        # The type of the data source. Valid values: `MYSQL`, `MARIADB`, `OB_MYSQL`, `OB_MYSQL_CE`, `OB_ORACLE`, `ORACLE`, `DB2_LUW`, `KAFKA`, `ROCKETMQ`, `DATAHUB`, `SYBASE`, `LOGPROXY`, `ADB`, `DBP_OP_ROUTE`, `DMS`, `IDB`, and `TIDB`.
         self.endpoint_type = endpoint_type
-        # The tag of the Post message when the destination data source is RocketMQ.
         self.msg_tags = msg_tags
-        # The partitioned index, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ, and the partitioning mode is set to ONE.
         self.partition = partition
-        # The partitioning mode, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: ONE, HASH, and TABLE.
         self.partition_mode = partition_mode
-        # The producer group of the Post message when the destination data source is RocketMQ.
         self.producer_group = producer_group
-        # The timeout period for a single Post message when the destination data source is RocketMQ.
         self.send_msg_timeout = send_msg_timeout
-        # Specifies whether to enable message sequencing when the destination data source is DataHub.
         self.sequence_enable = sequence_enable
-        # The start time of the sequence, which must be specified if the destination data source is DataHub and message sequencing is enabled. The value is a timestamp in seconds.
         self.sequence_start_timestamp = sequence_start_timestamp
-        # The text serialization type, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: Default, Canal, Dataworks, SharePlex, and DefaultExtendColumnType.
         self.serializer_type = serializer_type
-        # The type of the topic to which the Post message belongs when the destination data source is DataHub. Valid values: Tuple and Blob.
         self.topic_type = topic_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -758,37 +732,25 @@
         producer_group: str = None,
         send_msg_timeout: int = None,
         sequence_enable: bool = None,
         sequence_start_timestamp: int = None,
         serializer_type: str = None,
         topic_type: str = None,
     ):
-        # Specifies whether to enable message tracing when the destination data source is RocketMQ.
         self.enable_msg_trace = enable_msg_trace
-        # The ID of the data source.
         self.endpoint_id = endpoint_id
-        # The type of the data source. Valid values: `MYSQL`, `MARIADB`, `OB_MYSQL`, `OB_MYSQL_CE`, `OB_ORACLE`, `ORACLE`, `DB2_LUW`, `KAFKA`, `ROCKETMQ`, `DATAHUB`, `SYBASE`, `LOGPROXY`, `ADB`, `DBP_OP_ROUTE`, `DMS`, `IDB`, and `TIDB`.
         self.endpoint_type = endpoint_type
-        # The tag of the Post message when the destination data source is RocketMQ.
         self.msg_tags = msg_tags
-        # The partitioned index, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ, and the partitioning mode is set to ONE.
         self.partition = partition
-        # The partitioning mode, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: ONE, HASH, and TABLE.
         self.partition_mode = partition_mode
-        # The producer group of the Post message when the destination data source is RocketMQ.
         self.producer_group = producer_group
-        # The timeout period for a single Post message when the destination data source is RocketMQ.
         self.send_msg_timeout = send_msg_timeout
-        # Specifies whether to enable message sequencing when the destination data source is DataHub.
         self.sequence_enable = sequence_enable
-        # The start time of the sequence, which must be specified if the destination data source is DataHub and message sequencing is enabled. The value is a timestamp in seconds.
         self.sequence_start_timestamp = sequence_start_timestamp
-        # The text serialization type, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: Default, Canal, Dataworks, SharePlex, and DefaultExtendColumnType.
         self.serializer_type = serializer_type
-        # The type of the topic to which the Post message belongs when the destination data source is DataHub. Valid values: Tuple and Blob.
         self.topic_type = topic_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -855,21 +817,17 @@
     def __init__(
         self,
         distributed_keys: List[str] = None,
         partition_life_cycle: int = None,
         partition_statement: str = None,
         primary_keys: List[str] = None,
     ):
-        # The list of distribution key columns.
         self.distributed_keys = distributed_keys
-        # The lifecycle of the table.
         self.partition_life_cycle = partition_life_cycle
-        # The partitioning expression.
         self.partition_statement = partition_statement
-        # The list of primary key columns.
         self.primary_keys = primary_keys
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -908,29 +866,21 @@
         mapped_name: str = None,
         shard_columns: List[str] = None,
         table_id: str = None,
         table_name: str = None,
         type: str = None,
         where_clause: str = None,
     ):
-        # The schema of the ADB table. If the destination data source is ADB, you need to configure additional information for schema synchronization.
         self.adb_table_schema = adb_table_schema
-        # The list of filter columns, which are the columns to be synchronized.
         self.filter_columns = filter_columns
-        # The name of the mapped-to table or topic. If the destination data source is a database, this parameter specifies the name of the mapped-to table. If the destination data source is a message queue system, this parameter specifies the name of the mapped-to topic.
         self.mapped_name = mapped_name
-        # The list of sharding key columns. This parameter applies to scenarios where the destination data source is a message queue system.
         self.shard_columns = shard_columns
-        # The ID of the table. This parameter takes effect when the source data source is IDB.
         self.table_id = table_id
-        # The name of the table.
         self.table_name = table_name
-        # Valid values: DATABASE and TABLE.
         self.type = type
-        # The row filter conditions.
         self.where_clause = where_clause
 
     def validate(self):
         if self.adb_table_schema:
             self.adb_table_schema.validate()
 
     def to_map(self):
@@ -985,25 +935,19 @@
         database_id: str = None,
         database_name: str = None,
         mapped_name: str = None,
         tables: List[CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTables] = None,
         tenant_name: str = None,
         type: str = None,
     ):
-        # The ID of the database. This parameter takes effect when the source data source is IDB.
         self.database_id = database_id
-        # The name of the database.
         self.database_name = database_name
-        # The mapped-to database. This parameter takes effect when the destination data source is a database.
         self.mapped_name = mapped_name
-        # The settings for the target table objects in the current database.
         self.tables = tables
-        # The mapped-to tenant. This parameter takes effect when the source data source is OceanBase Database.
         self.tenant_name = tenant_name
-        # Valid values: DATABASE and TABLE.
         self.type = type
 
     def validate(self):
         if self.tables:
             for k in self.tables:
                 if k:
                     k.validate()
@@ -1052,17 +996,15 @@
 
 class CreateOmsOpenAPIProjectRequestTransferMapping(TeaModel):
     def __init__(
         self,
         databases: List[CreateOmsOpenAPIProjectRequestTransferMappingDatabases] = None,
         mode: str = None,
     ):
-        # The table mapping in the source data source, which is a conventional mapping scheme and takes effect only when Mode is set to NORMAL.
         self.databases = databases
-        # The mapping type. Valid values: \"NORMAL\" and \"WHITE_AND_BLACK_LIST\".
         self.mode = mode
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -1098,23 +1040,18 @@
         self,
         record_type_list: List[str] = None,
         start_timestamp: int = None,
         store_log_kept_hour: int = None,
         store_transaction_enabled: bool = None,
         transfer_step_type: str = None,
     ):
-        # The list of data types of incremental data synchronized in incremental synchronization.
         self.record_type_list = record_type_list
-        # The start time for incremental synchronization. The value is a timestamp in seconds.
         self.start_timestamp = start_timestamp
-        # The retention time of logs when incremental synchronization is enabled and the incremental log pull component is Store.
         self.store_log_kept_hour = store_log_kept_hour
-        # Specifies whether to enable intra-transaction sequencing when incremental synchronization is enabled and the incremental log pull component is Store.
         self.store_transaction_enabled = store_transaction_enabled
-        # Valid values: STRUCT, FULL, and INCR.
         self.transfer_step_type = transfer_step_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1153,21 +1090,17 @@
     def __init__(
         self,
         enable_full_sync: bool = None,
         enable_incr_sync: bool = None,
         enable_struct_sync: bool = None,
         incr_sync_step_transfer_config: CreateOmsOpenAPIProjectRequestTransferStepConfigIncrSyncStepTransferConfig = None,
     ):
-        # Specifies whether to enable full migration.
         self.enable_full_sync = enable_full_sync
-        # Specifies whether to enable incremental synchronization.
         self.enable_incr_sync = enable_incr_sync
-        # Specifies whether to enable schema synchronization.
         self.enable_struct_sync = enable_struct_sync
-        # The settings of incremental synchronization steps.
         self.incr_sync_step_transfer_config = incr_sync_step_transfer_config
 
     def validate(self):
         if self.incr_sync_step_transfer_config:
             self.incr_sync_step_transfer_config.validate()
 
     def to_map(self):
@@ -1210,33 +1143,26 @@
         page_size: int = None,
         project_name: str = None,
         source_config: CreateOmsOpenAPIProjectRequestSourceConfig = None,
         transfer_mapping: CreateOmsOpenAPIProjectRequestTransferMapping = None,
         transfer_step_config: CreateOmsOpenAPIProjectRequestTransferStepConfig = None,
         worker_grade_id: str = None,
     ):
-        # The business system identifier, which is optional and is a specific field of the Post message.
         self.business_name = business_name
-        # The settings of the destination data source.
         self.dest_config = dest_config
-        # A collection of label IDs.
         self.label_ids = label_ids
-        # The page number, which takes effect in a pagination query.
+        # 页序号，分页查询时生效
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # 页大小，分页查询时生效
         self.page_size = page_size
-        # The name of the project.
         self.project_name = project_name
-        # The settings of the source data source.
         self.source_config = source_config
-        # The mappings for the synchronization objects.
         self.transfer_mapping = transfer_mapping
-        # The settings of synchronization steps.
         self.transfer_step_config = transfer_step_config
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # 实例规格 ID，创建项目时生效
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         if self.dest_config:
             self.dest_config.validate()
         if self.source_config:
             self.source_config.validate()
@@ -1312,33 +1238,26 @@
         page_size: int = None,
         project_name: str = None,
         source_config_shrink: str = None,
         transfer_mapping_shrink: str = None,
         transfer_step_config_shrink: str = None,
         worker_grade_id: str = None,
     ):
-        # The business system identifier, which is optional and is a specific field of the Post message.
         self.business_name = business_name
-        # The settings of the destination data source.
         self.dest_config_shrink = dest_config_shrink
-        # A collection of label IDs.
         self.label_ids_shrink = label_ids_shrink
-        # The page number, which takes effect in a pagination query.
+        # 页序号，分页查询时生效
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # 页大小，分页查询时生效
         self.page_size = page_size
-        # The name of the project.
         self.project_name = project_name
-        # The settings of the source data source.
         self.source_config_shrink = source_config_shrink
-        # The mappings for the synchronization objects.
         self.transfer_mapping_shrink = transfer_mapping_shrink
-        # The settings of synchronization steps.
         self.transfer_step_config_shrink = transfer_step_config_shrink
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # 实例规格 ID，创建项目时生效
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1397,21 +1316,17 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
         self.code = code
-        # Valid values: CRITICAL, ERROR, and WARN.
         self.level = level
-        # The error description (new).
         self.message = message
-        # The suggestions (new).
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1453,35 +1368,24 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
         self.advice = advice
-        # The error code (old).
         self.code = code
-        # The time spent in processing the request, in seconds.
         self.cost = cost
-        # The project creation details.
         self.data = data
-        # The error details.
         self.error_detail = error_detail
-        # The error description (old).
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
         self.request_id = request_id
-        # Indicates whether the call is successful.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -1593,18 +1497,15 @@
         security_ip_group_name: str = None,
         security_ips: str = None,
     ):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
         # The name of the whitelist group.
         self.security_ip_group_name = security_ip_group_name
-        # The IP addresses or CIDR blocks in the IP address whitelist group.   
-        # It is a JSON array. Each object in the array is an IP address or CIDR block. The following two formats are supported:  
-        # - IP address: for example, 10.23.12.24. 
-        # - CIDR block: for example, 10.23.12.24/24, where 24 indicates the length of the prefix in the IP address, and the prefix is 1 to 30 characters in length.  Limit: You can set no more than 40 IP addresses or CIDR blocks for a whitelist group. A total of 200 IP addresses or CIDR blocks are supported for all whitelist groups.
+        # The return result of the request.
         self.security_ips = security_ips
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1634,20 +1535,24 @@
 class CreateSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         security_ip_group_name: str = None,
         security_ips: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # ```
+        # http(s)://[Endpoint]/?Action=CreateSecurityIpGroup
+        # &InstanceId=ob317v4uif****\
+        # &SecurityIps=192.168.1.1,192.168.0.0.1/8
+        # &SecurityIpGroupName=pay_online
+        # &Common request parameters
+        # ```
         self.instance_id = instance_id
-        # The name of the whitelist group.
+        # You can call this operation to create an IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name
-        # The IP addresses or CIDR blocks in the IP address whitelist group.   
-        # The return values of SecurityIps are strings that are separated with commas (,).
         self.security_ips = security_ips
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1676,17 +1581,19 @@
 
 class CreateSecurityIpGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         security_ip_group: CreateSecurityIpGroupResponseBodySecurityIpGroup = None,
     ):
-        # The request ID.
+        # The IP addresses or CIDR blocks in the IP address whitelist group.   
+        # The return values of SecurityIps are strings that are separated with commas (,).
         self.request_id = request_id
-        # The information of the whitelist group.
+        # The operation that you want to perform.   
+        # Set the value to **CreateSecurityIpGroup**.
         self.security_ip_group = security_ip_group
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -1767,51 +1674,42 @@
         tenant_mode: str = None,
         tenant_name: str = None,
         time_zone: str = None,
         unit_num: int = None,
         user_vswitch_id: str = None,
         user_vpc_id: str = None,
     ):
-        # The character set.    
-        # For more information, see DescribeCharset.
+        # The description of the database.
         self.charset = charset
-        # The number of CPU cores of the tenant.   
-        # 
-        # > <br>The CPU specification of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the CPU specification of the tenant cannot exceed 14 cores.
+        # The number of resource distribution nodes in the tenant.    
+        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
         self.cpu = cpu
-        # The description of the database.
+        # $.parameters[13].schema.example
         self.description = description
-        # The ID of the OceanBase cluster.
+        # The ID of the vSwitch.    
+        # If no suitable vSwitch is available, create a vSwitch as prompted.   
+        # For more information, see Use a vSwitch.
         self.instance_id = instance_id
-        # The memory size of the tenant, in GB.   
-        # 
-        # > <br>The memory size of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the memory size of the tenant cannot exceed 70 GB.
+        # The return result of the request.
         self.memory = memory
-        # The primary zone of the tenant.    
-        # It is one of the zones in which the cluster is deployed.
+        # $.parameters[12].schema.enumValueTitles
         self.primary_zone = primary_zone
-        # The tenant mode.    
-        # Valid values: Oracle and MySQL.   
-        # For more information, see [DescribeInstanceTenantModes](~~410354~~).
+        # The ID of the tenant.
         self.tenant_mode = tenant_mode
-        # The name of the tenant.    
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
+        # Alibaba Cloud CLI
         self.tenant_name = tenant_name
-        # The time zone of the tenant. For more information, see [DescribeTimeZones](~~410361~~).
+        # The memory size of the tenant, in GB.   
+        # 
+        # > <br>The memory size of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the memory size of the tenant cannot exceed 70 GB.
         self.time_zone = time_zone
-        # The number of resource distribution nodes in the tenant.    
-        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
+        # $.parameters[11].schema.description
         self.unit_num = unit_num
-        # The ID of the vSwitch.    
-        # If no suitable vSwitch is available, create a vSwitch as prompted.   
-        # For more information, see Use a vSwitch.
+        # $.parameters[12].schema.description
         self.user_vswitch_id = user_vswitch_id
-        # The ID of the VPC.   
-        #  If no suitable VPC is available, create a VPC as prompted.   
-        # For more information, see "What is a VPC".
+        # The time zone of the tenant.  For more information, see [DescribeTimeZones](https://help.aliyun.com/document_detail/410361.html).
         self.user_vpc_id = user_vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1876,17 +1774,17 @@
 
 class CreateTenantResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_id: str = None,
     ):
-        # The request ID.
+        # WB01144930
         self.request_id = request_id
-        # The ID of the tenant.
+        # You can call this operation to create a tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1956,21 +1854,16 @@
 class CreateTenantReadOnlyConnectionRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
         zone_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The ID of the zone.  
-        # 
-        # For more information, see AvailableZones in DescribeInstance.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1998,15 +1891,14 @@
 
 
 class CreateTenantReadOnlyConnectionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2079,43 +1971,27 @@
         tenant_id: str = None,
         user_name: str = None,
         user_password: str = None,
         user_type: str = None,
     ):
         # The description of the database.
         self.description = description
+        # 加密方式。
         self.encryption_type = encryption_type
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The role of the user account.   
-        # 
-        # - In Oracle mode, this parameter is left unspecified.    
-        # - In MySQL mode, the super administrator account has ALL PRIVILEGES, and you can leave this parameter unspecified.   
-        #  
-        # You need to specify the account information for a general user account. By default, the account information is a JSON array that contains the information of the role and the schema (Oracle mode) or database (MySQL mode). Valid values:  
-        # 
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.    
-        # - ReadOnly: a role that has only the read-only privilege SELECT.   
-        # - DDL: a role that has DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
-        #    
-        # - DML: a role that has DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
+        # The role of the user account.  In Oracle mode, this parameter unspecified is left unspecified.  In MySQL mode, the super administrator account has ALL PRIVILEGES, and you can leave this parameter unspecified.  You need to specify the account information for a general user account. By default, the account information is a JSON array that contains the information of the role and the schema (Oracle mode) or database (MySQL mode).  Valid values: ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES. ReadOnly: a role that has only the read-only privilege SELECT. DDL: a role that has DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW. DML: a role that has DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.roles = roles
         # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
+        # The name of the database account.  You cannot use reserved keywords, such as SYS and root.
         self.user_name = user_name
-        # The password of the database account. 
-        # 
-        # > <br>It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % ^ & \ * ( ) _ + - =\
+        # The password of the database account.  It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % \ ^ \ & \ * ( ) _ + - =\
         self.user_password = user_password
-        # The type of the database account. Valid values:   
-        # 
-        # - Admin: the super administrator account.   
-        # - Normal: a general account.
+        # The type of the database account. Valid values: Admin: the super administrator account. Normal: a general account.
         self.user_type = user_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2166,28 +2042,17 @@
     def __init__(
         self,
         database: str = None,
         role: str = None,
     ):
         # The name of the database.
         self.database = database
-        # The role of the account.   
-        # In Oracle mode, a role is a schema-level role. Valid values:  
-        # 
-        # - ReadWrite: a role that has the read and write privileges, including CREATE TABLE, CREATE VIEW, CREATE PROCEDURE, CREATE SYNONYM, CREATE SEQUENCE, CREATE TRIGGER, CREATE TYPE, CREATE SESSION, EXECUTE ANY PROCEDURE, CREATE ANY OUTLINE, ALTER ANY OUTLINE, DROP ANY OUTLINE, CREATE ANY PROCEDURE, ALTER ANY PROCEDURE, DROP ANY PROCEDURE, CREATE ANY SEQUENCE, ALTER ANY SEQUENCE, DROP ANY SEQUENCE, CREATE ANY TYPE, ALTER ANY TYPE, DROP ANY TYPE, SYSKM, CREATE ANY TRIGGER, ALTER ANY TRIGGER, DROP ANY TRIGGER, CREATE PROFILE, ALTER PROFILE, and DROP PROFILE.   
-        # - ReadOnly: a role that has only the read-only privilege SELECT. 
-        # 
-        # In MySQL mode, a role is a database-level role. Valid values:  
-        # 
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES. 
-        # - ReadOnly: a role that has only the read-only privilege SELECT.   
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW. 
-        # 
-        # > <br>By default, an Oracle account has the read and write privileges on its own schema, which are not listed here.
+        # The role of the account.  In Oracle mode, a role is a schema-level role. Valid values: - ReadWrite: a role that has the read and write privileges, including CREATE TABLE, CREATE VIEW, CREATE PROCEDURE, CREATE SYNONYM, CREATE SEQUENCE, CREATE TRIGGER, CREATE TYPE, CREATE SESSION, EXECUTE ANY PROCEDURE, CREATE ANY OUTLINE, ALTER ANY OUTLINE, DROP ANY OUTLINE, CREATE ANY PROCEDURE, ALTER ANY PROCEDURE, DROP ANY PROCEDURE, CREATE ANY SEQUENCE, ALTER ANY SEQUENCE, DROP ANY SEQUENCE, CREATE ANY TYPE, ALTER ANY TYPE, DROP ANY TYPE, SYSKM, CREATE ANY TRIGGER, ALTER ANY TRIGGER, DROP ANY TRIGGER, CREATE PROFILE, ALTER PROFILE, and DROP PROFILE. - ReadOnly: a role that has only the read-only privilege SELECT.
+        # In MySQL mode, a role is a database-level role. Valid values: - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES. - ReadOnly: a role that has only the read-only privilege SELECT. - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW. - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW. 
+        # * By default, an Oracle account has the read and write privileges on its own schema, which are not listed here.
         self.role = role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2218,21 +2083,17 @@
         user_status: str = None,
         user_type: str = None,
     ):
         # The roles of the accounts.
         self.roles = roles
         # The name of the database account.
         self.user_name = user_name
-        # The status of the database account. Valid values:    
-        # - Locked: The account is locked.   
-        # - ONLINE: The account is unlocked. The default status of a new account is ONLINE after it is created.
+        # The status of the database account. Valid values:  - Locked: The account is locked. - ONLINE: The account is unlocked. The default status of a new account is ONLINE after it is created.
         self.user_status = user_status
-        # The type of the database account. Valid values:   
-        #  - Admin: the super administrator account.   
-        #  - Normal: a general account.
+        # The type of the database account. Valid values:  - Admin: the super administrator account. - Normal: a general account.
         self.user_type = user_type
 
     def validate(self):
         if self.roles:
             for k in self.roles:
                 if k:
                     k.validate()
@@ -2361,20 +2222,16 @@
 class DeleteDatabasesRequest(TeaModel):
     def __init__(
         self,
         database_names: str = None,
         instance_id: str = None,
         tenant_id: str = None,
     ):
-        # The list of database names.    
-        # It is a JSON array. Each object in the array is a database name string.
         self.database_names = database_names
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The ID of the tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2402,15 +2259,14 @@
 
 
 class DeleteDatabasesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2475,23 +2331,15 @@
 
 class DeleteInstancesRequest(TeaModel):
     def __init__(
         self,
         backup_retain_mode: str = None,
         instance_ids: str = None,
     ):
-        # The backup retention strategy for cluster deletion. Valid values:  
-        # - receive_all: retains all backup sets.   
-        # - delete_all: deletes all backup sets.   
-        # - receive_last: retains the last backup set.    
-        # 
-        # > <br>Default value: delete_all.
         self.backup_retain_mode = backup_retain_mode
-        # The ID of the cluster to be deleted.   
-        # The value is a string in the JSON format.
         self.instance_ids = instance_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2515,15 +2363,14 @@
 
 
 class DeleteInstancesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2590,21 +2437,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2639,21 +2486,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **DeleteOmsOpenAPIProject**.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level
-        # The error description (new).
+        # The error code (new).
         self.message = message
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2695,35 +2542,29 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # You can call this operation to delete a data synchronization project.
         self.advice = advice
-        # The error code (old).
+        # Indicates whether the project has been deleted.
         self.code = code
-        # The time spent in processing the request, in seconds.
         self.cost = cost
-        # Indicates whether the project has been deleted.
         self.data = data
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail
-        # The error description (old).
+        # A system error occurred.
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -2830,18 +2671,18 @@
 
 class DeleteSecurityIpGroupRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         security_ip_group_name: str = None,
     ):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id
         # The name of the IP address whitelist group.    
         # It must be 2 to 32 characters in length, start with a lowercase letter, end with a lowercase letter or digit, and contain only lowercase letters, digits, and underscores (_).
+        self.instance_id = instance_id
+        # The information of the deleted IP whitelist group.
         self.security_ip_group_name = security_ip_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2866,17 +2707,15 @@
 
 class DeleteSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         security_ip_group_name: str = None,
     ):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The name of the deleted IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2901,17 +2740,16 @@
 
 class DeleteSecurityIpGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         security_ip_group: DeleteSecurityIpGroupResponseBodySecurityIpGroup = None,
     ):
-        # The request ID.
+        # Example 1
         self.request_id = request_id
-        # The information of the deleted IP whitelist group.
         self.security_ip_group = security_ip_group
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -2983,19 +2821,19 @@
 class DeleteTenantUsersRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
         users: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # Example 1
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # $.parameters[4].schema.enumValueTitles
         self.tenant_id = tenant_id
-        # A list of usernames and their respective roles.
+        # $.parameters[2].schema.example
         self.users = users
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3023,15 +2861,15 @@
 
 
 class DeleteTenantUsersResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
+        # DeleteTenantUsers
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3096,18 +2934,22 @@
 
 class DeleteTenantsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_ids: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # You can call this operation to delete one or more tenants from an OceanBase cluster.
         self.instance_id = instance_id
-        # The list of tenant IDs.   
-        # It is a JSON array. Each object in the array is a tenant name string.
+        # ```
+        # http(s)://[Endpoint]/?Action=DeleteTenants
+        # &TenantIds=["ob2mr3oae0****", "ob2mr3oae1****"]
+        # &InstanceId=ob317v4uif****\
+        # &Common request parameters
+        # ```
         self.tenant_ids = tenant_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3132,17 +2974,15 @@
 
 class DeleteTenantsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_ids: List[str] = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The list of tenant IDs.
         self.tenant_ids = tenant_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3225,54 +3065,53 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The language of the returned data.   
-        # Default value: CN for a China site and EN for an International site.
+        # The search value.
         self.accept_language = accept_language
-        # The name of the database.
+        # {
+        #   "UserName":testUser
+        # }
         self.db_name = db_name
-        # The end time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # zh-CN
         self.end_time = end_time
-        # The filter condition.   
-        # > <br> - All fields in OceanBase Database support filtering. <br> - You can write the key-value pair of a parameter in a JSON string in the JSON format to filter the parameter.
-        self.filter_condition = filter_condition
-        # The IP address of the node.
-        self.node_ip = node_ip
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
-        self.page_number = page_number
+        self.filter_condition = filter_condition
         # The number of rows to return on each page.    
         # - Maximum value: 100   
         # - Default value: 10
+        self.node_ip = node_ip
+        # desc
+        self.page_number = page_number
+        # The start time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.page_size = page_size
-        # SQLID.
+        # 1
         self.sqlid = sqlid
         # The search keyword.
         self.search_key_word = search_key_word
-        # The search parameter.
+        # The ID of the tenant.
         self.search_parameter = search_parameter
-        # The search rule.   
-        # Valid values: "=", ">", ">=", "<", and "<="
+        # Utilization above threshold
         self.search_rule = search_rule
-        # The search value.
+        # 10
         self.search_value = search_value
-        # The sorted column.
+        # The end time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.sort_column = sort_column
-        # The sorting rule.
+        # The request time, in ms.
         self.sort_order = sort_order
-        # The start time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The total count.
         self.start_time = start_time
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3367,54 +3206,53 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The language of the returned data.   
-        # Default value: CN for a China site and EN for an International site.
+        # The search value.
         self.accept_language = accept_language
-        # The name of the database.
+        # {
+        #   "UserName":testUser
+        # }
         self.db_name = db_name
-        # The end time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # zh-CN
         self.end_time = end_time
-        # The filter condition.   
-        # > <br> - All fields in OceanBase Database support filtering. <br> - You can write the key-value pair of a parameter in a JSON string in the JSON format to filter the parameter.
-        self.filter_condition_shrink = filter_condition_shrink
-        # The IP address of the node.
-        self.node_ip = node_ip
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
-        self.page_number = page_number
+        self.filter_condition_shrink = filter_condition_shrink
         # The number of rows to return on each page.    
         # - Maximum value: 100   
         # - Default value: 10
+        self.node_ip = node_ip
+        # desc
+        self.page_number = page_number
+        # The start time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.page_size = page_size
-        # SQLID.
+        # 1
         self.sqlid = sqlid
         # The search keyword.
         self.search_key_word = search_key_word
-        # The search parameter.
+        # The ID of the tenant.
         self.search_parameter = search_parameter
-        # The search rule.   
-        # Valid values: "=", ">", ">=", "<", and "<="
+        # Utilization above threshold
         self.search_rule = search_rule
-        # The search value.
+        # 10
         self.search_value = search_value
-        # The sorted column.
+        # The end time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.sort_column = sort_column
-        # The sorting rule.
+        # The request time, in ms.
         self.sort_order = sort_order
-        # The start time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The total count.
         self.start_time = start_time
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3505,37 +3343,66 @@
         request_time: float = None,
         request_time_utcstring: str = None,
         sqlid: str = None,
         sqltext: str = None,
         suggestion: str = None,
         user_name: str = None,
     ):
-        # The average CPU time, in ms.
         self.cpu_time = cpu_time
-        # The name of the database.
+        # {"name":"DescribeAnomalySQLList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":60000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeAnomalySQLList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"DbName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SearchKeyWord\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"update\"},{\"name\":\"SearchParameter\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SearchRule\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\">\"},{\"name\":\"SearchValue\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"0.01\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"NodeIp\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp19y05uq6xpacyqnlrc\"},{\"name\":\"AcceptLanguage\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"zh-CN\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"FilterCondition\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"enumValueTitles\":{\"UserName\":\"UserName\",\"Event\":\"Event\",\"SQLType\":\"SQLType\",\"ClientIp\":\"ClientIp\"},\"title\":\"\",\"description\":\"\",\"example\":\"{\\n  \\\"UserName\\\":testUser\\n}\"},{\"name\":\"SortColumn\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SortOrder\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"enumValueTitles\":{\"{     \\\"dbname\\\":test,     \\\"SQLType\\\":null\\t\\t }\":\"{     \\\"dbname\\\":test,     \\\"SQLType\\\":null\\t\\t }\"},\"title\":\"\",\"description\":\"\",\"example\":\"desc\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"AnomalySQLList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\" \",\"children\":[{\"name\":\"Key\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"DiagnosisRule\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"Suggestion\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"database1\"},{\"name\":\"RequestTimeUTCString\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2022-01-11T07:08:00Z\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"SQLId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"99E9D3BF****B486239E6C7BC79B****\"},{\"name\":\"Diagnosis\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"RequestTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.00\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"89043\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.db_name = db_name
-        # The diagnosis information.
         self.diagnosis = diagnosis
-        # The diagnostic rule.
+        # The list of suspicious SQL statements.
         self.diagnosis_rule = diagnosis_rule
-        # The number of executions.
         self.executions = executions
-        # The sequence number of the returned SQL statement.
+        # The average CPU time, in ms.
         self.key = key
-        # The request time, in ms.
         self.request_time = request_time
-        # The request time in UTC +0.
         self.request_time_utcstring = request_time_utcstring
-        # SQLID.
         self.sqlid = sqlid
-        # The SQL text.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeAnomalySQLList
+        # &TenantId=t2mr3oae0****\
+        # &StartTime=2021-06-13 15:40:43
+        # &EndTime=2021-06-13 15:40:43
+        # &DbName=testdb
+        # &SearchKeyWord=update
+        # &SearchParameter=cputime
+        # &SearchRule=>
+        # &SearchValue=0.01
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &NodeIp=i-bp19y05uq6xpacyqnlrc
+        # &AcceptLanguage=zh-CN
+        # &PageSize=10
+        # &PageNumber=1
+        # &SortColumn=cputime
+        # &SortOrder=desc
+        # &Common request parameters
+        # ```
         self.sqltext = sqltext
-        # The suggestions.
+        # {
+        #     "TotalCount": 2,
+        #     "RequestId": "473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E",
+        #     "AnomalySQLList": [
+        #         {
+        #             "Key": 1,
+        #             "DiagnosisRule": "Utilization above threshold",
+        #             "SQLText": "SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC",
+        #             "Suggestion": "Check your business scenarios, data distribution changes, request surges, and execution plan changes.",
+        #             "DbName": "database1",
+        #             "RequestTimeUTCString": "2022-01-11T07:08:00Z",
+        #             "SQLId": "99E9D3BF****B486239E6C7BC79B****",
+        #             "Diagnosis": "Total number of executions = 80199, Average CPU time = 6.8 ms, Overall CPU utilization = 87%",
+        #             "RequestTime": 1641884880000,
+        #             "Executions": 89043,
+        #             "UserName": "tester"
+        #         }
+        #     ]
+        # }
         self.suggestion = suggestion
-        # The username.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3601,19 +3468,19 @@
 class DescribeAnomalySQLListResponseBody(TeaModel):
     def __init__(
         self,
         anomaly_sqllist: List[DescribeAnomalySQLListResponseBodyAnomalySQLList] = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The list of suspicious SQL statements.
+        # The diagnostic rule.
         self.anomaly_sqllist = anomaly_sqllist
-        # The request ID.
+        # The sorting rule.
         self.request_id = request_id
-        # The total count.
+        # The SQL text.
         self.total_count = total_count
 
     def validate(self):
         if self.anomaly_sqllist:
             for k in self.anomaly_sqllist:
                 if k:
                     k.validate()
@@ -3695,23 +3562,26 @@
 class DescribeAvailableCpuResourceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         modify_type: str = None,
         tenant_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The CPU resources available.
         self.instance_id = instance_id
-        # The type of the privilege modification operation.   
-        #  Valid values:  
-        # update: updates all privileges. This is the default value.  
-        # add: adds a privilege.   
-        # delete: deletes a privilege.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeAvailableCpuResource
+        # &InstanceId=ob317v4uif****\
+        # &TenantId=ob2mr3oae0****\
+        # &ModifyType=update
+        # &Common request parameters
+        # ```
         self.modify_type = modify_type
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeAvailableCpuResource**.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3741,19 +3611,16 @@
 class DescribeAvailableCpuResourceResponseBodyData(TeaModel):
     def __init__(
         self,
         max_cpu: int = None,
         min_cpu: int = None,
         unit_num: int = None,
     ):
-        # The maximum number of CPU cores per resource unit.
         self.max_cpu = max_cpu
-        # The minimum number of CPU cores per resource unit.
         self.min_cpu = min_cpu
-        # The number of resource units in the tenant.
         self.unit_num = unit_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3782,17 +3649,15 @@
 
 class DescribeAvailableCpuResourceResponseBody(TeaModel):
     def __init__(
         self,
         data: List[DescribeAvailableCpuResourceResponseBodyData] = None,
         request_id: str = None,
     ):
-        # The CPU resources available.
         self.data = data
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -3871,22 +3736,21 @@
     def __init__(
         self,
         cpu_num: int = None,
         instance_id: str = None,
         tenant_id: str = None,
         unit_num: int = None,
     ):
-        # The number of CPU cores.
+        # The available memory size.
         self.cpu_num = cpu_num
-        # The ID of the OceanBase cluster.
+        # The ID of the region.
         self.instance_id = instance_id
         # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The number of resource distribution nodes in the tenant.   
-        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
+        # The number of resource units in the tenant.
         self.unit_num = unit_num
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3920,19 +3784,17 @@
 class DescribeAvailableMemResourceResponseBodyData(TeaModel):
     def __init__(
         self,
         max_mem: int = None,
         min_mem: int = None,
         used_mem: int = None,
     ):
-        # The maximum memory size for each resource unit, in GB.
         self.max_mem = max_mem
-        # The minimum memory size required for each resource unit, in GB.
+        # You can call this operation to query the available memory resource of an OceanBase Database tenant.
         self.min_mem = min_mem
-        # The number of resource units in the tenant.
         self.used_mem = used_mem
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3961,17 +3823,24 @@
 
 class DescribeAvailableMemResourceResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeAvailableMemResourceResponseBodyData = None,
         request_id: str = None,
     ):
-        # The available memory size.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeAvailableMemResource
+        # &InstanceId=ob317v4uif****\
+        # &TenantId=ob2mr3oae0****\
+        # &UnitNum=2
+        # &CpuNum=14
+        # &Common request parameters
+        # ```
         self.data = data
-        # The request ID.
+        # The number of CPU cores.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -4039,50 +3908,54 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCharsetRequest(TeaModel):
     def __init__(
         self,
+        series: str = None,
         tenant_mode: str = None,
     ):
-        # The tenant mode.    
-        # Valid values: Oracle and MySQL.   
-        # For more information, see [DescribeInstanceTenantModes](~~410354~~).
+        # 实例的系列  - normal（默认）：标准集群版（云盘）  - normal_ssd：标准集群版（本地盘） - history：历史库集群版。
+        self.series = series
+        # The return result of the request.
         self.tenant_mode = tenant_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.series is not None:
+            result['Series'] = self.series
         if self.tenant_mode is not None:
             result['TenantMode'] = self.tenant_mode
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Series') is not None:
+            self.series = m.get('Series')
         if m.get('TenantMode') is not None:
             self.tenant_mode = m.get('TenantMode')
         return self
 
 
 class DescribeCharsetResponseBodyCharset(TeaModel):
     def __init__(
         self,
         charset: str = None,
         collations: List[str] = None,
     ):
-        # The character set name.
+        # DescribeCharset
         self.charset = charset
-        # The collation set.
         self.collations = collations
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4107,17 +3980,22 @@
 
 class DescribeCharsetResponseBody(TeaModel):
     def __init__(
         self,
         charset: List[DescribeCharsetResponseBodyCharset] = None,
         request_id: str = None,
     ):
-        # The list of character sets.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeCharset
+        # &TenantMode=Oracle
+        # &Common request parameters
+        # ```
         self.charset = charset
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeCharset**.
         self.request_id = request_id
 
     def validate(self):
         if self.charset:
             for k in self.charset:
                 if k:
                     k.validate()
@@ -4198,31 +4076,30 @@
         database_name: str = None,
         page_number: int = None,
         page_size: int = None,
         search_key: str = None,
         tenant_id: str = None,
         with_tables: bool = None,
     ):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.database_name = database_name
-        # The number of the page to return.   
-        # - Start value: 1   
-        # - Default value: 1
+        # The return result of the request.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100.  
-        # - Default value: 10
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.page_size = page_size
-        # The search keyword.
+        # The information about the database tables.
         self.search_key = search_key
-        # The ID of the tenant.
+        # The request ID.
         self.tenant_id = tenant_id
-        # Specifies whether to return the information of tables in the database.   
-        # Default value: false.
+        # The role of the account.    
+        # In MySQL mode, a role is a database-level role. Valid values:  
+        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.  
+        # - ReadOnly: a role that has only the read-only privilege SELECT.   
+        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
+        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.with_tables = with_tables
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4262,15 +4139,14 @@
 
 
 class DescribeDatabasesResponseBodyDatabasesTables(TeaModel):
     def __init__(
         self,
         table_name: str = None,
     ):
-        # The name of the database table.
         self.table_name = table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4292,22 +4168,17 @@
 class DescribeDatabasesResponseBodyDatabasesUsers(TeaModel):
     def __init__(
         self,
         role: str = None,
         user_name: str = None,
         user_type: str = None,
     ):
-        # The role of the account.    
-        # In MySQL mode, a role is a database-level role. Valid values:  
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.  
-        # - ReadOnly: a role that has only the read-only privilege SELECT.   
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
+        # The request ID.
         self.role = role
-        # The name of the account.
+        # Example 1
         self.user_name = user_name
         # The type of the account. Valid values:  - Admin: the super administrator account. - Normal: a general account.
         self.user_type = user_type
 
     def validate(self):
         pass
 
@@ -4350,38 +4221,37 @@
         required_size: float = None,
         status: str = None,
         tables: List[DescribeDatabasesResponseBodyDatabasesTables] = None,
         tenant_id: str = None,
         users: List[DescribeDatabasesResponseBodyDatabasesUsers] = None,
     ):
         self.collation = collation
-        # The time when the database was created.
+        # Specifies whether to return the information of tables in the database.   
+        # Default value: false.
         self.create_time = create_time
-        # The actual data size, in GB.
         self.data_size = data_size
-        # The name of the database.
+        # The number of the page to return.   
+        # - Start value: 1   
+        # - Default value: 1
         self.database_name = database_name
-        # The database type.
+        # The return result of the request.
         self.db_type = db_type
-        # The description of the database.
+        # The name of the database.
         self.description = description
-        # The encoding standard of the database. Encoding standards such as utf8mb4 and GBK are supported.
-        self.encoding = encoding
-        self.instance_id = instance_id
-        # The storage space required, in GB.
-        self.required_size = required_size
         # The status of the database. Valid values:    
         # - ONLINE: The database is running.  
         # - DELETING: The database is being deleted.
+        self.encoding = encoding
+        self.instance_id = instance_id
+        self.required_size = required_size
+        # The list of databases in the tenant.
         self.status = status
-        # The information about the database tables.
         self.tables = tables
-        # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The accounts that have privileges on the database.
+        # The name of the database table.
         self.users = users
 
     def validate(self):
         if self.tables:
             for k in self.tables:
                 if k:
                     k.validate()
@@ -4468,19 +4338,18 @@
 class DescribeDatabasesResponseBody(TeaModel):
     def __init__(
         self,
         databases: List[DescribeDatabasesResponseBodyDatabases] = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The list of databases in the tenant.
+        # The ID of the tenant.
         self.databases = databases
-        # The request ID.
         self.request_id = request_id
-        # The total number of databases in the tenant.
+        # The search keyword.
         self.total_count = total_count
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -4562,23 +4431,19 @@
 class DescribeInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The size of the data disk, in GB.
         self.instance_id = instance_id
-        # The number of the page to return. 
-        # - Start value: 1  
-        # - Default value: 1
+        # The information about the storage resources of the cluster.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The server with the highest disk usage.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4608,19 +4473,23 @@
 class DescribeInstanceResponseBodyInstanceResourceCpu(TeaModel):
     def __init__(
         self,
         total_cpu: int = None,
         unit_cpu: int = None,
         used_cpu: int = None,
     ):
-        # The total number of CPU cores of the cluster.
+        # The series of the OceanBase cluster. Valid values:   
+        # - NORMAL: the high availability edition.   
+        # - BASIC: the basic edition.
         self.total_cpu = total_cpu
-        # The number of CPU cores of each replica node in the cluster.
+        # The type of the storage disk where the cluster is deployed. 
+        # 
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.unit_cpu = unit_cpu
-        # The number of CPU cores used in the cluster.
+        # Indicates whether automatic upgrade of the OBServer version is enabled.
         self.used_cpu = used_cpu
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4653,25 +4522,34 @@
         data_used_size: float = None,
         max_disk_used_ob_server: List[str] = None,
         max_disk_used_percent: float = None,
         total_disk_size: int = None,
         unit_disk_size: int = None,
         used_disk_size: int = None,
     ):
-        # The size of the data disk, in GB.
+        # The ID of the OceanBase cluster.
         self.data_used_size = data_used_size
-        # The server with the highest disk usage.
+        # The time in UTC when the cluster expires.
         self.max_disk_used_ob_server = max_disk_used_ob_server
         # The maximum disk usage, in percentage.
         self.max_disk_used_percent = max_disk_used_percent
-        # The total storage space of the cluster, in GB.
+        # The data replica distribution mode of the cluster. Valid values: 
+        # - n: indicates the single-IDC mode. 
+        # - n-n: indicates the dual-IDC mode. 
+        # - n-n-n: indicates the multi-IDC mode. 
+        # 
+        # > <br>The integer n represents the number of OBServer nodes in each IDC.
         self.total_disk_size = total_disk_size
-        # The storage space of each replica node in the cluster, in GB.
+        # The list of zones.
         self.unit_disk_size = unit_disk_size
-        # The size of used storage space of the cluster, in GB.
+        # The specifications of the cluster.  You can specify one of the following four plans:    
+        # - 8C32G: indicates 8 CPU cores and 32 GB of memory. 
+        # - 14C70G: indicates 14 CPU cores and 70 GB of memory. 
+        # - 30C180G: indicates 30 CPU cores and 180 GB of memory. 
+        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
         self.used_disk_size = used_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4712,17 +4590,17 @@
 
 class DescribeInstanceResponseBodyInstanceResourceLogDiskSize(TeaModel):
     def __init__(
         self,
         total_disk_size: int = None,
         unit_disk_size: int = None,
     ):
-        # The total log disk space of the cluster, in GB.
+        # The ID of the region.
         self.total_disk_size = total_disk_size
-        # The log disk space of each replica node in the cluster. Unit: GB.
+        # The request ID.
         self.unit_disk_size = unit_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4748,19 +4626,19 @@
 class DescribeInstanceResponseBodyInstanceResourceMemory(TeaModel):
     def __init__(
         self,
         total_memory: int = None,
         unit_memory: int = None,
         used_memory: int = None,
     ):
-        # The total memory size of the cluster, in GB.
+        # Indicates whether trusted ECS instances are used.
         self.total_memory = total_memory
-        # The memory size of each replica node in the cluster, in GB.
+        # The log disk space of each replica node in the cluster. Unit: GB.
         self.unit_memory = unit_memory
-        # The size of used memory in the cluster, in GB.
+        # The time in UTC when the cluster was created.
         self.used_memory = used_memory
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4792,23 +4670,25 @@
         self,
         cpu: DescribeInstanceResponseBodyInstanceResourceCpu = None,
         disk_size: DescribeInstanceResponseBodyInstanceResourceDiskSize = None,
         log_disk_size: DescribeInstanceResponseBodyInstanceResourceLogDiskSize = None,
         memory: DescribeInstanceResponseBodyInstanceResourceMemory = None,
         unit_count: int = None,
     ):
-        # The information about the CPU resources of the cluster.
+        # The information of the OceanBase cluster.
         self.cpu = cpu
-        # The information about the storage resources of the cluster.
+        # The number of the page to return. 
+        # - Start value: 1  
+        # - Default value: 1
         self.disk_size = disk_size
-        # The information about the log disk space of the cluster.
+        # The server with the highest disk usage.
         self.log_disk_size = log_disk_size
-        # The information about the memory resources of the cluster.
+        # The name of the OceanBase cluster.
         self.memory = memory
-        # The number of resource units in the cluster.
+        # The number of CPU cores used in the cluster.
         self.unit_count = unit_count
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -4861,112 +4741,77 @@
         auto_upgrade_ob_version: bool = None,
         available_zones: List[str] = None,
         create_time: str = None,
         data_merge_time: str = None,
         deploy_mode: str = None,
         deploy_type: str = None,
         disk_type: str = None,
+        enable_isolation_optimization: bool = None,
         enable_upgrade_log_disk: bool = None,
         expire_time: str = None,
         instance_class: str = None,
         instance_id: str = None,
         instance_name: str = None,
         instance_role: str = None,
         is_latest_ob_version: bool = None,
         is_trust_ecs: bool = None,
+        isolation_optimization: bool = None,
         maintain_time: str = None,
         node_num: str = None,
         ob_rpm_version: str = None,
         pay_type: str = None,
         resource: DescribeInstanceResponseBodyInstanceResource = None,
         series: str = None,
         status: str = None,
         version: str = None,
         zones: List[str] = None,
     ):
-        # Indicates whether automatic renewal is enabled. 
-        # 
-        # This parameter is valid only for clusters whose billing methods are set to PREPAY.
+        # The operation that you want to perform. <br>Set the value to **DescribeInstance**.
         self.auto_renewal = auto_renewal
-        # Indicates whether automatic upgrade of the OBServer version is enabled.
+        # Example 1
         self.auto_upgrade_ob_version = auto_upgrade_ob_version
-        # The list of zones.
         self.available_zones = available_zones
-        # The time in UTC when the cluster was created.
+        # Indicates whether the log disk specifications can be upgraded.
         self.create_time = create_time
-        # The time when the major compaction of cluster data is performed.
+        # The total number of CPU cores of the cluster.
         self.data_merge_time = data_merge_time
-        # The data replica distribution mode of the cluster. Valid values: 
-        # - n: indicates the single-IDC mode. 
-        # - n-n: indicates the dual-IDC mode. 
-        # - n-n-n: indicates the multi-IDC mode. 
-        # 
-        # > <br>The integer n represents the number of OBServer nodes in each IDC.
+        # Alibaba Cloud CLI
         self.deploy_mode = deploy_mode
-        # The deployment type of the cluster. Valid values:  
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.deploy_type = deploy_type
-        # The type of the storage disk where the cluster is deployed. 
-        # 
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
+        # The total storage space of the cluster, in GB.
         self.disk_type = disk_type
-        # Indicates whether the log disk specifications can be upgraded.
+        self.enable_isolation_optimization = enable_isolation_optimization
         self.enable_upgrade_log_disk = enable_upgrade_log_disk
-        # The time in UTC when the cluster expires.
+        # The information of the OceanBase cluster.
         self.expire_time = expire_time
-        # The specifications of the cluster.  You can specify one of the following four plans:    
-        # - 8C32G: indicates 8 CPU cores and 32 GB of memory. 
-        # - 14C70G: indicates 14 CPU cores and 70 GB of memory. 
-        # - 30C180G: indicates 30 CPU cores and 180 GB of memory. 
-        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
+        # The detailed information of the OBServer version.
         self.instance_class = instance_class
-        # The ID of the OceanBase cluster.
+        # The information about the log disk space of the cluster.
         self.instance_id = instance_id
-        # The name of the OceanBase cluster.
+        # Indicates whether automatic upgrade of the OBServer version is enabled.
         self.instance_name = instance_name
         self.instance_role = instance_role
-        # Indicates whether the OBServer version is the latest.
         self.is_latest_ob_version = is_latest_ob_version
-        # Indicates whether trusted ECS instances are used.
+        # The information about the CPU resources of the cluster.
         self.is_trust_ecs = is_trust_ecs
-        # The time period in UTC for the daily routine maintenance of the cluster.
+        self.isolation_optimization = isolation_optimization
+        # The time when the major compaction of cluster data is performed.
         self.maintain_time = maintain_time
         self.node_num = node_num
-        # The detailed information of the OBServer version.
         self.ob_rpm_version = ob_rpm_version
-        # The billing method of the OceanBase cluster. Valid values: 
-        # - PREPAY: the subscription billing method. 
-        # - POSTPAY: the pay-as-you-go billing method.
+        # The list of zones.
         self.pay_type = pay_type
-        # The information about cluster resources.
+        # The size of used memory in the cluster, in GB.
         self.resource = resource
-        # The series of the OceanBase cluster. Valid values:   
-        # - NORMAL: the high availability edition.   
-        # - BASIC: the basic edition.
+        # Indicates whether the OBServer version is the latest.
         self.series = series
-        # The status of the cluster. Valid values: 
-        #  - PENDING_CREATE: The cluster is being created. 
-        #  - ONLINE: The cluster is running. 
-        #  - TENANT_CREATING: The tenant is being created. 
-        # - TENANT_SPEC_MODIFYING: The tenant specifications are being modified. 
-        # - EXPANDING: Nodes are being added to the cluster to increase its capacity. 
-        # - REDUCING: Nodes are being removed from the cluster to reduce its capacity. 
-        # - SPEC_UPGRADING: The service plan is being upgraded. 
-        # - DISK_UPGRADING: The storage space is being expanded. 
-        # - WHITE_LIST_MODIFYING: The whitelist is being modified. 
-        # - PARAMETER_MODIFYING: Parameters are being modified. 
-        # - SSL_MODIFYING: The SSL certificate is being changed. 
-        # - PREPAID_EXPIRE_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to PREPAY. 
-        # - ARREARS_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to POSTPAY. 
-        # - PENDING_DELETE: The cluster is being deleted.    
-        # Generally, the cluster is in the ONLINE state.
+        # The information about cluster resources.
         self.status = status
-        # The OBServer version.
+        # You can call this operation to query the detailed information of an OceanBase cluster.
         self.version = version
         self.zones = zones
 
     def validate(self):
         if self.resource:
             self.resource.validate()
 
@@ -4988,14 +4833,16 @@
             result['DataMergeTime'] = self.data_merge_time
         if self.deploy_mode is not None:
             result['DeployMode'] = self.deploy_mode
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
         if self.disk_type is not None:
             result['DiskType'] = self.disk_type
+        if self.enable_isolation_optimization is not None:
+            result['EnableIsolationOptimization'] = self.enable_isolation_optimization
         if self.enable_upgrade_log_disk is not None:
             result['EnableUpgradeLogDisk'] = self.enable_upgrade_log_disk
         if self.expire_time is not None:
             result['ExpireTime'] = self.expire_time
         if self.instance_class is not None:
             result['InstanceClass'] = self.instance_class
         if self.instance_id is not None:
@@ -5004,14 +4851,16 @@
             result['InstanceName'] = self.instance_name
         if self.instance_role is not None:
             result['InstanceRole'] = self.instance_role
         if self.is_latest_ob_version is not None:
             result['IsLatestObVersion'] = self.is_latest_ob_version
         if self.is_trust_ecs is not None:
             result['IsTrustEcs'] = self.is_trust_ecs
+        if self.isolation_optimization is not None:
+            result['IsolationOptimization'] = self.isolation_optimization
         if self.maintain_time is not None:
             result['MaintainTime'] = self.maintain_time
         if self.node_num is not None:
             result['NodeNum'] = self.node_num
         if self.ob_rpm_version is not None:
             result['ObRpmVersion'] = self.ob_rpm_version
         if self.pay_type is not None:
@@ -5042,14 +4891,16 @@
             self.data_merge_time = m.get('DataMergeTime')
         if m.get('DeployMode') is not None:
             self.deploy_mode = m.get('DeployMode')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
         if m.get('DiskType') is not None:
             self.disk_type = m.get('DiskType')
+        if m.get('EnableIsolationOptimization') is not None:
+            self.enable_isolation_optimization = m.get('EnableIsolationOptimization')
         if m.get('EnableUpgradeLogDisk') is not None:
             self.enable_upgrade_log_disk = m.get('EnableUpgradeLogDisk')
         if m.get('ExpireTime') is not None:
             self.expire_time = m.get('ExpireTime')
         if m.get('InstanceClass') is not None:
             self.instance_class = m.get('InstanceClass')
         if m.get('InstanceId') is not None:
@@ -5058,14 +4909,16 @@
             self.instance_name = m.get('InstanceName')
         if m.get('InstanceRole') is not None:
             self.instance_role = m.get('InstanceRole')
         if m.get('IsLatestObVersion') is not None:
             self.is_latest_ob_version = m.get('IsLatestObVersion')
         if m.get('IsTrustEcs') is not None:
             self.is_trust_ecs = m.get('IsTrustEcs')
+        if m.get('IsolationOptimization') is not None:
+            self.isolation_optimization = m.get('IsolationOptimization')
         if m.get('MaintainTime') is not None:
             self.maintain_time = m.get('MaintainTime')
         if m.get('NodeNum') is not None:
             self.node_num = m.get('NodeNum')
         if m.get('ObRpmVersion') is not None:
             self.ob_rpm_version = m.get('ObRpmVersion')
         if m.get('PayType') is not None:
@@ -5086,17 +4939,17 @@
 
 class DescribeInstanceResponseBody(TeaModel):
     def __init__(
         self,
         instance: DescribeInstanceResponseBodyInstance = None,
         request_id: str = None,
     ):
-        # The information of the OceanBase cluster.
+        # The log disk space of each replica node in the cluster. Unit: GB.
         self.instance = instance
-        # The request ID.
+        # The total log disk space of the cluster, in GB.
         self.request_id = request_id
 
     def validate(self):
         if self.instance:
             self.instance.validate()
 
     def to_map(self):
@@ -5166,15 +5019,15 @@
 
 
 class DescribeInstanceCreatableZoneRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The ID of the zone.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5195,17 +5048,16 @@
 
 class DescribeInstanceCreatableZoneResponseBodyZoneList(TeaModel):
     def __init__(
         self,
         is_in_cluster: bool = None,
         zone: str = None,
     ):
-        # Indicates whether the cluster is deployed in the zone.
         self.is_in_cluster = is_in_cluster
-        # The ID of the zone.
+        # DescribeInstanceCreatableZone
         self.zone = zone
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5230,17 +5082,18 @@
 
 class DescribeInstanceCreatableZoneResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         zone_list: List[DescribeInstanceCreatableZoneResponseBodyZoneList] = None,
     ):
-        # The request ID.
+        # Indicates whether the cluster is deployed in the zone.
         self.request_id = request_id
-        # The list of zones.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceCreatableZone**.
         self.zone_list = zone_list
 
     def validate(self):
         if self.zone_list:
             for k in self.zone_list:
                 if k:
                     k.validate()
@@ -5521,17 +5374,17 @@
 
 class DescribeInstanceTagsRequest(TeaModel):
     def __init__(
         self,
         instance_ids: str = None,
         tags: str = None,
     ):
-        # The list of cluster IDs.
+        # The list of tags.
         self.instance_ids = instance_ids
-        # The tags.
+        # The returned response.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5557,19 +5410,17 @@
 class DescribeInstanceTagsResponseBodyTagResources(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
         tag: str = None,
     ):
-        # The resource ID.
+        # You can call this operation to view the tag value of a cluster.
         self.resource_id = resource_id
-        # The type of the resource.
         self.resource_type = resource_type
-        # The tag of the resource.
         self.tag = tag
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5598,17 +5449,17 @@
 
 class DescribeInstanceTagsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tag_resources: List[DescribeInstanceTagsResponseBodyTagResources] = None,
     ):
-        # The request ID.
+        # The resource ID.
         self.request_id = request_id
-        # The list of tags.
+        # The request ID.
         self.tag_resources = tag_resources
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -5684,15 +5535,16 @@
 
 
 class DescribeInstanceTenantModesRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceTenantModes**.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5713,17 +5565,15 @@
 
 class DescribeInstanceTenantModesResponseBody(TeaModel):
     def __init__(
         self,
         instance_modes: List[str] = None,
         request_id: str = None,
     ):
-        # The information of tenants.
         self.instance_modes = instance_modes
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5791,15 +5641,15 @@
 
 
 class DescribeInstanceTopologyRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The status of the node.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5830,36 +5680,30 @@
         unit_id: str = None,
         unit_memory: float = None,
         unit_status: str = None,
     ):
         # Indicates whether the migration can be canceled.   
         # This field is valid only for units that are being manually immigrated or emigrated.
         self.enable_cancel_migrate_unit = enable_cancel_migrate_unit
-        # Indicates whether migration can be performed.
+        # The return result of the request.
         self.enable_migrate_unit = enable_migrate_unit
-        # Indicates whether the migration is manually performed.
+        # The return result of the request.
         self.manual_migrate = manual_migrate
-        # The ID of the OBServer where the resource unit resides.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.node_id = node_id
-        # The number of CPU cores of the resource unit.
+        # Alibaba Cloud CLI
         self.unit_cpu = unit_cpu
-        # The data size of the unit.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceTopology**.
         self.unit_data_size = unit_data_size
-        # The ID of the resource unit.
+        # The topology of the cluster.
         self.unit_id = unit_id
-        # The memory size of the resource unit, in GB.
+        # The ID of the tenant.
         self.unit_memory = unit_memory
-        # The status of the resource unit. Valid values:    
-        # 
-        # - ONLINE: The resource unit is running.
-        # - IMMIGRATING: The resource unit is being immigrated.
-        # - EMIGRATING: The resource unit is being emigrated.
-        # - CANCEL_EMIGRATING: Resource node immigration is being canceled.
-        # - CANCEL_EMIGRATING: Resource node emigration is being canceled.
-        # - DELETING: The resource unit is being deleted.
+        # You can call this operation to query the topology of an OceanBase cluster.
         self.unit_status = unit_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5914,23 +5758,21 @@
     def __init__(
         self,
         is_primary_tenant_zone: str = None,
         tenant_zone_id: str = None,
         tenant_zone_role: str = None,
         units: List[DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZonesUnits] = None,
     ):
-        # Indicates whether the zone is the primary zone.
+        # The maximum disk usage, in percentage.
         self.is_primary_tenant_zone = is_primary_tenant_zone
-        # The ID of the zone.
+        # The server with the highest disk usage.
         self.tenant_zone_id = tenant_zone_id
-        # The role to access the zone. Valid values:   
-        #  - ReadWrite: a role that has the read and write privileges.
-        #  - ReadOnly: a role that has only the read-only privilege.
+        # The information of zones.
         self.tenant_zone_role = tenant_zone_role
-        # The information about resource units.
+        # The information about the storage resources.
         self.units = units
 
     def validate(self):
         if self.units:
             for k in self.units:
                 if k:
                     k.validate()
@@ -5979,47 +5821,33 @@
         tenant_memory: float = None,
         tenant_mode: str = None,
         tenant_name: str = None,
         tenant_status: str = None,
         tenant_unit_num: int = None,
         tenant_zones: List[DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZones] = None,
     ):
-        # The deployment type of the primary zone.
+        # The server with the highest disk usage.
         self.primary_zone_deploy_type = primary_zone_deploy_type
-        # The number of CPU cores of the tenant.
+        # The information about the memory resources of the node.
         self.tenant_cpu = tenant_cpu
-        # The deployment type of the tenant.   
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The name of the tenant.
         self.tenant_deploy_type = tenant_deploy_type
-        # The ID of the tenant.
+        # The size of used memory of the node, in GB.
         self.tenant_id = tenant_id
-        # The memory size of the tenant, in GB.
+        # The total storage space of the node, in GB.
         self.tenant_memory = tenant_memory
-        # The tenant mode. Valid values:   
-        # - Oracle   
-        # - MySQL
+        # The size of used storage space of the node, in GB.
         self.tenant_mode = tenant_mode
-        # The name of the tenant.
+        # The total memory size of the node, in GB.
         self.tenant_name = tenant_name
-        # The status of the tenant.   
-        # - PENDING_CREATE: The tenant is being created.   
-        # - RESTORE: The tenant is being recovered.   
-        # - ONLINE: The tenant is running.   
-        # - SPEC_MODIFYING: The specification of the tenant is being modified.   
-        # - ALLOCATING_INTERNET_ADDRESS: An Internet address is being allocated.   
-        # - PENDING_OFFLINE_INTERNET_ADDRESS: The Internet address is being disabled.   
-        # - PRIMARY_ZONE_MODIFYING: The tenant is switching to a new primary zone.   
-        # - PARAMETER_MODIFYING: Parameters are being modified.   
-        # - WHITE_LIST_MODIFYING: The whitelist is being modified.
+        # The size of used memory of the node, in GB.
         self.tenant_status = tenant_status
-        # The number of resource units in the tenant.
+        # The number of CPU cores of the tenant.
         self.tenant_unit_num = tenant_unit_num
-        # The zone information of the tenant.
+        # The information about the storage resources of the node.
         self.tenant_zones = tenant_zones
 
     def validate(self):
         if self.tenant_zones:
             for k in self.tenant_zones:
                 if k:
                     k.validate()
@@ -6084,17 +5912,17 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceCpu(TeaModel):
     def __init__(
         self,
         total_cpu: int = None,
         used_cpu: float = None,
     ):
-        # The total number of CPU cores for the node.
+        # The size of used storage space of the node, in GB.
         self.total_cpu = total_cpu
-        # The number of CPU cores used by the node.
+        # Indicates whether migration can be performed.
         self.used_cpu = used_cpu
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6119,17 +5947,26 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceDiskSize(TeaModel):
     def __init__(
         self,
         total_disk_size: float = None,
         used_disk_size: float = None,
     ):
-        # The total storage space of the node, in GB.
+        # The deployment type of the primary zone.
         self.total_disk_size = total_disk_size
-        # The size of used storage space of the node, in GB.
+        # The status of the tenant.   
+        # - PENDING_CREATE: The tenant is being created.   
+        # - RESTORE: The tenant is being recovered.   
+        # - ONLINE: The tenant is running.   
+        # - SPEC_MODIFYING: The specification of the tenant is being modified.   
+        # - ALLOCATING_INTERNET_ADDRESS: An Internet address is being allocated.   
+        # - PENDING_OFFLINE_INTERNET_ADDRESS: The Internet address is being disabled.   
+        # - PRIMARY_ZONE_MODIFYING: The tenant is switching to a new primary zone.   
+        # - PARAMETER_MODIFYING: Parameters are being modified.   
+        # - WHITE_LIST_MODIFYING: The whitelist is being modified.
         self.used_disk_size = used_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6154,17 +5991,17 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory(TeaModel):
     def __init__(
         self,
         total_memory: int = None,
         used_memory: float = None,
     ):
-        # The total memory size of the node, in GB.
+        # The ID of the replica node.
         self.total_memory = total_memory
-        # The size of used memory of the node, in GB.
+        # The information of node resources.
         self.used_memory = used_memory
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6190,19 +6027,21 @@
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResource(TeaModel):
     def __init__(
         self,
         cpu: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceCpu = None,
         disk_size: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceDiskSize = None,
         memory: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory = None,
     ):
-        # The information about the CPU resources of the node.
+        # The memory size of the tenant, in GB.
         self.cpu = cpu
-        # The information about the storage resources of the node.
+        # The information about the CPU resources of the node.
         self.disk_size = disk_size
-        # The information about the memory resources of the node.
+        # The role to access the zone. Valid values:   
+        #  - ReadWrite: a role that has the read and write privileges.
+        #  - ReadOnly: a role that has only the read-only privilege.
         self.memory = memory
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -6241,21 +6080,21 @@
     def __init__(
         self,
         node_copy_id: int = None,
         node_id: str = None,
         node_resource: List[DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResource] = None,
         node_status: str = None,
     ):
-        # The ID of the replica node.
+        # The information of zones.
         self.node_copy_id = node_copy_id
-        # The ID of the node.
+        # The ID of the resource unit.
         self.node_id = node_id
-        # The information of node resources.
+        # The ID of the node.
         self.node_resource = node_resource
-        # The status of the node.
+        # The ID of the OBServer where the resource unit resides.
         self.node_status = node_status
 
     def validate(self):
         if self.node_resource:
             for k in self.node_resource:
                 if k:
                     k.validate()
@@ -6296,17 +6135,16 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize(TeaModel):
     def __init__(
         self,
         max_disk_used_ob_server: List[str] = None,
         max_disk_used_percent: float = None,
     ):
-        # The server with the highest disk usage.
         self.max_disk_used_ob_server = max_disk_used_ob_server
-        # The maximum disk usage, in percentage.
+        # DescribeInstanceTopology
         self.max_disk_used_percent = max_disk_used_percent
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6330,15 +6168,14 @@
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResource(TeaModel):
     def __init__(
         self,
         disk_size: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize = None,
     ):
-        # The information about the storage resources of the node.
         self.disk_size = disk_size
 
     def validate(self):
         if self.disk_size:
             self.disk_size.validate()
 
     def to_map(self):
@@ -6364,23 +6201,23 @@
         self,
         nodes: List[DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodes] = None,
         region: str = None,
         zone_disk: str = None,
         zone_id: str = None,
         zone_resource: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResource = None,
     ):
-        # The information of the nodes.
-        self.nodes = nodes
         # The ID of the region.
+        self.nodes = nodes
+        # The zone information of the cluster.
         self.region = region
-        # The storage capacity of the zone.
+        # The information about the memory resources of the node.
         self.zone_disk = zone_disk
-        # The ID of the zone.
+        # The information of the tenant.
         self.zone_id = zone_id
-        # The information of zones.
+        # Example 1
         self.zone_resource = zone_resource
 
     def validate(self):
         if self.nodes:
             for k in self.nodes:
                 if k:
                     k.validate()
@@ -6428,17 +6265,17 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopology(TeaModel):
     def __init__(
         self,
         tenants: List[DescribeInstanceTopologyResponseBodyInstanceTopologyTenants] = None,
         zones: List[DescribeInstanceTopologyResponseBodyInstanceTopologyZones] = None,
     ):
-        # The information of the tenant.
+        # The total number of CPU cores for the node.
         self.tenants = tenants
-        # The zone information of the cluster.
+        # The information about resource units.
         self.zones = zones
 
     def validate(self):
         if self.tenants:
             for k in self.tenants:
                 if k:
                     k.validate()
@@ -6480,17 +6317,17 @@
 
 class DescribeInstanceTopologyResponseBody(TeaModel):
     def __init__(
         self,
         instance_topology: DescribeInstanceTopologyResponseBodyInstanceTopology = None,
         request_id: str = None,
     ):
-        # The topology of the cluster.
+        # The number of CPU cores used by the node.
         self.instance_topology = instance_topology
-        # The request ID.
+        # The information about the CPU resources of the node.
         self.request_id = request_id
 
     def validate(self):
         if self.instance_topology:
             self.instance_topology.validate()
 
     def to_map(self):
@@ -6565,32 +6402,25 @@
         instance_id: str = None,
         instance_name: str = None,
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
         search_key: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The number of CPU cores used in the cluster.
         self.instance_id = instance_id
-        # The name of the OceanBase cluster.    
-        # It must be 1 to 20 characters in length.   
-        # If this parameter is not specified, the value is the instance ID of the cluster by default.
+        # The size of used memory in the cluster, in GB.
         self.instance_name = instance_name
-        # The number of the page to return.    
-        # 
-        # - Start value: 1 
-        # - Default value: 1
+        # The total memory size of the cluster, in GB.
         self.page_number = page_number
-        # The number of rows to return on each page.    
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The information about the memory resources of the cluster.
         self.page_size = page_size
-        # The ID of the resource group.
+        # The number of CPU cores of each replica node in the cluster.
         self.resource_group_id = resource_group_id
-        # The search keyword.
+        # The memory size of each replica node in the cluster, in GB.
         self.search_key = search_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6632,19 +6462,25 @@
 class DescribeInstancesResponseBodyInstancesResourceCpu(TeaModel):
     def __init__(
         self,
         total_cpu: int = None,
         unit_cpu: int = None,
         used_cpu: int = None,
     ):
-        # The total number of CPU cores of the cluster.
+        # The name of the OceanBase cluster.    
+        # It must be 1 to 20 characters in length.   
+        # If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.total_cpu = total_cpu
-        # The number of CPU cores of each replica node in the cluster.
+        # The data replica distribution mode of the cluster. Valid values:    
+        # 
+        # - n: indicates the single-IDC mode.  
+        # - n-n: indicates the dual-IDC mode.  
+        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
         self.unit_cpu = unit_cpu
-        # The number of CPU cores used in the cluster.
+        # The search keyword.
         self.used_cpu = used_cpu
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6674,19 +6510,19 @@
 class DescribeInstancesResponseBodyInstancesResourceDiskSize(TeaModel):
     def __init__(
         self,
         total_disk_size: int = None,
         unit_disk_size: int = None,
         used_disk_size: int = None,
     ):
-        # The total storage space of the cluster, in GB.
+        # The request ID.
         self.total_disk_size = total_disk_size
-        # The storage space of each replica node in the cluster, in GB.
+        # Example 1
         self.unit_disk_size = unit_disk_size
-        # The size of used storage space of the cluster, in GB.
+        # $.parameters[7].schema.example
         self.used_disk_size = used_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6716,17 +6552,17 @@
 class DescribeInstancesResponseBodyInstancesResourceMemory(TeaModel):
     def __init__(
         self,
         total_memory: int = None,
         unit_memory: int = None,
         used_memory: int = None,
     ):
-        # The total memory size of the cluster, in GB.
+        # The number of CPU cores of the cluster.
         self.total_memory = total_memory
-        # The memory size of each replica node in the cluster, in GB.
+        # The size of used storage space of the cluster, in GB.
         self.unit_memory = unit_memory
         # The size of used memory in the cluster, in GB.
         self.used_memory = used_memory
 
     def validate(self):
         pass
 
@@ -6759,21 +6595,35 @@
     def __init__(
         self,
         cpu: DescribeInstancesResponseBodyInstancesResourceCpu = None,
         disk_size: DescribeInstancesResponseBodyInstancesResourceDiskSize = None,
         memory: DescribeInstancesResponseBodyInstancesResourceMemory = None,
         unit_count: int = None,
     ):
-        # The information about the CPU resources of the cluster.
+        # Indicates whether new nodes can be added.
         self.cpu = cpu
-        # The information about the storage resources of the cluster.
+        # The time elapsed since the expiration of the cluster, in seconds.
         self.disk_size = disk_size
-        # The information about the memory resources of the cluster.
+        # The status of the cluster. Valid values:   
+        # - PENDING_CREATE: The cluster is being created.  
+        # - ONLINE: The cluster is running.  
+        # - TENANT_CREATING: The tenant is being created.  
+        # - TENANT_SPEC_MODIFYING: The tenant specifications are being modified.  
+        # - EXPANDING: Nodes are being added to the cluster to increase its capacity.  
+        # - REDUCING: Nodes are being removed from the cluster to reduce its capacity.  
+        # - SPEC_UPGRADING: The service plan is being upgraded.  
+        # - DISK_UPGRADING: The storage space is being expanded.  
+        # - WHITE_LIST_MODIFYING: The whitelist is being modified.  
+        # - PARAMETER_MODIFYING: Parameters are being modified.  
+        # - SSL_MODIFYING: The SSL certificate is being changed.  
+        # - PREPAID_EXPIRE_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to PREPAY.  
+        # - ARREARS_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to POSTPAY.  
+        # - PENDING_DELETE: The cluster is being deleted.   
+        # Generally, the cluster is in the ONLINE state.
         self.memory = memory
-        # The number of resource units in the cluster.
         self.unit_count = unit_count
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -6839,98 +6689,73 @@
         security_ips: List[str] = None,
         series: str = None,
         state: str = None,
         used_disk_size: int = None,
         version: str = None,
         vpc_id: str = None,
     ):
-        # The information about the zone in which the cluster is deployed.
+        # The time in UTC when the cluster expires.
         self.available_zones = available_zones
+        # The storage space of each replica node in the cluster, in GB.
+        self.commodity_code = commodity_code
         # The product code of the OceanBase cluster.   
         # - oceanbase_oceanbasepre_public_cn: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in a China site.  
         # - oceanbase_oceanbasepost_public_cn: indicates an OceanBase cluster that is billed based on the pay-as-you-go plan and that is deployed in a China site.  
         # - oceanbase_obpre_public_intl: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in an international site.
-        self.commodity_code = commodity_code
-        # The number of CPU cores of the cluster.
         self.cpu = cpu
-        # The time in UTC when the cluster was created.
+        # The number of OceanBase clusters queried.
         self.create_time = create_time
-        # The data replica distribution mode of the cluster. Valid values:    
-        # 
-        # - n: indicates the single-IDC mode.  
-        # - n-n: indicates the dual-IDC mode.  
-        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
+        # The request ID.
         self.deploy_mode = deploy_mode
-        # The deployment type of the cluster. Valid values:   
-        # - multiple: multi-IDC deployment  
-        # - single: single-IDC deployment  
-        # - dual: dual-IDC deployment
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.deploy_type = deploy_type
-        # The size of the storage space, in GB.
+        # The information about the memory resources of the cluster.
         self.disk_size = disk_size
-        # The type of the storage disk where the cluster is deployed.   
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
+        # The number of CPU cores used in the cluster.
         self.disk_type = disk_type
-        # Indicates whether new nodes can be added.
+        # The ID of the OceanBase cluster.
         self.enable_upgrade_nodes = enable_upgrade_nodes
-        # The time elapsed since the expiration of the cluster, in seconds.
+        # The whitelist information of the cluster.
         self.expire_seconds = expire_seconds
-        # The time in UTC when the cluster expires.
+        # The information about the storage resources of the cluster.
         self.expire_time = expire_time
-        # The specifications of the cluster.  You can specify one of the following four plans:  
-        # - 8C32G: indicates 8 CPU cores and 32 GB of memory.  
-        # - 14C70G: indicates 14 CPU cores and 70 GB of memory.  
-        # - 30C180G: indicates 30 CPU cores and 180 GB of memory.  
-        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
+        # The instance type.
         self.instance_class = instance_class
-        # The ID of the OceanBase cluster.
+        # The total storage space of the cluster, in GB.
         self.instance_id = instance_id
-        # The name of the OceanBase cluster.
+        # The return result of the request.
         self.instance_name = instance_name
         self.instance_role = instance_role
-        # The instance type.
+        # You can call this operation to obtain the list of OceanBase clusters.
         self.instance_type = instance_type
-        # The time period in UTC for the daily routine maintenance of the cluster.
+        # The return result of the request.
         self.maintain_time = maintain_time
-        # The memory size of the instance, in GB.
+        # The information about the CPU resources of the cluster.
         self.mem = mem
-        # The billing method for the OceanBase cluster. Valid values:  
-        # - PREPAY: the subscription billing method.  
-        # - POSTPAY: the pay-as-you-go billing method.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.pay_type = pay_type
-        # The information about cluster resources.
+        # The type of the storage disk where the cluster is deployed.   
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.resource = resource
-        # The ID of the resource group.
+        # The number of OceanBase clusters queried.
         self.resource_group_id = resource_group_id
-        # The whitelist information of the cluster.
+        # The number of the page to return.    
+        # 
+        # - Start value: 1 
+        # - Default value: 1
         self.security_ips = security_ips
-        # The series of the OceanBase cluster. Valid values:   
-        # - NORMAL: the high availability edition.   
-        # - BASIC: the basic edition.
+        # The billing method for the OceanBase cluster. Valid values:  
+        # - PREPAY: the subscription billing method.  
+        # - POSTPAY: the pay-as-you-go billing method.
         self.series = series
-        # The status of the cluster. Valid values:   
-        # - PENDING_CREATE: The cluster is being created.  
-        # - ONLINE: The cluster is running.  
-        # - TENANT_CREATING: The tenant is being created.  
-        # - TENANT_SPEC_MODIFYING: The tenant specifications are being modified.  
-        # - EXPANDING: Nodes are being added to the cluster to increase its capacity.  
-        # - REDUCING: Nodes are being removed from the cluster to reduce its capacity.  
-        # - SPEC_UPGRADING: The service plan is being upgraded.  
-        # - DISK_UPGRADING: The storage space is being expanded.  
-        # - WHITE_LIST_MODIFYING: The whitelist is being modified.  
-        # - PARAMETER_MODIFYING: Parameters are being modified.  
-        # - SSL_MODIFYING: The SSL certificate is being changed.  
-        # - PREPAID_EXPIRE_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to PREPAY.  
-        # - ARREARS_CLOSED: The payment is overdue. This parameter is valid for a cluster whose billing method is set to POSTPAY.  
-        # - PENDING_DELETE: The cluster is being deleted.   
-        # Generally, the cluster is in the ONLINE state.
+        # The number of resource units in the cluster.
         self.state = state
-        # The size of used storage space of the cluster, in GB.
+        # The number of resource units in the cluster.
         self.used_disk_size = used_disk_size
-        # The OBServer version.
+        # The total number of CPU cores of the cluster.
         self.version = version
         # vpcId
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.resource:
             self.resource.validate()
@@ -7060,19 +6885,17 @@
 class DescribeInstancesResponseBody(TeaModel):
     def __init__(
         self,
         instances: List[DescribeInstancesResponseBodyInstances] = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information of the OceanBase cluster.
+        # The total storage space of the cluster, in GB.
         self.instances = instances
-        # The request ID.
         self.request_id = request_id
-        # The number of OceanBase clusters queried.
         self.total_count = total_count
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -7160,38 +6983,31 @@
         node_id_list: str = None,
         node_name: str = None,
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The end time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # $.parameters[7].schema.description
         self.end_time = end_time
-        # The ID of the OceanBase cluster.
+        # The list of nodes.
         self.instance_id = instance_id
-        # The monitoring metrics.     
-        # For more information about supported metrics, see [Node statistics](~~212099~~).
+        # $.parameters[7].schema.enumValueTitles
         self.metrics = metrics
-        # The list of nodes.
+        # $.parameters[10].schema.description
         self.node_id_list = node_id_list
-        # The name of the node.
+        # $.parameters[8].schema.example
         self.node_name = node_name
-        # The number of the page to return.   
-        # - Start value: 1   
-        # - Default value: 1
+        # $.parameters[6].schema.description
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The ID of the tenant.
         self.page_size = page_size
-        # The start time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # $.parameters[9].schema.example
         self.start_time = start_time
-        # The ID of the tenant.
+        # $.parameters[6].schema.enumValueTitles
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7245,19 +7061,30 @@
 class DescribeNodeMetricsResponseBody(TeaModel):
     def __init__(
         self,
         node_metrics: str = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The metrics of the node.
         self.node_metrics = node_metrics
-        # The request ID.
+        # You can call this operation to query the detailed metrics information of an OceanBase Database node.
         self.request_id = request_id
-        # The total count.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeNodeMetrics
+        # &InstanceId=ob317v4uif****\
+        # &PageSize=10
+        # &PageNumber=1
+        # &TenantId=ob2mr3oae0****\
+        # &StartTime=2021-06-13 15:40:43
+        # &EndTime=2021-09-13 15:40:43
+        # &Metrics=tps
+        # &NodeName=i-bp16niirq4zdmgvm****\
+        # &NodeIdList=["i-bp19y05uq6xpacyqnlrc","i-bp1blcr3htr3g3u2vqvu","i-bp1392ikhayhr3hi4fli"]
+        # &Common request parameters
+        # ```
         self.total_count = total_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8747,21 +8574,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # The read RT baseline of the source data source.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # The read/write RPS baseline of the destination data source.
         self.page_size = page_size
-        # The project ID.
+        # The read/write RT baseline of the destination data source.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The read RT baseline of the source data source.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8796,21 +8623,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code.
+        # The suggestions (old).
         self.code = code
-        # Valid values: CRITICAL, ERROR, and WARN.
+        # Contact the administrator.
         self.level = level
-        # The error message.
+        # A sub-status that indicates whether the checker has completed full verification.
         self.message = message
-        # The suggestions.
+        # The amount of data migrated.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8846,23 +8673,23 @@
         self,
         error_code: str = None,
         error_details: List[DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfoErrorDetails] = None,
         error_msg: str = None,
         error_param: Dict[str, str] = None,
         failed_time: str = None,
     ):
-        # The error code, such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
+        # The job ID.
         self.error_code = error_code
-        # The error details.
+        # Schema migration
         self.error_details = error_details
-        # The error message.
+        # The resource deployment ID.
         self.error_msg = error_msg
-        # The error related parameters.
+        # The error code (new).
         self.error_param = error_param
-        # The time when the error occurred.
+        # The additional information. The value is a JSON string.
         self.failed_time = failed_time
 
     def validate(self):
         if self.error_details:
             for k in self.error_details:
                 if k:
                     k.validate()
@@ -8909,21 +8736,21 @@
     def __init__(
         self,
         estimated_remaining_time_of_sec: int = None,
         estimated_total_count: int = None,
         finished_count: int = None,
         progress: int = None,
     ):
-        # The estimated maximum time remained, in seconds.
+        # A sub-status that indicates whether this step is skipped.
         self.estimated_remaining_time_of_sec = estimated_remaining_time_of_sec
-        # The estimated amount of data to migrate.
+        # The read RPS baseline of the source data source.
         self.estimated_total_count = estimated_total_count
-        # The amount of data migrated.
+        # The read/write RT per record of the destination data source, in ms.
         self.finished_count = finished_count
-        # finishedCount / estimatedTotalCount
+        # The business data returned.
         self.progress = progress
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8976,57 +8803,57 @@
         src_iops_ref: int = None,
         src_rps: int = None,
         src_rps_ref: int = None,
         src_rt: int = None,
         src_rt_ref: int = None,
         validated: bool = None,
     ):
-        # The estimated total number of rows.
+        # The total count, which takes effect in a pagination query.
         self.capacity = capacity
-        # The checkpoint. The value is a unix timestamp in seconds.
+        # The operation that you want to perform. Set the value to **DescribeOmsOpenAPIProjectSteps**.
         self.checkpoint = checkpoint
-        # The full synchronization progress.
+        # The error code, such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
         self.connector_full_progress_overview = connector_full_progress_overview
-        # The resource deployment ID.
+        # The page size, which takes effect in a pagination query.
         self.deploy_id = deploy_id
-        # The read/write throughput of the destination data source, in bytes per second.
+        # The error description (old).
         self.dst_iops = dst_iops
-        # The read/write RPS of the destination data source.
+        # The estimated amount of data to migrate.
         self.dst_rps = dst_rps
-        # The read/write RPS baseline of the destination data source.
+        # The step progress.
         self.dst_rps_ref = dst_rps_ref
-        # The read/write RT per record of the destination data source, in ms.
+        # The read requests per second (RPS) of the source data source.
         self.dst_rt = dst_rt
-        # The read/write RT baseline of the destination data source.
+        # A system error occurred.
         self.dst_rt_ref = dst_rt_ref
-        # The checkpoint collection time. The value is a unix timestamp in seconds.
+        # The full synchronization progress.
         self.gmt = gmt
-        # The amount of inconsistent data found during full verification.
+        # The read/write throughput of the destination data source, in bytes per second.
         self.inconsistencies = inconsistencies
-        # The checkpoint in incremental synchronization. The value is a unix timestamp in seconds.
+        # The read throughput of the source data source, in bytes per second.
         self.incr_timestamp_checkpoint = incr_timestamp_checkpoint
-        # The job ID.
+        # The error code (old).
         self.job_id = job_id
-        # The number of migrated rows.
+        # The error related parameters.
         self.processed_records = processed_records
-        # A sub-status that indicates whether this step is skipped.
+        # The time spent in processing the request, in seconds.
         self.skipped = skipped
-        # The read throughput of the source data source, in bytes per second.
+        # finishedCount / estimatedTotalCount
         self.src_iops = src_iops
-        # The read throughput baseline of the source data source.
+        # The end time, in the format of "2020-05-22T17:04:18".
         self.src_iops_ref = src_iops_ref
-        # The read requests per second (RPS) of the source data source.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.src_rps = src_rps
-        # The read RPS baseline of the source data source.
+        # The checkpoint. The value is a unix timestamp in seconds.
         self.src_rps_ref = src_rps_ref
-        # The read response time (RT) per record of the source data source, in ms.
+        # The error code.
         self.src_rt = src_rt
-        # The read RT baseline of the source data source.
+        # The checkpoint collection time. The value is a unix timestamp in seconds.
         self.src_rt_ref = src_rt_ref
-        # A sub-status that indicates whether the checker has completed full verification.
+        # The read/write RPS of the destination data source.
         self.validated = validated
 
     def validate(self):
         if self.connector_full_progress_overview:
             self.connector_full_progress_overview.validate()
 
     def to_map(self):
@@ -9142,35 +8969,35 @@
         step_description: str = None,
         step_info: DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfo = None,
         step_name: str = None,
         step_order: int = None,
         step_progress: int = None,
         step_status: str = None,
     ):
-        # The estimated time remained.
+        # The request ID.
         self.estimated_remaining_seconds = estimated_remaining_seconds
-        # The additional information. The value is a JSON string.
+        # A system error occurred.
         self.extra_info = extra_info
-        # The end time, in the format of "2020-05-22T17:04:18".
+        # $.parameters[3].schema.example
         self.finish_time = finish_time
-        # Indicates whether the current step must be confirmed by the user, rather than scheduled in the backend.
+        # $.parameters[5].schema.description
         self.interactive = interactive
-        # The start time, in the format of "2020-05-22T17:04:18".
+        # The error details.
         self.start_time = start_time
-        # The description of the step, for example, schema migration, full migration, full verification, incremental log pull, incremental synchronization, or incremental verification.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.step_description = step_description
-        # The step details. The value is a JSON string.
+        # The error related parameters.
         self.step_info = step_info
-        # The step name. Valid values: struct_migration, full_migration, full_validation, incr_log_pull, incr_sync/incr_validation, PRE_CHECK, PREPARE, STRUCT_MIGRATION, INDEX_MIGRATION, STRUCT_SYNC, FULL_MIGRATION, APP_SWITCH, REVERSE_INCR_SYNC, FULL_VALIDATION, INCR_LOG_PULL, INCR_SYNC, INCR_VALIDATION, SYNC_PREPARE, SYNC_INCR_LOG_PULL, CONNECTOR_FULL_SYNC, or CONNECTOR_INCR_SYNC.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.step_name = step_name
-        # The sequence of steps.
+        # DescribeOmsOpenAPIProjectSteps
         self.step_order = step_order
-        # The step progress.
+        # cn-hangzhou
         self.step_progress = step_progress
-        # The step status. Valid values: INIT, RUNNING, FAILED, FINISHED, SUSPEND, and MONITORING. The value MONITORING indicates the continuous monitoring of incremental synchronization and incremental verification.
+        # Indicates whether the call is successful.
         self.step_status = step_status
 
     def validate(self):
         if self.extra_info:
             self.extra_info.validate()
         if self.step_info:
             self.step_info.validate()
@@ -9238,21 +9065,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The error details.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # Valid values: CRITICAL, ERROR, and WARN.
         self.level = level
-        # The error description (new).
+        # A system error occurred.
         self.message = message
-        # The suggestions (new).
+        # Contact the administrator.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9294,35 +9121,35 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # The error related parameters.
         self.advice = advice
-        # The error code (old).
+        # The error code (old), such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
         self.code = code
-        # The time spent in processing the request, in seconds.
+        # The step end time, in the format of "yyyy-MM-ddTHH:mm:ss".
         self.cost = cost
-        # The business data returned.
+        # Indicates whether the current step must be confirmed by the user, rather than scheduled in the backend.
         self.data = data
-        # The error details.
+        # The step details. The value is a JSON string.
         self.error_detail = error_detail
-        # The error description (old).
+        # A system error occurred.
         self.message = message
-        # The page number, which takes effect in a pagination query.
+        # The additional information. The value is a JSON string.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # The step start time, in the format of "yyyy-MM-ddTHH:mm:ss".
         self.page_size = page_size
-        # The request ID.
+        # The time when the error occurred.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The read throughput baseline of the source data source.
         self.success = success
-        # The total count, which takes effect in a pagination query.
+        # The estimated remaining time. This parameter takes effect in full synchronization.
         self.total_count = total_count
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -9442,27 +9269,27 @@
         database_name: str = None,
         instance_id: str = None,
         is_concurrent_limit: bool = None,
         sqlid: str = None,
         table_name: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.
-        self.database_name = database_name
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id
         # - When the value is set to True, the throttling information in the database is queried based on the SQL ID.   
         # - When the value is set to False, the bound index or execution plan in the database is queried based on the SQL ID.
-        self.is_concurrent_limit = is_concurrent_limit
+        self.database_name = database_name
         # SQLID.
+        self.instance_id = instance_id
+        # The ID of the tenant.
+        self.is_concurrent_limit = is_concurrent_limit
+        # false
         self.sqlid = sqlid
+        # The name of the database.
+        self.table_name = table_name
         # The name of the tenant.    
         # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_). It cannot be set to SYS.
-        self.table_name = table_name
-        # The ID of the tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9504,23 +9331,24 @@
 class DescribeOutlineBindingResponseBodyOutlineBinding(TeaModel):
     def __init__(
         self,
         bind_index: str = None,
         bind_plan: str = None,
         max_concurrent: int = None,
         outline_id: int = None,
+        table_name: str = None,
     ):
-        # The bound index.
         self.bind_index = bind_index
-        # The bound plan.
+        # You can call this operation to query the outline binding information or throttling information of an SQL statement in the database based on an SQLID.
         self.bind_plan = bind_plan
-        # The maximum number of concurrent tasks.
         self.max_concurrent = max_concurrent
-        # OutlineID.
+        # {"name":"DescribeOutlineBinding","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeOutlineBinding\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"TableName\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"pay_online\"},{\"name\":\"DatabaseName\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"IsConcurrentLimit\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Boolean\",\"title\":\"\",\"description\":\"\",\"example\":\"false\"},{\"name\":\"InstanceId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"ob317v4uif****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"OutlineBinding\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"children\":[{\"name\":\"BindPlan\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"PHY_TABLE_SCAN | bmsql_order_line | 40 ******\"},{\"name\":\"OutlineId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"OutlineID\",\"description\":\"OutlineID。\",\"example\":\"-1\"},{\"name\":\"BindIndex\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"PRIMARY\"},{\"name\":\"MaxConcurrent\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"}],\"title\":\"\",\"description\":\"\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.outline_id = outline_id
+        # 表名称
+        self.table_name = table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -9531,38 +9359,50 @@
             result['BindIndex'] = self.bind_index
         if self.bind_plan is not None:
             result['BindPlan'] = self.bind_plan
         if self.max_concurrent is not None:
             result['MaxConcurrent'] = self.max_concurrent
         if self.outline_id is not None:
             result['OutlineId'] = self.outline_id
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BindIndex') is not None:
             self.bind_index = m.get('BindIndex')
         if m.get('BindPlan') is not None:
             self.bind_plan = m.get('BindPlan')
         if m.get('MaxConcurrent') is not None:
             self.max_concurrent = m.get('MaxConcurrent')
         if m.get('OutlineId') is not None:
             self.outline_id = m.get('OutlineId')
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
         return self
 
 
 class DescribeOutlineBindingResponseBody(TeaModel):
     def __init__(
         self,
         outline_binding: DescribeOutlineBindingResponseBodyOutlineBinding = None,
         request_id: str = None,
     ):
-        # The binding information.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeOutlineBinding
+        # &TenantId=t2mr3oae0****\
+        # &TableName=pay_online
+        # &DatabaseName=testdb
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &IsConcurrentLimit=false
+        # &InstanceId=ob317v4uif****\
+        # &Common request parameters
+        # ```
         self.outline_binding = outline_binding
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.outline_binding:
             self.outline_binding.validate()
 
     def to_map(self):
@@ -9634,21 +9474,19 @@
 class DescribeParametersRequest(TeaModel):
     def __init__(
         self,
         dimension: str = None,
         dimension_value: str = None,
         instance_id: str = None,
     ):
-        # The type of the parameter.    
-        # Valid values: CLUSTER and TENANT.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.dimension = dimension
-        # The resource ID of the parameter type.   
-        # You can leave this parameter unspecified when you call this operation to query cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # Alibaba Cloud CLI
         self.dimension_value = dimension_value
-        # The ID of the OceanBase cluster.
+        # 498529
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9680,39 +9518,60 @@
         self,
         acceptable_value: List[str] = None,
         current_value: str = None,
         default_value: str = None,
         description: str = None,
         name: str = None,
         need_reboot: bool = None,
+        readonly: bool = None,
         rejected_value: List[str] = None,
         value_type: str = None,
     ):
-        # The valid value range of the parameter.  It is an array with two string elements, which represents a range. The first element represents the minimum value and the second element represents the maximum value.
+        # DescribeParameters
         self.acceptable_value = acceptable_value
-        # The current value of the parameter.
+        # The ID of the OceanBase cluster.
         self.current_value = current_value
-        # The default value of the parameter.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeParameters
+        # &InstanceId=ob317v4uif****\
+        # &Dimension=TENANT
+        # &DimensionValue=ob2mr3oae0****\
+        # &Common request parameters
+        # ```
         self.default_value = default_value
         # The description of the parameter.
         self.description = description
-        # The name of the parameter.
+        # The request ID.
         self.name = name
-        # Indicates whether a restart is required for changes to the parameter to take effect. Valid values:   
-        # - true: A restart is required.   
-        # - false: A restart is not required.
+        # The name of the parameter.
         self.need_reboot = need_reboot
+        # 参数是否只读
+        self.readonly = readonly
+        # {
+        #     "RequestId": "EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C",
+        #     "Parameters": [
+        #         {
+        #             "Description": "The maximum delay allowed in weak-consistency reads.",
+        #             "ValueType": "CAPACITY",
+        #             "CurrentValue": "600",
+        #             "NeedReboot": false,
+        #             "Name": "connect_timeout",
+        #             "DefaultValue": "600s",
+        #             "RejectedValue": [
+        #                 "1s"
+        #             ],
+        #             "AcceptableValue": [
+        #                 "1s"
+        #             ]
+        #         }
+        #     ]
+        # }
+        self.rejected_value = rejected_value
         # The invalid value range of the parameter.    
         # It is an array with two string elements, which represents a range. The first element represents the minimum value and the second element represents the maximum value.
-        self.rejected_value = rejected_value
-        # The type of the parameter value.    Valid values:   
-        # - ENUM: an enumeration value.   
-        # - RANGE: a value range.   
-        # - TIME: a time value.   
-        # - CAPACITY: a storage capacity, in KB, MB, or GB.
         self.value_type = value_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9728,14 +9587,16 @@
             result['DefaultValue'] = self.default_value
         if self.description is not None:
             result['Description'] = self.description
         if self.name is not None:
             result['Name'] = self.name
         if self.need_reboot is not None:
             result['NeedReboot'] = self.need_reboot
+        if self.readonly is not None:
+            result['Readonly'] = self.readonly
         if self.rejected_value is not None:
             result['RejectedValue'] = self.rejected_value
         if self.value_type is not None:
             result['ValueType'] = self.value_type
         return result
 
     def from_map(self, m: dict = None):
@@ -9748,30 +9609,34 @@
             self.default_value = m.get('DefaultValue')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('NeedReboot') is not None:
             self.need_reboot = m.get('NeedReboot')
+        if m.get('Readonly') is not None:
+            self.readonly = m.get('Readonly')
         if m.get('RejectedValue') is not None:
             self.rejected_value = m.get('RejectedValue')
         if m.get('ValueType') is not None:
             self.value_type = m.get('ValueType')
         return self
 
 
 class DescribeParametersResponseBody(TeaModel):
     def __init__(
         self,
         parameters: List[DescribeParametersResponseBodyParameters] = None,
         request_id: str = None,
     ):
-        # The information of parameters.
+        # Indicates whether a restart is required for changes to the parameter to take effect. Valid values:   
+        # - true: A restart is required.   
+        # - false: A restart is not required.
         self.parameters = parameters
-        # The request ID.
+        # The return result of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
@@ -9853,33 +9718,27 @@
         dimension_value: str = None,
         end_time: str = None,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
     ):
-        # The type of the parameter.   
-        # Valid values: CLUSTER and TENANT.
+        # The value of the parameter after the modification.
         self.dimension = dimension
-        # The resource ID of the parameter type.   
-        # You can leave this parameter unspecified when you call this operation to query the modification history of cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # The list of parameter modification records.
         self.dimension_value = dimension_value
-        # The end time for the query of parameter modification history.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.end_time = end_time
-        # The ID of the OceanBase cluster.
+        # The name of the parameter.
         self.instance_id = instance_id
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # Default value: 10.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.page_size = page_size
-        # The start time of the time range for querying the parameter modification history.
+        # You can call this operation to query the modification history of cluster or tenant parameters.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9929,31 +9788,36 @@
         dimension_value: str = None,
         name: str = None,
         new_value: str = None,
         old_value: str = None,
         status: str = None,
         update_time: str = None,
     ):
-        # The time when the parameter modification was initiated.
+        # The request ID.
         self.create_time = create_time
-        # The resource ID of the parameter type.    
-        # - When you called this operation to query the modification history of cluster parameters, the value is DEFAULT_DIMENSION_VALUE.   
-        # - When you called this operation to query the modification history of tenant parameters, the value is the tenant ID.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeParametersHistory
+        # &InstanceId=ob317v4uif****\
+        # &Dimension=TENANT
+        # &DimensionValue=ob2mr3oae0****\
+        # &StartTime=2021-06-13 15:40:43
+        # &EndTime=2021-09-13 15:40:43
+        # &PageSize=10
+        # &PageNumber=1
+        # &Common request parameters
+        # ```
         self.dimension_value = dimension_value
-        # The name of the parameter.
+        # You can call this operation to query the modification history of cluster or tenant parameters.
         self.name = name
-        # The value of the parameter after the modification.
         self.new_value = new_value
-        # The parameter value before modification.
+        # The start time of the time range for querying the parameter modification history.
         self.old_value = old_value
-        # The modification status. Valid values:    
-        # - APPLIED: The modification was successful.   
-        # - SCHEDULING: The modification was to be made.
+        # -\
         self.status = status
-        # The time when the parameter modification took effect.
+        # The name of the parameter.
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9999,19 +9863,21 @@
 class DescribeParametersHistoryResponseBodyRespond(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         parameters: List[DescribeParametersHistoryResponseBodyRespondParameters] = None,
         total_count: int = None,
     ):
-        # The number of returned entries on each page.
+        # The end time for the query of parameter modification history.
         self.page_number = page_number
-        # The parameter modification history.
+        # The number of rows to return on each page.   
+        # - Maximum value: 100   
+        # - Default value: 10
         self.parameters = parameters
-        # The number of parameter modification records.
+        # The list of parameter modification records.
         self.total_count = total_count
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
@@ -10048,17 +9914,19 @@
 
 class DescribeParametersHistoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         respond: List[DescribeParametersHistoryResponseBodyRespond] = None,
     ):
-        # The request ID.
+        # The number of the page to return.    
+        # - Start value: 1   
+        # - Default value: 1
         self.request_id = request_id
-        # The list of parameter modification records.
+        # The time when the parameter modification took effect.
         self.respond = respond
 
     def validate(self):
         if self.respond:
             for k in self.respond:
                 if k:
                     k.validate()
@@ -10136,19 +10004,22 @@
 class DescribeRecommendIndexRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         sqlid: str = None,
         tenant_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The return result of the request.
         self.instance_id = instance_id
-        # You can obtain the SQL ID from the return value of the DescribeSlowSQLList or DescribeTopSQLList operation.
+        # The ID of the OceanBase cluster.
         self.sqlid = sqlid
-        # The ID of the tenant.
+        # The index recommended for the SQL statement after calculation by the diagnostic system.   
+        # - If the recommended index is the primary key, PRIMARY is returned.  
+        # - If an index created by the user is recommended, the index name is returned.   
+        # The system recommends only one index for an SQL statement. You can call the DescribeIndexes operation to view the indexes of a table.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10178,25 +10049,17 @@
 class DescribeRecommendIndexResponseBodyRecommendIndex(TeaModel):
     def __init__(
         self,
         suggest_index: str = None,
         table_list: str = None,
         tenant_mode: str = None,
     ):
-        # The index recommended for the SQL statement after calculation by the diagnostic system.   
-        # - If the recommended index is the primary key, PRIMARY is returned.  
-        # - If an index created by the user is recommended, the index name is returned.   
-        # The system recommends only one index for an SQL statement. You can call the DescribeIndexes operation to view the indexes of a table.
+        # Example 1
         self.suggest_index = suggest_index
-        # The tables.   
-        # The data tables involved in the SQL statement corresponding to the SQL ID are returned. For a single-table query, the data table accessed is returned. For a join query, all data tables accessed by the SQL statement are returned and separated with vertical bars (|), for example, "Table1|Table2".
         self.table_list = table_list
-        # The tenant mode.   Valid values:  
-        # Oracle   
-        # MySQL
         self.tenant_mode = tenant_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10227,15 +10090,17 @@
     def __init__(
         self,
         recommend_index: DescribeRecommendIndexResponseBodyRecommendIndex = None,
         request_id: str = None,
     ):
         # The information about the recommended index.
         self.recommend_index = recommend_index
-        # The request ID.
+        # The tenant mode.   Valid values:  
+        # Oracle   
+        # MySQL
         self.request_id = request_id
 
     def validate(self):
         if self.recommend_index:
             self.recommend_index.validate()
 
     def to_map(self):
@@ -10306,17 +10171,17 @@
 
 class DescribeSQLDetailsRequest(TeaModel):
     def __init__(
         self,
         sqlid: str = None,
         tenant_id: str = None,
     ):
-        # SQLID.
+        # The SQL text.
         self.sqlid = sqlid
-        # The ID of the tenant.
+        # SQLID.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10342,19 +10207,17 @@
 class DescribeSQLDetailsResponseBodySQLDetails(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         sqltext: str = None,
         user_name: str = None,
     ):
-        # The name of the database.
         self.db_name = db_name
-        # The SQL text.
+        # {"name":"DescribeSQLDetails","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSQLDetails\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SQLDetails\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.sqltext = sqltext
-        # The username.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10383,17 +10246,23 @@
 
 class DescribeSQLDetailsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         sqldetails: List[DescribeSQLDetailsResponseBodySQLDetails] = None,
     ):
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeSQLDetails**.
         self.request_id = request_id
-        # The details of the SQL statement.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeSQLDetails
+        # &TenantId=t2mr3oae0****\
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &Common request parameters
+        # ```
         self.sqldetails = sqldetails
 
     def validate(self):
         if self.sqldetails:
             for k in self.sqldetails:
                 if k:
                     k.validate()
@@ -10474,28 +10343,25 @@
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         sqlid: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The end time of the time range for querying the SQL execution history.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The number of block index cache hits.
         self.end_time = end_time
-        # The page number.
+        # The end time in UTC +0.
         self.page_number = page_number
-        # The number of entries returned on each page.   
-        # Default value: 10.
+        # The end time.
         self.page_size = page_size
-        # SQLID.
+        # The number of block index cache hits.
         self.sqlid = sqlid
-        # The start time of the time range for querying the SQL execution history.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time.
         self.start_time = start_time
-        # The ID of the tenant.
+        # The average CPU time.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10572,89 +10438,88 @@
         return_rows: int = None,
         row_cache_hit: int = None,
         schedule_time: float = None,
         ssstore_read_row_count: int = None,
         total_wait_time: float = None,
         user_name: str = None,
     ):
-        # The number of rows affected.
-        self.affected_rows = affected_rows
         # The wait time of the client.
+        self.affected_rows = affected_rows
+        # The IP address of the client.
         self.app_wait_time = app_wait_time
-        # The number of block cache hits.
+        # The number of logical reads.
         self.block_cache_hit = block_cache_hit
         # The number of block index cache hits.
         self.block_index_cache_hit = block_index_cache_hit
-        # The number of Bloom filter cache hits.
+        # The username.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit
-        # The IP address of the client.
+        # The number of remote plans.
         self.client_ip = client_ip
-        # The wait time in concurrent execution.
+        # The number of block cache hits.
         self.concurrency_wait_time = concurrency_wait_time
-        # The average CPU time.
+        # The page number.
         self.cpu_time = cpu_time
-        # The name of the database.
+        # The number of retries.
         self.db_name = db_name
-        # The time to wait for decoding.
+        # The number of rows read from the disk.
         self.decode_time = decode_time
-        # The number of physical reads.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.disk_read = disk_read
-        # The average response time.
+        # The number of row cache hits.
         self.elapsed_time = elapsed_time
-        # The end time.
+        # The maximum CPU time.
         self.end_time = end_time
-        # The end time in UTC +0.
+        # The number of rows read from the memory.
         self.end_time_utcstring = end_time_utcstring
-        # The wait event.
+        # The number of rows returned.
         self.event = event
-        # The number of executions per second.
+        # The queuing time.
         self.exec_per_second = exec_per_second
-        # The internal execution time.
+        # The execution history of the SQL statement.
         self.execute_time = execute_time
-        # The number of executions.
+        # The wait time in concurrent execution.
         self.executions = executions
-        # The number of failures.
+        # Example 1
         self.fail_times = fail_times
-        # The time spent in hard parsing.
+        # The number of RPCs.
         self.get_plan_time = get_plan_time
-        # The I/O wait time.
+        # The number of rows affected.
         self.iowait_time = iowait_time
-        # The number of logical reads.
         self.logical_read = logical_read
-        # The maximum CPU time.
+        # The number of row cache hits.
         self.max_cpu_time = max_cpu_time
-        # The maximum response time.
+        # The scheduling duration.
         self.max_elapsed_time = max_elapsed_time
-        # The number of rows read from the memory.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeSQLHistoryList**.
         self.memstore_read_row_count = memstore_read_row_count
-        # The number of plan misses.
+        # The number of Bloom filter cache hits.
         self.miss_plans = miss_plans
-        # The network latency.
+        # The return result of the request.
         self.net_wait_time = net_wait_time
-        # The IP address of the node.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.node_ip = node_ip
-        # The queuing time.
         self.queue_time = queue_time
-        # The number of RPCs.
+        # The quantity.
         self.rpccount = rpccount
-        # The number of remote plans.
+        # The list.
         self.remote_plans = remote_plans
-        # The number of retries.
+        # The number of executions.
         self.retry_count = retry_count
-        # The number of rows returned.
+        # The I/O wait time.
         self.return_rows = return_rows
-        # The number of row cache hits.
+        # {"name":"DescribeSQLHistoryList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSQLHistoryList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SQLHistoryList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"children\":[{\"name\":\"List\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"ExecPerSecond\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"163.0\"},{\"name\":\"MaxCpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"257.967\"},{\"name\":\"BlockCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"14\"},{\"name\":\"DecodeTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"RemotePlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"RPCCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NetWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DiskRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NodeIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"ConcurrencyWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"MemstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"527\"},{\"name\":\"AppWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"ElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"76.382\"},{\"name\":\"MissPlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"AffectedRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ScheduleTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"Event\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"mysql response wait client\"},{\"name\":\"TotalWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"10.966\"},{\"name\":\"ReturnRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecuteTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"61.044\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"89403\"},{\"name\":\"GetPlanTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.052\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"MaxElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"260.44\"},{\"name\":\"BlockIndexCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"4\"},{\"name\":\"EndTimeUTCString\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-12-28T02:08:18Z\"},{\"name\":\"EndTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-12-28T02:08:18Z\"},{\"name\":\"RetryCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ClientIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"1*2.***.1*3.***\"},{\"name\":\"BloomFilterCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"IOWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"FailTimes\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"QueueTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"15.275\"},{\"name\":\"RowCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"LogicalRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"19\"},{\"name\":\"SsstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"43086\"}],\"title\":\"\"},{\"name\":\"Count\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"}],\"title\":\"\",\"description\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.row_cache_hit = row_cache_hit
-        # The scheduling duration.
+        # The end time of the time range for querying the SQL execution history.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.schedule_time = schedule_time
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count
-        # The internal wait time.
+        # The average response time.
         self.total_wait_time = total_wait_time
-        # The username.
+        # The network latency.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10823,16 +10688,16 @@
 
 class DescribeSQLHistoryListResponseBodySQLHistoryList(TeaModel):
     def __init__(
         self,
         count: int = None,
         list: List[DescribeSQLHistoryListResponseBodySQLHistoryListList] = None,
     ):
-        # The quantity.
         self.count = count
+        # The I/O wait time.
         self.list = list
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
@@ -10865,17 +10730,17 @@
 
 class DescribeSQLHistoryListResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         sqlhistory_list: DescribeSQLHistoryListResponseBodySQLHistoryList = None,
     ):
-        # The request ID.
+        # The IP address of the client.
         self.request_id = request_id
-        # The execution history of the SQL statement.
+        # The number of Bloom filter cache hits.
         self.sqlhistory_list = sqlhistory_list
 
     def validate(self):
         if self.sqlhistory_list:
             self.sqlhistory_list.validate()
 
     def to_map(self):
@@ -10946,17 +10811,17 @@
 
 class DescribeSQLPlansRequest(TeaModel):
     def __init__(
         self,
         sqlid: str = None,
         tenant_id: str = None,
     ):
-        # SQLID.
+        # The time when the plan was loaded for the first time, .
         self.sqlid = sqlid
-        # The ID of the tenant.
+        # The time when the plan was loaded for the first time, .
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10995,45 +10860,43 @@
         outline_time_utcstring: str = None,
         plan_full: str = None,
         plan_id: int = None,
         plan_info: str = None,
         plan_union_hash: str = None,
         query_sql: str = None,
     ):
-        # The average execution duration, in ms.
+        # The time when the plan was bound.
         self.avg_execution_ms = avg_execution_ms
-        # The average execution duration when the database uses this execution plan, in ms.
+        # The time when the plan was loaded for the first time, in UTC +0.
         self.avg_execution_time_ms = avg_execution_time_ms
-        # The time when the plan was loaded for the first time, .
         self.first_load_time = first_load_time
-        # The time when the plan was loaded for the first time, in UTC +0.
+        # Example 1
         self.first_load_time_utcstring = first_load_time_utcstring
-        # The number of hits.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.hit_count = hit_count
-        # The major compaction version.
+        # The unique identifier of the SQL execution plan in the diagnostic system.
         self.merged_version = merged_version
-        # The IP address of the node.
+        # The complete execution plan of the SQL statement.
         self.node_ip = node_ip
-        # The outline data.
+        # The information about the plan.
         self.outline_data = outline_data
-        # OutlineID.
+        # SQLID.
         self.outline_id = outline_id
-        # The time when the plan was bound.
+        # The ID of the SQL execution plan in the database.
         self.outline_time = outline_time
-        # The time when the plan was bound, in UTC +0.
+        # The major compaction version.
         self.outline_time_utcstring = outline_time_utcstring
-        # The complete execution plan of the SQL statement.
+        # The information about the execution plan.
         self.plan_full = plan_full
-        # The ID of the SQL execution plan in the database.
+        # OutlineID.
         self.plan_id = plan_id
-        # The information about the plan.
         self.plan_info = plan_info
-        # The unique identifier of the SQL execution plan in the diagnostic system.
+        # The return result of the request.
         self.plan_union_hash = plan_union_hash
-        # The query SQL statement.
+        # The request ID.
         self.query_sql = query_sql
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11114,17 +10977,17 @@
 
 class DescribeSQLPlansResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         sqlplans: List[DescribeSQLPlansResponseBodySQLPlans] = None,
     ):
-        # The request ID.
+        # The return result of the request.
         self.request_id = request_id
-        # The information about the execution plan.
+        # master
         self.sqlplans = sqlplans
 
     def validate(self):
         if self.sqlplans:
             for k in self.sqlplans:
                 if k:
                     k.validate()
@@ -11229,18 +11092,15 @@
 
 class DescribeSecurityIpGroupsResponseBodySecurityIpGroups(TeaModel):
     def __init__(
         self,
         security_ip_group_name: str = None,
         security_ips: str = None,
     ):
-        # The name of the security group.
         self.security_ip_group_name = security_ip_group_name
-        # The list of IP addresses and CIDR blocks in the whitelist.   
-        # It is a JSON array. Each object in the array is an IP address or CIDR block.
         self.security_ips = security_ips
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11268,17 +11128,16 @@
         self,
         request_id: str = None,
         security_ip_groups: List[DescribeSecurityIpGroupsResponseBodySecurityIpGroups] = None,
         total_count: int = None,
     ):
         # The request ID.
         self.request_id = request_id
-        # The information of the IP address whitelist group.
         self.security_ip_groups = security_ip_groups
-        # The number of whitelist groups returned.
+        # Example 1
         self.total_count = total_count
 
     def validate(self):
         if self.security_ip_groups:
             for k in self.security_ip_groups:
                 if k:
                     k.validate()
@@ -11363,29 +11222,23 @@
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         sqlid: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The end time of the time range for querying the execution history of the slow SQL statement.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The number of RPCs.
         self.end_time = end_time
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The maximum response time.
         self.page_number = page_number
-        # The number of rows to return on each page.  
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of plan misses.
         self.page_size = page_size
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The wait time for network.
         self.sqlid = sqlid
-        # The start time of the time range for querying the execution history of the slow SQL statement.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The I/O wait time.
         self.start_time = start_time
         # The ID of the tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
@@ -11466,93 +11319,104 @@
         sql_id: str = None,
         sql_type: str = None,
         ssstore_read_row_count: float = None,
         tenant_name: str = None,
         total_wait_time: float = None,
         user_name: str = None,
     ):
-        # The number of rows affected.
+        # The wait event.
         self.affected_rows = affected_rows
-        # The wait time of the client.
+        # The number of row cache hits.
         self.app_wait_time = app_wait_time
-        # The number of block cache hits.
+        # The average CPU time.
         self.block_cache_hit = block_cache_hit
-        # The number of block index cache hits.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100   
+        # - Default value: 10
         self.block_index_cache_hit = block_index_cache_hit
-        # The number of Bloom filter cache hits.
+        # The number of executions.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit
-        # The IP address of the client.
+        # The number of retries.
         self.client_ip = client_ip
-        # The wait time in concurrent execution.
+        # $.parameters[6].schema.example
         self.concurrency_wait_time = concurrency_wait_time
-        # The average CPU time.
+        # $.parameters[6].schema.enumValueTitles
         self.cpu_time = cpu_time
-        # The name of the database.
+        # The IP address of the node.
         self.db_name = db_name
-        # The time to wait for decoding.
+        # $.parameters[7].schema.description
         self.decode_time = decode_time
-        # The number of physical reads.
+        # SQLID.
         self.disk_read = disk_read
-        # The average response time.
+        # The queuing time.
         self.elapsed_time = elapsed_time
-        # The end time.
         self.end_time_utcstring = end_time_utcstring
-        # The wait event.
+        # The internal wait time.
         self.event = event
-        # The number of executions per second.
+        # The number of failures.
         self.exec_per_second = exec_per_second
-        # The internal execution time.
+        # The request ID.
         self.execute_time = execute_time
-        # The number of executions.
+        # The maximum CPU time.
         self.executions = executions
-        # The number of failures.
+        # The number of rows returned.
         self.fail_times = fail_times
-        # Hard parsing time.
+        # Example 1
         self.get_plan_time = get_plan_time
-        # The I/O wait time.
+        # $.parameters[7].schema.enumValueTitles
         self.iowait_time = iowait_time
-        # The number of logical reads.
+        # The quantity.
         self.logical_read = logical_read
-        # The maximum CPU time.
+        # DescribeSlowSQLHistoryList
         self.max_cpu_time = max_cpu_time
-        # The maximum response time.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeSlowSQLHistoryList
+        # &TenantId=t384tolsj****\
+        # &StartTime=2021-12-14T02:34:49Z
+        # &EndTime=2021-12-14T08:34:49Z
+        # &SQLId=8D6E84735C0****1823D199E2CA1****\
+        # &PageNumber=1
+        # &PageSize=10
+        # &Common request parameters
+        # ```
         self.max_elapsed_time = max_elapsed_time
-        # The number of rows read from the memory.
+        # The wait time of the client.
         self.memstore_read_row_count = memstore_read_row_count
-        # The number of plan misses.
+        # The number of rows read from the disk.
         self.miss_plans = miss_plans
-        # The wait time for network.
+        # $.parameters[7].schema.example
         self.net_wait_time = net_wait_time
-        # The IP address of the node.
+        # The number of the page to return.    
+        # - Start value: 1   
+        # - Default value: 1
         self.node_ip = node_ip
-        # The queuing time.
+        # $.parameters[6].schema.description
         self.queue_time = queue_time
-        # The number of RPCs.
+        # The end time.
         self.rpccount = rpccount
-        # The number of remote plans.
+        # The time to wait for decoding.
         self.remote_plans = remote_plans
-        # The number of retries.
+        # The number of block index cache hits.
         self.retry_count = retry_count
-        # The number of rows returned.
+        # The number of executions per second.
         self.return_rows = return_rows
-        # The number of row cache hits.
+        # The execution history of the slow SQL statement.
         self.row_cache_hit = row_cache_hit
-        # The scheduling duration.
+        # You can call this operation to query the execution history of an SQL statement by SQL ID that is determined as a slow SQL statement during a specified period of time.
         self.schedule_time = schedule_time
-        # SQLID.
+        # The return result of the request.
         self.sql_id = sql_id
-        # The SQL type.
+        # The IP address of the client.
         self.sql_type = sql_type
-        # The number of rows read from the disk.
+        # The scheduling duration.
         self.ssstore_read_row_count = ssstore_read_row_count
-        # The name of the tenant.
+        # The return result of the request.
         self.tenant_name = tenant_name
-        # The internal wait time.
         self.total_wait_time = total_wait_time
-        # The username.
+        # The number of physical reads.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11729,17 +11593,16 @@
 
 class DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryList(TeaModel):
     def __init__(
         self,
         count: int = None,
         list: List[DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryListList] = None,
     ):
-        # The quantity.
         self.count = count
-        # The return result of the request.
+        # The SQL ID, which uniquely identifies an SQL statement.
         self.list = list
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
@@ -11772,17 +11635,18 @@
 
 class DescribeSlowSQLHistoryListResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         slow_sqlhistory_list: DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryList = None,
     ):
-        # The request ID.
+        # The end time of the time range for querying the execution history of the slow SQL statement.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.request_id = request_id
-        # The execution history of the slow SQL statement.
+        # Hard parsing time。
         self.slow_sqlhistory_list = slow_sqlhistory_list
 
     def validate(self):
         if self.slow_sqlhistory_list:
             self.slow_sqlhistory_list.validate()
 
     def to_map(self):
@@ -11866,49 +11730,46 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.db_name = db_name
-        # The end time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time
         # The filter condition.
         self.filter_condition = filter_condition
-        # The IP address of the database node.
+        # The number of plan misses.
         self.node_ip = node_ip
-        # The number of rows to return on each page.  
-        # - Maximum value: 100  
-        # - Default value: 10
-        self.page_number = page_number
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
+        self.page_number = page_number
+        # The return result of the request.
         self.page_size = page_size
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The internal wait time.
         self.sqlid = sqlid
-        # The search keyword.
+        # Alibaba Cloud CLI
         self.search_key_word = search_key_word
-        # The search parameter.
+        # The IP address of the database node.
         self.search_parameter = search_parameter
-        # The search rule.
+        # The queuing time.
         self.search_rule = search_rule
-        # The search value.
+        # The list of slow SQL statements.
         self.search_value = search_value
-        # The sorted column.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100  
+        # - Default value: 10
         self.sort_column = sort_column
-        # The sorting rule.
+        # The average CPU time.
         self.sort_order = sort_order
-        # The start time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The list of slow SQL statements.
         self.start_time = start_time
-        # The ID of the tenant.
+        # The number of logical reads.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11998,49 +11859,46 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.db_name = db_name
-        # The end time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time
         # The filter condition.
         self.filter_condition_shrink = filter_condition_shrink
-        # The IP address of the database node.
+        # The number of plan misses.
         self.node_ip = node_ip
-        # The number of rows to return on each page.  
-        # - Maximum value: 100  
-        # - Default value: 10
-        self.page_number = page_number
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
+        self.page_number = page_number
+        # The return result of the request.
         self.page_size = page_size
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The internal wait time.
         self.sqlid = sqlid
-        # The search keyword.
+        # Alibaba Cloud CLI
         self.search_key_word = search_key_word
-        # The search parameter.
+        # The IP address of the database node.
         self.search_parameter = search_parameter
-        # The search rule.
+        # The queuing time.
         self.search_rule = search_rule
-        # The search value.
+        # The list of slow SQL statements.
         self.search_value = search_value
-        # The sorted column.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100  
+        # - Default value: 10
         self.sort_column = sort_column
-        # The sorting rule.
+        # The average CPU time.
         self.sort_order = sort_order
-        # The start time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The list of slow SQL statements.
         self.start_time = start_time
-        # The ID of the tenant.
+        # The number of logical reads.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12155,93 +12013,105 @@
         sqltext: str = None,
         sqltype: int = None,
         schedule_time: float = None,
         ssstore_read_row_count: int = None,
         total_wait_time: float = None,
         user_name: str = None,
     ):
-        # The number of rows affected.
+        # The username.
         self.affected_rows = affected_rows
-        # The wait time of the client.
+        # The average response time.
         self.app_wait_time = app_wait_time
-        # The number of block cache hits.
+        # The wait time in concurrent execution.
         self.block_cache_hit = block_cache_hit
-        # The number of block index cache hits.
+        # The request ID.
         self.block_index_cache_hit = block_index_cache_hit
-        # The number of Bloom filter cache hits.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit
-        # The IP address of the client.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeSlowSQLList
+        # &TenantId=t2mr3oae0****\
+        # &StartTime=2021-06-13 15:40:43
+        # &EndTime=2021-09-13 15:40:43
+        # &DbName=testdb
+        # &SearchKeyWord=update
+        # &SearchParameter=cputime
+        # &SearchRule=>
+        # &SearchValue=0.01
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &NodeIp=i-bp18qljorblo8es*****\
+        # &PageNumber=10
+        # &PageSize=1
+        # &SortColumn=cputime
+        # &SortOrder=desc
+        # &Common request parameters
+        # ```
         self.client_ip = client_ip
-        # The wait time in concurrent execution.
+        # The sorted column.
         self.concurrency_wait_time = concurrency_wait_time
-        # The average CPU time.
+        # The wait event.
         self.cpu_time = cpu_time
-        # The name of the database.
+        # The search value.
         self.db_name = db_name
-        # The time to wait for decoding.
+        # The time spent in hard parsing.
         self.decode_time = decode_time
-        # The number of physical reads.
+        # The IP address of the client.
         self.disk_read = disk_read
-        # The average response time.
+        # The search rule.
         self.elapsed_time = elapsed_time
-        # The wait event.
+        # The number of row cache hits.
         self.event = event
-        # The number of executions per second.
+        # The total count.
         self.exec_per_second = exec_per_second
-        # The internal execution time.
+        # The number of block cache hits.
         self.execute_time = execute_time
-        # The number of executions.
+        # The IP address of the node.
         self.executions = executions
-        # The number of failures.
+        # {"name":"DescribeSlowSQLList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"GET|POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSlowSQLList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"DbName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SearchKeyWord\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"update\"},{\"name\":\"SearchParameter\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SearchRule\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\">\"},{\"name\":\"SearchValue\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"0.01\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"NodeIp\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"FilterCondition\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"[dbName:sys]\"},{\"name\":\"SortColumn\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SortOrder\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"desc\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SlowSQLList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"Key\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecPerSecond\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"163.0\"},{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"MaxCpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"257.967\"},{\"name\":\"BlockCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"14\"},{\"name\":\"DecodeTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"RemotePlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"RPCCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NetWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DiskRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NodeIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"ConcurrencyWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"MemstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"527\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"AppWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"ElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"76.382\"},{\"name\":\"MissPlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"AffectedRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ScheduleTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"Event\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"mysql response wait client\"},{\"name\":\"TotalWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"10.966\"},{\"name\":\"ReturnRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecuteTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"61.044\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"tester\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"89403\"},{\"name\":\"GetPlanTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.052\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"MaxElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"260.044\"},{\"name\":\"SQLType\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"BlockIndexCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"4\"},{\"name\":\"RetryCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"SQLId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"ClientIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"1*2.***.1*3.***\"},{\"name\":\"BloomFilterCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"IOWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"FailTimes\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"QueueTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"15.275\"},{\"name\":\"RowCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"LogicalRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"19\"},{\"name\":\"SsstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"43086\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.fail_times = fail_times
-        # The time spent in hard parsing.
+        # The number of Bloom filter cache hits.
         self.get_plan_time = get_plan_time
-        # The I/O wait time.
+        # You can call this operation to query the list of slow SQL statements
         self.iowait_time = iowait_time
-        # The sequence number of the returned SQL statement.
+        # The scheduling duration.
         self.key = key
-        # The number of logical reads.
         self.logical_read = logical_read
-        # The maximum CPU time.
+        # The name of the database.
         self.max_cpu_time = max_cpu_time
-        # The maximum response time.
+        # The sequence number of the returned SQL statement.
         self.max_elapsed_time = max_elapsed_time
-        # The number of rows read from the memory.
+        # The number of logical reads.
         self.memstore_read_row_count = memstore_read_row_count
-        # The number of plan misses.
+        # The number of RPCs.
         self.miss_plans = miss_plans
-        # The network latency.
+        # The search parameter.
         self.net_wait_time = net_wait_time
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip
-        # The queuing time.
         self.queue_time = queue_time
-        # The number of RPCs.
+        # The maximum response time.
         self.rpccount = rpccount
-        # The number of remote plans.
+        # The search keyword.
         self.remote_plans = remote_plans
-        # The number of retries.
+        # The number of physical reads.
         self.retry_count = retry_count
-        # The number of rows returned.
+        # The wait time of the client.
         self.return_rows = return_rows
-        # The number of row cache hits.
         self.row_cache_hit = row_cache_hit
-        # SQLID.
+        # Example 1
         self.sqlid = sqlid
-        # The SQL text.
+        # The network latency.
         self.sqltext = sqltext
-        # The SQL type.
+        # SQLID.
         self.sqltype = sqltype
-        # The scheduling duration.
+        # The internal execution time.
         self.schedule_time = schedule_time
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count
-        # The internal wait time.
+        # The SQL ID, which uniquely identifies an SQL statement.
         self.total_wait_time = total_wait_time
-        # The username.
+        # The number of executions.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12419,19 +12289,19 @@
 class DescribeSlowSQLListResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         slow_sqllist: List[DescribeSlowSQLListResponseBodySlowSQLList] = None,
         total_count: int = None,
     ):
-        # The request ID.
+        # The SQL text.
         self.request_id = request_id
-        # The list of slow SQL statements.
+        # The sorting rule.
         self.slow_sqllist = slow_sqllist
-        # The total count.
+        # The name of the database.
         self.total_count = total_count
 
     def validate(self):
         if self.slow_sqllist:
             for k in self.slow_sqllist:
                 if k:
                     k.validate()
@@ -12512,17 +12382,21 @@
 
 class DescribeTenantRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The status of the Internet address for accessing the tenant. Valid values:   
+        # - CLOSED: The address is disabled.   
+        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
+        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
+        # - ONLINE: The address is in service.
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # Indicates whether to enable transaction splitting.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12559,49 +12433,47 @@
         intranet_address_slave_zone_id: str = None,
         intranet_address_status: str = None,
         intranet_port: int = None,
         transaction_split: bool = None,
         v_switch_id: str = None,
         vpc_id: str = None,
     ):
-        # The type of the address.
+        # The primary zone of the tenant.
         self.address_type = address_type
-        # The service mode of the connection address. Valid values:  
-        # - ReadWrite: provides strong-consistency read and write services.   
-        # - ReadOnly: provides the read-only service to ensure ultimate consistency of data.   
-        # - Clog: provides transaction log services.
+        # 是否开启事务拆分
         self.connection_role = connection_role
-        # The list of zones corresponding to the tenant connection.
-        self.connection_zones = connection_zones
         # The Internet address for accessing the tenant.
+        self.connection_zones = connection_zones
+        # The ID of the VPC.
         self.internet_address = internet_address
-        # The status of the Internet address for accessing the tenant. Valid values:   
-        # - CLOSED: The address is disabled.   
-        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
-        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
-        # - ONLINE: The address is in service.
+        # 实例系列
         self.internet_address_status = internet_address_status
-        # The Internet port for accessing the tenant.
+        # 实例类型
         self.internet_port = internet_port
-        # The intranet address for accessing the tenant.
+        # The deployment type of the cluster. Valid values:  
+        # - multiple: multi-IDC deployment   
+        # - single: single-IDC deployment   
+        # - dual: dual-IDC deployment
         self.intranet_address = intranet_address
-        # The primary zone corresponding to the address for accessing the tenant.
+        # PayCore business database
         self.intranet_address_master_zone_id = intranet_address_master_zone_id
-        # The standby zone corresponding to the address for accessing the tenant.
+        # The total number of CPU cores of the tenant.
         self.intranet_address_slave_zone_id = intranet_address_slave_zone_id
-        # The status of the intranet address for accessing the tenant.  
-        # The value ONLINE indicates that the address is in service.
+        # 付费类型
         self.intranet_address_status = intranet_address_status
-        # The intranet port for accessing the tenant.
+        # The ID of the tenant.
         self.intranet_port = intranet_port
-        # Indicates whether to enable transaction splitting.
+        # The primary zone corresponding to the address for accessing the tenant.
         self.transaction_split = transaction_split
-        # The ID of the vSwitch.
+        # The connection access information of the tenant.
         self.v_switch_id = v_switch_id
-        # The ID of the VPC.
+        # The service mode of the connection address. Valid values:  
+        # ReadWrite: provides strong-consistency read and write services.   
+        # ReadOnly: provides the read-only service to ensure ultimate consistency of data.   
+        # Clog: provides transaction log services.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12675,19 +12547,27 @@
 class DescribeTenantResponseBodyTenantTenantResourceCpu(TeaModel):
     def __init__(
         self,
         total_cpu: float = None,
         unit_cpu: float = None,
         used_cpu: float = None,
     ):
-        # The total number of CPU cores of the tenant.
+        # The data replica distribution mode of the tenant.    
+        # 
+        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
+        # - For the basic version, N indicates the single-zone mode. 
+        # 
+        # > <br>N represents the number of nodes in a single zone.
         self.total_cpu = total_cpu
-        # The number of CPU cores in each resource unit of the tenant.
+        # The zone corresponding to the tenant connection.
         self.unit_cpu = unit_cpu
-        # The number of used CPU cores of the tenant.
+        # The tenant mode.   
+        # Valid values: 
+        # Oracle   
+        # MySQL
         self.used_cpu = used_cpu
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12715,15 +12595,15 @@
 
 
 class DescribeTenantResponseBodyTenantTenantResourceDiskSize(TeaModel):
     def __init__(
         self,
         used_disk_size: float = None,
     ):
-        # The size of used disk space of the tenant, in GB.
+        # The total memory size of the tenant, in GB.
         self.used_disk_size = used_disk_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12745,19 +12625,23 @@
 class DescribeTenantResponseBodyTenantTenantResourceMemory(TeaModel):
     def __init__(
         self,
         total_memory: float = None,
         unit_memory: float = None,
         used_memory: float = None,
     ):
-        # The total memory size of the tenant, in GB.
+        # The information about the memory resources of the tenant.
         self.total_memory = total_memory
-        # The memory size of each resource unit of the tenant, in GB.
+        # The time when the tenant was created.
         self.unit_memory = unit_memory
-        # The size of used memory of the tenant, in GB.
+        # The status of the Internet address for accessing the tenant. Valid values:   
+        # Closed: The address is disabled.   
+        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
+        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
+        # - ONLINE: The address is in service.
         self.used_memory = used_memory
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12788,21 +12672,24 @@
     def __init__(
         self,
         cpu: DescribeTenantResponseBodyTenantTenantResourceCpu = None,
         disk_size: DescribeTenantResponseBodyTenantTenantResourceDiskSize = None,
         memory: DescribeTenantResponseBodyTenantTenantResourceMemory = None,
         unit_num: int = None,
     ):
-        # The information about the CPU resources of the tenant.
+        # The enabling status of the Clog service.  
+        # CLOSED: The Clog service is disabled.  
+        # - ONLINE: The Clog service is running.
         self.cpu = cpu
-        # The information about the disk resources of the tenant.
+        # The status of the intranet address for accessing the tenant.  
+        # The value ONLINE indicates that the address is in service.
         self.disk_size = disk_size
-        # The information about the memory resources of the tenant.
+        # The description of the tenant.
         self.memory = memory
-        # The number of resource units in the tenant.
+        # Alibaba Cloud CLI
         self.unit_num = unit_num
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -12844,19 +12731,19 @@
 class DescribeTenantResponseBodyTenantTenantZones(TeaModel):
     def __init__(
         self,
         region: str = None,
         tenant_zone_id: str = None,
         tenant_zone_role: str = None,
     ):
-        # The region where the zone of the tenant resides.
+        # 是否允许开启读写分离地址
         self.region = region
-        # The ID of the zone.
+        # The intranet port for accessing the tenant.
         self.tenant_zone_id = tenant_zone_id
-        # The role of the zone of the tenant.
+        # The character set.
         self.tenant_zone_role = tenant_zone_role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12891,14 +12778,15 @@
         clog_service_status: str = None,
         collation: str = None,
         create_time: str = None,
         deploy_mode: str = None,
         deploy_type: str = None,
         description: str = None,
         disk_type: str = None,
+        enable_binlog_service: bool = None,
         enable_clog_service: bool = None,
         enable_internet_address_service: bool = None,
         enable_read_write_split: bool = None,
         instance_type: str = None,
         master_intranet_address_zone: str = None,
         pay_type: str = None,
         primary_zone: str = None,
@@ -12909,88 +12797,187 @@
         tenant_id: str = None,
         tenant_mode: str = None,
         tenant_name: str = None,
         tenant_resource: DescribeTenantResponseBodyTenantTenantResource = None,
         tenant_zones: List[DescribeTenantResponseBodyTenantTenantZones] = None,
         vpc_id: str = None,
     ):
-        # The list of zones.
+        # DescribeTenant
         self.available_zones = available_zones
-        # The character set.
+        # The number of CPU cores in each resource unit of the tenant.
         self.charset = charset
-        # The enabling status of the clog service.  
-        # - CLOSED: The clog service is disabled.  
-        # - ONLINE: The clog service is running.
+        # 地址类型
         self.clog_service_status = clog_service_status
-        # The collation.
+        # The request ID.
         self.collation = collation
-        # The time when the tenant was created.
+        # You can call this operation to create a single tenant in a specific cluster.
         self.create_time = create_time
-        # The data replica distribution mode of the tenant.    
-        # 
-        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
-        # - For the basic version, N indicates the single-zone mode. 
-        # 
-        # > <br>N represents the number of nodes in a single zone.
+        # The list of zones.
         self.deploy_mode = deploy_mode
-        # The deployment type of the cluster. Valid values:  
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The series of the instance.
         self.deploy_type = deploy_type
-        # The description of the tenant.
+        # Indicates whether to enable read/write splitting endpoint.
         self.description = description
-        # The type of the disk.
+        # You can call this operation to query the information of a specific tenant in a specific cluster.
         self.disk_type = disk_type
-        # Indicates whether the clog service is available. To enable the clog service, submit a ticket.
+        # 是否可以申请Binlog服务
+        self.enable_binlog_service = enable_binlog_service
+        # The intranet address for accessing the tenant.
         self.enable_clog_service = enable_clog_service
-        # Indicates whether the Internet address can be enabled for the tenant.
+        # The deployment type of the primary zone.
         self.enable_internet_address_service = enable_internet_address_service
-        # Indicates whether to enable read/write splitting endpoint.
         self.enable_read_write_split = enable_read_write_split
-        # The type of the instance.
+        # {
+        #     "RequestId": "EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C",
+        #     "Tenant": {
+        #         "TenantId": "t33h8y08k****",
+        #         "TenantName": "pay_online",
+        #         "TenantMode": "Oracle",
+        #         "VpcId": "vpc-bp1d2q3mhg9i23ofi****",
+        #         "Status": "ONLINE",
+        #         "PrimaryZone": "cn-hangzhou-i",
+        #         "DeployType": "multiple",
+        #         "DeployMode": "1-1-1",
+        #         "Description": "PayCore business database",
+        #         "CreateTime": "2021-09-17 15:52:17",
+        #         "TenantResource": {
+        #             "UnitNum": 1,
+        #             "Cpu": {
+        #                 "UsedCpu": 8,
+        #                 "TotalCpu": 10,
+        #                 "UnitCpu": 8
+        #             },
+        #             "Memory": {
+        #                 "UsedMemory": 30,
+        #                 "TotalMemory": 64,
+        #                 "UnitMemory": 32
+        #             },
+        #             "DiskSize": {
+        #                 "UsedDiskSize": 86
+        #             }
+        #         },
+        #         "TenantConnections": [
+        #             {
+        #                 "ConnectionRole": "ReadWrite",
+        #                 "IntranetAddress": "t32a7ru5u****.oceanbase.aliyuncs.com",
+        #                 "IntranetPort": 3306,
+        #                 "InternetAddress": "t32a7ru5u****mo.oceanbase.aliyuncs.com",
+        #                 "InternetPort": 3306,
+        #                 "VpcId": "vpc-bp1qiail1asmfe23t****",
+        #                 "VSwitchId": "vsw-bp11k1aypnzu1l3whi****",
+        #                 "IntranetAddressMasterZoneId": "cn-hangzhou-i",
+        #                 "IntranetAddressSlaveZoneId": "cn-hangzhou-j",
+        #                 "IntranetAddressStatus": "ONLINE",
+        #                 "ConnectionZones": [
+        #                     "cn-hangzhou-i"
+        #                 ],
+        #                 "InternetAddressStatus": "CLOSED"
+        #             }
+        #         ],
+        #         "TenantZones": [
+        #             {
+        #                 "TenantZoneId": "cn-hangzhou-i",
+        #                 "Region": "cn-hangzhou",
+        #                 "TenantZoneRole": "ReadOnly"
+        #             }
+        #         ],
+        #         "ClogServiceStatus": "CLOSED"
+        #     }
+        # }
         self.instance_type = instance_type
-        # The zone where the primary node is located.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeTenant
+        # &InstanceId=ob317v4uif****\
+        # &TenantId=ob2mr3oae0****\
+        # &Common request parameters
+        # ```
         self.master_intranet_address_zone = master_intranet_address_zone
-        # The type of the payment.
         self.pay_type = pay_type
-        # The primary zone of the tenant.
+        # The type of the payment.
         self.primary_zone = primary_zone
-        # The deployment type of the primary zone.
+        # Example 1
         self.primary_zone_deploy_type = primary_zone_deploy_type
-        # The series of the instance.
+        # <DescribeTenantResponse>
+        #     <RequestId>EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C</RequestId>
+        #     <Tenant>
+        #         <TenantId>t33h8y08k****</TenantId>
+        #         <TenantName>pay_online</TenantName>
+        #         <TenantMode>Oracle</TenantMode>
+        #         <VpcId>vpc-bp1d2q3mhg9i23ofi****</VpcId>
+        #         <Status>ONLINE</Status>
+        #         <PrimaryZone>cn-hangzhou-i</PrimaryZone>
+        #         <DeployType>multiple</DeployType>
+        #         <DeployMode>1-1-1</DeployMode>
+        #         <Description>PayCore business database</Description>
+        #         <CreateTime>2021-09-17 15:52:17</CreateTime>
+        #         <TenantResource>
+        #             <UnitNum>1</UnitNum>
+        #             <Cpu>
+        #                 <UsedCpu>8</UsedCpu>
+        #                 <TotalCpu>10</TotalCpu>
+        #                 <UnitCpu>8</UnitCpu>
+        #             </Cpu>
+        #             <Memory>
+        #                 <UsedMemory>30</UsedMemory>
+        #                 <TotalMemory>64</TotalMemory>
+        #                 <UnitMemory>32</UnitMemory>
+        #             </Memory>
+        #             <DiskSize>
+        #                 <UsedDiskSize>86</UsedDiskSize>
+        #             </DiskSize>
+        #         </TenantResource>
+        #         <TenantConnections>
+        #             <ConnectionRole>ReadWrite</ConnectionRole>
+        #             <IntranetAddress>t32a7ru5u****.oceanbase.aliyuncs.com</IntranetAddress>
+        #             <IntranetPort>3306</IntranetPort>
+        #             <InternetAddress>t32a7ru5u****mo.oceanbase.aliyuncs.com</InternetAddress>
+        #             <InternetPort>3306</InternetPort>
+        #             <VpcId>vpc-bp1qiail1asmfe23t****</VpcId>
+        #             <VSwitchId>vsw-bp11k1aypnzu1l3whi****</VSwitchId>
+        #             <IntranetAddressMasterZoneId>cn-hangzhou-i</IntranetAddressMasterZoneId>
+        #             <IntranetAddressSlaveZoneId>cn-hangzhou-j</IntranetAddressSlaveZoneId>
+        #             <IntranetAddressStatus>ONLINE</IntranetAddressStatus>
+        #             <ConnectionZones>cn-hangzhou-i</ConnectionZones>
+        #             <InternetAddressStatus>CLOSED</InternetAddressStatus>
+        #         </TenantConnections>
+        #         <TenantZones>
+        #             <TenantZoneId>cn-hangzhou-i</TenantZoneId>
+        #             <Region>cn-hangzhou</Region>
+        #             <TenantZoneRole>ReadOnly</TenantZoneRole>
+        #         </TenantZones>
+        #         <ClogServiceStatus>CLOSED</ClogServiceStatus>
+        #     </Tenant>
+        # </DescribeTenantResponse>
         self.series = series
+        # The character set.
+        self.status = status
         # The status of the tenant.   
         # - PENDING_CREATE: The tenant is being created.   
         # - RESTORE: The tenant is being recovered.   
         # - ONLINE: The tenant is running.   
         # - SPEC_MODIFYING: The specification of the tenant is being modified.   
         # - ALLOCATING_INTERNET_ADDRESS: An Internet address is being allocated.  
         # - PENDING_OFFLINE_INTERNET_ADDRESS: The Internet address is being disabled.  
         # - PRIMARY_ZONE_MODIFYING: The tenant is switching to a new primary zone.  
         # - PARAMETER_MODIFYING: Parameters are being modified.   
         # - WHITE_LIST_MODIFYING: The whitelist is being modified.
-        self.status = status
-        # The connection information of the tenant.
         self.tenant_connections = tenant_connections
-        # The ID of the tenant.
+        # The region where the zone of the tenant resides.
         self.tenant_id = tenant_id
-        # The tenant mode.   
-        # Valid values:
-        # - Oracle   
-        # - MySQL
+        # The enabling status of the clog service.  
+        # - CLOSED: The clog service is disabled.  
+        # - ONLINE: The clog service is running.
         self.tenant_mode = tenant_mode
-        # The name of the tenant.
+        # The request type of the zone of the tenant.  ReadWrite: The zone supports data reads and writes. ReadOnly: The zone supports only data reads. For a high availability cluster with multiple IDCs, the primary zone provides ReadWrite services, and the standby zone provides ReadOnly services. For a high availability cluster with a single IDC, all zones provide ReadWrite services.
         self.tenant_name = tenant_name
-        # The resource information of the tenant.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.tenant_resource = tenant_resource
-        # The zone information of the tenant.
+        # The standby zone corresponding to the address for accessing the tenant.
         self.tenant_zones = tenant_zones
-        # The ID of the VPC.    
-        # If no suitable VPC is available, create a VPC as prompted. For more information, see "What is a VPC".
+        # Indicates whether the clog service is available. To enable the clog service, submit a ticket.
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.tenant_connections:
             for k in self.tenant_connections:
                 if k:
                     k.validate()
@@ -13021,14 +13008,16 @@
             result['DeployMode'] = self.deploy_mode
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
         if self.description is not None:
             result['Description'] = self.description
         if self.disk_type is not None:
             result['DiskType'] = self.disk_type
+        if self.enable_binlog_service is not None:
+            result['EnableBinlogService'] = self.enable_binlog_service
         if self.enable_clog_service is not None:
             result['EnableClogService'] = self.enable_clog_service
         if self.enable_internet_address_service is not None:
             result['EnableInternetAddressService'] = self.enable_internet_address_service
         if self.enable_read_write_split is not None:
             result['EnableReadWriteSplit'] = self.enable_read_write_split
         if self.instance_type is not None:
@@ -13081,14 +13070,16 @@
             self.deploy_mode = m.get('DeployMode')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('DiskType') is not None:
             self.disk_type = m.get('DiskType')
+        if m.get('EnableBinlogService') is not None:
+            self.enable_binlog_service = m.get('EnableBinlogService')
         if m.get('EnableClogService') is not None:
             self.enable_clog_service = m.get('EnableClogService')
         if m.get('EnableInternetAddressService') is not None:
             self.enable_internet_address_service = m.get('EnableInternetAddressService')
         if m.get('EnableReadWriteSplit') is not None:
             self.enable_read_write_split = m.get('EnableReadWriteSplit')
         if m.get('InstanceType') is not None:
@@ -13131,17 +13122,17 @@
 
 class DescribeTenantResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant: DescribeTenantResponseBodyTenant = None,
     ):
-        # The request ID.
+        # The zone information of the tenant.
         self.request_id = request_id
-        # The information of the tenant.
+        # The ID of the zone.
         self.tenant = tenant
 
     def validate(self):
         if self.tenant:
             self.tenant.validate()
 
     def to_map(self):
@@ -13219,41 +13210,28 @@
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
         tenant_id: str = None,
         tenant_id_list: str = None,
         tenant_name: str = None,
     ):
-        # The end time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time
-        # The ID of the OceanBase cluster.
+        # 2021-06-13T15:40:43Z
         self.instance_id = instance_id
-        # The monitoring metrics.   
-        # For more information about supported metrics, see [View tenant statistics](~~212125~~).
+        # {"name":"DescribeTenantMetrics","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeTenantMetrics\"},{\"name\":\"InstanceId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"ob317v4uif****\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"TenantName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":true,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"pay_online\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:45:43Z\"},{\"name\":\"Metrics\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tps\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":true,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tfafd34fs****\"},{\"name\":\"TenantIdList\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"[tdak3nac****,tdakc42df****]\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"9\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C\"},{\"name\":\"TenantMetrics\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\\\"Metrics\\\":[ {\\\"request_queue_rt\\\":0.0,\\\"TimeStamp\\\":\\\"2022-02-23T01:58:00Z\\\"}]\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.metrics = metrics
-        # The number of the page to return.    
-        # - Start value: 1 
-        # - Default value: 1
+        # The ID of the OceanBase cluster.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # tfafd34fs****\
         self.page_size = page_size
-        # The start time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # Example 1
         self.start_time = start_time
-        # The ID of the tenant.   
-        # > <br>This parameter will be deprecated. We recommend that you use the TenantIdList parameter instead.
         self.tenant_id = tenant_id
-        # The list of tenant IDs.
         self.tenant_id_list = tenant_id_list
-        # The name of the tenant.    
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.   
-        # > <br>This parameter will be deprecated. We recommend that you use the TenantIdList parameter instead.
+        # 2021-06-13T15:45:43Z
         self.tenant_name = tenant_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13307,19 +13285,16 @@
 class DescribeTenantMetricsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_metrics: str = None,
         total_count: int = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The metrics of the tenant.
         self.tenant_metrics = tenant_metrics
-        # The total count.
         self.total_count = total_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13818,23 +13793,15 @@
 
 class DescribeTenantUserRolesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         role: List[str] = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The list of roles of the user.   
-        # Valid values: 
-        # 
-        # ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.
-        # ReadOnly: a role that has only the read-only privilege SELECT.
-        # DDL: a role that has DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.
-        # DML: a role that has DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.role = role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13906,26 +13873,24 @@
         self,
         page_number: int = None,
         page_size: int = None,
         search_key: str = None,
         tenant_id: str = None,
         user_name: str = None,
     ):
-        # The number of the page to return.    
-        # Start value: 1. Default value: 1.
+        # The database privileges of the account.
         self.page_number = page_number
-        # The number of rows to return on each page.    
-        # Maximum value: 100. Default value: 10.
+        # The return result of the request.
         self.page_size = page_size
-        # The search keyword.
+        # The return result of the request.
         self.search_key = search_key
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTenantUsers**.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13963,29 +13928,16 @@
 class DescribeTenantUsersResponseBodyTenantUsersDatabases(TeaModel):
     def __init__(
         self,
         database: str = None,
         role: str = None,
         table: str = None,
     ):
-        # The name of the database (MySQL mode) or schema (Oracle mode).
         self.database = database
-        # The role of the account.   
-        # In Oracle mode, a role is a schema-level role. Valid values:  
-        # - ReadWrite: a role that has the read and write privileges, including: CREATE TABLE, CREATE VIEW, CREATE PROCEDURE, CREATE SYNONYM, CREATE SEQUENCE, CREATE TRIGGER, CREATE TYPE, CREATE SESSION, EXECUTE ANY PROCEDURE, CREATE ANY OUTLINE, ALTER ANY OUTLINE, DROP ANY OUTLINE, CREATE ANY PROCEDURE, ALTER ANY PROCEDURE, DROP ANY PROCEDURE, CREATE ANY SEQUENCE, ALTER ANY SEQUENCE, DROP ANY SEQUENCE, CREATE ANY TYPE, ALTER ANY TYPE, DROP ANY TYPE, SYSKM, CREATE ANY TRIGGER, ALTER ANY TRIGGER, DROP ANY TRIGGER, CREATE PROFILE, ALTER PROFILE, and DROP PROFILE.  
-        # - ReadOnly: a role that has only the read-only privilege SELECT.
-        # In MySQL mode, a role is a database-level role. Valid values: 
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.   
-        # - ReadOnly: a role that has only the read-only privilege SELECT.   
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.   
-        # 
-        # > <br>By default, an Oracle account has the read and write privileges on its own schema, which are not listed here.
         self.role = role
-        # The name of the table.
         self.table = table
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14019,29 +13971,22 @@
         description: str = None,
         instance_id: str = None,
         tenant_id: str = None,
         user_name: str = None,
         user_status: str = None,
         user_type: str = None,
     ):
-        # The database privileges of the account.
         self.databases = databases
-        # The description of the database account.
         self.description = description
+        # 所属集群Id
         self.instance_id = instance_id
+        # 所属租户Id
         self.tenant_id = tenant_id
-        # The name of the database account.
         self.user_name = user_name
-        # The status of the database account. Valid values:   
-        #  - LOCKED: The account is locked.   
-        # - NORMAL: The account is unlocked.
         self.user_status = user_status
-        # The type of the database account. Valid values:    
-        # - Admin: the super administrator account.   
-        # - NORMAL: a general account.
         self.user_type = user_type
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -14095,19 +14040,31 @@
 class DescribeTenantUsersResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_users: List[DescribeTenantUsersResponseBodyTenantUsers] = None,
         total_count: int = None,
     ):
-        # The request ID.
+        # The name of the database account.
         self.request_id = request_id
-        # The list of database accounts in the tenant.
+        # The type of the database account. Valid values:    
+        # - Admin: the super administrator account.   
+        # - NORMAL: a general account.
         self.tenant_users = tenant_users
-        # The total number of database accounts in the tenant.
+        # The role of the account.   
+        # In Oracle mode, a role is a schema-level role. Valid values:  
+        # - ReadWrite: a role that has the read and write privileges, including: CREATE TABLE, CREATE VIEW, CREATE PROCEDURE, CREATE SYNONYM, CREATE SEQUENCE, CREATE TRIGGER, CREATE TYPE, CREATE SESSION, EXECUTE ANY PROCEDURE, CREATE ANY OUTLINE, ALTER ANY OUTLINE, DROP ANY OUTLINE, CREATE ANY PROCEDURE, ALTER ANY PROCEDURE, DROP ANY PROCEDURE, CREATE ANY SEQUENCE, ALTER ANY SEQUENCE, DROP ANY SEQUENCE, CREATE ANY TYPE, ALTER ANY TYPE, DROP ANY TYPE, SYSKM, CREATE ANY TRIGGER, ALTER ANY TRIGGER, DROP ANY TRIGGER, CREATE PROFILE, ALTER PROFILE, and DROP PROFILE.  
+        # - ReadOnly: a role that has only the read-only privilege SELECT.
+        # In MySQL mode, a role is a database-level role. Valid values: 
+        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.   
+        # - ReadOnly: a role that has only the read-only privilege SELECT.   
+        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
+        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.   
+        # 
+        # > <br>By default, an Oracle account has the read and write privileges on its own schema, which are not listed here.
         self.total_count = total_count
 
     def validate(self):
         if self.tenant_users:
             for k in self.tenant_users:
                 if k:
                     k.validate()
@@ -14188,17 +14145,17 @@
 
 class DescribeTenantZonesReadRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The zone information of the tenant.
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14226,23 +14183,19 @@
         self,
         is_electable: bool = None,
         is_primary: bool = None,
         is_read_only_address_master: bool = None,
         is_readable: str = None,
         zone: str = None,
     ):
-        # Indicates whether the zone can be set as the primary zone.
+        # Example 1
         self.is_electable = is_electable
-        # Indicates whether the zone is the primary zone.
         self.is_primary = is_primary
-        # Indicates whether a read-only connection has been created.
         self.is_read_only_address_master = is_read_only_address_master
-        # Indicates whether a read-only connection needs to be created for the zone.
         self.is_readable = is_readable
-        # The ID of the zone.
         self.zone = zone
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14279,17 +14232,17 @@
 
 class DescribeTenantZonesReadResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_zones: List[DescribeTenantZonesReadResponseBodyTenantZones] = None,
     ):
-        # The request ID.
+        # Indicates whether a read-only connection needs to be created for the zone.
         self.request_id = request_id
-        # The zone information of the tenant.
+        # The request ID.
         self.tenant_zones = tenant_zones
 
     def validate(self):
         if self.tenant_zones:
             for k in self.tenant_zones:
                 if k:
                     k.validate()
@@ -14370,30 +14323,25 @@
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         search_key: str = None,
         tenant_id: str = None,
         tenant_name: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The number of used disks of the tenant.
         self.instance_id = instance_id
-        # The number of the page to return.   
-        # Start value: 1
-        # - Default value: 1
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100.
-        # - Default value: 10
+        # You can call this operation to query the tenants in an OceanBase cluster.
         self.page_size = page_size
-        # The search keyword.
+        # The primary zone of the tenant.
         self.search_key = search_key
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id
-        # The name of the tenant.   
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
+        # The information of tenants.
         self.tenant_name = tenant_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14454,63 +14402,74 @@
         used_disk_size: float = None,
         vpc_id: str = None,
     ):
         self.charset = charset
         self.collation = collation
         # The total number of CPU cores of the tenant.
         self.cpu = cpu
-        # The time when the tenant was created.
+        # The number of CPU cores in each resource unit of the tenant.
         self.create_time = create_time
-        # The data replica distribution mode of the tenant.   
-        # 
-        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
-        # - For the basic version, N indicates the single-zone mode. 
-        # 
-        # > <br>N represents the number of nodes in a single zone.
+        # The search keyword.
         self.deploy_mode = deploy_mode
-        # The deployment type of the tenant. <br>
-        # - multiple: multi-IDC deployment
-        # - single: single-IDC deployment
-        # - dual: dual-IDC deployment
+        # The name of the tenant.   
+        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
         self.deploy_type = deploy_type
-        # The description of the tenant.
+        # Example 1
         self.description = description
-        # The total memory size of the tenant, in GB.
+        # The number of the page to return.   
+        # Start value: 1
+        # - Default value: 1
         self.mem = mem
-        # The primary zone of the tenant.
+        # The return result of the request.
         self.primary_zone = primary_zone
         # The status of the tenant.  <br>
         # - PENDING_CREATE: The tenant is being created.
         # - RESTORE: The tenant is being recovered.
         # - ONLINE: The tenant is running.
         # - SPEC_MODIFYING: The specification of the tenant is being modified.
         # ALLOCATING_INTERNET_ADDRESS: An Internet address is being allocated.
         # PENDING_OFFLINE_INTERNET_ADDRESS: The Internet address is being disabled.
         # - PRIMARY_ZONE_MODIFYING: The tenant is switching to a new primary zone.
         # - PARAMETER_MODIFYING: Parameters are being modified.
         # - WHITE_LIST_MODIFYING: The whitelist is being modified.
         self.status = status
-        # The ID of the tenant.
+        # You can call this operation to query the tenants in an OceanBase cluster.
         self.tenant_id = tenant_id
-        # The tenant mode.   
-        # Valid values:   
-        # Oracle
-        # MySQL
+        # {
+        #     "TotalCount": 1,
+        #     "RequestId": "EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C",
+        #     "Tenants": [
+        #         {
+        #             "VpcId": "vpc-bp1d2q3mhg9i23ofi****",
+        #             "Status": "ONLINE",
+        #             "PrimaryZone": "cn-hangzhou-i",
+        #             "DeployType": "multiple",
+        #             "DeployMode": "1-1-1",
+        #             "CreateTime": "2021-09-17 15:52:17.0",
+        #             "TenantName": "pay_online",
+        #             "Mem": 20,
+        #             "Cpu": 10,
+        #             "Description": "PayCore business database",
+        #             "TenantMode": "Oracle",
+        #             "TenantId": "t33h8y08k****",
+        #             "UnitCpu": 5,
+        #             "UnitMem": 10,
+        #             "UnitNum": 2,
+        #             "UsedDiskSize": 10
+        #         }
+        #     ]
+        # }
         self.tenant_mode = tenant_mode
-        # The name of the tenant.
+        # The information of tenants.
         self.tenant_name = tenant_name
-        # The number of CPU cores in each resource unit of the tenant.
         self.unit_cpu = unit_cpu
-        # The memory size of each resource unit of the tenant, in GB.
         self.unit_mem = unit_mem
-        # The number of resource units in the tenant.
         self.unit_num = unit_num
-        # The number of used disks of the tenant.
         self.used_disk_size = used_disk_size
-        # The ID of the VPC.   <br>If no suitable VPC is available, create a VPC as prompted. For more information, see "What is a VPC".
+        # The time when the tenant was created.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14600,19 +14559,19 @@
 class DescribeTenantsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenants: List[DescribeTenantsResponseBodyTenants] = None,
         total_count: int = None,
     ):
-        # The request ID.
+        # The ID of the tenant.
         self.request_id = request_id
-        # The information of tenants.
+        # The ID of the OceanBase cluster.
         self.tenants = tenants
-        # The total number of tenants in the specified OceanBase cluster.
+        # The total memory size of the tenant, in GB.
         self.total_count = total_count
 
     def validate(self):
         if self.tenants:
             for k in self.tenants:
                 if k:
                     k.validate()
@@ -14693,17 +14652,18 @@
 
 class DescribeTimeZonesResponseBodyTimeZonesList(TeaModel):
     def __init__(
         self,
         description: str = None,
         time_zone: str = None,
     ):
-        # The description of the time zone.
+        # Example 1
         self.description = description
-        # The name of the time zone.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTimeZones**.
         self.time_zone = time_zone
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14728,15 +14688,14 @@
 
 class DescribeTimeZonesResponseBodyTimeZones(TeaModel):
     def __init__(
         self,
         default: str = None,
         list: List[DescribeTimeZonesResponseBodyTimeZonesList] = None,
     ):
-        # The default time zone.
         self.default = default
         # The list of time zones.
         self.list = list
 
     def validate(self):
         if self.list:
             for k in self.list:
@@ -14771,17 +14730,17 @@
 
 class DescribeTimeZonesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         time_zones: DescribeTimeZonesResponseBodyTimeZones = None,
     ):
-        # The request ID.
+        # DescribeTimeZones
         self.request_id = request_id
-        # The time zones supported by the tenant.
+        # The description of the time zone.
         self.time_zones = time_zones
 
     def validate(self):
         if self.time_zones:
             self.time_zones.validate()
 
     def to_map(self):
@@ -14865,49 +14824,46 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.
+        # The number of block index cache hits.
         self.db_name = db_name
-        # The end time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The SQL type.
         self.end_time = end_time
-        # The filter condition.
+        # The average number of logical reads of the SQL statement during the specified period of time.   
+        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
+        # 
+        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
         self.filter_condition = filter_condition
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The queuing time, in ms.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of row cache hits.
         self.page_size = page_size
-        # SQLID.
+        # The I/O wait time, in ms.
         self.sqlid = sqlid
-        # The search keyword.
+        # The number of retries.
         self.search_key_word = search_key_word
-        # The search parameter.
+        # SQLID.
         self.search_parameter = search_parameter
-        # The search rule.
+        # The IP address of the client.
         self.search_rule = search_rule
-        # The search value.
+        # The number of Bloom filter cache hits.
         self.search_value = search_value
-        # The sorted column.
+        # The number of rows read from the disk.
         self.sort_column = sort_column
-        # The sorting rule.
+        # The list of top SQL statements.
         self.sort_order = sort_order
-        # The start time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time, in ms.
         self.start_time = start_time
-        # The ID of the tenant.
+        # The average CPU time, in ms.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14997,49 +14953,46 @@
         search_rule: str = None,
         search_value: str = None,
         sort_column: str = None,
         sort_order: str = None,
         start_time: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.
+        # The number of block index cache hits.
         self.db_name = db_name
-        # The end time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The SQL type.
         self.end_time = end_time
-        # The filter condition.
+        # The average number of logical reads of the SQL statement during the specified period of time.   
+        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
+        # 
+        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
         self.filter_condition_shrink = filter_condition_shrink
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The queuing time, in ms.
         self.page_number = page_number
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of row cache hits.
         self.page_size = page_size
-        # SQLID.
+        # The I/O wait time, in ms.
         self.sqlid = sqlid
-        # The search keyword.
+        # The number of retries.
         self.search_key_word = search_key_word
-        # The search parameter.
+        # SQLID.
         self.search_parameter = search_parameter
-        # The search rule.
+        # The IP address of the client.
         self.search_rule = search_rule
-        # The search value.
+        # The number of Bloom filter cache hits.
         self.search_value = search_value
-        # The sorted column.
+        # The number of rows read from the disk.
         self.sort_column = sort_column
-        # The sorting rule.
+        # The list of top SQL statements.
         self.sort_order = sort_order
-        # The start time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time, in ms.
         self.start_time = start_time
-        # The ID of the tenant.
+        # The average CPU time, in ms.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15154,96 +15107,114 @@
         sqltext: str = None,
         sqltype: int = None,
         schedule_time: float = None,
         ssstore_read_row_count: int = None,
         total_wait_time: float = None,
         user_name: str = None,
     ):
-        # The number of rows affected.
+        # The internal wait time, in ms.
         self.affected_rows = affected_rows
-        # The wait time of the client, in ms.
+        # The wait time in concurrent execution, in ms.
         self.app_wait_time = app_wait_time
-        # The number of block cache hits.
+        # The average CPU time, in ms.
         self.block_cache_hit = block_cache_hit
-        # The number of block index cache hits.
+        # $.parameters[16].schema.example
         self.block_index_cache_hit = block_index_cache_hit
-        # The number of Bloom filter cache hits.
+        # $.parameters[14].schema.enumValueTitles
         self.bloom_filter_cache_hit = bloom_filter_cache_hit
-        # The IP address of the client.
+        # $.parameters[14].schema.description
         self.client_ip = client_ip
-        # The wait time in concurrent execution, in ms.
+        # The number of rows returned.
         self.concurrency_wait_time = concurrency_wait_time
-        # The average CPU time, in ms.
+        # The maximum CPU time, in ms.
         self.cpu_time = cpu_time
-        # The name of the database.
+        # The number of remote plans.
         self.db_name = db_name
-        # The time to wait for decoding, in ms.
+        # The number of rows to return on each page.   
+        # - Maximum value: 100   
+        # - Default value: 10
         self.decode_time = decode_time
-        # The number of physical reads.
+        # The IP address of the client.
         self.disk_read = disk_read
-        # The average response time, in ms.
+        # The sorting rule.
         self.elapsed_time = elapsed_time
-        # The wait event.
+        # The number of rows read from the disk.
         self.event = event
-        # The number of executions per second.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTopSQLList**.
         self.exec_per_second = exec_per_second
-        # The internal execution time, in ms.
+        # The number of rows read from the memory.
         self.execute_time = execute_time
-        # The number of executions.
+        # The number of executions per second.
         self.executions = executions
-        # The number of failures.
+        # $.parameters[12].schema.description
         self.fail_times = fail_times
-        # The time spent in hard parsing, in ms.
+        # The queuing time, in ms.
         self.get_plan_time = get_plan_time
-        # The I/O wait time, in ms.
+        # $.parameters[15].schema.example
         self.iowait_time = iowait_time
-        # The sequence number of the returned SQL statement.
+        # The name of the database.
         self.key = key
-        # The average number of logical reads of the SQL statement during the specified period of time.   
-        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
-        # 
-        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
+        # You can call this operation to query SQL execution performance data collected by the diagnostic system.
         self.logical_read = logical_read
-        # The maximum CPU time, in ms.
+        # SQLID.
         self.max_cpu_time = max_cpu_time
-        # The maximum response time, in ms.
+        # The sequence number of the returned SQL statement.
         self.max_elapsed_time = max_elapsed_time
-        # The number of rows read from the memory.
+        # The name of the database.
         self.memstore_read_row_count = memstore_read_row_count
-        # The number of plan misses.
+        # The total count.
         self.miss_plans = miss_plans
-        # The network latency, in ms.
+        # The end time of the time range for querying TOP SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.net_wait_time = net_wait_time
-        # The IP address of the node.
+        # The username.
         self.node_ip = node_ip
-        # The queuing time, in ms.
+        # $.parameters[12].schema.enumValueTitles
         self.queue_time = queue_time
-        # The number of RPCs.
+        # The start time of the time range for querying TOP SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.rpccount = rpccount
-        # The number of remote plans.
+        # The return result of the request.
         self.remote_plans = remote_plans
-        # The number of retries.
+        # $.parameters[13].schema.description
         self.retry_count = retry_count
-        # The number of rows returned.
+        # The wait event.
         self.return_rows = return_rows
-        # The number of row cache hits.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeTopSQLList
+        # &TenantId=t2mr3oae0****\
+        # &StartTime=2021-06-13 15:40:43
+        # &EndTime=2021-09-13 15:40:43
+        # &DbName=testdb
+        # &SearchKeyWord=update
+        # &SearchParameter=cputime
+        # &SearchRule=>
+        # &SearchValue=0.01
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &NodeIp=i-bp19y05uq6xpacyqnlrc
+        # &PageNumber=1
+        # &PageSize=10
+        # &SortColumn=cputime
+        # &SortOrder=desc
+        # &Common request parameters
+        # ```
         self.row_cache_hit = row_cache_hit
-        # SQLID.
+        # $.parameters[13].schema.example
         self.sqlid = sqlid
-        # The SQL text.
+        # The list of top SQL statements.
         self.sqltext = sqltext
-        # The SQL type.
+        # The request ID.
         self.sqltype = sqltype
-        # The scheduling duration, in ms.
+        # The search keyword.
         self.schedule_time = schedule_time
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count
-        # The internal wait time, in ms.
+        # -\
         self.total_wait_time = total_wait_time
-        # The username.
+        # The number of Bloom filter cache hits.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15421,19 +15392,19 @@
 class DescribeTopSQLListResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         top_sqllist: List[DescribeTopSQLListResponseBodyTopSQLList] = None,
         total_count: int = None,
     ):
-        # The request ID.
+        # Alibaba Cloud CLI
         self.request_id = request_id
-        # The list of top SQL statements.
+        # The I/O wait time, in ms.
         self.top_sqllist = top_sqllist
-        # The total count.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.total_count = total_count
 
     def validate(self):
         if self.top_sqllist:
             for k in self.top_sqllist:
                 if k:
                     k.validate()
@@ -15514,21 +15485,18 @@
 
 class DescribeZonesRequest(TeaModel):
     def __init__(
         self,
         deploy_type: str = None,
         series: str = None,
     ):
-        # The deployment type of the cluster. Valid values:   
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The operation that you want to perform.   
+        # Set the value to **DescribeZones**.
         self.deploy_type = deploy_type
-        # The series of the OceanBase cluster. Valid values:   
-        # NORMAL: the high availability version. This is the default value.
+        # The deployment mode.
         self.series = series
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15555,23 +15523,17 @@
     def __init__(
         self,
         deploy_type: str = None,
         series: str = None,
         zone_id: str = None,
         zone_name: str = None,
     ):
-        # The deployment mode.
         self.deploy_type = deploy_type
-        # The series of the OceanBase cluster. Valid values:   
-        # NORMAL: the high availability version. This is the default value.
         self.series = series
-        # The list of zone IDs.   
-        # For a cluster with multiple zones, separate the zone names with commas (,).
         self.zone_id = zone_id
-        # The name of the zone.
         self.zone_name = zone_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15604,17 +15566,22 @@
 
 class DescribeZonesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         zones: List[DescribeZonesResponseBodyZones] = None,
     ):
-        # The request ID.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeZones
+        # &Series=normal
+        # &DeployType=single
+        # &Common request parameters
+        # ```
         self.request_id = request_id
-        # The list of zones.
+        # You can call this operation to learn of zones where a cluster can be created in an Alibaba Cloud region.
         self.zones = zones
 
     def validate(self):
         if self.zones:
             for k in self.zones:
                 if k:
                     k.validate()
@@ -15685,30 +15652,256 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeZonesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class KillProcessListRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        session_list: str = None,
+        tenant_id: str = None,
+    ):
+        # The ID of the OceanBase cluster.
+        self.instance_id = instance_id
+        # The list of the sessions that need to be closed.
+        self.session_list = session_list
+        # The ID of the tenant.
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.session_list is not None:
+            result['SessionList'] = self.session_list
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SessionList') is not None:
+            self.session_list = m.get('SessionList')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class KillProcessListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        client_ip: str = None,
+        command: str = None,
+        database: str = None,
+        error_message: str = None,
+        execute_time: str = None,
+        server_ip: str = None,
+        session_id: int = None,
+        sql_text: str = None,
+        status: str = None,
+        tenant_id: str = None,
+        user: str = None,
+    ):
+        # The client IP address.
+        self.client_ip = client_ip
+        # The start command for the container of the application.
+        self.command = command
+        # The name of the database.
+        self.database = database
+        # The error message.
+        self.error_message = error_message
+        # Execution time (UTC+8). If it is left empty, it means to execute immediately.
+        self.execute_time = execute_time
+        # The IP address of the server.
+        self.server_ip = server_ip
+        # The ID of the session.
+        self.session_id = session_id
+        # The SQL statement.
+        self.sql_text = sql_text
+        # The status of the task.
+        self.status = status
+        # The ID of the tenant.
+        self.tenant_id = tenant_id
+        # The database username.
+        self.user = user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.command is not None:
+            result['Command'] = self.command
+        if self.database is not None:
+            result['Database'] = self.database
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.execute_time is not None:
+            result['ExecuteTime'] = self.execute_time
+        if self.server_ip is not None:
+            result['ServerIp'] = self.server_ip
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        if self.sql_text is not None:
+            result['SqlText'] = self.sql_text
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('Command') is not None:
+            self.command = m.get('Command')
+        if m.get('Database') is not None:
+            self.database = m.get('Database')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('ExecuteTime') is not None:
+            self.execute_time = m.get('ExecuteTime')
+        if m.get('ServerIp') is not None:
+            self.server_ip = m.get('ServerIp')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        if m.get('SqlText') is not None:
+            self.sql_text = m.get('SqlText')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class KillProcessListResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[KillProcessListResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        # The data returned.
+        self.data = data
+        # The request ID.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = KillProcessListResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class KillProcessListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: KillProcessListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = KillProcessListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyDatabaseDescriptionRequest(TeaModel):
     def __init__(
         self,
         database_name: str = None,
         description: str = None,
         instance_id: str = None,
         tenant_id: str = None,
     ):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # Example 1
         self.database_name = database_name
-        # The description of the database.
         self.description = description
-        # The ID of the OceanBase cluster.
+        # The description of the database.
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyDatabaseDescription**.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15740,15 +15933,14 @@
 
 
 class ModifyDatabaseDescriptionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15815,22 +16007,21 @@
     def __init__(
         self,
         database_name: str = None,
         instance_id: str = None,
         tenant_id: str = None,
         users: str = None,
     ):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # The ID of the tenant.
         self.database_name = database_name
-        # The ID of the OceanBase cluster.
+        # The account information.
         self.instance_id = instance_id
-        # The ID of the tenant.
-        self.tenant_id = tenant_id
         # A list of usernames and their respective roles.
+        self.tenant_id = tenant_id
+        # The ID of the OceanBase cluster.
         self.users = users
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15863,22 +16054,15 @@
 
 class ModifyDatabaseUserRolesResponseBodyTenantUserUsers(TeaModel):
     def __init__(
         self,
         role: str = None,
         user_name: str = None,
     ):
-        # The role of the account.   
-        # In MySQL mode, a role is a database-level role. Valid values:
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.
-        # - ReadOnly: a role that has only the read-only privilege SELECT. 
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW. 
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.role = role
-        # The name of the account.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15904,19 +16088,17 @@
 class ModifyDatabaseUserRolesResponseBodyTenantUser(TeaModel):
     def __init__(
         self,
         database_name: str = None,
         tenant_id: str = None,
         users: List[ModifyDatabaseUserRolesResponseBodyTenantUserUsers] = None,
     ):
-        # The name of the database.
+        # Example 1
         self.database_name = database_name
-        # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The accounts that have privileges on the database.
         self.users = users
 
     def validate(self):
         if self.users:
             for k in self.users:
                 if k:
                     k.validate()
@@ -15953,17 +16135,16 @@
 
 class ModifyDatabaseUserRolesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_user: ModifyDatabaseUserRolesResponseBodyTenantUser = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The account information.
+        # The name of the database.
         self.tenant_user = tenant_user
 
     def validate(self):
         if self.tenant_user:
             self.tenant_user.validate()
 
     def to_map(self):
@@ -16034,18 +16215,17 @@
 
 class ModifyInstanceNameRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         instance_name: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.instance_id = instance_id
-        # The name of the OceanBase cluster.   
-        # It must be 1 to 20 characters in length.
+        # The ID of the OceanBase cluster.
         self.instance_name = instance_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16072,15 +16252,16 @@
     def __init__(
         self,
         instance_name: str = None,
         request_id: str = None,
     ):
         # The name of the OceanBase cluster.
         self.instance_name = instance_name
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyInstanceName**.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16433,17 +16614,17 @@
 
 class ModifyInstanceTagsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tags: str = None,
     ):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id
         # The tags.
+        self.instance_id = instance_id
+        # You can call this operation to modify the value of the cluster tags.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16468,17 +16649,15 @@
 
 class ModifyInstanceTagsResponseBody(TeaModel):
     def __init__(
         self,
         message: str = None,
         request_id: str = None,
     ):
-        # The update status of the tags.
         self.message = message
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16549,26 +16728,22 @@
     def __init__(
         self,
         dimension: str = None,
         dimension_value: str = None,
         instance_id: str = None,
         parameters: str = None,
     ):
-        # The type of the parameter.   
-        # Valid values: CLUSTER and TENANT.
+        # The ID of the OceanBase cluster.
         self.dimension = dimension
-        # The resource ID of the parameter type.    
-        # You can leave this parameter unspecified when you call this operation to modify cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # The cause of the modification failure.
         self.dimension_value = dimension_value
-        # The ID of the OceanBase cluster.
+        # Alibaba Cloud CLI
         self.instance_id = instance_id
-        # The parameters.   
-        # It is a JSON array. Each object in the array has two elements: Name and Value. 
-        # 
-        # > <br>The names and values of cluster parameters that can be modified are different from those of tenant parameters. For more information, see DescribeParameters.
+        # The resource ID of the parameter type.    
+        # You can leave this parameter unspecified when you call this operation to modify cluster parameters. In the case of tenant parameters, pass the tenant ID.
         self.parameters = parameters
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16601,19 +16776,15 @@
 
 class ModifyParametersResponseBodyResults(TeaModel):
     def __init__(
         self,
         message: str = None,
         success: bool = None,
     ):
-        # The cause of the modification failure.
         self.message = message
-        # Indicates whether the parameter has been modified. Valid values:   
-        # true: The modification is successful. 
-        # false: The modification failed.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16638,17 +16809,18 @@
 
 class ModifyParametersResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         results: ModifyParametersResponseBodyResults = None,
     ):
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyParameters**.
         self.request_id = request_id
-        # The modification results.
+        # Example 1
         self.results = results
 
     def validate(self):
         if self.results:
             self.results.validate()
 
     def to_map(self):
@@ -16722,16 +16894,15 @@
         self,
         instance_id: str = None,
         security_ip_group_name: str = None,
         security_ips: str = None,
     ):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The name of the IP address whitelist group.   
-        # It must be 2 to 32 characters in length, start with a lowercase letter, end with a lowercase letter or digit, and contain only lowercase letters, digits, and underscores (_).
+        # The information of the IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name
         # The list of IP addresses and CIDR blocks in the whitelist.   
         # It is a JSON array. Each object in the array is an IP address or CIDR block. You can specify at most 40 IP addresses or CIDR blocks.
         self.security_ips = security_ips
 
     def validate(self):
         pass
@@ -16764,20 +16935,16 @@
 class ModifySecurityIpsResponseBodySecurityIpGroup(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         security_ip_group_name: str = None,
         security_ips: str = None,
     ):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id
-        # The name of the security group.
         self.security_ip_group_name = security_ip_group_name
-        # The list of IP addresses and CIDR blocks in the whitelist.   
-        # The return values of SecurityIps are strings that are separated with commas (,).
         self.security_ips = security_ips
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16808,15 +16975,15 @@
     def __init__(
         self,
         request_id: str = None,
         security_ip_group: ModifySecurityIpsResponseBodySecurityIpGroup = None,
     ):
         # The request ID.
         self.request_id = request_id
-        # The information of the IP address whitelist group.
+        # Example 1
         self.security_ip_group = security_ip_group
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -16892,28 +17059,34 @@
         master_intranet_address_zone: str = None,
         modify_type: str = None,
         primary_zone: str = None,
         primary_zone_deploy_type: str = None,
         tenant_id: str = None,
         user_vswitch_id: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The primary zone of the tenant.    
+        # It is one of the zones in which the cluster is deployed.
         self.instance_id = instance_id
-        # The availability zone where the primary node is located.
+        # ```
+        # http(s)://[Endpoint]/?Action=ModifyTenantPrimaryZone
+        # &TenantId=ob2mr3oae0****\
+        # &InstanceId=ob317v4uif****\
+        # &PrimaryZone=cn-hangzhou-h
+        # &Common request parameters
+        # ```
         self.master_intranet_address_zone = master_intranet_address_zone
         # The switching mode.
         self.modify_type = modify_type
-        # The primary zone of the tenant.    
-        # It is one of the zones in which the cluster is deployed.
+        # The ID of the vSwitch.
         self.primary_zone = primary_zone
-        # The deployment type of the primary zone.
+        # Example 1
         self.primary_zone_deploy_type = primary_zone_deploy_type
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id
-        # The ID of the vSwitch.
+        # The request ID.
         self.user_vswitch_id = user_vswitch_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16957,15 +17130,14 @@
 
 
 class ModifyTenantPrimaryZoneResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17032,21 +17204,22 @@
     def __init__(
         self,
         cpu: int = None,
         instance_id: str = None,
         memory: int = None,
         tenant_id: str = None,
     ):
-        # The information about the CPU resources of the tenant.
+        # The memory size of the tenant, in GB.
         self.cpu = cpu
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantResource**.
         self.instance_id = instance_id
-        # The memory size of the tenant, in GB.
-        self.memory = memory
         # The ID of the tenant.
+        self.memory = memory
+        # The information about the CPU resources of the tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17079,17 +17252,15 @@
 
 class ModifyTenantResourceResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The ID of the tenant.
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17276,22 +17447,22 @@
     def __init__(
         self,
         description: str = None,
         instance_id: str = None,
         tenant_id: str = None,
         user_name: str = None,
     ):
-        # The description of the database.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserDescription**.
         self.description = description
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
         # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
+        # The description of the database.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17323,15 +17494,15 @@
 
 
 class ModifyTenantUserDescriptionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
+        # You can call this operation to modify the description of a specified account in a tenant.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17393,51 +17564,62 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantUserPasswordRequest(TeaModel):
     def __init__(
         self,
+        encryption_type: str = None,
         instance_id: str = None,
         tenant_id: str = None,
         user_name: str = None,
         user_password: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # 加密方式。
+        self.encryption_type = encryption_type
         self.instance_id = instance_id
-        # The ID of the tenant.
+        # ```
+        # http(s)://[Endpoint]/?Action=ModifyTenantUserPassword
+        # &UserName=pay_test
+        # &TenantId=ob2mr3oae0****\
+        # &UserPassword=!Aliyun4Oceanbase
+        # &InstanceId=ob317v4uif****\
+        # &Common request parameters
+        # ```
         self.tenant_id = tenant_id
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The ID of the OceanBase cluster.
         self.user_name = user_name
-        # The password of the database account.    
-        # It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % \ ^ \ & \ * ( ) _ + - =\
+        # You can call this operation to change the logon password of a specified account in a tenant.
         self.user_password = user_password
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.encryption_type is not None:
+            result['EncryptionType'] = self.encryption_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.user_name is not None:
             result['UserName'] = self.user_name
         if self.user_password is not None:
             result['UserPassword'] = self.user_password
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('EncryptionType') is not None:
+            self.encryption_type = m.get('EncryptionType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         if m.get('UserPassword') is not None:
@@ -17446,15 +17628,14 @@
 
 
 class ModifyTenantUserPasswordResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17522,28 +17703,30 @@
         self,
         instance_id: str = None,
         modify_type: str = None,
         tenant_id: str = None,
         user_name: str = None,
         user_role: str = None,
     ):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id
         # The type of the privilege modification operation.   
         # Valid values:  
         # update: updates all privileges. This is the default value.  
         # add: adds a privilege.  
         # delete: deletes a privilege.
+        self.instance_id = instance_id
+        # The name of the table.
         self.modify_type = modify_type
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserRoles**.
         self.tenant_id = tenant_id
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
-        self.user_name = user_name
         # The role of the database account.
+        self.user_name = user_name
+        # The type of the account. Valid values:   
+        # - Admin: the super administrator account.   
+        # - Normal: a general account.
         self.user_role = user_role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17582,21 +17765,27 @@
     def __init__(
         self,
         database: str = None,
         is_success: bool = None,
         role: str = None,
         table: str = None,
     ):
-        # The name of the database (MySQL mode) or schema (Oracle mode).
+        # ```
+        # http(s)://[Endpoint]/?Action=ModifyTenantUserRoles
+        # &UserName=pay_test
+        # &TenantId=ob2mr3oae0****\
+        # &UserRole=[{"Database":"20210824160559","Role":"readwrite"}]
+        # &InstanceId=ob317v4uif****\
+        # &ModifyType=update
+        # &Common request parameters
+        # ```
         self.database = database
-        # Indicates whether the privilege was granted to the role.
         self.is_success = is_success
-        # The role of the account.
+        # You can call this operation to modify the database privileges of a specified account in a tenant.
         self.role = role
-        # The name of the table.
         self.table = table
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17630,21 +17819,17 @@
 class ModifyTenantUserRolesResponseBodyTenantUser(TeaModel):
     def __init__(
         self,
         tenant_id: str = None,
         user_name: str = None,
         user_role: List[ModifyTenantUserRolesResponseBodyTenantUserUserRole] = None,
     ):
-        # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The name of the account.
         self.user_name = user_name
-        # The type of the account. Valid values:   
-        # - Admin: the super administrator account.   
-        # - Normal: a general account.
+        # The name of the database (MySQL mode) or schema (Oracle mode).
         self.user_role = user_role
 
     def validate(self):
         if self.user_role:
             for k in self.user_role:
                 if k:
                     k.validate()
@@ -17681,17 +17866,16 @@
 
 class ModifyTenantUserRolesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_user: ModifyTenantUserRolesResponseBodyTenantUser = None,
     ):
-        # The request ID.
         self.request_id = request_id
-        # The list of database accounts in the tenant.
+        # The ID of the tenant.
         self.tenant_user = tenant_user
 
     def validate(self):
         if self.tenant_user:
             self.tenant_user.validate()
 
     def to_map(self):
@@ -17764,20 +17948,20 @@
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
         user_name: str = None,
         user_status: str = None,
     ):
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserStatus**.
         self.instance_id = instance_id
         # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The list of database accounts in the tenant.
         self.user_name = user_name
         # The status of the database account. Valid values:   
         # - Locked: The account is locked. 
         # - Online: The account is unlocked.
         self.user_status = user_status
 
     def validate(self):
@@ -17815,21 +17999,16 @@
 class ModifyTenantUserStatusResponseBodyTenantUser(TeaModel):
     def __init__(
         self,
         tenant_id: str = None,
         user_name: str = None,
         user_status: str = None,
     ):
-        # The ID of the tenant.
         self.tenant_id = tenant_id
-        # The name of the account.
         self.user_name = user_name
-        # The status of the database account. Valid values:   
-        # - LOCKED: The account is locked. 
-        # - ONLINE: The account is unlocked.
         self.user_status = user_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17858,17 +18037,16 @@
 
 class ModifyTenantUserStatusResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tenant_user: List[ModifyTenantUserStatusResponseBodyTenantUser] = None,
     ):
-        # The request ID.
+        # Example 1
         self.request_id = request_id
-        # The list of database accounts in the tenant.
         self.tenant_user = tenant_user
 
     def validate(self):
         if self.tenant_user:
             for k in self.tenant_user:
                 if k:
                     k.validate()
@@ -17947,21 +18125,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17996,21 +18174,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **ReleaseOmsOpenAPIProject**.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level
-        # The error description (new).
+        # The error code (new).
         self.message = message
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18052,35 +18230,29 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # You can call this operation to release a data synchronization project.
         self.advice = advice
-        # The error code (old).
+        # Indicates whether the project is released.
         self.code = code
-        # The time spent, in seconds.
         self.cost = cost
-        # Indicates whether the project is released.
         self.data = data
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail
-        # The error description (old).
+        # A system error occurred.
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -18189,21 +18361,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18238,21 +18410,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **ResetOmsOpenAPIProject**.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level
-        # The error description (new).
+        # The error code (new).
         self.message = message
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18294,35 +18466,29 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # You can call this operation to reset a data synchronization project.
         self.advice = advice
-        # The error code (old).
+        # Indicates whether the resetting is successful.
         self.code = code
-        # The time spent, in seconds.
         self.cost = cost
-        # Indicates whether the resetting is successful.
         self.data = data
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail
-        # The error description (old).
+        # A system error occurred.
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -18431,21 +18597,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # Indicates whether the call is successful.
         self.page_size = page_size
-        # The project ID.
+        # Contact the administrator.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The suggestions (old).
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18480,21 +18646,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The suggestions (new).
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The operation that you want to perform. Set the value to **ResumeOmsOpenAPIProject**.
         self.level = level
-        # The error description (new).
+        # The error description (old).
         self.message = message
-        # The suggestions (new).
+        # The error code (new).
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18536,35 +18702,30 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # The request ID.
         self.advice = advice
-        # The error code (old).
+        # The page number, which takes effect in a pagination query.
         self.code = code
-        # The time spent, in seconds.
         self.cost = cost
-        # Indicates whether the project is resumed.
         self.data = data
-        # The error details.
+        # The page number, which takes effect in a pagination query.
         self.error_detail = error_detail
-        # The error description (old).
+        # The error details.
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
+        # Example 1
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -18677,29 +18838,29 @@
         max_point_num: int = None,
         metric: str = None,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The query start time, which is a second-level timestamp.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.begin_time = begin_time
-        # The query end time, which is a second-level timestamp.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.end_time = end_time
-        # The maximum number of query points.
+        # Contact the administrator.
         self.max_point_num = max_point_num
-        # The query metric. For example, if you want to query the incremental transactions per second (TPS), set the value to CONNECTOR_TPS. Valid values: CONNECTOR_TPS: the TPS of the Connector component; CONNECTOR_DELAY: the latency of the Connector component; CONNECTOR_SOURCE_QUEUE_SIZE: the queue size of the Connector source; CONNECTOR_IOPS: the Connector IOPS; CONNECTOR_WRITE_COST: the time spent in writing at the Connector destination; CONNECTOR_SOURCE_READ_COST: the time spent in reading at the Connector source; JDBCWRITER_DELAY: the latency of the JDBCWriter; JDBCWRITER_IOPS: the IOPS of the JDBCWriter; JDBCWRITER_RPS: the requests per second (RPS) of the JDBCWriter; STORE_DELAY: the latency of the Store component; STORE_CONN: the number of store connections; STORE_IOPS: the IOPS of the Store component; STORE_TPS: the TPS of the Store component; CHECKER_SOURCE_NONE_RPS: the instantaneous RPS of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_RPS: the average RPS of the Checker component at the source end during full migration; CHECKER_DEST_NONE_RPS: the instantaneous RPS of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_RPS: the average RPS of the Checker component at the destination end during full migration; CHECKER_SOURCE_NONE_RT: the instantaneous response time (RT) of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_RT: the average RT of the Checker component at the source end during full migration; CHECKER_DEST_NONE_RT: the instantaneous RT of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_RT: the average RT of the Checker component at the destination end during full migration; CHECKER_SOURCE_NONE_READ_IOPS: the instantaneous read IOPS of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_READ_IOPS: the average read IOPS of the Checker component at the source end during full migration; CHECKER_DEST_NONE_WRITE_IOPS: the instantaneous write IOPS of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_WRITE_IOPS: the average write IOPS of the Checker component at the destination end during full migration; CHECKER_VERIFY_SOURCE_NONE_RPS: the instantaneous RPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_RPS: the average RPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_RPS: the instantaneous RPS of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_DEST_AVG_RPS: the average RPS of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_SOURCE_NONE_RT: the instantaneous RT of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_RT: the average RT of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_RT: the instantaneous RT of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_DEST_AVG_RT: the average RT of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_SOURCE_NONE_READ_IOPS: the instantaneous read IOPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_READ_IOPS: the average read IOPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_READ_IOPS: the instantaneous read IOPS of the Checker-Verify component at the destination end during full verification; and CHECKER_VERIFY_DEST_AVG_READ_IOPS: the average read IOPS of the Checker-Verify component at the destination end during full verification.
+        # The business data returned.
         self.metric = metric
-        # The page number, which takes effect in a pagination query.
+        # The information about the object.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # A millisecond-level timestamp.
         self.page_size = page_size
-        # The ID of the project to query.
+        # The value corresponding to the time.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The name of the metric.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18748,17 +18909,15 @@
 
 class SearchOmsOpenAPIMonitorMetricResponseBodyDataDataPoints(TeaModel):
     def __init__(
         self,
         timestamp: int = None,
         value: float = None,
     ):
-        # A millisecond-level timestamp.
         self.timestamp = timestamp
-        # The value corresponding to the time.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18786,15 +18945,14 @@
         self,
         data_points: List[SearchOmsOpenAPIMonitorMetricResponseBodyDataDataPoints] = None,
         metric: str = None,
         tags: Dict[str, str] = None,
     ):
         # connector data point
         self.data_points = data_points
-        # The name of the metric.
         self.metric = metric
         # metric tags
         self.tags = tags
 
     def validate(self):
         if self.data_points:
             for k in self.data_points:
@@ -18835,21 +18993,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The information about the object.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (old).
         self.level = level
-        # The error description (new).
+        # The ID of the project to query.
         self.message = message
-        # The suggestions (new).
+        # The error description (new).
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18891,35 +19049,34 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.advice = advice
-        # The error code (old).
+        # The business data returned.
         self.code = code
-        # The time spent in processing the request, in seconds.
+        # The request ID.
         self.cost = cost
-        # The business data returned.
         self.data = data
-        # The error details.
+        # A system error occurred.
         self.error_detail = error_detail
-        # The error description (old).
+        # The suggestions (old).
         self.message = message
-        # The page number, which takes effect in a pagination query.
+        # The error code (new).
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # The page number, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
+        # The time spent in processing the request, in seconds.
         self.request_id = request_id
-        # Indicates whether the call is successful.
-        self.success = success
         # The total count, which takes effect in a pagination query.
+        self.success = success
+        # The error details.
         self.total_count = total_count
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -20563,21 +20720,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.page_size = page_size
-        # The project ID.
+        # The page number, which takes effect in a pagination query.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The total count, which takes effect in a pagination query.
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20612,21 +20769,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The error description (old).
         self.code = code
-        # Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (new).
         self.level = level
-        # The error description (new).
+        # The page number, which takes effect in a pagination query.
         self.message = message
-        # The suggestions (new).
+        # The error details.
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20668,35 +20825,27 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions.
         self.advice = advice
-        # The error code (old).
+        # The request ID.
         self.code = code
-        # The time spent in processing the request, in seconds.
         self.cost = cost
-        # Indicates whether the project is started.
         self.data = data
-        # The error details.
+        # The operation that you want to perform. Set the value to **StartOmsOpenAPIProject**.
         self.error_detail = error_detail
-        # The error description (old).
         self.message = message
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The suggestions (new).
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -20805,21 +20954,21 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
     ):
-        # The page number, which takes effect in a pagination query.
+        # The suggestions (old).
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size
-        # The project ID.
+        # The total count, which takes effect in a pagination query.
         self.project_id = project_id
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Alibaba Cloud CLI
         self.worker_grade_id = worker_grade_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20854,21 +21003,21 @@
     def __init__(
         self,
         code: str = None,
         level: str = None,
         message: str = None,
         proposal: str = None,
     ):
-        # The error code (new).
+        # The time spent in processing the request, in seconds.
         self.code = code
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (old).
         self.level = level
-        # The error description (new).
+        # The project ID.
         self.message = message
-        # The suggestions (new).
+        # The error description (new).
         self.proposal = proposal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20910,35 +21059,31 @@
         message: str = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The suggestions (old).
+        # Indicates whether the project is paused.
         self.advice = advice
-        # The error code (old).
+        # The page size, which takes effect in a pagination query.
         self.code = code
-        # The time spent in processing the request, in seconds.
         self.cost = cost
-        # Indicates whether the project is paused.
         self.data = data
-        # The error details.
+        # A system error occurred.
         self.error_detail = error_detail
-        # The error description (old).
+        # The page size, which takes effect in a pagination query.
         self.message = message
-        # The page number, which takes effect in a pagination query.
+        # Pause a data synchronization project
         self.page_number = page_number
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size
-        # The request ID.
+        # A system error occurred.
         self.request_id = request_id
-        # Indicates whether the call is successful.
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.success = success
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.7/setup.py` & `alibabacloud_oceanbasepro20190901-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901.
 
-Created on 10/04/2023
+Created on 19/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python"
```

