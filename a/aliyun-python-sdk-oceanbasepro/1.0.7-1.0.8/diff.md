# Comparing `tmp/aliyun-python-sdk-oceanbasepro-1.0.7.tar.gz` & `tmp/aliyun-python-sdk-oceanbasepro-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-oceanbasepro-1.0.7.tar", last modified: Mon Apr 10 02:31:40 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-oceanbasepro-1.0.8.tar", last modified: Fri May 19 06:28:30 2023, max compression
```

## Comparing `aliyun-python-sdk-oceanbasepro-1.0.7.tar` & `aliyun-python-sdk-oceanbasepro-1.0.8.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1582 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      545 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1582 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5654 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/
--rw-r--r--   0 root         (0) root         (0)     2618 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3486 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2384 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py
--rw-r--r--   0 root         (0) root         (0)     4110 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
--rw-r--r--   0 root         (0) root         (0)     2410 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-10 02:31:40.000000 aliyun-python-sdk-oceanbasepro-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-10 02:31:39.000000 aliyun-python-sdk-oceanbasepro-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      545 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5720 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/setup.py
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/LICENSE` & `aliyun-python-sdk-oceanbasepro-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/PKG-INFO` & `aliyun-python-sdk-oceanbasepro-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oceanbasepro
-Version: 1.0.7
+Version: 1.0.8
 Summary: The oceanbasepro module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oceanbasepro
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/README.rst` & `aliyun-python-sdk-oceanbasepro-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oceanbasepro
-Version: 1.0.7
+Version: 1.0.8
 Summary: The oceanbasepro module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oceanbasepro
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py
+aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/endpoint.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_TenantMode(self): # String
 		return self.get_body_params().get('TenantMode')
 
 	def set_TenantMode(self, TenantMode):  # String
 		self.add_body_params('TenantMode', TenantMode)
+	def get_Series(self): # String
+		return self.get_body_params().get('Series')
+
+	def set_Series(self, Series):  # String
+		self.add_body_params('Series', Series)
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DiskSize(self): # Long
-		return self.get_body_params().get('DiskSize')
-
-	def set_DiskSize(self, DiskSize):  # Long
-		self.add_body_params('DiskSize', DiskSize)
 	def get_InstanceClass(self): # String
 		return self.get_body_params().get('InstanceClass')
 
 	def set_InstanceClass(self, InstanceClass):  # String
 		self.add_body_params('InstanceClass', InstanceClass)
+	def get_DiskSize(self): # Long
+		return self.get_body_params().get('DiskSize')
+
+	def set_DiskSize(self, DiskSize):  # Long
+		self.add_body_params('DiskSize', DiskSize)
 	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoceanbasepro.endpoint import endpoint_data
 
-class ModifyTenantUserPasswordRequest(RpcRequest):
+class ModifyTenantUserRolesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserPassword','oceanbase')
+		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserRoles','oceanbase')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_UserPassword(self): # String
-		return self.get_body_params().get('UserPassword')
+	def get_UserRole(self): # String
+		return self.get_body_params().get('UserRole')
 
-	def set_UserPassword(self, UserPassword):  # String
-		self.add_body_params('UserPassword', UserPassword)
+	def set_UserRole(self, UserRole):  # String
+		self.add_body_params('UserRole', UserRole)
 	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
+	def get_ModifyType(self): # String
+		return self.get_body_params().get('ModifyType')
+
+	def set_ModifyType(self, ModifyType):  # String
+		self.add_body_params('ModifyType', ModifyType)
 	def get_TenantId(self): # String
 		return self.get_body_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # String
 		self.add_body_params('TenantId', TenantId)
 	def get_UserName(self): # String
 		return self.get_body_params().get('UserName')
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,40 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoceanbasepro.endpoint import endpoint_data
 
-class ModifyTenantUserRolesRequest(RpcRequest):
+class ModifyTenantUserStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserRoles','oceanbase')
+		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserStatus','oceanbase')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_UserRole(self): # String
-		return self.get_body_params().get('UserRole')
+	def get_UserStatus(self): # String
+		return self.get_body_params().get('UserStatus')
 
-	def set_UserRole(self, UserRole):  # String
-		self.add_body_params('UserRole', UserRole)
+	def set_UserStatus(self, UserStatus):  # String
+		self.add_body_params('UserStatus', UserStatus)
 	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
-	def get_ModifyType(self): # String
-		return self.get_body_params().get('ModifyType')
-
-	def set_ModifyType(self, ModifyType):  # String
-		self.add_body_params('ModifyType', ModifyType)
 	def get_TenantId(self): # String
 		return self.get_body_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # String
 		self.add_body_params('TenantId', TenantId)
 	def get_UserName(self): # String
 		return self.get_body_params().get('UserName')
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,38 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoceanbasepro.endpoint import endpoint_data
 
-class ModifyTenantUserStatusRequest(RpcRequest):
+class ModifyTenantUserPasswordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserStatus','oceanbase')
+		RpcRequest.__init__(self, 'OceanBasePro', '2019-09-01', 'ModifyTenantUserPassword','oceanbase')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_UserStatus(self): # String
-		return self.get_body_params().get('UserStatus')
+	def get_UserPassword(self): # String
+		return self.get_body_params().get('UserPassword')
 
-	def set_UserStatus(self, UserStatus):  # String
-		self.add_body_params('UserStatus', UserStatus)
+	def set_UserPassword(self, UserPassword):  # String
+		self.add_body_params('UserPassword', UserPassword)
 	def get_InstanceId(self): # String
 		return self.get_body_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_body_params('InstanceId', InstanceId)
 	def get_TenantId(self): # String
 		return self.get_body_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # String
 		self.add_body_params('TenantId', TenantId)
+	def get_EncryptionType(self): # String
+		return self.get_body_params().get('EncryptionType')
+
+	def set_EncryptionType(self, EncryptionType):  # String
+		self.add_body_params('EncryptionType', EncryptionType)
 	def get_UserName(self): # String
 		return self.get_body_params().get('UserName')
 
 	def set_UserName(self, UserName):  # String
 		self.add_body_params('UserName', UserName)
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.7/setup.py` & `aliyun-python-sdk-oceanbasepro-1.0.8/setup.py`

 * *Files identical despite different names*

