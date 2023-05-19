# Comparing `tmp/aliyun-python-sdk-cdn-3.8.7.tar.gz` & `tmp/aliyun-python-sdk-cdn-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cdn-3.8.7.tar", last modified: Thu May  4 07:50:48 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cdn-3.8.8.tar", last modified: Fri May 19 01:25:25 2023, max compression
```

## Comparing `aliyun-python-sdk-cdn-3.8.7.tar` & `aliyun-python-sdk-cdn-3.8.8.tar`

### file list

```diff
@@ -1,174 +1,172 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10594 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/
--rw-r--r--   0 root         (0) root         (0)     3573 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2767 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2414 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1459 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainSSLCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3087 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-04 07:50:48.000000 aliyun-python-sdk-cdn-3.8.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10456 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainSSLCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-19 01:25:25.000000 aliyun-python-sdk-cdn-3.8.8/setup.py
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/LICENSE` & `aliyun-python-sdk-cdn-3.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/PKG-INFO` & `aliyun-python-sdk-cdn-3.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cdn
-Version: 3.8.7
+Version: 3.8.8
 Summary: The cdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cdn
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/README.rst` & `aliyun-python-sdk-cdn-3.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/PKG-INFO` & `aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cdn
-Version: 3.8.7
+Version: 3.8.8
 Summary: The cdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cdn
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyun_python_sdk_cdn.egg-info/SOURCES.txt` & `aliyun-python-sdk-cdn-3.8.8/aliyun_python_sdk_cdn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py
 aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py
 aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py
 aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py
 aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py
 aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py
 aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py
-aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py
 aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py
 aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py
 aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py
 aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py
 aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py
 aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py
 aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py
@@ -110,15 +109,14 @@
 aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py
 aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py
 aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py
 aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py
 aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py
 aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py
 aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py
-aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py
 aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py
 aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py
 aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py
 aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py
 aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py
 aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py
 aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/endpoint.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class CreateIllegalUrlExportTaskRequest(RpcRequest):
+class DescribeCdnDomainByCertificateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'CreateIllegalUrlExportTask')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnDomainByCertificate')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_TaskName(self): # String
-		return self.get_query_params().get('TaskName')
+	def get_SSLPub(self): # String
+		return self.get_query_params().get('SSLPub')
 
-	def set_TaskName(self, TaskName):  # String
-		self.add_query_param('TaskName', TaskName)
-	def get_TimePoint(self): # String
-		return self.get_query_params().get('TimePoint')
+	def set_SSLPub(self, SSLPub):  # String
+		self.add_query_param('SSLPub', SSLPub)
+	def get_SSLStatus(self): # Boolean
+		return self.get_query_params().get('SSLStatus')
 
-	def set_TimePoint(self, TimePoint):  # String
-		self.add_query_param('TimePoint', TimePoint)
+	def set_SSLStatus(self, SSLStatus):  # Boolean
+		self.add_query_param('SSLStatus', SSLStatus)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeCdnDomainByCertificateRequest(RpcRequest):
+class DescribeCdnServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnDomainByCertificate')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnService')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SSLPub(self): # String
-		return self.get_query_params().get('SSLPub')
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
 
-	def set_SSLPub(self, SSLPub):  # String
-		self.add_query_param('SSLPub', SSLPub)
-	def get_SSLStatus(self): # Boolean
-		return self.get_query_params().get('SSLStatus')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
 
-	def set_SSLStatus(self, SSLStatus):  # Boolean
-		self.add_query_param('SSLStatus', SSLStatus)
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeCdnServiceRequest(RpcRequest):
+class DescribeCdnUserQuotaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnService')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnUserQuota')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeCdnUserQuotaRequest(RpcRequest):
+class DescribeCdnUserResourcePackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnUserQuota')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnUserResourcePackage')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
+
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def get_Status(self): # String
+		return self.get_query_params().get('Status')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
+	def set_Status(self, Status):  # String
+		self.add_query_param('Status', Status)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeCdnUserResourcePackageRequest(RpcRequest):
+class DescribeDomainRealTimeSrcTrafficDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeCdnUserResourcePackage')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainRealTimeSrcTrafficData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_Status(self): # String
-		return self.get_query_params().get('Status')
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
 
