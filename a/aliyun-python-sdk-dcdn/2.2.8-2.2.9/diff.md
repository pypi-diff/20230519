# Comparing `tmp/aliyun-python-sdk-dcdn-2.2.8.tar.gz` & `tmp/aliyun-python-sdk-dcdn-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dcdn-2.2.8.tar", last modified: Thu Nov 17 12:08:07 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dcdn-2.2.9.tar", last modified: Tue Nov 29 08:48:19 2022, max compression
```

## Comparing `aliyun-python-sdk-dcdn-2.2.8.tar` & `aliyun-python-sdk-dcdn-2.2.9.tar`

### file list

```diff
@@ -1,202 +1,203 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/
--rw-r--r--   0 root         (0) root         (0)      575 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12813 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3477 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/
--rw-r--r--   0 root         (0) root         (0)     3404 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/AddDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     3170 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/AddDcdnIpaDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2995 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchAddDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchCreateDcdnWafRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2281 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1625 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnWafRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchModifyDcdnWafRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2921 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2257 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnIpaDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnWafDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CheckDcdnProjectExistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CommitStagingRoutineCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2315 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3021 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnSLSRealTimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2229 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnWafPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1955 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateRoutineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateSlrAndSlsProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2733 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DcdnHttpRequestTestToolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2040 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaSpecificConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnRealTimeLogProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1441 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1619 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnWafPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineCodeRevisionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1757 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineConfEnvsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1587 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1581 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteWasmRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnAclFieldsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2519 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2145 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBlockedRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1853 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeletedDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1634 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeliverListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2585 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainByCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2929 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCcActivityLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCertificateInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1643 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1855 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2193 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2770 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2967 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2187 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaConnDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2975 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIspDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2360 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainMultiUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2197 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2205 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPropertyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2585 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2421 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2037 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeByteHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2946 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeDetailDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2432 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2421 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2035 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeReqHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2036 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2030 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRegionDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopReferVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopUrlVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2593 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2708 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2603 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2613 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2611 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2324 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnErUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnHttpsDomainListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3884 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaUserDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnL2VipsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRealTimeDeliveryFieldRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1628 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTaskByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3303 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1664 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRegionAndIspRequest.py
--rw-r--r--   0 root         (0) root         (0)     1626 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2692 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealTimeLogTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1893 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1865 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecFuncInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecSpecInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1449 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnStagingIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1445 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSubListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2347 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnTopDomainsByFlowRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserCertificateExpireCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2611 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsByFuncRequest.py
--rw-r--r--   0 root         (0) root         (0)     4129 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1683 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserRealTimeDeliveryFieldRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropByMinuteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1948 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropRequest.py
--rw-r--r--   0 root         (0) root         (0)     1447 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnVerifyContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafFilterInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafGeoInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1624 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2265 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyValidDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafScenesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafSpecInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2356 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnsecServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRDDomainConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineCanaryEnvsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1853 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineCodeRevisionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1591 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1445 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineUserInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnIpaStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1451 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserErStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserLogserviceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1959 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/EditRoutineConfRequest.py
--rw-r--r--   0 root         (0) root         (0)     2237 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ListDcdnRealTimeDeliveryProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDCdnDomainSchdmByPropertyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2037 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2011 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2161 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2058 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/OpenDcdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2195 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PreloadDcdnObjectCachesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1873 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PublishDcdnStagingConfigToProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2005 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PublishRoutineCodeRevisionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/RefreshDcdnObjectCachesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/RollbackDcdnStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3090 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2271 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainSMCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2041 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnFullDomainsBlockIPRequest.py
--rw-r--r--   0 root         (0) root         (0)     2219 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnUserConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1635 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetRoutineSubdomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1837 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StartDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StartDcdnIpaDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StopDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StopDcdnIpaDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2331 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/TagDcdnResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2309 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UntagDcdnResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2495 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2448 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnIpaDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2819 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnSLSRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2171 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1846 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnUserRealTimeDeliveryFieldRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UploadRoutineCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UploadStagingRoutineCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/VerifyDcdnDomainOwnerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-11-17 12:08:07.000000 aliyun-python-sdk-dcdn-2.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2022-11-17 12:08:06.000000 aliyun-python-sdk-dcdn-2.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12873 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/
+-rw-r--r--   0 root         (0) root         (0)     3404 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/AddDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/AddDcdnIpaDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchAddDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchCreateDcdnWafRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnWafRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchModifyDcdnWafRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnIpaDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnWafDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CheckDcdnProjectExistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CommitStagingRoutineCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnSLSRealTimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnWafPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateRoutineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateSlrAndSlsProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DcdnHttpRequestTestToolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaSpecificConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnRealTimeLogProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnWafPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineCodeRevisionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineConfEnvsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteWasmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnAclFieldsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBlockedRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeletedDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeliverListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainByCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCcActivityLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCertificateInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaConnDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIspDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainMultiUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPropertyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeByteHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeDetailDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeReqHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRegionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopReferVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopUrlVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnErUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnHttpsDomainListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3884 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaUserDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnL2VipsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRealTimeDeliveryFieldRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTaskByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRegionAndIspRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealTimeLogTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecFuncInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecSpecInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnStagingIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSubListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnTopDomainsByFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserCertificateExpireCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsByFuncRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserRealTimeDeliveryFieldRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropByMinuteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnVerifyContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafFilterInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafGeoInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyValidDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafScenesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafSpecInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnsecServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRDDomainConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRDDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineCanaryEnvsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineCodeRevisionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineUserInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnIpaStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserErStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserLogserviceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/EditRoutineConfRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ListDcdnRealTimeDeliveryProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDCdnDomainSchdmByPropertyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/OpenDcdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PreloadDcdnObjectCachesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PublishDcdnStagingConfigToProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PublishRoutineCodeRevisionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/RefreshDcdnObjectCachesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/RollbackDcdnStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainSMCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnFullDomainsBlockIPRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnUserConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetRoutineSubdomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StartDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StartDcdnIpaDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StopDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StopDcdnIpaDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/TagDcdnResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UntagDcdnResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnIpaDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnSLSRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnUserRealTimeDeliveryFieldRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UploadRoutineCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UploadStagingRoutineCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/VerifyDcdnDomainOwnerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-11-29 08:48:19.000000 aliyun-python-sdk-dcdn-2.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2022-11-29 08:48:18.000000 aliyun-python-sdk-dcdn-2.2.9/setup.py
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/LICENSE` & `aliyun-python-sdk-dcdn-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/PKG-INFO` & `aliyun-python-sdk-dcdn-2.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dcdn
-Version: 2.2.8
+Version: 2.2.9
 Summary: The dcdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dcdn
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/README.rst` & `aliyun-python-sdk-dcdn-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/PKG-INFO` & `aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dcdn
-Version: 2.2.8
+Version: 2.2.9
 Summary: The dcdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dcdn
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyun_python_sdk_dcdn.egg-info/SOURCES.txt` & `aliyun-python-sdk-dcdn-2.2.9/aliyun_python_sdk_dcdn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRulesRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeDcdnWafScenesRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeDcdnWafServiceRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeDcdnWafSpecInfoRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeDcdnWafUsageDataRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeDcdnsecServiceRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRDDomainConfigRequest.py
+aliyunsdkdcdn/request/v20180115/DescribeRDDomainsRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRoutineCanaryEnvsRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRoutineCodeRevisionRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRoutineRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRoutineSpecRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeRoutineUserInfoRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeUserDcdnIpaStatusRequest.py
 aliyunsdkdcdn/request/v20180115/DescribeUserDcdnStatusRequest.py
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/endpoint.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/AddDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/AddDcdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/AddDcdnIpaDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/AddDcdnIpaDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchAddDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchAddDcdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchCreateDcdnWafRulesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchCreateDcdnWafRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnWafRulesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchDeleteDcdnWafRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchModifyDcdnWafRulesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchModifyDcdnWafRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainCertificateRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnIpaDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnIpaDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/BatchSetDcdnWafDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/BatchSetDcdnWafDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CheckDcdnProjectExistRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CheckDcdnProjectExistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CommitStagingRoutineCodeRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CommitStagingRoutineCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnDeliverTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnSLSRealTimeLogDeliveryRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnSLSRealTimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnSubTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateDcdnWafPolicyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateDcdnWafPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateRoutineRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateRoutineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/CreateSlrAndSlsProjectRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/CreateSlrAndSlsProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DcdnHttpRequestTestToolRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DcdnHttpRequestTestToolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnDeliverTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaSpecificConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnIpaSpecificConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnRealTimeLogProjectRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnRealTimeLogProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificStagingConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSpecificStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnSubTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteDcdnWafPolicyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteDcdnWafPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineCodeRevisionRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineCodeRevisionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineConfEnvsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineConfEnvsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteRoutineRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteRoutineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DeleteWasmRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DeleteWasmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnAclFieldsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnAclFieldsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpBpsDataRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,37 +32,32 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_Isp(self): # String
 		return self.get_query_params().get('Isp')
 
 	def set_Isp(self, Isp):  # String
 		self.add_query_param('Isp', Isp)
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_DevicePort(self): # String
-		return self.get_query_params().get('DevicePort')
-
-	def set_DevicePort(self, DevicePort):  # String
-		self.add_query_param('DevicePort', DevicePort)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
 	def get_Interval(self): # String
 		return self.get_query_params().get('Interval')
 
 	def set_Interval(self, Interval):  # String
 		self.add_query_param('Interval', Interval)
 	def get_DeviceName(self): # String
 		return self.get_query_params().get('DeviceName')
 
 	def set_DeviceName(self, DeviceName):  # String
 		self.add_query_param('DeviceName', DeviceName)
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
+	def get_DevicePort(self): # String
+		return self.get_query_params().get('DevicePort')
+
+	def set_DevicePort(self, DevicePort):  # String
+		self.add_query_param('DevicePort', DevicePort)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafUsageDataRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnBgpTrafficDataRequest(RpcRequest):
+class DescribeDcdnWafUsageDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnBgpTrafficData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnWafUsageData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Isp(self): # String
-		return self.get_query_params().get('Isp')
-
-	def set_Isp(self, Isp):  # String
-		self.add_query_param('Isp', Isp)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
+	def get_SplitBy(self): # String
+		return self.get_query_params().get('SplitBy')
+
+	def set_SplitBy(self, SplitBy):  # String
+		self.add_query_param('SplitBy', SplitBy)
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
+
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnBlockedRegionsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBlockedRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateDetailRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeletedDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRDDomainsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDeletedDomainsRequest(RpcRequest):
+class DescribeRDDomainsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDeletedDomains')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeRDDomains')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeliverListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDeliverListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataByLayerRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainByCertificateRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainByCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCcActivityLogRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCcActivityLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCertificateInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCertificateInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCnameRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainCnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainDetailRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHitRateDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataByLayerRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaConnDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginBpsDataRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDomainIpaConnDataRequest(RpcRequest):
+class DescribeDcdnDomainOriginBpsDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainIpaConnData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainOriginBpsData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_SplitBy(self): # String
-		return self.get_query_params().get('SplitBy')
-
-	def set_SplitBy(self, SplitBy):  # String
-		self.add_query_param('SplitBy', SplitBy)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
@@ -52,7 +47,12 @@
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
+
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIspDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIspDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainLogRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainMultiUsageDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainMultiUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginTrafficDataRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDomainOriginBpsDataRequest(RpcRequest):
+class DescribeDcdnDomainOriginTrafficDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainOriginBpsData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainOriginTrafficData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainOriginTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRegionDataRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDomainOriginTrafficDataRequest(RpcRequest):
+class DescribeDcdnDomainRegionDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainOriginTrafficData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainRegionData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,12 +47,7 @@
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_Interval(self): # String
-		return self.get_query_params().get('Interval')
-
-	def set_Interval(self, Interval):  # String
-		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPropertyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPropertyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPvDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainPvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataByLayerRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeByteHitRateDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeByteHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeDetailDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeDetailDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeHttpCodeDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeQpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeReqHitRateDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeReqHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcHttpCodeDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeSrcTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRealTimeTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainRegionDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUvDataRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDomainRegionDataRequest(RpcRequest):
+class DescribeDcdnDomainUvDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainRegionData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainUvData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopReferVisitRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopReferVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopUrlVisitRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTopUrlVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUsageDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainUvDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainIpaConnDataRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,38 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnDomainUvDataRequest(RpcRequest):
+class DescribeDcdnDomainIpaConnDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainUvData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnDomainIpaConnData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
+	def get_SplitBy(self): # String
+		return self.get_query_params().get('SplitBy')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
+	def set_SplitBy(self, SplitBy):  # String
+		self.add_query_param('SplitBy', SplitBy)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketBpsDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketHttpCodeDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketTrafficDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnDomainWebsocketTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnErUsageDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnErUsageDataRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,37 +27,32 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_Spec(self): # String
-		return self.get_query_params().get('Spec')
-
-	def set_Spec(self, Spec):  # String
-		self.add_query_param('Spec', Spec)
 	def get_RoutineID(self): # String
 		return self.get_query_params().get('RoutineID')
 
 	def set_RoutineID(self, RoutineID):  # String
 		self.add_query_param('RoutineID', RoutineID)
