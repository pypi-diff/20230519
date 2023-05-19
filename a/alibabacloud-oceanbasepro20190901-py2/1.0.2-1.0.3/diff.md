# Comparing `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.2.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.2.tar", last modified: Mon Apr 10 03:09:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.3.tar", last modified: Fri May 19 10:09:23 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2.tar` & `alibabacloud_oceanbasepro20190901_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2526 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108324 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   798154 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2526 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2948 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109067 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)   835668 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/LICENSE` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/README-CN.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/README.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,16 @@
 
     def create_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_instance_with_options(request, runtime)
 
     def create_oms_mysql_data_source_with_options(self, request, runtime):
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
 
         @param request: CreateOmsMysqlDataSourceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateOmsMysqlDataSourceResponse
@@ -174,15 +175,16 @@
         return TeaCore.from_map(
             ocean_base_pro_20190901_models.CreateOmsMysqlDataSourceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_oms_mysql_data_source(self, request):
         """
-        To call this operation, you must add the IP address of the OceanBase Migration Service (OMS) server to the whitelist of the Alibaba Cloud database instance, the security rules of the ECS instance, or the security settings of your self-managed database (usually the firewall of your self-managed database) to ensure that OMS can successfully access your database instance. To obtain the IP address of the OMS server, go to the OMS data source management page in the OMS console.
+        The description of the data source.
+        It must be 2 to 256 characters in length. The default value is null.
         
 
         @param request: CreateOmsMysqlDataSourceRequest
 
         @return: CreateOmsMysqlDataSourceResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -432,17 +434,15 @@
 
     def delete_databases(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_databases_with_options(request, runtime)
 
     def delete_instances_with_options(self, request, runtime):
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
 
         @param request: DeleteInstancesRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteInstancesResponse
@@ -470,17 +470,15 @@
         return TeaCore.from_map(
             ocean_base_pro_20190901_models.DeleteInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_instances(self, request):
         """
-        Before you call this operation, ensure that the following requirements are met:
-        - The cluster is in the Running state.
-        - The cluster is a primary cluster and the billing method is pay-as-you-go.
+        Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         
 
         @param request: DeleteInstancesRequest
 
         @return: DeleteInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -739,14 +737,16 @@
     def describe_available_mem_resource(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_available_mem_resource_with_options(request, runtime)
 
     def describe_charset_with_options(self, request, runtime):
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
@@ -1866,14 +1866,46 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_zones(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_zones_with_options(request, runtime)
 
+    def kill_process_list_with_options(self, request, runtime):
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
+    def kill_process_list(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.kill_process_list_with_options(request, runtime)
+
     def modify_database_description_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.database_name):
             body['DatabaseName'] = request.database_name
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -2265,14 +2297,16 @@
     def modify_tenant_user_description(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_tenant_user_description_with_options(request, runtime)
 
     def modify_tenant_user_password_with_options(self, request, runtime):
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

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class CreateDatabaseRequest(TeaModel):
     def __init__(self, client_token=None, collation=None, database_name=None, description=None, encoding=None,
                  instance_id=None, tenant_id=None):
-        # The token used to ensure idempotence.  
-        # The value of this parameter is generated by the client and is unique among different requests.   
-        # 
-        # > <br>ClientToken can contain only ASCII characters, and cannot exceed 64 characters in length.
+        # The name of the database.
         self.client_token = client_token  # type: str
-        # The collation.
+        # The encoding standard of the database.
+        # For more information, see the Charset field returned by the DescribeCharset operation.
         self.collation = collation  # type: str
-        # The name of the database.   
-        # You cannot use reserved keywords, such as test and mysql.
+        # Alibaba Cloud CLI
         self.database_name = database_name  # type: str
-        # The description of the database.
+        # The operation that you want to perform.   
+        # Set the value to **CreateDatabase**.
         self.description = description  # type: str
-        # The encoding standard of the database.
-        # For more information, see the Charset field returned by the DescribeCharset operation.
+        # The ID of the tenant.
         self.encoding = encoding  # type: str
-        # The ID of the OceanBase cluster.
+        # The collation.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # The name of the database.   
+        # You cannot use reserved keywords, such as test and mysql.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDatabaseRequest, self).to_map()
@@ -68,17 +66,16 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class CreateDatabaseResponseBody(TeaModel):
     def __init__(self, database_name=None, request_id=None):
-        # The name of the database.
+        # CreateDatabase
         self.database_name = database_name  # type: str
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDatabaseResponseBody, self).to_map()
@@ -146,60 +143,63 @@
                  series=None, zones=None):
         # Specifies whether to enable automatic renewal.   
         # This parameter is valid only when the ChargeType parameter is set to PrePaid. Valid values: 
         # - true: enables automatic renewal for the instance.   
         # - false: disables automatic renewal for the instance. This is the default value.
         self.auto_renew = auto_renew  # type: bool
         # The automatic renewal period of the instance. This parameter is required when the AutoRenew parameter is set to true. Valid values:  
-        # - If the PeriodUnit parameter is set to Week: 1, 2, and 3.   
-        # - If the PeriodUnit parameter is set to Month: 1, 2, 3, 6, and 12.
+        # - If the PeriodUnit parameter is set to Year: "1", "2", and "3".   
+        # - If the PeriodUnit parameter is set to Month: "1", "2", "3", "6", and "12".
         self.auto_renew_period = auto_renew_period  # type: long
         # The billing method of the instance. Valid values:  
-        # -PrePay: the subscription billing method. You must ensure that the remaining balance or credit balance of your account can cover the cost of the subscription. Otherwise, you will receive an InvalidPayMethod error. 
+        # - PrePay: the subscription billing method. You must ensure that the remaining balance or credit balance of your account can cover the cost of the subscription. Otherwise, you will receive an InvalidPayMethod error. 
         # - PostPay: the pay-as-you-go billing method. This is the default value. By default, fees are charged on an hourly basis.
         self.charge_type = charge_type  # type: str
-        # The size of the storage space, in GB.    
+        # The size of the storage space,in GB.    
         # The limits on the storage space vary with the cluster specifications:   
         # - 8C32GB: 100 GB to 10000 GB   
         # - 14C70GB: 200 GB to 10000 GB   
         # - 30C180GB: 400 GB to 10000 GB   
         # - 62C400GB: 800 GB to 10000 GB    
         # The preceding minimum storage space sizes are the default storage space sizes of the corresponding cluster specification plans.
         self.disk_size = disk_size  # type: long
+        # The return result of the request.
         self.disk_type = disk_type  # type: str
         # The specifications of the cluster.     
         # You can specify one of the following four plans:   
         #  - 8C32GB: indicates 8 CPU cores and 32 GB of memory.    
-        #  - 14C70GB: indicates 14 CPU cores and 70 GB of memory. This is the default value.     
+        #  - 14C70GB: indicates 14 CPU cores and 70 GB of memory. This is the default value.
         # - 30C180GB: indicates 30 CPU cores and 180 GB of memory.     
         # - 62C400GB: indicates 62 CPU cores and 400 GB of memory.
         self.instance_class = instance_class  # type: str
         # The name of the OceanBase cluster.    
         # It must be 1 to 20 characters in length.   
         # If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.instance_name = instance_name  # type: str
+        # OceanBase Server version number.
         self.ob_version = ob_version  # type: str
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
         self.period = period  # type: long
         # The unit of the valid duration of the purchased resources.     
-        # Valid value for subscription: Month.   
+        # Valid value for subscription: Month or Year.
         # Default value: Month for subscription, and Hour for pay-as-you-go.
         self.period_unit = period_unit  # type: str
         # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id  # type: str
         # The series of the OceanBase cluster. Valid values:    
-        # normal: the high availability edition. This is the default value.
+        # - normal: Standard Cluster Edition (Cloud Disk). This is the default value.
+        # - normal_ssd: Standard Cluster Edition (Local Disk).
+        # - history: History Database Cluster Edition.
         self.series = series  # type: str
         # The ID of the zone to which the instance belongs.   
-        # For more information about how to obtain the list of zones, see [DescribeZones](https://www.alibabacloud.com/help/zh/doc-detail/25610.htm).
+        # For more information about how to obtain the list of zones, see [DescribeZones](~~25610~~).
         self.zones = zones  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateInstanceRequest, self).to_map()
@@ -264,15 +264,17 @@
         if m.get('Zones') is not None:
             self.zones = m.get('Zones')
         return self
 
 
 class CreateInstanceResponseBodyData(TeaModel):
     def __init__(self, instance_id=None, order_id=None, resource_group_id=None):
+        # 订单ID。该参数只有创建包年包月ECS实例（请求参数InstanceChargeType=PrePaid）时有返回值。
         self.instance_id = instance_id  # type: str
+        # 资源组ID
         self.order_id = order_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -298,16 +300,17 @@
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class CreateInstanceResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
+        # 实例ID
         self.data = data  # type: CreateInstanceResponseBodyData
-        # The request ID.
+        # Response parameters
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -370,53 +373,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateOmsMysqlDataSourceRequest(TeaModel):
     def __init__(self, description=None, dg_database_id=None, instance_id=None, ip=None, name=None, password=None,
                  port=None, schema=None, type=None, username=None, vpc_id=None):
-        # The description of the data source.   
-        # It must be 2 to 256 characters in length. The default value is null.
         self.description = description  # type: str
-        # The ID of the database gateway instance.   
-        # 
-        # > <br>If Type is set to DG, this parameter is required.
         self.dg_database_id = dg_database_id  # type: str
-        # The ID of the ECS instance of the data source.   
-        # 
-        # > <br>If Type is set to RDS, POLARDB, or DG, this parameter is required.
         self.instance_id = instance_id  # type: str
-        # The IP address of the data source.   
-        # 
-        # > <br>If Type is set to INTERNET or VPC, this parameter is required.
         self.ip = ip  # type: str
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
         self.name = name  # type: str
-        # The password of the username that is used to access the database. It must be Base64 encoded.   
-        # For example, for the password abcd123@!, the Base64-encoded value is YWJjZDEyM0Ah.
         self.password = password  # type: str
-        # The port number of the data source.   
-        # 
-        # > <br>If Type is set to INTERNET or VPC, this parameter is required.
         self.port = port  # type: str
-        # The name of the database.   
-        # 
-        # > <br>If you specify this parameter, subsequent migration or synchronization operations will take effect on this database only.
         self.schema = schema  # type: str
-        # The type of the MySQL data source.   
-        # Valid values: INTERNET, VPC, RDS, POLARDB, and DG.
         self.type = type  # type: str
-        # The username that is used to access the database.
         self.username = username  # type: str
-        # The ID of the VPC to which the data source belongs.   
-        # 
-        # > <br>If Type is set to VPC, this parameter is required.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsMysqlDataSourceRequest, self).to_map()
@@ -473,15 +462,14 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class CreateOmsMysqlDataSourceResponseBodyData(TeaModel):
     def __init__(self, endpoint_id=None):
-        # The ID of the data source record.
         self.endpoint_id = endpoint_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsMysqlDataSourceResponseBodyData, self).to_map()
@@ -498,17 +486,15 @@
         if m.get('EndpointId') is not None:
             self.endpoint_id = m.get('EndpointId')
         return self
 
 
 class CreateOmsMysqlDataSourceResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The return result of the request.
         self.data = data  # type: CreateOmsMysqlDataSourceResponseBodyData
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -572,37 +558,25 @@
         return self
 
 
 class CreateOmsOpenAPIProjectRequestDestConfig(TeaModel):
     def __init__(self, enable_msg_trace=None, endpoint_id=None, endpoint_type=None, msg_tags=None, partition=None,
                  partition_mode=None, producer_group=None, send_msg_timeout=None, sequence_enable=None,
                  sequence_start_timestamp=None, serializer_type=None, topic_type=None):
-        # Specifies whether to enable message tracing when the destination data source is RocketMQ.
         self.enable_msg_trace = enable_msg_trace  # type: bool
-        # The ID of the data source.
         self.endpoint_id = endpoint_id  # type: str
-        # The type of the data source. Valid values: `MYSQL`, `MARIADB`, `OB_MYSQL`, `OB_MYSQL_CE`, `OB_ORACLE`, `ORACLE`, `DB2_LUW`, `KAFKA`, `ROCKETMQ`, `DATAHUB`, `SYBASE`, `LOGPROXY`, `ADB`, `DBP_OP_ROUTE`, `DMS`, `IDB`, and `TIDB`.
         self.endpoint_type = endpoint_type  # type: str
-        # The tag of the Post message when the destination data source is RocketMQ.
         self.msg_tags = msg_tags  # type: str
-        # The partitioned index, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ, and the partitioning mode is set to ONE.
         self.partition = partition  # type: int
-        # The partitioning mode, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: ONE, HASH, and TABLE.
         self.partition_mode = partition_mode  # type: str
-        # The producer group of the Post message when the destination data source is RocketMQ.
         self.producer_group = producer_group  # type: str
-        # The timeout period for a single Post message when the destination data source is RocketMQ.
         self.send_msg_timeout = send_msg_timeout  # type: long
-        # Specifies whether to enable message sequencing when the destination data source is DataHub.
         self.sequence_enable = sequence_enable  # type: bool
-        # The start time of the sequence, which must be specified if the destination data source is DataHub and message sequencing is enabled. The value is a timestamp in seconds.
         self.sequence_start_timestamp = sequence_start_timestamp  # type: long
-        # The text serialization type, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: Default, Canal, Dataworks, SharePlex, and DefaultExtendColumnType.
         self.serializer_type = serializer_type  # type: str
-        # The type of the topic to which the Post message belongs when the destination data source is DataHub. Valid values: Tuple and Blob.
         self.topic_type = topic_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectRequestDestConfig, self).to_map()
@@ -665,37 +639,25 @@
         return self
 
 
 class CreateOmsOpenAPIProjectRequestSourceConfig(TeaModel):
     def __init__(self, enable_msg_trace=None, endpoint_id=None, endpoint_type=None, msg_tags=None, partition=None,
                  partition_mode=None, producer_group=None, send_msg_timeout=None, sequence_enable=None,
                  sequence_start_timestamp=None, serializer_type=None, topic_type=None):
-        # Specifies whether to enable message tracing when the destination data source is RocketMQ.
         self.enable_msg_trace = enable_msg_trace  # type: bool
-        # The ID of the data source.
         self.endpoint_id = endpoint_id  # type: str
-        # The type of the data source. Valid values: `MYSQL`, `MARIADB`, `OB_MYSQL`, `OB_MYSQL_CE`, `OB_ORACLE`, `ORACLE`, `DB2_LUW`, `KAFKA`, `ROCKETMQ`, `DATAHUB`, `SYBASE`, `LOGPROXY`, `ADB`, `DBP_OP_ROUTE`, `DMS`, `IDB`, and `TIDB`.
         self.endpoint_type = endpoint_type  # type: str
-        # The tag of the Post message when the destination data source is RocketMQ.
         self.msg_tags = msg_tags  # type: str
-        # The partitioned index, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ, and the partitioning mode is set to ONE.
         self.partition = partition  # type: int
-        # The partitioning mode, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: ONE, HASH, and TABLE.
         self.partition_mode = partition_mode  # type: str
-        # The producer group of the Post message when the destination data source is RocketMQ.
         self.producer_group = producer_group  # type: str
-        # The timeout period for a single Post message when the destination data source is RocketMQ.
         self.send_msg_timeout = send_msg_timeout  # type: long
-        # Specifies whether to enable message sequencing when the destination data source is DataHub.
         self.sequence_enable = sequence_enable  # type: bool
-        # The start time of the sequence, which must be specified if the destination data source is DataHub and message sequencing is enabled. The value is a timestamp in seconds.
         self.sequence_start_timestamp = sequence_start_timestamp  # type: long
-        # The text serialization type, which must be specified if the destination data source is a message queue system, such as Kafka, DataHub, or RocketMQ. Valid values: Default, Canal, Dataworks, SharePlex, and DefaultExtendColumnType.
         self.serializer_type = serializer_type  # type: str
-        # The type of the topic to which the Post message belongs when the destination data source is DataHub. Valid values: Tuple and Blob.
         self.topic_type = topic_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectRequestSourceConfig, self).to_map()
@@ -757,21 +719,17 @@
             self.topic_type = m.get('TopicType')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTablesAdbTableSchema(TeaModel):
     def __init__(self, distributed_keys=None, partition_life_cycle=None, partition_statement=None,
                  primary_keys=None):
-        # The list of distribution key columns.
         self.distributed_keys = distributed_keys  # type: list[str]
-        # The lifecycle of the table.
         self.partition_life_cycle = partition_life_cycle  # type: int
-        # The partitioning expression.
         self.partition_statement = partition_statement  # type: str
-        # The list of primary key columns.
         self.primary_keys = primary_keys  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTablesAdbTableSchema, self).to_map()
@@ -801,29 +759,21 @@
             self.primary_keys = m.get('PrimaryKeys')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTables(TeaModel):
     def __init__(self, adb_table_schema=None, filter_columns=None, mapped_name=None, shard_columns=None,
                  table_id=None, table_name=None, type=None, where_clause=None):
-        # The schema of the ADB table. If the destination data source is ADB, you need to configure additional information for schema synchronization.
         self.adb_table_schema = adb_table_schema  # type: CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTablesAdbTableSchema
-        # The list of filter columns, which are the columns to be synchronized.
         self.filter_columns = filter_columns  # type: list[str]
-        # The name of the mapped-to table or topic. If the destination data source is a database, this parameter specifies the name of the mapped-to table. If the destination data source is a message queue system, this parameter specifies the name of the mapped-to topic.
         self.mapped_name = mapped_name  # type: str
-        # The list of sharding key columns. This parameter applies to scenarios where the destination data source is a message queue system.
         self.shard_columns = shard_columns  # type: list[str]
-        # The ID of the table. This parameter takes effect when the source data source is IDB.
         self.table_id = table_id  # type: str
-        # The name of the table.
         self.table_name = table_name  # type: str
-        # Valid values: DATABASE and TABLE.
         self.type = type  # type: str
-        # The row filter conditions.
         self.where_clause = where_clause  # type: str
 
     def validate(self):
         if self.adb_table_schema:
             self.adb_table_schema.validate()
 
     def to_map(self):
@@ -871,25 +821,19 @@
             self.where_clause = m.get('WhereClause')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferMappingDatabases(TeaModel):
     def __init__(self, database_id=None, database_name=None, mapped_name=None, tables=None, tenant_name=None,
                  type=None):
-        # The ID of the database. This parameter takes effect when the source data source is IDB.
         self.database_id = database_id  # type: str
-        # The name of the database.
         self.database_name = database_name  # type: str
-        # The mapped-to database. This parameter takes effect when the destination data source is a database.
         self.mapped_name = mapped_name  # type: str
-        # The settings for the target table objects in the current database.
         self.tables = tables  # type: list[CreateOmsOpenAPIProjectRequestTransferMappingDatabasesTables]
-        # The mapped-to tenant. This parameter takes effect when the source data source is OceanBase Database.
         self.tenant_name = tenant_name  # type: str
-        # Valid values: DATABASE and TABLE.
         self.type = type  # type: str
 
     def validate(self):
         if self.tables:
             for k in self.tables:
                 if k:
                     k.validate()
@@ -934,17 +878,15 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferMapping(TeaModel):
     def __init__(self, databases=None, mode=None):
-        # The table mapping in the source data source, which is a conventional mapping scheme and takes effect only when Mode is set to NORMAL.
         self.databases = databases  # type: list[CreateOmsOpenAPIProjectRequestTransferMappingDatabases]
-        # The mapping type. Valid values: \"NORMAL\" and \"WHITE_AND_BLACK_LIST\".
         self.mode = mode  # type: str
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -974,23 +916,18 @@
             self.mode = m.get('Mode')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferStepConfigIncrSyncStepTransferConfig(TeaModel):
     def __init__(self, record_type_list=None, start_timestamp=None, store_log_kept_hour=None,
                  store_transaction_enabled=None, transfer_step_type=None):
-        # The list of data types of incremental data synchronized in incremental synchronization.
         self.record_type_list = record_type_list  # type: list[str]
-        # The start time for incremental synchronization. The value is a timestamp in seconds.
         self.start_timestamp = start_timestamp  # type: long
-        # The retention time of logs when incremental synchronization is enabled and the incremental log pull component is Store.
         self.store_log_kept_hour = store_log_kept_hour  # type: long
-        # Specifies whether to enable intra-transaction sequencing when incremental synchronization is enabled and the incremental log pull component is Store.
         self.store_transaction_enabled = store_transaction_enabled  # type: bool
-        # Valid values: STRUCT, FULL, and INCR.
         self.transfer_step_type = transfer_step_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectRequestTransferStepConfigIncrSyncStepTransferConfig, self).to_map()
@@ -1024,21 +961,17 @@
             self.transfer_step_type = m.get('TransferStepType')
         return self
 
 
 class CreateOmsOpenAPIProjectRequestTransferStepConfig(TeaModel):
     def __init__(self, enable_full_sync=None, enable_incr_sync=None, enable_struct_sync=None,
                  incr_sync_step_transfer_config=None):
-        # Specifies whether to enable full migration.
         self.enable_full_sync = enable_full_sync  # type: bool
-        # Specifies whether to enable incremental synchronization.
         self.enable_incr_sync = enable_incr_sync  # type: bool
-        # Specifies whether to enable schema synchronization.
         self.enable_struct_sync = enable_struct_sync  # type: bool
-        # The settings of incremental synchronization steps.
         self.incr_sync_step_transfer_config = incr_sync_step_transfer_config  # type: CreateOmsOpenAPIProjectRequestTransferStepConfigIncrSyncStepTransferConfig
 
     def validate(self):
         if self.incr_sync_step_transfer_config:
             self.incr_sync_step_transfer_config.validate()
 
     def to_map(self):
@@ -1070,33 +1003,26 @@
             self.incr_sync_step_transfer_config = temp_model.from_map(m['IncrSyncStepTransferConfig'])
         return self
 
 
 class CreateOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, business_name=None, dest_config=None, label_ids=None, page_number=None, page_size=None,
                  project_name=None, source_config=None, transfer_mapping=None, transfer_step_config=None, worker_grade_id=None):
-        # The business system identifier, which is optional and is a specific field of the Post message.
         self.business_name = business_name  # type: str
-        # The settings of the destination data source.
         self.dest_config = dest_config  # type: CreateOmsOpenAPIProjectRequestDestConfig
-        # A collection of label IDs.
         self.label_ids = label_ids  # type: list[str]
-        # The page number, which takes effect in a pagination query.
+        # 页序号，分页查询时生效
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # 页大小，分页查询时生效
         self.page_size = page_size  # type: int
-        # The name of the project.
         self.project_name = project_name  # type: str
-        # The settings of the source data source.
         self.source_config = source_config  # type: CreateOmsOpenAPIProjectRequestSourceConfig
-        # The mappings for the synchronization objects.
         self.transfer_mapping = transfer_mapping  # type: CreateOmsOpenAPIProjectRequestTransferMapping
-        # The settings of synchronization steps.
         self.transfer_step_config = transfer_step_config  # type: CreateOmsOpenAPIProjectRequestTransferStepConfig
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # 实例规格 ID，创建项目时生效
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         if self.dest_config:
             self.dest_config.validate()
         if self.source_config:
             self.source_config.validate()
@@ -1162,33 +1088,26 @@
         return self
 
 
 class CreateOmsOpenAPIProjectShrinkRequest(TeaModel):
     def __init__(self, business_name=None, dest_config_shrink=None, label_ids_shrink=None, page_number=None,
                  page_size=None, project_name=None, source_config_shrink=None, transfer_mapping_shrink=None,
                  transfer_step_config_shrink=None, worker_grade_id=None):
-        # The business system identifier, which is optional and is a specific field of the Post message.
         self.business_name = business_name  # type: str
-        # The settings of the destination data source.
         self.dest_config_shrink = dest_config_shrink  # type: str
-        # A collection of label IDs.
         self.label_ids_shrink = label_ids_shrink  # type: str
-        # The page number, which takes effect in a pagination query.
+        # 页序号，分页查询时生效
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # 页大小，分页查询时生效
         self.page_size = page_size  # type: int
-        # The name of the project.
         self.project_name = project_name  # type: str
-        # The settings of the source data source.
         self.source_config_shrink = source_config_shrink  # type: str
-        # The mappings for the synchronization objects.
         self.transfer_mapping_shrink = transfer_mapping_shrink  # type: str
-        # The settings of synchronization steps.
         self.transfer_step_config_shrink = transfer_step_config_shrink  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # 实例规格 ID，创建项目时生效
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectShrinkRequest, self).to_map()
@@ -1241,21 +1160,17 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class CreateOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
         self.code = code  # type: str
-        # Valid values: CRITICAL, ERROR, and WARN.
         self.level = level  # type: str
-        # The error description (new).
         self.message = message  # type: str
-        # The suggestions (new).
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -1285,35 +1200,24 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class CreateOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
         self.advice = advice  # type: str
-        # The error code (old).
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
         self.cost = cost  # type: str
-        # The project creation details.
         self.data = data  # type: str
-        # The error details.
         self.error_detail = error_detail  # type: CreateOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -1415,18 +1319,15 @@
 
 class CreateSecurityIpGroupRequest(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
         # The name of the whitelist group.
         self.security_ip_group_name = security_ip_group_name  # type: str
-        # The IP addresses or CIDR blocks in the IP address whitelist group.   
-        # It is a JSON array. Each object in the array is an IP address or CIDR block. The following two formats are supported:  
-        # - IP address: for example, 10.23.12.24. 
-        # - CIDR block: for example, 10.23.12.24/24, where 24 indicates the length of the prefix in the IP address, and the prefix is 1 to 30 characters in length.  Limit: You can set no more than 40 IP addresses or CIDR blocks for a whitelist group. A total of 200 IP addresses or CIDR blocks are supported for all whitelist groups.
+        # The return result of the request.
         self.security_ips = security_ips  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateSecurityIpGroupRequest, self).to_map()
@@ -1451,20 +1352,24 @@
         if m.get('SecurityIps') is not None:
             self.security_ips = m.get('SecurityIps')
         return self
 
 
 class CreateSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None):
-        # The ID of the OceanBase cluster.
+        # ```
+        # http(s)://[Endpoint]/?Action=CreateSecurityIpGroup
+        # &InstanceId=ob317v4uif****\
+        # &SecurityIps=192.168.1.1,192.168.0.0.1/8
+        # &SecurityIpGroupName=pay_online
+        # &Common request parameters
+        # ```
         self.instance_id = instance_id  # type: str
-        # The name of the whitelist group.
+        # You can call this operation to create an IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name  # type: str
-        # The IP addresses or CIDR blocks in the IP address whitelist group.   
-        # The return values of SecurityIps are strings that are separated with commas (,).
         self.security_ips = security_ips  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateSecurityIpGroupResponseBodySecurityIpGroup, self).to_map()
@@ -1489,17 +1394,19 @@
         if m.get('SecurityIps') is not None:
             self.security_ips = m.get('SecurityIps')
         return self
 
 
 class CreateSecurityIpGroupResponseBody(TeaModel):
     def __init__(self, request_id=None, security_ip_group=None):
-        # The request ID.
+        # The IP addresses or CIDR blocks in the IP address whitelist group.   
+        # The return values of SecurityIps are strings that are separated with commas (,).
         self.request_id = request_id  # type: str
-        # The information of the whitelist group.
+        # The operation that you want to perform.   
+        # Set the value to **CreateSecurityIpGroup**.
         self.security_ip_group = security_ip_group  # type: CreateSecurityIpGroupResponseBodySecurityIpGroup
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -1562,51 +1469,42 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTenantRequest(TeaModel):
     def __init__(self, charset=None, cpu=None, description=None, instance_id=None, memory=None, primary_zone=None,
                  tenant_mode=None, tenant_name=None, time_zone=None, unit_num=None, user_vswitch_id=None, user_vpc_id=None):
-        # The character set.    
-        # For more information, see DescribeCharset.
+        # The description of the database.
         self.charset = charset  # type: str
-        # The number of CPU cores of the tenant.   
-        # 
-        # > <br>The CPU specification of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the CPU specification of the tenant cannot exceed 14 cores.
+        # The number of resource distribution nodes in the tenant.    
+        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
         self.cpu = cpu  # type: int
-        # The description of the database.
+        # $.parameters[13].schema.example
         self.description = description  # type: str
-        # The ID of the OceanBase cluster.
+        # The ID of the vSwitch.    
+        # If no suitable vSwitch is available, create a vSwitch as prompted.   
+        # For more information, see Use a vSwitch.
         self.instance_id = instance_id  # type: str
-        # The memory size of the tenant, in GB.   
-        # 
-        # > <br>The memory size of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the memory size of the tenant cannot exceed 70 GB.
+        # The return result of the request.
         self.memory = memory  # type: int
-        # The primary zone of the tenant.    
-        # It is one of the zones in which the cluster is deployed.
+        # $.parameters[12].schema.enumValueTitles
         self.primary_zone = primary_zone  # type: str