-	def set_Status(self, Status):  # String
-		self.add_query_param('Status', Status)
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeDomainRealTimeSrcTrafficDataRequest(RpcRequest):
+class DescribeDomainSrcTopUrlVisitRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainRealTimeSrcTrafficData')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainSrcTopUrlVisit')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,17 @@
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
+	def get_SortBy(self): # String
+		return self.get_query_params().get('SortBy')
+
+	def set_SortBy(self, SortBy):  # String
+		self.add_query_param('SortBy', SortBy)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeDomainSrcTopUrlVisitRequest(RpcRequest):
+class DescribeDomainSrcTrafficDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainSrcTopUrlVisit')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainSrcTrafficData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,17 +37,17 @@
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_SortBy(self): # String
-		return self.get_query_params().get('SortBy')
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
 
-	def set_SortBy(self, SortBy):  # String
-		self.add_query_param('SortBy', SortBy)
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeDomainSrcTrafficDataRequest(RpcRequest):
+class DescribeDomainsUsageByDayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainSrcTrafficData')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainsUsageByDay')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,17 +37,12 @@
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_Interval(self): # String
-		return self.get_query_params().get('Interval')
-
-	def set_Interval(self, Interval):  # String
-		self.add_query_param('Interval', Interval)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeDomainsUsageByDayRequest(RpcRequest):
+class DescribeEsExceptionDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeDomainsUsageByDay')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeEsExceptionData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
-
-	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
+	def get_RuleId(self): # String
+		return self.get_query_params().get('RuleId')
+
+	def set_RuleId(self, RuleId):  # String
+		self.add_query_param('RuleId', RuleId)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeEsExceptionDataRequest(RpcRequest):
+class DescribeEsExecuteDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeEsExceptionData')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeEsExecuteData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeEsExecuteDataRequest(RpcRequest):
+class DescribeRealtimeDeliveryAccRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeEsExecuteData')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeRealtimeDeliveryAcc')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
+	def get_Project(self): # String
+		return self.get_query_params().get('Project')
+
+	def set_Project(self, Project):  # String
+		self.add_query_param('Project', Project)
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
+
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_RuleId(self): # String
-		return self.get_query_params().get('RuleId')
+	def get_LogStore(self): # String
+		return self.get_query_params().get('LogStore')
 
-	def set_RuleId(self, RuleId):  # String
-		self.add_query_param('RuleId', RuleId)
+	def set_LogStore(self, LogStore):  # String
+		self.add_query_param('LogStore', LogStore)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeIllegalUrlExportTaskRequest(RpcRequest):
+class DescribeIpStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeIllegalUrlExportTask')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeIpStatus')
+		self.set_method('GET')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_TaskId(self): # String
-		return self.get_query_params().get('TaskId')
+	def get_Ips(self): # String
+		return self.get_query_params().get('Ips')
 
-	def set_TaskId(self, TaskId):  # String
-		self.add_query_param('TaskId', TaskId)
+	def set_Ips(self, Ips):  # String
+		self.add_query_param('Ips', Ips)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeIpStatusRequest(RpcRequest):
+class DescribeRefreshTaskByIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeIpStatus')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeRefreshTaskById')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Ips(self): # String
-		return self.get_query_params().get('Ips')
+	def get_TaskId(self): # String
+		return self.get_query_params().get('TaskId')
 
-	def set_Ips(self, Ips):  # String
-		self.add_query_param('Ips', Ips)
+	def set_TaskId(self, TaskId):  # String
+		self.add_query_param('TaskId', TaskId)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,43 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeRealtimeDeliveryAccRequest(RpcRequest):
+class SetWaitingRoomConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeRealtimeDeliveryAcc')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'SetWaitingRoomConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
+	def get_MaxTimeWait(self): # Integer
+		return self.get_query_params().get('MaxTimeWait')
 
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_Project(self): # String
-		return self.get_query_params().get('Project')
-
-	def set_Project(self, Project):  # String
-		self.add_query_param('Project', Project)
-	def get_Interval(self): # String
-		return self.get_query_params().get('Interval')
-
-	def set_Interval(self, Interval):  # String
-		self.add_query_param('Interval', Interval)
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_LogStore(self): # String
-		return self.get_query_params().get('LogStore')
+	def set_MaxTimeWait(self, MaxTimeWait):  # Integer
+		self.add_query_param('MaxTimeWait', MaxTimeWait)
+	def get_WaitUrl(self): # String
+		return self.get_query_params().get('WaitUrl')
+
+	def set_WaitUrl(self, WaitUrl):  # String
+		self.add_query_param('WaitUrl', WaitUrl)
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
+
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
+	def get_AllowPct(self): # Integer
+		return self.get_query_params().get('AllowPct')
+
+	def set_AllowPct(self, AllowPct):  # Integer
+		self.add_query_param('AllowPct', AllowPct)
+	def get_GapTime(self): # Integer
+		return self.get_query_params().get('GapTime')
+
+	def set_GapTime(self, GapTime):  # Integer
+		self.add_query_param('GapTime', GapTime)
+	def get_WaitUri(self): # String
+		return self.get_query_params().get('WaitUri')
 