+	def get_Spec(self): # String
+		return self.get_query_params().get('Spec')
+
+	def set_Spec(self, Spec):  # String
+		self.add_query_param('Spec', Spec)
 	def get_SplitBy(self): # String
 		return self.get_query_params().get('SplitBy')
 
 	def set_SplitBy(self, SplitBy):  # String
 		self.add_query_param('SplitBy', SplitBy)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnHttpsDomainListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnHttpsDomainListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainDetailRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaServiceRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaUserDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnIpaUserDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnL2VipsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnL2VipsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRealTimeDeliveryFieldRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserRealTimeDeliveryFieldRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnRealTimeDeliveryFieldRequest(RpcRequest):
+class DescribeDcdnUserRealTimeDeliveryFieldRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnRealTimeDeliveryField')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnUserRealTimeDeliveryField')
+		self.set_method('GET')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_BusinessType(self): # String
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshQuotaRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTaskByIdRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTaskByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTasksRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRefreshTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnRegionAndIspRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRegionAndIspRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealTimeLogTypeRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealTimeLogTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSLSRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateDetailRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSMCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecFuncInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecFuncInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSecSpecInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnStagingIpRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnSecSpecInfoRequest(RpcRequest):
+class DescribeDcdnStagingIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnSecSpecInfo')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnStagingIp')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnServiceRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnStagingIpRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineUserInfoRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnStagingIpRequest(RpcRequest):
+class DescribeRoutineUserInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnStagingIp')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeRoutineUserInfo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnSubListRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnSubListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnTagResourcesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnTopDomainsByFlowRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnTopDomainsByFlowRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillHistoryRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillTypeRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserBillTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserCertificateExpireCountRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserCertificateExpireCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserConfigsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsByFuncRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsByFuncRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserQuotaRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserRealTimeDeliveryFieldRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetRoutineSubdomainRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnUserRealTimeDeliveryFieldRequest(RpcRequest):
+class SetRoutineSubdomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnUserRealTimeDeliveryField')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'SetRoutineSubdomain')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_BusinessType(self): # String
-		return self.get_query_params().get('BusinessType')
+	def get_Subdomains(self): # String
+		return self.get_body_params().get('Subdomains')
 
