# Comparing `tmp/coinlib-2.2.2.tar.gz` & `tmp/coinlib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coinlib-2.2.2.tar", last modified: Mon Apr 17 07:56:52 2023, max compression
+gzip compressed data, was "dist/coinlib-2.2.3.tar", last modified: Fri May 19 06:58:40 2023, max compression
```

## Comparing `coinlib-2.2.2.tar` & `coinlib-2.2.3.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.215870 coinlib-2.2.2/
--rw-r--r--   0 root         (0) root         (0)      642 2023-04-17 07:56:52.214870 coinlib-2.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.179867 coinlib-2.2.2/coinlib/
--rw-rw-rw-   0 root         (0) root         (0)    27933 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/BasicJob.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/BasicJobSessionStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9331 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsIndicatorJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibCrypto.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibDataInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibWorkspace.py
--rw-rw-rw-   0 root         (0) root         (0)    26721 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/DataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/InfluxDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/PluginLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     6388 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/PluginsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Registrar.py
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/WorkerJobProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     5812 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.184868 coinlib-2.2.2/coinlib/broker/
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/Broker.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/BrokerDTO.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerFuture.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerMargin.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerSpot.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibSessionManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.187868 coinlib-2.2.2/coinlib/brokerWorker/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     7841 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerSession.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerSessionWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/TestProtocolResult.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/coinlibFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.188868 coinlib-2.2.2/coinlib/data/
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/CollectionInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/DataTable.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    78656 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/dataWorker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   164353 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/dataWorker_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.190868 coinlib-2.2.2/coinlib/drawable/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/CoinlibDrawable.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/DrawableComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/WindowGrid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.191868 coinlib-2.2.2/coinlib/event/
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/EventConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/EventInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.194868 coinlib-2.2.2/coinlib/feature/
--rw-rw-rw-   0 root         (0) root         (0)    13862 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeature.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureFetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureLake.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureDTO.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9545 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/Features.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/helper.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/index.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.202869 coinlib-2.2.2/coinlib/logics/
--rw-rw-rw-   0 root         (0) root         (0)    13495 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/Logic.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicBasicWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicDTo.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicJob.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineJob.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerData.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerScreener.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerTrader.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineDataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineJob.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineScreenerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineTraderWorker.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8512 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicRegistrationInstance.py
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicTestBrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.203869 coinlib-2.2.2/coinlib/logics/broker/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/broker/LogicBrokerInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.204869 coinlib-2.2.2/coinlib/logics/manager/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/LogicJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/LogicManager.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/PortfolioModel.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.206869 coinlib-2.2.2/coinlib/logics/offlineManager/
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
--rw-rw-rw-   0 root         (0) root         (0)    11492 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.207870 coinlib-2.2.2/coinlib/logics/onlineManager/
--rw-rw-rw-   0 root         (0) root         (0)     6706 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/onlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.208870 coinlib-2.2.2/coinlib/notification/
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/Notification.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/NotificationFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/NotificationWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.211870 coinlib-2.2.2/coinlib/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticMethodJob.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticRuleJob.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/Statistics.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsMethodFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsMethodWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsRuleFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsRuleWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.213870 coinlib-2.2.2/coinlib/symbols/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/SymbolFactory.py
--rw-rw-rw-   0 root         (0) root         (0)    14991 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/SymbolWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/Symbols.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.181867 coinlib-2.2.2/coinlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 07:56:52.215870 coinlib-2.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-17 07:56:35.000000 coinlib-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.214870 coinlib-2.2.2/test/
--rw-rw-rw-   0 root         (0) root         (0)     4048 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testchartworker.py
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testcross.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.357585 coinlib-2.2.3/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-19 06:58:40.356585 coinlib-2.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.336585 coinlib-2.2.3/coinlib/
+-rw-rw-rw-   0 root         (0) root         (0)    27933 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/BasicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/BasicJobSessionStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9436 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsIndicatorJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/ChartsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibCrypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibDataInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/CoinlibWorkspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    26721 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/DataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/InfluxDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/PluginLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/PluginsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5960 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17647 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/Simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/WorkerJobProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.340585 coinlib-2.2.3/coinlib/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     7229 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/Broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/BrokerDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerFuture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerMargin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibBrokerSpot.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/CoinlibSessionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.341585 coinlib-2.2.3/coinlib/brokerWorker/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7841 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerSession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerSessionWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/BrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/TestProtocolResult.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/brokerWorker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/coinlibFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.342585 coinlib-2.2.3/coinlib/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/CollectionInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/DataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    78656 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/dataWorker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   164353 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/dataWorker_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.343585 coinlib-2.2.3/coinlib/drawable/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/CoinlibDrawable.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/DrawableComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/WindowGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/drawable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.343585 coinlib-2.2.3/coinlib/event/
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/EventConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/EventInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.345585 coinlib-2.2.3/coinlib/feature/
+-rw-rw-rw-   0 root         (0) root         (0)    14475 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureFetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureLake.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/CoinlibFeatureProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9545 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/FeatureWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/Features.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/feature/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.350585 coinlib-2.2.3/coinlib/logics/
+-rw-rw-rw-   0 root         (0) root         (0)    13495 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/Logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicBasicWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicDTo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerData.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerScreener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerTrader.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineDataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineScreenerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineTraderWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14919 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOnlineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8512 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicRegistrationInstance.py
+-rw-rw-rw-   0 root         (0) root         (0)    16758 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/LogicTestBrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.350585 coinlib-2.2.3/coinlib/logics/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/broker/LogicBrokerInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.351585 coinlib-2.2.3/coinlib/logics/manager/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/LogicJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/LogicManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/PortfolioModel.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.352585 coinlib-2.2.3/coinlib/logics/offlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11492 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/offlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.352585 coinlib-2.2.3/coinlib/logics/onlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)     6706 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/logics/onlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.353585 coinlib-2.2.3/coinlib/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/Notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/NotificationFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/NotificationWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.355585 coinlib-2.2.3/coinlib/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticMethodJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticRuleJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/Statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsMethodFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsMethodWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsRuleFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/StatisticsRuleWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/statistics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.356585 coinlib-2.2.3/coinlib/symbols/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/SymbolFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14991 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/SymbolWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/Symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 06:58:28.000000 coinlib-2.2.3/coinlib/symbols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.338585 coinlib-2.2.3/coinlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 06:58:40.000000 coinlib-2.2.3/coinlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 06:58:40.357585 coinlib-2.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-19 06:58:28.000000 coinlib-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:58:40.356585 coinlib-2.2.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4048 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testchartworker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testcross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-05-19 06:58:28.000000 coinlib-2.2.3/test/testplot.py
```

### Comparing `coinlib-2.2.2/PKG-INFO` & `coinlib-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.2
+Version: 2.2.3
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.2/coinlib/BasicJob.py` & `coinlib-2.2.3/coinlib/BasicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/BasicJobSessionStorage.py` & `coinlib-2.2.3/coinlib/BasicJobSessionStorage.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/ChartsIndicatorJob.py` & `coinlib-2.2.3/coinlib/ChartsIndicatorJob.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 additional["yValue"] = data
             elif chartType == "cloud":
 
                 self.table.setColumn(":top", data["top"])
                 self.table.setColumn(":middle", data["middle"])
                 self.table.setColumn(":bottom", data["bottom"])
                 column_names = [":top", ":middle", ":bottom"]
