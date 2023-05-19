# Comparing `tmp/mqtt-entity-0.0.2.tar.gz` & `tmp/mqtt-entity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-entity-0.0.2.tar", last modified: Sun Apr 16 22:23:41 2023, max compression
+gzip compressed data, was "mqtt-entity-0.0.3.tar", last modified: Fri May 19 12:44:55 2023, max compression
```

## Comparing `mqtt-entity-0.0.2.tar` & `mqtt-entity-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/mqtt_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/mqtt_entity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/mqtt_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:23:41.000000 mqtt-entity-0.0.2/mqtt_entity.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:41.242721 mqtt-entity-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-16 22:23:32.000000 mqtt-entity-0.0.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/mqtt_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/mqtt_entity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/mqtt_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:44:55.000000 mqtt-entity-0.0.3/mqtt_entity.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:44:55.621442 mqtt-entity-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 12:44:42.000000 mqtt-entity-0.0.3/tests/test_helpers.py
```

### Comparing `mqtt-entity-0.0.2/LICENSE` & `mqtt-entity-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.2/PKG-INFO` & `mqtt-entity-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-entity
-Version: 0.0.2
+Version: 0.0.3
 Summary: MQTT client to manage Home Assistant entities via MQTT
 Home-page: https://github.com/kellerza/mqtt-entity/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: home-assistant,mqtt,library,discovery,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mqtt-entity-0.0.2/README.md` & `mqtt-entity-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.2/mqtt_entity/client.py` & `mqtt-entity-0.0.3/mqtt_entity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """MQTTClient."""
 import asyncio
 import inspect
 import logging
 from json import dumps
-from typing import Any, Callable, Optional, Sequence
+from typing import Any, Callable, Optional, Sequence, Union
 
 from paho.mqtt.client import Client, MQTTMessage  # type: ignore
 
 from mqtt_entity.entities import Availability, Entity
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -76,18 +76,24 @@
         def _stop() -> None:
             # Do not disconnect, we want the broker to always publish will
             self._client.loop_stop()
 
         await asyncio.get_running_loop().run_in_executor(None, _stop)
 
     async def publish(
-        self, topic: str, payload: Optional[str], qos: int = 0, retain: bool = False
+        self,
+        topic: Union[str, Entity],
+        payload: Optional[str],
+        qos: int = 0,
+        retain: bool = False,
     ) -> None:
         """Publish a MQTT message."""
         # async with self._paho_lock:
+        if isinstance(topic, Entity):
+            topic = topic.state_topic
         if not isinstance(qos, int):
             qos = 0
         if retain:
             qos = 1
         _LOGGER.debug(
             "MQTT: Publish %s%s %s, %s", qos, "R" if retain else "", topic, payload
         )
```

### Comparing `mqtt-entity-0.0.2/mqtt_entity/entities.py` & `mqtt-entity-0.0.3/mqtt_entity/entities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,159 @@
 """MQTT entities."""
 import inspect
 import logging
 from typing import Any, Callable, Optional, Sequence, Union
 
-import attr
+import attrs
 from attrs import validators
 
-from mqtt_entity.utils import required
+from mqtt_entity.utils import BOOL_OFF, BOOL_ON, required
 
 _LOGGER = logging.getLogger(__name__)
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
-@attr.define
+@attrs.define
 class Device:
     """A Home Assistant Device, used to group entities."""
 