-	def set_BusinessType(self, BusinessType):  # String
-		self.add_query_param('BusinessType', BusinessType)
+	def set_Subdomains(self, Subdomains):  # String
+		self.add_body_params('Subdomains', Subdomains)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserResourcePackageRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserResourcePackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropByMinuteRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropByMinuteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserSecDropRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserTagsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnUserTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnVerifyContentRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnVerifyContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainDetailRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafFilterInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafFilterInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafGeoInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafGeoInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPoliciesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyValidDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafPolicyValidDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRuleRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRuleRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,17 +27,12 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
 	def get_RuleId(self): # Long
 		return self.get_query_params().get('RuleId')
 
 	def set_RuleId(self, RuleId):  # Long
 		self.add_query_param('RuleId', RuleId)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRulesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafScenesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafScenesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafServiceRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafSpecInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafSpecInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnWafUsageDataRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnDomainRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeDcdnWafUsageDataRequest(RpcRequest):
+class UpdateDcdnDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnWafUsageData')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
+	def get_Sources(self): # String
+		return self.get_query_params().get('Sources')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_SplitBy(self): # String
-		return self.get_query_params().get('SplitBy')
+	def set_Sources(self, Sources):  # String
+		self.add_query_param('Sources', Sources)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
+
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
+	def get_TopLevelDomain(self): # String
+		return self.get_query_params().get('TopLevelDomain')
 