-        # The tenant mode.    
-        # Valid values: Oracle and MySQL.   
-        # For more information, see [DescribeInstanceTenantModes](~~410354~~).
+        # The ID of the tenant.
         self.tenant_mode = tenant_mode  # type: str
-        # The name of the tenant.    
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
+        # Alibaba Cloud CLI
         self.tenant_name = tenant_name  # type: str
-        # The time zone of the tenant. For more information, see [DescribeTimeZones](~~410361~~).
+        # The memory size of the tenant, in GB.   
+        # 
+        # > <br>The memory size of a single tenant cannot exceed that of the corresponding cluster. <br>For example, if the specification of the cluster is 14 CPU cores and 70 GB of memory, the memory size of the tenant cannot exceed 70 GB.
         self.time_zone = time_zone  # type: str
-        # The number of resource distribution nodes in the tenant.    
-        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
+        # $.parameters[11].schema.description
         self.unit_num = unit_num  # type: int
-        # The ID of the vSwitch.    
-        # If no suitable vSwitch is available, create a vSwitch as prompted.   
-        # For more information, see Use a vSwitch.
+        # $.parameters[12].schema.description
         self.user_vswitch_id = user_vswitch_id  # type: str
-        # The ID of the VPC.   
-        #  If no suitable VPC is available, create a VPC as prompted.   
-        # For more information, see "What is a VPC".
+        # The time zone of the tenant.  For more information, see [DescribeTimeZones](https://help.aliyun.com/document_detail/410361.html).
         self.user_vpc_id = user_vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantRequest, self).to_map()
@@ -1667,17 +1565,17 @@
         if m.get('UserVpcId') is not None:
             self.user_vpc_id = m.get('UserVpcId')
         return self
 
 
 class CreateTenantResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_id=None):
-        # The request ID.
+        # WB01144930
         self.request_id = request_id  # type: str
-        # The ID of the tenant.
+        # You can call this operation to create a tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantResponseBody, self).to_map()
@@ -1737,21 +1635,16 @@
             temp_model = CreateTenantResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTenantReadOnlyConnectionRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_id=None, zone_id=None):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The ID of the zone.  
-        # 
-        # For more information, see AvailableZones in DescribeInstance.
         self.zone_id = zone_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantReadOnlyConnectionRequest, self).to_map()
@@ -1776,15 +1669,14 @@
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
 class CreateTenantReadOnlyConnectionResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantReadOnlyConnectionResponseBody, self).to_map()
@@ -1843,43 +1735,27 @@
 
 
 class CreateTenantUserRequest(TeaModel):
     def __init__(self, description=None, encryption_type=None, instance_id=None, roles=None, tenant_id=None,
                  user_name=None, user_password=None, user_type=None):
         # The description of the database.
         self.description = description  # type: str
+        # 加密方式。
         self.encryption_type = encryption_type  # type: str
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
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
         self.roles = roles  # type: str
         # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
+        # The name of the database account.  You cannot use reserved keywords, such as SYS and root.
         self.user_name = user_name  # type: str
-        # The password of the database account. 
-        # 
-        # > <br>It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % ^ & \ * ( ) _ + - =\
+        # The password of the database account.  It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % \ ^ \ & \ * ( ) _ + - =\
         self.user_password = user_password  # type: str
-        # The type of the database account. Valid values:   
-        # 
-        # - Admin: the super administrator account.   
-        # - Normal: a general account.
+        # The type of the database account. Valid values: Admin: the super administrator account. Normal: a general account.
         self.user_type = user_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantUserRequest, self).to_map()
@@ -1926,28 +1802,17 @@
         return self
 
 
 class CreateTenantUserResponseBodyTenantUserRoles(TeaModel):
     def __init__(self, database=None, role=None):
         # The name of the database.
         self.database = database  # type: str
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
         self.role = role  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTenantUserResponseBodyTenantUserRoles, self).to_map()
@@ -1972,21 +1837,17 @@
 
 class CreateTenantUserResponseBodyTenantUser(TeaModel):
     def __init__(self, roles=None, user_name=None, user_status=None, user_type=None):
         # The roles of the accounts.
         self.roles = roles  # type: list[CreateTenantUserResponseBodyTenantUserRoles]
         # The name of the database account.
         self.user_name = user_name  # type: str
-        # The status of the database account. Valid values:    
-        # - Locked: The account is locked.   
-        # - ONLINE: The account is unlocked. The default status of a new account is ONLINE after it is created.
+        # The status of the database account. Valid values:  - Locked: The account is locked. - ONLINE: The account is unlocked. The default status of a new account is ONLINE after it is created.
         self.user_status = user_status  # type: str
-        # The type of the database account. Valid values:   
-        #  - Admin: the super administrator account.   
-        #  - Normal: a general account.
+        # The type of the database account. Valid values:  - Admin: the super administrator account. - Normal: a general account.
         self.user_type = user_type  # type: str
 
     def validate(self):
         if self.roles:
             for k in self.roles:
                 if k:
                     k.validate()
@@ -2101,20 +1962,16 @@
             temp_model = CreateTenantUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDatabasesRequest(TeaModel):
     def __init__(self, database_names=None, instance_id=None, tenant_id=None):
-        # The list of database names.    
-        # It is a JSON array. Each object in the array is a database name string.
         self.database_names = database_names  # type: str
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDatabasesRequest, self).to_map()
@@ -2139,15 +1996,14 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DeleteDatabasesResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDatabasesResponseBody, self).to_map()
@@ -2203,23 +2059,15 @@
             temp_model = DeleteDatabasesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteInstancesRequest(TeaModel):
     def __init__(self, backup_retain_mode=None, instance_ids=None):
-        # The backup retention strategy for cluster deletion. Valid values:  
-        # - receive_all: retains all backup sets.   
-        # - delete_all: deletes all backup sets.   
-        # - receive_last: retains the last backup set.    
-        # 
-        # > <br>Default value: delete_all.
         self.backup_retain_mode = backup_retain_mode  # type: str
-        # The ID of the cluster to be deleted.   
-        # The value is a string in the JSON format.
         self.instance_ids = instance_ids  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteInstancesRequest, self).to_map()
@@ -2240,15 +2088,14 @@
         if m.get('InstanceIds') is not None:
             self.instance_ids = m.get('InstanceIds')
         return self
 
 
 class DeleteInstancesResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteInstancesResponseBody, self).to_map()
@@ -2304,21 +2151,21 @@
             temp_model = DeleteInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteOmsOpenAPIProjectRequest, self).to_map()
@@ -2347,21 +2194,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class DeleteOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **DeleteOmsOpenAPIProject**.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level  # type: str
-        # The error description (new).
+        # The error code (new).
         self.message = message  # type: str
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -2391,35 +2238,29 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class DeleteOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # You can call this operation to delete a data synchronization project.
         self.advice = advice  # type: str
-        # The error code (old).
+        # Indicates whether the project has been deleted.
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the project has been deleted.
         self.data = data  # type: bool
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail  # type: DeleteOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
+        # A system error occurred.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -2517,18 +2358,18 @@
             temp_model = DeleteOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteSecurityIpGroupRequest(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id  # type: str
         # The name of the IP address whitelist group.    
         # It must be 2 to 32 characters in length, start with a lowercase letter, end with a lowercase letter or digit, and contain only lowercase letters, digits, and underscores (_).
+        self.instance_id = instance_id  # type: str
+        # The information of the deleted IP whitelist group.
         self.security_ip_group_name = security_ip_group_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteSecurityIpGroupRequest, self).to_map()
@@ -2549,17 +2390,15 @@
         if m.get('SecurityIpGroupName') is not None:
             self.security_ip_group_name = m.get('SecurityIpGroupName')
         return self
 
 
 class DeleteSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The name of the deleted IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteSecurityIpGroupResponseBodySecurityIpGroup, self).to_map()
@@ -2580,17 +2419,16 @@
         if m.get('SecurityIpGroupName') is not None:
             self.security_ip_group_name = m.get('SecurityIpGroupName')
         return self
 
 
 class DeleteSecurityIpGroupResponseBody(TeaModel):
     def __init__(self, request_id=None, security_ip_group=None):
-        # The request ID.
+        # Example 1
         self.request_id = request_id  # type: str
-        # The information of the deleted IP whitelist group.
         self.security_ip_group = security_ip_group  # type: DeleteSecurityIpGroupResponseBodySecurityIpGroup
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -2652,19 +2490,19 @@
             temp_model = DeleteSecurityIpGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteTenantUsersRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_id=None, users=None):
-        # The ID of the OceanBase cluster.
+        # Example 1
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # $.parameters[4].schema.enumValueTitles
         self.tenant_id = tenant_id  # type: str
-        # A list of usernames and their respective roles.
+        # $.parameters[2].schema.example
         self.users = users  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTenantUsersRequest, self).to_map()
@@ -2689,15 +2527,15 @@
         if m.get('Users') is not None:
             self.users = m.get('Users')
         return self
 
 
 class DeleteTenantUsersResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
+        # DeleteTenantUsers
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTenantUsersResponseBody, self).to_map()
@@ -2753,18 +2591,22 @@
             temp_model = DeleteTenantUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteTenantsRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_ids=None):
-        # The ID of the OceanBase cluster.
+        # You can call this operation to delete one or more tenants from an OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The list of tenant IDs.   
-        # It is a JSON array. Each object in the array is a tenant name string.
+        # ```
+        # http(s)://[Endpoint]/?Action=DeleteTenants
+        # &TenantIds=["ob2mr3oae0****", "ob2mr3oae1****"]
+        # &InstanceId=ob317v4uif****\
+        # &Common request parameters
+        # ```
         self.tenant_ids = tenant_ids  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTenantsRequest, self).to_map()
@@ -2785,17 +2627,15 @@
         if m.get('TenantIds') is not None:
             self.tenant_ids = m.get('TenantIds')
         return self
 
 
 class DeleteTenantsResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_ids=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The list of tenant IDs.
         self.tenant_ids = tenant_ids  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTenantsResponseBody, self).to_map()
@@ -2857,54 +2697,53 @@
         return self
 
 
 class DescribeAnomalySQLListRequest(TeaModel):
     def __init__(self, accept_language=None, db_name=None, end_time=None, filter_condition=None, node_ip=None,
                  page_number=None, page_size=None, sqlid=None, search_key_word=None, search_parameter=None, search_rule=None,
                  search_value=None, sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The language of the returned data.   
-        # Default value: CN for a China site and EN for an International site.
+        # The search value.
         self.accept_language = accept_language  # type: str
-        # The name of the database.
+        # {
+        #   "UserName":testUser
+        # }
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # zh-CN
         self.end_time = end_time  # type: str
-        # The filter condition.   
-        # > <br> - All fields in OceanBase Database support filtering. <br> - You can write the key-value pair of a parameter in a JSON string in the JSON format to filter the parameter.
-        self.filter_condition = filter_condition  # type: dict[str, any]
-        # The IP address of the node.
-        self.node_ip = node_ip  # type: str
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
-        self.page_number = page_number  # type: int
+        self.filter_condition = filter_condition  # type: dict[str, any]
         # The number of rows to return on each page.    
         # - Maximum value: 100   
         # - Default value: 10
+        self.node_ip = node_ip  # type: str
+        # desc
+        self.page_number = page_number  # type: int
+        # The start time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.page_size = page_size  # type: int
-        # SQLID.
+        # 1
         self.sqlid = sqlid  # type: str
         # The search keyword.
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # The ID of the tenant.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.   
-        # Valid values: "=", ">", ">=", "<", and "<="
+        # Utilization above threshold
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # 10
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The end time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The request time, in ms.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The total count.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAnomalySQLListRequest, self).to_map()
@@ -2983,54 +2822,53 @@
         return self
 
 
 class DescribeAnomalySQLListShrinkRequest(TeaModel):
     def __init__(self, accept_language=None, db_name=None, end_time=None, filter_condition_shrink=None,
                  node_ip=None, page_number=None, page_size=None, sqlid=None, search_key_word=None, search_parameter=None,
                  search_rule=None, search_value=None, sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The language of the returned data.   
-        # Default value: CN for a China site and EN for an International site.
+        # The search value.
         self.accept_language = accept_language  # type: str
-        # The name of the database.
+        # {
+        #   "UserName":testUser
+        # }
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # zh-CN
         self.end_time = end_time  # type: str
-        # The filter condition.   
-        # > <br> - All fields in OceanBase Database support filtering. <br> - You can write the key-value pair of a parameter in a JSON string in the JSON format to filter the parameter.
-        self.filter_condition_shrink = filter_condition_shrink  # type: str
-        # The IP address of the node.
-        self.node_ip = node_ip  # type: str
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
-        self.page_number = page_number  # type: int
+        self.filter_condition_shrink = filter_condition_shrink  # type: str
         # The number of rows to return on each page.    
         # - Maximum value: 100   
         # - Default value: 10
+        self.node_ip = node_ip  # type: str
+        # desc
+        self.page_number = page_number  # type: int
+        # The start time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.page_size = page_size  # type: int
-        # SQLID.
+        # 1
         self.sqlid = sqlid  # type: str
         # The search keyword.
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # The ID of the tenant.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.   
-        # Valid values: "=", ">", ">=", "<", and "<="
+        # Utilization above threshold
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # 10
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The end time of the time range for querying suspicious SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The request time, in ms.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying suspicious SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The total count.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAnomalySQLListShrinkRequest, self).to_map()
@@ -3108,37 +2946,66 @@
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeAnomalySQLListResponseBodyAnomalySQLList(TeaModel):
     def __init__(self, cpu_time=None, db_name=None, diagnosis=None, diagnosis_rule=None, executions=None, key=None,
                  request_time=None, request_time_utcstring=None, sqlid=None, sqltext=None, suggestion=None, user_name=None):
-        # The average CPU time, in ms.
         self.cpu_time = cpu_time  # type: float
-        # The name of the database.
+        # {"name":"DescribeAnomalySQLList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":60000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeAnomalySQLList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"DbName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SearchKeyWord\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"update\"},{\"name\":\"SearchParameter\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SearchRule\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\">\"},{\"name\":\"SearchValue\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"0.01\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"NodeIp\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp19y05uq6xpacyqnlrc\"},{\"name\":\"AcceptLanguage\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"zh-CN\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"FilterCondition\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"enumValueTitles\":{\"UserName\":\"UserName\",\"Event\":\"Event\",\"SQLType\":\"SQLType\",\"ClientIp\":\"ClientIp\"},\"title\":\"\",\"description\":\"\",\"example\":\"{\\n  \\\"UserName\\\":testUser\\n}\"},{\"name\":\"SortColumn\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SortOrder\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"enumValueTitles\":{\"{     \\\"dbname\\\":test,     \\\"SQLType\\\":null\\t\\t }\":\"{     \\\"dbname\\\":test,     \\\"SQLType\\\":null\\t\\t }\"},\"title\":\"\",\"description\":\"\",\"example\":\"desc\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"AnomalySQLList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\" \",\"children\":[{\"name\":\"Key\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"DiagnosisRule\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"Suggestion\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"database1\"},{\"name\":\"RequestTimeUTCString\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2022-01-11T07:08:00Z\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"SQLId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"99E9D3BF****B486239E6C7BC79B****\"},{\"name\":\"Diagnosis\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\"},{\"name\":\"RequestTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.00\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"89043\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.db_name = db_name  # type: str
-        # The diagnosis information.
         self.diagnosis = diagnosis  # type: str
-        # The diagnostic rule.
+        # The list of suspicious SQL statements.
         self.diagnosis_rule = diagnosis_rule  # type: str
-        # The number of executions.
         self.executions = executions  # type: long
-        # The sequence number of the returned SQL statement.
+        # The average CPU time, in ms.
         self.key = key  # type: long
-        # The request time, in ms.
         self.request_time = request_time  # type: float
-        # The request time in UTC +0.
         self.request_time_utcstring = request_time_utcstring  # type: str
-        # SQLID.
         self.sqlid = sqlid  # type: str
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
         self.sqltext = sqltext  # type: str
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
         self.suggestion = suggestion  # type: str
-        # The username.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAnomalySQLListResponseBodyAnomalySQLList, self).to_map()
@@ -3199,19 +3066,19 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeAnomalySQLListResponseBody(TeaModel):
     def __init__(self, anomaly_sqllist=None, request_id=None, total_count=None):
-        # The list of suspicious SQL statements.
+        # The diagnostic rule.
         self.anomaly_sqllist = anomaly_sqllist  # type: list[DescribeAnomalySQLListResponseBodyAnomalySQLList]
-        # The request ID.
+        # The sorting rule.
         self.request_id = request_id  # type: str
-        # The total count.
+        # The SQL text.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.anomaly_sqllist:
             for k in self.anomaly_sqllist:
                 if k:
                     k.validate()
@@ -3283,23 +3150,26 @@
             temp_model = DescribeAnomalySQLListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAvailableCpuResourceRequest(TeaModel):
     def __init__(self, instance_id=None, modify_type=None, tenant_id=None):
-        # The ID of the OceanBase cluster.
+        # The CPU resources available.
         self.instance_id = instance_id  # type: str
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
         self.modify_type = modify_type  # type: str
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeAvailableCpuResource**.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAvailableCpuResourceRequest, self).to_map()
@@ -3324,19 +3194,16 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeAvailableCpuResourceResponseBodyData(TeaModel):
     def __init__(self, max_cpu=None, min_cpu=None, unit_num=None):
-        # The maximum number of CPU cores per resource unit.
         self.max_cpu = max_cpu  # type: long
-        # The minimum number of CPU cores per resource unit.
         self.min_cpu = min_cpu  # type: long
-        # The number of resource units in the tenant.
         self.unit_num = unit_num  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAvailableCpuResourceResponseBodyData, self).to_map()
@@ -3361,17 +3228,15 @@
         if m.get('UnitNum') is not None:
             self.unit_num = m.get('UnitNum')
         return self
 
 
 class DescribeAvailableCpuResourceResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The CPU resources available.
         self.data = data  # type: list[DescribeAvailableCpuResourceResponseBodyData]
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -3439,22 +3304,21 @@
             temp_model = DescribeAvailableCpuResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAvailableMemResourceRequest(TeaModel):
     def __init__(self, cpu_num=None, instance_id=None, tenant_id=None, unit_num=None):
-        # The number of CPU cores.
+        # The available memory size.
         self.cpu_num = cpu_num  # type: long
-        # The ID of the OceanBase cluster.
+        # The ID of the region.
         self.instance_id = instance_id  # type: str
         # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The number of resource distribution nodes in the tenant.   
-        # The number is determined by the deployment mode of the cluster. If the cluster is deployed in 2-2-2 mode, the maximum number of resource distribution nodes is 2.
+        # The number of resource units in the tenant.
         self.unit_num = unit_num  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAvailableMemResourceRequest, self).to_map()
@@ -3483,19 +3347,17 @@
         if m.get('UnitNum') is not None:
             self.unit_num = m.get('UnitNum')
         return self
 
 
 class DescribeAvailableMemResourceResponseBodyData(TeaModel):
     def __init__(self, max_mem=None, min_mem=None, used_mem=None):
-        # The maximum memory size for each resource unit, in GB.
         self.max_mem = max_mem  # type: long
-        # The minimum memory size required for each resource unit, in GB.
+        # You can call this operation to query the available memory resource of an OceanBase Database tenant.
         self.min_mem = min_mem  # type: long
-        # The number of resource units in the tenant.
         self.used_mem = used_mem  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAvailableMemResourceResponseBodyData, self).to_map()
@@ -3520,17 +3382,24 @@
         if m.get('UsedMem') is not None:
             self.used_mem = m.get('UsedMem')
         return self
 
 
 class DescribeAvailableMemResourceResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The available memory size.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeAvailableMemResource
+        # &InstanceId=ob317v4uif****\
+        # &TenantId=ob2mr3oae0****\
+        # &UnitNum=2
+        # &CpuNum=14
+        # &Common request parameters
+        # ```
         self.data = data  # type: DescribeAvailableMemResourceResponseBodyData
-        # The request ID.
+        # The number of CPU cores.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -3591,45 +3460,48 @@
         if m.get('body') is not None:
             temp_model = DescribeAvailableMemResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCharsetRequest(TeaModel):
-    def __init__(self, tenant_mode=None):
-        # The tenant mode.    
-        # Valid values: Oracle and MySQL.   
-        # For more information, see [DescribeInstanceTenantModes](~~410354~~).
+    def __init__(self, series=None, tenant_mode=None):
+        # 实例的系列  - normal（默认）：标准集群版（云盘）  - normal_ssd：标准集群版（本地盘） - history：历史库集群版。
+        self.series = series  # type: str
+        # The return result of the request.
         self.tenant_mode = tenant_mode  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCharsetRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.series is not None:
+            result['Series'] = self.series
         if self.tenant_mode is not None:
             result['TenantMode'] = self.tenant_mode
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('Series') is not None:
+            self.series = m.get('Series')
         if m.get('TenantMode') is not None:
             self.tenant_mode = m.get('TenantMode')
         return self
 
 
 class DescribeCharsetResponseBodyCharset(TeaModel):
     def __init__(self, charset=None, collations=None):
-        # The character set name.
+        # DescribeCharset
         self.charset = charset  # type: str
-        # The collation set.
         self.collations = collations  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCharsetResponseBodyCharset, self).to_map()
@@ -3650,17 +3522,22 @@
         if m.get('Collations') is not None:
             self.collations = m.get('Collations')
         return self
 
 
 class DescribeCharsetResponseBody(TeaModel):
     def __init__(self, charset=None, request_id=None):
-        # The list of character sets.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeCharset
+        # &TenantMode=Oracle
+        # &Common request parameters
+        # ```
         self.charset = charset  # type: list[DescribeCharsetResponseBodyCharset]
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeCharset**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.charset:
             for k in self.charset:
                 if k:
                     k.validate()
@@ -3729,31 +3606,30 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDatabasesRequest(TeaModel):
     def __init__(self, database_name=None, page_number=None, page_size=None, search_key=None, tenant_id=None,
                  with_tables=None):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.database_name = database_name  # type: str
-        # The number of the page to return.   
-        # - Start value: 1   
-        # - Default value: 1
+        # The return result of the request.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100.  
-        # - Default value: 10
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.page_size = page_size  # type: int
-        # The search keyword.
+        # The information about the database tables.
         self.search_key = search_key  # type: str
-        # The ID of the tenant.
+        # The request ID.
         self.tenant_id = tenant_id  # type: str
-        # Specifies whether to return the information of tables in the database.   
-        # Default value: false.
+        # The role of the account.    
+        # In MySQL mode, a role is a database-level role. Valid values:  
+        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.  
+        # - ReadOnly: a role that has only the read-only privilege SELECT.   
+        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
+        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.with_tables = with_tables  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDatabasesRequest, self).to_map()
@@ -3790,15 +3666,14 @@
         if m.get('WithTables') is not None:
             self.with_tables = m.get('WithTables')
         return self
 
 
 class DescribeDatabasesResponseBodyDatabasesTables(TeaModel):
     def __init__(self, table_name=None):
-        # The name of the database table.
         self.table_name = table_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDatabasesResponseBodyDatabasesTables, self).to_map()
@@ -3815,22 +3690,17 @@
         if m.get('TableName') is not None:
             self.table_name = m.get('TableName')
         return self
 
 
 class DescribeDatabasesResponseBodyDatabasesUsers(TeaModel):
     def __init__(self, role=None, user_name=None, user_type=None):
-        # The role of the account.    
-        # In MySQL mode, a role is a database-level role. Valid values:  
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.  
-        # - ReadOnly: a role that has only the read-only privilege SELECT.   
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.   
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
+        # The request ID.
         self.role = role  # type: str
-        # The name of the account.
+        # Example 1
         self.user_name = user_name  # type: str
         # The type of the account. Valid values:  - Admin: the super administrator account. - Normal: a general account.
         self.user_type = user_type  # type: str
 
     def validate(self):
         pass
 
@@ -3860,38 +3730,37 @@
 
 
 class DescribeDatabasesResponseBodyDatabases(TeaModel):
     def __init__(self, collation=None, create_time=None, data_size=None, database_name=None, db_type=None,
                  description=None, encoding=None, instance_id=None, required_size=None, status=None, tables=None, tenant_id=None,
                  users=None):
         self.collation = collation  # type: str
-        # The time when the database was created.
+        # Specifies whether to return the information of tables in the database.   
+        # Default value: false.
         self.create_time = create_time  # type: str
-        # The actual data size, in GB.
         self.data_size = data_size  # type: float
-        # The name of the database.
+        # The number of the page to return.   
+        # - Start value: 1   
+        # - Default value: 1
         self.database_name = database_name  # type: str
-        # The database type.
+        # The return result of the request.
         self.db_type = db_type  # type: str
-        # The description of the database.
+        # The name of the database.
         self.description = description  # type: str
-        # The encoding standard of the database. Encoding standards such as utf8mb4 and GBK are supported.
-        self.encoding = encoding  # type: str
-        self.instance_id = instance_id  # type: str
-        # The storage space required, in GB.
-        self.required_size = required_size  # type: float
         # The status of the database. Valid values:    
         # - ONLINE: The database is running.  
         # - DELETING: The database is being deleted.
+        self.encoding = encoding  # type: str
+        self.instance_id = instance_id  # type: str
+        self.required_size = required_size  # type: float
+        # The list of databases in the tenant.
         self.status = status  # type: str
-        # The information about the database tables.
         self.tables = tables  # type: list[DescribeDatabasesResponseBodyDatabasesTables]
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The accounts that have privileges on the database.
+        # The name of the database table.
         self.users = users  # type: list[DescribeDatabasesResponseBodyDatabasesUsers]
 
     def validate(self):
         if self.tables:
             for k in self.tables:
                 if k:
                     k.validate()
@@ -3973,19 +3842,18 @@
                 temp_model = DescribeDatabasesResponseBodyDatabasesUsers()
                 self.users.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDatabasesResponseBody(TeaModel):
     def __init__(self, databases=None, request_id=None, total_count=None):
-        # The list of databases in the tenant.
+        # The ID of the tenant.
         self.databases = databases  # type: list[DescribeDatabasesResponseBodyDatabases]
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The total number of databases in the tenant.
+        # The search keyword.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -4057,23 +3925,19 @@
             temp_model = DescribeDatabasesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceRequest(TeaModel):
     def __init__(self, instance_id=None, page_number=None, page_size=None):
-        # The ID of the OceanBase cluster.
+        # The size of the data disk, in GB.
         self.instance_id = instance_id  # type: str
-        # The number of the page to return. 
-        # - Start value: 1  
-        # - Default value: 1
+        # The information about the storage resources of the cluster.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The server with the highest disk usage.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceRequest, self).to_map()
@@ -4098,19 +3962,23 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeInstanceResponseBodyInstanceResourceCpu(TeaModel):
     def __init__(self, total_cpu=None, unit_cpu=None, used_cpu=None):
-        # The total number of CPU cores of the cluster.
+        # The series of the OceanBase cluster. Valid values:   
+        # - NORMAL: the high availability edition.   
+        # - BASIC: the basic edition.
         self.total_cpu = total_cpu  # type: long
-        # The number of CPU cores of each replica node in the cluster.
+        # The type of the storage disk where the cluster is deployed. 
+        # 
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.unit_cpu = unit_cpu  # type: long
-        # The number of CPU cores used in the cluster.
+        # Indicates whether automatic upgrade of the OBServer version is enabled.
         self.used_cpu = used_cpu  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceResponseBodyInstanceResourceCpu, self).to_map()
@@ -4136,25 +4004,34 @@
             self.used_cpu = m.get('UsedCpu')
         return self
 
 
 class DescribeInstanceResponseBodyInstanceResourceDiskSize(TeaModel):
     def __init__(self, data_used_size=None, max_disk_used_ob_server=None, max_disk_used_percent=None,
                  total_disk_size=None, unit_disk_size=None, used_disk_size=None):
-        # The size of the data disk, in GB.
+        # The ID of the OceanBase cluster.
         self.data_used_size = data_used_size  # type: float
-        # The server with the highest disk usage.
+        # The time in UTC when the cluster expires.
         self.max_disk_used_ob_server = max_disk_used_ob_server  # type: list[str]
         # The maximum disk usage, in percentage.
         self.max_disk_used_percent = max_disk_used_percent  # type: float
-        # The total storage space of the cluster, in GB.
+        # The data replica distribution mode of the cluster. Valid values: 
+        # - n: indicates the single-IDC mode. 
+        # - n-n: indicates the dual-IDC mode. 
+        # - n-n-n: indicates the multi-IDC mode. 
+        # 
+        # > <br>The integer n represents the number of OBServer nodes in each IDC.
         self.total_disk_size = total_disk_size  # type: long
-        # The storage space of each replica node in the cluster, in GB.
+        # The list of zones.
         self.unit_disk_size = unit_disk_size  # type: long