-	def set_LogStore(self, LogStore):  # String
-		self.add_query_param('LogStore', LogStore)
+	def set_WaitUri(self, WaitUri):  # String
+		self.add_query_param('WaitUri', WaitUri)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class DescribeRefreshTaskByIdRequest(RpcRequest):
+class RollbackStagingConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'DescribeRefreshTaskById')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'RollbackStagingConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_TaskId(self): # String
-		return self.get_query_params().get('TaskId')
+	def get_DomainName(self): # String
+		return self.get_query_params().get('DomainName')
 
-	def set_TaskId(self, TaskId):  # String
-		self.add_query_param('TaskId', TaskId)
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class RollbackStagingConfigRequest(RpcRequest):
+class SetCdnDomainCSRCertificateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'RollbackStagingConfig')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'SetCdnDomainCSRCertificate')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ServerCertificate(self): # String
+		return self.get_query_params().get('ServerCertificate')
+
+	def set_ServerCertificate(self, ServerCertificate):  # String
+		self.add_query_param('ServerCertificate', ServerCertificate)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class SetCdnDomainCSRCertificateRequest(RpcRequest):
+class StartCdnDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'SetCdnDomainCSRCertificate')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'StartCdnDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ServerCertificate(self): # String
-		return self.get_query_params().get('ServerCertificate')
+	def get_SecurityToken(self): # String
+		return self.get_query_params().get('SecurityToken')
 
-	def set_ServerCertificate(self, ServerCertificate):  # String
-		self.add_query_param('ServerCertificate', ServerCertificate)
+	def set_SecurityToken(self, SecurityToken):  # String
+		self.add_query_param('SecurityToken', SecurityToken)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainSSLCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainSSLCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class SetWaitingRoomConfigRequest(RpcRequest):
+class UpdateCdnDeliverTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'SetWaitingRoomConfig')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'UpdateCdnDeliverTask')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_MaxTimeWait(self): # Integer
-		return self.get_query_params().get('MaxTimeWait')
+	def get_Reports(self): # String
+		return self.get_body_params().get('Reports')
 
-	def set_MaxTimeWait(self, MaxTimeWait):  # Integer
-		self.add_query_param('MaxTimeWait', MaxTimeWait)
-	def get_WaitUrl(self): # String
-		return self.get_query_params().get('WaitUrl')
+	def set_Reports(self, Reports):  # String
+		self.add_body_params('Reports', Reports)
+	def get_Schedule(self): # String
+		return self.get_body_params().get('Schedule')
+
+	def set_Schedule(self, Schedule):  # String
+		self.add_body_params('Schedule', Schedule)
+	def get_Name(self): # String
+		return self.get_body_params().get('Name')
 
-	def set_WaitUrl(self, WaitUrl):  # String
-		self.add_query_param('WaitUrl', WaitUrl)
+	def set_Name(self, Name):  # String
+		self.add_body_params('Name', Name)
 	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
+		return self.get_body_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
-	def get_AllowPct(self): # Integer
-		return self.get_query_params().get('AllowPct')
-
-	def set_AllowPct(self, AllowPct):  # Integer
-		self.add_query_param('AllowPct', AllowPct)
-	def get_GapTime(self): # Integer
-		return self.get_query_params().get('GapTime')
-
-	def set_GapTime(self, GapTime):  # Integer
-		self.add_query_param('GapTime', GapTime)
-	def get_WaitUri(self): # String
-		return self.get_query_params().get('WaitUri')
+		self.add_body_params('DomainName', DomainName)
+	def get_Deliver(self): # String
+		return self.get_body_params().get('Deliver')
+
+	def set_Deliver(self, Deliver):  # String
+		self.add_body_params('Deliver', Deliver)
+	def get_DeliverId(self): # Long
+		return self.get_body_params().get('DeliverId')
 
