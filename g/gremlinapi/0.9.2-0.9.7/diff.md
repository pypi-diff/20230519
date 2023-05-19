# Comparing `tmp/gremlinapi-0.9.2.tar.gz` & `tmp/gremlinapi-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gremlinapi-0.9.2.tar", last modified: Mon Mar  8 21:42:00 2021, max compression
+gzip compressed data, was "gremlinapi-0.9.7.tar", last modified: Tue Mar  9 20:40:31 2021, max compression
```

## Comparing `gremlinapi-0.9.2.tar` & `gremlinapi-0.9.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 21:42:00.261064 gremlinapi-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    22396 2021-03-08 21:42:00.261064 gremlinapi-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17697 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 21:42:00.257064 gremlinapi-0.9.2/gremlinapi/
--rw-r--r--   0 runner    (1001) docker     (121)     8990 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/alfi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/apikeys.py
--rw-r--r--   0 runner    (1001) docker     (121)    58067 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/attack_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/attacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     7441 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/companies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/contracts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/executions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5421 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/gremlinapi.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/halts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6488 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/http_clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/saml.py
--rw-r--r--   0 runner    (1001) docker     (121)    16595 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/scenario_graph_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6561 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/scenario_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11544 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (121)     8545 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/schedules.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)    14990 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/users.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/gremlinapi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 21:42:00.261064 gremlinapi-0.9.2/gremlinapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22396 2021-03-08 21:41:59.000000 gremlinapi-0.9.2/gremlinapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-03-08 21:42:00.000000 gremlinapi-0.9.2/gremlinapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-08 21:41:59.000000 gremlinapi-0.9.2/gremlinapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-08 21:41:59.000000 gremlinapi-0.9.2/gremlinapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-03-08 21:41:59.000000 gremlinapi-0.9.2/gremlinapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-08 21:41:59.000000 gremlinapi-0.9.2/gremlinapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-08 21:42:00.261064 gremlinapi-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-08 21:42:00.261064 gremlinapi-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/tests/test_gremlinapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-03-08 21:41:45.000000 gremlinapi-0.9.2/tests/test_httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 20:40:31.317862 gremlinapi-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)    22396 2021-03-09 20:40:31.317862 gremlinapi-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17697 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 20:40:31.313861 gremlinapi-0.9.7/gremlinapi/
+-rw-r--r--   0 runner    (1001) docker     (121)     9636 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/alfi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/apikeys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58339 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/attack_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5310 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/attacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7725 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/companies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/executions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5483 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/gremlinapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/halts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6846 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/http_clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3851 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/orgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4288 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/saml.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16887 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/scenario_graph_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6834 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/scenario_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12237 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8822 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15547 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/users.py
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/gremlinapi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 20:40:31.317862 gremlinapi-0.9.7/gremlinapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22396 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-09 20:40:31.000000 gremlinapi-0.9.7/gremlinapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-09 20:40:31.317862 gremlinapi-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-09 20:40:31.317862 gremlinapi-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/tests/test_gremlinapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-03-09 20:40:20.000000 gremlinapi-0.9.7/tests/test_httpclient.py
```

### Comparing `gremlinapi-0.9.2/PKG-INFO` & `gremlinapi-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinapi
-Version: 0.9.2
+Version: 0.9.7
 Summary: Gremlin library for Python
 Home-page: https://github.com/gremlin/gremlin-python/
 Author: Kyle Hultman
 Author-email: kyle@gremlin.com
 License: Apache 2.0
 Description: # gremlin-python
```

### Comparing `gremlinapi-0.9.2/README.md` & `gremlinapi-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `gremlinapi-0.9.2/gremlinapi/__init__.py` & `gremlinapi-0.9.7/gremlinapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,177 +8,252 @@
 import time
 
 from datetime import datetime, timezone
 
 from gremlinapi.alfi import GremlinALFI as alfi
 from gremlinapi.apikeys import GremlinAPIapikeys as apikeys
 from gremlinapi.attack_helpers import (
-    GremlinAttackHelper, GremlinAttackTargetHelper, GremlinTargetHosts, GremlinTargetContainers,
-    GremlinAttackCommandHelper, GremlinResourceAttackHelper, GremlinStateAttackHelper, GremlinNetworkAttackHelper,
-    GremlinCPUAttack, GremlinMemoryAttack, GremlinDiskSpaceAttack, GremlinDiskIOAttack,
-    GremlinShutdownAttack, GremlinProcessKillerAttack, GremlinTimeTravelAttack,
-    GremlinBlackholeAttack, GremlinDNSAttack, GremlinLatencyAttack, GremlinPacketLossAttack)
+    GremlinAttackHelper,
+    GremlinAttackTargetHelper,
+    GremlinTargetHosts,
+    GremlinTargetContainers,
+    GremlinAttackCommandHelper,
+    GremlinResourceAttackHelper,
+    GremlinStateAttackHelper,
+    GremlinNetworkAttackHelper,
+    GremlinCPUAttack,
+    GremlinMemoryAttack,
+    GremlinDiskSpaceAttack,
+    GremlinDiskIOAttack,
+    GremlinShutdownAttack,
+    GremlinProcessKillerAttack,
+    GremlinTimeTravelAttack,
+    GremlinBlackholeAttack,
+    GremlinDNSAttack,
+    GremlinLatencyAttack,
+    GremlinPacketLossAttack,
+)
 from gremlinapi.attacks import GremlinAPIAttacks as Attacks
 from gremlinapi.clients import GremlinAPIClients as Clients
 from gremlinapi.companies import GremlinAPICompanies as Companies
 from gremlinapi.config import GremlinAPIConfig
 from gremlinapi.containers import GremlinAPIContainers as Containers
 from gremlinapi.contracts import GremlinAPIContracts as Contracts
 from gremlinapi.exceptions import *
 from gremlinapi.executions import GremlinAPIExecutions as Executions
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.halts import GremlinAPIHalts as Halts
 from gremlinapi.http_clients import get_gremlin_httpclient
-from gremlinapi.kubernetes import (GremlinAPIKubernetesAttacks as KubernetesAttacks,
-                                   GremlinAPIKubernetesTargets as KubernetesTargets)
+from gremlinapi.kubernetes import (
+    GremlinAPIKubernetesAttacks as KubernetesAttacks,
+    GremlinAPIKubernetesTargets as KubernetesTargets,
+)
 from gremlinapi.metadata import GremlinAPIMetadata as Metadata
 from gremlinapi.metrics import GremlinAPIMetrics as Metrics
 from gremlinapi.orgs import GremlinAPIOrgs as Orgs
 from gremlinapi.providers import GremlinAPIProviders as Providers
-from gremlinapi.reports import GremlinAPIReports as Reports, GremlinAPIReportsSecurity as SecurityReports
+from gremlinapi.reports import (
+    GremlinAPIReports as Reports,
+    GremlinAPIReportsSecurity as SecurityReports,
+)
 from gremlinapi.saml import GremlinAPISaml
-from gremlinapi.scenario_helpers import (GremlinScenarioHelper, GremlinScenarioStep, GremlinILFIStep)
-from gremlinapi.scenario_graph_helpers import (GremlinScenarioGraphHelper, GremlinScenarioNode,
-                                               GremlinScenarioAttackNode, GremlinScenarioILFINode,
-                                               GremlinScenarioALFINode, GremlinScenarioDelayNode,
-                                               GremlinScenarioStatusCheckNode)
-from gremlinapi.scenarios import (GremlinAPIScenarios as Scenarios,
-                                  GremlinAPIScenariosRecommended as RecommendedScenarios)
+from gremlinapi.scenario_helpers import (
+    GremlinScenarioHelper,
+    GremlinScenarioStep,
+    GremlinILFIStep,
+)
+from gremlinapi.scenario_graph_helpers import (
+    GremlinScenarioGraphHelper,
+    GremlinScenarioNode,
+    GremlinScenarioAttackNode,
+    GremlinScenarioILFINode,
+    GremlinScenarioALFINode,
+    GremlinScenarioDelayNode,
+    GremlinScenarioStatusCheckNode,
+)
+from gremlinapi.scenarios import (
+    GremlinAPIScenarios as Scenarios,
+    GremlinAPIScenariosRecommended as RecommendedScenarios,
+)
 from gremlinapi.schedules import GremlinAPISchedules as Schedules
 from gremlinapi.templates import GremlinAPITemplates as Templates
-from gremlinapi.users import (GremlinAPIUsers as Users,
-                              GremlinAPIUsersAuth as userAuth,
-                              GremlinAPIUsersAuthMFA as userMFAuth)
+from gremlinapi.users import (
+    GremlinAPIUsers as Users,
+    GremlinAPIUsersAuth as userAuth,
+    GremlinAPIUsersAuthMFA as userMFAuth,
+)
 from gremlinapi.util import get_version
 
 
 __version__ = get_version()
 
 
 # Logging Configuration
 class SecretsFilter(logging.Filter):
     def filter(self, record):
         secret_length = 5
         if len(GremlinAPIConfig.api_key) >= secret_length:
-            record.msg = re.sub(rf"{GremlinAPIConfig.api_key}[\'\s]?",
-                                '...'+GremlinAPIConfig.api_key[-4:],
-                                record.msg)
+            record.msg = re.sub(
+                rf"{GremlinAPIConfig.api_key}[\'\s]?",
+                "..." + GremlinAPIConfig.api_key[-4:],
+                record.msg,
+            )
         if len(GremlinAPIConfig.bearer_token) >= secret_length:
-            record.msg = re.sub(rf"{GremlinAPIConfig.bearer_token}[\'\s]?",
-                                '...'+GremlinAPIConfig.bearer_token[-4:],
-                                record.msg)
+            record.msg = re.sub(
+                rf"{GremlinAPIConfig.bearer_token}[\'\s]?",
+                "..." + GremlinAPIConfig.bearer_token[-4:],
+                record.msg,
+            )
         if len(GremlinAPIConfig.password) >= secret_length:
-            record.msg = re.sub(rf"{GremlinAPIConfig.password}[\'\s]?",
-                                '[PASSWORD REDACTED]',
-                                record.msg)
+            record.msg = re.sub(
+                rf"{GremlinAPIConfig.password}[\'\s]?",
+                "[PASSWORD REDACTED]",
+                record.msg,
+            )
         return record
 
+
 logging_levels = {
-    'CRITICAL': logging.CRITICAL,
-    'ERROR': logging.ERROR,
-    'WARNING': logging.WARNING,
-    'INFO': logging.INFO,
-    'DEBUG': logging.DEBUG
+    "CRITICAL": logging.CRITICAL,
+    "ERROR": logging.ERROR,
+    "WARNING": logging.WARNING,
+    "INFO": logging.INFO,
+    "DEBUG": logging.DEBUG,
 }
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 log_handler = logging.StreamHandler()
-log_formatter = logging.Formatter('%(asctime)s %(name)-12s %(levelname)-8s %(message)s')
+log_formatter = logging.Formatter("%(asctime)s %(name)-12s %(levelname)-8s %(message)s")
 log_handler.setFormatter(log_formatter)
 log.addFilter(SecretsFilter())
 log.addHandler(log_handler)
-log.setLevel(logging_levels.get(os.getenv('GREMLIN_PYTHON_API_LOG_LEVEL', 'WARNING'), logging.WARNING))
+log.setLevel(
+    logging_levels.get(
+        os.getenv("GREMLIN_PYTHON_API_LOG_LEVEL", "WARNING"), logging.WARNING
+    )
+)
 
 # API Settings
-_api_host = 'https://api.gremlin.com'
-_api_version = 'v1'
+_api_host = "https://api.gremlin.com"
+_api_version = "v1"
 
-_api_key = os.getenv('GREMLIN_API_KEY', '')
-_api_bearer_token = os.getenv('GREMLIN_BEARER_TOKEN', '')
+_api_key = os.getenv("GREMLIN_API_KEY", "")
+_api_bearer_token = os.getenv("GREMLIN_BEARER_TOKEN", "")
 _bearer_token_timestamp = None
-_max_bearer_interval=os.getenv('GREMLIN_MAX_BEARER_INTERVAL', 86400)
-_api_user = os.getenv('GREMLIN_USER', '')
-_api_password = os.getenv('GREMLIN_PASSWORD', '')
-_api_user_mfa_token = os.getenv('GREMLIN_USER_MFA_TOKEN', None)
-_api_company = os.getenv('GREMLIN_COMPANY', '')
-_api_team_id = os.getenv('GREMLIN_TEAM_ID', '')
+_max_bearer_interval = os.getenv("GREMLIN_MAX_BEARER_INTERVAL", 86400)
+_api_user = os.getenv("GREMLIN_USER", "")
+_api_password = os.getenv("GREMLIN_PASSWORD", "")
+_api_user_mfa_token = os.getenv("GREMLIN_USER_MFA_TOKEN", None)
+_api_company = os.getenv("GREMLIN_COMPANY", "")
+_api_team_id = os.getenv("GREMLIN_TEAM_ID", "")
 
-_http_proxy = os.getenv('GREMLIN_HTTP_PROXY', os.getenv('HTTP_PROXY', None))
-_https_proxy = os.getenv('GREMLIN_HTTPS_PROXY', os.getenv('HTTPS_PROXY', None))
+_http_proxy = os.getenv("GREMLIN_HTTP_PROXY", os.getenv("HTTP_PROXY", None))
+_https_proxy = os.getenv("GREMLIN_HTTPS_PROXY", os.getenv("HTTPS_PROXY", None))
 
 
 GremlinAPIConfig.user = _api_user
 GremlinAPIConfig.password = _api_password
 GremlinAPIConfig.user_mfa_token_value = _api_user_mfa_token
-GremlinAPIConfig.base_uri = f'{_api_host}/{_api_version}'
+GremlinAPIConfig.base_uri = f"{_api_host}/{_api_version}"
 GremlinAPIConfig.company_name = _api_company
 GremlinAPIConfig.api_key = _api_key
 GremlinAPIConfig.bearer_token = _api_bearer_token
 GremlinAPIConfig.bearer_timestamp = _bearer_token_timestamp
 GremlinAPIConfig.max_bearer_interval = _max_bearer_interval
 GremlinAPIConfig.http_proxy = _http_proxy
 GremlinAPIConfig.https_proxy = _https_proxy
 
 
 def _auth_response_to_bearer_config(auth_response):
-    # log.debug(auth_response[0]['header'])
-    GremlinAPIConfig.bearer_token = auth_response[0]['header']
+    # if (log.getEffectiveLevel() == logging.DEBUG): log.debug(auth_response[0]['header'])
+    GremlinAPIConfig.bearer_token = auth_response[0]["header"]
     GremlinAPIConfig.bearer_timestamp = datetime.now(timezone.utc)
-    GremlinAPIConfig.bearer_expires = datetime.strptime(auth_response[0]['expires_at'], '%Y-%m-%dT%H:%M:%S.%f%z')
+    GremlinAPIConfig.bearer_expires = datetime.strptime(
+        auth_response[0]["expires_at"], "%Y-%m-%dT%H:%M:%S.%f%z"
+    )
 
 
-def login(email=GremlinAPIConfig.user, password=GremlinAPIConfig.password,
-          company_name=GremlinAPIConfig.company_name, token=GremlinAPIConfig.user_mfa_token_value):
+def login(
+    email=GremlinAPIConfig.user,
+    password=GremlinAPIConfig.password,
+    company_name=GremlinAPIConfig.company_name,
+    token=GremlinAPIConfig.user_mfa_token_value,
+):
     if GremlinAPIConfig.user != email:
-        log.debug('Received user without value being present in config, updating config to match.')
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(
+                "Received user without value being present in config, updating config to match."
+            )
         GremlinAPIConfig.user = email
     if GremlinAPIConfig.password != password:
-        log.debug('Received password without value being present in config, updating config to match.')
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(
+                "Received password without value being present in config, updating config to match."
+            )
         GremlinAPIConfig.password = password
     if GremlinAPIConfig.company_name != company_name:
-        log.debug('Received company name without value being present in config, updating config to match.')
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(
+                "Received company name without value being present in config, updating config to match."
+            )
         GremlinAPIConfig.company_name = company_name
     if token and GremlinAPIConfig.user_mfa_token_value != token:
-        log.debug('Received mfa token without value being present in config, updating config to match.')
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(
+                "Received mfa token without value being present in config, updating config to match."
+            )
         GremlinAPIConfig.user_mfa_token_value = token
-    if(not GremlinAPIConfig.bearer_timestamp
-       or not GremlinAPIConfig.bearer_token
-       or GremlinAPIConfig.is_bearer_expired()):
+    if (
+        not GremlinAPIConfig.bearer_timestamp
+        or not GremlinAPIConfig.bearer_token
+        or GremlinAPIConfig.is_bearer_expired()
+    ):
         if token:
-            log.debug(f'MFA Login for {email} in company {company_name}')
-            auth_response = userMFAuth.auth_user(email=email, password=password,
-                                                 companyName=company_name, token=token)
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"MFA Login for {email} in company {company_name}")
+            auth_response = userMFAuth.auth_user(
+                email=email, password=password, companyName=company_name, token=token
+            )
         else:
-            log.debug(f'Non-MFA Login for {email} in company {company_name}')
-            auth_response = userAuth.auth_user(email=email, password=password, companyName=company_name)
-        # log.debug(auth_response)
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"Non-MFA Login for {email} in company {company_name}")
+            auth_response = userAuth.auth_user(
+                email=email, password=password, companyName=company_name
+            )
+        # if (log.getEffectiveLevel() == logging.DEBUG): log.debug(auth_response)
         _auth_response_to_bearer_config(auth_response)
 
 
 def saml_login(email=GremlinAPIConfig.user, saml_assertion=None, relay_state=None):
     """
     Use SAML to perform an API login and return a bearer token
 
     :param email: email address of the user/service account
     :param saml_assertion:
     :param relay_state:
     :return:
     """
     if GremlinAPIConfig.user != email:
-        log.debug('Received user without value being present in config, updating config to match.')
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(
+                "Received user without value being present in config, updating config to match."
+            )
         GremlinAPIConfig.user = email
     if not saml_assertion and relay_state:
-        error_msg = f'Expecting a SAML assertion and relay state, received none'
+        error_msg = f"Expecting a SAML assertion and relay state, received none"
         log.fatal(error_msg)
         raise GremlinParameterError(error_msg)
-    acs_response = GremlinAPISaml.acs(SAMLResponse=saml_assertion, RelayState=relay_state)
+    acs_response = GremlinAPISaml.acs(
+        SAMLResponse=saml_assertion, RelayState=relay_state
+    )
     try:
         # redirect = re.search('window\.location="(.+?)"', acs_response).group(1)
-        saml_session_code = re.search('SamlSessionCode=(.+?)&', acs_response.headers['location']).group(1)
+        saml_session_code = re.search(
+            "SamlSessionCode=(.+?)&", acs_response.headers["location"]
+        ).group(1)
     except AttributeError:
-        error_msg = 'SAML Response did not provide a valid saml session code'
+        error_msg = "SAML Response did not provide a valid saml session code"
         log.fatal(error_msg)
         raise GremlinAuthError(error_msg)
     saml_sessions = GremlinAPISaml.sessions(code=saml_session_code)
-    GremlinAPIConfig.bearer_token = saml_sessions['header']
+    GremlinAPIConfig.bearer_token = saml_sessions["header"]
     return GremlinAPIConfig.bearer_token
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/alfi.py` & `gremlinapi-0.9.7/gremlinapi/templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,75 +6,89 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
-class GremlinALFI(GremlinAPI):
+class GremlinAPITemplates(GremlinAPI):
     @classmethod
-    @register_cli_action('create_alfi_experiment', ('body',), ('teamId'))
-    def create_alfi_experiment(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint('/experiments', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+    @register_cli_action("list_templates", ("",), ("teamId",))
+    def list_templates(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/templates", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_all_alfi_experiments', ('',), ('teamId',))
-    def halt_all_alfi_experiments(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        endpoint = cls._optional_team_endpoint('/experiments', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("create_template", ("body",), ("teamId",))
+    def create_template(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "POST"
+        data = cls._error_if_not_json_body(**kwargs)
+        endpoint = cls._optional_team_endpoint(f"/templates", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_alfi_experiment_details', ('guid',), ('teamId',))
-    def get_alfi_experiment_details(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/experiments/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_template", ("guid",), ("teamId",))
+    def get_template(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/templates/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_alfi_experiment', ('guid',), ('teamId',))
-    def halt_alfi_experiment(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/experiments/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("delete_template", ("guid",), ("teamId",))
+    def delete_template(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/templates/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_alfi_experiments', ('',), ('teamId',))
-    def list_active_alfi_experiments(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint('/experiments/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_command_templates", ("",), ("teamId",))
+    def list_command_templates(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/templates/command", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_completed_alfi_experiments', ('',), ('teamId'))
-    def list_completed_alfi_experiments(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint('/experiments/completed', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_target_templates", ("",), ("teamId",))
+    def list_target_templates(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/templates/target", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
+    @classmethod
+    @register_cli_action("list_trigger_templates", ("",), ("teamId",))
+    def list_trigger_templates(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/templates/trigger", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
+        (resp, body) = https_client.api_call(method, endpoint, **payload)
+        return body
```

### Comparing `gremlinapi-0.9.2/gremlinapi/apikeys.py` & `gremlinapi-0.9.7/gremlinapi/apikeys.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,48 +5,56 @@
 import logging
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIapikeys(GremlinAPI):
     @classmethod