-        # The size of used storage space of the cluster, in GB.
+        # The specifications of the cluster.  You can specify one of the following four plans:    
+        # - 8C32G: indicates 8 CPU cores and 32 GB of memory. 
+        # - 14C70G: indicates 14 CPU cores and 70 GB of memory. 
+        # - 30C180G: indicates 30 CPU cores and 180 GB of memory. 
+        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
         self.used_disk_size = used_disk_size  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceResponseBodyInstanceResourceDiskSize, self).to_map()
@@ -4191,17 +4068,17 @@
         if m.get('UsedDiskSize') is not None:
             self.used_disk_size = m.get('UsedDiskSize')
         return self
 
 
 class DescribeInstanceResponseBodyInstanceResourceLogDiskSize(TeaModel):
     def __init__(self, total_disk_size=None, unit_disk_size=None):
-        # The total log disk space of the cluster, in GB.
+        # The ID of the region.
         self.total_disk_size = total_disk_size  # type: long
-        # The log disk space of each replica node in the cluster. Unit: GB.
+        # The request ID.
         self.unit_disk_size = unit_disk_size  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceResponseBodyInstanceResourceLogDiskSize, self).to_map()
@@ -4222,19 +4099,19 @@
         if m.get('UnitDiskSize') is not None:
             self.unit_disk_size = m.get('UnitDiskSize')
         return self
 
 
 class DescribeInstanceResponseBodyInstanceResourceMemory(TeaModel):
     def __init__(self, total_memory=None, unit_memory=None, used_memory=None):
-        # The total memory size of the cluster, in GB.
+        # Indicates whether trusted ECS instances are used.
         self.total_memory = total_memory  # type: long
-        # The memory size of each replica node in the cluster, in GB.
+        # The log disk space of each replica node in the cluster. Unit: GB.
         self.unit_memory = unit_memory  # type: long
-        # The size of used memory in the cluster, in GB.
+        # The time in UTC when the cluster was created.
         self.used_memory = used_memory  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceResponseBodyInstanceResourceMemory, self).to_map()
@@ -4259,23 +4136,25 @@
         if m.get('UsedMemory') is not None:
             self.used_memory = m.get('UsedMemory')
         return self
 
 
 class DescribeInstanceResponseBodyInstanceResource(TeaModel):
     def __init__(self, cpu=None, disk_size=None, log_disk_size=None, memory=None, unit_count=None):
-        # The information about the CPU resources of the cluster.
+        # The information of the OceanBase cluster.
         self.cpu = cpu  # type: DescribeInstanceResponseBodyInstanceResourceCpu
-        # The information about the storage resources of the cluster.
+        # The number of the page to return. 
+        # - Start value: 1  
+        # - Default value: 1
         self.disk_size = disk_size  # type: DescribeInstanceResponseBodyInstanceResourceDiskSize
-        # The information about the log disk space of the cluster.
+        # The server with the highest disk usage.
         self.log_disk_size = log_disk_size  # type: DescribeInstanceResponseBodyInstanceResourceLogDiskSize
-        # The information about the memory resources of the cluster.
+        # The name of the OceanBase cluster.
         self.memory = memory  # type: DescribeInstanceResponseBodyInstanceResourceMemory
-        # The number of resource units in the cluster.
+        # The number of CPU cores used in the cluster.
         self.unit_count = unit_count  # type: long
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -4319,98 +4198,62 @@
         if m.get('UnitCount') is not None:
             self.unit_count = m.get('UnitCount')
         return self
 
 
 class DescribeInstanceResponseBodyInstance(TeaModel):
     def __init__(self, auto_renewal=None, auto_upgrade_ob_version=None, available_zones=None, create_time=None,
-                 data_merge_time=None, deploy_mode=None, deploy_type=None, disk_type=None, enable_upgrade_log_disk=None,
-                 expire_time=None, instance_class=None, instance_id=None, instance_name=None, instance_role=None,
-                 is_latest_ob_version=None, is_trust_ecs=None, maintain_time=None, node_num=None, ob_rpm_version=None, pay_type=None,
-                 resource=None, series=None, status=None, version=None, zones=None):
-        # Indicates whether automatic renewal is enabled. 
-        # 
-        # This parameter is valid only for clusters whose billing methods are set to PREPAY.
+                 data_merge_time=None, deploy_mode=None, deploy_type=None, disk_type=None, enable_isolation_optimization=None,
+                 enable_upgrade_log_disk=None, expire_time=None, instance_class=None, instance_id=None, instance_name=None,
+                 instance_role=None, is_latest_ob_version=None, is_trust_ecs=None, isolation_optimization=None,
+                 maintain_time=None, node_num=None, ob_rpm_version=None, pay_type=None, resource=None, series=None, status=None,
+                 version=None, zones=None):
+        # The operation that you want to perform. <br>Set the value to **DescribeInstance**.
         self.auto_renewal = auto_renewal  # type: bool
-        # Indicates whether automatic upgrade of the OBServer version is enabled.
+        # Example 1
         self.auto_upgrade_ob_version = auto_upgrade_ob_version  # type: bool
-        # The list of zones.
         self.available_zones = available_zones  # type: list[str]
-        # The time in UTC when the cluster was created.
+        # Indicates whether the log disk specifications can be upgraded.
         self.create_time = create_time  # type: str
-        # The time when the major compaction of cluster data is performed.
+        # The total number of CPU cores of the cluster.
         self.data_merge_time = data_merge_time  # type: str
-        # The data replica distribution mode of the cluster. Valid values: 
-        # - n: indicates the single-IDC mode. 
-        # - n-n: indicates the dual-IDC mode. 
-        # - n-n-n: indicates the multi-IDC mode. 
-        # 
-        # > <br>The integer n represents the number of OBServer nodes in each IDC.
+        # Alibaba Cloud CLI
         self.deploy_mode = deploy_mode  # type: str
-        # The deployment type of the cluster. Valid values:  
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.deploy_type = deploy_type  # type: str
-        # The type of the storage disk where the cluster is deployed. 
-        # 
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
+        # The total storage space of the cluster, in GB.
         self.disk_type = disk_type  # type: str
-        # Indicates whether the log disk specifications can be upgraded.
+        self.enable_isolation_optimization = enable_isolation_optimization  # type: bool
         self.enable_upgrade_log_disk = enable_upgrade_log_disk  # type: bool
-        # The time in UTC when the cluster expires.
+        # The information of the OceanBase cluster.
         self.expire_time = expire_time  # type: str
-        # The specifications of the cluster.  You can specify one of the following four plans:    
-        # - 8C32G: indicates 8 CPU cores and 32 GB of memory. 
-        # - 14C70G: indicates 14 CPU cores and 70 GB of memory. 
-        # - 30C180G: indicates 30 CPU cores and 180 GB of memory. 
-        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
+        # The detailed information of the OBServer version.
         self.instance_class = instance_class  # type: str
-        # The ID of the OceanBase cluster.
+        # The information about the log disk space of the cluster.
         self.instance_id = instance_id  # type: str
-        # The name of the OceanBase cluster.
+        # Indicates whether automatic upgrade of the OBServer version is enabled.
         self.instance_name = instance_name  # type: str
         self.instance_role = instance_role  # type: str
-        # Indicates whether the OBServer version is the latest.
         self.is_latest_ob_version = is_latest_ob_version  # type: bool
-        # Indicates whether trusted ECS instances are used.
+        # The information about the CPU resources of the cluster.
         self.is_trust_ecs = is_trust_ecs  # type: bool
-        # The time period in UTC for the daily routine maintenance of the cluster.
+        self.isolation_optimization = isolation_optimization  # type: bool
+        # The time when the major compaction of cluster data is performed.
         self.maintain_time = maintain_time  # type: str
         self.node_num = node_num  # type: str
-        # The detailed information of the OBServer version.
         self.ob_rpm_version = ob_rpm_version  # type: str
-        # The billing method of the OceanBase cluster. Valid values: 
-        # - PREPAY: the subscription billing method. 
-        # - POSTPAY: the pay-as-you-go billing method.
+        # The list of zones.
         self.pay_type = pay_type  # type: str
-        # The information about cluster resources.
+        # The size of used memory in the cluster, in GB.
         self.resource = resource  # type: DescribeInstanceResponseBodyInstanceResource
-        # The series of the OceanBase cluster. Valid values:   
-        # - NORMAL: the high availability edition.   
-        # - BASIC: the basic edition.
+        # Indicates whether the OBServer version is the latest.
         self.series = series  # type: str
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
         self.status = status  # type: str
-        # The OBServer version.
+        # You can call this operation to query the detailed information of an OceanBase cluster.
         self.version = version  # type: str
         self.zones = zones  # type: list[str]
 
     def validate(self):
         if self.resource:
             self.resource.validate()
 
@@ -4432,14 +4275,16 @@
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
@@ -4448,14 +4293,16 @@
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
@@ -4486,14 +4333,16 @@
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
@@ -4502,14 +4351,16 @@
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
@@ -4526,17 +4377,17 @@
         if m.get('Zones') is not None:
             self.zones = m.get('Zones')
         return self
 
 
 class DescribeInstanceResponseBody(TeaModel):
     def __init__(self, instance=None, request_id=None):
-        # The information of the OceanBase cluster.
+        # The log disk space of each replica node in the cluster. Unit: GB.
         self.instance = instance  # type: DescribeInstanceResponseBodyInstance
-        # The request ID.
+        # The total log disk space of the cluster, in GB.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.instance:
             self.instance.validate()
 
     def to_map(self):
@@ -4598,15 +4449,15 @@
             temp_model = DescribeInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceCreatableZoneRequest(TeaModel):
     def __init__(self, instance_id=None):
-        # The ID of the OceanBase cluster.
+        # The ID of the zone.
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceCreatableZoneRequest, self).to_map()
@@ -4623,17 +4474,16 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class DescribeInstanceCreatableZoneResponseBodyZoneList(TeaModel):
     def __init__(self, is_in_cluster=None, zone=None):
-        # Indicates whether the cluster is deployed in the zone.
         self.is_in_cluster = is_in_cluster  # type: bool
-        # The ID of the zone.
+        # DescribeInstanceCreatableZone
         self.zone = zone  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceCreatableZoneResponseBodyZoneList, self).to_map()
@@ -4654,17 +4504,18 @@
         if m.get('Zone') is not None:
             self.zone = m.get('Zone')
         return self
 
 
 class DescribeInstanceCreatableZoneResponseBody(TeaModel):
     def __init__(self, request_id=None, zone_list=None):
-        # The request ID.
+        # Indicates whether the cluster is deployed in the zone.
         self.request_id = request_id  # type: str
-        # The list of zones.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceCreatableZone**.
         self.zone_list = zone_list  # type: list[DescribeInstanceCreatableZoneResponseBodyZoneList]
 
     def validate(self):
         if self.zone_list:
             for k in self.zone_list:
                 if k:
                     k.validate()
@@ -4913,17 +4764,17 @@
             temp_model = DescribeInstanceSecurityConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceTagsRequest(TeaModel):
     def __init__(self, instance_ids=None, tags=None):
-        # The list of cluster IDs.
+        # The list of tags.
         self.instance_ids = instance_ids  # type: str
-        # The tags.
+        # The returned response.
         self.tags = tags  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTagsRequest, self).to_map()
@@ -4944,19 +4795,17 @@
         if m.get('Tags') is not None:
             self.tags = m.get('Tags')
         return self
 
 
 class DescribeInstanceTagsResponseBodyTagResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag=None):
-        # The resource ID.
+        # You can call this operation to view the tag value of a cluster.
         self.resource_id = resource_id  # type: str
-        # The type of the resource.
         self.resource_type = resource_type  # type: str
-        # The tag of the resource.
         self.tag = tag  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTagsResponseBodyTagResources, self).to_map()
@@ -4981,17 +4830,17 @@
         if m.get('Tag') is not None:
             self.tag = m.get('Tag')
         return self
 
 
 class DescribeInstanceTagsResponseBody(TeaModel):
     def __init__(self, request_id=None, tag_resources=None):
-        # The request ID.
+        # The resource ID.
         self.request_id = request_id  # type: str
-        # The list of tags.
+        # The request ID.
         self.tag_resources = tag_resources  # type: list[DescribeInstanceTagsResponseBodyTagResources]
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -5059,15 +4908,16 @@
             temp_model = DescribeInstanceTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceTenantModesRequest(TeaModel):
     def __init__(self, instance_id=None):
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceTenantModes**.
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTenantModesRequest, self).to_map()
@@ -5084,17 +4934,15 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class DescribeInstanceTenantModesResponseBody(TeaModel):
     def __init__(self, instance_modes=None, request_id=None):
-        # The information of tenants.
         self.instance_modes = instance_modes  # type: list[str]
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTenantModesResponseBody, self).to_map()
@@ -5154,15 +5002,15 @@
             temp_model = DescribeInstanceTenantModesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceTopologyRequest(TeaModel):
     def __init__(self, instance_id=None):
-        # The ID of the OceanBase cluster.
+        # The status of the node.
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyRequest, self).to_map()
@@ -5183,36 +5031,30 @@
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZonesUnits(TeaModel):
     def __init__(self, enable_cancel_migrate_unit=None, enable_migrate_unit=None, manual_migrate=None,
                  node_id=None, unit_cpu=None, unit_data_size=None, unit_id=None, unit_memory=None, unit_status=None):
         # Indicates whether the migration can be canceled.   
         # This field is valid only for units that are being manually immigrated or emigrated.
         self.enable_cancel_migrate_unit = enable_cancel_migrate_unit  # type: bool
-        # Indicates whether migration can be performed.
+        # The return result of the request.
         self.enable_migrate_unit = enable_migrate_unit  # type: bool
-        # Indicates whether the migration is manually performed.
+        # The return result of the request.
         self.manual_migrate = manual_migrate  # type: bool
-        # The ID of the OBServer where the resource unit resides.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.node_id = node_id  # type: str
-        # The number of CPU cores of the resource unit.
+        # Alibaba Cloud CLI
         self.unit_cpu = unit_cpu  # type: float
-        # The data size of the unit.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeInstanceTopology**.
         self.unit_data_size = unit_data_size  # type: long
-        # The ID of the resource unit.
+        # The topology of the cluster.
         self.unit_id = unit_id  # type: str
-        # The memory size of the resource unit, in GB.
+        # The ID of the tenant.
         self.unit_memory = unit_memory  # type: float
-        # The status of the resource unit. Valid values:    
-        # 
-        # - ONLINE: The resource unit is running.
-        # - IMMIGRATING: The resource unit is being immigrated.
-        # - EMIGRATING: The resource unit is being emigrated.
-        # - CANCEL_EMIGRATING: Resource node immigration is being canceled.
-        # - CANCEL_EMIGRATING: Resource node emigration is being canceled.
-        # - DELETING: The resource unit is being deleted.
+        # You can call this operation to query the topology of an OceanBase cluster.
         self.unit_status = unit_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZonesUnits, self).to_map()
@@ -5261,23 +5103,21 @@
         if m.get('UnitStatus') is not None:
             self.unit_status = m.get('UnitStatus')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZones(TeaModel):
     def __init__(self, is_primary_tenant_zone=None, tenant_zone_id=None, tenant_zone_role=None, units=None):
-        # Indicates whether the zone is the primary zone.
+        # The maximum disk usage, in percentage.
         self.is_primary_tenant_zone = is_primary_tenant_zone  # type: str
-        # The ID of the zone.
+        # The server with the highest disk usage.
         self.tenant_zone_id = tenant_zone_id  # type: str
-        # The role to access the zone. Valid values:   
-        #  - ReadWrite: a role that has the read and write privileges.
-        #  - ReadOnly: a role that has only the read-only privilege.
+        # The information of zones.
         self.tenant_zone_role = tenant_zone_role  # type: str
-        # The information about resource units.
+        # The information about the storage resources.
         self.units = units  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZonesUnits]
 
     def validate(self):
         if self.units:
             for k in self.units:
                 if k:
                     k.validate()
@@ -5316,47 +5156,33 @@
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyTenants(TeaModel):
     def __init__(self, primary_zone_deploy_type=None, tenant_cpu=None, tenant_deploy_type=None, tenant_id=None,
                  tenant_memory=None, tenant_mode=None, tenant_name=None, tenant_status=None, tenant_unit_num=None,
                  tenant_zones=None):
-        # The deployment type of the primary zone.
+        # The server with the highest disk usage.
         self.primary_zone_deploy_type = primary_zone_deploy_type  # type: str
-        # The number of CPU cores of the tenant.
+        # The information about the memory resources of the node.
         self.tenant_cpu = tenant_cpu  # type: float
-        # The deployment type of the tenant.   
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The name of the tenant.
         self.tenant_deploy_type = tenant_deploy_type  # type: str
-        # The ID of the tenant.
+        # The size of used memory of the node, in GB.
         self.tenant_id = tenant_id  # type: str
-        # The memory size of the tenant, in GB.
+        # The total storage space of the node, in GB.
         self.tenant_memory = tenant_memory  # type: float
-        # The tenant mode. Valid values:   
-        # - Oracle   
-        # - MySQL
+        # The size of used storage space of the node, in GB.
         self.tenant_mode = tenant_mode  # type: str
-        # The name of the tenant.
+        # The total memory size of the node, in GB.
         self.tenant_name = tenant_name  # type: str
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
         self.tenant_status = tenant_status  # type: str
-        # The number of resource units in the tenant.
+        # The number of CPU cores of the tenant.
         self.tenant_unit_num = tenant_unit_num  # type: int
-        # The zone information of the tenant.
+        # The information about the storage resources of the node.
         self.tenant_zones = tenant_zones  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZones]
 
     def validate(self):
         if self.tenant_zones:
             for k in self.tenant_zones:
                 if k:
                     k.validate()
@@ -5417,17 +5243,17 @@
                 temp_model = DescribeInstanceTopologyResponseBodyInstanceTopologyTenantsTenantZones()
                 self.tenant_zones.append(temp_model.from_map(k))
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceCpu(TeaModel):
     def __init__(self, total_cpu=None, used_cpu=None):
-        # The total number of CPU cores for the node.
+        # The size of used storage space of the node, in GB.
         self.total_cpu = total_cpu  # type: int
-        # The number of CPU cores used by the node.
+        # Indicates whether migration can be performed.
         self.used_cpu = used_cpu  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceCpu, self).to_map()
@@ -5448,17 +5274,26 @@
         if m.get('UsedCpu') is not None:
             self.used_cpu = m.get('UsedCpu')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceDiskSize(TeaModel):
     def __init__(self, total_disk_size=None, used_disk_size=None):
-        # The total storage space of the node, in GB.
+        # The deployment type of the primary zone.
         self.total_disk_size = total_disk_size  # type: float
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
         self.used_disk_size = used_disk_size  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceDiskSize, self).to_map()
@@ -5479,17 +5314,17 @@
         if m.get('UsedDiskSize') is not None:
             self.used_disk_size = m.get('UsedDiskSize')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory(TeaModel):
     def __init__(self, total_memory=None, used_memory=None):
-        # The total memory size of the node, in GB.
+        # The ID of the replica node.
         self.total_memory = total_memory  # type: long
-        # The size of used memory of the node, in GB.
+        # The information of node resources.
         self.used_memory = used_memory  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory, self).to_map()
@@ -5510,19 +5345,21 @@
         if m.get('UsedMemory') is not None:
             self.used_memory = m.get('UsedMemory')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResource(TeaModel):
     def __init__(self, cpu=None, disk_size=None, memory=None):
-        # The information about the CPU resources of the node.
+        # The memory size of the tenant, in GB.
         self.cpu = cpu  # type: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceCpu
-        # The information about the storage resources of the node.
+        # The information about the CPU resources of the node.
         self.disk_size = disk_size  # type: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceDiskSize
-        # The information about the memory resources of the node.
+        # The role to access the zone. Valid values:   
+        #  - ReadWrite: a role that has the read and write privileges.
+        #  - ReadOnly: a role that has only the read-only privilege.
         self.memory = memory  # type: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -5555,21 +5392,21 @@
             temp_model = DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResourceMemory()
             self.memory = temp_model.from_map(m['Memory'])
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodes(TeaModel):
     def __init__(self, node_copy_id=None, node_id=None, node_resource=None, node_status=None):
-        # The ID of the replica node.
+        # The information of zones.
         self.node_copy_id = node_copy_id  # type: long
-        # The ID of the node.
+        # The ID of the resource unit.
         self.node_id = node_id  # type: str
-        # The information of node resources.
+        # The ID of the node.
         self.node_resource = node_resource  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodesNodeResource]
-        # The status of the node.
+        # The ID of the OBServer where the resource unit resides.
         self.node_status = node_status  # type: str
 
     def validate(self):
         if self.node_resource:
             for k in self.node_resource:
                 if k:
                     k.validate()
@@ -5606,17 +5443,16 @@
         if m.get('NodeStatus') is not None:
             self.node_status = m.get('NodeStatus')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize(TeaModel):
     def __init__(self, max_disk_used_ob_server=None, max_disk_used_percent=None):
-        # The server with the highest disk usage.
         self.max_disk_used_ob_server = max_disk_used_ob_server  # type: list[str]
-        # The maximum disk usage, in percentage.
+        # DescribeInstanceTopology
         self.max_disk_used_percent = max_disk_used_percent  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize, self).to_map()
@@ -5637,15 +5473,14 @@
         if m.get('MaxDiskUsedPercent') is not None:
             self.max_disk_used_percent = m.get('MaxDiskUsedPercent')
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResource(TeaModel):
     def __init__(self, disk_size=None):
-        # The information about the storage resources of the node.
         self.disk_size = disk_size  # type: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize
 
     def validate(self):
         if self.disk_size:
             self.disk_size.validate()
 
     def to_map(self):
@@ -5664,23 +5499,23 @@
             temp_model = DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResourceDiskSize()
             self.disk_size = temp_model.from_map(m['DiskSize'])
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopologyZones(TeaModel):
     def __init__(self, nodes=None, region=None, zone_disk=None, zone_id=None, zone_resource=None):
-        # The information of the nodes.
-        self.nodes = nodes  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodes]
         # The ID of the region.
+        self.nodes = nodes  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyZonesNodes]
+        # The zone information of the cluster.
         self.region = region  # type: str
-        # The storage capacity of the zone.
+        # The information about the memory resources of the node.
         self.zone_disk = zone_disk  # type: str
-        # The ID of the zone.
+        # The information of the tenant.
         self.zone_id = zone_id  # type: str
-        # The information of zones.
+        # Example 1
         self.zone_resource = zone_resource  # type: DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResource
 
     def validate(self):
         if self.nodes:
             for k in self.nodes:
                 if k:
                     k.validate()
@@ -5724,17 +5559,17 @@
             temp_model = DescribeInstanceTopologyResponseBodyInstanceTopologyZonesZoneResource()
             self.zone_resource = temp_model.from_map(m['ZoneResource'])
         return self
 
 
 class DescribeInstanceTopologyResponseBodyInstanceTopology(TeaModel):
     def __init__(self, tenants=None, zones=None):
-        # The information of the tenant.
+        # The total number of CPU cores for the node.
         self.tenants = tenants  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyTenants]
-        # The zone information of the cluster.
+        # The information about resource units.
         self.zones = zones  # type: list[DescribeInstanceTopologyResponseBodyInstanceTopologyZones]
 
     def validate(self):
         if self.tenants:
             for k in self.tenants:
                 if k:
                     k.validate()
@@ -5772,17 +5607,17 @@
                 temp_model = DescribeInstanceTopologyResponseBodyInstanceTopologyZones()
                 self.zones.append(temp_model.from_map(k))
         return self
 
 
 class DescribeInstanceTopologyResponseBody(TeaModel):
     def __init__(self, instance_topology=None, request_id=None):
-        # The topology of the cluster.
+        # The number of CPU cores used by the node.
         self.instance_topology = instance_topology  # type: DescribeInstanceTopologyResponseBodyInstanceTopology
-        # The request ID.
+        # The information about the CPU resources of the node.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.instance_topology:
             self.instance_topology.validate()
 
     def to_map(self):
@@ -5845,32 +5680,25 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstancesRequest(TeaModel):
     def __init__(self, instance_id=None, instance_name=None, page_number=None, page_size=None,
                  resource_group_id=None, search_key=None):
-        # The ID of the OceanBase cluster.
+        # The number of CPU cores used in the cluster.
         self.instance_id = instance_id  # type: str
-        # The name of the OceanBase cluster.    
-        # It must be 1 to 20 characters in length.   
-        # If this parameter is not specified, the value is the instance ID of the cluster by default.
+        # The size of used memory in the cluster, in GB.
         self.instance_name = instance_name  # type: str
-        # The number of the page to return.    
-        # 
-        # - Start value: 1 
-        # - Default value: 1
+        # The total memory size of the cluster, in GB.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.    
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The information about the memory resources of the cluster.
         self.page_size = page_size  # type: int
-        # The ID of the resource group.
+        # The number of CPU cores of each replica node in the cluster.
         self.resource_group_id = resource_group_id  # type: str
-        # The search keyword.
+        # The memory size of each replica node in the cluster, in GB.
         self.search_key = search_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesRequest, self).to_map()
@@ -5907,19 +5735,25 @@
         if m.get('SearchKey') is not None:
             self.search_key = m.get('SearchKey')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceCpu(TeaModel):
     def __init__(self, total_cpu=None, unit_cpu=None, used_cpu=None):
-        # The total number of CPU cores of the cluster.
+        # The name of the OceanBase cluster.    
+        # It must be 1 to 20 characters in length.   
+        # If this parameter is not specified, the value is the instance ID of the cluster by default.
         self.total_cpu = total_cpu  # type: long
-        # The number of CPU cores of each replica node in the cluster.
+        # The data replica distribution mode of the cluster. Valid values:    
+        # 
+        # - n: indicates the single-IDC mode.  
+        # - n-n: indicates the dual-IDC mode.  
+        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
         self.unit_cpu = unit_cpu  # type: long
-        # The number of CPU cores used in the cluster.
+        # The search keyword.
         self.used_cpu = used_cpu  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesResourceCpu, self).to_map()
@@ -5944,19 +5778,19 @@
         if m.get('UsedCpu') is not None:
             self.used_cpu = m.get('UsedCpu')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceDiskSize(TeaModel):
     def __init__(self, total_disk_size=None, unit_disk_size=None, used_disk_size=None):
-        # The total storage space of the cluster, in GB.
+        # The request ID.
         self.total_disk_size = total_disk_size  # type: long
-        # The storage space of each replica node in the cluster, in GB.
+        # Example 1
         self.unit_disk_size = unit_disk_size  # type: long
-        # The size of used storage space of the cluster, in GB.
+        # $.parameters[7].schema.example
         self.used_disk_size = used_disk_size  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesResourceDiskSize, self).to_map()
@@ -5981,17 +5815,17 @@
         if m.get('UsedDiskSize') is not None:
             self.used_disk_size = m.get('UsedDiskSize')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResourceMemory(TeaModel):
     def __init__(self, total_memory=None, unit_memory=None, used_memory=None):
-        # The total memory size of the cluster, in GB.
+        # The number of CPU cores of the cluster.
         self.total_memory = total_memory  # type: long
-        # The memory size of each replica node in the cluster, in GB.
+        # The size of used storage space of the cluster, in GB.
         self.unit_memory = unit_memory  # type: long
         # The size of used memory in the cluster, in GB.
         self.used_memory = used_memory  # type: long
 
     def validate(self):
         pass
 
@@ -6018,21 +5852,35 @@
         if m.get('UsedMemory') is not None:
             self.used_memory = m.get('UsedMemory')
         return self
 
 
 class DescribeInstancesResponseBodyInstancesResource(TeaModel):
     def __init__(self, cpu=None, disk_size=None, memory=None, unit_count=None):
-        # The information about the CPU resources of the cluster.
+        # Indicates whether new nodes can be added.
         self.cpu = cpu  # type: DescribeInstancesResponseBodyInstancesResourceCpu
-        # The information about the storage resources of the cluster.
+        # The time elapsed since the expiration of the cluster, in seconds.
         self.disk_size = disk_size  # type: DescribeInstancesResponseBodyInstancesResourceDiskSize
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
         self.memory = memory  # type: DescribeInstancesResponseBodyInstancesResourceMemory
-        # The number of resource units in the cluster.
         self.unit_count = unit_count  # type: long
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -6073,98 +5921,73 @@
 
 class DescribeInstancesResponseBodyInstances(TeaModel):
     def __init__(self, available_zones=None, commodity_code=None, cpu=None, create_time=None, deploy_mode=None,
                  deploy_type=None, disk_size=None, disk_type=None, enable_upgrade_nodes=None, expire_seconds=None,
                  expire_time=None, instance_class=None, instance_id=None, instance_name=None, instance_role=None,
                  instance_type=None, maintain_time=None, mem=None, pay_type=None, resource=None, resource_group_id=None,
                  security_ips=None, series=None, state=None, used_disk_size=None, version=None, vpc_id=None):
-        # The information about the zone in which the cluster is deployed.
+        # The time in UTC when the cluster expires.
         self.available_zones = available_zones  # type: list[str]