-    identifiers: list[Union[str, tuple[str, Any]]] = attr.field(
+    identifiers: list[Union[str, tuple[str, Any]]] = attrs.field(
         validator=[validators.instance_of(list), validators.min_len(1)]
     )
-    connections: list[str] = attr.field(factory=list)
-    configuration_url: str = attr.field(default="")
-    manufacturer: str = attr.field(default="")
-    model: str = attr.field(default="")
-    name: str = attr.field(default="")
-    suggested_area: str = attr.field(default="")
-    sw_version: str = attr.field(default="")
-    via_device: str = attr.field(default="")
+    connections: list[str] = attrs.field(factory=list)
+    configuration_url: str = attrs.field(default="")
+    manufacturer: str = attrs.field(default="")
+    model: str = attrs.field(default="")
+    name: str = attrs.field(default="")
+    suggested_area: str = attrs.field(default="")
+    sw_version: str = attrs.field(default="")
+    via_device: str = attrs.field(default="")
 
     @property
     def id(self) -> str:  # pylint: disable=invalid-name
         """The device identifier."""
         return str(self.identifiers[0])
 
 
-@attr.define
+@attrs.define
 class Availability:
     """Represent Home Assistant entity availability."""
 
-    topic: str = attr.field()
-    payload_available: str = attr.field(default="online")
-    payload_not_available: str = attr.field(default="offline")
-    value_template: str = attr.field(default="")
+    topic: str = attrs.field()
+    payload_available: str = attrs.field(default="online")
+    payload_not_available: str = attrs.field(default="offline")
+    value_template: str = attrs.field(default="")
 
 
-@attr.define
+@attrs.define
 class Entity:
     """A generic Home Assistant entity used as the base class for other entities."""
 
-    unique_id: str = attr.field()
-    device: Device = attr.field()
-    state_topic: str = attr.field()
-    name: str = attr.field()
-    availability: list[Availability] = attr.field(factory=list)
-    availability_mode: str = attr.field(default="")
-    device_class: str = attr.field(default="")
-    unit_of_measurement: str = attr.field(default="")
-    state_class: str = attr.field(default="")
-    expire_after: int = attr.field(default=0)
+    unique_id: str = attrs.field()
+    device: Device = attrs.field()
+    state_topic: str = attrs.field()
+    name: str = attrs.field()
+    availability: list[Availability] = attrs.field(factory=list)
+    availability_mode: str = attrs.field(default="")
+    device_class: str = attrs.field(default="")
+    unit_of_measurement: str = attrs.field(default="")
+    state_class: str = attrs.field(default="")
+    expire_after: int = attrs.field(default=0)
     """Unavailable if not updated."""
-    enabled_by_default: bool = attr.field(default=True)
-    entity_category: str = attr.field(default="")
-    icon: str = attr.field(default="")
+    enabled_by_default: bool = attrs.field(default=True)
+    entity_category: str = attrs.field(default="")
+    icon: str = attrs.field(default="")
+    attributes_topic: str = attrs.field(default="")
+    """Used by the set_attributes helper."""
 
     _path = ""
 
     def __attrs_post_init__(self) -> None:
         """Init the class."""
         if not self._path:
             raise TypeError(f"Do not instantiate {self.__class__.__name__} directly")
         if not self.state_class and self.device_class == "energy":
             self.state_class = "total_increasing"
 
     @property
     def asdict(self) -> dict:
         """Represent the entity as a dictionary, without empty values and defaults."""
 
-        def _filter(atrb: attr.Attribute, value: Any) -> bool:
+        def _filter(atrb: attrs.Attribute, value: Any) -> bool:
             return (
                 bool(value) and atrb.default != value and not inspect.isfunction(value)
             )
 
-        return attr.asdict(self, filter=_filter)
+        return attrs.asdict(self, filter=_filter)
 
     @property
     def topic(self) -> str:
         """Discovery topic."""
         uid, did = self.unique_id, self.device.id
         if uid.startswith(did):
             uid = uid[len(did) :].strip("_")
         return f"homeassistant/{self._path}/{did}/{uid}/config"
 
 
-@attr.define
+@attrs.define
 class SensorEntity(Entity):
     """A Home Assistant Sensor entity."""
 
     _path = "sensor"
 
 
-@attr.define
+@attrs.define
 class BinarySensorEntity(Entity):
     """A Home Assistant Binary Sensor entity."""
 
-    payload_on: str = attr.field(default="ON")
-    payload_off: str = attr.field(default="OFF")
+    payload_on: str = attrs.field(default=BOOL_ON)
+    payload_off: str = attrs.field(default=BOOL_OFF)
 
     _path = "binary_sensor"
 
 
-@attr.define
+@attrs.define
 class RWEntity(Entity):
-    """Read/Write entity base class."""
+    """Read/Write entity base class.
 
-    command_topic: str = attr.field(
+    This will default to a text entity.
+    """
+
+    command_topic: str = attrs.field(
         default="", validator=(validators.instance_of(str), validators.min_len(2))
     )
 
-    on_change: Optional[Callable] = attr.field(default=None)
+    on_change: Optional[Callable] = attrs.field(default=None)
+
+    _path = "text"
 
 
-@attr.define
+@attrs.define
 class SelectEntity(RWEntity):
     """A HomeAssistant Select entity."""
 
-    options: Sequence[str] = attr.field(default=None, validator=required)
+    options: Sequence[str] = attrs.field(default=None, validator=required)
 
     _path = "select"
 
 
-@attr.define
+@attrs.define
 class SwitchEntity(RWEntity):
-    """A Home Assistant Binary Sensor entity."""
+    """A Home Assistant Switch entity."""
 
-    payload_on: Union[str, int] = attr.field(default=1)
-    payload_off: Union[str, int] = attr.field(default=0)
+    payload_on: str = attrs.field(default=BOOL_ON)
+    payload_off: str = attrs.field(default=BOOL_OFF)
 
     _path = "switch"
 
 
-@attr.define
+@attrs.define
 class NumberEntity(RWEntity):
     """A HomeAssistant Number entity."""
 
-    min: float = attr.field(default=0.0)
-    max: float = attr.field(default=100.0)
-    mode: str = attr.field(default="auto")
-    step: float = attr.field(default=1.0)
+    min: float = attrs.field(default=0.0)
+    max: float = attrs.field(default=100.0)
+    mode: str = attrs.field(default="auto")
+    step: float = attrs.field(default=1.0)
 
     _path = "number"
```

### Comparing `mqtt-entity-0.0.2/mqtt_entity.egg-info/PKG-INFO` & `mqtt-entity-0.0.3/mqtt_entity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-entity
-Version: 0.0.2
+Version: 0.0.3
 Summary: MQTT client to manage Home Assistant entities via MQTT
 Home-page: https://github.com/kellerza/mqtt-entity/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: home-assistant,mqtt,library,discovery,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mqtt-entity-0.0.2/setup.cfg` & `mqtt-entity-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 [options.extras_require]
 tests = 
 	pytest
 	pytest-asyncio
 	pytest-cov
 	pytest-github-actions-annotate-failures
 	pylint
-	black==23.1.0
+	black==23.3.0
 
 [isort]
 profile = black
 
 [flake8]
 extend-ignore = E203, E501, W503
```

### Comparing `mqtt-entity-0.0.2/tests/conftest.py` & `mqtt-entity-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.2/tests/test_client.py` & `mqtt-entity-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mqtt-entity-0.0.2/tests/test_entities.py` & `mqtt-entity-0.0.3/tests/test_entities.py`

 * *Files identical despite different names*