-            elif chartType == "marker":
+            elif chartType == "marker" or chartType == "cross":
                 # it is a numpy array
                 if isinstance(data, (pd.core.series.Series)):
                     self.table.setColumn(":marker", data.values, type=str)
                 else:
                     self.table.setColumn(":marker", data, type=str)
                 column_names = [":marker"]
 
@@ -214,14 +214,16 @@
             options["tooltip"] = tooltip
         if size is not None:
             options["size"] = size
         if fill is not None:
             options["fill"] = fill
         if fill_from is not None:
             options["fill_from"] = fill_from
+        if chartType == "cross":
+            options["chartTypeIcon"] = "\ue84a"
         if chartTypeIcon is not None:
             options["chartTypeIcon"] = chartTypeIcon
 
         options["additional"] = json.dumps(additional)
         options["connectGaps"] = connectGaps
         options["chartType"] = chartType
         options["chart"] = str(chart) if chart is not None else None
```

### Comparing `coinlib-2.2.2/coinlib/ChartsWorker.py` & `coinlib-2.2.3/coinlib/ChartsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/CoinlibCrypto.py` & `coinlib-2.2.3/coinlib/CoinlibCrypto.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/CoinlibDataInterface.py` & `coinlib-2.2.3/coinlib/CoinlibDataInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/CoinlibWorkspace.py` & `coinlib-2.2.3/coinlib/CoinlibWorkspace.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/DataWorker.py` & `coinlib-2.2.3/coinlib/DataWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/Functions.py` & `coinlib-2.2.3/coinlib/Functions.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/InfluxDatabase.py` & `coinlib-2.2.3/coinlib/InfluxDatabase.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/PluginLoader.py` & `coinlib-2.2.3/coinlib/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/PluginsWorker.py` & `coinlib-2.2.3/coinlib/PluginsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/Registrar.py` & `coinlib-2.2.3/coinlib/Registrar.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/Simulator.py` & `coinlib-2.2.3/coinlib/Simulator.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/WorkerJobProcess.py` & `coinlib-2.2.3/coinlib/WorkerJobProcess.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     original: any
     subfeature: str
     name: str
 
 class WorkerJobProcess:
     def __init__(self, workerJob, factory):
         self.workerChannel = None