+        # The storage space of each replica node in the cluster, in GB.
+        self.commodity_code = commodity_code  # type: str
         # The product code of the OceanBase cluster.   
         # - oceanbase_oceanbasepre_public_cn: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in a China site.  
         # - oceanbase_oceanbasepost_public_cn: indicates an OceanBase cluster that is billed based on the pay-as-you-go plan and that is deployed in a China site.  
         # - oceanbase_obpre_public_intl: indicates an OceanBase cluster that is billed based on the subscription plan and that is deployed in an international site.
-        self.commodity_code = commodity_code  # type: str
-        # The number of CPU cores of the cluster.
         self.cpu = cpu  # type: int
-        # The time in UTC when the cluster was created.
+        # The number of OceanBase clusters queried.
         self.create_time = create_time  # type: str
-        # The data replica distribution mode of the cluster. Valid values:    
-        # 
-        # - n: indicates the single-IDC mode.  
-        # - n-n: indicates the dual-IDC mode.  
-        # - n-n-n: indicates the multi-IDC mode. The integer n represents the number of OBServer nodes in each IDC.
+        # The request ID.
         self.deploy_mode = deploy_mode  # type: str
-        # The deployment type of the cluster. Valid values:   
-        # - multiple: multi-IDC deployment  
-        # - single: single-IDC deployment  
-        # - dual: dual-IDC deployment
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.deploy_type = deploy_type  # type: str
-        # The size of the storage space, in GB.
+        # The information about the memory resources of the cluster.
         self.disk_size = disk_size  # type: str
-        # The type of the storage disk where the cluster is deployed.   
-        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
+        # The number of CPU cores used in the cluster.
         self.disk_type = disk_type  # type: str
-        # Indicates whether new nodes can be added.
+        # The ID of the OceanBase cluster.
         self.enable_upgrade_nodes = enable_upgrade_nodes  # type: bool
-        # The time elapsed since the expiration of the cluster, in seconds.
+        # The whitelist information of the cluster.
         self.expire_seconds = expire_seconds  # type: int
-        # The time in UTC when the cluster expires.
+        # The information about the storage resources of the cluster.
         self.expire_time = expire_time  # type: str
-        # The specifications of the cluster.  You can specify one of the following four plans:  
-        # - 8C32G: indicates 8 CPU cores and 32 GB of memory.  
-        # - 14C70G: indicates 14 CPU cores and 70 GB of memory.  
-        # - 30C180G: indicates 30 CPU cores and 180 GB of memory.  
-        # - 62C400G: indicates 62 CPU cores and 400 GB of memory.
+        # The instance type.
         self.instance_class = instance_class  # type: str
-        # The ID of the OceanBase cluster.
+        # The total storage space of the cluster, in GB.
         self.instance_id = instance_id  # type: str
-        # The name of the OceanBase cluster.
+        # The return result of the request.
         self.instance_name = instance_name  # type: str
         self.instance_role = instance_role  # type: str
-        # The instance type.
+        # You can call this operation to obtain the list of OceanBase clusters.
         self.instance_type = instance_type  # type: str
-        # The time period in UTC for the daily routine maintenance of the cluster.
+        # The return result of the request.
         self.maintain_time = maintain_time  # type: str
-        # The memory size of the instance, in GB.
+        # The information about the CPU resources of the cluster.
         self.mem = mem  # type: long
-        # The billing method for the OceanBase cluster. Valid values:  
-        # - PREPAY: the subscription billing method.  
-        # - POSTPAY: the pay-as-you-go billing method.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.pay_type = pay_type  # type: str
-        # The information about cluster resources.
+        # The type of the storage disk where the cluster is deployed.   
+        # The default value is cloud_essd_pl1, which indicates an ESSD cloud disk.
         self.resource = resource  # type: DescribeInstancesResponseBodyInstancesResource
-        # The ID of the resource group.
+        # The number of OceanBase clusters queried.
         self.resource_group_id = resource_group_id  # type: str
-        # The whitelist information of the cluster.
+        # The number of the page to return.    
+        # 
+        # - Start value: 1 
+        # - Default value: 1
         self.security_ips = security_ips  # type: list[str]
-        # The series of the OceanBase cluster. Valid values:   
-        # - NORMAL: the high availability edition.   
-        # - BASIC: the basic edition.
+        # The billing method for the OceanBase cluster. Valid values:  
+        # - PREPAY: the subscription billing method.  
+        # - POSTPAY: the pay-as-you-go billing method.
         self.series = series  # type: str
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
         self.state = state  # type: str
-        # The size of used storage space of the cluster, in GB.
+        # The number of resource units in the cluster.
         self.used_disk_size = used_disk_size  # type: long
-        # The OBServer version.
+        # The total number of CPU cores of the cluster.
         self.version = version  # type: str
         # vpcId
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.resource:
             self.resource.validate()
@@ -6289,19 +6112,17 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeInstancesResponseBody(TeaModel):
     def __init__(self, instances=None, request_id=None, total_count=None):
-        # The information of the OceanBase cluster.
+        # The total storage space of the cluster, in GB.
         self.instances = instances  # type: list[DescribeInstancesResponseBodyInstances]
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The number of OceanBase clusters queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -6374,38 +6195,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeNodeMetricsRequest(TeaModel):
     def __init__(self, end_time=None, instance_id=None, metrics=None, node_id_list=None, node_name=None,
                  page_number=None, page_size=None, start_time=None, tenant_id=None):
-        # The end time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # $.parameters[7].schema.description
         self.end_time = end_time  # type: str
-        # The ID of the OceanBase cluster.
+        # The list of nodes.
         self.instance_id = instance_id  # type: str
-        # The monitoring metrics.     
-        # For more information about supported metrics, see [Node statistics](~~212099~~).
+        # $.parameters[7].schema.enumValueTitles
         self.metrics = metrics  # type: str
-        # The list of nodes.
+        # $.parameters[10].schema.description
         self.node_id_list = node_id_list  # type: str
-        # The name of the node.
+        # $.parameters[8].schema.example
         self.node_name = node_name  # type: str
-        # The number of the page to return.   
-        # - Start value: 1   
-        # - Default value: 1
+        # $.parameters[6].schema.description
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The ID of the tenant.
         self.page_size = page_size  # type: int
-        # The start time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # $.parameters[9].schema.example
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # $.parameters[6].schema.enumValueTitles
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeNodeMetricsRequest, self).to_map()
@@ -6454,19 +6268,30 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeNodeMetricsResponseBody(TeaModel):
     def __init__(self, node_metrics=None, request_id=None, total_count=None):
-        # The metrics of the node.
         self.node_metrics = node_metrics  # type: str
-        # The request ID.
+        # You can call this operation to query the detailed metrics information of an OceanBase Database node.
         self.request_id = request_id  # type: str
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
         self.total_count = total_count  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeNodeMetricsResponseBody, self).to_map()
@@ -7789,21 +7614,21 @@
             temp_model = DescribeOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # The read RT baseline of the source data source.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # The read/write RPS baseline of the destination data source.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The read/write RT baseline of the destination data source.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The read RT baseline of the source data source.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOmsOpenAPIProjectStepsRequest, self).to_map()
@@ -7832,21 +7657,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfoErrorDetails(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code.
+        # The suggestions (old).
         self.code = code  # type: str
-        # Valid values: CRITICAL, ERROR, and WARN.
+        # Contact the administrator.
         self.level = level  # type: str
-        # The error message.
+        # A sub-status that indicates whether the checker has completed full verification.
         self.message = message  # type: str
-        # The suggestions.
+        # The amount of data migrated.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfoErrorDetails, self).to_map()
@@ -7875,23 +7700,23 @@
         if m.get('Proposal') is not None:
             self.proposal = m.get('Proposal')
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfo(TeaModel):
     def __init__(self, error_code=None, error_details=None, error_msg=None, error_param=None, failed_time=None):
-        # The error code, such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
+        # The job ID.
         self.error_code = error_code  # type: str
-        # The error details.
+        # Schema migration
         self.error_details = error_details  # type: list[DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfoErrorDetails]
-        # The error message.
+        # The resource deployment ID.
         self.error_msg = error_msg  # type: str
-        # The error related parameters.
+        # The error code (new).
         self.error_param = error_param  # type: dict[str, str]
-        # The time when the error occurred.
+        # The additional information. The value is a JSON string.
         self.failed_time = failed_time  # type: str
 
     def validate(self):
         if self.error_details:
             for k in self.error_details:
                 if k:
                     k.validate()
@@ -7933,21 +7758,21 @@
             self.failed_time = m.get('FailedTime')
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfoConnectorFullProgressOverview(TeaModel):
     def __init__(self, estimated_remaining_time_of_sec=None, estimated_total_count=None, finished_count=None,
                  progress=None):
-        # The estimated maximum time remained, in seconds.
+        # A sub-status that indicates whether this step is skipped.
         self.estimated_remaining_time_of_sec = estimated_remaining_time_of_sec  # type: long
-        # The estimated amount of data to migrate.
+        # The read RPS baseline of the source data source.
         self.estimated_total_count = estimated_total_count  # type: long
-        # The amount of data migrated.
+        # The read/write RT per record of the destination data source, in ms.
         self.finished_count = finished_count  # type: long
-        # finishedCount / estimatedTotalCount
+        # The business data returned.
         self.progress = progress  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfoConnectorFullProgressOverview, self).to_map()
@@ -7979,57 +7804,57 @@
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfo(TeaModel):
     def __init__(self, capacity=None, checkpoint=None, connector_full_progress_overview=None, deploy_id=None,
                  dst_iops=None, dst_rps=None, dst_rps_ref=None, dst_rt=None, dst_rt_ref=None, gmt=None, inconsistencies=None,
                  incr_timestamp_checkpoint=None, job_id=None, processed_records=None, skipped=None, src_iops=None, src_iops_ref=None,
                  src_rps=None, src_rps_ref=None, src_rt=None, src_rt_ref=None, validated=None):
-        # The estimated total number of rows.
+        # The total count, which takes effect in a pagination query.
         self.capacity = capacity  # type: long
-        # The checkpoint. The value is a unix timestamp in seconds.
+        # The operation that you want to perform. Set the value to **DescribeOmsOpenAPIProjectSteps**.
         self.checkpoint = checkpoint  # type: str
-        # The full synchronization progress.
+        # The error code, such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
         self.connector_full_progress_overview = connector_full_progress_overview  # type: DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfoConnectorFullProgressOverview
-        # The resource deployment ID.
+        # The page size, which takes effect in a pagination query.
         self.deploy_id = deploy_id  # type: str
-        # The read/write throughput of the destination data source, in bytes per second.
+        # The error description (old).
         self.dst_iops = dst_iops  # type: long
-        # The read/write RPS of the destination data source.
+        # The estimated amount of data to migrate.
         self.dst_rps = dst_rps  # type: long
-        # The read/write RPS baseline of the destination data source.
+        # The step progress.
         self.dst_rps_ref = dst_rps_ref  # type: long
-        # The read/write RT per record of the destination data source, in ms.
+        # The read requests per second (RPS) of the source data source.
         self.dst_rt = dst_rt  # type: long
-        # The read/write RT baseline of the destination data source.
+        # A system error occurred.
         self.dst_rt_ref = dst_rt_ref  # type: long
-        # The checkpoint collection time. The value is a unix timestamp in seconds.
+        # The full synchronization progress.
         self.gmt = gmt  # type: long
-        # The amount of inconsistent data found during full verification.
+        # The read/write throughput of the destination data source, in bytes per second.
         self.inconsistencies = inconsistencies  # type: long
-        # The checkpoint in incremental synchronization. The value is a unix timestamp in seconds.
+        # The read throughput of the source data source, in bytes per second.
         self.incr_timestamp_checkpoint = incr_timestamp_checkpoint  # type: long
-        # The job ID.
+        # The error code (old).
         self.job_id = job_id  # type: str
-        # The number of migrated rows.
+        # The error related parameters.
         self.processed_records = processed_records  # type: long
-        # A sub-status that indicates whether this step is skipped.
+        # The time spent in processing the request, in seconds.
         self.skipped = skipped  # type: bool
-        # The read throughput of the source data source, in bytes per second.
+        # finishedCount / estimatedTotalCount
         self.src_iops = src_iops  # type: long
-        # The read throughput baseline of the source data source.
+        # The end time, in the format of "2020-05-22T17:04:18".
         self.src_iops_ref = src_iops_ref  # type: long
-        # The read requests per second (RPS) of the source data source.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.src_rps = src_rps  # type: long
-        # The read RPS baseline of the source data source.
+        # The checkpoint. The value is a unix timestamp in seconds.
         self.src_rps_ref = src_rps_ref  # type: long
-        # The read response time (RT) per record of the source data source, in ms.
+        # The error code.
         self.src_rt = src_rt  # type: long
-        # The read RT baseline of the source data source.
+        # The checkpoint collection time. The value is a unix timestamp in seconds.
         self.src_rt_ref = src_rt_ref  # type: long
-        # A sub-status that indicates whether the checker has completed full verification.
+        # The read/write RPS of the destination data source.
         self.validated = validated  # type: bool
 
     def validate(self):
         if self.connector_full_progress_overview:
             self.connector_full_progress_overview.validate()
 
     def to_map(self):
@@ -8134,35 +7959,35 @@
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyData(TeaModel):
     def __init__(self, estimated_remaining_seconds=None, extra_info=None, finish_time=None, interactive=None,
                  start_time=None, step_description=None, step_info=None, step_name=None, step_order=None, step_progress=None,
                  step_status=None):
-        # The estimated time remained.
+        # The request ID.
         self.estimated_remaining_seconds = estimated_remaining_seconds  # type: long
-        # The additional information. The value is a JSON string.
+        # A system error occurred.
         self.extra_info = extra_info  # type: DescribeOmsOpenAPIProjectStepsResponseBodyDataExtraInfo
-        # The end time, in the format of "2020-05-22T17:04:18".
+        # $.parameters[3].schema.example
         self.finish_time = finish_time  # type: str
-        # Indicates whether the current step must be confirmed by the user, rather than scheduled in the backend.
+        # $.parameters[5].schema.description
         self.interactive = interactive  # type: bool
-        # The start time, in the format of "2020-05-22T17:04:18".
+        # The error details.
         self.start_time = start_time  # type: str
-        # The description of the step, for example, schema migration, full migration, full verification, incremental log pull, incremental synchronization, or incremental verification.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.step_description = step_description  # type: str
-        # The step details. The value is a JSON string.
+        # The error related parameters.
         self.step_info = step_info  # type: DescribeOmsOpenAPIProjectStepsResponseBodyDataStepInfo
-        # The step name. Valid values: struct_migration, full_migration, full_validation, incr_log_pull, incr_sync/incr_validation, PRE_CHECK, PREPARE, STRUCT_MIGRATION, INDEX_MIGRATION, STRUCT_SYNC, FULL_MIGRATION, APP_SWITCH, REVERSE_INCR_SYNC, FULL_VALIDATION, INCR_LOG_PULL, INCR_SYNC, INCR_VALIDATION, SYNC_PREPARE, SYNC_INCR_LOG_PULL, CONNECTOR_FULL_SYNC, or CONNECTOR_INCR_SYNC.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.step_name = step_name  # type: str
-        # The sequence of steps.
+        # DescribeOmsOpenAPIProjectSteps
         self.step_order = step_order  # type: int
-        # The step progress.
+        # cn-hangzhou
         self.step_progress = step_progress  # type: int
-        # The step status. Valid values: INIT, RUNNING, FAILED, FINISHED, SUSPEND, and MONITORING. The value MONITORING indicates the continuous monitoring of incremental synchronization and incremental verification.
+        # Indicates whether the call is successful.
         self.step_status = step_status  # type: str
 
     def validate(self):
         if self.extra_info:
             self.extra_info.validate()
         if self.step_info:
             self.step_info.validate()
@@ -8224,21 +8049,21 @@
         if m.get('StepStatus') is not None:
             self.step_status = m.get('StepStatus')
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The error details.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # Valid values: CRITICAL, ERROR, and WARN.
         self.level = level  # type: str
-        # The error description (new).
+        # A system error occurred.
         self.message = message  # type: str
-        # The suggestions (new).
+        # Contact the administrator.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOmsOpenAPIProjectStepsResponseBodyErrorDetail, self).to_map()
@@ -8268,35 +8093,35 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class DescribeOmsOpenAPIProjectStepsResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # The error related parameters.
         self.advice = advice  # type: str
-        # The error code (old).
+        # The error code (old), such as AUTHENTICATION_ERROR, PARAM_ERROR, PARAM_ERROR_MESSAGE, NOT_IMPLEMENTED_ERROR, SHARD_COLUMNS_CONFLICT_MESSAGE, FAILED_PARSE_TOKEN_MESSAGE, CONNECT_CHECK_ERROR, NOT_SUPPORT_ERROR, CE_NOT_SUPPORT_ERROR, NOT_FOUND_ERROR, SHARDING_COLUMN_NOT_INCLUDED_ERROR, INNER_ERROR, DB_QUERY_ERROR, DATAHUB_QUERY_ERROR, USER_LACK_SYS_PRIV_ERROR, USER_LACK_TABLE_PRIV_ERROR, RM_API_ERROR, RM_TASK_ERROR, CM_API_ERROR, CM_API_NOT_SUCCESS, BAGUALU_API_ERROR, IDB_API_ERROR, SUPERVISOR_API_ERROR, OCP_API_ERROR, OCP_SERVICE_ERROR, OCP_QUERY_VERSION_FAILED, OCP_VERSION_INCORRECT_ERROR, OCP_VERSION_NOT_SUPPORTED_ERROR, OCP_API_USER_PASSWORD_INCORRECT_ERROR, OBSCHEMA_ERROR, EXECUTOR_THREAD_POOL_BUSY, NO_TABLE_SELECTED, NO_VIEW_SELECTED, SOURCE_CRAWLER_START_FAILED, SOURCE_CRAWLER_START_FAILED_DATA_EXPIRED, SOURCE_CRAWLER_START_TIMEOUT, DEST_WRITER_START_FAILED, WRITER_UNKNOWN_STATUS, DRC_TOPIC_EXISTS_ERROR, TOPIC_EMPTY_ERROR, REACH_WRITER_LIMIT_ERROR, FOUND_NO_FEASIBLE_STORE_ERROR, TOO_MANY_STORES_FOR_SUBTOPIC, TIMEOUT_EXCEPTION, KIPP_API_ERROR, KIPP_API_RESOURCE_NOT_FOUND, KIPP_API_INVALID_PARAM, KIPP_API_UNKNOWN_ERROR, KIPP_API_INTERNAL_ERROR, KIPP_API_SERVICE_UNAVAILABLE, OMS_AGENT_API_ERROR, KMS_API_ERROR, OMS_ENCRYPT_API_ERROR, OMS_DECRYPT_API_ERROR, ALIYUN_SDK_ERROR, YAOCHI_API_ERROR, RESOURCE_WITHOUT_STOCK_ERROR, RESOURCE_NO_AVAILABLE_ZONE, CM_SDK_ERROR, MIGRATION_PROJECT_STEP_PRECHECK_FAILED, PRE_CHECK_ERROR, FAILURES_CORRECT_ERROR, EXECUTE_DDL_FAILURE, EXECUTE_DDL_UNSUPPORTED_OR_FAILURE, STRUCT_RECORD_DDL_NOT_FOUND, STRUCT_RECORD_INDEX_NOT_FOUND, STRUCT_RECORD_NOT_FOUND, STRUCT_RECORD_NOT_FOUND_IN_DBCAT, SCHEMA_OBJECT_TYPE_NOT_SUPPORT_ERROR, POLAR_MYSQL_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_NETWORK_TYPE_NOT_SUPPORT_ERROR, RDS_VPC_NETWORK_NOT_SUPPORT_ERROR, DB_TYPE_NOT_SUPPORT_ERROR, SYNC_TYPE_NOT_SUPPORT_ERROR, SLAVE_OPERATION_STEP_NOT_SUPPORT_ERROR, BYTE_USED_TYPE_NOT_SUPPORT_ERROR, MANY_TO_ONE_SCHEMA_TABLE_REVERSE_INCR_NOT_SUPPORT_ERROR, DUPLICATE_SCHEMA_TABLE_ERROR, OMS_STEP_NOT_SUPPORT_ERROR, ORACLE_DATABASE_ROLE_NOT_SUPPORT_ERROR, OLD_PRE_CHECK_NOT_SUPPORT_ERROR, SCHEMA_ONE_TO_MANY_NOT_SUPPORT_ERROR, PROJECT_NOT_FOUND_ERROR, ENDPOINT_NOT_FOUND_ERROR, ENDPOINT_NAME_ALREADY_EXIST_ERROR, ENDPOINT_QUERY_ERROR, ENDPOINT_SQL_QUERY_ERROR, PROJECT_NAME_ALREADY_EXIST_ERROR, CHECKER_NOT_FOUND_ERROR, CHECKER_FAILED_ERROR, CHECKER_STATUS_UNEXPECTED_ERROR, CHECKER_NO_TASK_TYPE_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR, WORKER_INSTANCE_ALLOCATING_ERROR, LOG_SERVICE_TOPIC_NOT_FOUND_ERROR, CLUSTER_NOT_FOUND_ERROR, TENANT_NOT_FOUND_ERROR, DATABASE_NOT_FOUND_ERROR, TABLE_NOT_FOUND_ERROR, COLUMN_NOT_FOUND_ERROR, TABLE_META_NOT_FOUND_ERROR, SYBASE_CHARSET_NOT_FOUND_ERROR, OCP_NOT_FOUND_ERROR, REGION_NOT_FOUND_ERROR, OCP_ALREADY_EXIST_ERROR, ALARM_CHANNEL_NAME_ALREADY_EXIST_ERROR, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_RESPONSE, SEND_MARKDOWN_TEXT_TO_WEBHOOK_FAILED_EXCEPTION_STATUS, LABEL_ALREADY_EXIST_ERROR, LABEL_NOT_EXIST_ERROR, OCP_ALREADY_USED_ERROR, REGION_INFO_INCONSISTENT_ERROR, OCP_NAME_EMPTY_ERROR, MASTER_SLAVE_ENDPOINT_NAME_INCONSISTENT_ERROR, LOG_FILE_NOT_FOUND_ERROR, OPERATION_NOT_ALLOWED_ERROR, PROJECT_OPERATION_NOT_ALLOWED_ERROR, PROJECT_RELEASE_FAILED, STRUCT_MIGRATION_RETRY_NOT_ALLOWED_ERROR, WORKER_INSTANCE_OPERATION_NOT_ALLOWED_ERROR, USER_OPERATION_NOT_ALLOWED_ERROR, OCP_NAME_OR_REGION_NOT_ALLOWED_UPDATE, UPDATE_CONFIG_WITH_NEWLINE_NOT_ALLOWED, EXIST_UNRELEASED_PROJECT_ERROR, EXIST_UNRELEASED_TOPIC_ERROR, LABEL_CREATE_NOT_ALLOWED_ERROR, LABEL_UPDATE_NOT_ALLOWED_ERROR, LABEL_DELETE_NOT_ALLOWED_ERROR, TOPIC_NAME_INVALID_ERROR, INVALID_STATUS_ERROR, INVALID_CSV_HEAD_ERROR, INVALID_CSV_BODY_ERROR, DUPLICATE_SCHEMA_TABLE_SETTING_ERROR, PROJECT_INVALID_STATUS_ERROR, PROJECT_INVALID_CONNECTOR_COUNT_ERROR, WORKER_INSTANCE_INVALID_STATUS_ERROR, LOG_SERVICE_INVALID_STATUS_ERROR, STEP_INVALID_STATUS_ERROR, UPDATE_ALLOW_DEST_TABLE_NOT_EMPTY_NOT_ALLOWED_ERROR, EXIST_INCONSISTENCY_ERROR, OMS_SWITCH_SUBSTEP_FAILED_ERROR, ENDPOINT_ID_INVALID_ERROR, DB_QUERY_VERSION_EMPTY_ERROR, ENDPOINT_NAME_INVALID_ERROR, ENDPOINT_SCHEMA_NOT_ALLOWED_ERROR, ENDPOINT_SCHEMA_CHAR_NOT_ALLOWED_ERROR, NAME_HAS_SPACE_EXCEPTION, CONFIG_CONVERT_VALUE_ERROR, CONFIG_VALUE_EXCEEDS_LIMIT_ERROR, CONFIG_KEY_NOT_FOUND_KEY_ERROR, CONFIG_VALUE_NOT_EMPTY_ERROR, SCHEMA_HAS_CONVERT_INFO, TIME_SERIES_QUERY_SERVICE_ERROR, ETL_VERIFY_ERROR, ETL_SYNTAX_UNSUPPORTED, ETL_FIELD_NOTFOUND, ETL_FAILED_PARSE_SQL, ETL_VAL_TYPE_ERROR, NOT_SUPPORT_GENERATE_COLUMNS, NOT_SUPPORT_UPDATE_ETL, LOCK_FAILED, OMS_USER_EXIST_ERROR, OMS_USER_NOT_FOUND_ERROR, OMS_USER_NAME_LENGTH_CONSTRAINT, OMS_USER_PASSWORD_ERROR, USER_NAME_OR_PASSWORD_ERROR, OMS_USER_PASSWORD_VALIDATION_ERROR, OMS_USER_PASSWORD_DEFAULT_ERROR, OMS_USER_PERMISSION_DENIED_ERROR, OMS_USER_EDIT_ADMIN_ROLE_INFO_PERMISSION_DENIED_ERROR, OMS_USER_ILLEGAL_DELETED_ERROR, CONNECTOR_TASK_NOT_FOUND_ERROR, CONNECTOR_TASK_NUM_LIMIT_ERROR, CONNECTOR_TASK_DELETE_ERROR, METRIC_SERVICE_ERROR, SYNC_PROJECT_TYPE_INVALID_ERROR, SYNC_SHARDING_COLUMNS_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_INVALID_ERROR, SYNC_PROJECT_PRODUCER_GROUP_LIMIT_EXCEEDS_ERROR, SYNC_PROJECT_COMPLEMENT_CONFIG_ERROR, META_SCHEMA_CREATE_FAILED, RESUME_STEP_FAILED, SCHEMA_INCONSISTENCY, SCHEMA_CASCADE_MAPPING_NOT_SUPPORT_ERROR, SCHEMA_NOT_EXISTED, SCHEMA_EXISTED, SCHEMA_NOT_EXIST, BLACK_LIST_MATCH_ALL, BLACK_LIST_CONTAIN_NON_WHITE_SCHEMA, BLACK_WHITE_LIST_PARAM_INVALID_ERROR, OPERATOR_ERROR, OPERATOR_DIMENSION_NOT_SUPPORT, OPERATOR_PULL_LOG_ERROR, OPERATOR_UPDATE_CONFIG_NOT_SUPPORT, KAFKA_CREATE_TOPIC_ERROR, KAFKA_QUERY_TOPIC_ERROR, KAFKA_BUILD_PROPERTIES_ERROR, ROCKETMQ_CREATE_TOPIC_ERROR, ROCKETMQ_QUERY_TOPIC_ERROR, SYNC_OBJECT_EMPTY_ERROR, WRITER_NUMBER_NOT_UNIQUE, WRITER_NOT_ACTIVE, PROJECT_NAME_DUPLICATE_ERROR, EMPTY_FAILED_STRUCT_MIGRATION_TABLES_ERROR, LOGIC_TABLE_NOT_SUPPORT_UPDATE_OBJECT_ERROR, LOGIC_REQUEST_ERROR, LOGIC_DTO_BUILD_ERROR, UNEXPECTED_REMOTE_API_RESULT, OCEANBASE_USER_UNEXPECTED, STORE_CREATE_FAILED_ERROR, STORE_START_FAILED, STORE_NOT_PULL_LOG_ERROR, ALL_HOSTS_STATUS_ERROR, WORKER_ECS_NOT_FOUND_ERROR, WORKER_ECS_NOT_FOUND_FOR_USER_ERROR, WORKER_POD_NOT_FOUND_ERROR, WORKER_POD_NOT_FOUND_FOR_USER_ERROR, WORKER_INSTANCE_NOT_FOUND_ERROR_V2, and WORKER_INSTANCE_NOT_FOUND_FOR_USER_ERROR.
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
+        # The step end time, in the format of "yyyy-MM-ddTHH:mm:ss".
         self.cost = cost  # type: str
-        # The business data returned.
+        # Indicates whether the current step must be confirmed by the user, rather than scheduled in the backend.
         self.data = data  # type: list[DescribeOmsOpenAPIProjectStepsResponseBodyData]
-        # The error details.
+        # The step details. The value is a JSON string.
         self.error_detail = error_detail  # type: DescribeOmsOpenAPIProjectStepsResponseBodyErrorDetail
-        # The error description (old).
+        # A system error occurred.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
+        # The additional information. The value is a JSON string.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # The step start time, in the format of "yyyy-MM-ddTHH:mm:ss".
         self.page_size = page_size  # type: int
