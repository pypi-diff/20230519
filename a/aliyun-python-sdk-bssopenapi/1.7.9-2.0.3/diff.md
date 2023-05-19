# Comparing `tmp/aliyun-python-sdk-bssopenapi-1.7.9.tar.gz` & `tmp/aliyun-python-sdk-bssopenapi-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-bssopenapi-1.7.9.tar", last modified: Mon Mar 28 03:30:47 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-bssopenapi-2.0.3.tar", last modified: Tue Nov 23 05:50:08 2021, max compression
```

## Comparing `aliyun-python-sdk-bssopenapi-1.7.9.tar` & `aliyun-python-sdk-bssopenapi-2.0.3.tar`

### file list

```diff
@@ -1,110 +1,107 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/
--rw-r--r--   0 root         (0) root         (0)      575 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1572 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6691 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/
--rw-r--r--   0 root         (0) root         (0)     2819 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/AddAccountRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3142 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/AllocateCostUnitResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3320 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ApplyInvoiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1614 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CancelOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2744 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ChangeResellerConsumeAmountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2749 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ConfirmRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2434 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ConvertChargeTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3034 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateAgAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2030 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateCostUnitRequest.py
--rw-r--r--   0 root         (0) root         (0)     3515 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1990 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateResellerUserQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2657 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3170 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateSavingsPlansInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1616 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DeleteCostUnitRequest.py
--rw-r--r--   0 root         (0) root         (0)     3879 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeInstanceBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribePricingModuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2657 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2277 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageTotalRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourcePackageProductRequest.py
--rw-r--r--   0 root         (0) root         (0)     2651 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2271 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageTotalRequest.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageTotalRequest.py
--rw-r--r--   0 root         (0) root         (0)     2432 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageTotalRequest.py
--rw-r--r--   0 root         (0) root         (0)     4238 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSplitItemBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/EnableBillGenerationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetAccountRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1463 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetCustomerAccountInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1280 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetCustomerListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1620 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetOrderDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2930 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetPayAsYouGoPriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3037 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetResourcePackagePriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4141 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetSubscriptionPriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2084 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/InquiryPriceRefundInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3245 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyAccountRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2021 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyCostUnitRequest.py
--rw-r--r--   0 root         (0) root         (0)     3135 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1288 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountBalanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3023 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     3241 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2747 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3827 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAvailableInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2301 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillOverviewRequest.py
--rw-r--r--   0 root         (0) root         (0)     3459 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     1302 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillToOSSSubscriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1929 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCashCouponsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitRequest.py
--rw-r--r--   0 root         (0) root         (0)     1986 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1467 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCustomerAddressListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3230 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryDPUtilizationDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3986 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryEvaluateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1463 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryFinancialAccountInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     3660 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2178 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceByTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     2472 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceGaapCostRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInvoicingCustomerListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2661 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyInstanceConsumptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3242 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryOrdersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryPermissionListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1931 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryPrepaidCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryProductListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2878 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRIUtilizationDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2274 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRedeemRequest.py
--rw-r--r--   0 root         (0) root         (0)     2073 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRelationListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryResellerAvailableQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2677 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryResourcePackageInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansDeductLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2791 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3672 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySettleBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     3379 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySettlementBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2828 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySplitItemBillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2497 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryUserOmsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2299 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RefundInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2261 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RelieveAccountRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2426 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RenewInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2243 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RenewResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3077 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SaveUserCreditRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetAllExpirationDayRequest.py
--rw-r--r--   0 root         (0) root         (0)     4804 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetCreditLabelActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2910 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetRenewalRequest.py
--rw-r--r--   0 root         (0) root         (0)     1883 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserAlarmThresholdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2423 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SubscribeBillToOSSRequest.py
--rw-r--r--   0 root         (0) root         (0)     2166 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/UnsubscribeBillToOSSRequest.py
--rw-r--r--   0 root         (0) root         (0)     2144 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/UpgradeResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2487 2022-03-28 03:30:47.000000 aliyun-python-sdk-bssopenapi-1.7.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1572 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6486 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/
+-rw-r--r--   0 root         (0) root         (0)     2819 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/AddAccountRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/AllocateCostUnitResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ApplyInvoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CancelOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ChangeResellerConsumeAmountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ConfirmRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ConvertChargeTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateAgAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateCostUnitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateResellerUserQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateSavingsPlansInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DeleteCostUnitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeInstanceBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribePricingModuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageTotalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourcePackageProductRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageTotalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageTotalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageTotalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSplitItemBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/EnableBillGenerationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetCustomerAccountInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetCustomerListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetOrderDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetPayAsYouGoPriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetResourcePackagePriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4141 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetSubscriptionPriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyAccountRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyCostUnitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountBalanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAvailableInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillOverviewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillToOSSSubscriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCashCouponsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCustomerAddressListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3230 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryDPUtilizationDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryEvaluateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryFinancialAccountInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceByTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceGaapCostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInvoicingCustomerListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyInstanceConsumptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryPermissionListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryPrepaidCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryProductListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRIUtilizationDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRedeemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRelationListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryResellerAvailableQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryResourcePackageInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansDeductLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySettleBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySettlementBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySplitItemBillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryUserOmsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RelieveAccountRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RenewInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RenewResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SaveUserCreditRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetAllExpirationDayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4804 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetCreditLabelActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetRenewalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserAlarmThresholdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SubscribeBillToOSSRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UnsubscribeBillToOSSRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UpgradeResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-23 05:50:08.000000 aliyun-python-sdk-bssopenapi-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2487 2021-11-23 05:50:07.000000 aliyun-python-sdk-bssopenapi-2.0.3/setup.py
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/LICENSE` & `aliyun-python-sdk-bssopenapi-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/PKG-INFO` & `aliyun-python-sdk-bssopenapi-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-bssopenapi
-Version: 1.7.9
+Version: 2.0.3
 Summary: The bssopenapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-bssopenapi
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/README.rst` & `aliyun-python-sdk-bssopenapi-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/PKG-INFO` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-bssopenapi
-Version: 1.7.9
+Version: 2.0.3
 Summary: The bssopenapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-bssopenapi
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyun_python_sdk_bssopenapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyun_python_sdk_bssopenapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,20 @@
 aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageTotalRequest.py
 aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageDetailRequest.py
 aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageTotalRequest.py
 aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageDetailRequest.py
 aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageTotalRequest.py
 aliyunsdkbssopenapi/request/v20171214/DescribeSplitItemBillRequest.py
 aliyunsdkbssopenapi/request/v20171214/EnableBillGenerationRequest.py
-aliyunsdkbssopenapi/request/v20171214/GetAccountRelationRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetCustomerAccountInfoRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetCustomerListRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetOrderDetailRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetPayAsYouGoPriceRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetResourcePackagePriceRequest.py
 aliyunsdkbssopenapi/request/v20171214/GetSubscriptionPriceRequest.py
-aliyunsdkbssopenapi/request/v20171214/InquiryPriceRefundInstanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/ModifyAccountRelationRequest.py
 aliyunsdkbssopenapi/request/v20171214/ModifyCostUnitRequest.py
 aliyunsdkbssopenapi/request/v20171214/ModifyInstanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/QueryAccountBalanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/QueryAccountBillRequest.py
 aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionDetailsRequest.py
 aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionsRequest.py
@@ -81,15 +79,14 @@
 aliyunsdkbssopenapi/request/v20171214/QueryResourcePackageInstancesRequest.py
 aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansDeductLogRequest.py
 aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansInstanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/QuerySettleBillRequest.py
 aliyunsdkbssopenapi/request/v20171214/QuerySettlementBillRequest.py
 aliyunsdkbssopenapi/request/v20171214/QuerySplitItemBillRequest.py
 aliyunsdkbssopenapi/request/v20171214/QueryUserOmsDataRequest.py
-aliyunsdkbssopenapi/request/v20171214/RefundInstanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/RelieveAccountRelationRequest.py
 aliyunsdkbssopenapi/request/v20171214/RenewInstanceRequest.py
 aliyunsdkbssopenapi/request/v20171214/RenewResourcePackageRequest.py
 aliyunsdkbssopenapi/request/v20171214/SaveUserCreditRequest.py
 aliyunsdkbssopenapi/request/v20171214/SetAllExpirationDayRequest.py
 aliyunsdkbssopenapi/request/v20171214/SetCreditLabelActionRequest.py
 aliyunsdkbssopenapi/request/v20171214/SetRenewalRequest.py
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/endpoint.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/AddAccountRelationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/AddAccountRelationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/AllocateCostUnitResourceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/AllocateCostUnitResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ApplyInvoiceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ApplyInvoiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CancelOrderRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CancelOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ChangeResellerConsumeAmountRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ChangeResellerConsumeAmountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ConfirmRelationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ConfirmRelationRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,12 +58,7 @@
 		self.add_query_param('RequestId', RequestId)
 	def get_PermissionCodess(self): # RepeatList
 		return self.get_query_params().get('PermissionCodes')
 
 	def set_PermissionCodess(self, PermissionCodes):  # RepeatList
 		for depth1 in range(len(PermissionCodes)):
 			self.add_query_param('PermissionCodes.' + str(depth1 + 1), PermissionCodes[depth1])
-	def get_RelationId(self): # Long
-		return self.get_query_params().get('RelationId')
-
-	def set_RelationId(self, RelationId):  # Long
-		self.add_query_param('RelationId', RelationId)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ConvertChargeTypeRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ConvertChargeTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateAgAccountRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateAgAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateCostUnitRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateCostUnitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateResellerUserQuotaRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateResellerUserQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateResourcePackageRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateResourcePackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/CreateSavingsPlansInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/CreateSavingsPlansInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DeleteCostUnitRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DeleteCostUnitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeInstanceBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeInstanceBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribePricingModuleRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribePricingModuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageTotalRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceCoverageTotalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourcePackageProductRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourcePackageProductRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageTotalRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeResourceUsageTotalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageTotalRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansCoverageTotalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageTotalRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSavingsPlansUsageTotalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/DescribeSplitItemBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/DescribeSplitItemBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/EnableBillGenerationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/EnableBillGenerationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetAccountRelationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryPermissionListRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,28 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class GetAccountRelationRequest(RpcRequest):
+class QueryPermissionListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'GetAccountRelation')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'QueryPermissionList')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_RequestId(self): # String
-		return self.get_query_params().get('RequestId')
-
-	def set_RequestId(self, RequestId):  # String
-		self.add_query_param('RequestId', RequestId)
 	def get_RelationId(self): # Long
 		return self.get_query_params().get('RelationId')
 
 	def set_RelationId(self, RelationId):  # Long
 		self.add_query_param('RelationId', RelationId)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetCustomerAccountInfoRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetCustomerAccountInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetCustomerListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetCustomerListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetOrderDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetOrderDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetPayAsYouGoPriceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetPayAsYouGoPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetResourcePackagePriceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetResourcePackagePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/GetSubscriptionPriceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/GetSubscriptionPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/InquiryPriceRefundInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RenewInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class InquiryPriceRefundInstanceRequest(RpcRequest):
+class RenewInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'InquiryPriceRefundInstance')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'RenewInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,17 +37,27 @@
 	def set_ProductCode(self, ProductCode):  # String
 		self.add_query_param('ProductCode', ProductCode)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
 	def get_ProductType(self): # String
 		return self.get_query_params().get('ProductType')
 
 	def set_ProductType(self, ProductType):  # String
 		self.add_query_param('ProductType', ProductType)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
+	def get_RenewPeriod(self): # Integer
+		return self.get_query_params().get('RenewPeriod')
+
+	def set_RenewPeriod(self, RenewPeriod):  # Integer
+		self.add_query_param('RenewPeriod', RenewPeriod)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyAccountRelationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyAccountRelationRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,40 +32,29 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ChildNick(self): # String
 		return self.get_query_params().get('ChildNick')
 
 	def set_ChildNick(self, ChildNick):  # String
 		self.add_query_param('ChildNick', ChildNick)
-	def get_ParentUserId(self): # Long
-		return self.get_query_params().get('ParentUserId')
-
-	def set_ParentUserId(self, ParentUserId):  # Long
-		self.add_query_param('ParentUserId', ParentUserId)
-	def get_RelationId(self): # Long
-		return self.get_query_params().get('RelationId')
-
-	def set_RelationId(self, RelationId):  # Long
-		self.add_query_param('RelationId', RelationId)
-	def get_RoleCodess(self): # RepeatList
-		return self.get_query_params().get('RoleCodes')
-
-	def set_RoleCodess(self, RoleCodes):  # RepeatList
-		for depth1 in range(len(RoleCodes)):
-			self.add_query_param('RoleCodes.' + str(depth1 + 1), RoleCodes[depth1])
 	def get_RelationOperation(self): # String
 		return self.get_query_params().get('RelationOperation')
 
 	def set_RelationOperation(self, RelationOperation):  # String
 		self.add_query_param('RelationOperation', RelationOperation)
 	def get_RelationType(self): # String
 		return self.get_query_params().get('RelationType')
 
 	def set_RelationType(self, RelationType):  # String
 		self.add_query_param('RelationType', RelationType)
+	def get_ParentUserId(self): # Long
+		return self.get_query_params().get('ParentUserId')
+
+	def set_ParentUserId(self, ParentUserId):  # Long
+		self.add_query_param('ParentUserId', ParentUserId)
 	def get_ChildUserId(self): # Long
 		return self.get_query_params().get('ChildUserId')
 
 	def set_ChildUserId(self, ChildUserId):  # Long
 		self.add_query_param('ChildUserId', ChildUserId)
 	def get_RequestId(self): # String
 		return self.get_query_params().get('RequestId')
@@ -74,7 +63,13 @@
 		self.add_query_param('RequestId', RequestId)
 	def get_PermissionCodess(self): # RepeatList
 		return self.get_query_params().get('PermissionCodes')
 
 	def set_PermissionCodess(self, PermissionCodes):  # RepeatList
 		for depth1 in range(len(PermissionCodes)):
 			self.add_query_param('PermissionCodes.' + str(depth1 + 1), PermissionCodes[depth1])
+	def get_RoleCodess(self): # RepeatList
+		return self.get_query_params().get('RoleCodes')
+
+	def set_RoleCodess(self, RoleCodes):  # RepeatList
+		for depth1 in range(len(RoleCodes)):
+			self.add_query_param('RoleCodes.' + str(depth1 + 1), RoleCodes[depth1])
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyCostUnitRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyCostUnitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/ModifyInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/ModifyInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountBalanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountBalanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionDetailsRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionDetailsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionsRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAccountTransactionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryAvailableInstancesRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryAvailableInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillOverviewRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillOverviewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryBillToOSSSubscriptionRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryBillToOSSSubscriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCashCouponsRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCashCouponsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitResourceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCostUnitResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryCustomerAddressListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryCustomerAddressListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryDPUtilizationDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryDPUtilizationDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryEvaluateListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryEvaluateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryFinancialAccountInfoRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryFinancialAccountInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceByTagRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceByTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInstanceGaapCostRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInstanceGaapCostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryInvoicingCustomerListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryInvoicingCustomerListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyInstanceConsumptionRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryMonthlyInstanceConsumptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryOrdersRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryOrdersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryPermissionListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetAllExpirationDayRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class QueryPermissionListRequest(RpcRequest):
+class SetAllExpirationDayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'QueryPermissionList')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetAllExpirationDay')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_RelationId(self): # Long
-		return self.get_query_params().get('RelationId')
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
 
-	def set_RelationId(self, RelationId):  # Long
-		self.add_query_param('RelationId', RelationId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_UnifyExpireDay(self): # String
+		return self.get_query_params().get('UnifyExpireDay')
+
+	def set_UnifyExpireDay(self, UnifyExpireDay):  # String
+		self.add_query_param('UnifyExpireDay', UnifyExpireDay)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryPrepaidCardsRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryPrepaidCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryProductListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryProductListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRIUtilizationDetailRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRIUtilizationDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRedeemRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRedeemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryRelationListRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryRelationListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryResellerAvailableQuotaRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryResellerAvailableQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryResourcePackageInstancesRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryResourcePackageInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansDeductLogRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansDeductLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySavingsPlansInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySettleBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySettleBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySettlementBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySettlementBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QuerySplitItemBillRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QuerySplitItemBillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/QueryUserOmsDataRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/QueryUserOmsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RefundInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserAlarmThresholdRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,43 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class RefundInstanceRequest(RpcRequest):
+class SetResellerUserAlarmThresholdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'RefundInstance')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserAlarmThreshold')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ProductCode(self): # String
-		return self.get_query_params().get('ProductCode')
+	def get_AlarmType(self): # String
+		return self.get_query_params().get('AlarmType')
 
-	def set_ProductCode(self, ProductCode):  # String
-		self.add_query_param('ProductCode', ProductCode)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
+	def set_AlarmType(self, AlarmType):  # String
+		self.add_query_param('AlarmType', AlarmType)
+	def get_AlarmThresholds(self): # String
+		return self.get_query_params().get('AlarmThresholds')
+
+	def set_AlarmThresholds(self, AlarmThresholds):  # String
+		self.add_query_param('AlarmThresholds', AlarmThresholds)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_ImmediatelyRelease(self): # String
-		return self.get_query_params().get('ImmediatelyRelease')
-
-	def set_ImmediatelyRelease(self, ImmediatelyRelease):  # String
-		self.add_query_param('ImmediatelyRelease', ImmediatelyRelease)
-	def get_ProductType(self): # String
-		return self.get_query_params().get('ProductType')
-
-	def set_ProductType(self, ProductType):  # String
-		self.add_query_param('ProductType', ProductType)
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
-
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RelieveAccountRelationRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RelieveAccountRelationRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,12 +47,7 @@
 	def set_ChildUserId(self, ChildUserId):  # Long
 		self.add_query_param('ChildUserId', ChildUserId)
 	def get_RequestId(self): # String
 		return self.get_query_params().get('RequestId')
 
 	def set_RequestId(self, RequestId):  # String
 		self.add_query_param('RequestId', RequestId)
-	def get_RelationId(self): # Long
-		return self.get_query_params().get('RelationId')
-
-	def set_RelationId(self, RelationId):  # Long
-		self.add_query_param('RelationId', RelationId)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RenewInstanceRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/RenewResourcePackageRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,48 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class RenewInstanceRequest(RpcRequest):
+class RenewResourcePackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'RenewInstance')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'RenewResourcePackage')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ProductCode(self): # String
-		return self.get_query_params().get('ProductCode')
-
-	def set_ProductCode(self, ProductCode):  # String
-		self.add_query_param('ProductCode', ProductCode)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_ProductType(self): # String
-		return self.get_query_params().get('ProductType')
+	def get_EffectiveDate(self): # String
+		return self.get_query_params().get('EffectiveDate')
+
+	def set_EffectiveDate(self, EffectiveDate):  # String
+		self.add_query_param('EffectiveDate', EffectiveDate)
+	def get_Duration(self): # Integer
+		return self.get_query_params().get('Duration')
 
-	def set_ProductType(self, ProductType):  # String
-		self.add_query_param('ProductType', ProductType)
+	def set_Duration(self, Duration):  # Integer
+		self.add_query_param('Duration', Duration)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_RenewPeriod(self): # Integer
-		return self.get_query_params().get('RenewPeriod')
+	def get_PricingCycle(self): # String
+		return self.get_query_params().get('PricingCycle')
 
-	def set_RenewPeriod(self, RenewPeriod):  # Integer
-		self.add_query_param('RenewPeriod', RenewPeriod)
+	def set_PricingCycle(self, PricingCycle):  # String
+		self.add_query_param('PricingCycle', PricingCycle)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/RenewResourcePackageRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UpgradeResourcePackageRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,43 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class RenewResourcePackageRequest(RpcRequest):
+class UpgradeResourcePackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'RenewResourcePackage')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'UpgradeResourcePackage')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Specification(self): # String
+		return self.get_query_params().get('Specification')
+
+	def set_Specification(self, Specification):  # String
+		self.add_query_param('Specification', Specification)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_EffectiveDate(self): # String
 		return self.get_query_params().get('EffectiveDate')
 
 	def set_EffectiveDate(self, EffectiveDate):  # String
 		self.add_query_param('EffectiveDate', EffectiveDate)
-	def get_Duration(self): # Integer
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self, Duration):  # Integer
-		self.add_query_param('Duration', Duration)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_PricingCycle(self): # String
-		return self.get_query_params().get('PricingCycle')
-
-	def set_PricingCycle(self, PricingCycle):  # String
-		self.add_query_param('PricingCycle', PricingCycle)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SaveUserCreditRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SaveUserCreditRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetAllExpirationDayRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserQuotaRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,28 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class SetAllExpirationDayRequest(RpcRequest):
+class SetResellerUserQuotaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetAllExpirationDay')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserQuota')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Amount(self): # String
+		return self.get_query_params().get('Amount')
+
+	def set_Amount(self, Amount):  # String
+		self.add_query_param('Amount', Amount)
+	def get_OutBizId(self): # String
+		return self.get_query_params().get('OutBizId')
+
+	def set_OutBizId(self, OutBizId):  # String
+		self.add_query_param('OutBizId', OutBizId)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_UnifyExpireDay(self): # String
-		return self.get_query_params().get('UnifyExpireDay')
+	def get_Currency(self): # String
+		return self.get_query_params().get('Currency')
 
-	def set_UnifyExpireDay(self, UnifyExpireDay):  # String
-		self.add_query_param('UnifyExpireDay', UnifyExpireDay)
+	def set_Currency(self, Currency):  # String
+		self.add_query_param('Currency', Currency)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetCreditLabelActionRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetCreditLabelActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetRenewalRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetRenewalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserAlarmThresholdRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SetResellerUserStatusRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class SetResellerUserAlarmThresholdRequest(RpcRequest):
+class SetResellerUserStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserAlarmThreshold')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AlarmType(self): # String
-		return self.get_query_params().get('AlarmType')
-
-	def set_AlarmType(self, AlarmType):  # String
-		self.add_query_param('AlarmType', AlarmType)
-	def get_AlarmThresholds(self): # String
-		return self.get_query_params().get('AlarmThresholds')
-
-	def set_AlarmThresholds(self, AlarmThresholds):  # String
-		self.add_query_param('AlarmThresholds', AlarmThresholds)
-	def get_OwnerId(self): # Long
+	def get_OwnerId(self): # String
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self, OwnerId):  # Long
+	def set_OwnerId(self, OwnerId):  # String
 		self.add_query_param('OwnerId', OwnerId)
+	def get_BusinessType(self): # String
+		return self.get_query_params().get('BusinessType')
+
+	def set_BusinessType(self, BusinessType):  # String
+		self.add_query_param('BusinessType', BusinessType)
+	def get_Status(self): # String
+		return self.get_query_params().get('Status')
+
+	def set_Status(self, Status):  # String
+		self.add_query_param('Status', Status)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserQuotaRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UntagResourcesRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,38 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class SetResellerUserQuotaRequest(RpcRequest):
+class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserQuota')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'UntagResources')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Amount(self): # String
-		return self.get_query_params().get('Amount')
+	def get_All(self): # Boolean
+		return self.get_query_params().get('All')
 
-	def set_Amount(self, Amount):  # String
-		self.add_query_param('Amount', Amount)
-	def get_OutBizId(self): # String
-		return self.get_query_params().get('OutBizId')
+	def set_All(self, All):  # Boolean
+		self.add_query_param('All', All)
+	def get_ResourceIds(self): # RepeatList
+		return self.get_query_params().get('ResourceId')
 
-	def set_OutBizId(self, OutBizId):  # String
-		self.add_query_param('OutBizId', OutBizId)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_TagKeys(self): # RepeatList
+		return self.get_query_params().get('TagKey')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_Currency(self): # String
-		return self.get_query_params().get('Currency')
+	def set_TagKeys(self, TagKey):  # RepeatList
+		for depth1 in range(len(TagKey)):
+			self.add_query_param('TagKey.' + str(depth1 + 1), TagKey[depth1])
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
 
-	def set_Currency(self, Currency):  # String
-		self.add_query_param('Currency', Currency)
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SetResellerUserStatusRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/UnsubscribeBillToOSSRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkbssopenapi.endpoint import endpoint_data
 
-class SetResellerUserStatusRequest(RpcRequest):
+class UnsubscribeBillToOSSRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'SetResellerUserStatus')
+		RpcRequest.__init__(self, 'BssOpenApi', '2017-12-14', 'UnsubscribeBillToOSS')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_OwnerId(self): # String
-		return self.get_query_params().get('OwnerId')
+	def get_SubscribeType(self): # String
+		return self.get_query_params().get('SubscribeType')
 
-	def set_OwnerId(self, OwnerId):  # String
-		self.add_query_param('OwnerId', OwnerId)
-	def get_BusinessType(self): # String
-		return self.get_query_params().get('BusinessType')
+	def set_SubscribeType(self, SubscribeType):  # String
+		self.add_query_param('SubscribeType', SubscribeType)
+	def get_MultAccountRelSubscribe(self): # String
+		return self.get_query_params().get('MultAccountRelSubscribe')
 
-	def set_BusinessType(self, BusinessType):  # String
-		self.add_query_param('BusinessType', BusinessType)
-	def get_Status(self): # String
-		return self.get_query_params().get('Status')
-
-	def set_Status(self, Status):  # String
-		self.add_query_param('Status', Status)
+	def set_MultAccountRelSubscribe(self, MultAccountRelSubscribe):  # String
+		self.add_query_param('MultAccountRelSubscribe', MultAccountRelSubscribe)
```

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/SubscribeBillToOSSRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/SubscribeBillToOSSRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/aliyunsdkbssopenapi/request/v20171214/TagResourcesRequest.py` & `aliyun-python-sdk-bssopenapi-2.0.3/aliyunsdkbssopenapi/request/v20171214/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bssopenapi-1.7.9/setup.py` & `aliyun-python-sdk-bssopenapi-2.0.3/setup.py`

 * *Files identical despite different names*