-    @register_cli_action('create_apikey', ('description', 'identifier',), ('teamId',))
+    @register_cli_action(
+        "create_apikey",
+        (
+            "description",
+            "identifier",
+        ),
+        ("teamId",),
+    )
     def create_apikey(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        data = {'description': cls._error_if_not_param('description', **kwargs),
-                'identifier': cls._error_if_not_param('identifier', **kwargs)}
-        endpoint = cls._optional_team_endpoint(f'/apikeys', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        method = "POST"
+        data = {
+            "description": cls._error_if_not_param("description", **kwargs),
+            "identifier": cls._error_if_not_param("identifier", **kwargs),
+        }
+        endpoint = cls._optional_team_endpoint(f"/apikeys", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
-
     @classmethod
-    @register_cli_action('list_apikeys', ('',), ('teamId',))
+    @register_cli_action("list_apikeys", ("",), ("teamId",))
     def list_apikeys(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/apikeys', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/apikeys", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('revoke_apikey', ('identifier',), ('teamId',))
+    @register_cli_action("revoke_apikey", ("identifier",), ("teamId",))
     def revoke_apikey(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/apikeys/{identifier}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/apikeys/{identifier}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
-        return body
+        return body
```

### Comparing `gremlinapi-0.9.2/gremlinapi/attack_helpers.py` & `gremlinapi-0.9.7/gremlinapi/attack_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,144 +5,161 @@
 import json
 import logging
 import re
 
 from gremlinapi.exceptions import (
     GremlinCommandTargetError,
     GremlinIdentifierError,
-    GremlinParameterError
+    GremlinParameterError,
 )
 
 from gremlinapi.clients import GremlinAPIClients as clients
 from gremlinapi.containers import GremlinAPIContainers as containers
 from gremlinapi.providers import GremlinAPIProviders as providers
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAttackHelper(object):
     def __init__(self, *args, **kwargs):
         self._command = None
         self._target = None
-        self.command = kwargs.get('command', GremlinCPUAttack())
-        self.target = kwargs.get('target', GremlinTargetHosts())
+        self.command = kwargs.get("command", GremlinCPUAttack())
+        self.target = kwargs.get("target", GremlinTargetHosts())
 
     @property
     def command(self):
         return self._command
 
     @command.setter
     def command(self, _command=None):
         if not issubclass(type(_command), GremlinAttackCommandHelper):
-            error_msg = f'Command needs to be a child class of {type(GremlinAttackCommandHelper)}'
+            error_msg = f"Command needs to be a child class of {type(GremlinAttackCommandHelper)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        if issubclass(type(_command), GremlinTimeTravelAttack) and \
-                issubclass(type(self.target), GremlinTargetContainers):
-            error_msg = f'TimeTravel cannot target containers'
+        if issubclass(type(_command), GremlinTimeTravelAttack) and issubclass(
+            type(self.target), GremlinTargetContainers
+        ):
+            error_msg = f"TimeTravel cannot target containers"
             log.fatal(error_msg)
             raise GremlinCommandTargetError(error_msg)
         self._command = _command
 
     @property
     def target(self):
         return self._target
 
     @target.setter
     def target(self, _target=None):
         if not issubclass(type(_target), GremlinAttackTargetHelper):
-            error_msg = f'Command needs to be a child class of {type(GremlinAttackTargetHelper)}'
+            error_msg = f"Command needs to be a child class of {type(GremlinAttackTargetHelper)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        if issubclass(type(_target), GremlinTargetContainers) and \
-                issubclass(type(self.command), GremlinTimeTravelAttack):
-            error_msg = f'TimeTravel cannot target containers'
+        if issubclass(type(_target), GremlinTargetContainers) and issubclass(
+            type(self.command), GremlinTimeTravelAttack
+        ):
+            error_msg = f"TimeTravel cannot target containers"
             log.fatal(error_msg)
             raise GremlinCommandTargetError(error_msg)
         self._target = _target
 
     def repr_model(self):
         model = {
-            'target': json.loads(str(self.target)),
-            'command': json.loads(str(self.command))
+            "target": json.loads(str(self.target)),
+            "command": json.loads(str(self.command)),
         }
         return model
 
     def __repr__(self):
         model = self.repr_model()
         return json.dumps(model)
 
 
 class GremlinAttackTargetHelper(object):
     def __init__(self, *args, **kwargs):
         self._strategy_type = None
         self._exact = 0
         self._percent = 10
-        self._allowed_strategy_types = {'exact': 'Exact', 'random': 'Random'}
-        self.exact = kwargs.get('exact', self._exact)
-        self.percent = kwargs.get('percent', self._percent)
-        self.strategy_type = kwargs.get('strategy_type', 'random')  # Validate Random or Exact
+        self._allowed_strategy_types = {"exact": "Exact", "random": "Random"}
+        self.exact = kwargs.get("exact", self._exact)
+        self.percent = kwargs.get("percent", self._percent)
+        self.strategy_type = kwargs.get(
+            "strategy_type", "random"
+        )  # Validate Random or Exact
 
     def target_definition(self):
         model = self.repr_model()
-        _target_definition = {
-            'strategyType': self.strategy_type,
-            'strategy': dict()
-        }
-        if model.get('percent', None):
-            _target_definition['strategy'] = {'percentage': model['percent']}
-        elif model.get('exact', None):
-            _target_definition['strategy'] = {'count': model['exact']}
+        _target_definition = {"strategyType": self.strategy_type, "strategy": dict()}
+        if model.get("percent", None):
+            _target_definition["strategy"] = {"percentage": model["percent"]}
+        elif model.get("exact", None):
+            _target_definition["strategy"] = {"count": model["exact"]}
         else:
-            error_msg = 'Targeting was not properly defined'
+            error_msg = "Targeting was not properly defined"
             log.fatal(error_msg)
             raise GremlinCommandTargetError(error_msg)
-        if type(model.get('containers')) == dict and model.get('containers').get('multiSelectLabels'):
-            _target_definition['strategy']['multiSelectLabels'] = model['containers']['multiSelectLabels']
-        if type(model.get('hosts')) == dict and model.get('hosts').get('multiSelectLabels'):
-            _target_definition['strategy']['multiSelectLabels'] = model['hosts']['multiSelectLabels']
+        if type(model.get("containers")) == dict and model.get("containers").get(
+            "multiSelectLabels"
+        ):
+            _target_definition["strategy"]["multiSelectLabels"] = model["containers"][
+                "multiSelectLabels"
+            ]
+        if type(model.get("hosts")) == dict and model.get("hosts").get(
+            "multiSelectLabels"
+        ):
+            _target_definition["strategy"]["multiSelectLabels"] = model["hosts"][
+                "multiSelectLabels"
+            ]
         return _target_definition
 
     def target_definition_graph(self):
         model = self.repr_model()
-        _target_definition = {
-            'strategy_type': self.strategy_type,
-            'strategy': dict()
-        }
-        if model.get('percent', None):
-            _target_definition['strategy'] = {'type': 'RandomPercent', 'percentage': model['percent']}
-        elif model.get('exact', None):
-            _target_definition['strategy'] = {'type': 'Exact', 'count': model['exact']}
+        _target_definition = {"strategy_type": self.strategy_type, "strategy": dict()}
+        if model.get("percent", None):
+            _target_definition["strategy"] = {
+                "type": "RandomPercent",
+                "percentage": model["percent"],
+            }
+        elif model.get("exact", None):
+            _target_definition["strategy"] = {"type": "Exact", "count": model["exact"]}
         else:
-            error_msg = 'Targeting was not properly defined'
+            error_msg = "Targeting was not properly defined"
             log.fatal(error_msg)
             raise GremlinCommandTargetError(error_msg)
-        if type(model.get('containers')) == dict and model.get('containers').get('multiSelectLabels'):
-            _target_definition['target_type'] = 'Container'
-            _target_definition['strategy']['attrs'] = dict()
-            _target_definition['strategy']['attrs']['multiSelectLabels'] = model['containers']['multiSelectLabels']
-        if type(model.get('hosts')) == dict and model.get('hosts').get('multiSelectLabels'):
-            _target_definition['target_type'] = 'Host'
-            _target_definition['strategy']['attrs'] = dict()
-            _target_definition['strategy']['attrs']['multiSelectLabels'] = model['hosts']['multiSelectLabels']
+        if type(model.get("containers")) == dict and model.get("containers").get(
+            "multiSelectLabels"
+        ):
+            _target_definition["target_type"] = "Container"
+            _target_definition["strategy"]["attrs"] = dict()
+            _target_definition["strategy"]["attrs"]["multiSelectLabels"] = model[
+                "containers"
+            ]["multiSelectLabels"]
+        if type(model.get("hosts")) == dict and model.get("hosts").get(
+            "multiSelectLabels"
+        ):
+            _target_definition["target_type"] = "Host"
+            _target_definition["strategy"]["attrs"] = dict()
+            _target_definition["strategy"]["attrs"]["multiSelectLabels"] = model[
+                "hosts"
+            ]["multiSelectLabels"]
         return _target_definition
 
     @property
     def exact(self):
         return self._exact
 
     @exact.setter
     def exact(self, _exact=None):
         if not _exact:
             self._exact = 0
         elif isinstance(_exact, int) and _exact > 0:
             self._exact = _exact
             self._percent = 0
         else:
-            error_msg = f'Exact number of targets must be an integer greater than 0'
+            error_msg = f"Exact number of targets must be an integer greater than 0"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def percent(self):
         return self._percent
 
@@ -150,39 +167,43 @@
     def percent(self, _percent=None):
         if not _percent:
             self._percent = 0
         elif isinstance(_percent, int) and 1 <= _percent <= 100:
             self._percent = _percent
             self._exact = 0
         else:
-            error_msg = f'Target percentage must be an integer between 1 and 100'
+            error_msg = f"Target percentage must be an integer between 1 and 100"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def strategy_type(self):
         return self._strategy_type
 
     @strategy_type.setter
     def strategy_type(self, _target_type=None):
-        if not isinstance(_target_type, str) or not self._allowed_strategy_types.get(_target_type.lower(), None):
-            error_msg = f'strategy_type needs to be one of {str(self._allowed_strategy_types.keys())[1:-2]}'
+        if not isinstance(_target_type, str) or not self._allowed_strategy_types.get(
+            _target_type.lower(), None
+        ):
+            error_msg = f"strategy_type needs to be one of {str(self._allowed_strategy_types.keys())[1:-2]}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        self._strategy_type = self._allowed_strategy_types.get(_target_type.lower(), None)
+        self._strategy_type = self._allowed_strategy_types.get(
+            _target_type.lower(), None
+        )
 
     def repr_model(self):
         model = dict()
-        model['type'] = self.strategy_type
+        model["type"] = self.strategy_type
         if self.exact >= 0 and not self.percent:
-            model['exact'] = str(self.exact)
-        elif self.strategy_type == 'Random':
-            model['percent'] = self.percent
+            model["exact"] = str(self.exact)
+        elif self.strategy_type == "Random":
+            model["percent"] = self.percent
         else:
-            error_msg = f'Type not correctly set, needs to be one of {str(self._allowed_strategy_types.keys())[1:-2]}'
+            error_msg = f"Type not correctly set, needs to be one of {str(self._allowed_strategy_types.keys())[1:-2]}"
             log.error(error_msg)
             raise GremlinParameterError(error_msg)
         return model
 
     def __repr__(self):
         model = self.repr_model()
         return json.dumps(model)
@@ -192,50 +213,54 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._active_clients = list()
         self._active_identifiers = list()
         self._active_tags = dict()
         self._ids = list()
         self._multiSelectTags = dict()
-        self._nativeTags = {'os-type': 'os_type', 'os-version': 'os_version'}
+        self._nativeTags = {"os-type": "os_type", "os-version": "os_version"}
         self._target_all_hosts = False
-        self.target_all_hosts = kwargs.get('target_all_hosts', True)
+        self.target_all_hosts = kwargs.get("target_all_hosts", True)
 
     # def target_definition(self):
     #     model = json.loads(self.__repr__())
     #     del model['type']
     #     _target_definition = super().target_definition()
     #     _target_definition['strategy'] = model
     #     _target_definition['targetType'] = 'Host'
     #     return _target_definition
 
     def target_definition(self):
         _target_definition = super().target_definition()
-        _target_definition['targetType'] = 'Host'
+        _target_definition["targetType"] = "Host"
         return _target_definition
 
     @property
     def ids(self):
         return self._ids
 
     @ids.setter
     def ids(self, _ids=None):
         if not isinstance(_ids, list):
-            error_msg = f'ids expects a list of strings, received {type(_ids)}'
+            error_msg = f"ids expects a list of strings, received {type(_ids)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         for _identifier in _ids:
             if not isinstance(_identifier, str):
-                error_msg = f'Identifier not string; ids expect a string or list of strings'
+                error_msg = (
+                    f"Identifier not string; ids expect a string or list of strings"
+                )
                 log.fatal(error_msg)
                 raise GremlinParameterError(error_msg)
             if self._valid_identifier(_identifier):
                 self._ids.append(_identifier)
             else:
-                error_msg = f'Target identifier "{_identifier}" not found in active clients'
+                error_msg = (
+                    f'Target identifier "{_identifier}" not found in active clients'
+                )
                 log.warning(error_msg)
                 raise GremlinIdentifierError(error_msg)
         self._multiSelectTags = {}
         self.target_all_hosts = False
 
     @property
     def tags(self):
@@ -261,34 +286,34 @@
         else:
             self._target_all_hosts = False
 
     def _filter_active_identifiers(self):
         if not len(self._active_identifiers) > 0:
             self._load_active_clients()
             for _client in self._active_clients:
-                self._active_identifiers.append(_client['identifier'])
+                self._active_identifiers.append(_client["identifier"])
 
     def _filter_active_tags(self):
         if not len(self._active_tags) > 0:
             self._load_active_clients()
             for _client in self._active_clients:
                 for _tag in self._nativeTags:
                     if not self._active_tags.get(_tag):
                         self._active_tags[_tag] = list()
                     if _client.get(_tag) not in self._active_tags[_tag]:
                         self._active_tags[_tag].append(_client.get(_tag))
-                for _tag in _client.get('tags'):
+                for _tag in _client.get("tags"):
                     if not self._active_tags.get(_tag):
                         self._active_tags[_tag] = list()
-                    _tag_value = _client['tags'].get(_tag)
+                    _tag_value = _client["tags"].get(_tag)
                     if isinstance(_tag_value, str):
                         if _tag_value not in self._active_tags[_tag]:
                             self._active_tags[_tag].append(_tag_value)
                     elif isinstance(_tag_value, list):
-                        for _inner_tag_value in _client['tags'].get(_tag):
+                        for _inner_tag_value in _client["tags"].get(_tag):
                             if _inner_tag_value not in self._active_tags[_tag]:
                                 self._active_tags[_tag].append(_inner_tag_value)
 
     def _load_active_clients(self):
         if not len(self._active_clients) > 0:
             self._active_clients = clients.list_active_clients()
 
@@ -305,24 +330,20 @@
         if tagValue in self._active_tags.get(tagKey, []):
             return True
         return False
 
     def repr_model(self):
         model = super().repr_model()
         if self.target_all_hosts:
-            model['hosts'] = 'all'
+            model["hosts"] = "all"
         else:
             if len(self.ids) > 0:
-                model['hosts'] = {
-                    'ids': self.ids
-                }
+                model["hosts"] = {"ids": self.ids}
             elif len(self.tags) > 0:
-                model['hosts'] = {
-                    'multiSelectTags': self.tags
-                }
+                model["hosts"] = {"multiSelectTags": self.tags}
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     if self.target_all_hosts:
     #         model['hosts'] = 'all'
     #     else:
@@ -341,19 +362,19 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._active_containers = list()
         self._active_identifiers = list()
         self._active_labels = dict()
         self._ids = list()
         self._multiSelectLabels = dict()
-        #self._nativeTags = {'os-type': 'os_type', 'os-version': 'os_version'}
+        # self._nativeTags = {'os-type': 'os_type', 'os-version': 'os_version'}
         self._target_all_containers = True
-        self.target_all_containers = kwargs.get('target_all_containers', True)
-        self.ids = kwargs.get('ids', list())
-        self.labels = kwargs.get('labels', dict())
+        self.target_all_containers = kwargs.get("target_all_containers", True)
+        self.ids = kwargs.get("ids", list())
+        self.labels = kwargs.get("labels", dict())
 
     # def target_definition(self):
     #     model = json.loads(self.__repr__())
     #     del model['type']
     #     _target_definition = super().target_definition()
     #     _target_definition['strategy'] = {
     #         'percent': model['percent']
@@ -361,50 +382,54 @@
     #     if model.get('multiSelectLabels'):
     #         _target_definition['strategy']['multiSelectLabels'] = model['multiSelectLabels']
     #     _target_definition['targetType'] = 'Container'
     #     return _target_definition
 
     def target_definition(self):
         _target_definition = super().target_definition()
-        _target_definition['targetType'] = 'Container'
+        _target_definition["targetType"] = "Container"
         return _target_definition
 
     @property
     def ids(self):
         return self._ids
 
     @ids.setter
     def ids(self, _ids=None):
         if not isinstance(_ids, list):
-            error_msg = f'ids expects a list of strings, received {type(_ids)}'
+            error_msg = f"ids expects a list of strings, received {type(_ids)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if len(_ids) >= 1:
             for _identifier in _ids:
                 if not isinstance(_identifier, str):
-                    error_msg = f'Identifier not string; ids expect a string or list of strings'
+                    error_msg = (
+                        f"Identifier not string; ids expect a string or list of strings"
+                    )
                     log.fatal(error_msg)
                     raise GremlinParameterError(error_msg)
                 if self._valid_identifier(_identifier):
                     self._ids.append(_identifier)
                 else:
-                    error_msg = f'Target identifier "{_identifier}" not found in active clients'
+                    error_msg = (
+                        f'Target identifier "{_identifier}" not found in active clients'
+                    )
                     log.warning(error_msg)
                     raise GremlinIdentifierError(error_msg)
             self._multiSelectLabels = {}
             self.target_all_containers = False
 
     @property
     def labels(self):
         return self._multiSelectLabels
 
     @labels.setter
     def labels(self, _labels=None):
         if not isinstance(_labels, dict):
-            error_msg = f'labels expects a dictionary, received {type(_labels)}'
+            error_msg = f"labels expects a dictionary, received {type(_labels)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if bool(_labels):
             for _label in _labels:
                 if isinstance(_labels[_label], str):
                     if self._valid_label_pair(_label, _labels[_label]):
                         if isinstance(self._multiSelectLabels.get(_label, None), list):
@@ -431,29 +456,31 @@
         else:
             self._target_all_containers = False
 
     def _filter_active_identifiers(self):
         if not len(self._active_identifiers) > 0:
             self._load_active_containers()
             for _container in self._active_containers:
-                self._active_identifiers.append(_container['identifier'])
+                self._active_identifiers.append(_container["identifier"])
 
     def _filter_active_labels(self):
         if not len(self._active_labels) > 0:
             self._load_active_containers()
             for _container in self._active_containers:
-                for _label in _container.get('container_labels'):
+                for _label in _container.get("container_labels"):
                     if not self._active_labels.get(_label):
                         self._active_labels[_label] = list()
-                    _label_value = _container['container_labels'].get(_label)
+                    _label_value = _container["container_labels"].get(_label)
                     if isinstance(_label_value, str):
                         if _label_value not in self._active_labels[_label]:
                             self._active_labels[_label].append(_label_value)
                     elif isinstance(_label_value, list):
-                        for _inner_label_value in _container['container_labels'].get(_label):
+                        for _inner_label_value in _container["container_labels"].get(
+                            _label
+                        ):
                             if _inner_label_value not in self._active_labels[_label]:
                                 self._active_labels[_label].append(_inner_label_value)
 
     def _load_active_containers(self):
         if not len(self._active_containers) > 0:
             self._active_containers = containers.list_containers()
 
@@ -470,24 +497,20 @@
         if labelValue in self._active_labels.get(labelKey, []):
             return True
         return False
 
     def repr_model(self):
         model = super().repr_model()
         if self.target_all_containers:
-            model['containers'] = 'all'
+            model["containers"] = "all"
         else:
             if len(self.ids) > 0:
-                model['containers'] = {
-                    'ids': self.ids
-                }
+                model["containers"] = {"ids": self.ids}
             elif len(self.labels) > 0:
-                model['containers'] = {
-                    'multiSelectLabels': self.labels
-                }
+                model["containers"] = {"multiSelectLabels": self.labels}
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     if self.target_all_containers:
     #         model['containers'] = 'all'
     #     else:
@@ -504,217 +527,222 @@
 
 class GremlinAttackCommandHelper(object):
     def __init__(self, *args, **kwargs):
         self._length = 60
         self._commandType = str()
         self._shortType = str()
         self._typeMap = {
-            'cpu': 'CPU',
-            'memory': 'Memory',
-            'disk': 'Disk',
-            'io': 'IO',
-            'process_killer': 'Process Killer',
-            'shutdown': 'Shutdown',
-            'time_travel': 'Time Travel',
-            'blackhole': 'Blackhole',
-            'dns': 'DNS',
-            'latency': 'Latency',
-            'packet_loss': 'Packet Loss'
+            "cpu": "CPU",
+            "memory": "Memory",
+            "disk": "Disk",
+            "io": "IO",
+            "process_killer": "Process Killer",
+            "shutdown": "Shutdown",
+            "time_travel": "Time Travel",
+            "blackhole": "Blackhole",
+            "dns": "DNS",
+            "latency": "Latency",
+            "packet_loss": "Packet Loss",
         }
-        self.length = kwargs.get('length', 60)
+        self.length = kwargs.get("length", 60)
 
     def impact_definition(self):
         model = self.repr_model()
         _impact_definition = {
-            'commandArgs': {
-                'cliArgs': [str(self.shortType)],
-                'length': self.length
-            },
-            'commandType': str(self.shortType)
+            "commandArgs": {"cliArgs": [str(self.shortType)], "length": self.length},
+            "commandType": str(self.shortType),
         }
-        _impact_definition['commandArgs']['cliArgs'].extend(model['args'])
+        _impact_definition["commandArgs"]["cliArgs"].extend(model["args"])
         return _impact_definition
 
     def impact_definition_graph(self):
         model = self.repr_model()
         _impact_definition = {
-            'infra_command_args': {
-                'cli_args': [str(self.shortType)],
-                'type': str(self.shortType)
+            "infra_command_args": {
+                "cli_args": [str(self.shortType)],
+                "type": str(self.shortType),
             },
-            'infra_command_type': str(self.shortType)
+            "infra_command_type": str(self.shortType),
         }
-        _impact_definition['infra_command_args']['cli_args'].extend(model['args'])
+        _impact_definition["infra_command_args"]["cli_args"].extend(model["args"])
         return _impact_definition
 
     @property
     def commandType(self):
         return self._commandType
 
     @commandType.setter
     def commandType(self, _commandType=None):
         if not isinstance(_commandType, str):
-            error_msg = f'commandType expects a string, received {type(_commandType)}'
+            error_msg = f"commandType expects a string, received {type(_commandType)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         try:
-            self._shortType = list(self._typeMap.keys())[list(self._typeMap.values()).index(_commandType)]
+            self._shortType = list(self._typeMap.keys())[
+                list(self._typeMap.values()).index(_commandType)
+            ]
         except ValueError:
-            error_msg = f'commandType needs to be one of: {str(self._typeMap.values())[1:-2]}'
+            error_msg = (
+                f"commandType needs to be one of: {str(self._typeMap.values())[1:-2]}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._commandType = _commandType
 
     @property
     def length(self):
         return self._length
 
     @length.setter
     def length(self, _length=None):
-        if not (isinstance(_length, int) and 1 <= _length <= 31449600):  # Roughly 1 year in seconds
-            error_msg = f'Attack length needs to be an integer between 1 and 31449600'
+        if not (
+            isinstance(_length, int) and 1 <= _length <= 31449600
+        ):  # Roughly 1 year in seconds
+            error_msg = f"Attack length needs to be an integer between 1 and 31449600"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._length = _length
 
     @property
     def shortType(self):
         return self._shortType
 
     @shortType.setter
     def shortType(self, _shortType=None):
         if not isinstance(_shortType, str):
-            error_msg = f'type_ expects a string, received {type(_shortType)}'
+            error_msg = f"type_ expects a string, received {type(_shortType)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if not _shortType.lower() in self._typeMap:
-            error_msg = f'invalid attack type, expected one of {str(self._typeMap.keys())[1:-2]}'
+            error_msg = f"invalid attack type, expected one of {str(self._typeMap.keys())[1:-2]}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._commandType = self._typeMap[_shortType]
         self._shortType = _shortType
 
     def repr_model(self):
         model = {
-            'type': self.shortType,
-            'commandType': self.commandType,
-            'args': [
-                '-l', str(self.length)
-            ]
+            "type": self.shortType,
+            "commandType": self.commandType,
+            "args": ["-l", str(self.length)],
         }
         return model
 
     def __repr__(self):
         model = self.repr_model()
         return json.dumps(model)
 
 
 class GremlinResourceAttackHelper(GremlinAttackCommandHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._blocksize = 4
-        self._directory = '/tmp'
+        self._directory = "/tmp"
         self._percent = 100
         self._workers = 1
 
     @property
     def blocksize(self):
         return self._blocksize
 
     @blocksize.setter
     def blocksize(self, _blocksize=None):
         if not (isinstance(_blocksize, int) and _blocksize >= 1):
-            error_msg = f'blocksize requires a positive integer'
+            error_msg = f"blocksize requires a positive integer"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._blocksize = _blocksize
 
     @property
     def directory(self):
         return self._directory
 
     @directory.setter
     def directory(self, _directory=None):
         if not isinstance(_directory, str):
-            error_msg = f'directory requires a string, received {type(_directory)}'
+            error_msg = f"directory requires a string, received {type(_directory)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._directory = _directory
 
     @property
     def percent(self):
         return self._percent
 
     @percent.setter
     def percent(self, _percent=None):
         if not (isinstance(_percent, int) and 1 <= _percent <= 100):
-            error_msg = f'percent is required to be an int between 1 and 100'
+            error_msg = f"percent is required to be an int between 1 and 100"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._percent = _percent
 
     @property
     def workers(self):
         return self._workers
 
     @workers.setter
     def workers(self, _workers=None):
         if not (isinstance(_workers, int) and _workers >= 1):
-            error_msg = 'workers requires a positive integer'
+            error_msg = "workers requires a positive integer"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._workers = _workers
 
 
 class GremlinStateAttackHelper(GremlinAttackCommandHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class GremlinNetworkAttackHelper(GremlinAttackCommandHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._allowed_protocols = ['ICMP', 'TCP', 'UDP']
+        self._allowed_protocols = ["ICMP", "TCP", "UDP"]
         self._ips = list()
-        self._hostnames = ['^api.gremlin.com']
+        self._hostnames = ["^api.gremlin.com"]
         self._device = None
-        self._egress_ports = ['^53']
+        self._egress_ports = ["^53"]
         self._ingress_ports = list()
-        self._port_regex = '([0-9]{1,4}|[1-5][0-9]{4}|6[0-4][0-9]{3}|65[0-4][0-9]{2}|655[0-2][0-9]|6553[0-5])'
-        self._port_validator = re.compile(f'^\^?{self._port_regex}(-{self._port_regex})?$')
+        self._port_regex = "([0-9]{1,4}|[1-5][0-9]{4}|6[0-4][0-9]{3}|65[0-4][0-9]{2}|655[0-2][0-9]|6553[0-5])"
+        self._port_validator = re.compile(
+            f"^\^?{self._port_regex}(-{self._port_regex})?$"
+        )
         self._protocol = None
         self._providers = list()
         self._providers_filter = None
         self._source_ports = None
         self._tags = list()
         self._tags_filter = None
-        self.device = kwargs.get('device', None)        # -d, str
-        self.ips = kwargs.get('ips', None)              # -i, str
-        self.protocol = kwargs.get('protocol', None)    # -P, str
-        self.providers = kwargs.get('providers', None)  # providers block
-        self.tags = kwargs.get('tags', None)            # tags block
+        self.device = kwargs.get("device", None)  # -d, str
+        self.ips = kwargs.get("ips", None)  # -i, str
+        self.protocol = kwargs.get("protocol", None)  # -P, str
+        self.providers = kwargs.get("providers", None)  # providers block
+        self.tags = kwargs.get("tags", None)  # tags block
 
     def _filter_providers(self):
         _providers = providers.list_providers()
         for _provider in _providers:
-            self._providers_filter.extend(getattr(providers, f'list_{_provider}_services')())
+            self._providers_filter.extend(
+                getattr(providers, f"list_{_provider}_services")()
+            )
 
     def _port_maker(self, _ports=None):
         port_list = list()
         if not _ports:
             pass
         elif isinstance(_ports, int) or isinstance(_ports, str):
             if self._validate_port_or_range(str(_ports)):
                 port_list = [str(_ports)]
         elif isinstance(_ports, list):
             for _port in _ports:
                 if self._validate_port_or_range(str(_port)):
                     port_list.append(str(_port))
         else:
-            error_msg = f'_port_maker expects a {type(str)} or {type(int)} or a {type(list)} of the previous types'
+            error_msg = f"_port_maker expects a {type(str)} or {type(int)} or a {type(list)} of the previous types"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return port_list
 
     def _valid_tag_pair(self, tagKey=None, tagValue=None):
         return True
 
@@ -722,15 +750,15 @@
         return True
 
     def _validate_ip(self, _ip=None):
         return True
 
     def _validate_port_or_range(self, _port_or_range):
         if not self._port_validator.match(_port_or_range):
-            error_msg = f'{_port_or_range} is not a valid port or port range'
+            error_msg = f"{_port_or_range} is not a valid port or port range"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return True
 
     def _validate_provider(self, _provider=None):
         if not len(self._providers_filter) > 0:
             self._filter_providers()
@@ -744,15 +772,15 @@
 
     @device.setter
     def device(self, _device=None):
         if not _device:
             self._device = None
             return
         elif not isinstance(_device, str):
-            error_msg = f'device expects type {type(str)}'
+            error_msg = f"device expects type {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._device = _device
 
     @property
     def egress_ports(self):
         return self._egress_ports
@@ -783,55 +811,57 @@
             self._ips = [_ips]
         elif isinstance(_ips, list):
             for _ip in _ips:
                 if self._validate_ip(_ip):
                     pass
             self._ips = _ips
         else:
-            error_msg = f'valid ip addresses required'
+            error_msg = f"valid ip addresses required"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def hostnames(self):
         return self._hostnames
 
     @hostnames.setter
     def hostnames(self, _hostnames=None):
         if not _hostnames:
             pass
         elif isinstance(_hostnames, str):
             if not self._validate_hostname(_hostnames):
-                error_msg = f'valid hostnames required'
+                error_msg = f"valid hostnames required"
                 log.fatal(error_msg)
                 raise GremlinParameterError(error_msg)
             self._hostnames = [_hostnames]
         elif isinstance(_hostnames, list):
             for _hostname in _hostnames:
                 if not self._validate_hostname(_hostname):
-                    error_msg = f'valid hostnames required'
+                    error_msg = f"valid hostnames required"
                     log.fatal(error_msg)
                     raise GremlinParameterError(error_msg)
                 self._hostnames = _hostname
         else:
-            error_msg = f'hostnames requires a {type(str)} or {type(list)}'
+            error_msg = f"hostnames requires a {type(str)} or {type(list)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def protocol(self):
         return self._protocol
 
     @protocol.setter
     def protocol(self, _protocol=None):
         if not _protocol:
             self._protocol = None
             return
-        elif not (isinstance(_protocol, str) and _protocol.upper() in self._allowed_protocols):
-            error_msg = f'Protocol must be a string and one of {str(self._allowed_protocols)[1:-2]}'
+        elif not (
+            isinstance(_protocol, str) and _protocol.upper() in self._allowed_protocols
+        ):
+            error_msg = f"Protocol must be a string and one of {str(self._allowed_protocols)[1:-2]}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._protocol = _protocol.upper()
 
     @property
     def providers(self):
         return self._providers
@@ -845,15 +875,15 @@
                 self._providers = [_providers]
         elif isinstance(_providers, list):
             self._providers = list()
             for _provider in _providers:
                 if self._validate_provider(_provider):
                     self._providers.append(_provider)
         else:
-            error_msg = f'providers expect a {type(str)} or {type(list)}'
+            error_msg = f"providers expect a {type(str)} or {type(list)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def source_ports(self):
         return self._source_ports
 
@@ -873,25 +903,23 @@
                     self._multiSelectTags[_tag] = _tags[_tag]
         self._ids = []
         self.target_all_hosts = False
 
     def repr_model(self):
         model = super().repr_model()
         if self.device:
-            model['args'].extend(['-d', self.device])
+            model["args"].extend(["-d", self.device])
         if len(self.ips) > 0:
-            model['args'].extend(['-i', ','.join(self.ips)])
+            model["args"].extend(["-i", ",".join(self.ips)])
         if self.protocol:
-            model['args'].extend(['-P', self.protocol])
+            model["args"].extend(["-P", self.protocol])
         if self.providers and len(self.providers) > 0:
-            model['providers'] = self.providers
+            model["providers"] = self.providers
         if self.tags and len(self.tags) > 0:
-            model['trafficImpactMapping'] = {
-                'multiSelectTags': self.tags
-            }
+            model["trafficImpactMapping"] = {"multiSelectTags": self.tags}
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     if self.device:
     #         model['args'].extend(['-d', self.device])
     #     if len(self.ips) > 0:
@@ -906,65 +934,65 @@
     #         }
     #     return json.dumps(model)
 
 
 class GremlinCPUAttack(GremlinResourceAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'cpu'
+        self.shortType = "cpu"
         self._all_cores = False  # ['-a']
         self._capacity = 100  # ['-p', int]
         self._cores = 1  # ['-c', int]
-        self.all_cores = kwargs.get('all_cores', False)  # -a
-        self.capacity = kwargs.get('capacity', 100)      # -p, int
-        self.cores = kwargs.get('cores', 1)              # -c, int
+        self.all_cores = kwargs.get("all_cores", False)  # -a
+        self.capacity = kwargs.get("capacity", 100)  # -p, int
+        self.cores = kwargs.get("cores", 1)  # -c, int
 
     @property
     def all_cores(self):
         return self._all_cores
 
     @all_cores.setter
     def all_cores(self, _all_cores=None):
         if not isinstance(_all_cores, bool):
-            error_msg = f'all_cores expects a bool, received {type(_all_cores)}'
+            error_msg = f"all_cores expects a bool, received {type(_all_cores)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._all_cores = _all_cores
 
     @property
     def capacity(self):
         return self._capacity
 
     @capacity.setter
     def capacity(self, _capacity=None):
         if not (isinstance(_capacity, int) and 1 <= _capacity <= 100):
-            error_msg = f'Capacity expects an integer between 1 and 100'
+            error_msg = f"Capacity expects an integer between 1 and 100"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._capacity = _capacity
 
     @property
     def cores(self):
         return self._cores
 
     @cores.setter
     def cores(self, _cores=None):
         if not (isinstance(_cores, int) and _cores >= 1):
-            error_msg = f'Cores expects a positive integer'
+            error_msg = f"Cores expects a positive integer"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._cores = _cores
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-p', str(self.capacity)])
+        model["args"].extend(["-p", str(self.capacity)])
         if self.all_cores:
-            model['args'].append('-a')
+            model["args"].append("-a")
         else:
-            model['args'].extend(['-c', str(self.cores)])
+            model["args"].extend(["-c", str(self.cores)])
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-p', str(self.capacity)])
     #     if self.all_cores:
     #         model['args'].append('-a')
@@ -972,69 +1000,74 @@
     #         model['args'].extend(['-c', str(self.cores)])
     #     return json.dumps(model)
 
 
 class GremlinMemoryAttack(GremlinResourceAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'memory'
-        self._allowedAmountTypes = ['MB', 'GB', '%']
-        self._amount = '75'
-        self._amountType = '%'
-        self.amount = kwargs.get('amount', 100)          # ['-g' || '-m' || '-p'], int
-        self.amountType = kwargs.get('amountType', '%')  # ['-g' || '-m' || '-p']
+        self.shortType = "memory"
+        self._allowedAmountTypes = ["MB", "GB", "%"]
+        self._amount = "75"
+        self._amountType = "%"
+        self.amount = kwargs.get("amount", 100)  # ['-g' || '-m' || '-p'], int
+        self.amountType = kwargs.get("amountType", "%")  # ['-g' || '-m' || '-p']
 
     # def impact_definition(self):
     #     model = json.loads(self.__repr__())
     #     _impact_definition = super().impact_definition()
     #     _impact_definition['commandArgs']['cliArgs'].extend(model['args'])
     #     return _impact_definition
 
     @property
     def amount(self):
         return self._amount
 
     @amount.setter
     def amount(self, _amount=None):
         if not (isinstance(_amount, int) and _amount >= 1):
-            error_msg = f'amount expects a positive integer, received {type(_amount)}'
+            error_msg = f"amount expects a positive integer, received {type(_amount)}"
             log.fata(error_msg)
             raise GremlinParameterError(error_msg)
-        if self.amountType == '%' and not 1 <= _amount <= 100:
-            error_msg = f'amount must be an integer between 1 and 100 when amountType is set to %'
+        if self.amountType == "%" and not 1 <= _amount <= 100:
+            error_msg = f"amount must be an integer between 1 and 100 when amountType is set to %"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._amount = _amount
 
     @property
     def amountType(self):
         return self._amountType
 
     @amountType.setter
     def amountType(self, _amountType=None):
-        if not (isinstance(_amountType, str) and _amountType.upper() in self._allowedAmountTypes):
-            error_msg = f'amountType expects a string with a value belonging to {str(self._allowedAmountTypes)[1:-2]}'
+        if not (
+            isinstance(_amountType, str)
+            and _amountType.upper() in self._allowedAmountTypes
+        ):
+            error_msg = f"amountType expects a string with a value belonging to {str(self._allowedAmountTypes)[1:-2]}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        if _amountType == '%' and not 1 <= self.amount <= 100:
-            error_msg = f'amountType cannot be set to % while amount is not between 1 and 100'
+        if _amountType == "%" and not 1 <= self.amount <= 100:
+            error_msg = (
+                f"amountType cannot be set to % while amount is not between 1 and 100"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._amountType = _amountType.upper()
 
     def repr_model(self):
         model = super().repr_model()
-        if self.amountType == 'MB':
-            model['args'].extend(['-m', str(self.amount)])
-        elif self.amountType == 'GB':
-            model['args'].extend(['-g', str(self.amount)])
-        elif self.amountType == '%':
-            model['args'].extend(['-p', str(self.amount)])
+        if self.amountType == "MB":
+            model["args"].extend(["-m", str(self.amount)])
+        elif self.amountType == "GB":
+            model["args"].extend(["-g", str(self.amount)])
+        elif self.amountType == "%":
+            model["args"].extend(["-p", str(self.amount)])
         else:
-            error_msg = f'Fatal error, data model may be corrupted, amountType: {self._amountType} is not valid'
+            error_msg = f"Fatal error, data model may be corrupted, amountType: {self._amountType} is not valid"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     if self.amountType == 'MB':
@@ -1049,81 +1082,82 @@
     #         raise GremlinParameterError(error_msg)
     #     return json.dumps(model)
 
 
 class GremlinDiskSpaceAttack(GremlinResourceAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'disk'
-        self.blocksize = kwargs.get('blocksize', 4)
-        self.directory = kwargs.get('directory', '/tmp')
-        self.percent = kwargs.get('percent', 100)
-        self.workers = kwargs.get('workers', 1)
+        self.shortType = "disk"
+        self.blocksize = kwargs.get("blocksize", 4)
+        self.directory = kwargs.get("directory", "/tmp")
+        self.percent = kwargs.get("percent", 100)
+        self.workers = kwargs.get("workers", 1)
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].expand(['-d', str(self.directory)])
-        model['args'].expand(['-w', str(self.workers)])
-        model['args'].expand(['-b', str(self.blocksize)])
-        model['args'].expand(['-p', str(self.percent)])
+        model["args"].expand(["-d", str(self.directory)])
+        model["args"].expand(["-w", str(self.workers)])
+        model["args"].expand(["-b", str(self.blocksize)])
+        model["args"].expand(["-p", str(self.percent)])
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].expand(['-d', str(self.directory)])
     #     model['args'].expand(['-w', str(self.workers)])
     #     model['args'].expand(['-b', str(self.blocksize)])
     #     model['args'].expand(['-p', str(self.percent)])
     #     return json.dumps(model)
 
 
 class GremlinDiskIOAttack(GremlinResourceAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'io'
-        self._allowed_modes = ['r', 'rw', 'w']
+        self.shortType = "io"
+        self._allowed_modes = ["r", "rw", "w"]
         self._blockcount = 1
-        self._mode = 'rw'
-        self.blockcount = kwargs.get('blockcount', 1)     # -c, int
-        self.blocksize = kwargs.get('blocksize', 4)       # -s, int
-        self.directory = kwargs.get('directory', '/tmp')  # -d, str
-        self.mode = kwargs.get('mode', 'rw')              # -m, str
-        self.workers = kwargs.get('workers', 1)            # -w, int
+        self._mode = "rw"
+        self.blockcount = kwargs.get("blockcount", 1)  # -c, int
+        self.blocksize = kwargs.get("blocksize", 4)  # -s, int
+        self.directory = kwargs.get("directory", "/tmp")  # -d, str
+        self.mode = kwargs.get("mode", "rw")  # -m, str
+        self.workers = kwargs.get("workers", 1)  # -w, int
 
     @property
     def blockcount(self):
         return self._blockcount
 
     @blockcount.setter
     def blockcount(self, _blockcount=None):
         if not (isinstance(_blockcount, int) and _blockcount >= 1):
-            error_msg = f'blockcount requires a positive integer'
-            log.debug(error_msg)
+            error_msg = f"blockcount requires a positive integer"
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(error_msg)
             raise GremlinParameterError(error_msg)
         self._blockcount = _blockcount
 
     @property
     def mode(self):
         return self._mode
 
     @mode.setter
     def mode(self, _mode=None):
         if not (isinstance(_mode, str) and _mode.lower() in self._allowed_modes):
-            error_msg = f'mode needs to be one of {str(self._allowed_modes)[1:-2]}'
+            error_msg = f"mode needs to be one of {str(self._allowed_modes)[1:-2]}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._mode = _mode.lower()
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-c', str(self.blockcount)])
-        model['args'].extend(['-d', self.directory])
-        model['args'].extend(['-m', self.mode])
-        model['args'].extend(['-s', str(self.blocksize)])
-        model['args'].extend(['-w', str(self.workers)])
+        model["args"].extend(["-c", str(self.blockcount)])
+        model["args"].extend(["-d", self.directory])
+        model["args"].extend(["-m", self.mode])
+        model["args"].extend(["-s", str(self.blocksize)])
+        model["args"].extend(["-w", str(self.workers)])
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-c', str(self.blockcount)])
     #     model['args'].extend(['-d', self.directory])
     #     model['args'].extend(['-m', self.mode])
@@ -1131,152 +1165,152 @@
     #     model['args'].extend(['-w', str(self.workers)])
     #     return json.dumps(model)
 
 
 class GremlinShutdownAttack(GremlinStateAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'shutdown'
+        self.shortType = "shutdown"
         self._delay = 1
         self._reboot = False
-        self.delay = kwargs.get('delay', 1)        # -d, int
-        self.reboot = kwargs.get('reboot', False)  # -r
+        self.delay = kwargs.get("delay", 1)  # -d, int
+        self.reboot = kwargs.get("reboot", False)  # -r
 
     @property
     def delay(self):
         return self._delay
 
     @delay.setter
     def delay(self, _delay=None):
         if not (isinstance(_delay, int) and _delay >= 1):
-            error_msg = f'delay expects a positive {type(int)}'
+            error_msg = f"delay expects a positive {type(int)}"
             log.fatal(error_msg)
-            raise GremlinParameterError (error_msg)
+            raise GremlinParameterError(error_msg)
         self._delay = _delay
 
     @property
     def reboot(self):
         return self._reboot
 
     @reboot.setter
     def reboot(self, _reboot=None):
         if not isinstance(_reboot, bool):
-            error_msg = f'reboot expects a {type(bool)}'
+            error_msg = f"reboot expects a {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._reboot = _reboot
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'] = ['-d', str(self.delay)]
+        model["args"] = ["-d", str(self.delay)]
         if self.reboot:
-            model['args'].append('-r')
+            model["args"].append("-r")
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'] = ['-d', str(self.delay)]
     #     if self.reboot:
     #         model['args'].append('-r')
     #     return json.dumps(model)
 
 
 class GremlinProcessKillerAttack(GremlinStateAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'process_killer'
+        self.shortType = "process_killer"
         self._exact = False
         self._full_match = False
         self._group = str()
         self._interval = 1
         self._kill_children = False
         self._process = str()
         self._target_newest = False
         self._target_oldest = False
         self._user = str()
-        self.exact = kwargs.get('exact', False)                   # -e
-        self.full_match = kwargs.get('full_match', False)         # -f
-        self.group = kwargs.get('group', str())                   # -g, str
-        self.interval = kwargs.get('interval', 1)                 # -i, int
-        self.kill_children = kwargs.get('kill_children', False)   # -c
-        self.process = kwargs.get('process', str())               # -p, str
-        self.target_newest = kwargs.get('target_newest', False)   # -n
-        self._target_oldest = kwargs.get('target_oldest', False)  # -o
-        self.user = kwargs.get('user', str())                     # -p, str
+        self.exact = kwargs.get("exact", False)  # -e
+        self.full_match = kwargs.get("full_match", False)  # -f
+        self.group = kwargs.get("group", str())  # -g, str
+        self.interval = kwargs.get("interval", 1)  # -i, int
+        self.kill_children = kwargs.get("kill_children", False)  # -c
+        self.process = kwargs.get("process", str())  # -p, str
+        self.target_newest = kwargs.get("target_newest", False)  # -n
+        self._target_oldest = kwargs.get("target_oldest", False)  # -o
+        self.user = kwargs.get("user", str())  # -p, str
 
     @property
     def exact(self):
         return self._exact
 
     @exact.setter
     def exact(self, _exact=None):
         if not isinstance(_exact, bool):
-            error_msg = f'exact expects type {type(bool)}'
+            error_msg = f"exact expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._exact = _exact
 
     @property
     def full_match(self):
         return self._full_match
 
     @full_match.setter
     def full_match(self, _full_match=None):
         if not _full_match:
             self._full_match = False
         elif not isinstance(_full_match, bool):
-            error_msg = f'exact expects type {type(bool)}'
+            error_msg = f"exact expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._full_match = True
 
     @property
     def group(self):
         return self._group
 
     @group.setter
     def group(self, _group=None):
         if not isinstance(_group, str):
-            error_msg = f'group expects type {type(str)}'
+            error_msg = f"group expects type {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._group = _group
 
     @property
     def interval(self):
         return self._interval
 
     @interval.setter
     def interval(self, _interval=None):
         if not (isinstance(_interval, int) and _interval >= 1):
-            error_msg = f'group expects positive integer of type {type(int)}'
+            error_msg = f"group expects positive integer of type {type(int)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._interval = _interval
 
     @property
     def kill_children(self):
         return self._kill_children
 
     @kill_children.setter
     def kill_children(self, _kill_children=None):
         if not isinstance(_kill_children, bool):
-            error_msg = f'kill_children expects {type(bool)}'
+            error_msg = f"kill_children expects {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._kill_children = _kill_children
 
     @property
     def process(self):
         return self._process
 
     @process.setter
     def process(self, _process=None):
         if not isinstance(_process, str):
-            error_msg = f'process expects {type(str)}'
+            error_msg = f"process expects {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._process = _process
 
     @property
     def target_newest(self):
         return self._target_newest
@@ -1286,15 +1320,15 @@
         if isinstance(_target_newest, bool):
             if _target_newest == True:
                 self._target_newest = True
                 self._target_oldest = False
             else:
                 self._target_newest = False
         else:
-            error_msg = f'target_newest expects type {type(bool)}'
+            error_msg = f"target_newest expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def target_oldest(self):
         return self._target_oldest
 
@@ -1303,56 +1337,56 @@
         if isinstance(_target_oldest, bool):
             if _target_oldest == True:
                 self._target_oldest = True
                 self._target_newest = False
             else:
                 self.target_oldest = False
         else:
-            error_msg = f'target_oldest expects type {type(bool)}'
+            error_msg = f"target_oldest expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def user(self):
         return self._user
 
     @user.setter
     def user(self, _user=None):
         if not _user:
             self._user = None
         elif isinstance(_user, str):
             self._user = _user
         else:
-            error_msg = f'user expects {type(str)}'
+            error_msg = f"user expects {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-i', str(self.interval)])
+        model["args"].extend(["-i", str(self.interval)])
         if self.group:
-            model['args'].extend(['-g', self.group])
+            model["args"].extend(["-g", self.group])
         if self.process:
-            model['args'].extend(['-p', self.process])
+            model["args"].extend(["-p", self.process])
         else:
-            error_msg = f'process is required to a be a non-empty string'
+            error_msg = f"process is required to a be a non-empty string"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if self.user:
-            model['args'].extend(['-u', self.user])
+            model["args"].extend(["-u", self.user])
         if self.exact:
-            model['args'].append('-e')
+            model["args"].append("-e")
         if self.full_match:
-            model['args'].append('-f')
+            model["args"].append("-f")
         if self.kill_children:
-            model['args'].append('-c')
+            model["args"].append("-c")
         if self.target_newest and not self.target_oldest:
-            model['args'].append('-n')
+            model["args"].append("-n")
         if self.target_oldest and not self.target_newest:
-            model['args'].append('-o')
+            model["args"].append("-o")
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-i', str(self.interval)])
     #     if self.group:
     #         model['args'].extend(['-g', self.group])
@@ -1376,135 +1410,135 @@
     #         model['args'].append('-o')
     #     return json.dumps(model)
 
 
 class GremlinTimeTravelAttack(GremlinStateAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'time_travel'
+        self.shortType = "time_travel"
         self._block_ntp = False
         self._offset = 86400
-        self.block_ntp = kwargs.get('block_ntp', False)  # -n
-        self.offset = kwargs.get('offset', 86400)        # -o, int
+        self.block_ntp = kwargs.get("block_ntp", False)  # -n
+        self.offset = kwargs.get("offset", 86400)  # -o, int
 
     @property
     def block_ntp(self):
         return self._block_ntp
 
     @block_ntp.setter
     def block_ntp(self, _block_ntp=None):
         if not isinstance(_block_ntp, bool):
-            error_msg = f'block_ntp expects type {type(bool)}'
+            error_msg = f"block_ntp expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._block_ntp = _block_ntp
 
     @property
     def offset(self):
         return self._offset
 
     @offset.setter
     def offset(self, offset=None):
         if not isinstance(offset, int):
-            error_msg = f'Offset needs to be an integer, received {type(offset)}'
+            error_msg = f"Offset needs to be an integer, received {type(offset)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._offset = offset
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-o', str(self.offset)])
+        model["args"].extend(["-o", str(self.offset)])
         if self.block_ntp:
-            model['args'].append('-n')
+            model["args"].append("-n")
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-o', str(self.offset)])
     #     if self.block_ntp:
     #         model['args'].append('-n')
     #     return json.dumps(model)
 
 
 class GremlinBlackholeAttack(GremlinNetworkAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'blackhole'
-        self.egress_ports = kwargs.get('egress_ports', ['^53'])       # -p, str
-        self.hostnames = kwargs.get('hostnames', '^api.gremlin.com')  # -h, str
-        self.ingress_ports = kwargs.get('ingress_ports', None)        # -n, str
+        self.shortType = "blackhole"
+        self.egress_ports = kwargs.get("egress_ports", ["^53"])  # -p, str
+        self.hostnames = kwargs.get("hostnames", "^api.gremlin.com")  # -h, str
+        self.ingress_ports = kwargs.get("ingress_ports", None)  # -n, str
 
     def repr_model(self):
         model = super().repr_model()
         if len(self.egress_ports) > 0:
-            model['args'].extend(['-p', ','.join(self.egress_ports)])
+            model["args"].extend(["-p", ",".join(self.egress_ports)])
         if len(self.hostnames) > 0:
-            model['args'].extend(['-h', ','.join(self.hostnames)])
+            model["args"].extend(["-h", ",".join(self.hostnames)])
         if len(self.ingress_ports) > 0:
-            model['args'].extend(['-n', ','.join(self.ingress_ports)])
+            model["args"].extend(["-n", ",".join(self.ingress_ports)])
         return model
 
     def __repr__(self):
         model = json.loads(super().__repr__())
         if len(self.egress_ports) > 0:
-            model['args'].extend(['-p', ','.join(self.egress_ports)])
+            model["args"].extend(["-p", ",".join(self.egress_ports)])
         if len(self.hostnames) > 0:
-            model['args'].extend(['-h', ','.join(self.hostnames)])
+            model["args"].extend(["-h", ",".join(self.hostnames)])
         if len(self.ingress_ports) > 0:
-            model['args'].extend(['-n', ','.join(self.ingress_ports)])
+            model["args"].extend(["-n", ",".join(self.ingress_ports)])
         return json.dumps(model)
 
 
 class GremlinDNSAttack(GremlinNetworkAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'dns'
-        self._allowed_protocols = ['TCP', 'UDP']
-        self.protocol = kwargs.get('protocol', None)
+        self.shortType = "dns"
+        self._allowed_protocols = ["TCP", "UDP"]
+        self.protocol = kwargs.get("protocol", None)
 
     def repr_model(self):
         model = super().repr_model()
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     return json.dumps(model)
 
 
 class GremlinLatencyAttack(GremlinNetworkAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'latency'
+        self.shortType = "latency"
         self._delay = 100
-        self.delay = kwargs.get('delay', 100)                         # -m, int
-        self.egress_ports = kwargs.get('egress_ports', ['^53'])       # -p, str
-        self.hostnames = kwargs.get('hostnames', '^api.gremlin.com')  # -h, str
-        self.source_ports = kwargs.get('source_ports', None)          # -s, str
+        self.delay = kwargs.get("delay", 100)  # -m, int
+        self.egress_ports = kwargs.get("egress_ports", ["^53"])  # -p, str
+        self.hostnames = kwargs.get("hostnames", "^api.gremlin.com")  # -h, str
+        self.source_ports = kwargs.get("source_ports", None)  # -s, str
 
     @property
     def delay(self):
         return self._delay
 
     @delay.setter
     def delay(self, _delay=None):
         if not (isinstance(_delay, int) and _delay >= 1):
-            error_msg = f'delay expects a positive integer type {type(int)}'
+            error_msg = f"delay expects a positive integer type {type(int)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._delay = _delay
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-m', str(self.delay)])
+        model["args"].extend(["-m", str(self.delay)])
         if len(self.egress_ports) > 0:
-            model['args'].extend(['-p', ','.join(self.egress_ports)])
+            model["args"].extend(["-p", ",".join(self.egress_ports)])
         if len(self.hostnames) > 0:
-            model['args'].extend(['-h', ','.join(self.hostnames)])
+            model["args"].extend(["-h", ",".join(self.hostnames)])
         if len(self.source_ports) > 0:
-            model['args'].extend(['-s', ','.join(self.source_ports)])
+            model["args"].extend(["-s", ",".join(self.source_ports)])
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-m', str(self.delay)])
     #     if len(self.egress_ports) > 0:
     #         model['args'].extend(['-p', ','.join(self.egress_ports)])
@@ -1514,69 +1548,70 @@
     #         model['args'].extend(['-s', ','.join(self.source_ports)])
     #     return json.dumps(model)
 
 
 class GremlinPacketLossAttack(GremlinNetworkAttackHelper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.shortType = 'packet_loss'
+        self.shortType = "packet_loss"
         self._corrupt = False
         self._percent = 1
-        self.corrupt = kwargs.get('corrupt', False)                   # -c
-        self.egress_ports = kwargs.get('egress_ports', ['^53'])       # -p, str
-        self.hostnames = kwargs.get('hostnames', '^api.gremlin.com')  # -h, str
-        self.percent = kwargs.get('percent', 1)                       # -r, int
-        self.source_ports = kwargs.get('source_ports', None)          # -s, str
+        self.corrupt = kwargs.get("corrupt", False)  # -c
+        self.egress_ports = kwargs.get("egress_ports", ["^53"])  # -p, str
+        self.hostnames = kwargs.get("hostnames", "^api.gremlin.com")  # -h, str
+        self.percent = kwargs.get("percent", 1)  # -r, int
+        self.source_ports = kwargs.get("source_ports", None)  # -s, str
 
     @property
     def corrupt(self):
         return self._corrupt
 
     @corrupt.setter
     def corrupt(self, _corrupt=None):
         if not _corrupt:
             self._corrupt = False
             return
         if not isinstance(_corrupt, bool):
-            error_msg = f'corrupt expects type {type(bool)}'
+            error_msg = f"corrupt expects type {type(bool)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._corrupt = _corrupt
 
     @property
     def percent(self):
         return self._percent
 
     @percent.setter
     def percent(self, _percent=None):
         if not (isinstance(_percent, int) and 1 <= _percent <= 100):
-            error_msg = f'percent expects positive integer type {type(int)} between 1 and 100'
+            error_msg = (
+                f"percent expects positive integer type {type(int)} between 1 and 100"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._percent = _percent
 
     def repr_model(self):
         model = super().repr_model()
-        model['args'].extend(['-r', str(self.percent)])
+        model["args"].extend(["-r", str(self.percent)])
         if len(self.egress_ports) > 0:
-            model['args'].extend(['-p', ','.join(self.egress_ports)])
+            model["args"].extend(["-p", ",".join(self.egress_ports)])
         if len(self.hostnames) > 0:
-            model['args'].extend(['-h', ','.join(self.hostnames)])
+            model["args"].extend(["-h", ",".join(self.hostnames)])
         if len(self.source_ports) > 0:
-            model['args'].extend(['-s', ','.join(self.source_ports)])
+            model["args"].extend(["-s", ",".join(self.source_ports)])
         if self.corrupt:
-            model['args'].append('-c')
+            model["args"].append("-c")
         return model
 
     # def __repr__(self):
     #     model = json.loads(super().__repr__())
     #     model['args'].extend(['-r', str(self.percent)])
     #     if len(self.egress_ports) > 0:
     #         model['args'].extend(['-p', ','.join(self.egress_ports)])
     #     if len(self.hostnames) > 0:
     #         model['args'].extend(['-h', ','.join(self.hostnames)])
     #     if len(self.source_ports) > 0:
     #         model['args'].extend(['-s', ','.join(self.source_ports)])
     #     if self.corrupt:
     #         model['args'].append('-c')
     #     return json.dumps(model)
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/attacks.py` & `gremlinapi-0.9.7/gremlinapi/attacks.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,122 +7,126 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.attack_helpers import GremlinAttackHelper
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIAttacks(GremlinAPI):
     @classmethod
     def _list_endpoint(cls, endpoint, *args, **kwargs):
         if not endpoint:
-            error_msg = f'endpoint not passed correctly: {args} :: {kwargs}'
+            error_msg = f"endpoint not passed correctly: {args} :: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        source = cls._info_if_not_param('source', **kwargs)
-        page_size = cls._info_if_not_param('pageSize', **kwargs)
+        source = cls._info_if_not_param("source", **kwargs)
+        page_size = cls._info_if_not_param("pageSize", **kwargs)
         if source or page_size:
-            endpoint += '/?'
-            if source and (source.lower() == 'adhoc' or source.lower() == 'scenario'):
-                endpoint += f'source={source}&'
+            endpoint += "/?"
+            if source and (source.lower() == "adhoc" or source.lower() == "scenario"):
+                endpoint += f"source={source}&"
             if page_size and isinstance(page_size, int):
-                endpoint += f'pageSize={page_size}&'
+                endpoint += f"pageSize={page_size}&"
         return cls._optional_team_endpoint(endpoint, **kwargs)
 
     @classmethod
     def _error_if_not_attack_body(cls, **kwargs):
-        body = cls._error_if_not_param('body', **kwargs)
+        body = cls._error_if_not_param("body", **kwargs)
         if issubclass(type(body), GremlinAttackHelper):
             return str(body)
         else:
-            error_msg = f'Body present but not of type {type(GremlinAttackHelper)}'
+            error_msg = f"Body present but not of type {type(GremlinAttackHelper)}"
             log.warning(error_msg)
         return body
 
     @classmethod
-    @register_cli_action('create_attack', ('body',), ('teamId',))
+    @register_cli_action("create_attack", ("body",), ("teamId",))
     def create_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = cls._error_if_not_attack_body(**kwargs)
-        endpoint = cls._optional_team_endpoint('/attacks/new', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint("/attacks/new", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_attacks', ('',), ('source', 'pageSize', 'teamId'))
-    def list_active_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._list_endpoint('/attacks/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_active_attacks", ("",), ("source", "pageSize", "teamId"))
+    def list_active_attacks(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._list_endpoint("/attacks/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_attacks', ('',), ('source', 'pageSize', 'teamId'))
+    @register_cli_action("list_attacks", ("",), ("source", "pageSize", "teamId"))
     def list_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
         """
         :param https_client:
         :param kwargs: { source(adhoc or scenario, query), pageSize(int32, query), teamId(string, query) }
         :return:
         """
-        method = 'GET'
-        endpoint = cls._list_endpoint('/attacks', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._list_endpoint("/attacks", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
-
     @classmethod
-    @register_cli_action('list_complete_attacks', ('',), ('source', 'pageSize', 'teamId'))
-    def list_completed_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+    @register_cli_action(
+        "list_complete_attacks", ("",), ("source", "pageSize", "teamId")
+    )
+    def list_completed_attacks(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
         """
         :param https_client:
         :param kwargs: { source(adhoc or scenario, query), pageSize(int32, query), teamId(string, query) }
         :return:
         """
-        method = 'GET'
-        endpoint = cls._list_endpoint('/attacks/completed', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._list_endpoint("/attacks/completed", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_attack', ('guid',), ('teamId',))
+    @register_cli_action("get_attack", ("guid",), ("teamId",))
     def get_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/attacks/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/attacks/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_all_attacks', ('',), ('teamId',))
+    @register_cli_action("halt_all_attacks", ("",), ("teamId",))
     def halt_all_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        endpoint = cls._optional_team_endpoint('/attacks', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        endpoint = cls._optional_team_endpoint("/attacks", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_attack', ('guid',), ('teamId',))
+    @register_cli_action("halt_attack", ("guid",), ("teamId",))
     def halt_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/attacks/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/attacks/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/cli.py` & `gremlinapi-0.9.7/gremlinapi/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,151 +8,189 @@
 import logging
 import os
 import sys
 
 from gremlinapi.config import GremlinAPIConfig
 from gremlinapi.exceptions import GremlinAuthError
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 cli_actions = dict()
 
+
 def register_cli_action(cls_names, required=tuple(), optional=tuple()):
     def wrap(f):
         @functools.wraps(f)
         def wrapped_f(*args, **kwargs):
             return f(*args, **kwargs)
 
         in_obj = True
         classes = cls_names
         if type(classes) != tuple:
             classes = (classes,)
 
         for cls_name in classes:
             if cls_name not in cli_actions:
                 cli_actions[cls_name] = {}
-            action = f.__name__.replace("_","-")
+            action = f.__name__.replace("_", "-")
             cli_actions[cls_name][action] = (required, optional, in_obj)
 
         return wrapped_f
+
     return wrap
 
+
 def _base_args():
     p = argparse.ArgumentParser(description="Gremlin API Command Line Interface")
-    p.add_argument("--version",
-                   help="Display the version.",
-                   type=bool,
-                   action="store",
-                   dest="version",
-                   default=False)
-    p.add_argument("-v", "--verbose",
-                   help="Verbose Mode",
-                   type=bool,
-                   action="store",
-                   dest="verbose",
-                   default=False)
-    p.add_argument("-d", "--debug",
-                   help="Debug mode (may expose authentication credentials to logs!)",
-                   type=bool,
-                   action="store",
-                   dest="debug",
-                   default=False)
-    auth = p.add_argument_group('Authentication Configuration Options')
-    auth.add_argument("-a", "--apikey",
-                      help="User provided API key",
-                      type=str,
-                      action="store",
-                      dest="gremlin_api_key",
-                      default=os.getenv('GREMLIN_API_KEY', None))
-    auth.add_argument("-b", "--bearer",
-                      help="User provided bearer token",
-                      type=str,
-                      action="store",
-                      dest="gremlin_bearer",
-                      default=os.getenv('GREMLIN_BEARER_TOKEN', None))
-    auth.add_argument("-i", "--bearer-interval",
-                      help="Maximum bearer token age in seconds if using login methods",
-                      type=int,
-                      action="store",
-                      dest="max_bearer_interval",
-                      default=os.getenv('GREMLIN_MAX_BEARER_INTERVAL', 86400))
-    auth.add_argument("-u", "--user",
-                      help="Gremlin user (email) to use for login functions",
-                      type=str,
-                      dest="gremlin_user",
-                      default=os.getenv('GREMLIN_USER', ''))
-    auth.add_argument("-p", "--password",
-                      help="Password to use for login functions (will be exposed in logs if debug mode is enabled!)",
-                      type=str,
-                      action="store",
-                      dest="gremlin_password",
-                      default=os.getenv('GREMLIN_PASSWORD', ''))
-    auth.add_argument("-m", "--mfa",
-                      help="MFA OTP Token for login functions",
-                      type=int,
-                      action="store",
-                      dest="gremlin_user_mfa_token",
-                      default=os.getenv('GREMLIN_USER_MFA_TOKEN', None))
-    auth.add_argument("-c", "--company",
-                      help="Company Name, as it appears in the Gremlin UI or API, for user login functions",
-                      type=str,
-                      action="store",
-                      dest="gremlin_company",
-                      default=os.getenv('GREMLIN_COMPANY', ''))
-    auth.add_argument("-t", "--team_id",
-                      help="Gremlin Team ID, required for RBAC enabled accounts",
-                      type=str,
-                      action="store",
-                      dest="gremlin_team_id",
-                      default=os.getenv('GREMLIN_TEAM_ID', ''))
+    p.add_argument(
+        "--version",
+        help="Display the version.",
+        type=bool,
+        action="store",
+        dest="version",
+        default=False,
+    )
+    p.add_argument(
+        "-v",
+        "--verbose",
+        help="Verbose Mode",
+        type=bool,
+        action="store",
+        dest="verbose",
+        default=False,
+    )
+    p.add_argument(
+        "-d",
+        "--debug",
+        help="Debug mode (may expose authentication credentials to logs!)",
+        type=bool,
+        action="store",
+        dest="debug",
+        default=False,
+    )
+    auth = p.add_argument_group("Authentication Configuration Options")
+    auth.add_argument(
+        "-a",
+        "--apikey",
+        help="User provided API key",
+        type=str,
+        action="store",
+        dest="gremlin_api_key",
+        default=os.getenv("GREMLIN_API_KEY", None),
+    )
+    auth.add_argument(
+        "-b",
+        "--bearer",
+        help="User provided bearer token",
+        type=str,
+        action="store",
+        dest="gremlin_bearer",
+        default=os.getenv("GREMLIN_BEARER_TOKEN", None),
+    )
+    auth.add_argument(
+        "-i",
+        "--bearer-interval",
+        help="Maximum bearer token age in seconds if using login methods",
+        type=int,
+        action="store",
+        dest="max_bearer_interval",
+        default=os.getenv("GREMLIN_MAX_BEARER_INTERVAL", 86400),
+    )
+    auth.add_argument(
+        "-u",
+        "--user",
+        help="Gremlin user (email) to use for login functions",
+        type=str,
+        dest="gremlin_user",
+        default=os.getenv("GREMLIN_USER", ""),
+    )
+    auth.add_argument(
+        "-p",
+        "--password",
+        help="Password to use for login functions (will be exposed in logs if debug mode is enabled!)",
+        type=str,
+        action="store",
+        dest="gremlin_password",
+        default=os.getenv("GREMLIN_PASSWORD", ""),
+    )
+    auth.add_argument(
+        "-m",
+        "--mfa",
+        help="MFA OTP Token for login functions",
+        type=int,
+        action="store",
+        dest="gremlin_user_mfa_token",
+        default=os.getenv("GREMLIN_USER_MFA_TOKEN", None),
+    )
+    auth.add_argument(
+        "-c",
+        "--company",
+        help="Company Name, as it appears in the Gremlin UI or API, for user login functions",
+        type=str,
+        action="store",
+        dest="gremlin_company",
+        default=os.getenv("GREMLIN_COMPANY", ""),
+    )
+    auth.add_argument(
+        "-t",
+        "--team_id",
+        help="Gremlin Team ID, required for RBAC enabled accounts",
+        type=str,
+        action="store",
+        dest="gremlin_team_id",
+        default=os.getenv("GREMLIN_TEAM_ID", ""),
+    )
     return p
 
+
 def _get_parser(cli_module):
     parser = _base_args()
     return cli_module.extend_parser(parser)
 
+
 def _parse_args():
     parser = _base_args()
-    #args = parser.parse_known_args(sys.argv[1:])
+    # args = parser.parse_known_args(sys.argv[1:])
     (options, args) = parser.parse_known_args(sys.argv)
-    cli_module = importlib.import_module('gremlinapi.cli.cli')
+    cli_module = importlib.import_module("gremlinapi.cli.cli")
     parser = _get_parser(cli_module)
     try:
         import argcomplete
+
         argcomplete.autocomplete(parser)
     except Exception:
         pass
     # Sanity check input
     try:
-        if not (args.gremlin_user and args.gremlin_password) and not (args.gremlin_bearer or args.gremlin_api_key):
-            error_msg = f'No form of API authentication provided: {args}'
+        if not (args.gremlin_user and args.gremlin_password) and not (
+            args.gremlin_bearer or args.gremlin_api_key
+        ):
+            error_msg = f"No form of API authentication provided: {args}"
             log.fatal(error_msg)
             raise GremlinAuthError(error_msg)
         elif args.gremlin_api_key:
-            log.debug(f'API authentication supplied: key {args.gremlin_api_key}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"API authentication supplied: key {args.gremlin_api_key}")
         elif args.bearer:
-            log.debug(f'Bearer supplied at CLI runtime: {args.bearer}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"Bearer supplied at CLI runtime: {args.bearer}")
             GremlinAPIConfig.bearer_token = args.bearer
         elif args.gremlin_user and args.gremlin_password:
-            log.debug(f'User authentication provided for user: {args.gremlin_user}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"User authentication provided for user: {args.gremlin_user}")
             GremlinAPIConfig.user = args.gremlin_user
             GremlinAPIConfig.password = args.gremlin_password
             if args.gremlin_user_mfa_token:
-                log.debug(f'MFA token provided for user {args.gremlin_user}')
+                if log.getEffectiveLevel() == logging.DEBUG:
+                    log.debug(f"MFA token provided for user {args.gremlin_user}")
                 GremlinAPIConfig.user_mfa_token_value = args.gremlin_user_mfa_token
         else:
-            error_msg = f'Unexpected state, authentication logic fallthrough: {args}'
+            error_msg = f"Unexpected state, authentication logic fallthrough: {args}"
             log.fatal(error_msg)
             raise GremlinAuthError(error_msg)
     except GremlinAuthError:
         parser.print_help()
 
 
 def main():
     _parse_args()
-
-
-
-
-
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/clients.py` & `gremlinapi-0.9.7/gremlinapi/clients.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,56 +6,55 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIClients(GremlinAPI):
-
     @classmethod
-    @register_cli_action('activate_client', ('guid',), ('teamId',))
+    @register_cli_action("activate_client", ("guid",), ("teamId",))
     def activate_client(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'PUT'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/clients/{guid}/activate', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "PUT"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/clients/{guid}/activate", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('deactivate_client', ('guid',), ('teamId',))
+    @register_cli_action("deactivate_client", ("guid",), ("teamId",))
     def deactivate_client(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/clients/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/clients/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_clients', ('',), ('teamId',))
+    @register_cli_action("list_active_clients", ("",), ("teamId",))
     def list_active_clients(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/clients/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/clients/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_clients', ('',), ('teamId',))
+    @register_cli_action("list_clients", ("",), ("teamId",))
     def list_clients(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/clients', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/clients", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
-        return body
+        return body
```

### Comparing `gremlinapi-0.9.2/gremlinapi/companies.py` & `gremlinapi-0.9.7/gremlinapi/companies.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,155 +6,186 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPICompanies(GremlinAPI):
-
     @classmethod
-    @register_cli_action('get_company', ('identifier',), ('',))
+    @register_cli_action("get_company", ("identifier",), ("",))
     def get_company(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        endpoint = f'/companies/{identifier}'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        endpoint = f"/companies/{identifier}"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_company_clients', ('identifier',), ('',))
+    @register_cli_action("list_company_clients", ("identifier",), ("",))
     def list_company_clients(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        endpoint = f'/companies/{identifier}/clients'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        endpoint = f"/companies/{identifier}/clients"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('invite_company_user', ('identifier', 'body'), ('',))
+    @register_cli_action("invite_company_user", ("identifier", "body"), ("",))
     def invite_company_user(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "POST"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
         if isinstance(data, dict):
             data = [dict(data)]
-        endpoint = f'/companies/{identifier}/invites'
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = f"/companies/{identifier}/invites"
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_company_invite', ('identifier', 'email'), ('',))
+    @register_cli_action("delete_company_invite", ("identifier", "email"), ("",))
     def delete_company_invite(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'DELETE'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "DELETE"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         email = cls._error_if_not_email(**kwargs)
-        endpoint = f'/companies/{identifier}/invites/{email}'
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = f"/companies/{identifier}/invites/{email}"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('company_mfa_prefs', ('identifier',), ('forceMfa', 'mfaProviders', 'defaultMfaProvider',))
+    @register_cli_action(
+        "company_mfa_prefs",
+        ("identifier",),
+        (
+            "forceMfa",
+            "mfaProviders",
+            "defaultMfaProvider",
+        ),
+    )
     def company_mfa_prefs(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "POST"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         data = {
-            'forceMfa': cls._info_if_not_param('forceMfa', **kwargs),
-            'mfaProviders': cls._info_if_not_param('mfaProviders', **kwargs),
-            'defaultMfaProvider': cls._info_if_not_param('defaultMfaProvider', **kwargs)
+            "forceMfa": cls._info_if_not_param("forceMfa", **kwargs),
+            "mfaProviders": cls._info_if_not_param("mfaProviders", **kwargs),
+            "defaultMfaProvider": cls._info_if_not_param(
+                "defaultMfaProvider", **kwargs
+            ),
         }
         data = {k: v for k, v in data.items() if v is not None}
-        endpoint = f'/companies/{identifier}/mfaPrefs'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        endpoint = f"/companies/{identifier}/mfaPrefs"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_company_prefs', ('identifier',), ('domain',))
+    @register_cli_action("update_company_prefs", ("identifier",), ("domain",))
     def update_company_prefs(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        data = {'domain': cls._info_if_not_param('domain', **kwargs)}
+        method = "POST"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        data = {"domain": cls._info_if_not_param("domain", **kwargs)}
         data = {k: v for k, v in data.items() if v is not None}
-        endpoint = f'/companies/{identifier}/prefs'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        endpoint = f"/companies/{identifier}/prefs"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_company_saml_props',
-                         ('identifier',),
-                         ('enabled', 'entityId', 'idpUrl', 'certificate', 'forced'))
+    @register_cli_action(
+        "update_company_saml_props",
+        ("identifier",),
+        ("enabled", "entityId", "idpUrl", "certificate", "forced"),
+    )
     def update_company_saml_props(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "POST"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         data = {
-            'enabled': cls._info_if_not_param('enabled', **kwargs),
-            'entityId': cls._info_if_not_param('entityId', **kwargs),
-            'idpUrl': cls._info_if_not_param('idpUrl', **kwargs),
-            'certificate': cls._info_if_not_param('certificate', **kwargs),
-            'forced': cls._info_if_not_param('forced', **kwargs)
+            "enabled": cls._info_if_not_param("enabled", **kwargs),
+            "entityId": cls._info_if_not_param("entityId", **kwargs),
+            "idpUrl": cls._info_if_not_param("idpUrl", **kwargs),
+            "certificate": cls._info_if_not_param("certificate", **kwargs),
+            "forced": cls._info_if_not_param("forced", **kwargs),
         }
         data = {k: v for k, v in data.items() if v is not None}
-        endpoint = f'/companies/{identifier}/saml/props'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        endpoint = f"/companies/{identifier}/saml/props"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_company_users', ('identifier',), ('',))
+    @register_cli_action("list_company_users", ("identifier",), ("",))
     def list_company_users(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        endpoint = f'/companies/{identifier}/users'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        endpoint = f"/companies/{identifier}/users"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_company_users', ('identifier', 'email',), ('body',))
+    @register_cli_action(
+        "list_company_users",
+        (
+            "identifier",
+            "email",
+        ),
+        ("body",),
+    )
     def update_company_user_role(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'PUT'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "PUT"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         email = cls._error_if_not_email(**kwargs)
         data = cls._warn_if_not_json_body(**kwargs)
-        endpoint = f'​/companies​/{identifier}​/users​/{email}'
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = f"​/companies​/{identifier}​/users​/{email}"
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('activate_company_user', ('identifier', 'email',), ('',))
+    @register_cli_action(
+        "activate_company_user",
+        (
+            "identifier",
+            "email",
+        ),
+        ("",),
+    )
     def activate_company_user(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "POST"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         email = cls._error_if_not_email(**kwargs)
-        endpoint = f'​/companies​/{identifier}​/users​/{email}​/active'
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = f"​/companies​/{identifier}​/users​/{email}​/active"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('deactivate_company_user', ('identifier', 'email',), ('',))
+    @register_cli_action(
+        "deactivate_company_user",
+        (
+            "identifier",
+            "email",
+        ),
+        ("",),
+    )
     def deactivate_company_user(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'DELETE'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "DELETE"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         email = cls._error_if_not_email(**kwargs)
-        endpoint = f'​/companies​/{identifier}​/users​/{email}​/active'
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = f"​/companies​/{identifier}​/users​/{email}​/active"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/config.py` & `gremlinapi-0.9.7/gremlinapi/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 # Copyright (C) 2020 Kyle Hultman <kyle@gremlin.com>, Gremlin Inc <sales@gremlin.com>
 
 
 import logging
 
 from datetime import datetime, timezone
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIConfig(object):
-
     def __init__(self):
         self._api_key = None
         self._base_uri = None
         self._bearer_expires = None
         self._bearer_timestamp = None
         self._bearer_token = None
         self._company_name = None
@@ -155,8 +154,8 @@
     @classmethod
     def is_bearer_expired(cls) -> bool:
         """
         Built-in to let the user check in the bearer token is expired
         Primarily used by the login function
         :return: bool
         """
-        return datetime.now(timezone.utc) >= cls.bearer_expires
+        return datetime.now(timezone.utc) >= cls.bearer_expires
```

### Comparing `gremlinapi-0.9.2/gremlinapi/containers.py` & `gremlinapi-0.9.7/gremlinapi/containers.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,26 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIContainers(GremlinAPI):
-
     @classmethod
-    @register_cli_action('list_containers', ('',), ('teamId'))
+    @register_cli_action("list_containers", ("",), ("teamId"))
     def list_containers(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/containers', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/containers", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/contracts.py` & `gremlinapi-0.9.7/gremlinapi/contracts.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIContracts(GremlinAPI):
-
     @classmethod
-    @register_cli_action('update_contract', ('identifier', 'body'), ('',))
+    @register_cli_action("update_contract", ("identifier", "body"), ("",))
     def update_contract(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'PATCH'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
+        method = "PATCH"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = f'/companies/{identifier}/contracts/current'
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = f"/companies/{identifier}/contracts/current"
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/exceptions.py` & `gremlinapi-0.9.7/gremlinapi/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 Kyle Hultman <kyle@gremlin.com>, Gremlin Inc <sales@gremlin.com>
 
 import logging
 
 
-
-log = logging.getLogger('GremlinAPI.client')
-
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIException(Exception):
     """
     Base exception class
     """
 
+
 class APIError(GremlinAPIException):
     def __init__(self, message):
         super(APIError, self).__init__(message)
 
+
 class GremlinAuthError(GremlinAPIException):
     def __init__(self, message):
         super(GremlinAuthError, self).__init__(message)
 
+
 class GremlinIdentifierError(GremlinAPIException):
     def __init__(self, message):
         super(GremlinIdentifierError, self).__init__(message)
 
+
 class GremlinParameterError(GremlinAPIException):
     def __init__(self, message):
         super(GremlinParameterError, self).__init__(message)
 
+
 class GremlinCommandTargetError(GremlinAPIException):
     def __init__(self, message):
         super(GremlinCommandTargetError, self).__init__(message)
 
+
 class ProxyError(GremlinAPIException):
     def __init__(self, uri, method, **kwargs):
-        message = f'Error for {method} to {uri}, please verify proxy configuration'
+        message = f"Error for {method} to {uri}, please verify proxy configuration"
         super(ProxyError, self).__init__(message)
 
+
 class ClientError(GremlinAPIException):
     def __init__(self, uri, method, **kwargs):
-        message = f'Error for {method} to {uri}, please check your network configuration'
+        message = (
+            f"Error for {method} to {uri}, please check your network configuration"
+        )
         super(ClientError, self).__init__(message)
 
+
 class HTTPTimeout(GremlinAPIException):
     def __init__(self, uri, method, timeout, **kwargs):
-        message = f'{method} to {uri} timed out after {timeout}'
+        message = f"{method} to {uri} timed out after {timeout}"
         super(HTTPTimeout, self).__init__(message)
 
+
 class HTTPError(GremlinAPIException):
     def __init__(self, status_code=None, reason=None):
-        message = f'Request returned status code {status_code} {reason}'
+        message = f"Request returned status code {status_code} {reason}"
         super(HTTPError, self).__init__(message)
 
+
 class HTTPBadHeader(GremlinAPIException):
     def __init__(self, reason=None):
-        message = f'Failed to create HTTPHeader: {reason}'
+        message = f"Failed to create HTTPHeader: {reason}"
         super(HTTPBadHeader, self).__init__(message)
```

### Comparing `gremlinapi-0.9.2/gremlinapi/executions.py` & `gremlinapi-0.9.7/gremlinapi/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,35 +6,26 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
-class GremlinAPIExecutions(GremlinAPI):
-
-    @classmethod
-    def _optional_taskid_endpoint(cls, endpoint, **kwargs):
-        task_id = cls._info_if_not_param('taskId', **kwargs)
-        if task_id:
-            endpoint += f'/?taskId={task_id}'
-        return cls._optional_team_endpoint(endpoint, **kwargs)
-
+class GremlinAPIMetadata(GremlinAPI):
     @classmethod
-    @register_cli_action('list_executions', ('',), ('taskId', 'teamId'))
-    def list_executions(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_taskid_endpoint('/executions', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_metadata", ("",), ("teamId",))
+    def get_metadata(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/metadata", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/gremlinapi.py` & `gremlinapi-0.9.7/gremlinapi/gremlinapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,141 +10,145 @@
 
 from gremlinapi.exceptions import (
     APIError,
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.http_clients import get_gremlin_httpclient
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPI(object):
     def __init__(self):
         pass
 
     @classmethod
     def _add_query_param(cls, endpoint, param_name, param_value):
         if endpoint and param_name and param_value:
-            if '/?' in endpoint and not str(endpoint).endswith('?'):
-                endpoint += f'&{param_name}={param_value}'
-            elif '/?' in endpoint and (str(endpoint).endswith('?') or str(endpoint).endswith('&')):
-                endpoint += f'{param_name}={param_value}'
-            elif '/?' not in endpoint:
-                endpoint += f'/?{param_name}={param_value}'
+            if "/?" in endpoint and not str(endpoint).endswith("?"):
+                endpoint += f"&{param_name}={param_value}"
+            elif "/?" in endpoint and (
+                str(endpoint).endswith("?") or str(endpoint).endswith("&")
+            ):
+                endpoint += f"{param_name}={param_value}"
+            elif "/?" not in endpoint:
+                endpoint += f"/?{param_name}={param_value}"
         return endpoint
 
     @classmethod
     def _build_query_string_endpoint(cls, endpoint, params, **kwargs):
         if not endpoint:
-            error_msg = 'expected endpoint, received nothing'
+            error_msg = "expected endpoint, received nothing"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if not params or type(params) != type(list()):
-            error_msg = f'Expected list of params, received {type(params)}'
+            error_msg = f"Expected list of params, received {type(params)}"
             log.fatal(error_msg)
-            raise(error_msg)
+            raise (error_msg)
         for param_name in params:
-            endpoint = cls._add_query_param(endpoint, param_name, cls._error_if_not_param(param_name, **kwargs))
+            endpoint = cls._add_query_param(
+                endpoint, param_name, cls._error_if_not_param(param_name, **kwargs)
+            )
         return endpoint
 
     @classmethod
     def _build_query_string_option_team_endpoint(cls, endpoint, params, **kwargs):
         endpoint = cls._build_query_string_endpoint(endpoint, params, **kwargs)
-        if 'teamId' not in params:
+        if "teamId" not in params:
             endpoint = cls._optional_team_endpoint(endpoint, **kwargs)
         return endpoint
 
     @classmethod
     def _build_query_string_required_team_endpoint(cls, endpoint, params, **kwargs):
         endpoint = cls._build_query_string_endpoint(endpoint, params, **kwargs)
-        if 'teamId' not in params:
+        if "teamId" not in params:
             endpoint = cls._required_team_endpoint(endpoint, **kwargs)
         return endpoint
 
     @classmethod
     def _optional_team_endpoint(cls, endpoint, **kwargs):
-        team_id = cls._info_if_not_param('teamId', **kwargs)
+        team_id = cls._info_if_not_param("teamId", **kwargs)
         if not team_id and type(config.team_id) is str:
             team_id = config.team_id
         if team_id:
-            endpoint = cls._add_query_param(endpoint, 'teamId', team_id)
+            endpoint = cls._add_query_param(endpoint, "teamId", team_id)
         return endpoint
 
     @classmethod
     def _required_team_endpoint(cls, endpoint, **kwargs):
-        team_id = cls._warn_if_not_param('teamId', **kwargs)
+        team_id = cls._warn_if_not_param("teamId", **kwargs)
         if not team_id and type(config.team_id) is str:
             team_id = config.team_id
         else:
-            error_msg = f'Endpoint requires a team_id, none supplied'
+            error_msg = f"Endpoint requires a team_id, none supplied"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        endpoint = cls._add_query_param(endpoint, 'teamId', team_id)
+        endpoint = cls._add_query_param(endpoint, "teamId", team_id)
 
     @classmethod
     def _error_if_not_json_body(cls, **kwargs):
         body = cls._warn_if_not_json_body(**kwargs)
         if not body:
-            error_msg = f'JSON Body not supplied: {kwargs}'
+            error_msg = f"JSON Body not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return body
 
     @classmethod
     def _error_if_not_email(cls, **kwargs):
-        email = cls._info_if_not_param('email', **kwargs)
+        email = cls._info_if_not_param("email", **kwargs)
         if not email:
-            error_msg = f'email address not passed: {kwargs}'
+            error_msg = f"email address not passed: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         # Do some email regex validation here...
         return email
 
     @classmethod
     def _error_if_not_param(cls, parameter_name, **kwargs):
         param = cls._info_if_not_param(parameter_name, **kwargs)
         if not param:
-            error_msg = f'{parameter_name} not supplied: {kwargs}'
+            error_msg = f"{parameter_name} not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return param
 
     @classmethod
     def _info_if_not_param(cls, parameter_name, default=None, **kwargs):
         param = kwargs.get(parameter_name, None)
         if param is None:
-            error_msg = f'{parameter_name} not found in arguments: {kwargs}'
+            error_msg = f"{parameter_name} not found in arguments: {kwargs}"
             log.info(error_msg)
             param = default
         return param
 
     @classmethod
     def _payload(cls, **kwargs):
-        headers = kwargs.get('headers', None)
-        body = kwargs.get('body', None)
-        data = kwargs.get('data', None)
-        payload = {'headers': headers, 'data': data, 'body': body}
+        headers = kwargs.get("headers", None)
+        body = kwargs.get("body", None)
+        data = kwargs.get("data", None)
+        payload = {"headers": headers, "data": data, "body": body}
         payload = {k: v for k, v in payload.items() if v is not None}
         return payload
 
     @classmethod
     def _warn_if_not_json_body(cls, **kwargs):
-        body = cls._info_if_not_param('body', **kwargs)
+        body = cls._info_if_not_param("body", **kwargs)
         if not body:
-            error_msg = f'JSON Body not supplied: {kwargs}'
+            error_msg = f"JSON Body not supplied: {kwargs}"
             log.warning(error_msg)
         # Do some json validation
         return body
 
     @classmethod
     def _warn_if_not_param(cls, parameter_name, default=None, **kwargs):
         param = cls._info_if_not_param(parameter_name, **kwargs)
         if not param:
-            error_msg = f'{parameter_name} not found in arguments: {kwargs}'
+            error_msg = f"{parameter_name} not found in arguments: {kwargs}"
             log.warning(error_msg)
             param = default
         return param
```

### Comparing `gremlinapi-0.9.2/gremlinapi/halts.py` & `gremlinapi-0.9.7/gremlinapi/halts.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,30 +6,27 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
-
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIHalts(GremlinAPI):
-
     @classmethod
-    @register_cli_action('halt_all_attacks', ('',), ('teamId', 'body'))
+    @register_cli_action("halt_all_attacks", ("",), ("teamId", "body"))
     def halt_all_attacks(cls, https_client=get_gremlin_httpclient(), **kwargs):
-        method = 'POST'
+        method = "POST"
         data = cls._warn_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint('/halts', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint("/halts", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/http_clients.py` & `gremlinapi-0.9.7/gremlinapi/http_clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,86 +6,86 @@
 import logging
 
 from gremlinapi.exceptions import (
     ProxyError,
     ClientError,
     HTTPTimeout,
     HTTPError,
-    HTTPBadHeader
+    HTTPBadHeader,
 )
 
 from gremlinapi.config import GremlinAPIConfig
 from gremlinapi.util import get_version
 
 try:
     import requests
     import requests.adapters
 except ImportError:
     requests = None
     import urllib3
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIHttpClient(object):
     @classmethod
     def api_call(cls, method, uri, *args, **kwargs):
-        error_message = f'This function is not implemented, please consume the proper http library for your environment'
+        error_message = f"This function is not implemented, please consume the proper http library for your environment"
         log.fatal(error_message)
         raise NotImplementedError(error_message)
 
     @classmethod
     def base_uri(cls, uri):
-        if not uri.startswith('http') and GremlinAPIConfig.base_uri not in uri:
-            uri = f'{GremlinAPIConfig.base_uri}{uri}'
+        if not uri.startswith("http") and GremlinAPIConfig.base_uri not in uri:
+            uri = f"{GremlinAPIConfig.base_uri}{uri}"
         return uri
 
     @classmethod
     def header(cls, *args, **kwargs):
-        api_key = kwargs.get('api_key', None)
-        bearer_token = kwargs.get('bearer_token', None)
+        api_key = kwargs.get("api_key", None)
+        bearer_token = kwargs.get("bearer_token", None)
         header = dict()
         if not (api_key and bearer_token):
             if GremlinAPIConfig.bearer_token:
                 bearer_token = GremlinAPIConfig.bearer_token
             if GremlinAPIConfig.api_key:
                 api_key = GremlinAPIConfig.api_key
         if api_key and not bearer_token:
             if "Key" in api_key:
-                header['Authorization'] = api_key
+                header["Authorization"] = api_key
             else:
-                header['Authorization'] = f'Key {api_key}'
+                header["Authorization"] = f"Key {api_key}"
         elif bearer_token:
             if "Bearer" in bearer_token:
-                header['Authorization'] = bearer_token
+                header["Authorization"] = bearer_token
             else:
-                header['Authorization'] = f'Bearer {bearer_token}'
+                header["Authorization"] = f"Bearer {bearer_token}"
         else:
-            error_msg = f'Missing API Key or Bearer Token, none supplied: {api_key}, {bearer_token}'
+            error_msg = f"Missing API Key or Bearer Token, none supplied: {api_key}, {bearer_token}"
             log.fatal(error_msg)
             # raise HTTPBadHeader(error_msg)
-        header['X-Gremlin-Agent'] = f'gremlin-sdk-python/{get_version()}'
+        header["X-Gremlin-Agent"] = f"gremlin-sdk-python/{get_version()}"
         return header
 
     @classmethod
     def proxies(cls):
-        error_message = f'This function is not implemented, please consume the proper http library for your environment'
+        error_message = f"This function is not implemented, please consume the proper http library for your environment"
         log.fatal(error_message)
         raise NotImplementedError(error_message)
 
 
 class GremlineAPIRequestsClient(GremlinAPIHttpClient):
     @classmethod
     def proxies(cls):
         proxies = dict()
 
         if GremlinAPIConfig.http_proxy and type(GremlinAPIConfig.http_proxy) is str:
-            proxies['http'] = GremlinAPIConfig.http_proxy
+            proxies["http"] = GremlinAPIConfig.http_proxy
         if GremlinAPIConfig.https_proxy and type(GremlinAPIConfig.https_proxy) is str:
-            proxies['https'] = GremlinAPIConfig.https_proxy
+            proxies["https"] = GremlinAPIConfig.https_proxy
 
         return proxies
 
     @classmethod
     def api_call(cls, method, endpoint, *args, **kwargs):
 
         request_methods = {
@@ -98,94 +98,103 @@
         }
 
         # uri = f'{GremlinAPIConfig.base_uri}{endpoint}'
         uri = cls.base_uri(endpoint)
         client = request_methods.get(method.upper())
         raw_content = kwargs.pop("raw_content", False)
         data = None
-        if 'data' in kwargs:
-            data = kwargs.pop('data')
-        elif 'body' in kwargs:
+        if "data" in kwargs:
+            data = kwargs.pop("data")
+        elif "body" in kwargs:
             if "Content-Type" not in kwargs["headers"]:
                 kwargs["headers"]["Content-Type"] = "application/json"
-            data = kwargs.pop('body')
+            data = kwargs.pop("body")
             if not isinstance(data, str):
                 data = json.dumps(data)
-            log.debug(f'body: {data}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"body: {data}")
 
-        kwargs['proxies'] = cls.proxies()
-        log.debug(f'httpd client kwargs: {kwargs}')
+        kwargs["proxies"] = cls.proxies()
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(f"httpd client kwargs: {kwargs}")
 
         if data:
             resp = client(uri, data=data, allow_redirects=False, **kwargs)
         else:
             resp = client(uri, allow_redirects=False, **kwargs)
 
         if resp.status_code >= 400:
-            error_msg = f'error {resp.status_code} : {resp.reason}'
+            error_msg = f"error {resp.status_code} : {resp.reason}"
             log.warning(error_msg)
-            log.debug(f'{client}\n{uri}\n{data}\n{kwargs}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(f"{client}\n{uri}\n{data}\n{kwargs}")
             raise HTTPError(error_msg)
 
         if raw_content:
             body = resp.content
         else:
             try:
                 body = resp.json()
             except ValueError:
                 # No JSON in response
                 try:
                     body = str(resp.content, resp.encoding)
                 except TypeError:
                     # Response must be empty, return something nice
-                    body = 'Success'
+                    body = "Success"
 
         return resp, body
 
 
 class GremlinAPIurllibClient(GremlinAPIHttpClient):
     """Fallback library in the event requests library is unavailable."""
+
     @classmethod
     def api_call(cls, method, endpoint, *args, **kwargs):
 
-        log.warning(f'The request to {endpoint} is using the urllib3 library. Consider installing th requests library.')
+        log.warning(
+            f"The request to {endpoint} is using the urllib3 library. Consider installing th requests library."
+        )
         form_data = None
         request_body = None
 
-        if 'data' in kwargs:
-            form_data = kwargs.pop('data')
-        elif 'body' in kwargs:
+        if "data" in kwargs:
+            form_data = kwargs.pop("data")
+        elif "body" in kwargs:
             if "Content-Type" not in kwargs["headers"]:
                 kwargs["headers"]["Content-Type"] = "application/json"
             request_body = json.dumps(kwargs.pop("body"))
 
-        uri = f'{GremlinAPIConfig.base_uri}{endpoint}'
+        uri = f"{GremlinAPIConfig.base_uri}{endpoint}"
 
         if GremlinAPIConfig.https_proxy and type(GremlinAPIConfig.https_proxy) is str:
             http_client = urllib3.ProxyManager(GremlinAPIConfig.https_proxy)
         elif GremlinAPIConfig.http_proxy and type(GremlinAPIConfig.http_proxy) is str:
             http_client = urllib3.ProxyManager(GremlinAPIConfig.http_proxy)
         else:
             http_client = urllib3.PoolManager()
 
         if form_data:
             resp = http_client.request(method, uri, fields=form_data, **kwargs)
         elif request_body:
             resp = http_client.request(method, uri, body=request_body, **kwargs)
         else:
             resp = http_client.request(method, uri, **kwargs)
-        log.debug(resp)
+        if log.getEffectiveLevel() == logging.DEBUG:
+            log.debug(resp)
 
         if resp.status >= 400:
-            log.debug(f'Failed response: {resp.status}\n{http_client}\n{uri}\n{kwargs}\n{resp}')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug(
+                    f"Failed response: {resp.status}\n{http_client}\n{uri}\n{kwargs}\n{resp}"
+                )
             raise HTTPError(resp)
 
         body = json.loads(resp.data)
         return resp, body
 
 
 def get_gremlin_httpclient():
     if requests:
         return GremlineAPIRequestsClient
     else:
         return GremlinAPIurllibClient
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/kubernetes.py` & `gremlinapi-0.9.7/gremlinapi/kubernetes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,79 +6,90 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIKubernetesAttacks(GremlinAPI):
-
     @classmethod
-    @register_cli_action('list_all_kubernetes_attacks', ('',), ('teamId'))
-    def list_all_kubernetes_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint('/kubernetes/attacks', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_all_kubernetes_attacks", ("",), ("teamId"))
+    def list_all_kubernetes_attacks(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/kubernetes/attacks", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_kubernetes_attack', ('uid',), ('teamId'))
-    def get_kubernetes_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        uid = cls._error_if_not_param('uid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/kubernetes/attacks/{uid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_kubernetes_attack", ("uid",), ("teamId"))
+    def get_kubernetes_attack(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        uid = cls._error_if_not_param("uid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/kubernetes/attacks/{uid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_kubernetes_attack', ('uid',), ('teamId',))
-    def halt_kubernetes_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        uid = cls._error_if_not_param('uid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/kubernetes/attacks/{uid}/halt', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("halt_kubernetes_attack", ("uid",), ("teamId",))
+    def halt_kubernetes_attack(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
+        uid = cls._error_if_not_param("uid", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/kubernetes/attacks/{uid}/halt", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_all_kubernetes_attacks', ('',), ('teamId',))
-    def halt_all_kubernetes_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        endpoint = cls._optional_team_endpoint('/kubernetes/attacks/halt', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("halt_all_kubernetes_attacks", ("",), ("teamId",))
+    def halt_all_kubernetes_attacks(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
+        endpoint = cls._optional_team_endpoint("/kubernetes/attacks/halt", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('new_kubernetes_attack', ('body',), ('teamId'))
-    def new_kubernetes_attack(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+    @register_cli_action("new_kubernetes_attack", ("body",), ("teamId"))
+    def new_kubernetes_attack(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint('/kubernetes/attacks/new', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint("/kubernetes/attacks/new", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
 
 class GremlinAPIKubernetesTargets(GremlinAPI):
-
     @classmethod
-    @register_cli_action('list_kubernetes_targets', ('',), ('teamId',))
-    def list_kubernetes_targets(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint('/kubernetes/targets', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_kubernetes_targets", ("",), ("teamId",))
+    def list_kubernetes_targets(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/kubernetes/targets", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/metrics.py` & `gremlinapi-0.9.7/gremlinapi/saml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,68 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 Kyle Hultman <kyle@gremlin.com>, Gremlin Inc <sales@gremlin.com>
 
 import logging
 
 from gremlinapi.cli import register_cli_action
+from gremlinapi.config import GremlinAPIConfig
 from gremlinapi.exceptions import (
     GremlinParameterError,
+    GremlinAuthError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
-class GremlinAPIMetrics(GremlinAPI):
+class GremlinAPISaml(GremlinAPI):
+    @classmethod
+    def acs(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "POST"
+        endpoint = "/users/auth/saml/acs"
+        data = {
+            "SAMLResponse": cls._error_if_not_param("SAMLResponse", **kwargs),
+            "RelayState": cls._error_if_not_param("RelayState", **kwargs),
+        }
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
+        (resp, body) = https_client.api_call(method, endpoint, **payload)
+        return resp
 
     @classmethod
-    @register_cli_action('get_attack_metrics', ('attackId',), ('teamId',))
-    def get_attack_metrics(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        attack_id = cls._error_if_not_param('attackId', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/metrics/attacks/{attack_id}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action(
+        "samllogin", ("companyName", "destination", "acsHandler"), ("",)
+    )
+    def samllogin(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        params = ["companyName", "destination", "acsHandler"]
+        method = "GET"
+        endpoint = cls._build_query_string_endpoint(
+            "/users/auth/saml/login", params, **kwargs
+        )
+        payload = cls._payload(**{})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_scenario_run_metrics', ('scenarioId', 'scenarioRunNumber'), ('teamId',))
-    def get_scenario_run_metrics(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        scenario_id = cls._error_if_not_param('scenarioId', **kwargs)
-        scenario_run_number = cls._error_if_not_param('scenarioRunNumber', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/metrics/scenarios/{scenario_id}/runs/{scenario_run_number}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("metadata", ("",), ("",))
+    def metadata(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "GET"
+        endpoint = "/users/auth/saml/metadata"
+        payload = cls._payload(**{})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
+    @classmethod
+    def sessions(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
+        method = "POST"
+        endpoint = "/users/auth/saml/sessions"
+        data = {"code": cls._error_if_not_param("code", **kwargs)}
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
+        (resp, body) = https_client.api_call(method, endpoint, **payload)
+        return body
```

### Comparing `gremlinapi-0.9.2/gremlinapi/orgs.py` & `gremlinapi-0.9.7/gremlinapi/orgs.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,91 +6,89 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIOrgs(GremlinAPI):
-
     @classmethod
-    @register_cli_action('list_orgs', ('',), ('',))
+    @register_cli_action("list_orgs", ("",), ("",))
     def list_orgs(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = '/orgs'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = "/orgs"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_org', ('identifier',), ('',))
+    @register_cli_action("get_org", ("identifier",), ("",))
     def get_org(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        identifier = cls._error_if_not_param('identifier', **kwargs)
-        endpoint = f'/orgs/{identifier}'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        identifier = cls._error_if_not_param("identifier", **kwargs)
+        endpoint = f"/orgs/{identifier}"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('create_org', ('name',), ('addUser',))
+    @register_cli_action("create_org", ("name",), ("addUser",))
     def create_org(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        add_user = cls._info_if_not_param('addUser', True, **kwargs)
-        endpoint = cls._add_query_param('/orgs', 'addUser', add_user)
-        data = {
-            'name': cls._error_if_not_param('name', **kwargs)
-        }
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        method = "POST"
+        add_user = cls._info_if_not_param("addUser", True, **kwargs)
+        endpoint = cls._add_query_param("/orgs", "addUser", add_user)
+        data = {"name": cls._error_if_not_param("name", **kwargs)}
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('new_certificate', ('',), ('teamId',))
+    @register_cli_action("new_certificate", ("",), ("teamId",))
     def new_certificate(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        endpoint = cls._optional_team_endpoint('/orgs/auth/certificate', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "POST"
+        endpoint = cls._optional_team_endpoint("/orgs/auth/certificate", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_certificate', ('',), ('teamId',))
+    @register_cli_action("delete_certificate", ("",), ("teamId",))
     def delete_certificate(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        endpoint = cls._optional_team_endpoint('/orgs/auth/certificate', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        endpoint = cls._optional_team_endpoint("/orgs/auth/certificate", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_old_certificate', ('',), ('teamId',))
-    def delete_old_certificate(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        endpoint = cls._optional_team_endpoint('/orgs/auth/certificate/old', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("delete_old_certificate", ("",), ("teamId",))
+    def delete_old_certificate(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        endpoint = cls._optional_team_endpoint("/orgs/auth/certificate/old", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('reset_secret', ('',), ('identifier', 'teamId'))
+    @register_cli_action("reset_secret", ("",), ("identifier", "teamId"))
     def reset_secret(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        endpoint = cls._optional_team_endpoint('/orgs/auth/secret/reset', **kwargs)
+        method = "POST"
+        endpoint = cls._optional_team_endpoint("/orgs/auth/secret/reset", **kwargs)
         data = dict()
-        identifier = cls._info_if_not_param('identifier', **kwargs)
+        identifier = cls._info_if_not_param("identifier", **kwargs)
         if identifier:
-            data['identifier'] = identifier
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+            data["identifier"] = identifier
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/reports.py` & `gremlinapi-0.9.7/gremlinapi/alfi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 Kyle Hultman <kyle@gremlin.com>, Gremlin Inc <sales@gremlin.com>
 
 import logging
 
-from datetime import date
-
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
-
+log = logging.getLogger("GremlinAPI.client")
 
-class GremlinAPIReports(GremlinAPI):
-    @classmethod
-    @register_cli_action('report_attacks', ('',), ('start', 'end', 'period', 'teamId'))
-    def report_attacks(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['start', 'end', 'period']
-        endpoint = cls._build_query_string_option_team_endpoint('/reports/attacks', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
-        (resp, body) = https_client.api_call(method, endpoint, **payload)
-        return body
 
+class GremlinALFI(GremlinAPI):
     @classmethod
-    @register_cli_action('report_clients', ('',), ('start', 'end', 'period', 'teamId'))
-    def report_clients(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['start', 'end', 'period']
-        endpoint = cls._build_query_string_option_team_endpoint('/reports/clients', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("create_alfi_experiment", ("body",), ("teamId"))
+    def create_alfi_experiment(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
+        data = cls._error_if_not_json_body(**kwargs)
+        endpoint = cls._optional_team_endpoint("/experiments", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('report_companies', ('',), ('start', 'end', 'period', 'teamId'))
-    def report_companies(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['startDate', 'endDate']
-        endpoint = cls._build_query_string_endpoint('/reports/companies', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("halt_all_alfi_experiments", ("",), ("teamId",))
+    def halt_all_alfi_experiments(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        endpoint = cls._optional_team_endpoint("/experiments", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    def report_pricing(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['startDate', 'endDate', 'trackingPeriod']
-        endpoint = cls._build_query_string_endpoint('/reports/pricing', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_alfi_experiment_details", ("guid",), ("teamId",))
+    def get_alfi_experiment_details(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/experiments/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('report_teams', ('',), ('start', 'end', 'period', 'teamId'))
-    def report_teams(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['startDate', 'endDate']
-        endpoint = cls._build_query_string_option_team_endpoint('/reports/teams', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("halt_alfi_experiment", ("guid",), ("teamId",))
+    def halt_alfi_experiment(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/experiments/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('report_users', ('',), ('start', 'end', 'period', 'teamId'))
-    def report_users(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['start', 'end', 'period']
-        endpoint = cls._build_query_string_option_team_endpoint('/reports/users', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_active_alfi_experiments", ("",), ("teamId",))
+    def list_active_alfi_experiments(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/experiments/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
-class GremlinAPIReportsSecurity(GremlinAPI):
     @classmethod
-    @register_cli_action('report_security_access', ('start', 'end'), ('',))
-    def report_security_access(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        params = ['start', 'end']
-        endpoint = cls._build_query_string_endpoint('/reports/security/access', params, **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_completed_alfi_experiments", ("",), ("teamId"))
+    def list_completed_alfi_experiments(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/experiments/completed", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/scenario_graph_helpers.py` & `gremlinapi-0.9.7/gremlinapi/scenario_graph_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,88 +6,96 @@
 import json
 import logging
 import uuid
 
 from gremlinapi.exceptions import (
     GremlinCommandTargetError,
     GremlinIdentifierError,
-    GremlinParameterError
+    GremlinParameterError,
 )
 
-from gremlinapi.attack_helpers import GremlinAttackCommandHelper, GremlinAttackTargetHelper
+from gremlinapi.attack_helpers import (
+    GremlinAttackCommandHelper,
+    GremlinAttackTargetHelper,
+)
 from gremlinapi.clients import GremlinAPIClients as clients
 from gremlinapi.containers import GremlinAPIContainers as containers
 from gremlinapi.providers import GremlinAPIProviders as providers
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
+
 
 class GremlinScenarioGraphHelper(object):
     def __init__(self, *args, **kwargs):
         self._description = str()
         self._hypothesis = str()
         self._name = str()
         self._nodes = _GremlinNodeGraph()
         self._start = str()
-        self.description = kwargs.get('description', None)
-        self.hypothesis = kwargs.get('hypothesis', None)
-        self.name = kwargs.get('name', None)
+        self.description = kwargs.get("description", None)
+        self.hypothesis = kwargs.get("hypothesis", None)
+        self.name = kwargs.get("name", None)
 
     def add_node(self, _node=None):
         if not issubclass(type(_node), GremlinScenarioNode):
-            error_msg = f'add_node expects GremlinScenarioNode (or None), received {type(_node)}'
+            error_msg = f"add_node expects GremlinScenarioNode (or None), received {type(_node)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._nodes.append(_node)
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, _description=None):
         if not isinstance(_description, str):
-            error_msg = f'Description expects string {type(str())}, received {type(_description)}'
+            error_msg = f"Description expects string {type(str())}, received {type(_description)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._description = _description
 
     @property
     def hypothesis(self):
         return self._hypothesis
 
     @hypothesis.setter
     def hypothesis(self, _hypothesis=None):
         if not isinstance(_hypothesis, str):
-            error_msg = f'Hypothesis expects string {type(str())}, received {type(_hypothesis)}'
+            error_msg = (
+                f"Hypothesis expects string {type(str())}, received {type(_hypothesis)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._hypothesis = _hypothesis
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, _name=None):
         if not isinstance(_name, str):
-            error_msg = f'Name expects string {type(str())}, received {type(_name)}'
+            error_msg = f"Name expects string {type(str())}, received {type(_name)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._name = _name
 
     def repr_model(self):
         model = {
-            'description': self.description,
-            'hypothesis': self.hypothesis,
-            'name': self.name
+            "description": self.description,
+            "hypothesis": self.hypothesis,
+            "name": self.name,
         }
         if self._nodes.head is not None:
-            model['graph'] = {
-                'start_id': self._nodes.head.uuid,
-                'nodes': {node.uuid: data for node, data in self._nodes.nodes_data_linear()}
+            model["graph"] = {
+                "start_id": self._nodes.head.uuid,
+                "nodes": {
+                    node.uuid: data for node, data in self._nodes.nodes_data_linear()
+                },
             }
         return model
 
     def __repr__(self):
         model = self.repr_model()
         return json.dumps(model)
 
@@ -97,101 +105,103 @@
         self._edges = dict()
         self._id = str()
         self._previous = None
         self._name = str()
         self._next = None
         self._node_type = str()
         self.id = str(uuid.uuid4())
-        self.name = kwargs.get('name', None)
+        self.name = kwargs.get("name", None)
 
     def add_edge(self, _node=None, _weight=None):
         if not issubclass(type(_node), GremlinScenarioNode):
-            error_msg = f'add_edge expects a GremlinScenarioNode, received {type(_node)}'
+            error_msg = (
+                f"add_edge expects a GremlinScenarioNode, received {type(_node)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        self._edges[_node.id] = {'node': _node, 'weight': _weight}
+        self._edges[_node.id] = {"node": _node, "weight": _weight}
 
     @property
     def data(self):
         return self.repr_model()
 
     @property
     def id(self):
         return self._id
 
     @id.setter
     def id(self, _id=None):
         if not isinstance(_id, str):
-            error_msg = f'id expects a string {type(str)}, received {type(str)}'
+            error_msg = f"id expects a string {type(str)}, received {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._id = _id
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, _name=None):
         if not isinstance(_name, str):
-            error_msg = f'name expects type string {type(str)}, received {type(_name)}'
+            error_msg = f"name expects type string {type(str)}, received {type(_name)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._name = _name
 
     @property
     def next(self):
         return self._next
 
     @next.setter
     def next(self, _node=None):
         if not issubclass(type(_node), GremlinScenarioNode):
-            error_msg = f'next expects a GremlinScenarioNode, received {type(_node)}'
+            error_msg = f"next expects a GremlinScenarioNode, received {type(_node)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._next = _node
 
     @property
     def node_type(self):
         return self._node_type
 
     @node_type.setter
     def node_type(self, _node_type=None):
         if not isinstance(_node_type, str):
-            error_msg = f'node_type expects string {type(str)}, received {type(_node_type)}'
+            error_msg = (
+                f"node_type expects string {type(str)}, received {type(_node_type)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._node_type = _node_type
 
     @property
     def previous(self):
         return self._previous
 
     @previous.setter
     def previous(self, _node=None):
         if not issubclass(type(_node), GremlinScenarioNode):
-            error_msg = f'previous expects a GremlinScenarioNode, received {type(_node)}'
+            error_msg = (
+                f"previous expects a GremlinScenarioNode, received {type(_node)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._previous = _node
 
     @property
     def uuid(self):
         if not self.name:
-            error_msg = f'Node Name is required to build a scenario node, please set a node name'
+            error_msg = f"Node Name is required to build a scenario node, please set a node name"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        return f'{self.name}-{self.id}'
+        return f"{self.name}-{self.id}"
 
     def repr_model(self):
-        model = {
-            'type': self.node_type,
-            'id': self.uuid,
-            'next': self.next.uuid
-        }
+        model = {"type": self.node_type, "id": self.uuid, "next": self.next.uuid}
         return model
 
     def __repr__(self):
         return json.dumps(self.repr_model)
 
 
 class GremlinScenarioAttackNode(GremlinScenarioNode):
@@ -203,137 +213,145 @@
     @property
     def attack_type(self):
         return self._attack_type
 
     @attack_type.setter
     def attack_type(self, _attack_type=None):
         if not isinstance(_attack_type, str):
-            error_msg = f'attack_type expects string {type(str)}, received {type(_attack_type)}'
+            error_msg = (
+                f"attack_type expects string {type(str)}, received {type(_attack_type)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._attack_type = _attack_type
 
 
 class GremlinScenarioILFINode(GremlinScenarioAttackNode):
     def __init__(self, *args, **kwargs):
-        if not kwargs.get('name', None) and kwargs.get('command', None):
-            kwargs['name'] = kwargs.get('command').shortType
+        if not kwargs.get("name", None) and kwargs.get("command", None):
+            kwargs["name"] = kwargs.get("command").shortType
         super().__init__(*args, **kwargs)
         self._command = None
         self._target = None
         self.node_type = "InfraAttack"
-        self.command = kwargs.get('command', self._command)
-        self.target = kwargs.get('target', self._target)
+        self.command = kwargs.get("command", self._command)
+        self.target = kwargs.get("target", self._target)
 
     @property
     def command(self):
         return self._command
 
     @command.setter
     def command(self, _command=None):
         if not issubclass(type(_command), GremlinAttackCommandHelper):
-            error_msg = f'impact_definition expects a GremlinAttackCommandHelper, received {type(_command)}'
+            error_msg = f"impact_definition expects a GremlinAttackCommandHelper, received {type(_command)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._command = _command
 
     def repr_model(self):
         model = super().repr_model()
-        model['impact_definition'] = self.command.impact_definition_graph()
-        model['target_definition'] = self.target.target_definition_graph()
+        model["impact_definition"] = self.command.impact_definition_graph()
+        model["target_definition"] = self.target.target_definition_graph()
         return model
 
     @property
     def target(self):
         return self._target
 
     @target.setter
     def target(self, _target=None):
         if not issubclass(type(_target), GremlinAttackTargetHelper):
-            error_msg = f'target_definition expects a GremlinAttackTargetHelper, received {type(_target)}'
+            error_msg = f"target_definition expects a GremlinAttackTargetHelper, received {type(_target)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._target = _target
 
 
 class GremlinScenarioALFINode(GremlinScenarioAttackNode):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.attack_type = "ALFI"
-        raise NotImplementedError('ALFI Scenarios NOT IMPLEMENTED')
+        raise NotImplementedError("ALFI Scenarios NOT IMPLEMENTED")
 
 
 class GremlinScenarioDelayNode(GremlinScenarioNode):
     def __init__(self, *args, **kwargs):
-        if not kwargs.get('name', None):
-            kwargs['name'] = 'Delay'
+        if not kwargs.get("name", None):
+            kwargs["name"] = "Delay"
         super().__init__(*args, **kwargs)
         self._delay = int()
-        self._delay = kwargs.get('delay', None)
+        self._delay = kwargs.get("delay", None)
         self.node_type = "Delay"
 
     def repr_model(self):
         model = super().repr_model()
-        model['delay'] = self.delay
+        model["delay"] = self.delay
         return model
 
     @property
     def delay(self):
         return self._delay
 
     @delay.setter
     def delay(self, _duration=None):
         if not isinstance(_duration, int):
-            error_msg = f'delay expects int type {type(int)}, received {type(_duration)}'
+            error_msg = (
+                f"delay expects int type {type(int)}, received {type(_duration)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._delay = _duration
 
 
 class GremlinScenarioStatusCheckNode(GremlinScenarioNode):
     def __init__(self, *args, **kwargs):
-        if not kwargs.get('name', None):
-            kwargs['name'] = 'status-check'
+        if not kwargs.get("name", None):
+            kwargs["name"] = "status-check"
         super().__init__(*args, **kwargs)
         self.node_type = "SynchronousStatusCheck"
         self._description = str()
         self._endpoint_url = str()
         self._endpoint_headers = None
         self._evaluation_ok_status_codes = list()
         self._evaluation_ok_latency_max = int()
         self._evaluation_response_body_evaluation = None
-        self.description = kwargs.get('description', None)
-        self.endpoint_url = kwargs.get('endpoint_url', None)
-        self.endpoint_headers = kwargs.get('endpoint_headers', None)
-        self.evaluation_ok_status_codes = kwargs.get('evaluation_ok_status_codes', ["200-203"])
-        self.evaluation_ok_latency_max = kwargs.get('evaluation_ok_latency_max', 500)
-        self.evaluation_response_body_evaluation = kwargs.get('evaluation_response_body_evaluation', "")
+        self.description = kwargs.get("description", None)
+        self.endpoint_url = kwargs.get("endpoint_url", None)
+        self.endpoint_headers = kwargs.get("endpoint_headers", None)
+        self.evaluation_ok_status_codes = kwargs.get(
+            "evaluation_ok_status_codes", ["200-203"]
+        )
+        self.evaluation_ok_latency_max = kwargs.get("evaluation_ok_latency_max", 500)
+        self.evaluation_response_body_evaluation = kwargs.get(
+            "evaluation_response_body_evaluation", ""
+        )
 
     def repr_model(self):
         model = super().repr_model()
-        model['endpointConfiguration'] = {
-            'url': self.endpoint_url,
-            'headers': self.endpoint_headers
+        model["endpointConfiguration"] = {
+            "url": self.endpoint_url,
+            "headers": self.endpoint_headers,
         }
-        model['evaluationConfiguration'] = {
-            'okStatusCodes': self.evaluation_ok_status_codes,
-            'okLatencyMaxMs': self.evaluation_ok_latency_max,
-            'responseBodyEvaluation': self.evaluation_response_body_evaluation
+        model["evaluationConfiguration"] = {
+            "okStatusCodes": self.evaluation_ok_status_codes,
+            "okLatencyMaxMs": self.evaluation_ok_latency_max,
+            "responseBodyEvaluation": self.evaluation_response_body_evaluation,
         }
-        model['thirdPartyPresets'] = 'PythonSDK'
+        model["thirdPartyPresets"] = "PythonSDK"
         return model
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, _description=None):
         if not isinstance(_description, str):
-            error_msg = f'description expects string, received {type(_description)}'
+            error_msg = f"description expects string, received {type(_description)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._description = _description
 
     @property
     def endpoint_headers(self):
         return self._endpoint_headers
@@ -345,51 +363,55 @@
     @property
     def endpoint_url(self):
         return self._endpoint_url
 
     @endpoint_url.setter
     def endpoint_url(self, _url=None):
         if not isinstance(_url, str):
-            error_msg = f'url expects a valid url string, received {type(_url)}'
+            error_msg = f"url expects a valid url string, received {type(_url)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._endpoint_url = _url
 
     @property
     def evaluation_ok_status_codes(self):
         return self._evaluation_ok_status_codes
 
     @evaluation_ok_status_codes.setter
     def evaluation_ok_status_codes(self, _status_codes=None):
         if not isinstance(_status_codes, list):
-            error_msg = f'evaluation_ok_status_codes expects a list of integers or strings, received {type(_status_codes)}'
+            error_msg = f"evaluation_ok_status_codes expects a list of integers or strings, received {type(_status_codes)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._evaluation_ok_status_codes = _status_codes
 
     @property
     def evaluation_ok_latency_max(self):
         return self._evaluation_ok_latency_max
 
     @evaluation_ok_latency_max.setter
     def evaluation_ok_latency_max(self, _latency=None):
         if not isinstance(_latency, int):
-            error_msg = f'evaluation_ok_latency_max expects an int, received {type(_latency)}'
+            error_msg = (
+                f"evaluation_ok_latency_max expects an int, received {type(_latency)}"
+            )
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._evaluation_ok_latency_max = _latency
 
     @property
     def evaluation_response_body_evaluation(self):
         return self._evaluation_response_body_evaluation
 
     @evaluation_response_body_evaluation.setter
-    def evaluation_response_body_evaluation(self, _evaluation_response_body_evaluation=None):
+    def evaluation_response_body_evaluation(
+        self, _evaluation_response_body_evaluation=None
+    ):
         if not _evaluation_response_body_evaluation:
-            error_msg = f'evaluation_response_body_evaluation expects an argument, none provided'
+            error_msg = f"evaluation_response_body_evaluation expects an argument, none provided"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         self._evaluation_response_body_evaluation = _evaluation_response_body_evaluation
 
 
 class _GremlinNodeGraph(object):
     def __init__(self):
@@ -408,15 +430,15 @@
             new_node.previous = new_node
             self.head = new_node
         else:
             self.insert_after(self.head.previous, new_node)
 
     def get_node(self, _index=None):
         if not isinstance(_index, int):
-            error_msg = f'get_node expects index as integer, received {type(_index)}'
+            error_msg = f"get_node expects index as integer, received {type(_index)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         node = self.head
         for idx in range(_index):
             node = node.next
             if node == self.head:
                 return None
@@ -451,15 +473,15 @@
             data = node.data
             yield node, data
 
     def nodes_data_linear(self):
         for node in self.nodes():
             data = node.data
             if node.next == self.head:
-                data.pop('next')
+                data.pop("next")
             yield node, data
 
     def previous(self):
         self.head = self.head.previous
 
     def push(self, new_node=None):
         self._validate_type(new_node)
@@ -485,12 +507,11 @@
     def head(self, node=None):
         self._validate_type(node)
         self._head = node
 
     def _validate_type(self, _node=None):
         _caller = inspect.stack()[2][3]
         if not issubclass(type(_node), GremlinScenarioNode):
-            error_msg = f'{_caller} expects node to be a subclass of GremlinScenarioNode, received {type(_node)}'
+            error_msg = f"{_caller} expects node to be a subclass of GremlinScenarioNode, received {type(_node)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return True
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/scenario_helpers.py` & `gremlinapi-0.9.7/gremlinapi/scenario_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,65 +5,78 @@
 import json
 import logging
 import uuid
 
 from gremlinapi.exceptions import (
     GremlinCommandTargetError,
     GremlinIdentifierError,
-    GremlinParameterError
+    GremlinParameterError,
 )
 
-from gremlinapi.attack_helpers import GremlinAttackCommandHelper, GremlinAttackTargetHelper
+from gremlinapi.attack_helpers import (
+    GremlinAttackCommandHelper,
+    GremlinAttackTargetHelper,
+)
 from gremlinapi.clients import GremlinAPIClients as clients
 from gremlinapi.containers import GremlinAPIContainers as containers
 from gremlinapi.providers import GremlinAPIProviders as providers
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinScenarioHelper(object):
     def __init__(self, *args, **kwargs):
         self._description = str()
         self._hypothesis = str()
         self._name = str()
         self._steps = list()
-        self.description = kwargs.get('description', self._description)
-        self.hypothesis = kwargs.get('hypothesis', self._hypothesis)
-        self.name = kwargs.get('name', self._name)
+        self.description = kwargs.get("description", self._description)
+        self.hypothesis = kwargs.get("hypothesis", self._hypothesis)
+        self.name = kwargs.get("name", self._name)
 
     def add_step(self, _step=None):
         if not issubclass(type(_step), GremlinScenarioStep):
-            error_msg = f'The step must extend from {type(GremlinScenarioStep)}'
+            error_msg = f"The step must extend from {type(GremlinScenarioStep)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         _cur_step_obj = json.loads(str(_step))
         if len(self._steps) > 0:
-            log.debug('checking last step')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug("checking last step")
             _last_step_obj = self._steps[-1]
-            last_attack_type = _last_step_obj['attacks'][0]['attackType']
-            last_target_type = _last_step_obj['attacks'][0]['targetDefinition']['targetType']
-            last_command_type = _last_step_obj['attacks'][0]['impactDefinition']['commandType']
-            cur_attack_type = _cur_step_obj['attacks'][0]['attackType']
-            cur_target_type = _cur_step_obj['attacks'][0]['targetDefinition']['targetType']
-            cur_command_type = _cur_step_obj['attacks'][0]['impactDefinition']['commandType']
+            last_attack_type = _last_step_obj["attacks"][0]["attackType"]
+            last_target_type = _last_step_obj["attacks"][0]["targetDefinition"][
+                "targetType"
+            ]
+            last_command_type = _last_step_obj["attacks"][0]["impactDefinition"][
+                "commandType"
+            ]
+            cur_attack_type = _cur_step_obj["attacks"][0]["attackType"]
+            cur_target_type = _cur_step_obj["attacks"][0]["targetDefinition"][
+                "targetType"
+            ]
+            cur_command_type = _cur_step_obj["attacks"][0]["impactDefinition"][
+                "commandType"
+            ]
             if not last_attack_type == cur_attack_type:
-                error_msg = f'Each step must target the same attackType'
+                error_msg = f"Each step must target the same attackType"
                 log.fatal(error_msg)
                 raise GremlinCommandTargetError(error_msg)
             if not last_target_type == cur_target_type:
-                error_msg = f'Each step must target the same primitive typeset'
+                error_msg = f"Each step must target the same primitive typeset"
                 log.fatal(error_msg)
                 raise GremlinCommandTargetError(error_msg)
             if not last_command_type == cur_command_type:
-                error_msg = f'Each step must use the same command type'
+                error_msg = f"Each step must use the same command type"
                 log.fatal(error_msg)
                 raise GremlinCommandTargetError(error_msg)
             self._steps.append(_cur_step_obj)
         else:
-            log.debug('fist step, just adding')
+            if log.getEffectiveLevel() == logging.DEBUG:
+                log.debug("fist step, just adding")
             self._steps.append(_cur_step_obj)
 
     @property
     def description(self):
         return self._description
 
     @description.setter
@@ -83,112 +96,111 @@
         return self._name
 
     @name.setter
     def name(self, _name=None):
         if isinstance(_name, str):
             self._name = _name
         else:
-            error_msg = f'name expects type {type(str)}'
+            error_msg = f"name expects type {type(str)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def steps(self):
         return self._steps
 
     @steps.setter
     def steps(self, _steps=None):
-        error_msg = f'Interface not implemented, use `add_step`'
+        error_msg = f"Interface not implemented, use `add_step`"
         log.warning(error_msg)
         raise NotImplemented(error_msg)
 
     def __repr__(self):
         model = {
-            'description': self.description,
-            'hypothesis': self.hypothesis,
-            'name': self.name,
-            'steps': self.steps
+            "description": self.description,
+            "hypothesis": self.hypothesis,
+            "name": self.name,
+            "steps": self.steps,
         }
         return json.dumps(model)
 
 
 class GremlinScenarioStep(object):
     def __init__(self, *args, **kwargs):
         self._delay = 5
-        self.delay = kwargs.get('delay', self._delay)
+        self.delay = kwargs.get("delay", self._delay)
 
     @property
     def delay(self):
         return self._delay
 
     @delay.setter
     def delay(self, _delay):
         if isinstance(_delay, int) and _delay >= 1:
             self._delay = _delay
         else:
-            error_msg = f'delay expects a positive integer {type(int)}'
+            error_msg = f"delay expects a positive integer {type(int)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     def __repr__(self):
-        model = {
-            'delay': self.delay
-        }
+        model = {"delay": self.delay}
         return json.dumps(model)
 
 
 class GremlinILFIStep(GremlinScenarioStep):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._command = None
         self._target = None
-        self.command = kwargs.get('command', self._command)
-        self.target = kwargs.get('target', self._target)
+        self.command = kwargs.get("command", self._command)
+        self.target = kwargs.get("target", self._target)
 
     @property
     def command(self):
         return self._command
 
     @command.setter
     def command(self, _command=None):
         if _command and issubclass(type(_command), GremlinAttackCommandHelper):
             self._command = _command
         else:
-            error_msg = f'command expects a GremlinAttackCommandHelper {type(GremlinAttackCommandHelper)}'
+            error_msg = f"command expects a GremlinAttackCommandHelper {type(GremlinAttackCommandHelper)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     @property
     def target(self):
         return self._target
 
     @target.setter
     def target(self, _target=None):
         if _target and issubclass(type(_target), GremlinAttackTargetHelper):
             self._target = _target
         else:
-            error_msg = f'target expects a GremlinAttackTargetHelper {type(GremlinAttackTargetHelper)}'
+            error_msg = f"target expects a GremlinAttackTargetHelper {type(GremlinAttackTargetHelper)}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
 
     def __repr__(self):
         model = json.loads(super().__repr__())
-        model['attacks'] = [{
-            'attackType': 'ILFI',
-            'impactDefinition': self.command.impact_definition(),
-            'targetDefinition': self.target.target_definition()
-        }]
-        model['id'] = str(uuid.uuid3(uuid.NAMESPACE_X500, str(model['attacks'])))
+        model["attacks"] = [
+            {
+                "attackType": "ILFI",
+                "impactDefinition": self.command.impact_definition(),
+                "targetDefinition": self.target.target_definition(),
+            }
+        ]
+        model["id"] = str(uuid.uuid3(uuid.NAMESPACE_X500, str(model["attacks"])))
         return json.dumps(model)
 
 
 class GremlinALFIStep(GremlinScenarioStep):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        error_msg = f'GremlinALFIStep NOT IMPLEMENTED'
+        error_msg = f"GremlinALFIStep NOT IMPLEMENTED"
         log.fatal(error_msg)
         raise NotImplemented(error_msg)
 
     def __repr__(self):
         model = json.loads(super().__repr__())
         return json.dumps(model)
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/scenarios.py` & `gremlinapi-0.9.7/gremlinapi/scenarios.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,231 +6,307 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 from gremlinapi.scenario_helpers import GremlinScenarioHelper
 from gremlinapi.scenario_graph_helpers import GremlinScenarioGraphHelper
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIScenarios(GremlinAPI):
     @classmethod
     def _error_if_not_scenario_body(cls, **kwargs):
-        body = cls._error_if_not_param('body', **kwargs)
-        if issubclass(type(body), GremlinScenarioHelper) or issubclass(type(body), GremlinScenarioGraphHelper):
+        body = cls._error_if_not_param("body", **kwargs)
+        if issubclass(type(body), GremlinScenarioHelper) or issubclass(
+            type(body), GremlinScenarioGraphHelper
+        ):
             return str(body)
         else:
-            error_msg = f'Body present but not of type {type(GremlinScenarioHelper)}'
+            error_msg = f"Body present but not of type {type(GremlinScenarioHelper)}"
             log.warning(error_msg)
         return body
 
     @classmethod
-    @register_cli_action('list_scenarios', ('',), ('teamId',))
+    @register_cli_action("list_scenarios", ("",), ("teamId",))
     def list_scenarios(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint('/scenarios', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint("/scenarios", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('create_scenario', ('body',), ('teamId',))
+    @register_cli_action("create_scenario", ("body",), ("teamId",))
     def create_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = cls._error_if_not_scenario_body(**kwargs)
-        endpoint = cls._optional_team_endpoint('/scenarios', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint("/scenarios", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_scenario', ('guid',), ('teamId',))
+    @register_cli_action("get_scenario", ("guid",), ("teamId",))
     def get_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_scenario', ('guid', 'body'), ('teamId',))
+    @register_cli_action("update_scenario", ("guid", "body"), ("teamId",))
     def update_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'PUT'
-        guid = cls._error_if_not_param('guid', **kwargs)
+        method = "PUT"
+        guid = cls._error_if_not_param("guid", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('archive_scenario', ('guid',), ('teamId',))
+    @register_cli_action("archive_scenario", ("guid",), ("teamId",))
     def archive_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/archive', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}/archive", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('restore_scenario', ('guid',), ('teamId',))
+    @register_cli_action("restore_scenario", ("guid",), ("teamId",))
     def restore_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/restore', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}/restore", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_scenario_runs', ('guid',), ('startDate', 'endDate', 'teamId',))
+    @register_cli_action(
+        "list_scenario_runs",
+        ("guid",),
+        (
+            "startDate",
+            "endDate",
+            "teamId",
+        ),
+    )
     def list_scenario_runs(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        timeset = ''
-        start = cls._info_if_not_param('startDate', **kwargs)
-        end = cls._info_if_not_param('endDate', **kwargs)
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        timeset = ""
+        start = cls._info_if_not_param("startDate", **kwargs)
+        end = cls._info_if_not_param("endDate", **kwargs)
         if start:
-            timeset += f'startDate={start}&'
+            timeset += f"startDate={start}&"
         if end:
-            timeset += f'endDate={end}'
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/runs/?{timeset}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+            timeset += f"endDate={end}"
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/{guid}/runs/?{timeset}", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('run_scenario', ('guid',), ('teamId', 'body',))
+    @register_cli_action(
+        "run_scenario",
+        ("guid",),
+        (
+            "teamId",
+            "body",
+        ),
+    )
     def run_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
         data = cls._warn_if_not_json_body(**kwargs, default=dict())
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/runs', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}/runs", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_scenario_run_details', ('guid', 'runNumber',), ('teamId',))
-    def get_scenario_run_details(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        run_number = cls._error_if_not_param('runNumber', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/runs/{run_number}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action(
+        "get_scenario_run_details",
+        (
+            "guid",
+            "runNumber",
+        ),
+        ("teamId",),
+    )
+    def get_scenario_run_details(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        run_number = cls._error_if_not_param("runNumber", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/{guid}/runs/{run_number}", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_scenario_result_flags', ('guid', 'runNumber', 'body',), ('teamId',))
-    def update_scenario_result_flags(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'PUT'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        run_number = cls._error_if_not_param('runNumber', **kwargs)
+    @register_cli_action(
+        "update_scenario_result_flags",
+        (
+            "guid",
+            "runNumber",
+            "body",
+        ),
+        ("teamId",),
+    )
+    def update_scenario_result_flags(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "PUT"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        run_number = cls._error_if_not_param("runNumber", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/runs/{run_number}/resultFlags', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/{guid}/runs/{run_number}/resultFlags", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_scenario_result_notes', ('guid', 'runNumber', 'body',), ('teamId',))
-    def update_scenario_result_notes(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'PUT'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        run_number = cls._error_if_not_param('runNumber', **kwargs)
+    @register_cli_action(
+        "update_scenario_result_notes",
+        (
+            "guid",
+            "runNumber",
+            "body",
+        ),
+        ("teamId",),
+    )
+    def update_scenario_result_notes(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "PUT"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        run_number = cls._error_if_not_param("runNumber", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/runs/{run_number}/resultNotes', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/{guid}/runs/{run_number}/resultNotes", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_scenario_schedules', ('guid',), ('teamId',))
-    def list_scenario_schedules(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/{guid}/schedules', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_scenario_schedules", ("guid",), ("teamId",))
+    def list_scenario_schedules(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/scenarios/{guid}/schedules", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_scenarios', ('',), ('teamId',))
-    def list_active_scenarios(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/scenarios/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_active_scenarios", ("",), ("teamId",))
+    def list_active_scenarios(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/scenarios/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_archived_scenarios', ('',), ('teamId',))
-    def list_archived_scenarios(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/scenarios/archived', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_archived_scenarios", ("",), ("teamId",))
+    def list_archived_scenarios(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/scenarios/archived", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_draft_scenarios', ('',), ('teamId',))
-    def list_draft_scenarios(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/scenarios/drafts', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_draft_scenarios", ("",), ("teamId",))
+    def list_draft_scenarios(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/scenarios/drafts", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('halt_scenario', ('guid', 'runNumber'), ('teamId',))
+    @register_cli_action("halt_scenario", ("guid", "runNumber"), ("teamId",))
     def halt_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        run_number = cls._error_if_not_param('runNumber', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/halt/{guid}/runs/{run_number}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        run_number = cls._error_if_not_param("runNumber", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/halt/{guid}/runs/{run_number}", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
-class GremlinAPIScenariosRecommended(GremlinAPI):
 
+class GremlinAPIScenariosRecommended(GremlinAPI):
     @classmethod
-    @register_cli_action('list_recommended_scenarios', ('',), ('teamId',))
-    def list_recommended_scenarios(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/scenarios/recommended', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_recommended_scenarios", ("",), ("teamId",))
+    def list_recommended_scenarios(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/scenarios/recommended", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_recommended_scenario', ('guid',), ('teamId',))
-    def get_recommended_scenario(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/recommended/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_recommended_scenario", ("guid",), ("teamId",))
+    def get_recommended_scenario(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/recommended/{guid}", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_recommended_scenario_static', ('staticEndpointName',), ('teamId',))
-    def get_recommended_scenario_static(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        static_endpoint_name = cls._error_if_not_param('staticEndpointName', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/scenarios/recommended/static/{static_endpoint_name}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action(
+        "get_recommended_scenario_static", ("staticEndpointName",), ("teamId",)
+    )
+    def get_recommended_scenario_static(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        static_endpoint_name = cls._error_if_not_param("staticEndpointName", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/scenarios/recommended/static/{static_endpoint_name}", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
-        return body
+        return body
```

### Comparing `gremlinapi-0.9.2/gremlinapi/schedules.py` & `gremlinapi-0.9.7/gremlinapi/schedules.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,176 +6,210 @@
 
 from gremlinapi.cli import register_cli_action
 from gremlinapi.exceptions import (
     GremlinParameterError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPISchedules(GremlinAPI):
 
     # @classmethod
     # @register_cli_action('list_schedules', ('',), ('teamId',))
     # def list_schedules(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
     #     method = 'GET'
     #     endpoint = cls._optional_team_endpoint(f'/schedules', **kwargs)
     #     payload = cls._payload(**{'headers': https_client.header()})
     #     (resp, body) = https_client.api_call(method, endpoint, **payload)
     #     return body
 
     @classmethod
-    @register_cli_action('create_schedule', ('body',), ('teamId',))
+    @register_cli_action("create_schedule", ("body",), ("teamId",))
     def create_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/schedules", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_schedule', ('guid',), ('teamId',))
+    @register_cli_action("get_schedule", ("guid",), ("teamId",))
     def get_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_schedule', ('guid',), ('teamId',))
+    @register_cli_action("delete_schedule", ("guid",), ("teamId",))
     def delete_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_schedules', ('',), ('teamId',))
-    def list_active_schedules(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/schedules/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_active_schedules", ("",), ("teamId",))
+    def list_active_schedules(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/schedules/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_attack_schedules', ('',), ('teamId',))
-    def list_attack_schedules(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/schedules/attacks', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_attack_schedules", ("",), ("teamId",))
+    def list_attack_schedules(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/schedules/attacks", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('create_attack_schedule', ('body',), ('teamId',))
-    def create_attack_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+    @register_cli_action("create_attack_schedule", ("body",), ("teamId",))
+    def create_attack_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/attacks', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/schedules/attacks", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_attack_schedule', ('guid',), ('teamId',))
-    def get_attack_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/attacks/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_attack_schedule", ("guid",), ("teamId",))
+    def get_attack_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/attacks/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_attack_schedule', ('guid',), ('teamId',))
-    def delete_attack_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/attacks/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("delete_attack_schedule", ("guid",), ("teamId",))
+    def delete_attack_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/attacks/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_scenario_schedules', ('',), ('teamId',))
-    def list_scenario_schedules(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("list_scenario_schedules", ("",), ("teamId",))
+    def list_scenario_schedules(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/schedules/scenarios", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('create_scenario_schedule', ('body',), ('teamId',))
-    def create_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+    @register_cli_action("create_scenario_schedule", ("body",), ("teamId",))
+    def create_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/schedules/scenarios", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_scenario_schedule', ('guid',), ('teamId',))
-    def get_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_scenario_schedule", ("guid",), ("teamId",))
+    def get_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/scenarios/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_scenario_schedule', ('guid', 'body',), ('teamId',))
-    def update_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
+    @register_cli_action(
+        "update_scenario_schedule",
+        (
+            "guid",
+            "body",
+        ),
+        ("teamId",),
+    )
+    def update_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/schedules/scenarios/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('delete_scenario_schedule', ('guid',), ('teamId',))
-    def delete_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios/{guid}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("delete_scenario_schedule", ("guid",), ("teamId",))
+    def delete_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(f"/schedules/scenarios/{guid}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('enable_scenario_schedule', ('guid',), ('teamId',))
-    def enable_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios/{guid}/enabled', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("enable_scenario_schedule", ("guid",), ("teamId",))
+    def enable_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "POST"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/schedules/scenarios/{guid}/enabled", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('disable_scenario_schedule', ('guid',), ('teamId',))
-    def disable_scenario_schedule(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        guid = cls._error_if_not_param('guid', **kwargs)
-        endpoint = cls._optional_team_endpoint(f'/schedules/scenarios/{guid}/enabled', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("disable_scenario_schedule", ("guid",), ("teamId",))
+    def disable_scenario_schedule(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "DELETE"
+        guid = cls._error_if_not_param("guid", **kwargs)
+        endpoint = cls._optional_team_endpoint(
+            f"/schedules/scenarios/{guid}/enabled", **kwargs
+        )
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi/users.py` & `gremlinapi-0.9.7/gremlinapi/users.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,335 +8,393 @@
 from gremlinapi.config import GremlinAPIConfig
 from gremlinapi.exceptions import (
     GremlinParameterError,
     GremlinAuthError,
     ProxyError,
     ClientError,
     HTTPTimeout,
-    HTTPError
+    HTTPError,
 )
 
 from gremlinapi.gremlinapi import GremlinAPI
 from gremlinapi.http_clients import get_gremlin_httpclient
 
 
-log = logging.getLogger('GremlinAPI.client')
+log = logging.getLogger("GremlinAPI.client")
 
 
 class GremlinAPIUsers(GremlinAPI):
-
     @classmethod
     def _error_if_not_valid_role_statement(cls, **kwargs):
-        role = kwargs.get('role', None)
+        role = kwargs.get("role", None)
         if not role:
-            error_msg = f'Role object not passed to users endpoint: {kwargs}'
+            error_msg = f"Role object not passed to users endpoint: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         return role
 
     @classmethod
-    @register_cli_action('list_user', ('',), ('teamId',))
+    @register_cli_action("list_user", ("",), ("teamId",))
     def list_users(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/users', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/users", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('add_user_to_team', ('body',), ('teamId',))
+    @register_cli_action("add_user_to_team", ("body",), ("teamId",))
     def add_user_to_team(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = cls._error_if_not_json_body(**kwargs)
         if isinstance(data, dict):
             data = [dict(data)]
-        endpoint = cls._optional_team_endpoint(f'/users', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = cls._optional_team_endpoint(f"/users", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_user', ('email', 'role'), ('teamId',))
+    @register_cli_action("update_user", ("email", "role"), ("teamId",))
     def update_user(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'PUT'
+        method = "PUT"
         email = cls._error_if_not_email(**kwargs)
         role = cls._error_if_not_valid_role_statement(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/users/{email}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header(), 'data': role})
+        endpoint = cls._optional_team_endpoint(f"/users/{email}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header(), "data": role})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('deactivate_user', ('email',), ('teamId',))
+    @register_cli_action("deactivate_user", ("email",), ("teamId",))
     def deactivate_user(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
+        method = "DELETE"
         email = cls._error_if_not_email(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/users/{email}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = cls._optional_team_endpoint(f"/users/{email}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('list_active_user', ('',), ('teamId',))
+    @register_cli_action("list_active_user", ("",), ("teamId",))
     def list_active_users(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = cls._optional_team_endpoint(f'/users/active', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = cls._optional_team_endpoint(f"/users/active", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('invite_user', ('email',), ('teamId',))
+    @register_cli_action("invite_user", ("email",), ("teamId",))
     def invite_user(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         email = cls._error_if_not_email(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/users/invite', **kwargs)
-        data = {'email': email}
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        endpoint = cls._optional_team_endpoint(f"/users/invite", **kwargs)
+        data = {"email": email}
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('revoke_user_invite', ('email',), ('teamId',))
+    @register_cli_action("revoke_user_invite", ("email",), ("teamId",))
     def revoke_user_invite(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
+        method = "DELETE"
         email = cls._error_if_not_email(**kwargs)
-        endpoint = cls._optional_team_endpoint(f'/users/invite/{email}', **kwargs)
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = cls._optional_team_endpoint(f"/users/invite/{email}", **kwargs)
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('renew_user_authorization', ('email', 'orgId', 'renewToken'), ('',))
-    def renew_user_authorization(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
+    @register_cli_action(
+        "renew_user_authorization", ("email", "orgId", "renewToken"), ("",)
+    )
+    def renew_user_authorization(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
         email = cls._error_if_not_email(**kwargs)
-        org_id = kwargs.get('orgId', None)
-        renew_token = kwargs.get('renewToken', None)
+        org_id = kwargs.get("orgId", None)
+        renew_token = kwargs.get("renewToken", None)
         if not org_id:
-            error_msg = f'orgId required parameter not supplied: {kwargs}'
+            error_msg = f"orgId required parameter not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if not renew_token:
-            error_msg = f'renewToken required parameter not supplied: {kwargs}'
+            error_msg = f"renewToken required parameter not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        data = {'email': email, 'orgId': org_id, 'renewToken': renew_token}
-        endpoint = f'/users/renew'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        data = {"email": email, "orgId": org_id, "renewToken": renew_token}
+        endpoint = f"/users/renew"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('renew_user_authorization_rbac', ('email', 'companyId', 'teamId', 'renewToken'), ('',))
-    def renew_user_authorization_rbac(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
+    @register_cli_action(
+        "renew_user_authorization_rbac",
+        ("email", "companyId", "teamId", "renewToken"),
+        ("",),
+    )
+    def renew_user_authorization_rbac(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
         email = cls._error_if_not_email(**kwargs)
-        company_id = kwargs.get('companyId', None)
-        team_id =  cls._error_if_not_param('teamnId', **kwargs)
-        renew_token = kwargs.get('renewToken', None)
+        company_id = kwargs.get("companyId", None)
+        team_id = cls._error_if_not_param("teamnId", **kwargs)
+        renew_token = kwargs.get("renewToken", None)
         if not company_id:
-            error_msg = f'orgId required parameter not supplied: {kwargs}'
+            error_msg = f"orgId required parameter not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
         if not renew_token:
-            error_msg = f'renewToken required parameter not supplied: {kwargs}'
+            error_msg = f"renewToken required parameter not supplied: {kwargs}"
             log.fatal(error_msg)
             raise GremlinParameterError(error_msg)
-        data = {'email': email, 'companyId': company_id, 'teamId': team_id, 'renewToken': renew_token}
-        endpoint = f'/users/renew/rbac'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        data = {
+            "email": email,
+            "companyId": company_id,
+            "teamId": team_id,
+            "renewToken": renew_token,
+        }
+        endpoint = f"/users/renew/rbac"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_user_self', ('',), ('',))
+    @register_cli_action("get_user_self", ("",), ("",))
     def get_user_self(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = f'/users/self'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "GET"
+        endpoint = f"/users/self"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('update_user_self', ('body',), ('',))
+    @register_cli_action("update_user_self", ("body",), ("",))
     def get_user_self(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'PATCH'
+        method = "PATCH"
         data = cls._error_if_not_json_body(**kwargs)
-        endpoint = f'/users/self'
-        payload = cls._payload(**{'headers': https_client.header(), 'body': data})
+        endpoint = f"/users/self"
+        payload = cls._payload(**{"headers": https_client.header(), "body": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_user_session', ('',), ('getCompanySession',))
+    @register_cli_action("get_user_session", ("",), ("getCompanySession",))
     def get_user_session(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        get_company_session = kwargs.get('getCompanySession', None)
-        endpoint = f'/users/sessions'
+        method = "GET"
+        get_company_session = kwargs.get("getCompanySession", None)
+        endpoint = f"/users/sessions"
         if get_company_session:
-            endpoint += f'/?getCompanySession=true'
-        payload = cls._payload(**{'headers': https_client.header()})
+            endpoint += f"/?getCompanySession=true"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
 
 class GremlinAPIUsersAuth(GremlinAPI):
-
     @classmethod
-    @register_cli_action('auth_user', ('email', 'password', 'companyName',), ('getCompanySession',))
+    @register_cli_action(
+        "auth_user",
+        (
+            "email",
+            "password",
+            "companyName",
+        ),
+        ("getCompanySession",),
+    )
     def auth_user(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'email': cls._error_if_not_param('email', **kwargs),
-            'password': cls._error_if_not_param('password', **kwargs),
-            'companyName': cls._error_if_not_param('companyName', **kwargs)
+            "email": cls._error_if_not_param("email", **kwargs),
+            "password": cls._error_if_not_param("password", **kwargs),
+            "companyName": cls._error_if_not_param("companyName", **kwargs),
         }
-        get_company_session = cls._info_if_not_param('getCompanySession', **kwargs)
-        payload = cls._payload(**{'data': data})
-        endpoint = '/users/auth'
+        get_company_session = cls._info_if_not_param("getCompanySession", **kwargs)
+        payload = cls._payload(**{"data": data})
+        endpoint = "/users/auth"
         if get_company_session:
-            endpoint += '/?getCompanySession=true'
+            endpoint += "/?getCompanySession=true"
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('auth_user_sso', ('accessToken', 'email', 'provider', 'companyName'), ('getCompanySession',))
+    @register_cli_action(
+        "auth_user_sso",
+        ("accessToken", "email", "provider", "companyName"),
+        ("getCompanySession",),
+    )
     def auth_user_sso(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'accessToken': cls._error_if_not_param('accessToken', **kwargs),
-            'email': cls._error_if_not_param('email', **kwargs),
-            'provider': cls._error_if_not_param('provider', **kwargs),
-            'companyName': cls._error_if_not_param('companyName', **kwargs)
+            "accessToken": cls._error_if_not_param("accessToken", **kwargs),
+            "email": cls._error_if_not_param("email", **kwargs),
+            "provider": cls._error_if_not_param("provider", **kwargs),
+            "companyName": cls._error_if_not_param("companyName", **kwargs),
         }
-        get_company_session = cls._info_if_not_param('getCompanySession', **kwargs)
-        payload = cls._payload(**{'data': data})
-        endpoint = '/users/auth'
+        get_company_session = cls._info_if_not_param("getCompanySession", **kwargs)
+        payload = cls._payload(**{"data": data})
+        endpoint = "/users/auth"
         if get_company_session:
-            endpoint += '/?getCompanySession=true'
+            endpoint += "/?getCompanySession=true"
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('invalidate_session', ('',), ('',))
+    @register_cli_action("invalidate_session", ("",), ("",))
     def invalidate_session(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'DELETE'
-        endpoint = '/users/auth'
-        payload = cls._payload(**{'headers': https_client.header()})
+        method = "DELETE"
+        endpoint = "/users/auth"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_company_affiliations', ('email',), ('',))
-    def get_company_affiliations(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
+    @register_cli_action("get_company_affiliations", ("email",), ("",))
+    def get_company_affiliations(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
         email = cls._error_if_not_email(**kwargs)
-        endpoint = f'/users/auth/emailCompanies/?email={email}'
-        payload = cls._payload(**{'headers': https_client.header()})
+        endpoint = f"/users/auth/emailCompanies/?email={email}"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('get_saml_metadata', ('',), ('',))
+    @register_cli_action("get_saml_metadata", ("",), ("",))
     def get_saml_metadata(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = '/users/auth/saml/metadata'
+        method = "GET"
+        endpoint = "/users/auth/saml/metadata"
         (resp, body) = https_client.api_call(method, endpoint)
         return body
 
-class GremlinAPIUsersAuthMFA(GremlinAPI):
 
+class GremlinAPIUsersAuthMFA(GremlinAPI):
     @classmethod
-    @register_cli_action('auth_user_mfa', ('email', 'password', 'token', 'company',), ('getCompanySession',))
+    @register_cli_action(
+        "auth_user_mfa",
+        (
+            "email",
+            "password",
+            "token",
+            "company",
+        ),
+        ("getCompanySession",),
+    )
     def auth_user(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'email': kwargs.get('email', None),
-            'password': kwargs.get('password', None),
-            'token': kwargs.get('token', None),
-            'companyName': kwargs.get('company', None)
+            "email": kwargs.get("email", None),
+            "password": kwargs.get("password", None),
+            "token": kwargs.get("token", None),
+            "companyName": kwargs.get("company", None),
         }
-        get_company_session = cls._info_if_not_param('getCompanySession', **kwargs)
-        payload = cls._payload(**{'data': data})
-        endpoint = '/users/auth/mfa/auth'
+        get_company_session = cls._info_if_not_param("getCompanySession", **kwargs)
+        payload = cls._payload(**{"data": data})
+        endpoint = "/users/auth/mfa/auth"
         if get_company_session:
-            endpoint += '/?getCompanySession=true'
+            endpoint += "/?getCompanySession=true"
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
     def auth_user_mfa(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
         # Alias to auth_user
         return cls.auth_user(https_client, *args, **kwargs)
 
     @classmethod
-    @register_cli_action('get_mfa_status', ('email',), (''))
+    @register_cli_action("get_mfa_status", ("email",), (""))
     def get_mfa_status(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
+        method = "GET"
         email = cls._error_if_not_email(**kwargs)
-        endpoint = f'/users/auth/mfa/{email}/enabled'
+        endpoint = f"/users/auth/mfa/{email}/enabled"
         (resp, body) = https_client.api_call(method, endpoint)
         return body
 
     @classmethod
-    @register_cli_action('get_user_mfa_status', ('',), ('',))
-    def get_user_mfa_status(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'GET'
-        endpoint = '/users/auth/mfa/info'
-        payload = cls._payload(**{'headers': https_client.header()})
+    @register_cli_action("get_user_mfa_status", ("",), ("",))
+    def get_user_mfa_status(
+        cls, https_client=get_gremlin_httpclient(), *args, **kwargs
+    ):
+        method = "GET"
+        endpoint = "/users/auth/mfa/info"
+        payload = cls._payload(**{"headers": https_client.header()})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('disable_mfa', ('email', 'password', 'token',), ('',))
+    @register_cli_action(
+        "disable_mfa",
+        (
+            "email",
+            "password",
+            "token",
+        ),
+        ("",),
+    )
     def disable_mfa(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'email': cls._error_if_not_email(**kwargs),
-            'password': cls._error_if_not_param('password', **kwargs),
-            'token': cls._error_if_not_param('token', **kwargs)
+            "email": cls._error_if_not_email(**kwargs),
+            "password": cls._error_if_not_param("password", **kwargs),
+            "token": cls._error_if_not_param("token", **kwargs),
         }
-        endpoint = '/users/auth/mfa/disable'
-        payload = cls._payload(**{'data': data})
+        endpoint = "/users/auth/mfa/disable"
+        payload = cls._payload(**{"data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('force_disable_mfa', ('email',), ('',))
+    @register_cli_action("force_disable_mfa", ("email",), ("",))
     def force_disable_mfa(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
-        data = {
-            'email': cls._error_if_not_email(**kwargs)
-        }
-        endpoint = '/users/auth/mfa/forceDisable'
-        payload = cls._payload(**{'headers': https_client.header(), 'data': data})
+        method = "POST"
+        data = {"email": cls._error_if_not_email(**kwargs)}
+        endpoint = "/users/auth/mfa/forceDisable"
+        payload = cls._payload(**{"headers": https_client.header(), "data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('enable_mfa', ('email', 'password', 'provider',), ('',))
+    @register_cli_action(
+        "enable_mfa",
+        (
+            "email",
+            "password",
+            "provider",
+        ),
+        ("",),
+    )
     def enable_mfa(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'email': cls._error_if_not_email(**kwargs),
-            'password': cls._error_if_not_param('password', **kwargs),
-            'provider': cls._error_if_not_param('provider', **kwargs)
+            "email": cls._error_if_not_email(**kwargs),
+            "password": cls._error_if_not_param("password", **kwargs),
+            "provider": cls._error_if_not_param("provider", **kwargs),
         }
-        endpoint = '/users/auth/mfa/enable'
-        payload = cls._payload(**{'data': data})
+        endpoint = "/users/auth/mfa/enable"
+        payload = cls._payload(**{"data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
 
     @classmethod
-    @register_cli_action('validate_token', ('email', 'token',), (''))
+    @register_cli_action(
+        "validate_token",
+        (
+            "email",
+            "token",
+        ),
+        (""),
+    )
     def validate_token(cls, https_client=get_gremlin_httpclient(), *args, **kwargs):
-        method = 'POST'
+        method = "POST"
         data = {
-            'email': cls._error_if_not_email(**kwargs),
-            'token': cls._error_if_not_param('token', **kwargs)
+            "email": cls._error_if_not_email(**kwargs),
+            "token": cls._error_if_not_param("token", **kwargs),
         }
-        endpoint = '/users/auth/mfa/validate'
-        payload = cls._payload(**{'data': data})
+        endpoint = "/users/auth/mfa/validate"
+        payload = cls._payload(**{"data": data})
         (resp, body) = https_client.api_call(method, endpoint, **payload)
         return body
-
```

### Comparing `gremlinapi-0.9.2/gremlinapi.egg-info/PKG-INFO` & `gremlinapi-0.9.7/gremlinapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinapi
-Version: 0.9.2
+Version: 0.9.7
 Summary: Gremlin library for Python
 Home-page: https://github.com/gremlin/gremlin-python/
 Author: Kyle Hultman
 Author-email: kyle@gremlin.com
 License: Apache 2.0
 Description: # gremlin-python
```

### Comparing `gremlinapi-0.9.2/gremlinapi.egg-info/SOURCES.txt` & `gremlinapi-0.9.7/gremlinapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gremlinapi-0.9.2/tests/test_httpclient.py` & `gremlinapi-0.9.7/tests/test_httpclient.py`

 * *Files identical despite different names*