-        # The request ID.
+        # The time when the error occurred.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The read throughput baseline of the source data source.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
+        # The estimated remaining time. This parameter takes effect in full synchronization.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -8404,27 +8229,27 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeOutlineBindingRequest(TeaModel):
     def __init__(self, database_name=None, instance_id=None, is_concurrent_limit=None, sqlid=None, table_name=None,
                  tenant_id=None):
-        # The name of the database.
-        self.database_name = database_name  # type: str
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id  # type: str
         # - When the value is set to True, the throttling information in the database is queried based on the SQL ID.   
         # - When the value is set to False, the bound index or execution plan in the database is queried based on the SQL ID.
-        self.is_concurrent_limit = is_concurrent_limit  # type: bool
+        self.database_name = database_name  # type: str
         # SQLID.
+        self.instance_id = instance_id  # type: str
+        # The ID of the tenant.
+        self.is_concurrent_limit = is_concurrent_limit  # type: bool
+        # false
         self.sqlid = sqlid  # type: str
+        # The name of the database.
+        self.table_name = table_name  # type: str
         # The name of the tenant.    
         # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_). It cannot be set to SYS.
-        self.table_name = table_name  # type: str
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOutlineBindingRequest, self).to_map()
@@ -8460,23 +8285,23 @@
             self.table_name = m.get('TableName')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeOutlineBindingResponseBodyOutlineBinding(TeaModel):
-    def __init__(self, bind_index=None, bind_plan=None, max_concurrent=None, outline_id=None):
-        # The bound index.
+    def __init__(self, bind_index=None, bind_plan=None, max_concurrent=None, outline_id=None, table_name=None):
         self.bind_index = bind_index  # type: str
-        # The bound plan.
+        # You can call this operation to query the outline binding information or throttling information of an SQL statement in the database based on an SQLID.
         self.bind_plan = bind_plan  # type: str
-        # The maximum number of concurrent tasks.
         self.max_concurrent = max_concurrent  # type: int
-        # OutlineID.
+        # {"name":"DescribeOutlineBinding","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeOutlineBinding\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"TableName\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"pay_online\"},{\"name\":\"DatabaseName\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"IsConcurrentLimit\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Boolean\",\"title\":\"\",\"description\":\"\",\"example\":\"false\"},{\"name\":\"InstanceId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"ob317v4uif****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"OutlineBinding\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"children\":[{\"name\":\"BindPlan\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"PHY_TABLE_SCAN | bmsql_order_line | 40 ******\"},{\"name\":\"OutlineId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"OutlineID\",\"description\":\"OutlineID。\",\"example\":\"-1\"},{\"name\":\"BindIndex\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"PRIMARY\"},{\"name\":\"MaxConcurrent\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"}],\"title\":\"\",\"description\":\"\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.outline_id = outline_id  # type: long
+        # 表名称
+        self.table_name = table_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeOutlineBindingResponseBodyOutlineBinding, self).to_map()
         if _map is not None:
@@ -8487,34 +8312,46 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, outline_binding=None, request_id=None):
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
         self.outline_binding = outline_binding  # type: DescribeOutlineBindingResponseBodyOutlineBinding
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.outline_binding:
             self.outline_binding.validate()
 
     def to_map(self):
@@ -8576,21 +8413,19 @@
             temp_model = DescribeOutlineBindingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeParametersRequest(TeaModel):
     def __init__(self, dimension=None, dimension_value=None, instance_id=None):
-        # The type of the parameter.    
-        # Valid values: CLUSTER and TENANT.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.dimension = dimension  # type: str
-        # The resource ID of the parameter type.   
-        # You can leave this parameter unspecified when you call this operation to query cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # Alibaba Cloud CLI
         self.dimension_value = dimension_value  # type: str
-        # The ID of the OceanBase cluster.
+        # 498529
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeParametersRequest, self).to_map()
@@ -8615,37 +8450,57 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class DescribeParametersResponseBodyParameters(TeaModel):
     def __init__(self, acceptable_value=None, current_value=None, default_value=None, description=None, name=None,
-                 need_reboot=None, rejected_value=None, value_type=None):
-        # The valid value range of the parameter.  It is an array with two string elements, which represents a range. The first element represents the minimum value and the second element represents the maximum value.
+                 need_reboot=None, readonly=None, rejected_value=None, value_type=None):
+        # DescribeParameters
         self.acceptable_value = acceptable_value  # type: list[str]
-        # The current value of the parameter.
+        # The ID of the OceanBase cluster.
         self.current_value = current_value  # type: str
-        # The default value of the parameter.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeParameters
+        # &InstanceId=ob317v4uif****\
+        # &Dimension=TENANT
+        # &DimensionValue=ob2mr3oae0****\
+        # &Common request parameters
+        # ```
         self.default_value = default_value  # type: str
         # The description of the parameter.
         self.description = description  # type: str
-        # The name of the parameter.
+        # The request ID.
         self.name = name  # type: str
-        # Indicates whether a restart is required for changes to the parameter to take effect. Valid values:   
-        # - true: A restart is required.   
-        # - false: A restart is not required.
+        # The name of the parameter.
         self.need_reboot = need_reboot  # type: bool
+        # 参数是否只读
+        self.readonly = readonly  # type: bool
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
+        self.rejected_value = rejected_value  # type: list[str]
         # The invalid value range of the parameter.    
         # It is an array with two string elements, which represents a range. The first element represents the minimum value and the second element represents the maximum value.
-        self.rejected_value = rejected_value  # type: list[str]
-        # The type of the parameter value.    Valid values:   
-        # - ENUM: an enumeration value.   
-        # - RANGE: a value range.   
-        # - TIME: a time value.   
-        # - CAPACITY: a storage capacity, in KB, MB, or GB.
         self.value_type = value_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeParametersResponseBodyParameters, self).to_map()
@@ -8661,14 +8516,16 @@
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
 
     def from_map(self, m=None):
@@ -8681,26 +8538,30 @@
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
     def __init__(self, parameters=None, request_id=None):
-        # The information of parameters.
+        # Indicates whether a restart is required for changes to the parameter to take effect. Valid values:   
+        # - true: A restart is required.   
+        # - false: A restart is not required.
         self.parameters = parameters  # type: list[DescribeParametersResponseBodyParameters]
-        # The request ID.
+        # The return result of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
@@ -8769,33 +8630,27 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeParametersHistoryRequest(TeaModel):
     def __init__(self, dimension=None, dimension_value=None, end_time=None, instance_id=None, page_number=None,
                  page_size=None, start_time=None):
-        # The type of the parameter.   
-        # Valid values: CLUSTER and TENANT.
+        # The value of the parameter after the modification.
         self.dimension = dimension  # type: str
-        # The resource ID of the parameter type.   
-        # You can leave this parameter unspecified when you call this operation to query the modification history of cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # The list of parameter modification records.
         self.dimension_value = dimension_value  # type: str
-        # The end time for the query of parameter modification history.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.end_time = end_time  # type: str
-        # The ID of the OceanBase cluster.
+        # The name of the parameter.
         self.instance_id = instance_id  # type: str
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # Default value: 10.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.page_size = page_size  # type: int
-        # The start time of the time range for querying the parameter modification history.
+        # You can call this operation to query the modification history of cluster or tenant parameters.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeParametersHistoryRequest, self).to_map()
@@ -8837,31 +8692,36 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeParametersHistoryResponseBodyRespondParameters(TeaModel):
     def __init__(self, create_time=None, dimension_value=None, name=None, new_value=None, old_value=None,
                  status=None, update_time=None):
-        # The time when the parameter modification was initiated.
+        # The request ID.
         self.create_time = create_time  # type: str
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
         self.dimension_value = dimension_value  # type: str
-        # The name of the parameter.
+        # You can call this operation to query the modification history of cluster or tenant parameters.
         self.name = name  # type: str
-        # The value of the parameter after the modification.
         self.new_value = new_value  # type: str
-        # The parameter value before modification.
+        # The start time of the time range for querying the parameter modification history.
         self.old_value = old_value  # type: str
-        # The modification status. Valid values:    
-        # - APPLIED: The modification was successful.   
-        # - SCHEDULING: The modification was to be made.
+        # -\
         self.status = status  # type: str
-        # The time when the parameter modification took effect.
+        # The name of the parameter.
         self.update_time = update_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeParametersHistoryResponseBodyRespondParameters, self).to_map()
@@ -8902,19 +8762,21 @@
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         return self
 
 
 class DescribeParametersHistoryResponseBodyRespond(TeaModel):
     def __init__(self, page_number=None, parameters=None, total_count=None):
-        # The number of returned entries on each page.
+        # The end time for the query of parameter modification history.
         self.page_number = page_number  # type: int
-        # The parameter modification history.
+        # The number of rows to return on each page.   
+        # - Maximum value: 100   
+        # - Default value: 10
         self.parameters = parameters  # type: list[DescribeParametersHistoryResponseBodyRespondParameters]
-        # The number of parameter modification records.
+        # The list of parameter modification records.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.parameters:
             for k in self.parameters:
                 if k:
                     k.validate()
@@ -8947,17 +8809,19 @@
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeParametersHistoryResponseBody(TeaModel):
     def __init__(self, request_id=None, respond=None):
-        # The request ID.
+        # The number of the page to return.    
+        # - Start value: 1   
+        # - Default value: 1
         self.request_id = request_id  # type: str
-        # The list of parameter modification records.
+        # The time when the parameter modification took effect.
         self.respond = respond  # type: list[DescribeParametersHistoryResponseBodyRespond]
 
     def validate(self):
         if self.respond:
             for k in self.respond:
                 if k:
                     k.validate()
@@ -9025,19 +8889,22 @@
             temp_model = DescribeParametersHistoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRecommendIndexRequest(TeaModel):
     def __init__(self, instance_id=None, sqlid=None, tenant_id=None):
-        # The ID of the OceanBase cluster.
+        # The return result of the request.
         self.instance_id = instance_id  # type: str
-        # You can obtain the SQL ID from the return value of the DescribeSlowSQLList or DescribeTopSQLList operation.
+        # The ID of the OceanBase cluster.
         self.sqlid = sqlid  # type: str
-        # The ID of the tenant.
+        # The index recommended for the SQL statement after calculation by the diagnostic system.   
+        # - If the recommended index is the primary key, PRIMARY is returned.  
+        # - If an index created by the user is recommended, the index name is returned.   
+        # The system recommends only one index for an SQL statement. You can call the DescribeIndexes operation to view the indexes of a table.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRecommendIndexRequest, self).to_map()
@@ -9062,25 +8929,17 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeRecommendIndexResponseBodyRecommendIndex(TeaModel):
     def __init__(self, suggest_index=None, table_list=None, tenant_mode=None):
-        # The index recommended for the SQL statement after calculation by the diagnostic system.   
-        # - If the recommended index is the primary key, PRIMARY is returned.  
-        # - If an index created by the user is recommended, the index name is returned.   
-        # The system recommends only one index for an SQL statement. You can call the DescribeIndexes operation to view the indexes of a table.
+        # Example 1
         self.suggest_index = suggest_index  # type: str
-        # The tables.   
-        # The data tables involved in the SQL statement corresponding to the SQL ID are returned. For a single-table query, the data table accessed is returned. For a join query, all data tables accessed by the SQL statement are returned and separated with vertical bars (|), for example, "Table1|Table2".
         self.table_list = table_list  # type: str
-        # The tenant mode.   Valid values:  
-        # Oracle   
-        # MySQL
         self.tenant_mode = tenant_mode  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRecommendIndexResponseBodyRecommendIndex, self).to_map()
@@ -9107,15 +8966,17 @@
         return self
 
 
 class DescribeRecommendIndexResponseBody(TeaModel):
     def __init__(self, recommend_index=None, request_id=None):
         # The information about the recommended index.
         self.recommend_index = recommend_index  # type: DescribeRecommendIndexResponseBodyRecommendIndex
-        # The request ID.
+        # The tenant mode.   Valid values:  
+        # Oracle   
+        # MySQL
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.recommend_index:
             self.recommend_index.validate()
 
     def to_map(self):
@@ -9177,17 +9038,17 @@
             temp_model = DescribeRecommendIndexResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSQLDetailsRequest(TeaModel):
     def __init__(self, sqlid=None, tenant_id=None):
-        # SQLID.
+        # The SQL text.
         self.sqlid = sqlid  # type: str
-        # The ID of the tenant.
+        # SQLID.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLDetailsRequest, self).to_map()
@@ -9208,19 +9069,17 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeSQLDetailsResponseBodySQLDetails(TeaModel):
     def __init__(self, db_name=None, sqltext=None, user_name=None):
-        # The name of the database.
         self.db_name = db_name  # type: str
-        # The SQL text.
+        # {"name":"DescribeSQLDetails","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSQLDetails\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SQLDetails\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.sqltext = sqltext  # type: str
-        # The username.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLDetailsResponseBodySQLDetails, self).to_map()
@@ -9245,17 +9104,23 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeSQLDetailsResponseBody(TeaModel):
     def __init__(self, request_id=None, sqldetails=None):
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeSQLDetails**.
         self.request_id = request_id  # type: str
-        # The details of the SQL statement.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeSQLDetails
+        # &TenantId=t2mr3oae0****\
+        # &SQLId=8D6E84****0B8FB1823D199E2CA1****\
+        # &Common request parameters
+        # ```
         self.sqldetails = sqldetails  # type: list[DescribeSQLDetailsResponseBodySQLDetails]
 
     def validate(self):
         if self.sqldetails:
             for k in self.sqldetails:
                 if k:
                     k.validate()
@@ -9323,28 +9188,25 @@
             temp_model = DescribeSQLDetailsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSQLHistoryListRequest(TeaModel):
     def __init__(self, end_time=None, page_number=None, page_size=None, sqlid=None, start_time=None, tenant_id=None):
-        # The end time of the time range for querying the SQL execution history.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The number of block index cache hits.
         self.end_time = end_time  # type: str
-        # The page number.
+        # The end time in UTC +0.
         self.page_number = page_number  # type: int
-        # The number of entries returned on each page.   
-        # Default value: 10.
+        # The end time.
         self.page_size = page_size  # type: int
-        # SQLID.
+        # The number of block index cache hits.
         self.sqlid = sqlid  # type: str
-        # The start time of the time range for querying the SQL execution history.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # The average CPU time.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLHistoryListRequest, self).to_map()
@@ -9387,89 +9249,88 @@
     def __init__(self, affected_rows=None, app_wait_time=None, block_cache_hit=None, block_index_cache_hit=None,
                  bloom_filter_cache_hit=None, client_ip=None, concurrency_wait_time=None, cpu_time=None, db_name=None, decode_time=None,
                  disk_read=None, elapsed_time=None, end_time=None, end_time_utcstring=None, event=None, exec_per_second=None,
                  execute_time=None, executions=None, fail_times=None, get_plan_time=None, iowait_time=None, logical_read=None,
                  max_cpu_time=None, max_elapsed_time=None, memstore_read_row_count=None, miss_plans=None, net_wait_time=None,
                  node_ip=None, queue_time=None, rpccount=None, remote_plans=None, retry_count=None, return_rows=None,
                  row_cache_hit=None, schedule_time=None, ssstore_read_row_count=None, total_wait_time=None, user_name=None):
-        # The number of rows affected.
-        self.affected_rows = affected_rows  # type: long
         # The wait time of the client.
+        self.affected_rows = affected_rows  # type: long
+        # The IP address of the client.
         self.app_wait_time = app_wait_time  # type: float
-        # The number of block cache hits.
+        # The number of logical reads.
         self.block_cache_hit = block_cache_hit  # type: long
         # The number of block index cache hits.
         self.block_index_cache_hit = block_index_cache_hit  # type: long
-        # The number of Bloom filter cache hits.
+        # The username.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit  # type: long
-        # The IP address of the client.
+        # The number of remote plans.
         self.client_ip = client_ip  # type: str
-        # The wait time in concurrent execution.
+        # The number of block cache hits.
         self.concurrency_wait_time = concurrency_wait_time  # type: float
-        # The average CPU time.
+        # The page number.
         self.cpu_time = cpu_time  # type: float
-        # The name of the database.
+        # The number of retries.
         self.db_name = db_name  # type: str
-        # The time to wait for decoding.
+        # The number of rows read from the disk.
         self.decode_time = decode_time  # type: float
-        # The number of physical reads.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.disk_read = disk_read  # type: long
-        # The average response time.
+        # The number of row cache hits.
         self.elapsed_time = elapsed_time  # type: float
-        # The end time.
+        # The maximum CPU time.
         self.end_time = end_time  # type: long
-        # The end time in UTC +0.
+        # The number of rows read from the memory.
         self.end_time_utcstring = end_time_utcstring  # type: str
-        # The wait event.
+        # The number of rows returned.
         self.event = event  # type: str
-        # The number of executions per second.
+        # The queuing time.
         self.exec_per_second = exec_per_second  # type: long
-        # The internal execution time.
+        # The execution history of the SQL statement.
         self.execute_time = execute_time  # type: float
-        # The number of executions.
+        # The wait time in concurrent execution.
         self.executions = executions  # type: long
-        # The number of failures.
+        # Example 1
         self.fail_times = fail_times  # type: long
-        # The time spent in hard parsing.
+        # The number of RPCs.
         self.get_plan_time = get_plan_time  # type: float
-        # The I/O wait time.
+        # The number of rows affected.
         self.iowait_time = iowait_time  # type: float
-        # The number of logical reads.
         self.logical_read = logical_read  # type: long
-        # The maximum CPU time.
+        # The number of row cache hits.
         self.max_cpu_time = max_cpu_time  # type: float
-        # The maximum response time.
+        # The scheduling duration.
         self.max_elapsed_time = max_elapsed_time  # type: float
-        # The number of rows read from the memory.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeSQLHistoryList**.
         self.memstore_read_row_count = memstore_read_row_count  # type: long
-        # The number of plan misses.
+        # The number of Bloom filter cache hits.
         self.miss_plans = miss_plans  # type: long
-        # The network latency.
+        # The return result of the request.
         self.net_wait_time = net_wait_time  # type: float
-        # The IP address of the node.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.node_ip = node_ip  # type: str
-        # The queuing time.
         self.queue_time = queue_time  # type: float
-        # The number of RPCs.
+        # The quantity.
         self.rpccount = rpccount  # type: long
-        # The number of remote plans.
+        # The list.
         self.remote_plans = remote_plans  # type: long
-        # The number of retries.
+        # The number of executions.
         self.retry_count = retry_count  # type: long
-        # The number of rows returned.
+        # The I/O wait time.
         self.return_rows = return_rows  # type: long
-        # The number of row cache hits.
+        # {"name":"DescribeSQLHistoryList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSQLHistoryList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"SQLID\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SQLHistoryList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"children\":[{\"name\":\"List\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"ExecPerSecond\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"163.0\"},{\"name\":\"MaxCpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"257.967\"},{\"name\":\"BlockCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"14\"},{\"name\":\"DecodeTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"RemotePlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"RPCCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NetWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DiskRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NodeIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"ConcurrencyWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"MemstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"527\"},{\"name\":\"AppWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"ElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"76.382\"},{\"name\":\"MissPlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"AffectedRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ScheduleTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"Event\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"mysql response wait client\"},{\"name\":\"TotalWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"10.966\"},{\"name\":\"ReturnRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecuteTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"61.044\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tester\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"89403\"},{\"name\":\"GetPlanTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.052\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"MaxElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"260.44\"},{\"name\":\"BlockIndexCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"4\"},{\"name\":\"EndTimeUTCString\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-12-28T02:08:18Z\"},{\"name\":\"EndTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-12-28T02:08:18Z\"},{\"name\":\"RetryCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ClientIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"1*2.***.1*3.***\"},{\"name\":\"BloomFilterCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"IOWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"FailTimes\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"QueueTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"title\":\"\",\"description\":\"\",\"example\":\"15.275\"},{\"name\":\"RowCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"LogicalRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"19\"},{\"name\":\"SsstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"43086\"}],\"title\":\"\"},{\"name\":\"Count\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"}],\"title\":\"\",\"description\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{\"2014\":[{\"code\":\"2014\",\"defaultError\":false,\"errorCode\":\"InternalError\",\"errorMessage\":\"The request processing has failed due to some unknown error.\",\"errorMessageCn\":\"\",\"type\":\"user\"}]}"}
         self.row_cache_hit = row_cache_hit  # type: long
-        # The scheduling duration.
+        # The end time of the time range for querying the SQL execution history.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.schedule_time = schedule_time  # type: float
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count  # type: long
-        # The internal wait time.
+        # The average response time.
         self.total_wait_time = total_wait_time  # type: float
-        # The username.
+        # The network latency.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLHistoryListResponseBodySQLHistoryListList, self).to_map()
@@ -9634,16 +9495,16 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeSQLHistoryListResponseBodySQLHistoryList(TeaModel):
     def __init__(self, count=None, list=None):
-        # The quantity.
         self.count = count  # type: long
+        # The I/O wait time.
         self.list = list  # type: list[DescribeSQLHistoryListResponseBodySQLHistoryListList]
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
@@ -9672,17 +9533,17 @@
                 temp_model = DescribeSQLHistoryListResponseBodySQLHistoryListList()
                 self.list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeSQLHistoryListResponseBody(TeaModel):
     def __init__(self, request_id=None, sqlhistory_list=None):
-        # The request ID.
+        # The IP address of the client.
         self.request_id = request_id  # type: str
-        # The execution history of the SQL statement.
+        # The number of Bloom filter cache hits.
         self.sqlhistory_list = sqlhistory_list  # type: DescribeSQLHistoryListResponseBodySQLHistoryList
 
     def validate(self):
         if self.sqlhistory_list:
             self.sqlhistory_list.validate()
 
     def to_map(self):
@@ -9744,17 +9605,17 @@
             temp_model = DescribeSQLHistoryListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSQLPlansRequest(TeaModel):
     def __init__(self, sqlid=None, tenant_id=None):
-        # SQLID.
+        # The time when the plan was loaded for the first time, .
         self.sqlid = sqlid  # type: str
-        # The ID of the tenant.
+        # The time when the plan was loaded for the first time, .
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLPlansRequest, self).to_map()
@@ -9778,45 +9639,43 @@
 
 
 class DescribeSQLPlansResponseBodySQLPlans(TeaModel):
     def __init__(self, avg_execution_ms=None, avg_execution_time_ms=None, first_load_time=None,
                  first_load_time_utcstring=None, hit_count=None, merged_version=None, node_ip=None, outline_data=None, outline_id=None,
                  outline_time=None, outline_time_utcstring=None, plan_full=None, plan_id=None, plan_info=None,
                  plan_union_hash=None, query_sql=None):
-        # The average execution duration, in ms.
+        # The time when the plan was bound.
         self.avg_execution_ms = avg_execution_ms  # type: float
-        # The average execution duration when the database uses this execution plan, in ms.
+        # The time when the plan was loaded for the first time, in UTC +0.
         self.avg_execution_time_ms = avg_execution_time_ms  # type: long
-        # The time when the plan was loaded for the first time, .
         self.first_load_time = first_load_time  # type: long
-        # The time when the plan was loaded for the first time, in UTC +0.
+        # Example 1
         self.first_load_time_utcstring = first_load_time_utcstring  # type: str
-        # The number of hits.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.hit_count = hit_count  # type: int
-        # The major compaction version.
+        # The unique identifier of the SQL execution plan in the diagnostic system.
         self.merged_version = merged_version  # type: int
-        # The IP address of the node.
+        # The complete execution plan of the SQL statement.
         self.node_ip = node_ip  # type: str
-        # The outline data.
+        # The information about the plan.
         self.outline_data = outline_data  # type: str
-        # OutlineID.
+        # SQLID.
         self.outline_id = outline_id  # type: long
-        # The time when the plan was bound.
+        # The ID of the SQL execution plan in the database.
         self.outline_time = outline_time  # type: long
-        # The time when the plan was bound, in UTC +0.
+        # The major compaction version.
         self.outline_time_utcstring = outline_time_utcstring  # type: str
-        # The complete execution plan of the SQL statement.
+        # The information about the execution plan.
         self.plan_full = plan_full  # type: str
-        # The ID of the SQL execution plan in the database.
+        # OutlineID.
         self.plan_id = plan_id  # type: int
-        # The information about the plan.
         self.plan_info = plan_info  # type: str
-        # The unique identifier of the SQL execution plan in the diagnostic system.
+        # The return result of the request.
         self.plan_union_hash = plan_union_hash  # type: str
-        # The query SQL statement.
+        # The request ID.
         self.query_sql = query_sql  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSQLPlansResponseBodySQLPlans, self).to_map()
@@ -9893,17 +9752,17 @@
         if m.get('QuerySQL') is not None:
             self.query_sql = m.get('QuerySQL')
         return self
 
 
 class DescribeSQLPlansResponseBody(TeaModel):
     def __init__(self, request_id=None, sqlplans=None):
-        # The request ID.
+        # The return result of the request.
         self.request_id = request_id  # type: str
-        # The information about the execution plan.
+        # master
         self.sqlplans = sqlplans  # type: list[DescribeSQLPlansResponseBodySQLPlans]
 
     def validate(self):
         if self.sqlplans:
             for k in self.sqlplans:
                 if k:
                     k.validate()
@@ -9996,18 +9855,15 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class DescribeSecurityIpGroupsResponseBodySecurityIpGroups(TeaModel):
     def __init__(self, security_ip_group_name=None, security_ips=None):
-        # The name of the security group.
         self.security_ip_group_name = security_ip_group_name  # type: str
-        # The list of IP addresses and CIDR blocks in the whitelist.   
-        # It is a JSON array. Each object in the array is an IP address or CIDR block.
         self.security_ips = security_ips  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSecurityIpGroupsResponseBodySecurityIpGroups, self).to_map()
@@ -10030,17 +9886,16 @@
         return self
 
 
 class DescribeSecurityIpGroupsResponseBody(TeaModel):
     def __init__(self, request_id=None, security_ip_groups=None, total_count=None):
         # The request ID.
         self.request_id = request_id  # type: str
-        # The information of the IP address whitelist group.
         self.security_ip_groups = security_ip_groups  # type: list[DescribeSecurityIpGroupsResponseBodySecurityIpGroups]
-        # The number of whitelist groups returned.
+        # Example 1
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.security_ip_groups:
             for k in self.security_ip_groups:
                 if k:
                     k.validate()
@@ -10112,29 +9967,23 @@
             temp_model = DescribeSecurityIpGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSlowSQLHistoryListRequest(TeaModel):
     def __init__(self, end_time=None, page_number=None, page_size=None, sqlid=None, start_time=None, tenant_id=None):
-        # The end time of the time range for querying the execution history of the slow SQL statement.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The number of RPCs.
         self.end_time = end_time  # type: str
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The maximum response time.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.  
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of plan misses.
         self.page_size = page_size  # type: int
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The wait time for network.
         self.sqlid = sqlid  # type: str
-        # The start time of the time range for querying the execution history of the slow SQL statement.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The I/O wait time.
         self.start_time = start_time  # type: str
         # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
@@ -10180,93 +10029,104 @@
                  bloom_filter_cache_hit=None, client_ip=None, concurrency_wait_time=None, cpu_time=None, db_name=None, decode_time=None,
                  disk_read=None, elapsed_time=None, end_time_utcstring=None, event=None, exec_per_second=None,
                  execute_time=None, executions=None, fail_times=None, get_plan_time=None, iowait_time=None, logical_read=None,
                  max_cpu_time=None, max_elapsed_time=None, memstore_read_row_count=None, miss_plans=None, net_wait_time=None,
                  node_ip=None, queue_time=None, rpccount=None, remote_plans=None, retry_count=None, return_rows=None,
                  row_cache_hit=None, schedule_time=None, sql_id=None, sql_type=None, ssstore_read_row_count=None,
                  tenant_name=None, total_wait_time=None, user_name=None):
-        # The number of rows affected.
+        # The wait event.
         self.affected_rows = affected_rows  # type: float
-        # The wait time of the client.
+        # The number of row cache hits.
         self.app_wait_time = app_wait_time  # type: float
-        # The number of block cache hits.
+        # The average CPU time.
         self.block_cache_hit = block_cache_hit  # type: float
-        # The number of block index cache hits.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100   
+        # - Default value: 10
         self.block_index_cache_hit = block_index_cache_hit  # type: float
-        # The number of Bloom filter cache hits.
+        # The number of executions.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit  # type: float
-        # The IP address of the client.
+        # The number of retries.
         self.client_ip = client_ip  # type: str
-        # The wait time in concurrent execution.
+        # $.parameters[6].schema.example
         self.concurrency_wait_time = concurrency_wait_time  # type: float
-        # The average CPU time.
+        # $.parameters[6].schema.enumValueTitles
         self.cpu_time = cpu_time  # type: float
-        # The name of the database.
+        # The IP address of the node.
         self.db_name = db_name  # type: str
-        # The time to wait for decoding.
+        # $.parameters[7].schema.description
         self.decode_time = decode_time  # type: float
-        # The number of physical reads.
+        # SQLID.
         self.disk_read = disk_read  # type: float
-        # The average response time.
+        # The queuing time.
         self.elapsed_time = elapsed_time  # type: float
