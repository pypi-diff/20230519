# Comparing `tmp/autotraders-1.0.4.tar.gz` & `tmp/autotraders-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.0.4.tar", last modified: Mon May 15 17:30:21 2023, max compression
+gzip compressed data, was "autotraders-1.0.5.tar", last modified: Fri May 19 00:43:06 2023, max compression
```

## Comparing `autotraders-1.0.4.tar` & `autotraders-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.031735 autotraders-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-15 17:30:07.000000 autotraders-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 17:30:21.031735 autotraders-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 17:30:07.000000 autotraders-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.027735 autotraders-1.0.4/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.031735 autotraders-1.0.4/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.031735 autotraders-1.0.4/autotraders/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-15 17:30:07.000000 autotraders-1.0.4/autotraders/waypoint_types/shipyard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.031735 autotraders-1.0.4/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 17:30:21.000000 autotraders-1.0.4/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 17:30:21.000000 autotraders-1.0.4/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:30:21.000000 autotraders-1.0.4/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 17:30:21.000000 autotraders-1.0.4/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 17:30:07.000000 autotraders-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:30:21.031735 autotraders-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:30:21.031735 autotraders-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-15 17:30:07.000000 autotraders-1.0.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 00:42:53.000000 autotraders-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 00:43:06.461463 autotraders-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 00:42:53.000000 autotraders-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.457463 autotraders-1.0.5/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/shipyard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 00:42:53.000000 autotraders-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:43:06.461463 autotraders-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-19 00:42:53.000000 autotraders-1.0.5/tests/test_util.py
```

### Comparing `autotraders-1.0.4/LICENSE` & `autotraders-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/PKG-INFO` & `autotraders-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.4
+Version: 1.0.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.4/README.md` & `autotraders-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/autotraders/agent.py` & `autotraders-1.0.5/autotraders/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import math
+
 import requests
 
 from autotraders.ship import get_all_ships
 from autotraders.contract import get_all_contracts
 
 
 class Agent:
     def __init__(self, session: requests.Session, update=True):
         self.session = session
+        self.credits = math.nan
         if update:
             self.update()
 
     def update(self, data=None):
+        """Uses 3 API requests to get all agent details"""
         if data is None:
             r = self.session.get("https://api.spacetraders.io/v2/my/agent")
             j = r.json()
             if "error" in j:
                 raise IOError(j["error"]["message"])
             data = j["data"]
         self.account_id = data["accountId"]
```

### Comparing `autotraders-1.0.4/autotraders/contract.py` & `autotraders-1.0.5/autotraders/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,21 @@
             "https://api.spacetraders.io/v2/my/contracts/"
             + self.contract_id
             + "/fulfill"
         ).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
 
+    @staticmethod
+    def all(session):
+        r = session.get("https://api.spacetraders.io/v2/my/contracts")
+        j = r.json()
+        contracts = []
+        for contract in j["data"]:
+            c = Contract(contract["id"], session, False)
+            c.update(contract)
+            contracts.append(c)
+        return contracts
+
 
 def get_all_contracts(session):
-    r = session.get("https://api.spacetraders.io/v2/my/contracts")
-    j = r.json()
-    contracts = []
-    for contract in j["data"]:
-        c = Contract(contract["id"], session, False)
-        c.update(contract)
-        contracts.append(c)
-    return contracts
+    return Contract.all(session)
```

### Comparing `autotraders-1.0.4/autotraders/faction.py` & `autotraders-1.0.5/autotraders/faction.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,23 @@
         self.name = data["name"]
         self.description = data["description"]
         self.headquarters = data["headquarters"]
         self.traits = []
         for trait in data["traits"]:
             self.traits.append(Trait(trait))
 
+    @staticmethod
+    def all(session):
+        r = session.get("https://api.spacetraders.io/v2/factions")
+        j = r.json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+        factions = []
+        for f in j["data"]:
+            faction = Faction(f["symbol"], session, False)
+            faction.update(f)
+            factions.append(faction)
+        return factions
+
 
 def get_all_factions(session):
-    r = session.get("https://api.spacetraders.io/v2/factions")
-    j = r.json()
-    if "error" in j:
-        raise IOError(j["error"]["message"])
-    factions = []
-    for f in j["data"]:
-        faction = Faction(f["symbol"], session, False)
-        faction.update(f)
-        factions.append(faction)
-    return factions
+    return Faction.all(session)
```

### Comparing `autotraders-1.0.4/autotraders/ship/__init__.py` & `autotraders-1.0.5/autotraders/ship/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 
 
 class Cargo:
     def __init__(self, j):
         self.capacity = j["capacity"]
         inventory = j["inventory"]
         self.inventory = {}
+        self.current = 0
         for symbol in inventory:
             self.inventory[symbol["symbol"]] = symbol["units"]
+            self.current += symbol["units"]
 
 
 class Route:
     def __init__(self, data):
         self.destination = data["destination"]
         self.departure = data["departure"]["symbol"]
         self.moving = self.destination == self.departure