-	def set_SplitBy(self, SplitBy):  # String
-		self.add_query_param('SplitBy', SplitBy)
+	def set_TopLevelDomain(self, TopLevelDomain):  # String
+		self.add_query_param('TopLevelDomain', TopLevelDomain)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_Interval(self): # String
-		return self.get_query_params().get('Interval')
-
-	def set_Interval(self, Interval):  # String
-		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeDcdnsecServiceRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnsecServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRDDomainConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRDDomainConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineCanaryEnvsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineCanaryEnvsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineCodeRevisionRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineCodeRevisionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineSpecRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeRoutineSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeRoutineUserInfoRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserErStatusRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeRoutineUserInfoRequest(RpcRequest):
+class DescribeUserErStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeRoutineUserInfo')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeUserErStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnIpaStatusRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnIpaStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnStatusRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserDcdnStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserErStatusRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeUserLogserviceStatusRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeUserErStatusRequest(RpcRequest):
+class DescribeUserLogserviceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeUserErStatus')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeUserLogserviceStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/DescribeUserLogserviceStatusRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StartDcdnIpaDomainRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class DescribeUserLogserviceStatusRequest(RpcRequest):
+class StartDcdnIpaDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeUserLogserviceStatus')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StartDcdnIpaDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
 	def get_SecurityToken(self): # String
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
+
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/EditRoutineConfRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/EditRoutineConfRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ListDcdnRealTimeDeliveryProjectRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ListDcdnRealTimeDeliveryProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDCdnDomainSchdmByPropertyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDCdnDomainSchdmByPropertyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyDomainsRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafRuleRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/ModifyDcdnWafRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/OpenDcdnServiceRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/OpenDcdnServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PreloadDcdnObjectCachesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PreloadDcdnObjectCachesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PublishDcdnStagingConfigToProductionRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PublishDcdnStagingConfigToProductionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/PublishRoutineCodeRevisionRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/PublishRoutineCodeRevisionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/RefreshDcdnObjectCachesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/RefreshDcdnObjectCachesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/RollbackDcdnStagingConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainStagingConfigRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class RollbackDcdnStagingConfigRequest(RpcRequest):
+class SetDcdnDomainStagingConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'RollbackDcdnStagingConfig')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'SetDcdnDomainStagingConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Functions(self): # String
+		return self.get_query_params().get('Functions')
+
+	def set_Functions(self, Functions):  # String
+		self.add_query_param('Functions', Functions)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainCertificateRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainSMCertificateRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnDomainSMCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StopDcdnIpaDomainRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class SetDcdnDomainStagingConfigRequest(RpcRequest):
+class StopDcdnIpaDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'SetDcdnDomainStagingConfig')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StopDcdnIpaDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Functions(self): # String
-		return self.get_query_params().get('Functions')
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
 