-        # The end time.
         self.end_time_utcstring = end_time_utcstring  # type: str
-        # The wait event.
+        # The internal wait time.
         self.event = event  # type: str
-        # The number of executions per second.
+        # The number of failures.
         self.exec_per_second = exec_per_second  # type: float
-        # The internal execution time.
+        # The request ID.
         self.execute_time = execute_time  # type: float
-        # The number of executions.
+        # The maximum CPU time.
         self.executions = executions  # type: float
-        # The number of failures.
+        # The number of rows returned.
         self.fail_times = fail_times  # type: float
-        # Hard parsing time.
+        # Example 1
         self.get_plan_time = get_plan_time  # type: float
-        # The I/O wait time.
+        # $.parameters[7].schema.enumValueTitles
         self.iowait_time = iowait_time  # type: float
-        # The number of logical reads.
+        # The quantity.
         self.logical_read = logical_read  # type: float
-        # The maximum CPU time.
+        # DescribeSlowSQLHistoryList
         self.max_cpu_time = max_cpu_time  # type: float
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
         self.max_elapsed_time = max_elapsed_time  # type: float
-        # The number of rows read from the memory.
+        # The wait time of the client.
         self.memstore_read_row_count = memstore_read_row_count  # type: float
-        # The number of plan misses.
+        # The number of rows read from the disk.
         self.miss_plans = miss_plans  # type: float
-        # The wait time for network.
+        # $.parameters[7].schema.example
         self.net_wait_time = net_wait_time  # type: float
-        # The IP address of the node.
+        # The number of the page to return.    
+        # - Start value: 1   
+        # - Default value: 1
         self.node_ip = node_ip  # type: str
-        # The queuing time.
+        # $.parameters[6].schema.description
         self.queue_time = queue_time  # type: float
-        # The number of RPCs.
+        # The end time.
         self.rpccount = rpccount  # type: float
-        # The number of remote plans.
+        # The time to wait for decoding.
         self.remote_plans = remote_plans  # type: float
-        # The number of retries.
+        # The number of block index cache hits.
         self.retry_count = retry_count  # type: float
-        # The number of rows returned.
+        # The number of executions per second.
         self.return_rows = return_rows  # type: float
-        # The number of row cache hits.
+        # The execution history of the slow SQL statement.
         self.row_cache_hit = row_cache_hit  # type: float
-        # The scheduling duration.
+        # You can call this operation to query the execution history of an SQL statement by SQL ID that is determined as a slow SQL statement during a specified period of time.
         self.schedule_time = schedule_time  # type: float
-        # SQLID.
+        # The return result of the request.
         self.sql_id = sql_id  # type: str
-        # The SQL type.
+        # The IP address of the client.
         self.sql_type = sql_type  # type: str
-        # The number of rows read from the disk.
+        # The scheduling duration.
         self.ssstore_read_row_count = ssstore_read_row_count  # type: float
-        # The name of the tenant.
+        # The return result of the request.
         self.tenant_name = tenant_name  # type: str
-        # The internal wait time.
         self.total_wait_time = total_wait_time  # type: float
-        # The username.
+        # The number of physical reads.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryListList, self).to_map()
@@ -10439,17 +10299,16 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryList(TeaModel):
     def __init__(self, count=None, list=None):
-        # The quantity.
         self.count = count  # type: long
-        # The return result of the request.
+        # The SQL ID, which uniquely identifies an SQL statement.
         self.list = list  # type: list[DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryListList]
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
@@ -10478,17 +10337,18 @@
                 temp_model = DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryListList()
                 self.list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeSlowSQLHistoryListResponseBody(TeaModel):
     def __init__(self, request_id=None, slow_sqlhistory_list=None):
-        # The request ID.
+        # The end time of the time range for querying the execution history of the slow SQL statement.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.request_id = request_id  # type: str
-        # The execution history of the slow SQL statement.
+        # Hard parsing time。
         self.slow_sqlhistory_list = slow_sqlhistory_list  # type: DescribeSlowSQLHistoryListResponseBodySlowSQLHistoryList
 
     def validate(self):
         if self.slow_sqlhistory_list:
             self.slow_sqlhistory_list.validate()
 
     def to_map(self):
@@ -10552,49 +10412,46 @@
         return self
 
 
 class DescribeSlowSQLListRequest(TeaModel):
     def __init__(self, db_name=None, end_time=None, filter_condition=None, node_ip=None, page_number=None,
                  page_size=None, sqlid=None, search_key_word=None, search_parameter=None, search_rule=None, search_value=None,
                  sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The name of the database.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time  # type: str
         # The filter condition.
         self.filter_condition = filter_condition  # type: dict[str, any]
-        # The IP address of the database node.
+        # The number of plan misses.
         self.node_ip = node_ip  # type: str
-        # The number of rows to return on each page.  
-        # - Maximum value: 100  
-        # - Default value: 10
-        self.page_number = page_number  # type: int
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
+        self.page_number = page_number  # type: int
+        # The return result of the request.
         self.page_size = page_size  # type: int
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The internal wait time.
         self.sqlid = sqlid  # type: str
-        # The search keyword.
+        # Alibaba Cloud CLI
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # The IP address of the database node.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.
+        # The queuing time.
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # The list of slow SQL statements.
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100  
+        # - Default value: 10
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The average CPU time.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The list of slow SQL statements.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # The number of logical reads.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSlowSQLListRequest, self).to_map()
@@ -10669,49 +10526,46 @@
         return self
 
 
 class DescribeSlowSQLListShrinkRequest(TeaModel):
     def __init__(self, db_name=None, end_time=None, filter_condition_shrink=None, node_ip=None, page_number=None,
                  page_size=None, sqlid=None, search_key_word=None, search_parameter=None, search_rule=None, search_value=None,
                  sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The name of the database.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time  # type: str
         # The filter condition.
         self.filter_condition_shrink = filter_condition_shrink  # type: str
-        # The IP address of the database node.
+        # The number of plan misses.
         self.node_ip = node_ip  # type: str
-        # The number of rows to return on each page.  
-        # - Maximum value: 100  
-        # - Default value: 10
-        self.page_number = page_number  # type: int
         # The number of the page to return.    
         # - Start value: 1   
         # - Default value: 1
+        self.page_number = page_number  # type: int
+        # The return result of the request.
         self.page_size = page_size  # type: int
-        # The SQL ID, which uniquely identifies an SQL statement.
+        # The internal wait time.
         self.sqlid = sqlid  # type: str
-        # The search keyword.
+        # Alibaba Cloud CLI
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # The IP address of the database node.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.
+        # The queuing time.
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # The list of slow SQL statements.
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The number of rows to return on each page.  
+        # - Maximum value: 100  
+        # - Default value: 10
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The average CPU time.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying slow SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The list of slow SQL statements.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # The number of logical reads.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSlowSQLListShrinkRequest, self).to_map()
@@ -10791,93 +10645,105 @@
                  bloom_filter_cache_hit=None, client_ip=None, concurrency_wait_time=None, cpu_time=None, db_name=None, decode_time=None,
                  disk_read=None, elapsed_time=None, event=None, exec_per_second=None, execute_time=None, executions=None,
                  fail_times=None, get_plan_time=None, iowait_time=None, key=None, logical_read=None, max_cpu_time=None,
                  max_elapsed_time=None, memstore_read_row_count=None, miss_plans=None, net_wait_time=None, node_ip=None,
                  queue_time=None, rpccount=None, remote_plans=None, retry_count=None, return_rows=None, row_cache_hit=None,
                  sqlid=None, sqltext=None, sqltype=None, schedule_time=None, ssstore_read_row_count=None,
                  total_wait_time=None, user_name=None):
-        # The number of rows affected.
+        # The username.
         self.affected_rows = affected_rows  # type: long
-        # The wait time of the client.
+        # The average response time.
         self.app_wait_time = app_wait_time  # type: float
-        # The number of block cache hits.
+        # The wait time in concurrent execution.
         self.block_cache_hit = block_cache_hit  # type: long
-        # The number of block index cache hits.
+        # The request ID.
         self.block_index_cache_hit = block_index_cache_hit  # type: long
-        # The number of Bloom filter cache hits.
         self.bloom_filter_cache_hit = bloom_filter_cache_hit  # type: long
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
         self.client_ip = client_ip  # type: str
-        # The wait time in concurrent execution.
+        # The sorted column.
         self.concurrency_wait_time = concurrency_wait_time  # type: float
-        # The average CPU time.
+        # The wait event.
         self.cpu_time = cpu_time  # type: float
-        # The name of the database.
+        # The search value.
         self.db_name = db_name  # type: str
-        # The time to wait for decoding.
+        # The time spent in hard parsing.
         self.decode_time = decode_time  # type: float
-        # The number of physical reads.
+        # The IP address of the client.
         self.disk_read = disk_read  # type: long
-        # The average response time.
+        # The search rule.
         self.elapsed_time = elapsed_time  # type: float
-        # The wait event.
+        # The number of row cache hits.
         self.event = event  # type: str
-        # The number of executions per second.
+        # The total count.
         self.exec_per_second = exec_per_second  # type: float
-        # The internal execution time.
+        # The number of block cache hits.
         self.execute_time = execute_time  # type: float
-        # The number of executions.
+        # The IP address of the node.
         self.executions = executions  # type: long
-        # The number of failures.
+        # {"name":"DescribeSlowSQLList","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"GET|POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeSlowSQLList\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"t2mr3oae0****\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-09-13T15:40:43Z\"},{\"name\":\"DbName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"SearchKeyWord\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"update\"},{\"name\":\"SearchParameter\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SearchRule\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\">\"},{\"name\":\"SearchValue\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"0.01\"},{\"name\":\"SQLId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"NodeIp\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"FilterCondition\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"[dbName:sys]\"},{\"name\":\"SortColumn\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"cputime\"},{\"name\":\"SortOrder\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"desc\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"\",\"description\":\"\",\"example\":\"2\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"473469C7-AA6F-4DC5-B3DB-A3DC0DE3C83E\"},{\"name\":\"SlowSQLList\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"description\":\"  \",\"children\":[{\"name\":\"Key\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecPerSecond\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"163.0\"},{\"name\":\"SQLText\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"SELECT  ****   FROM ****   WHERE **** = ? AND **** = ?   ORDER BY **** ASC\"},{\"name\":\"MaxCpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"257.967\"},{\"name\":\"BlockCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"14\"},{\"name\":\"DecodeTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"RemotePlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"RPCCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NetWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"DiskRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"NodeIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"i-bp18qljorblo8es*****\"},{\"name\":\"ConcurrencyWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"MemstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"527\"},{\"name\":\"DbName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"testdb\"},{\"name\":\"AppWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"ElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"76.382\"},{\"name\":\"MissPlans\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"AffectedRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"ScheduleTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"Event\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"mysql response wait client\"},{\"name\":\"TotalWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"10.966\"},{\"name\":\"ReturnRows\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"ExecuteTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"61.044\"},{\"name\":\"UserName\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"tester\"},{\"name\":\"Executions\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"89403\"},{\"name\":\"GetPlanTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.052\"},{\"name\":\"CpuTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"50.13\"},{\"name\":\"MaxElapsedTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"260.044\"},{\"name\":\"SQLType\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"BlockIndexCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"4\"},{\"name\":\"RetryCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"SQLId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"SQLID。\",\"example\":\"8D6E84****0B8FB1823D199E2CA1****\"},{\"name\":\"ClientIp\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"1*2.***.1*3.***\"},{\"name\":\"BloomFilterCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"IOWaitTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"0.0\"},{\"name\":\"FailTimes\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"QueueTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Float\",\"description\":\"\",\"example\":\"15.275\"},{\"name\":\"RowCacheHit\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"0\"},{\"name\":\"LogicalRead\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"19\"},{\"name\":\"SsstoreReadRowCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Long\",\"description\":\"\",\"example\":\"43086\"}],\"title\":\"\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.fail_times = fail_times  # type: long
-        # The time spent in hard parsing.
+        # The number of Bloom filter cache hits.
         self.get_plan_time = get_plan_time  # type: float
-        # The I/O wait time.
+        # You can call this operation to query the list of slow SQL statements
         self.iowait_time = iowait_time  # type: float
-        # The sequence number of the returned SQL statement.
+        # The scheduling duration.
         self.key = key  # type: long
-        # The number of logical reads.
         self.logical_read = logical_read  # type: long
-        # The maximum CPU time.
+        # The name of the database.
         self.max_cpu_time = max_cpu_time  # type: float
-        # The maximum response time.
+        # The sequence number of the returned SQL statement.
         self.max_elapsed_time = max_elapsed_time  # type: float
-        # The number of rows read from the memory.
+        # The number of logical reads.
         self.memstore_read_row_count = memstore_read_row_count  # type: long
-        # The number of plan misses.
+        # The number of RPCs.
         self.miss_plans = miss_plans  # type: long
-        # The network latency.
+        # The search parameter.
         self.net_wait_time = net_wait_time  # type: float
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip  # type: str
-        # The queuing time.
         self.queue_time = queue_time  # type: float
-        # The number of RPCs.
+        # The maximum response time.
         self.rpccount = rpccount  # type: long
-        # The number of remote plans.
+        # The search keyword.
         self.remote_plans = remote_plans  # type: long
-        # The number of retries.
+        # The number of physical reads.
         self.retry_count = retry_count  # type: long
-        # The number of rows returned.
+        # The wait time of the client.
         self.return_rows = return_rows  # type: long
-        # The number of row cache hits.
         self.row_cache_hit = row_cache_hit  # type: long
-        # SQLID.
+        # Example 1
         self.sqlid = sqlid  # type: str
-        # The SQL text.
+        # The network latency.
         self.sqltext = sqltext  # type: str
-        # The SQL type.
+        # SQLID.
         self.sqltype = sqltype  # type: long
-        # The scheduling duration.
+        # The internal execution time.
         self.schedule_time = schedule_time  # type: float
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count  # type: long
-        # The internal wait time.
+        # The SQL ID, which uniquely identifies an SQL statement.
         self.total_wait_time = total_wait_time  # type: float
-        # The username.
+        # The number of executions.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSlowSQLListResponseBodySlowSQLList, self).to_map()
@@ -11050,19 +10916,19 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeSlowSQLListResponseBody(TeaModel):
     def __init__(self, request_id=None, slow_sqllist=None, total_count=None):
-        # The request ID.
+        # The SQL text.
         self.request_id = request_id  # type: str
-        # The list of slow SQL statements.
+        # The sorting rule.
         self.slow_sqllist = slow_sqllist  # type: list[DescribeSlowSQLListResponseBodySlowSQLList]
-        # The total count.
+        # The name of the database.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.slow_sqllist:
             for k in self.slow_sqllist:
                 if k:
                     k.validate()
@@ -11134,17 +11000,21 @@
             temp_model = DescribeSlowSQLListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_id=None):
-        # The ID of the OceanBase cluster.
+        # The status of the Internet address for accessing the tenant. Valid values:   
+        # - CLOSED: The address is disabled.   
+        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
+        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
+        # - ONLINE: The address is in service.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # Indicates whether to enable transaction splitting.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantRequest, self).to_map()
@@ -11168,49 +11038,47 @@
 
 
 class DescribeTenantResponseBodyTenantTenantConnections(TeaModel):
     def __init__(self, address_type=None, connection_role=None, connection_zones=None, internet_address=None,
                  internet_address_status=None, internet_port=None, intranet_address=None, intranet_address_master_zone_id=None,
                  intranet_address_slave_zone_id=None, intranet_address_status=None, intranet_port=None, transaction_split=None, v_switch_id=None,
                  vpc_id=None):
-        # The type of the address.
+        # The primary zone of the tenant.
         self.address_type = address_type  # type: str
-        # The service mode of the connection address. Valid values:  
-        # - ReadWrite: provides strong-consistency read and write services.   
-        # - ReadOnly: provides the read-only service to ensure ultimate consistency of data.   
-        # - Clog: provides transaction log services.
+        # 是否开启事务拆分
         self.connection_role = connection_role  # type: str
-        # The list of zones corresponding to the tenant connection.
-        self.connection_zones = connection_zones  # type: list[str]
         # The Internet address for accessing the tenant.
+        self.connection_zones = connection_zones  # type: list[str]
+        # The ID of the VPC.
         self.internet_address = internet_address  # type: str
-        # The status of the Internet address for accessing the tenant. Valid values:   
-        # - CLOSED: The address is disabled.   
-        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
-        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
-        # - ONLINE: The address is in service.
+        # 实例系列
         self.internet_address_status = internet_address_status  # type: str
-        # The Internet port for accessing the tenant.
+        # 实例类型
         self.internet_port = internet_port  # type: int
-        # The intranet address for accessing the tenant.
+        # The deployment type of the cluster. Valid values:  
+        # - multiple: multi-IDC deployment   
+        # - single: single-IDC deployment   
+        # - dual: dual-IDC deployment
         self.intranet_address = intranet_address  # type: str
-        # The primary zone corresponding to the address for accessing the tenant.
+        # PayCore business database
         self.intranet_address_master_zone_id = intranet_address_master_zone_id  # type: str
-        # The standby zone corresponding to the address for accessing the tenant.
+        # The total number of CPU cores of the tenant.
         self.intranet_address_slave_zone_id = intranet_address_slave_zone_id  # type: str
-        # The status of the intranet address for accessing the tenant.  
-        # The value ONLINE indicates that the address is in service.
+        # 付费类型
         self.intranet_address_status = intranet_address_status  # type: str
-        # The intranet port for accessing the tenant.
+        # The ID of the tenant.
         self.intranet_port = intranet_port  # type: int
-        # Indicates whether to enable transaction splitting.
+        # The primary zone corresponding to the address for accessing the tenant.
         self.transaction_split = transaction_split  # type: bool
-        # The ID of the vSwitch.
+        # The connection access information of the tenant.
         self.v_switch_id = v_switch_id  # type: str
-        # The ID of the VPC.
+        # The service mode of the connection address. Valid values:  
+        # ReadWrite: provides strong-consistency read and write services.   
+        # ReadOnly: provides the read-only service to ensure ultimate consistency of data.   
+        # Clog: provides transaction log services.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantResponseBodyTenantTenantConnections, self).to_map()
@@ -11279,19 +11147,27 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeTenantResponseBodyTenantTenantResourceCpu(TeaModel):
     def __init__(self, total_cpu=None, unit_cpu=None, used_cpu=None):
-        # The total number of CPU cores of the tenant.
+        # The data replica distribution mode of the tenant.    
+        # 
+        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
+        # - For the basic version, N indicates the single-zone mode. 
+        # 
+        # > <br>N represents the number of nodes in a single zone.
         self.total_cpu = total_cpu  # type: float
-        # The number of CPU cores in each resource unit of the tenant.
+        # The zone corresponding to the tenant connection.
         self.unit_cpu = unit_cpu  # type: float
-        # The number of used CPU cores of the tenant.
+        # The tenant mode.   
+        # Valid values: 
+        # Oracle   
+        # MySQL
         self.used_cpu = used_cpu  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantResponseBodyTenantTenantResourceCpu, self).to_map()
@@ -11316,15 +11192,15 @@
         if m.get('UsedCpu') is not None:
             self.used_cpu = m.get('UsedCpu')
         return self
 
 
 class DescribeTenantResponseBodyTenantTenantResourceDiskSize(TeaModel):
     def __init__(self, used_disk_size=None):
-        # The size of used disk space of the tenant, in GB.
+        # The total memory size of the tenant, in GB.
         self.used_disk_size = used_disk_size  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantResponseBodyTenantTenantResourceDiskSize, self).to_map()
@@ -11341,19 +11217,23 @@
         if m.get('UsedDiskSize') is not None:
             self.used_disk_size = m.get('UsedDiskSize')
         return self
 
 
 class DescribeTenantResponseBodyTenantTenantResourceMemory(TeaModel):
     def __init__(self, total_memory=None, unit_memory=None, used_memory=None):
-        # The total memory size of the tenant, in GB.
+        # The information about the memory resources of the tenant.
         self.total_memory = total_memory  # type: float
-        # The memory size of each resource unit of the tenant, in GB.
+        # The time when the tenant was created.
         self.unit_memory = unit_memory  # type: float
-        # The size of used memory of the tenant, in GB.
+        # The status of the Internet address for accessing the tenant. Valid values:   
+        # Closed: The address is disabled.   
+        # - ALLOCATING_INTERNET_ADDRESS: An address is being applied for.   
+        # - PENDING_OFFLINE_INTERNET_ADDRESS: The address is being disabled.   
+        # - ONLINE: The address is in service.
         self.used_memory = used_memory  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantResponseBodyTenantTenantResourceMemory, self).to_map()
@@ -11378,21 +11258,24 @@
         if m.get('UsedMemory') is not None:
             self.used_memory = m.get('UsedMemory')
         return self
 
 
 class DescribeTenantResponseBodyTenantTenantResource(TeaModel):
     def __init__(self, cpu=None, disk_size=None, memory=None, unit_num=None):
-        # The information about the CPU resources of the tenant.
+        # The enabling status of the Clog service.  
+        # CLOSED: The Clog service is disabled.  
+        # - ONLINE: The Clog service is running.
         self.cpu = cpu  # type: DescribeTenantResponseBodyTenantTenantResourceCpu
-        # The information about the disk resources of the tenant.
+        # The status of the intranet address for accessing the tenant.  
+        # The value ONLINE indicates that the address is in service.
         self.disk_size = disk_size  # type: DescribeTenantResponseBodyTenantTenantResourceDiskSize
-        # The information about the memory resources of the tenant.
+        # The description of the tenant.
         self.memory = memory  # type: DescribeTenantResponseBodyTenantTenantResourceMemory
-        # The number of resource units in the tenant.
+        # Alibaba Cloud CLI
         self.unit_num = unit_num  # type: int
 
     def validate(self):
         if self.cpu:
             self.cpu.validate()
         if self.disk_size:
             self.disk_size.validate()
@@ -11429,19 +11312,19 @@
         if m.get('UnitNum') is not None:
             self.unit_num = m.get('UnitNum')
         return self
 
 
 class DescribeTenantResponseBodyTenantTenantZones(TeaModel):
     def __init__(self, region=None, tenant_zone_id=None, tenant_zone_role=None):
-        # The region where the zone of the tenant resides.
+        # 是否允许开启读写分离地址
         self.region = region  # type: str
-        # The ID of the zone.
+        # The intranet port for accessing the tenant.
         self.tenant_zone_id = tenant_zone_id  # type: str
-        # The role of the zone of the tenant.
+        # The character set.
         self.tenant_zone_role = tenant_zone_role  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantResponseBodyTenantTenantZones, self).to_map()
@@ -11467,92 +11350,191 @@
             self.tenant_zone_role = m.get('TenantZoneRole')
         return self
 
 
 class DescribeTenantResponseBodyTenant(TeaModel):
     def __init__(self, available_zones=None, charset=None, clog_service_status=None, collation=None,
                  create_time=None, deploy_mode=None, deploy_type=None, description=None, disk_type=None,
-                 enable_clog_service=None, enable_internet_address_service=None, enable_read_write_split=None, instance_type=None,
-                 master_intranet_address_zone=None, pay_type=None, primary_zone=None, primary_zone_deploy_type=None, series=None, status=None,
-                 tenant_connections=None, tenant_id=None, tenant_mode=None, tenant_name=None, tenant_resource=None, tenant_zones=None,
-                 vpc_id=None):
-        # The list of zones.
+                 enable_binlog_service=None, enable_clog_service=None, enable_internet_address_service=None,
+                 enable_read_write_split=None, instance_type=None, master_intranet_address_zone=None, pay_type=None, primary_zone=None,
+                 primary_zone_deploy_type=None, series=None, status=None, tenant_connections=None, tenant_id=None, tenant_mode=None,
+                 tenant_name=None, tenant_resource=None, tenant_zones=None, vpc_id=None):
+        # DescribeTenant
         self.available_zones = available_zones  # type: list[str]
-        # The character set.
+        # The number of CPU cores in each resource unit of the tenant.
         self.charset = charset  # type: str
-        # The enabling status of the clog service.  
-        # - CLOSED: The clog service is disabled.  
-        # - ONLINE: The clog service is running.
+        # 地址类型
         self.clog_service_status = clog_service_status  # type: str
-        # The collation.
+        # The request ID.
         self.collation = collation  # type: str
-        # The time when the tenant was created.
+        # You can call this operation to create a single tenant in a specific cluster.
         self.create_time = create_time  # type: str
-        # The data replica distribution mode of the tenant.    
-        # 
-        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
-        # - For the basic version, N indicates the single-zone mode. 
-        # 
-        # > <br>N represents the number of nodes in a single zone.
+        # The list of zones.
         self.deploy_mode = deploy_mode  # type: str
-        # The deployment type of the cluster. Valid values:  
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The series of the instance.
         self.deploy_type = deploy_type  # type: str
-        # The description of the tenant.
+        # Indicates whether to enable read/write splitting endpoint.
         self.description = description  # type: str
-        # The type of the disk.
+        # You can call this operation to query the information of a specific tenant in a specific cluster.
         self.disk_type = disk_type  # type: str
-        # Indicates whether the clog service is available. To enable the clog service, submit a ticket.
+        # 是否可以申请Binlog服务
+        self.enable_binlog_service = enable_binlog_service  # type: bool
+        # The intranet address for accessing the tenant.
         self.enable_clog_service = enable_clog_service  # type: bool
-        # Indicates whether the Internet address can be enabled for the tenant.
+        # The deployment type of the primary zone.
         self.enable_internet_address_service = enable_internet_address_service  # type: bool
-        # Indicates whether to enable read/write splitting endpoint.
         self.enable_read_write_split = enable_read_write_split  # type: bool
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
         self.instance_type = instance_type  # type: str
-        # The zone where the primary node is located.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeTenant
+        # &InstanceId=ob317v4uif****\
+        # &TenantId=ob2mr3oae0****\
+        # &Common request parameters
+        # ```
         self.master_intranet_address_zone = master_intranet_address_zone  # type: str
-        # The type of the payment.
         self.pay_type = pay_type  # type: str
-        # The primary zone of the tenant.
+        # The type of the payment.
         self.primary_zone = primary_zone  # type: str
-        # The deployment type of the primary zone.
+        # Example 1
         self.primary_zone_deploy_type = primary_zone_deploy_type  # type: str
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
         self.series = series  # type: str
+        # The character set.
+        self.status = status  # type: str
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
-        self.status = status  # type: str
-        # The connection information of the tenant.
         self.tenant_connections = tenant_connections  # type: list[DescribeTenantResponseBodyTenantTenantConnections]
-        # The ID of the tenant.
+        # The region where the zone of the tenant resides.
         self.tenant_id = tenant_id  # type: str
-        # The tenant mode.   
-        # Valid values:
-        # - Oracle   
-        # - MySQL
+        # The enabling status of the clog service.  
+        # - CLOSED: The clog service is disabled.  
+        # - ONLINE: The clog service is running.
         self.tenant_mode = tenant_mode  # type: str
-        # The name of the tenant.
+        # The request type of the zone of the tenant.  ReadWrite: The zone supports data reads and writes. ReadOnly: The zone supports only data reads. For a high availability cluster with multiple IDCs, the primary zone provides ReadWrite services, and the standby zone provides ReadOnly services. For a high availability cluster with a single IDC, all zones provide ReadWrite services.
         self.tenant_name = tenant_name  # type: str
-        # The resource information of the tenant.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.tenant_resource = tenant_resource  # type: DescribeTenantResponseBodyTenantTenantResource
-        # The zone information of the tenant.
+        # The standby zone corresponding to the address for accessing the tenant.
         self.tenant_zones = tenant_zones  # type: list[DescribeTenantResponseBodyTenantTenantZones]
-        # The ID of the VPC.    
-        # If no suitable VPC is available, create a VPC as prompted. For more information, see "What is a VPC".
+        # Indicates whether the clog service is available. To enable the clog service, submit a ticket.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.tenant_connections:
             for k in self.tenant_connections:
                 if k:
                     k.validate()
@@ -11583,14 +11565,16 @@
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
@@ -11643,14 +11627,16 @@
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
@@ -11689,17 +11675,17 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeTenantResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant=None):
-        # The request ID.
+        # The zone information of the tenant.
         self.request_id = request_id  # type: str
-        # The information of the tenant.
+        # The ID of the zone.
         self.tenant = tenant  # type: DescribeTenantResponseBodyTenant
 
     def validate(self):
         if self.tenant:
             self.tenant.validate()
 
     def to_map(self):
@@ -11762,41 +11748,28 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantMetricsRequest(TeaModel):
     def __init__(self, end_time=None, instance_id=None, metrics=None, page_number=None, page_size=None,
                  start_time=None, tenant_id=None, tenant_id_list=None, tenant_name=None):
-        # The end time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.end_time = end_time  # type: str
-        # The ID of the OceanBase cluster.
+        # 2021-06-13T15:40:43Z
         self.instance_id = instance_id  # type: str