-	def set_WaitUri(self, WaitUri):  # String
-		self.add_query_param('WaitUri', WaitUri)
+	def set_DeliverId(self, DeliverId):  # Long
+		self.add_body_params('DeliverId', DeliverId)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class StartCdnDomainRequest(RpcRequest):
+class StopCdnDomainRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'StartCdnDomain')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'StopCdnDomain')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,33 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class StopCdnDomainRequest(RpcRequest):
+class UpdateFCTriggerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'StopCdnDomain')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'UpdateFCTrigger')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SecurityToken(self): # String
-		return self.get_query_params().get('SecurityToken')
+	def get_TriggerARN(self): # String
+		return self.get_query_params().get('TriggerARN')
 
-	def set_SecurityToken(self, SecurityToken):  # String
-		self.add_query_param('SecurityToken', SecurityToken)
-	def get_DomainName(self): # String
-		return self.get_query_params().get('DomainName')
-
-	def set_DomainName(self, DomainName):  # String
-		self.add_query_param('DomainName', DomainName)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def set_TriggerARN(self, TriggerARN):  # String
+		self.add_query_param('TriggerARN', TriggerARN)
+	def get_Notes(self): # String
+		return self.get_body_params().get('Notes')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
+	def set_Notes(self, Notes):  # String
+		self.add_body_params('Notes', Notes)
+	def get_SourceARN(self): # String
+		return self.get_body_params().get('SourceARN')
+
+	def set_SourceARN(self, SourceARN):  # String
+		self.add_body_params('SourceARN', SourceARN)
+	def get_RoleARN(self): # String
+		return self.get_body_params().get('RoleARN')
+
+	def set_RoleARN(self, RoleARN):  # String
+		self.add_body_params('RoleARN', RoleARN)
+	def get_FunctionARN(self): # String
+		return self.get_body_params().get('FunctionARN')
+
+	def set_FunctionARN(self, FunctionARN):  # String
+		self.add_body_params('FunctionARN', FunctionARN)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,48 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcdn.endpoint import endpoint_data
 
-class UpdateCdnDeliverTaskRequest(RpcRequest):
+class UpdateCdnSubTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'UpdateCdnDeliverTask')
+		RpcRequest.__init__(self, 'Cdn', '2018-05-10', 'UpdateCdnSubTask')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Reports(self): # String
-		return self.get_body_params().get('Reports')
+	def get_ReportIds(self): # String
+		return self.get_body_params().get('ReportIds')
 
-	def set_Reports(self, Reports):  # String
-		self.add_body_params('Reports', Reports)
-	def get_Schedule(self): # String
-		return self.get_body_params().get('Schedule')
-
-	def set_Schedule(self, Schedule):  # String
-		self.add_body_params('Schedule', Schedule)
-	def get_Name(self): # String
-		return self.get_body_params().get('Name')
-
-	def set_Name(self, Name):  # String
-		self.add_body_params('Name', Name)
+	def set_ReportIds(self, ReportIds):  # String
+		self.add_body_params('ReportIds', ReportIds)
 	def get_DomainName(self): # String
 		return self.get_body_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_body_params('DomainName', DomainName)
-	def get_Deliver(self): # String
-		return self.get_body_params().get('Deliver')
+	def get_EndTime(self): # String
+		return self.get_body_params().get('EndTime')
 
-	def set_Deliver(self, Deliver):  # String
-		self.add_body_params('Deliver', Deliver)
-	def get_DeliverId(self): # Long
-		return self.get_body_params().get('DeliverId')
+	def set_EndTime(self, EndTime):  # String
+		self.add_body_params('EndTime', EndTime)
+	def get_StartTime(self): # String
+		return self.get_body_params().get('StartTime')
 
-	def set_DeliverId(self, DeliverId):  # Long
-		self.add_body_params('DeliverId', DeliverId)
+	def set_StartTime(self, StartTime):  # String
+		self.add_body_params('StartTime', StartTime)
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py` & `aliyun-python-sdk-cdn-3.8.8/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_GlobalResourcePlan(self): # String
+		return self.get_query_params().get('GlobalResourcePlan')
+
+	def set_GlobalResourcePlan(self, GlobalResourcePlan):  # String
+		self.add_query_param('GlobalResourcePlan', GlobalResourcePlan)
 	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
 	def set_DomainName(self, DomainName):  # String
 		self.add_query_param('DomainName', DomainName)
 	def get_VerifyType(self): # String
 		return self.get_query_params().get('VerifyType')
```

### Comparing `aliyun-python-sdk-cdn-3.8.7/setup.py` & `aliyun-python-sdk-cdn-3.8.8/setup.py`

 * *Files identical despite different names*