-	def set_Functions(self, Functions):  # String
-		self.add_query_param('Functions', Functions)
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnFullDomainsBlockIPRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnFullDomainsBlockIPRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetDcdnUserConfigRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/SetDcdnUserConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/SetRoutineSubdomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StartDcdnDomainRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class SetRoutineSubdomainRequest(RpcRequest):
+class StartDcdnDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'SetRoutineSubdomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StartDcdnDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Subdomains(self): # String
-		return self.get_body_params().get('Subdomains')
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
 
-	def set_Subdomains(self, Subdomains):  # String
-		self.add_body_params('Subdomains', Subdomains)
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
+
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StartDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/StopDcdnDomainRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class StartDcdnDomainRequest(RpcRequest):
+class StopDcdnDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StartDcdnDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StopDcdnDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StartDcdnIpaDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/VerifyDcdnDomainOwnerRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class StartDcdnIpaDomainRequest(RpcRequest):
+class VerifyDcdnDomainOwnerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StartDcdnIpaDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'VerifyDcdnDomainOwner')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def get_VerifyType(self): # String
+		return self.get_query_params().get('VerifyType')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
+	def set_VerifyType(self, VerifyType):  # String
+		self.add_query_param('VerifyType', VerifyType)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StopDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnBgpTrafficDataRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class StopDcdnDomainRequest(RpcRequest):
+class DescribeDcdnBgpTrafficDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StopDcdnDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnBgpTrafficData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
+	def get_Isp(self): # String
+		return self.get_query_params().get('Isp')
 