-        # The monitoring metrics.   
-        # For more information about supported metrics, see [View tenant statistics](~~212125~~).
+        # {"name":"DescribeTenantMetrics","product":"OceanBasePro","version":"2019-09-01","path":"/","deprecated":0,"method":"POST|GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"Action\",\"position\":\"Query\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"\",\"example\":\"DescribeTenantMetrics\"},{\"name\":\"InstanceId\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"ob317v4uif****\"},{\"name\":\"PageSize\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"10\"},{\"name\":\"PageNumber\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"1\"},{\"name\":\"TenantName\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":true,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"pay_online\"},{\"name\":\"StartTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:40:43Z\"},{\"name\":\"EndTime\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"2021-06-13T15:45:43Z\"},{\"name\":\"Metrics\",\"position\":\"Body\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tps\"},{\"name\":\"TenantId\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":true,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"tfafd34fs****\"},{\"name\":\"TenantIdList\",\"position\":\"Body\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"[tdak3nac****,tdakc42df****]\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"TotalCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"\",\"description\":\"\",\"example\":\"9\"},{\"name\":\"RequestId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"EE205C00-30E4-XXXX-XXXX-87E3A8A2AA0C\"},{\"name\":\"TenantMetrics\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"\",\"description\":\"\",\"example\":\"\\\"Metrics\\\":[ {\\\"request_queue_rt\\\":0.0,\\\"TimeStamp\\\":\\\"2022-02-23T01:58:00Z\\\"}]\"}],\"title\":\"\",\"description\":\"\"}","errors":"{}"}
         self.metrics = metrics  # type: str
-        # The number of the page to return.    
-        # - Start value: 1 
-        # - Default value: 1
+        # The ID of the OceanBase cluster.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # tfafd34fs****\
         self.page_size = page_size  # type: int
-        # The start time of the time range for querying monitoring data.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # Example 1
         self.start_time = start_time  # type: str
-        # The ID of the tenant.   
-        # > <br>This parameter will be deprecated. We recommend that you use the TenantIdList parameter instead.
         self.tenant_id = tenant_id  # type: str
-        # The list of tenant IDs.
         self.tenant_id_list = tenant_id_list  # type: str
-        # The name of the tenant.    
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.   
-        # > <br>This parameter will be deprecated. We recommend that you use the TenantIdList parameter instead.
+        # 2021-06-13T15:45:43Z
         self.tenant_name = tenant_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantMetricsRequest, self).to_map()
@@ -11845,19 +11818,16 @@
         if m.get('TenantName') is not None:
             self.tenant_name = m.get('TenantName')
         return self
 
 
 class DescribeTenantMetricsResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_metrics=None, total_count=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The metrics of the tenant.
         self.tenant_metrics = tenant_metrics  # type: str
-        # The total count.
         self.total_count = total_count  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantMetricsResponseBody, self).to_map()
@@ -12298,23 +12268,15 @@
             temp_model = DescribeTenantTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantUserRolesResponseBody(TeaModel):
     def __init__(self, request_id=None, role=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The list of roles of the user.   
-        # Valid values: 
-        # 
-        # ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.
-        # ReadOnly: a role that has only the read-only privilege SELECT.
-        # DDL: a role that has DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW.
-        # DML: a role that has DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.role = role  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantUserRolesResponseBody, self).to_map()
@@ -12374,26 +12336,24 @@
             temp_model = DescribeTenantUserRolesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantUsersRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, search_key=None, tenant_id=None, user_name=None):
-        # The number of the page to return.    
-        # Start value: 1. Default value: 1.
+        # The database privileges of the account.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.    
-        # Maximum value: 100. Default value: 10.
+        # The return result of the request.
         self.page_size = page_size  # type: int
-        # The search keyword.
+        # The return result of the request.
         self.search_key = search_key  # type: str
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTenantUsers**.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantUsersRequest, self).to_map()
@@ -12426,29 +12386,16 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeTenantUsersResponseBodyTenantUsersDatabases(TeaModel):
     def __init__(self, database=None, role=None, table=None):
-        # The name of the database (MySQL mode) or schema (Oracle mode).
         self.database = database  # type: str
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
         self.role = role  # type: str
-        # The name of the table.
         self.table = table  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantUsersResponseBodyTenantUsersDatabases, self).to_map()
@@ -12474,29 +12421,22 @@
             self.table = m.get('Table')
         return self
 
 
 class DescribeTenantUsersResponseBodyTenantUsers(TeaModel):
     def __init__(self, databases=None, description=None, instance_id=None, tenant_id=None, user_name=None,
                  user_status=None, user_type=None):
-        # The database privileges of the account.
         self.databases = databases  # type: list[DescribeTenantUsersResponseBodyTenantUsersDatabases]
-        # The description of the database account.
         self.description = description  # type: str
+        # 所属集群Id
         self.instance_id = instance_id  # type: str
+        # 所属租户Id
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.
         self.user_name = user_name  # type: str
-        # The status of the database account. Valid values:   
-        #  - LOCKED: The account is locked.   
-        # - NORMAL: The account is unlocked.
         self.user_status = user_status  # type: str
-        # The type of the database account. Valid values:    
-        # - Admin: the super administrator account.   
-        # - NORMAL: a general account.
         self.user_type = user_type  # type: str
 
     def validate(self):
         if self.databases:
             for k in self.databases:
                 if k:
                     k.validate()
@@ -12545,19 +12485,31 @@
         if m.get('UserType') is not None:
             self.user_type = m.get('UserType')
         return self
 
 
 class DescribeTenantUsersResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_users=None, total_count=None):
-        # The request ID.
+        # The name of the database account.
         self.request_id = request_id  # type: str
-        # The list of database accounts in the tenant.
+        # The type of the database account. Valid values:    
+        # - Admin: the super administrator account.   
+        # - NORMAL: a general account.
         self.tenant_users = tenant_users  # type: list[DescribeTenantUsersResponseBodyTenantUsers]
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
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.tenant_users:
             for k in self.tenant_users:
                 if k:
                     k.validate()
@@ -12629,17 +12581,17 @@
             temp_model = DescribeTenantUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantZonesReadRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_id=None):
-        # The ID of the OceanBase cluster.
+        # The zone information of the tenant.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantZonesReadRequest, self).to_map()
@@ -12661,23 +12613,19 @@
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class DescribeTenantZonesReadResponseBodyTenantZones(TeaModel):
     def __init__(self, is_electable=None, is_primary=None, is_read_only_address_master=None, is_readable=None,
                  zone=None):
-        # Indicates whether the zone can be set as the primary zone.
+        # Example 1
         self.is_electable = is_electable  # type: bool
-        # Indicates whether the zone is the primary zone.
         self.is_primary = is_primary  # type: bool
-        # Indicates whether a read-only connection has been created.
         self.is_read_only_address_master = is_read_only_address_master  # type: bool
-        # Indicates whether a read-only connection needs to be created for the zone.
         self.is_readable = is_readable  # type: str
-        # The ID of the zone.
         self.zone = zone  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantZonesReadResponseBodyTenantZones, self).to_map()
@@ -12710,17 +12658,17 @@
         if m.get('Zone') is not None:
             self.zone = m.get('Zone')
         return self
 
 
 class DescribeTenantZonesReadResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_zones=None):
-        # The request ID.
+        # Indicates whether a read-only connection needs to be created for the zone.
         self.request_id = request_id  # type: str
-        # The zone information of the tenant.
+        # The request ID.
         self.tenant_zones = tenant_zones  # type: list[DescribeTenantZonesReadResponseBodyTenantZones]
 
     def validate(self):
         if self.tenant_zones:
             for k in self.tenant_zones:
                 if k:
                     k.validate()
@@ -12789,30 +12737,25 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTenantsRequest(TeaModel):
     def __init__(self, instance_id=None, page_number=None, page_size=None, search_key=None, tenant_id=None,
                  tenant_name=None):
-        # The ID of the OceanBase cluster.
+        # The number of used disks of the tenant.
         self.instance_id = instance_id  # type: str
-        # The number of the page to return.   
-        # Start value: 1
-        # - Default value: 1
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100.
-        # - Default value: 10
+        # You can call this operation to query the tenants in an OceanBase cluster.
         self.page_size = page_size  # type: int
-        # The search keyword.
+        # The primary zone of the tenant.
         self.search_key = search_key  # type: str
-        # The ID of the tenant.
+        # Alibaba Cloud CLI
         self.tenant_id = tenant_id  # type: str
-        # The name of the tenant.   
-        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
+        # The information of tenants.
         self.tenant_name = tenant_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantsRequest, self).to_map()
@@ -12855,63 +12798,74 @@
     def __init__(self, charset=None, collation=None, cpu=None, create_time=None, deploy_mode=None, deploy_type=None,
                  description=None, mem=None, primary_zone=None, status=None, tenant_id=None, tenant_mode=None, tenant_name=None,
                  unit_cpu=None, unit_mem=None, unit_num=None, used_disk_size=None, vpc_id=None):
         self.charset = charset  # type: str
         self.collation = collation  # type: str
         # The total number of CPU cores of the tenant.
         self.cpu = cpu  # type: int
-        # The time when the tenant was created.
+        # The number of CPU cores in each resource unit of the tenant.
         self.create_time = create_time  # type: str
-        # The data replica distribution mode of the tenant.   
-        # 
-        # - For the high availability version, N-N-N indicates the three-zone mode, and N-N indicates the dual-zone or single-zone mode.
-        # - For the basic version, N indicates the single-zone mode. 
-        # 
-        # > <br>N represents the number of nodes in a single zone.
+        # The search keyword.
         self.deploy_mode = deploy_mode  # type: str
-        # The deployment type of the tenant. <br>
-        # - multiple: multi-IDC deployment
-        # - single: single-IDC deployment
-        # - dual: dual-IDC deployment
+        # The name of the tenant.   
+        # It must start with a letter or an underscore (_), and contain 2 to 20 characters, which can be uppercase letters, lowercase letters, digits, and underscores (_).  It cannot be set to sys.
         self.deploy_type = deploy_type  # type: str
-        # The description of the tenant.
+        # Example 1
         self.description = description  # type: str
-        # The total memory size of the tenant, in GB.
+        # The number of the page to return.   
+        # Start value: 1
+        # - Default value: 1
         self.mem = mem  # type: int
-        # The primary zone of the tenant.
+        # The return result of the request.
         self.primary_zone = primary_zone  # type: str
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
         self.status = status  # type: str
-        # The ID of the tenant.
+        # You can call this operation to query the tenants in an OceanBase cluster.
         self.tenant_id = tenant_id  # type: str
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
         self.tenant_mode = tenant_mode  # type: str
-        # The name of the tenant.
+        # The information of tenants.
         self.tenant_name = tenant_name  # type: str
-        # The number of CPU cores in each resource unit of the tenant.
         self.unit_cpu = unit_cpu  # type: int
-        # The memory size of each resource unit of the tenant, in GB.
         self.unit_mem = unit_mem  # type: int
-        # The number of resource units in the tenant.
         self.unit_num = unit_num  # type: int
-        # The number of used disks of the tenant.
         self.used_disk_size = used_disk_size  # type: float
-        # The ID of the VPC.   <br>If no suitable VPC is available, create a VPC as prompted. For more information, see "What is a VPC".
+        # The time when the tenant was created.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTenantsResponseBodyTenants, self).to_map()
@@ -12996,19 +12950,19 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeTenantsResponseBody(TeaModel):
     def __init__(self, request_id=None, tenants=None, total_count=None):
-        # The request ID.
+        # The ID of the tenant.
         self.request_id = request_id  # type: str
-        # The information of tenants.
+        # The ID of the OceanBase cluster.
         self.tenants = tenants  # type: list[DescribeTenantsResponseBodyTenants]
-        # The total number of tenants in the specified OceanBase cluster.
+        # The total memory size of the tenant, in GB.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.tenants:
             for k in self.tenants:
                 if k:
                     k.validate()
@@ -13080,17 +13034,18 @@
             temp_model = DescribeTenantsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTimeZonesResponseBodyTimeZonesList(TeaModel):
     def __init__(self, description=None, time_zone=None):
-        # The description of the time zone.
+        # Example 1
         self.description = description  # type: str
-        # The name of the time zone.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTimeZones**.
         self.time_zone = time_zone  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTimeZonesResponseBodyTimeZonesList, self).to_map()
@@ -13111,15 +13066,14 @@
         if m.get('TimeZone') is not None:
             self.time_zone = m.get('TimeZone')
         return self
 
 
 class DescribeTimeZonesResponseBodyTimeZones(TeaModel):
     def __init__(self, default=None, list=None):
-        # The default time zone.
         self.default = default  # type: str
         # The list of time zones.
         self.list = list  # type: list[DescribeTimeZonesResponseBodyTimeZonesList]
 
     def validate(self):
         if self.list:
             for k in self.list:
@@ -13150,17 +13104,17 @@
                 temp_model = DescribeTimeZonesResponseBodyTimeZonesList()
                 self.list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTimeZonesResponseBody(TeaModel):
     def __init__(self, request_id=None, time_zones=None):
-        # The request ID.
+        # DescribeTimeZones
         self.request_id = request_id  # type: str
-        # The time zones supported by the tenant.
+        # The description of the time zone.
         self.time_zones = time_zones  # type: DescribeTimeZonesResponseBodyTimeZones
 
     def validate(self):
         if self.time_zones:
             self.time_zones.validate()
 
     def to_map(self):
@@ -13224,49 +13178,46 @@
         return self
 
 
 class DescribeTopSQLListRequest(TeaModel):
     def __init__(self, db_name=None, end_time=None, filter_condition=None, node_ip=None, page_number=None,
                  page_size=None, sqlid=None, search_key_word=None, search_parameter=None, search_rule=None, search_value=None,
                  sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The name of the database.
+        # The number of block index cache hits.
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The SQL type.
         self.end_time = end_time  # type: str
-        # The filter condition.
+        # The average number of logical reads of the SQL statement during the specified period of time.   
+        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
+        # 
+        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
         self.filter_condition = filter_condition  # type: dict[str, any]
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip  # type: str
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The queuing time, in ms.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of row cache hits.
         self.page_size = page_size  # type: int
-        # SQLID.
+        # The I/O wait time, in ms.
         self.sqlid = sqlid  # type: str
-        # The search keyword.
+        # The number of retries.
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # SQLID.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.
+        # The IP address of the client.
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # The number of Bloom filter cache hits.
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The number of rows read from the disk.
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The list of top SQL statements.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time, in ms.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # The average CPU time, in ms.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTopSQLListRequest, self).to_map()
@@ -13341,49 +13292,46 @@
         return self
 
 
 class DescribeTopSQLListShrinkRequest(TeaModel):
     def __init__(self, db_name=None, end_time=None, filter_condition_shrink=None, node_ip=None, page_number=None,
                  page_size=None, sqlid=None, search_key_word=None, search_parameter=None, search_rule=None, search_value=None,
                  sort_column=None, sort_order=None, start_time=None, tenant_id=None):
-        # The name of the database.
+        # The number of block index cache hits.
         self.db_name = db_name  # type: str
-        # The end time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The SQL type.
         self.end_time = end_time  # type: str
-        # The filter condition.
+        # The average number of logical reads of the SQL statement during the specified period of time.   
+        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
+        # 
+        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
         self.filter_condition_shrink = filter_condition_shrink  # type: str
-        # The IP address of the node.
+        # The number of failures.
         self.node_ip = node_ip  # type: str
-        # The number of the page to return.    
-        # - Start value: 1   
-        # - Default value: 1
+        # The queuing time, in ms.
         self.page_number = page_number  # type: int
-        # The number of rows to return on each page.   
-        # - Maximum value: 100   
-        # - Default value: 10
+        # The number of row cache hits.
         self.page_size = page_size  # type: int
-        # SQLID.
+        # The I/O wait time, in ms.
         self.sqlid = sqlid  # type: str
-        # The search keyword.
+        # The number of retries.
         self.search_key_word = search_key_word  # type: str
-        # The search parameter.
+        # SQLID.
         self.search_parameter = search_parameter  # type: str
-        # The search rule.
+        # The IP address of the client.
         self.search_rule = search_rule  # type: str
-        # The search value.
+        # The number of Bloom filter cache hits.
         self.search_value = search_value  # type: str
-        # The sorted column.
+        # The number of rows read from the disk.
         self.sort_column = sort_column  # type: str
-        # The sorting rule.
+        # The list of top SQL statements.
         self.sort_order = sort_order  # type: str
-        # The start time of the time range for querying TOP SQL statements.   
-        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
+        # The maximum response time, in ms.
         self.start_time = start_time  # type: str
-        # The ID of the tenant.
+        # The average CPU time, in ms.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTopSQLListShrinkRequest, self).to_map()
@@ -13463,96 +13411,114 @@
                  bloom_filter_cache_hit=None, client_ip=None, concurrency_wait_time=None, cpu_time=None, db_name=None, decode_time=None,
                  disk_read=None, elapsed_time=None, event=None, exec_per_second=None, execute_time=None, executions=None,
                  fail_times=None, get_plan_time=None, iowait_time=None, key=None, logical_read=None, max_cpu_time=None,
                  max_elapsed_time=None, memstore_read_row_count=None, miss_plans=None, net_wait_time=None, node_ip=None,
                  queue_time=None, rpccount=None, remote_plans=None, retry_count=None, return_rows=None, row_cache_hit=None,
                  sqlid=None, sqltext=None, sqltype=None, schedule_time=None, ssstore_read_row_count=None,
                  total_wait_time=None, user_name=None):
-        # The number of rows affected.
+        # The internal wait time, in ms.
         self.affected_rows = affected_rows  # type: long
-        # The wait time of the client, in ms.
+        # The wait time in concurrent execution, in ms.
         self.app_wait_time = app_wait_time  # type: float
-        # The number of block cache hits.
+        # The average CPU time, in ms.
         self.block_cache_hit = block_cache_hit  # type: long
-        # The number of block index cache hits.
+        # $.parameters[16].schema.example
         self.block_index_cache_hit = block_index_cache_hit  # type: long
-        # The number of Bloom filter cache hits.
+        # $.parameters[14].schema.enumValueTitles
         self.bloom_filter_cache_hit = bloom_filter_cache_hit  # type: long
-        # The IP address of the client.
+        # $.parameters[14].schema.description
         self.client_ip = client_ip  # type: str
-        # The wait time in concurrent execution, in ms.
+        # The number of rows returned.
         self.concurrency_wait_time = concurrency_wait_time  # type: float
-        # The average CPU time, in ms.
+        # The maximum CPU time, in ms.
         self.cpu_time = cpu_time  # type: float
-        # The name of the database.
+        # The number of remote plans.
         self.db_name = db_name  # type: str
-        # The time to wait for decoding, in ms.
+        # The number of rows to return on each page.   
+        # - Maximum value: 100   
+        # - Default value: 10
         self.decode_time = decode_time  # type: float
-        # The number of physical reads.
+        # The IP address of the client.
         self.disk_read = disk_read  # type: long
-        # The average response time, in ms.
+        # The sorting rule.
         self.elapsed_time = elapsed_time  # type: float
-        # The wait event.
+        # The number of rows read from the disk.
         self.event = event  # type: str
-        # The number of executions per second.
+        # The operation that you want to perform.   
+        # Set the value to **DescribeTopSQLList**.
         self.exec_per_second = exec_per_second  # type: float
-        # The internal execution time, in ms.
+        # The number of rows read from the memory.
         self.execute_time = execute_time  # type: float
-        # The number of executions.
+        # The number of executions per second.
         self.executions = executions  # type: long
-        # The number of failures.
+        # $.parameters[12].schema.description
         self.fail_times = fail_times  # type: long
-        # The time spent in hard parsing, in ms.
+        # The queuing time, in ms.
         self.get_plan_time = get_plan_time  # type: float
-        # The I/O wait time, in ms.
+        # $.parameters[15].schema.example
         self.iowait_time = iowait_time  # type: float
-        # The sequence number of the returned SQL statement.
+        # The name of the database.
         self.key = key  # type: long
-        # The average number of logical reads of the SQL statement during the specified period of time.   
-        # The value covers the numbers of reads of different caches and the number of disk I/Os. It is an important metric for measuring the SQL filtering performance.   
-        # 
-        # > <br> A higher ratio of the number of logical reads to the number of returned rows indicates poorer filtering performance. General causes include non-standard content written by SQL statements, non-standard table indexes created, and non-standard SQL execution plans.
+        # You can call this operation to query SQL execution performance data collected by the diagnostic system.
         self.logical_read = logical_read  # type: long
-        # The maximum CPU time, in ms.
+        # SQLID.
         self.max_cpu_time = max_cpu_time  # type: float
-        # The maximum response time, in ms.
+        # The sequence number of the returned SQL statement.
         self.max_elapsed_time = max_elapsed_time  # type: float
-        # The number of rows read from the memory.
+        # The name of the database.
         self.memstore_read_row_count = memstore_read_row_count  # type: long
-        # The number of plan misses.
+        # The total count.
         self.miss_plans = miss_plans  # type: long
-        # The network latency, in ms.
+        # The end time of the time range for querying TOP SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.net_wait_time = net_wait_time  # type: float
-        # The IP address of the node.
+        # The username.
         self.node_ip = node_ip  # type: str
-        # The queuing time, in ms.
+        # $.parameters[12].schema.enumValueTitles
         self.queue_time = queue_time  # type: float
-        # The number of RPCs.
+        # The start time of the time range for querying TOP SQL statements.   
+        # The value must be UTC time in the format of YYYY-MM-DDThh:mm:ssZ.
         self.rpccount = rpccount  # type: long
-        # The number of remote plans.
+        # The return result of the request.
         self.remote_plans = remote_plans  # type: long
-        # The number of retries.
+        # $.parameters[13].schema.description
         self.retry_count = retry_count  # type: long
-        # The number of rows returned.
+        # The wait event.
         self.return_rows = return_rows  # type: long
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
         self.row_cache_hit = row_cache_hit  # type: long
-        # SQLID.
+        # $.parameters[13].schema.example
         self.sqlid = sqlid  # type: str
-        # The SQL text.
+        # The list of top SQL statements.
         self.sqltext = sqltext  # type: str
-        # The SQL type.
+        # The request ID.
         self.sqltype = sqltype  # type: long
-        # The scheduling duration, in ms.
+        # The search keyword.
         self.schedule_time = schedule_time  # type: float
-        # The number of rows read from the disk.
         self.ssstore_read_row_count = ssstore_read_row_count  # type: long
-        # The internal wait time, in ms.
+        # -\
         self.total_wait_time = total_wait_time  # type: float
-        # The username.
+        # The number of Bloom filter cache hits.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTopSQLListResponseBodyTopSQLList, self).to_map()
@@ -13725,19 +13691,19 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class DescribeTopSQLListResponseBody(TeaModel):
     def __init__(self, request_id=None, top_sqllist=None, total_count=None):
-        # The request ID.
+        # Alibaba Cloud CLI
         self.request_id = request_id  # type: str
-        # The list of top SQL statements.
+        # The I/O wait time, in ms.
         self.top_sqllist = top_sqllist  # type: list[DescribeTopSQLListResponseBodyTopSQLList]
-        # The total count.
+        # It is an online CLI tool that allows you to quickly retrieve and debug APIs. It can dynamically generate executable SDK code samples.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.top_sqllist:
             for k in self.top_sqllist:
                 if k:
                     k.validate()
@@ -13809,21 +13775,18 @@
             temp_model = DescribeTopSQLListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeZonesRequest(TeaModel):
     def __init__(self, deploy_type=None, series=None):
-        # The deployment type of the cluster. Valid values:   
-        # - multiple: multi-IDC deployment   
-        # - single: single-IDC deployment   
-        # - dual: dual-IDC deployment
+        # The operation that you want to perform.   
+        # Set the value to **DescribeZones**.
         self.deploy_type = deploy_type  # type: str
-        # The series of the OceanBase cluster. Valid values:   
-        # NORMAL: the high availability version. This is the default value.
+        # The deployment mode.
         self.series = series  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeZonesRequest, self).to_map()
@@ -13844,23 +13807,17 @@
         if m.get('Series') is not None:
             self.series = m.get('Series')
         return self
 
 
 class DescribeZonesResponseBodyZones(TeaModel):
     def __init__(self, deploy_type=None, series=None, zone_id=None, zone_name=None):
-        # The deployment mode.
         self.deploy_type = deploy_type  # type: str
-        # The series of the OceanBase cluster. Valid values:   
-        # NORMAL: the high availability version. This is the default value.
         self.series = series  # type: str
-        # The list of zone IDs.   
-        # For a cluster with multiple zones, separate the zone names with commas (,).
         self.zone_id = zone_id  # type: str
-        # The name of the zone.
         self.zone_name = zone_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeZonesResponseBodyZones, self).to_map()
@@ -13889,17 +13846,22 @@
         if m.get('ZoneName') is not None:
             self.zone_name = m.get('ZoneName')
         return self
 
 
 class DescribeZonesResponseBody(TeaModel):
     def __init__(self, request_id=None, zones=None):
-        # The request ID.
+        # ```
+        # http(s)://[Endpoint]/?Action=DescribeZones
+        # &Series=normal
+        # &DeployType=single
+        # &Common request parameters
+        # ```
         self.request_id = request_id  # type: str
-        # The list of zones.
+        # You can call this operation to learn of zones where a cluster can be created in an Alibaba Cloud region.
         self.zones = zones  # type: list[DescribeZonesResponseBodyZones]
 
     def validate(self):
         if self.zones:
             for k in self.zones:
                 if k:
                     k.validate()
@@ -13965,24 +13927,224 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeZonesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class KillProcessListRequest(TeaModel):
+    def __init__(self, instance_id=None, session_list=None, tenant_id=None):
+        # The ID of the OceanBase cluster.
+        self.instance_id = instance_id  # type: str
+        # The list of the sessions that need to be closed.
+        self.session_list = session_list  # type: str
+        # The ID of the tenant.
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(KillProcessListRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, client_ip=None, command=None, database=None, error_message=None, execute_time=None,
+                 server_ip=None, session_id=None, sql_text=None, status=None, tenant_id=None, user=None):
+        # The client IP address.
+        self.client_ip = client_ip  # type: str
+        # The start command for the container of the application.
+        self.command = command  # type: str
+        # The name of the database.
+        self.database = database  # type: str
+        # The error message.
+        self.error_message = error_message  # type: str
+        # Execution time (UTC+8). If it is left empty, it means to execute immediately.
+        self.execute_time = execute_time  # type: str
+        # The IP address of the server.
+        self.server_ip = server_ip  # type: str
+        # The ID of the session.
+        self.session_id = session_id  # type: long
+        # The SQL statement.
+        self.sql_text = sql_text  # type: str
+        # The status of the task.
+        self.status = status  # type: str
+        # The ID of the tenant.
+        self.tenant_id = tenant_id  # type: str
+        # The database username.
+        self.user = user  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(KillProcessListResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        # The data returned.
+        self.data = data  # type: list[KillProcessListResponseBodyData]
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(KillProcessListResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: KillProcessListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(KillProcessListResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, database_name=None, description=None, instance_id=None, tenant_id=None):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # Example 1
         self.database_name = database_name  # type: str
-        # The description of the database.
         self.description = description  # type: str
-        # The ID of the OceanBase cluster.
+        # The description of the database.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyDatabaseDescription**.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDatabaseDescriptionRequest, self).to_map()
@@ -14011,15 +14173,14 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class ModifyDatabaseDescriptionResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDatabaseDescriptionResponseBody, self).to_map()
@@ -14075,22 +14236,21 @@
             temp_model = ModifyDatabaseDescriptionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDatabaseUserRolesRequest(TeaModel):
     def __init__(self, database_name=None, instance_id=None, tenant_id=None, users=None):
-        # The name of the database.    
-        # You cannot use reserved keywords, such as test and mysql.
+        # The ID of the tenant.
         self.database_name = database_name  # type: str
-        # The ID of the OceanBase cluster.
+        # The account information.
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
-        self.tenant_id = tenant_id  # type: str
         # A list of usernames and their respective roles.
+        self.tenant_id = tenant_id  # type: str
+        # The ID of the OceanBase cluster.
         self.users = users  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDatabaseUserRolesRequest, self).to_map()
@@ -14119,22 +14279,15 @@
         if m.get('Users') is not None:
             self.users = m.get('Users')
         return self
 
 
 class ModifyDatabaseUserRolesResponseBodyTenantUserUsers(TeaModel):
     def __init__(self, role=None, user_name=None):
-        # The role of the account.   
-        # In MySQL mode, a role is a database-level role. Valid values:
-        # - ReadWrite: a role that has the read and write privileges, namely ALL PRIVILEGES.
-        # - ReadOnly: a role that has only the read-only privilege SELECT. 
-        # - DDL: a role that has the DDL privileges such as CREATE, DROP, ALTER, SHOW VIEW, and CREATE VIEW. 
-        # - DML: a role that has the DML privileges such as SELECT, INSERT, UPDATE, DELETE, and SHOW VIEW.
         self.role = role  # type: str