+        self.finishedData = None
         if factory is not None:
             self.workerChannel = factory.createChannel()
         self.registrar = Registrar()
         self.chipmunkDb = None
         ##self.chipmunkDb = ChipmunkDb(self.registrar.chipmunkdb)
         if factory is not None:
             self.stub = stats.DataWorkerStub(self.workerChannel)
```

### Comparing `coinlib-2.2.2/coinlib/__init__.py` & `coinlib-2.2.3/coinlib/__init__.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/Broker.py` & `coinlib-2.2.3/coinlib/broker/Broker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/BrokerDTO.py` & `coinlib-2.2.3/coinlib/broker/BrokerDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/CoinlibBroker.py` & `coinlib-2.2.3/coinlib/broker/CoinlibBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/CoinlibBrokerFuture.py` & `coinlib-2.2.3/coinlib/broker/CoinlibBrokerFuture.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/CoinlibBrokerMargin.py` & `coinlib-2.2.3/coinlib/broker/CoinlibBrokerMargin.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/broker/CoinlibBrokerSpot.py` & `coinlib-2.2.3/coinlib/broker/CoinlibBrokerSpot.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/brokerWorker/BrokerSession.py` & `coinlib-2.2.3/coinlib/brokerWorker/BrokerSession.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/brokerWorker/BrokerSessionWorker.py` & `coinlib-2.2.3/coinlib/brokerWorker/BrokerSessionWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/brokerWorker/BrokerWorker.py` & `coinlib-2.2.3/coinlib/brokerWorker/BrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/brokerWorker/TestProtocolResult.py` & `coinlib-2.2.3/coinlib/brokerWorker/TestProtocolResult.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/coinlibFactory.py` & `coinlib-2.2.3/coinlib/coinlibFactory.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/config.py` & `coinlib-2.2.3/coinlib/config.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/data/CollectionInterface.py` & `coinlib-2.2.3/coinlib/data/CollectionInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/data/DataTable.py` & `coinlib-2.2.3/coinlib/data/DataTable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/dataWorker_pb2.py` & `coinlib-2.2.3/coinlib/dataWorker_pb2.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/dataWorker_pb2_grpc.py` & `coinlib-2.2.3/coinlib/dataWorker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/drawable/CoinlibDrawable.py` & `coinlib-2.2.3/coinlib/drawable/CoinlibDrawable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/drawable/WindowGrid.py` & `coinlib-2.2.3/coinlib/drawable/WindowGrid.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/event/EventConsumer.py` & `coinlib-2.2.3/coinlib/event/EventConsumer.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/event/EventInterface.py` & `coinlib-2.2.3/coinlib/event/EventInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/feature/CoinlibFeature.py` & `coinlib-2.2.3/coinlib/feature/CoinlibFeature.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,15 +140,16 @@
             stage = ""
 
         latest_data_with_symbol = {}
         df = pd.DataFrame()
         columns = []
         rows = {}
         for row in data:
-            fullindex = datetime.datetime.strftime(row["datetime"], "%Y-%m-%dT%H:%M:%S.%fZ")
+            datetime_as_str = datetime.datetime.strftime(row["datetime"], "%Y-%m-%dT%H:%M:%S.%fZ")
+            fullindex = datetime_as_str
 
             orig_key = row["identifier"]
             key = orig_key+stage
             full_identifier = row["identifier"]+stage
             if row["group"] is not None:
                 full_identifier = row["group"]+"."+full_identifier
                 key = row["group"]+"."+key
@@ -162,14 +163,16 @@
 
             d = {}
 
             if key not in columns:
                 columns.append({
                     "id": key,
                     "key": orig_key,
+                    "datetime": datetime_as_str,
+                    "value": row["value"],
                     "group": row["group"],
                     "stage": "dev" if self.registrar.isLiveEnvironment() else "live"
                 })
             if fullindex not in rows:
                 rows[fullindex] = {}
             latest_data_with_symbol[full_key] = {
                 "value": row["value"],
@@ -203,21 +206,26 @@
                 message_body = json.dumps({
                     "keys": columns, "data": data,
                     "transaction_id": 123,
                     "source": self.worker.getIdentifier() if self.worker else None
                 },
                     default=helper.serializeDTO)
 
-                url = self.registrar.coinlib_backend_host+"/api/v1/historicalfeatures/save/"+data_server_target
-
-                requests.post(url, data=message_body)
+                backend = self.registrar.coinlib_backend_host
+                if backend is None:
+                    backend = "http://"+self.registrar.workerEndpoint+":9001"
+                if backend is None:
+                    backend = 'http://localhost:9001'
+                url = backend+"/api/v1/historicalfeatures/save/"+data_server_target
 
+                requests.post(url, data=message_body, headers={'Content-type': 'application/json', 'Accept': 'text/plain'})
 
             except Exception as e:
-                    pass
+                print("Can not save data to "+databaseServer+" "+databaseId+" "+str(e))
+                pass
 
             self.save_statistics(columns, df2.shape[0])
         except Exception as e:
             print(e)
         return True
 
     def get_data(self, identifier=None, group=None, symbol=None, limit=10):
@@ -286,14 +294,17 @@
                 interval = self.defaultInterval
 
             if dt is None and self.transactions["default"]["datetime"] is None:
                 dt = CoinlibFeature.formatInterval(datetime.datetime.now(pytz.utc), interval)
                 self.transactions["default"]["datetime"] = dt
             elif dt is None:
                 dt = self.transactions["default"]["datetime"]
+            else:
+                dt = CoinlibFeature.formatInterval(dt, interval)
+
 
             self.transactions["default"]["data"].append({
                 "identifier": identifier,
                 "value": value,
                 "symbol": symbol,
                 "exchange": exchange,
                 "datetime": dt,
```

### Comparing `coinlib-2.2.2/coinlib/feature/CoinlibFeatureFetcher.py` & `coinlib-2.2.3/coinlib/feature/CoinlibFeatureFetcher.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/feature/CoinlibFeatureLake.py` & `coinlib-2.2.3/coinlib/feature/CoinlibFeatureLake.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/feature/FeatureDTO.py` & `coinlib-2.2.3/coinlib/feature/FeatureDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/feature/FeatureWorker.py` & `coinlib-2.2.3/coinlib/feature/FeatureWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/feature/Features.py` & `coinlib-2.2.3/coinlib/feature/Features.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         return grpc.insecure_channel(self.registrar.get_coinlib_backend_grpc(), options=grpc_chan_ops,
                                      compression=grpc.Compression.Gzip)
 
     def registerFeature(self, callbackClass: CoinlibFeature, featureIdentifier: str,
                        featureTitle: str,
                        type: FeatureModuleType = FeatureModuleType.processors,
                        description: str = "",
+                        timeout: int = 60*60,
                        estimatedDataInterval: int = 60*60,
                        options=None):
 
         registration = statsModel.FeatureRegistration()
         registration.identifier = featureIdentifier
         registration.name = featureTitle
         registration.estimatedDataInterval = estimatedDataInterval
```

### Comparing `coinlib-2.2.2/coinlib/helper.py` & `coinlib-2.2.3/coinlib/helper.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logger.py` & `coinlib-2.2.3/coinlib/logger.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/Logic.py` & `coinlib-2.2.3/coinlib/logics/Logic.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicBasicWorker.py` & `coinlib-2.2.3/coinlib/logics/LogicBasicWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicJob.py` & `coinlib-2.2.3/coinlib/logics/LogicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicLoader.py` & `coinlib-2.2.3/coinlib/logics/LogicLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicOfflineJob.py` & `coinlib-2.2.3/coinlib/logics/LogicOfflineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicOfflineWorker.py` & `coinlib-2.2.3/coinlib/logics/LogicOfflineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerTrader.py` & `coinlib-2.2.3/coinlib/logics/LogicOfflineWorkerTrader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicOnlineJob.py` & `coinlib-2.2.3/coinlib/logics/LogicOnlineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicOnlineWorker.py` & `coinlib-2.2.3/coinlib/logics/LogicOnlineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicRegistrationInstance.py` & `coinlib-2.2.3/coinlib/logics/LogicRegistrationInstance.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/LogicTestBrokerWorker.py` & `coinlib-2.2.3/coinlib/logics/LogicTestBrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/broker/LogicBrokerInterface.py` & `coinlib-2.2.3/coinlib/logics/broker/LogicBrokerInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/manager/LogicJobBroker.py` & `coinlib-2.2.3/coinlib/logics/manager/LogicJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/manager/LogicManager.py` & `coinlib-2.2.3/coinlib/logics/manager/LogicManager.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/manager/PortfolioModel.py` & `coinlib-2.2.3/coinlib/logics/manager/PortfolioModel.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py` & `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py` & `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py` & `coinlib-2.2.3/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/logics/onlineManager/LogicOnlineJobBroker.py` & `coinlib-2.2.3/coinlib/logics/onlineManager/LogicOnlineJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/notification/Notification.py` & `coinlib-2.2.3/coinlib/notification/Notification.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/notification/NotificationWorker.py` & `coinlib-2.2.3/coinlib/notification/NotificationWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/statistics/StatisticMethodJob.py` & `coinlib-2.2.3/coinlib/statistics/StatisticMethodJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/statistics/StatisticRuleJob.py` & `coinlib-2.2.3/coinlib/statistics/StatisticRuleJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/statistics/Statistics.py` & `coinlib-2.2.3/coinlib/statistics/Statistics.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/statistics/StatisticsMethodWorker.py` & `coinlib-2.2.3/coinlib/statistics/StatisticsMethodWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/statistics/StatisticsRuleWorker.py` & `coinlib-2.2.3/coinlib/statistics/StatisticsRuleWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/symbols/SymbolWorker.py` & `coinlib-2.2.3/coinlib/symbols/SymbolWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib/symbols/Symbols.py` & `coinlib-2.2.3/coinlib/symbols/Symbols.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/coinlib.egg-info/PKG-INFO` & `coinlib-2.2.3/coinlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.2
+Version: 2.2.3
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.2/coinlib.egg-info/SOURCES.txt` & `coinlib-2.2.3/coinlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/setup.py` & `coinlib-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="coinlib",
-    version="2.2.2",
+    version="2.2.3",
     description="Develop new code for your coindeck environment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/coinlib",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
```

### Comparing `coinlib-2.2.2/test/testchartworker.py` & `coinlib-2.2.3/test/testchartworker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/test/testcross.py` & `coinlib-2.2.3/test/testcross.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.2/test/testplot.py` & `coinlib-2.2.3/test/testplot.py`

 * *Files identical despite different names*