-	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def set_Isp(self, Isp):  # String
+		self.add_query_param('Isp', Isp)
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/StopDcdnIpaDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UploadStagingRoutineCodeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class StopDcdnIpaDomainRequest(RpcRequest):
+class UploadStagingRoutineCodeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'StopDcdnIpaDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UploadStagingRoutineCode')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def get_CodeDescription(self): # String
+		return self.get_body_params().get('CodeDescription')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
-	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
-
-	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
+	def set_CodeDescription(self, CodeDescription):  # String
+		self.add_body_params('CodeDescription', CodeDescription)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_Name(self): # String
+		return self.get_body_params().get('Name')
+
+	def set_Name(self, Name):  # String
+		self.add_body_params('Name', Name)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/TagDcdnResourcesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/TagDcdnResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UntagDcdnResourcesRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UntagDcdnResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnDeliverTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnIpaDomainRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class UpdateDcdnDomainRequest(RpcRequest):
+class UpdateDcdnIpaDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnIpaDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnIpaDomainRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnSubTaskRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,48 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class UpdateDcdnIpaDomainRequest(RpcRequest):
+class UpdateDcdnSubTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnIpaDomain')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnSubTask')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Sources(self): # String
-		return self.get_query_params().get('Sources')
+	def get_StartTime(self): # String
+		return self.get_body_params().get('StartTime')
 
-	def set_Sources(self, Sources):  # String
-		self.add_query_param('Sources', Sources)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
-
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
-	def get_TopLevelDomain(self): # String
-		return self.get_query_params().get('TopLevelDomain')
-
-	def set_TopLevelDomain(self, TopLevelDomain):  # String
-		self.add_query_param('TopLevelDomain', TopLevelDomain)
+	def set_StartTime(self, StartTime):  # String
+		self.add_body_params('StartTime', StartTime)
 	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