@@ -303,19 +305,23 @@
         for ship in j["data"]["ships"]:
             s = Ship(ship["data"], self.session, False)
             s.update(ship)
             ships.append(s)
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return ships
 
+    @staticmethod
+    def all(session):
+        r = session.get("https://api.spacetraders.io/v2/my/ships")
+        j = r.json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+        ships = []
+        for ship in j["data"]:
+            s = Ship(ship["symbol"], session, False)
+            s.update(ship)
+            ships.append(s)
+        return ships
+
 
 def get_all_ships(session):
-    r = session.get("https://api.spacetraders.io/v2/my/ships")
-    j = r.json()
-    if "error" in j:
-        raise IOError(j["error"]["message"])
-    ships = []
-    for ship in j["data"]:
-        s = Ship(ship["symbol"], session, False)
-        s.update(ship)
-        ships.append(s)
-    return ships
+    return Ship.all(session)
```

### Comparing `autotraders-1.0.4/autotraders/ship/ship_components.py` & `autotraders-1.0.5/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/autotraders/system.py` & `autotraders-1.0.5/autotraders/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import math
+
 import requests
 
 from autotraders.waypoint import Waypoint
 
 
 class System:
     def __init__(self, symbol, session: requests.Session, update=True):
         self.session = session
         self.symbol = symbol
-        self.waypoints = []
+        self.x = math.nan
+        self.y = math.nan
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
             r = self.session.get(
                 "https://api.spacetraders.io/v2/systems/" + self.symbol
@@ -23,17 +26,21 @@
         self.factions = data["factions"]
         self.star_type = data["type"]
         for w in data["waypoints"]:
             waypoint = Waypoint(w["symbol"], self.session, False)
             waypoint.update(w)
             self.waypoints.append(waypoint)
 
+    @staticmethod
+    def all(session, page=1):
+        r = session.get("https://api.spacetraders.io/v2/systems?limit=20&page=" + str(page))
+        j = r.json()["data"]
+        systems = []
+        for system in j:
+            s = System(system["symbol"], session, False)
+            s.update(system)
+            systems.append(s)
+        return systems, r.json()["meta"]["total"]
+
 
 def list_systems(session, page=1) -> (list[System], int):
-    r = session.get("https://api.spacetraders.io/v2/systems?limit=20&page=" + str(page))
-    j = r.json()["data"]
-    systems = []
-    for system in j:
-        s = System(system["symbol"], session, False)
-        s.update(system)
-        systems.append(s)
-    return systems, r.json()["meta"]["total"]
+    System.all(session, page)
```

### Comparing `autotraders-1.0.4/autotraders/waypoint.py` & `autotraders-1.0.5/autotraders/waypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from autotraders.trait import Trait
 
 
 class Waypoint:
     def __init__(self, symbol, session: requests.Session, update=True):
         self.session = session
         self.symbol = symbol
-        self.marketplace = False
-        self.shipyard = False
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
             split = self.symbol.split("-")
-            system_symbol = split[0] + "-" + split[1]
+            self.sector = split[0]
+            self.system_symbol = split[0] + "-" + split[1]
             waypoint_symbol = self.symbol
             data = self.session.get(
                 "https://api.spacetraders.io/v2/systems/"
-                + system_symbol
+                + self.system_symbol
                 + "/waypoints/"
                 + waypoint_symbol
             ).json()["data"]
         self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
         if "faction" in data:
@@ -31,23 +30,27 @@
         else:
             self.faction = None
         self.traits = []
         if "traits" in data:
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
         self.marketplace = (
-            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
-            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+                len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
         )
 
+    @staticmethod
+    def all(system, session):
+        r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
+        data = r.json()["data"]
+        waypoints = []
+        for w in data:
+            waypoint = Waypoint(w["symbol"], session, False)
+            waypoint.update(w)
+            waypoints.append(waypoint)
+        return waypoints
+
 
 def get_all_waypoints(system, session):
-    r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
-    data = r.json()["data"]
-    waypoints = []
-    for w in data:
-        waypoint = Waypoint(w["symbol"], session, False)
-        waypoint.update(w)
-        waypoints.append(waypoint)
-    return waypoints
+    return Waypoint.all(system, session)
```

### Comparing `autotraders-1.0.4/autotraders/waypoint_types/jumpgate.py` & `autotraders-1.0.5/autotraders/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/autotraders/waypoint_types/marketplace.py` & `autotraders-1.0.5/autotraders/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/autotraders/waypoint_types/shipyard.py` & `autotraders-1.0.5/autotraders/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/autotraders.egg-info/PKG-INFO` & `autotraders-1.0.5/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.4
+Version: 1.0.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.4/autotraders.egg-info/SOURCES.txt` & `autotraders-1.0.5/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.4/pyproject.toml` & `autotraders-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