-        # The name of the account.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDatabaseUserRolesResponseBodyTenantUserUsers, self).to_map()
@@ -14155,19 +14308,17 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class ModifyDatabaseUserRolesResponseBodyTenantUser(TeaModel):
     def __init__(self, database_name=None, tenant_id=None, users=None):
-        # The name of the database.
+        # Example 1
         self.database_name = database_name  # type: str
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The accounts that have privileges on the database.
         self.users = users  # type: list[ModifyDatabaseUserRolesResponseBodyTenantUserUsers]
 
     def validate(self):
         if self.users:
             for k in self.users:
                 if k:
                     k.validate()
@@ -14200,17 +14351,16 @@
                 temp_model = ModifyDatabaseUserRolesResponseBodyTenantUserUsers()
                 self.users.append(temp_model.from_map(k))
         return self
 
 
 class ModifyDatabaseUserRolesResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_user=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The account information.
+        # The name of the database.
         self.tenant_user = tenant_user  # type: ModifyDatabaseUserRolesResponseBodyTenantUser
 
     def validate(self):
         if self.tenant_user:
             self.tenant_user.validate()
 
     def to_map(self):
@@ -14272,18 +14422,17 @@
             temp_model = ModifyDatabaseUserRolesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceNameRequest(TeaModel):
     def __init__(self, instance_id=None, instance_name=None):
-        # The ID of the OceanBase cluster.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.instance_id = instance_id  # type: str
-        # The name of the OceanBase cluster.   
-        # It must be 1 to 20 characters in length.
+        # The ID of the OceanBase cluster.
         self.instance_name = instance_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyInstanceNameRequest, self).to_map()
@@ -14306,15 +14455,16 @@
         return self
 
 
 class ModifyInstanceNameResponseBody(TeaModel):
     def __init__(self, instance_name=None, request_id=None):
         # The name of the OceanBase cluster.
         self.instance_name = instance_name  # type: str
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyInstanceName**.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyInstanceNameResponseBody, self).to_map()
@@ -14625,17 +14775,17 @@
             temp_model = ModifyInstanceSpecResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceTagsRequest(TeaModel):
     def __init__(self, instance_id=None, tags=None):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id  # type: str
         # The tags.
+        self.instance_id = instance_id  # type: str
+        # You can call this operation to modify the value of the cluster tags.
         self.tags = tags  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyInstanceTagsRequest, self).to_map()
@@ -14656,17 +14806,15 @@
         if m.get('Tags') is not None:
             self.tags = m.get('Tags')
         return self
 
 
 class ModifyInstanceTagsResponseBody(TeaModel):
     def __init__(self, message=None, request_id=None):
-        # The update status of the tags.
         self.message = message  # type: str
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyInstanceTagsResponseBody, self).to_map()
@@ -14726,26 +14874,22 @@
             temp_model = ModifyInstanceTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyParametersRequest(TeaModel):
     def __init__(self, dimension=None, dimension_value=None, instance_id=None, parameters=None):
-        # The type of the parameter.   
-        # Valid values: CLUSTER and TENANT.
+        # The ID of the OceanBase cluster.
         self.dimension = dimension  # type: str
-        # The resource ID of the parameter type.    
-        # You can leave this parameter unspecified when you call this operation to modify cluster parameters. In the case of tenant parameters, pass the tenant ID.
+        # The cause of the modification failure.
         self.dimension_value = dimension_value  # type: str
-        # The ID of the OceanBase cluster.
+        # Alibaba Cloud CLI
         self.instance_id = instance_id  # type: str
-        # The parameters.   
-        # It is a JSON array. Each object in the array has two elements: Name and Value. 
-        # 
-        # > <br>The names and values of cluster parameters that can be modified are different from those of tenant parameters. For more information, see DescribeParameters.
+        # The resource ID of the parameter type.    
+        # You can leave this parameter unspecified when you call this operation to modify cluster parameters. In the case of tenant parameters, pass the tenant ID.
         self.parameters = parameters  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyParametersRequest, self).to_map()
@@ -14774,19 +14918,15 @@
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
         return self
 
 
 class ModifyParametersResponseBodyResults(TeaModel):
     def __init__(self, message=None, success=None):
-        # The cause of the modification failure.
         self.message = message  # type: str
-        # Indicates whether the parameter has been modified. Valid values:   
-        # true: The modification is successful. 
-        # false: The modification failed.
         self.success = success  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyParametersResponseBodyResults, self).to_map()
@@ -14807,17 +14947,18 @@
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class ModifyParametersResponseBody(TeaModel):
     def __init__(self, request_id=None, results=None):
-        # The request ID.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyParameters**.
         self.request_id = request_id  # type: str
-        # The modification results.
+        # Example 1
         self.results = results  # type: ModifyParametersResponseBodyResults
 
     def validate(self):
         if self.results:
             self.results.validate()
 
     def to_map(self):
@@ -14881,16 +15022,15 @@
         return self
 
 
 class ModifySecurityIpsRequest(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The name of the IP address whitelist group.   
-        # It must be 2 to 32 characters in length, start with a lowercase letter, end with a lowercase letter or digit, and contain only lowercase letters, digits, and underscores (_).
+        # The information of the IP address whitelist group.
         self.security_ip_group_name = security_ip_group_name  # type: str
         # The list of IP addresses and CIDR blocks in the whitelist.   
         # It is a JSON array. Each object in the array is an IP address or CIDR block. You can specify at most 40 IP addresses or CIDR blocks.
         self.security_ips = security_ips  # type: str
 
     def validate(self):
         pass
@@ -14918,20 +15058,16 @@
         if m.get('SecurityIps') is not None:
             self.security_ips = m.get('SecurityIps')
         return self
 
 
 class ModifySecurityIpsResponseBodySecurityIpGroup(TeaModel):
     def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None):
-        # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
-        # The name of the security group.
         self.security_ip_group_name = security_ip_group_name  # type: str
-        # The list of IP addresses and CIDR blocks in the whitelist.   
-        # The return values of SecurityIps are strings that are separated with commas (,).
         self.security_ips = security_ips  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifySecurityIpsResponseBodySecurityIpGroup, self).to_map()
@@ -14958,15 +15094,15 @@
         return self
 
 
 class ModifySecurityIpsResponseBody(TeaModel):
     def __init__(self, request_id=None, security_ip_group=None):
         # The request ID.
         self.request_id = request_id  # type: str
-        # The information of the IP address whitelist group.
+        # Example 1
         self.security_ip_group = security_ip_group  # type: ModifySecurityIpsResponseBodySecurityIpGroup
 
     def validate(self):
         if self.security_ip_group:
             self.security_ip_group.validate()
 
     def to_map(self):
@@ -15029,28 +15165,34 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantPrimaryZoneRequest(TeaModel):
     def __init__(self, instance_id=None, master_intranet_address_zone=None, modify_type=None, primary_zone=None,
                  primary_zone_deploy_type=None, tenant_id=None, user_vswitch_id=None):
-        # The ID of the OceanBase cluster.
+        # The primary zone of the tenant.    
+        # It is one of the zones in which the cluster is deployed.
         self.instance_id = instance_id  # type: str
-        # The availability zone where the primary node is located.
+        # ```
+        # http(s)://[Endpoint]/?Action=ModifyTenantPrimaryZone
+        # &TenantId=ob2mr3oae0****\
+        # &InstanceId=ob317v4uif****\
+        # &PrimaryZone=cn-hangzhou-h
+        # &Common request parameters
+        # ```
         self.master_intranet_address_zone = master_intranet_address_zone  # type: str
         # The switching mode.
         self.modify_type = modify_type  # type: str
-        # The primary zone of the tenant.    
-        # It is one of the zones in which the cluster is deployed.
+        # The ID of the vSwitch.
         self.primary_zone = primary_zone  # type: str
-        # The deployment type of the primary zone.
+        # Example 1
         self.primary_zone_deploy_type = primary_zone_deploy_type  # type: str
-        # The ID of the tenant.
+        # The return result of the request.
         self.tenant_id = tenant_id  # type: str
-        # The ID of the vSwitch.
+        # The request ID.
         self.user_vswitch_id = user_vswitch_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantPrimaryZoneRequest, self).to_map()
@@ -15091,15 +15233,14 @@
         if m.get('UserVSwitchId') is not None:
             self.user_vswitch_id = m.get('UserVSwitchId')
         return self
 
 
 class ModifyTenantPrimaryZoneResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantPrimaryZoneResponseBody, self).to_map()
@@ -15155,21 +15296,22 @@
             temp_model = ModifyTenantPrimaryZoneResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantResourceRequest(TeaModel):
     def __init__(self, cpu=None, instance_id=None, memory=None, tenant_id=None):
-        # The information about the CPU resources of the tenant.
+        # The memory size of the tenant, in GB.
         self.cpu = cpu  # type: int
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantResource**.
         self.instance_id = instance_id  # type: str
-        # The memory size of the tenant, in GB.
-        self.memory = memory  # type: int
         # The ID of the tenant.
+        self.memory = memory  # type: int
+        # The information about the CPU resources of the tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantResourceRequest, self).to_map()
@@ -15198,17 +15340,15 @@
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         return self
 
 
 class ModifyTenantResourceResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantResourceResponseBody, self).to_map()
@@ -15370,22 +15510,22 @@
             temp_model = ModifyTenantTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantUserDescriptionRequest(TeaModel):
     def __init__(self, description=None, instance_id=None, tenant_id=None, user_name=None):
-        # The description of the database.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserDescription**.
         self.description = description  # type: str
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
         # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
+        # The description of the database.
         self.user_name = user_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserDescriptionRequest, self).to_map()
@@ -15414,15 +15554,15 @@
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class ModifyTenantUserDescriptionResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
+        # You can call this operation to modify the description of a specified account in a tenant.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserDescriptionResponseBody, self).to_map()
@@ -15477,61 +15617,70 @@
         if m.get('body') is not None:
             temp_model = ModifyTenantUserDescriptionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantUserPasswordRequest(TeaModel):
-    def __init__(self, instance_id=None, tenant_id=None, user_name=None, user_password=None):
-        # The ID of the OceanBase cluster.
+    def __init__(self, encryption_type=None, instance_id=None, tenant_id=None, user_name=None, user_password=None):
+        # 加密方式。
+        self.encryption_type = encryption_type  # type: str
         self.instance_id = instance_id  # type: str
-        # The ID of the tenant.
+        # ```
+        # http(s)://[Endpoint]/?Action=ModifyTenantUserPassword
+        # &UserName=pay_test
+        # &TenantId=ob2mr3oae0****\
+        # &UserPassword=!Aliyun4Oceanbase
+        # &InstanceId=ob317v4uif****\
+        # &Common request parameters
+        # ```
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The ID of the OceanBase cluster.
         self.user_name = user_name  # type: str
-        # The password of the database account.    
-        # It must be 10 to 32 characters in length and contain three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. The special characters are ! @ # $ % \ ^ \ & \ * ( ) _ + - =\
+        # You can call this operation to change the logon password of a specified account in a tenant.
         self.user_password = user_password  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserPasswordRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
             self.user_password = m.get('UserPassword')
         return self
 
 
 class ModifyTenantUserPasswordResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserPasswordResponseBody, self).to_map()
@@ -15587,28 +15736,30 @@
             temp_model = ModifyTenantUserPasswordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantUserRolesRequest(TeaModel):
     def __init__(self, instance_id=None, modify_type=None, tenant_id=None, user_name=None, user_role=None):
-        # The ID of the OceanBase cluster.
-        self.instance_id = instance_id  # type: str
         # The type of the privilege modification operation.   
         # Valid values:  
         # update: updates all privileges. This is the default value.  
         # add: adds a privilege.  
         # delete: deletes a privilege.
+        self.instance_id = instance_id  # type: str
+        # The name of the table.
         self.modify_type = modify_type  # type: str
-        # The ID of the tenant.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserRoles**.
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.   
-        # You cannot use reserved keywords, such as SYS and root.
-        self.user_name = user_name  # type: str
         # The role of the database account.
+        self.user_name = user_name  # type: str
+        # The type of the account. Valid values:   
+        # - Admin: the super administrator account.   
+        # - Normal: a general account.
         self.user_role = user_role  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserRolesRequest, self).to_map()
@@ -15641,21 +15792,27 @@
         if m.get('UserRole') is not None:
             self.user_role = m.get('UserRole')
         return self
 
 
 class ModifyTenantUserRolesResponseBodyTenantUserUserRole(TeaModel):
     def __init__(self, database=None, is_success=None, role=None, table=None):
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
         self.database = database  # type: str
-        # Indicates whether the privilege was granted to the role.
         self.is_success = is_success  # type: bool
-        # The role of the account.
+        # You can call this operation to modify the database privileges of a specified account in a tenant.
         self.role = role  # type: str
-        # The name of the table.
         self.table = table  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserRolesResponseBodyTenantUserUserRole, self).to_map()
@@ -15684,21 +15841,17 @@
         if m.get('Table') is not None:
             self.table = m.get('Table')
         return self
 
 
 class ModifyTenantUserRolesResponseBodyTenantUser(TeaModel):
     def __init__(self, tenant_id=None, user_name=None, user_role=None):
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The name of the account.
         self.user_name = user_name  # type: str
-        # The type of the account. Valid values:   
-        # - Admin: the super administrator account.   
-        # - Normal: a general account.
+        # The name of the database (MySQL mode) or schema (Oracle mode).
         self.user_role = user_role  # type: list[ModifyTenantUserRolesResponseBodyTenantUserUserRole]
 
     def validate(self):
         if self.user_role:
             for k in self.user_role:
                 if k:
                     k.validate()
@@ -15731,17 +15884,16 @@
                 temp_model = ModifyTenantUserRolesResponseBodyTenantUserUserRole()
                 self.user_role.append(temp_model.from_map(k))
         return self
 
 
 class ModifyTenantUserRolesResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_user=None):
-        # The request ID.
         self.request_id = request_id  # type: str
-        # The list of database accounts in the tenant.
+        # The ID of the tenant.
         self.tenant_user = tenant_user  # type: ModifyTenantUserRolesResponseBodyTenantUser
 
     def validate(self):
         if self.tenant_user:
             self.tenant_user.validate()
 
     def to_map(self):
@@ -15803,20 +15955,20 @@
             temp_model = ModifyTenantUserRolesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTenantUserStatusRequest(TeaModel):
     def __init__(self, instance_id=None, tenant_id=None, user_name=None, user_status=None):
-        # The ID of the OceanBase cluster.
+        # The operation that you want to perform.   
+        # Set the value to **ModifyTenantUserStatus**.
         self.instance_id = instance_id  # type: str
         # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The name of the database account.    
-        # You cannot use reserved keywords, such as SYS and root.
+        # The list of database accounts in the tenant.
         self.user_name = user_name  # type: str
         # The status of the database account. Valid values:   
         # - Locked: The account is locked. 
         # - Online: The account is unlocked.
         self.user_status = user_status  # type: str
 
     def validate(self):
@@ -15849,21 +16001,16 @@
         if m.get('UserStatus') is not None:
             self.user_status = m.get('UserStatus')
         return self
 
 
 class ModifyTenantUserStatusResponseBodyTenantUser(TeaModel):
     def __init__(self, tenant_id=None, user_name=None, user_status=None):
-        # The ID of the tenant.
         self.tenant_id = tenant_id  # type: str
-        # The name of the account.
         self.user_name = user_name  # type: str
-        # The status of the database account. Valid values:   
-        # - LOCKED: The account is locked. 
-        # - ONLINE: The account is unlocked.
         self.user_status = user_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTenantUserStatusResponseBodyTenantUser, self).to_map()
@@ -15888,17 +16035,16 @@
         if m.get('UserStatus') is not None:
             self.user_status = m.get('UserStatus')
         return self
 
 
 class ModifyTenantUserStatusResponseBody(TeaModel):
     def __init__(self, request_id=None, tenant_user=None):
-        # The request ID.
+        # Example 1
         self.request_id = request_id  # type: str
-        # The list of database accounts in the tenant.
         self.tenant_user = tenant_user  # type: list[ModifyTenantUserStatusResponseBodyTenantUser]
 
     def validate(self):
         if self.tenant_user:
             for k in self.tenant_user:
                 if k:
                     k.validate()
@@ -15966,21 +16112,21 @@
             temp_model = ModifyTenantUserStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ReleaseOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReleaseOmsOpenAPIProjectRequest, self).to_map()
@@ -16009,21 +16155,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class ReleaseOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **ReleaseOmsOpenAPIProject**.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level  # type: str
-        # The error description (new).
+        # The error code (new).
         self.message = message  # type: str
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReleaseOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -16053,35 +16199,29 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class ReleaseOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # You can call this operation to release a data synchronization project.
         self.advice = advice  # type: str
-        # The error code (old).
+        # Indicates whether the project is released.
         self.code = code  # type: str
-        # The time spent, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the project is released.
         self.data = data  # type: bool
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail  # type: ReleaseOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
+        # A system error occurred.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -16179,21 +16319,21 @@
             temp_model = ReleaseOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResetOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # The total count, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Indicates whether the call is successful.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResetOmsOpenAPIProjectRequest, self).to_map()
@@ -16222,21 +16362,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class ResetOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The operation that you want to perform. Set the value to **ResetOmsOpenAPIProject**.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error description (old).
         self.level = level  # type: str
-        # The error description (new).
+        # The error code (new).
         self.message = message  # type: str
-        # The suggestions (new).
+        # The page number, which takes effect in a pagination query.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResetOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -16266,35 +16406,29 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class ResetOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # You can call this operation to reset a data synchronization project.
         self.advice = advice  # type: str
-        # The error code (old).
+        # Indicates whether the resetting is successful.
         self.code = code  # type: str
-        # The time spent, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the resetting is successful.
         self.data = data  # type: bool
-        # The error details.
+        # The suggestions (new).
         self.error_detail = error_detail  # type: ResetOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
+        # A system error occurred.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The page number, which takes effect in a pagination query.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -16392,21 +16526,21 @@
             temp_model = ResetOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResumeOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # Indicates whether the call is successful.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # Contact the administrator.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The suggestions (old).
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResumeOmsOpenAPIProjectRequest, self).to_map()
@@ -16435,21 +16569,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class ResumeOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The suggestions (new).
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The operation that you want to perform. Set the value to **ResumeOmsOpenAPIProject**.
         self.level = level  # type: str
-        # The error description (new).
+        # The error description (old).
         self.message = message  # type: str
-        # The suggestions (new).
+        # The error code (new).
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResumeOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -16479,35 +16613,30 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class ResumeOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # The request ID.
         self.advice = advice  # type: str
-        # The error code (old).
+        # The page number, which takes effect in a pagination query.
         self.code = code  # type: str
-        # The time spent, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the project is resumed.
         self.data = data  # type: bool
-        # The error details.
+        # The page number, which takes effect in a pagination query.
         self.error_detail = error_detail  # type: ResumeOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
+        # The error details.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
+        # Example 1
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The error level. Valid values: CRITICAL, ERROR, and WARN.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -16606,29 +16735,29 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SearchOmsOpenAPIMonitorMetricRequest(TeaModel):
     def __init__(self, begin_time=None, end_time=None, max_point_num=None, metric=None, page_number=None,
                  page_size=None, project_id=None, worker_grade_id=None):
-        # The query start time, which is a second-level timestamp.
+        # Alibaba Cloud provides SDKs in different languages to help you quickly integrate Alibaba Cloud products and services by using APIs. We recommend that you use an SDK to call APIs. In this way, you do not need to sign for verification.
         self.begin_time = begin_time  # type: long
-        # The query end time, which is a second-level timestamp.
+        # It is an Alibaba Cloud asset management and configuration tool, with which you can manage multiple Alibaba Cloud products and services by using commands. It is easy to use and a good helper in migration to cloud.
         self.end_time = end_time  # type: long
-        # The maximum number of query points.
+        # Contact the administrator.
         self.max_point_num = max_point_num  # type: long
-        # The query metric. For example, if you want to query the incremental transactions per second (TPS), set the value to CONNECTOR_TPS. Valid values: CONNECTOR_TPS: the TPS of the Connector component; CONNECTOR_DELAY: the latency of the Connector component; CONNECTOR_SOURCE_QUEUE_SIZE: the queue size of the Connector source; CONNECTOR_IOPS: the Connector IOPS; CONNECTOR_WRITE_COST: the time spent in writing at the Connector destination; CONNECTOR_SOURCE_READ_COST: the time spent in reading at the Connector source; JDBCWRITER_DELAY: the latency of the JDBCWriter; JDBCWRITER_IOPS: the IOPS of the JDBCWriter; JDBCWRITER_RPS: the requests per second (RPS) of the JDBCWriter; STORE_DELAY: the latency of the Store component; STORE_CONN: the number of store connections; STORE_IOPS: the IOPS of the Store component; STORE_TPS: the TPS of the Store component; CHECKER_SOURCE_NONE_RPS: the instantaneous RPS of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_RPS: the average RPS of the Checker component at the source end during full migration; CHECKER_DEST_NONE_RPS: the instantaneous RPS of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_RPS: the average RPS of the Checker component at the destination end during full migration; CHECKER_SOURCE_NONE_RT: the instantaneous response time (RT) of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_RT: the average RT of the Checker component at the source end during full migration; CHECKER_DEST_NONE_RT: the instantaneous RT of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_RT: the average RT of the Checker component at the destination end during full migration; CHECKER_SOURCE_NONE_READ_IOPS: the instantaneous read IOPS of the Checker component at the source end during full migration; CHECKER_SOURCE_AVG_READ_IOPS: the average read IOPS of the Checker component at the source end during full migration; CHECKER_DEST_NONE_WRITE_IOPS: the instantaneous write IOPS of the Checker component at the destination end during full migration; CHECKER_DEST_AVG_WRITE_IOPS: the average write IOPS of the Checker component at the destination end during full migration; CHECKER_VERIFY_SOURCE_NONE_RPS: the instantaneous RPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_RPS: the average RPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_RPS: the instantaneous RPS of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_DEST_AVG_RPS: the average RPS of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_SOURCE_NONE_RT: the instantaneous RT of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_RT: the average RT of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_RT: the instantaneous RT of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_DEST_AVG_RT: the average RT of the Checker-Verify component at the destination end during full verification; CHECKER_VERIFY_SOURCE_NONE_READ_IOPS: the instantaneous read IOPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_SOURCE_AVG_READ_IOPS: the average read IOPS of the Checker-Verify component at the source end during full verification; CHECKER_VERIFY_DEST_NONE_READ_IOPS: the instantaneous read IOPS of the Checker-Verify component at the destination end during full verification; and CHECKER_VERIFY_DEST_AVG_READ_IOPS: the average read IOPS of the Checker-Verify component at the destination end during full verification.
+        # The business data returned.
         self.metric = metric  # type: str
-        # The page number, which takes effect in a pagination query.
+        # The information about the object.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # A millisecond-level timestamp.
         self.page_size = page_size  # type: int
-        # The ID of the project to query.
+        # The value corresponding to the time.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The name of the metric.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SearchOmsOpenAPIMonitorMetricRequest, self).to_map()
@@ -16673,17 +16802,15 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class SearchOmsOpenAPIMonitorMetricResponseBodyDataDataPoints(TeaModel):
     def __init__(self, timestamp=None, value=None):
-        # A millisecond-level timestamp.
         self.timestamp = timestamp  # type: long
-        # The value corresponding to the time.
         self.value = value  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SearchOmsOpenAPIMonitorMetricResponseBodyDataDataPoints, self).to_map()
@@ -16706,15 +16833,14 @@
         return self
 
 
 class SearchOmsOpenAPIMonitorMetricResponseBodyData(TeaModel):
     def __init__(self, data_points=None, metric=None, tags=None):
         # connector data point
         self.data_points = data_points  # type: list[SearchOmsOpenAPIMonitorMetricResponseBodyDataDataPoints]
-        # The name of the metric.
         self.metric = metric  # type: str
         # metric tags
         self.tags = tags  # type: dict[str, str]
 
     def validate(self):
         if self.data_points:
             for k in self.data_points:
@@ -16749,21 +16875,21 @@
         if m.get('Tags') is not None:
             self.tags = m.get('Tags')
         return self
 
 
 class SearchOmsOpenAPIMonitorMetricResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The information about the object.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (old).
         self.level = level  # type: str
-        # The error description (new).
+        # The ID of the project to query.
         self.message = message  # type: str
-        # The suggestions (new).
+        # The error description (new).
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SearchOmsOpenAPIMonitorMetricResponseBodyErrorDetail, self).to_map()
@@ -16793,35 +16919,34 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class SearchOmsOpenAPIMonitorMetricResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.advice = advice  # type: str
-        # The error code (old).
+        # The business data returned.
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
+        # The request ID.
         self.cost = cost  # type: str
-        # The business data returned.
         self.data = data  # type: list[SearchOmsOpenAPIMonitorMetricResponseBodyData]
-        # The error details.
+        # A system error occurred.
         self.error_detail = error_detail  # type: SearchOmsOpenAPIMonitorMetricResponseBodyErrorDetail
-        # The error description (old).
+        # The suggestions (old).
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
+        # The error code (new).
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # The page number, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
+        # The time spent in processing the request, in seconds.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
-        self.success = success  # type: bool
         # The total count, which takes effect in a pagination query.
+        self.success = success  # type: bool
+        # The error details.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -18286,21 +18411,21 @@
             temp_model = SearchOmsOpenAPIProjectsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StartOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The page number, which takes effect in a pagination query.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # The total count, which takes effect in a pagination query.
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartOmsOpenAPIProjectRequest, self).to_map()
@@ -18329,21 +18454,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class StartOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The error description (old).
         self.code = code  # type: str
-        # Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (new).
         self.level = level  # type: str
-        # The error description (new).
+        # The page number, which takes effect in a pagination query.
         self.message = message  # type: str
-        # The suggestions (new).
+        # The error details.
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -18373,35 +18498,27 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class StartOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions.
         self.advice = advice  # type: str
-        # The error code (old).
+        # The request ID.
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the project is started.
         self.data = data  # type: bool
-        # The error details.
+        # The operation that you want to perform. Set the value to **StartOmsOpenAPIProject**.
         self.error_detail = error_detail  # type: StartOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The suggestions (new).
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.error_detail:
             self.error_detail.validate()
 
     def to_map(self):
@@ -18499,21 +18616,21 @@
             temp_model = StartOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StopOmsOpenAPIProjectRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
-        # The page number, which takes effect in a pagination query.
+        # The suggestions (old).
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
+        # Contact the administrator.
         self.page_size = page_size  # type: int
-        # The project ID.
+        # The total count, which takes effect in a pagination query.
         self.project_id = project_id  # type: str
-        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
+        # Alibaba Cloud CLI
         self.worker_grade_id = worker_grade_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StopOmsOpenAPIProjectRequest, self).to_map()
@@ -18542,21 +18659,21 @@
         if m.get('WorkerGradeId') is not None:
             self.worker_grade_id = m.get('WorkerGradeId')
         return self
 
 
 class StopOmsOpenAPIProjectResponseBodyErrorDetail(TeaModel):
     def __init__(self, code=None, level=None, message=None, proposal=None):
-        # The error code (new).
+        # The time spent in processing the request, in seconds.
         self.code = code  # type: str
-        # The error level. Valid values: CRITICAL, ERROR, and WARN.
+        # The error code (old).
         self.level = level  # type: str
-        # The error description (new).
+        # The project ID.
         self.message = message  # type: str
-        # The suggestions (new).
+        # The error description (new).
         self.proposal = proposal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StopOmsOpenAPIProjectResponseBodyErrorDetail, self).to_map()
@@ -18586,35 +18703,31 @@
             self.proposal = m.get('Proposal')
         return self
 
 
 class StopOmsOpenAPIProjectResponseBody(TeaModel):
     def __init__(self, advice=None, code=None, cost=None, data=None, error_detail=None, message=None,
                  page_number=None, page_size=None, request_id=None, success=None, total_count=None):
-        # The suggestions (old).
+        # Indicates whether the project is paused.
         self.advice = advice  # type: str
-        # The error code (old).
+        # The page size, which takes effect in a pagination query.
         self.code = code  # type: str
-        # The time spent in processing the request, in seconds.
         self.cost = cost  # type: str
-        # Indicates whether the project is paused.
         self.data = data  # type: bool
-        # The error details.
+        # A system error occurred.
         self.error_detail = error_detail  # type: StopOmsOpenAPIProjectResponseBodyErrorDetail
-        # The error description (old).
+        # The page size, which takes effect in a pagination query.
         self.message = message  # type: str
-        # The page number, which takes effect in a pagination query.
+        # Pause a data synchronization project
         self.page_number = page_number  # type: int
-        # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
-        # The request ID.
+        # A system error occurred.
         self.request_id = request_id  # type: str
-        # Indicates whether the call is successful.
+        # The ID of the migration instance. Generally, if you want to create a project on a public cloud, you must first purchase a migration instance.
         self.success = success  # type: bool
-        # The total count, which takes effect in a pagination query.
         self.total_count = total_count  # type: long
 
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

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901_py2.
 
-Created on 10/04/2023
+Created on 19/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2"
```