+		return self.get_body_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
+		self.add_body_params('DomainName', DomainName)
+	def get_EndTime(self): # String
+		return self.get_body_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # String
+		self.add_body_params('EndTime', EndTime)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_ReportIds(self): # String
+		return self.get_body_params().get('ReportIds')
+
+	def set_ReportIds(self, ReportIds):  # String
+		self.add_body_params('ReportIds', ReportIds)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnSLSRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnSLSRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnSubTaskRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UploadRoutineCodeRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,43 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class UpdateDcdnSubTaskRequest(RpcRequest):
+class UploadRoutineCodeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UpdateDcdnSubTask')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UploadRoutineCode')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_body_params().get('StartTime')
+	def get_CodeDescription(self): # String
+		return self.get_body_params().get('CodeDescription')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_body_params('StartTime', StartTime)
-	def get_DomainName(self): # String
-		return self.get_body_params().get('DomainName')
-
-	def set_DomainName(self, DomainName):  # String
-		self.add_body_params('DomainName', DomainName)
-	def get_EndTime(self): # String
-		return self.get_body_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_body_params('EndTime', EndTime)
+	def set_CodeDescription(self, CodeDescription):  # String
+		self.add_body_params('CodeDescription', CodeDescription)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_ReportIds(self): # String
-		return self.get_body_params().get('ReportIds')
+	def get_Name(self): # String
+		return self.get_body_params().get('Name')
 
-	def set_ReportIds(self, ReportIds):  # String
-		self.add_body_params('ReportIds', ReportIds)
+	def set_Name(self, Name):  # String
+		self.add_body_params('Name', Name)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UpdateDcdnUserRealTimeDeliveryFieldRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/UpdateDcdnUserRealTimeDeliveryFieldRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,22 +27,17 @@
 		self.set_method('GET')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_BusinessType(self): # String
-		return self.get_query_params().get('BusinessType')
-
-	def set_BusinessType(self, BusinessType):  # String
-		self.add_query_param('BusinessType', BusinessType)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
 	def get_Fields(self): # String
 		return self.get_query_params().get('Fields')
 
 	def set_Fields(self, Fields):  # String
 		self.add_query_param('Fields', Fields)
+	def get_BusinessType(self): # String
+		return self.get_query_params().get('BusinessType')
+
+	def set_BusinessType(self, BusinessType):  # String
+		self.add_query_param('BusinessType', BusinessType)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/UploadRoutineCodeRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/DescribeDcdnRealTimeDeliveryFieldRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,33 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class UploadRoutineCodeRequest(RpcRequest):
+class DescribeDcdnRealTimeDeliveryFieldRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'UploadRoutineCode')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'DescribeDcdnRealTimeDeliveryField')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_CodeDescription(self): # String
-		return self.get_body_params().get('CodeDescription')
+	def get_BusinessType(self): # String
+		return self.get_query_params().get('BusinessType')
 
-	def set_CodeDescription(self, CodeDescription):  # String
-		self.add_body_params('CodeDescription', CodeDescription)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_Name(self): # String
-		return self.get_body_params().get('Name')
-
-	def set_Name(self, Name):  # String
-		self.add_body_params('Name', Name)
+	def set_BusinessType(self, BusinessType):  # String
+		self.add_query_param('BusinessType', BusinessType)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/aliyunsdkdcdn/request/v20180115/VerifyDcdnDomainOwnerRequest.py` & `aliyun-python-sdk-dcdn-2.2.9/aliyunsdkdcdn/request/v20180115/RollbackDcdnStagingConfigRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,33 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdcdn.endpoint import endpoint_data
 
-class VerifyDcdnDomainOwnerRequest(RpcRequest):
+class RollbackDcdnStagingConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'VerifyDcdnDomainOwner')
+		RpcRequest.__init__(self, 'dcdn', '2018-01-15', 'RollbackDcdnStagingConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_VerifyType(self): # String
-		return self.get_query_params().get('VerifyType')
-
-	def set_VerifyType(self, VerifyType):  # String
-		self.add_query_param('VerifyType', VerifyType)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-dcdn-2.2.8/setup.py` & `aliyun-python-sdk-dcdn-2.2.9/setup.py`

 * *Files identical despite different names*

