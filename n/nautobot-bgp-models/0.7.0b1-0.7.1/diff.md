# Comparing `tmp/nautobot-bgp-models-0.7.0b1.tar.gz` & `tmp/nautobot_bgp_models-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot-bgp-models-0.7.0b1.tar", max compression
+gzip compressed data, was "nautobot_bgp_models-0.7.1.tar", max compression
```

## Comparing `nautobot-bgp-models-0.7.0b1.tar` & `nautobot_bgp_models-0.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      591 2022-09-20 13:58:04.408465 nautobot-bgp-models-0.7.0b1/LICENSE
--rw-r--r--   0        0        0     3705 2022-09-20 13:58:04.408465 nautobot-bgp-models-0.7.0b1/README.md
--rw-r--r--   0        0        0     1587 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/__init__.py
--rw-r--r--   0        0        0       54 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/__init__.py
--rw-r--r--   0        0        0     1554 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/filter_backends.py
--rw-r--r--   0        0        0     3194 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/nested_serializers.py
--rw-r--r--   0        0        0     9181 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/serializers.py
--rw-r--r--   0        0        0      793 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/urls.py
--rw-r--r--   0        0        0     4182 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/views.py
--rw-r--r--   0        0        0     1238 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/choices.py
--rw-r--r--   0        0        0     1006 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/dolt_compat.py
--rw-r--r--   0        0        0     1332 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filter_extensions.py
--rw-r--r--   0        0        0     8094 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filters.py
--rw-r--r--   0        0        0    18497 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/forms.py
--rw-r--r--   0        0        0    20854 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/__init__.py
--rw-r--r--   0        0        0    22471 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/models.py
--rw-r--r--   0        0        0     4736 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/navigation.py
--rw-r--r--   0        0        0     1148 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/signals.py
--rw-r--r--   0        0        0     7670 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tables.py
--rw-r--r--   0        0        0     2025 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/template_content.py
--rw-r--r--   0        0        0     3134 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html
--rw-r--r--   0        0        0     1309 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html
--rw-r--r--   0        0        0     1875 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html
--rw-r--r--   0        0        0     1507 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
--rw-r--r--   0        0        0      761 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
--rw-r--r--   0        0        0      839 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
--rw-r--r--   0        0        0      918 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
--rw-r--r--   0        0        0      793 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
--rw-r--r--   0        0        0      853 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
--rw-r--r--   0        0        0     3146 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
--rw-r--r--   0        0        0     6203 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html
--rw-r--r--   0        0        0     5349 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html
--rw-r--r--   0        0        0     3419 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html
--rw-r--r--   0        0        0     1085 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html
--rw-r--r--   0        0        0     2504 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html
--rw-r--r--   0        0        0     1112 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html
--rw-r--r--   0        0        0       49 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/__init__.py
--rw-r--r--   0        0        0    25709 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_api.py
--rw-r--r--   0        0        0    22414 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_filters.py
--rw-r--r--   0        0        0    12400 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_forms.py
--rw-r--r--   0        0        0    17933 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_models.py
--rw-r--r--   0        0        0    13861 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_views.py
--rw-r--r--   0        0        0     8872 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/urls.py
--rw-r--r--   0        0        0    16272 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/views.py
--rw-r--r--   0        0        0     2529 2022-09-20 13:58:15.228920 nautobot-bgp-models-0.7.0b1/pyproject.toml
--rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b1/setup.py
--rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-19 07:20:36.080850 nautobot_bgp_models-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4624 2023-05-19 07:20:36.080850 nautobot_bgp_models-0.7.1/README.md
+-rw-r--r--   0        0        0     1587 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/__init__.py
+-rw-r--r--   0        0        0     1554 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/filter_backends.py
+-rw-r--r--   0        0        0     3192 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/nested_serializers.py
+-rw-r--r--   0        0        0     9978 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/serializers.py
+-rw-r--r--   0        0        0      793 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/urls.py
+-rw-r--r--   0        0        0     4182 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/views.py
+-rw-r--r--   0        0        0     1238 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/choices.py
+-rw-r--r--   0        0        0     1005 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/dolt_compat.py
+-rw-r--r--   0        0        0     1332 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/filter_extensions.py
+-rw-r--r--   0        0        0     8094 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/filters.py
+-rw-r--r--   0        0        0    18497 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/forms.py
+-rw-r--r--   0        0        0    20853 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/migrations/__init__.py
+-rw-r--r--   0        0        0    22471 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/models.py
+-rw-r--r--   0        0        0     4736 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/navigation.py
+-rw-r--r--   0        0        0     1148 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/signals.py
+-rw-r--r--   0        0        0     7670 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tables.py
+-rw-r--r--   0        0        0     2025 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/template_content.py
+-rw-r--r--   0        0        0     3134 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html
+-rw-r--r--   0        0        0     1309 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html
+-rw-r--r--   0        0        0     1875 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html
+-rw-r--r--   0        0        0     1507 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
+-rw-r--r--   0        0        0      761 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
+-rw-r--r--   0        0        0      839 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
+-rw-r--r--   0        0        0      918 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
+-rw-r--r--   0        0        0      793 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
+-rw-r--r--   0        0        0      853 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
+-rw-r--r--   0        0        0     3146 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
+-rw-r--r--   0        0        0     6203 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html
+-rw-r--r--   0        0        0     5349 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html
+-rw-r--r--   0        0        0     3419 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html
+-rw-r--r--   0        0        0     1085 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html
+-rw-r--r--   0        0        0     2504 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html
+-rw-r--r--   0        0        0     1112 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html
+-rw-r--r--   0        0        0       49 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/__init__.py
+-rw-r--r--   0        0        0    42478 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_api.py
+-rw-r--r--   0        0        0     1524 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_basic.py
+-rw-r--r--   0        0        0    22414 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_filters.py
+-rw-r--r--   0        0        0    12400 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_forms.py
+-rw-r--r--   0        0        0    17933 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_models.py
+-rw-r--r--   0        0        0    16104 2023-05-19 07:20:36.104849 nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_views.py
+-rw-r--r--   0        0        0     8872 2023-05-19 07:20:36.108850 nautobot_bgp_models-0.7.1/nautobot_bgp_models/urls.py
+-rw-r--r--   0        0        0    16272 2023-05-19 07:20:36.108850 nautobot_bgp_models-0.7.1/nautobot_bgp_models/views.py
+-rw-r--r--   0        0        0     3005 2023-05-19 07:20:51.752883 nautobot_bgp_models-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 nautobot_bgp_models-0.7.1/PKG-INFO
```

### Comparing `nautobot-bgp-models-0.7.0b1/LICENSE` & `nautobot_bgp_models-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/__init__.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     name = "nautobot_bgp_models"
     verbose_name = "BGP Models"
     version = __version__
     author = "Network to Code, LLC"
     description = "Nautobot BGP Models Plugin."
     base_url = "bgp"
     required_settings = []
-    min_version = "1.3.0"
+    min_version = "1.5.4"
     max_version = "1.999"
     default_settings = {
         "default_statuses": {
             "AutonomousSystem": ["active", "available", "planned"],
             "Peering": ["active", "decommissioned", "deprovisioning", "offline", "planned", "provisioning"],
         }
     }
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/filter_backends.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/nested_serializers.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/nested_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "NestedAutonomousSystemSerializer",
     "NestedPeeringRoleSerializer",
     "NestedPeerGroupSerializer",
     "NestedPeerGroupTemplateSerializer",
     "NestedPeerEndpointSerializer",
     "NestedPeeringSerializer",
     "NestedAddressFamilySerializer",
-    "NestedRoutingInstanceSerializer",
+    "NestedBGPRoutingInstanceSerializer",
 )
 
 
 class NestedAutonomousSystemSerializer(WritableNestedSerializer):
     """Nested/brief serializer for AutonomousSystem."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:autonomoussystem-detail")
@@ -51,37 +51,37 @@
 class NestedPeerGroupTemplateSerializer(WritableNestedSerializer):
     """Nested/brief serializer for PeerGroup."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peergrouptemplate-detail")
 
     class Meta:
         model = models.PeerGroupTemplate
-        fields = ["id", "url", "name", "role", "enabled"]
+        fields = ["id", "url", "name"]
 
 
 class NestedPeerEndpointSerializer(WritableNestedSerializer):
     """Nested/brief serializer for PeerEndpoint."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peerendpoint-detail")
 
     class Meta:
         model = models.PeerEndpoint
         fields = ["id", "url"]
 
 
-class NestedRoutingInstanceSerializer(WritableNestedSerializer):
+class NestedBGPRoutingInstanceSerializer(WritableNestedSerializer):
     """Nested/brief serializer for PeerEndpoint."""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nautobot_bgp_models-api:bgproutinginstance-detail"
     )
 
     class Meta:
         model = models.BGPRoutingInstance
-        fields = ["id", "url"]
+        fields = ["display", "id", "url"]
 
 
 class NestedPeeringSerializer(WritableNestedSerializer):
     """Nested/brief serializer for Peering."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peering-detail")
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/serializers.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """REST API serializers for nautobot_bgp_models models."""
 
 from rest_framework import serializers
 
 from nautobot.dcim.api.serializers import NestedDeviceSerializer, NestedInterfaceSerializer
 from nautobot.ipam.api.serializers import NestedVRFSerializer, NestedIPAddressSerializer
-from nautobot.extras.api.customfields import CustomFieldModelSerializer
-from nautobot.extras.api.serializers import TaggedObjectSerializer, StatusModelSerializerMixin, NestedSecretSerializer
+from nautobot.apps.api import (
+    CustomFieldModelSerializerMixin,
+    RelationshipModelSerializerMixin,
+    StatusModelSerializerMixin,
+    TaggedModelSerializerMixin,
+)
+from nautobot.extras.api.serializers import NestedSecretSerializer
 from nautobot.core.settings_funcs import is_truthy
 
 from nautobot.circuits.api.serializers import NestedProviderSerializer
 
 from nautobot_bgp_models import models
 
 # We have to do this wildcard import of nested_serializers for the "brief" API parameter to work automatically.
 from .nested_serializers import *  # noqa:F401,F403 pylint: disable=wildcard-import,unused-wildcard-import
 
 
-class AutonomousSystemSerializer(TaggedObjectSerializer, StatusModelSerializerMixin, CustomFieldModelSerializer):
+class AutonomousSystemSerializer(
+    TaggedModelSerializerMixin,
+    StatusModelSerializerMixin,
+    CustomFieldModelSerializerMixin,
+    RelationshipModelSerializerMixin,
+):
     """REST API serializer for AutonomousSystem records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:autonomoussystem-detail")
     provider = NestedProviderSerializer(required=False, allow_null=True)
 
     class Meta:
         model = models.AutonomousSystem
         fields = ["id", "url", "asn", "description", "status", "provider", "tags"]
 
 
-class PeeringRoleSerializer(CustomFieldModelSerializer):
+class PeeringRoleSerializer(CustomFieldModelSerializerMixin, RelationshipModelSerializerMixin):
     """REST API serializer for PeeringRole records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peeringrole-detail")
 
     class Meta:
         model = models.PeeringRole
         fields = ["id", "url", "name", "slug", "color", "description"]
@@ -52,62 +62,71 @@
                 setattr(instance, field, data["value"])
         return super().to_representation(instance)
 
 
 class ExtraAttributesSerializerMixin(serializers.Serializer):  # pylint: disable=abstract-method
     """Common mixin for BGP Extra Attributes."""
 
-    extra_attributes = serializers.SerializerMethodField(read_only=True)
+    extra_attributes = serializers.JSONField(required=False, allow_null=True)
 
-    def get_extra_attributes(self, instance):
-        """Return either the `display` property of the instance or `str(instance)`."""
-        req = self.context["request"]
+    def to_representation(self, instance):
+        """Render the model instance to a Python dict.
 
+        If `include_inherited` is specified as a request parameter, include object's get_extra_attributes().
+        """
+        req = self.context["request"]
         if hasattr(req, "query_params") and is_truthy(req.query_params.get("include_inherited", False)):
-            return instance.get_extra_attributes()
-
-        return instance.extra_attributes
+            setattr(instance, "extra_attributes", instance.get_extra_attributes())
+        return super().to_representation(instance)
 
 
-class PeerGroupTemplateSerializer(CustomFieldModelSerializer, ExtraAttributesSerializerMixin):
+class PeerGroupTemplateSerializer(
+    CustomFieldModelSerializerMixin, ExtraAttributesSerializerMixin, RelationshipModelSerializerMixin
+):
     """REST API serializer for PeerGroup records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peergrouptemplate-detail")
 
-    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)
+    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)  # noqa: F405
     secret = NestedSecretSerializer(required=False, allow_null=True)
 
     class Meta:
         model = models.PeerGroupTemplate
         fields = [
             "id",
             "url",
             "name",
             "role",
             "description",
             "enabled",
             "autonomous_system",
             "import_policy",
             "export_policy",
+            "extra_attributes",
             "secret",
         ]
 
 
-class PeerGroupSerializer(InheritableFieldsSerializerMixin, CustomFieldModelSerializer, ExtraAttributesSerializerMixin):
+class PeerGroupSerializer(
+    InheritableFieldsSerializerMixin,
+    CustomFieldModelSerializerMixin,
+    ExtraAttributesSerializerMixin,
+    RelationshipModelSerializerMixin,
+):
     """REST API serializer for PeerGroup records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peergroup-detail")
     source_ip = NestedIPAddressSerializer(required=False, allow_null=True)  # noqa: F405
     source_interface = NestedInterfaceSerializer(required=False, allow_null=True)  # noqa: F405
 
-    routing_instance = NestedRoutingInstanceSerializer(required=True)
+    routing_instance = NestedBGPRoutingInstanceSerializer(required=True)  # noqa: F405
 
-    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)
+    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)  # noqa: F405
 
-    template = NestedPeerGroupTemplateSerializer(required=False, allow_null=True)
+    template = NestedPeerGroupTemplateSerializer(required=False, allow_null=True)  # noqa: F405
 
     secret = NestedSecretSerializer(required=False, allow_null=True)
 
     class Meta:
         model = models.PeerGroup
         fields = [
             "id",
@@ -126,28 +145,29 @@
             "import_policy",
             "export_policy",
         ]
 
 
 class PeerEndpointSerializer(
     InheritableFieldsSerializerMixin,
-    TaggedObjectSerializer,
-    CustomFieldModelSerializer,
+    TaggedModelSerializerMixin,
+    CustomFieldModelSerializerMixin,
     ExtraAttributesSerializerMixin,
+    RelationshipModelSerializerMixin,
 ):
     """REST API serializer for PeerEndpoint records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peerendpoint-detail")
     source_ip = NestedIPAddressSerializer(required=False, allow_null=True)  # noqa: F405
     source_interface = NestedInterfaceSerializer(required=False, allow_null=True)  # noqa: F405
     peer = NestedPeerEndpointSerializer(required=False, allow_null=True)  # noqa: F405
     peering = NestedPeeringSerializer(required=True, allow_null=True)  # noqa: F405
-    peer_group = NestedPeerGroupSerializer(required=False, allow_null=True)
-    routing_instance = NestedRoutingInstanceSerializer(required=False, allow_null=True)
-    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)
+    peer_group = NestedPeerGroupSerializer(required=False, allow_null=True)  # noqa: F405
+    routing_instance = NestedBGPRoutingInstanceSerializer(required=False, allow_null=True)  # noqa: F405
+    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)  # noqa: F405
     secret = NestedSecretSerializer(required=False, allow_null=True)
 
     class Meta:
         model = models.PeerEndpoint
         fields = [
             "id",
             "url",
@@ -159,14 +179,15 @@
             "peer",
             "import_policy",
             "export_policy",
             "peering",
             "secret",
             "tags",
             "enabled",
+            "extra_attributes",
         ]
 
     def create(self, validated_data):
         """Create a new PeerEndpoint and update the peer on both sides."""
         record = super().create(validated_data)
         record.peering.update_peers()
         return record
@@ -181,43 +202,46 @@
 
         if peering_has_been_updated:
             result.peering.update_peers()
 
         return result
 
 
-class BGPRoutingInstanceSerializer(CustomFieldModelSerializer, ExtraAttributesSerializerMixin):
+class BGPRoutingInstanceSerializer(
+    CustomFieldModelSerializerMixin, ExtraAttributesSerializerMixin, RelationshipModelSerializerMixin
+):
     """REST API serializer for Peering records."""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nautobot_bgp_models-api:bgproutinginstance-detail"
     )
 
     endpoints = NestedPeerEndpointSerializer(required=False, many=True)  # noqa: F405
 
     device = NestedDeviceSerializer()
 
-    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)
+    autonomous_system = NestedAutonomousSystemSerializer(required=False, allow_null=True)  # noqa: F405
 
     router_id = NestedIPAddressSerializer(required=False, allow_null=True)  # noqa: F405
 
     class Meta:
         model = models.BGPRoutingInstance
         fields = [
             "id",
             "url",
             "device",
             "description",
             "router_id",
             "autonomous_system",
             "endpoints",
+            "extra_attributes",
         ]
 
 
-class PeeringSerializer(CustomFieldModelSerializer, StatusModelSerializerMixin):
+class PeeringSerializer(CustomFieldModelSerializerMixin, StatusModelSerializerMixin, RelationshipModelSerializerMixin):
     """REST API serializer for Peering records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:peering-detail")
 
     endpoints = NestedPeerEndpointSerializer(required=False, many=True)  # noqa: F405
 
     class Meta:
@@ -226,20 +250,23 @@
             "id",
             "url",
             "status",
             "endpoints",
         ]
 
 
-class AddressFamilySerializer(CustomFieldModelSerializer):
+class AddressFamilySerializer(
+    CustomFieldModelSerializerMixin,
+    RelationshipModelSerializerMixin,
+):
     """REST API serializer for AddressFamily records."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:addressfamily-detail")
 
-    routing_instance = NestedRoutingInstanceSerializer(required=True)
+    routing_instance = NestedBGPRoutingInstanceSerializer(required=True)  # noqa: F405
 
     vrf = NestedVRFSerializer(required=False, allow_null=True)
 
     class Meta:
         model = models.AddressFamily
         fields = [
             "id",
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/urls.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/views.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/choices.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/dolt_compat.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/dolt_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     DOLT_AVAILABLE = False
 else:
     DOLT_AVAILABLE = True
 
 
 # Only do this if Dolt is available (aka "version control").
 if DOLT_AVAILABLE:
-
     # Tables used to display diffs
     dolt.register_diff_tables(
         {
             "nautobot_bgp_models": {
                 "bgproutinginstance": tables.BGPRoutingInstanceTable,
                 "autonomoussystem": tables.AutonomousSystemTable,
                 "peeringrole": tables.PeeringRoleTable,
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filter_extensions.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/filter_extensions.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filters.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/forms.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/0001_initial.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import nautobot.extras.models.statuses
 import nautobot.utilities.fields
 import taggit.managers
 import uuid
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("circuits", "0008_add_natural_indexing"),
         ("dcim", "0009_add_natural_indexing"),
         ("extras", "0033_add__optimized_indexing"),
         ("ipam", "0007_add_natural_indexing"),
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/models.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/models.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/navigation.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/signals.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tables.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/template_content.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_api.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,634 +1,544 @@
-"""Unit tests for nautobot_bgp_models."""
+"""Unit test automation for FilterSet classes in nautobot_bgp_models."""
 
 from django.contrib.contenttypes.models import ContentType
-from nautobot.circuits.models import Provider
+from django.test import TestCase
+
+# from nautobot.circuits.models import Provider
 from nautobot.dcim.choices import InterfaceTypeChoices
 from nautobot.dcim.models import Device, DeviceRole, DeviceType, Interface, Manufacturer, Site
 from nautobot.extras.models import Status
 from nautobot.ipam.models import IPAddress
-from nautobot.utilities.testing.api import APIViewTestCases
-
-from nautobot_bgp_models import models
 
-from nautobot_bgp_models import choices
 
+from nautobot_bgp_models import filters, models, choices
 
-class AutonomousSystemAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the AutonomousSystem API."""
 
-    model = models.AutonomousSystem
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = ["asn", "display", "id", "url"]
-    bulk_update_data = {
-        "description": "Reserved for use in documentation/sample code",
-    }
-    choices_fields = ["status"]
+class AutonomousSystemTestCase(TestCase):
+    """Test filtering of AutonomousSystem records."""
 
-    # Nautobot testing doesn't correctly handle the API representation of a Status as a slug instead of a PK yet.
-    validation_excluded_fields = ["status"]
+    queryset = models.AutonomousSystem.objects.all()
+    filterset = filters.AutonomousSystemFilterSet
 
     @classmethod
     def setUpTestData(cls):
+        """One-time class setup to prepopulate required data for tests."""
         status_active = Status.objects.get(slug="active")
         status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
 
+        status_primary_asn = Status.objects.create(name="Primary ASN", slug="primary-asn", color="FFFFFF")
+        status_primary_asn.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
+
+        status_remote_asn = Status.objects.create(name="Remote ASN", slug="remote-asn", color="FFFFFF")
+        status_remote_asn.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
+
         models.AutonomousSystem.objects.create(
             asn=4200000000, status=status_active, description="Reserved for private use"
         )
         models.AutonomousSystem.objects.create(
-            asn=4200000001, status=status_active, description="Also reserved for private use"
+            asn=4200000001, status=status_primary_asn, description="Also reserved for private use"
         )
         models.AutonomousSystem.objects.create(
-            asn=4200000002, status=status_active, description="Another reserved for private use"
+            asn=4200000002, status=status_remote_asn, description="Another reserved for private use"
         )
 
-        cls.create_data = [
-            {"asn": 64496, "status": "active"},
-            {"asn": 65551, "status": "active"},
-            {"asn": 4294967294, "status": "active", "description": "Reserved for private use"},
-        ]
+    def test_id(self):
+        """Test filtering by ID (primary key)."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
+    def test_asn(self):
+        """Test filtering by ASN."""
+        params = {"asn": [4200000000, 4200000001]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
-class PeeringRoleAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the PeeringRole API."""
+    def test_status(self):
+        """Test filtering by status."""
+        params = {"status": ["primary-asn", "remote-asn"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
-    model = models.PeeringRole
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = ["color", "display", "id", "name", "slug", "url"]
-    create_data = [
-        {"name": "Role 1", "slug": "role-1", "color": "ff0000"},
-        {"name": "Role 2", "slug": "role-2", "color": "00ff00"},
-        {"name": "Role 3", "slug": "role-3", "color": "0000ff", "description": "The third role"},
-    ]
-    bulk_update_data = {
-        "color": "112233",
-    }
+
+class PeeringRoleTestCase(TestCase):
+    """Test filtering of PeeringRole records."""
+
+    queryset = models.PeeringRole.objects.all()
+    filterset = filters.PeeringRoleFilterSet
 
     @classmethod
     def setUpTestData(cls):
-        models.PeeringRole.objects.create(name="Alpha", slug="alpha", color="ff0000")
+        """One-time class setup to prepopulate required data for tests."""
+        models.PeeringRole.objects.create(name="Alpha", slug="alpha", color="ff0000", description="Actually omega")
         models.PeeringRole.objects.create(name="Beta", slug="beta", color="00ff00")
         models.PeeringRole.objects.create(name="Gamma", slug="gamma", color="0000ff")
 
+    def test_search(self):
+        """Test text search."""
+        # Match on name/slug (case-insensitive)
+        self.assertEqual(self.filterset({"q": "Alpha"}, self.queryset).qs.count(), 1)
+        self.assertEqual(self.filterset({"q": "ALPHA"}, self.queryset).qs.count(), 1)
+        # Match on description
+        self.assertEqual(self.filterset({"q": "actually"}, self.queryset).qs.count(), 1)
+
+    def test_id(self):
+        """Test filtering by ID (primary key)."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_name(self):
+        """Test filtering by name field."""
+        params = {"name": ["Alpha", "Beta"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_slug(self):
+        """Test filtering by slug field."""
+        params = {"slug": ["alpha", "gamma"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_color(self):
+        """Test filtering by color field."""
+        params = {"color": ["ff0000", "0000ff"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
-class PeerGroupAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the PeerGroup API."""
 
-    model = models.PeerGroup
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = ["display", "enabled", "id", "name", "role", "url"]
-    bulk_update_data = {
-        "description": "Glenn was here.",
-        "enabled": True,
-        "autonomous_system": None,
-    }
+class PeerGroupTestCase(TestCase):
+    """Test filtering of PeerGroup records."""
 
-    # Nautobot testing doesn't correctly handle the API representation of a Status as a slug instead of a PK yet.
-    validation_excluded_fields = ["status"]
+    queryset = models.PeerGroup.objects.all()
+    filterset = filters.PeerGroupFilterSet
 
     @classmethod
     def setUpTestData(cls):
+        """One-time class setup."""
         status_active = Status.objects.get(slug="active")
         status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
 
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
         devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V", slug="csr1000v")
         site = Site.objects.create(name="Site 1", slug="site-1")
         devicerole = DeviceRole.objects.create(name="Router", slug="router", color="ff0000")
-        device = Device.objects.create(
+        cls.device_1 = Device.objects.create(
             device_type=devicetype, device_role=devicerole, name="Device 1", site=site, status=status_active
         )
-        # interface = Interface.objects.create(device=device, name="Loopback1", type=InterfaceTypeChoices.TYPE_VIRTUAL)
-
-        # vrf = VRF.objects.create(name="Ark B")
-        # cls.address = IPAddress.objects.create(
-        #     address="10.1.1.1/24", status=status_active, vrf=vrf, assigned_object=interface
-        # )
-
-        peeringrole = models.PeeringRole.objects.create(name="Internal", slug="internal", color="333333")
 
-        asn_15521 = models.AutonomousSystem.objects.create(
-            asn=15521, status=status_active, description="Hi ex Premium Internet AS!"
-        )
+        cls.asn_1 = models.AutonomousSystem.objects.create(asn=4294967294, status=status_active)
+        asn_2 = models.AutonomousSystem.objects.create(asn=4294967295, status=status_active)
 
-        asn_8545 = models.AutonomousSystem.objects.create(asn=8545, status=status_active, description="Hi ex PL-IX AS!")
+        cls.peeringrole_internal = models.PeeringRole.objects.create(name="Internal", slug="internal", color="333333")
+        peeringrole_external = models.PeeringRole.objects.create(name="External", slug="external", color="ffffff")
 
-        bgp_routing_instance = models.BGPRoutingInstance.objects.create(
+        cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
             description="Hello World!",
-            autonomous_system=asn_8545,
-            device=device,
+            autonomous_system=cls.asn_1,
+            device=cls.device_1,
         )
 
-        cls.create_data = [
-            {
-                "name": "Group A",
-                "routing_instance": bgp_routing_instance.pk,
-                "autonomous_system": asn_15521.pk,
-                "role": peeringrole.pk,
-                "description": "Telephone sanitizers",
-                "enabled": True,
-            },
-            {
-                "name": "Group B",
-                "routing_instance": bgp_routing_instance.pk,
-                "role": peeringrole.pk,
-            },
-            {
-                "name": "Group C",
-                "routing_instance": bgp_routing_instance.pk,
-                "role": peeringrole.pk,
-                "enabled": False,
-            },
-        ]
-
-        # router_id_relation = Relationship.objects.get(slug="bgp_device_router_id")
-        # RelationshipAssociation.objects.create(relationship=router_id_relation, source=device, destination=cls.address)
-
-        # asn_relation = Relationship.objects.get(slug="bgp_asn")
-        # RelationshipAssociation.objects.create(relationship=asn_relation, source=cls.asn, destination=device)
+        models.PeerGroup.objects.create(
+            routing_instance=cls.bgp_routing_instance,
+            name="Group A",
+            role=cls.peeringrole_internal,
+            autonomous_system=cls.asn_1,
+            description="Internal Group",
+        )
+        models.PeerGroup.objects.create(
+            routing_instance=cls.bgp_routing_instance,
+            name="Group B",
+            role=peeringrole_external,
+            autonomous_system=cls.asn_1,
+            enabled=False,
+            description="External Group",
+        )
+        models.PeerGroup.objects.create(
+            routing_instance=cls.bgp_routing_instance,
+            name="Group C",
+            role=cls.peeringrole_internal,
+            autonomous_system=asn_2,
+            description="Internal Group",
+            # vrf=cls.vrf
+        )
+
+    def test_search(self):
+        """Test text search."""
+        # Match on name (case-insensitive)
+        self.assertEqual(self.filterset({"q": "Group A"}, self.queryset).qs.count(), 1)
+        self.assertEqual(self.filterset({"q": "group a"}, self.queryset).qs.count(), 1)
+        self.assertEqual(self.filterset({"q": "Internal Group"}, self.queryset).qs.count(), 2)
+        self.assertEqual(self.filterset({"q": "External Group"}, self.queryset).qs.count(), 1)
+
+    def test_id(self):
+        """Test filtering by ID (primary key)."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_enabled(self):
+        """Test filtering by enabled status."""
+        params = {"enabled": True}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_role(self):
+        """Test filtering by peering role."""
+        params = {"role": [self.peeringrole_internal.slug]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_autonomous_system(self):
+        """Test filtering by autonomous system."""
+        params = {"autonomous_system": [4294967294]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_routing_instance(self):
+        """Test Routing Instance."""
+        self.assertEqual(
+            self.filterset({"routing_instance": self.bgp_routing_instance.pk}, self.queryset).qs.count(), 3
+        )
 
-        models.PeerGroup.objects.create(name="Group 1", role=peeringrole, routing_instance=bgp_routing_instance)
-        models.PeerGroup.objects.create(name="Group 2", role=peeringrole, routing_instance=bgp_routing_instance)
-        models.PeerGroup.objects.create(name="Group 3", role=peeringrole, routing_instance=bgp_routing_instance)
-
-        cls.maxDiff = None
-
-    # @override_settings(EXEMPT_VIEW_PERMISSIONS=[])
-    # def test_get_object_include_inherited(self):
-    #     """Test object retrieval with the `include_inherited` flag."""
-    #     instance = self._get_queryset()[0]
-    #
-    #     # Add object-level permission
-    #     obj_perm = ObjectPermission(
-    #         name="Test permission",
-    #         constraints={"pk": instance.pk},
-    #         actions=["view"],
-    #     )
-    #     obj_perm.save()
-    #     obj_perm.users.add(self.user)
-    #     obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-    #
-    #     url = self._get_detail_url(instance)
-    #     response = self.client.get(url, **self.header)
-    #     self.assertHttpStatus(response, status.HTTP_200_OK)
-    #     # # Properties not set on the instance
-    #     # self.assertIsNone(response.data["autonomous_system"])
-    #     # self.assertIsNone(response.data["router_id"])
-
-
-class PeerEndpointAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the PeerEndpoint API."""
-
-    model = models.PeerEndpoint
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = [
-        "display",
-        # "enabled",
-        "id",
-        # "local_ip",
-        # "peer_group",
-        "url",
-    ]
-    bulk_update_data = {
-        "enabled": False,
-    }
 
-    # Nautobot testing doesn't correctly handle the API representation of a Status as a slug instead of a PK yet.
-    validation_excluded_fields = ["status"]
+class PeerEndpointTestCase(TestCase):
+    """Test filtering of PeerEndpoint records."""
 
-    # TODO(mzb): Fix object changelog issue (2!=1)
-    test_create_object = None
+    queryset = models.PeerEndpoint.objects.all()
+    filterset = filters.PeerEndpointFilterSet
 
     @classmethod
     def setUpTestData(cls):
-        cls.status_active = Status.objects.get(slug="active")
-        cls.status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
-        cls.status_active.content_types.add(ContentType.objects.get_for_model(models.Peering))
-
-        cls.peeringrole = models.PeeringRole.objects.create(name="Internal", slug="internal", color="333333")
-
-        cls.peering = (
-            models.Peering.objects.create(
-                status=cls.status_active,
-            ),
-            models.Peering.objects.create(
-                status=cls.status_active,
-            ),
-            models.Peering.objects.create(
-                status=cls.status_active,
-            ),
-            models.Peering.objects.create(
-                status=cls.status_active,
-            ),
-        )
+        """One-time class setup."""
+        status_active = Status.objects.get(slug="active")
+        status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
 
+        # provider = Provider.objects.create(name="Provider", slug="provider")
+
+        asn = models.AutonomousSystem.objects.create(asn=4294967295, status=status_active)
+        # asn_15521 = models.AutonomousSystem.objects.create(asn=15521, status=status_active, provider=provider)
+
+        peeringrole = models.PeeringRole.objects.create(name="Internal", slug="internal", color="ffffff")
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
         cls.devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V", slug="csr1000v")
         cls.site = Site.objects.create(name="Site 1", slug="site-1")
         cls.devicerole = DeviceRole.objects.create(name="Router", slug="router", color="ff0000")
         device = Device.objects.create(
             device_type=cls.devicetype,
             device_role=cls.devicerole,
             name="Device 1",
             site=cls.site,
-            status=cls.status_active,
+            status=status_active,
         )
         interface = Interface.objects.create(device=device, name="Loopback1", type=InterfaceTypeChoices.TYPE_VIRTUAL)
 
-        # cls.vrf = VRF.objects.create(name="Ark B")
-
-        cls.addresses = (
-            IPAddress.objects.create(
-                address="10.1.1.1/24",
-                status=cls.status_active,
-                assigned_object=interface,
-            ),
-            IPAddress.objects.create(
-                address="10.1.2.1/24",
-                status=cls.status_active,
-                assigned_object=interface,
-            ),
-            IPAddress.objects.create(
-                address="10.1.3.1/24",
-                status=cls.status_active,
-                assigned_object=interface,
-            ),
-            IPAddress.objects.create(
-                address="10.10.1.1/24",
-                status=cls.status_active,
-            ),
-            IPAddress.objects.create(
-                address="10.10.2.1/24",
-                status=cls.status_active,
-            ),
-            IPAddress.objects.create(
-                address="10.10.3.1/24",
-                status=cls.status_active,
-            ),
-        )
-
-        cls.asn = models.AutonomousSystem.objects.create(asn=4294967294, status=cls.status_active)
-
-        provider = Provider.objects.create(name="Provider", slug="provider")
-        cls.provider_asn = models.AutonomousSystem.objects.create(
-            asn=15521,
-            status=cls.status_active,
-            provider=provider,
-        )
+        addresses = [
+            IPAddress.objects.create(address="1.1.1.1/32", status=status_active, assigned_object=interface),
+            IPAddress.objects.create(address="1.1.1.2/32", status=status_active, assigned_object=interface),
+            IPAddress.objects.create(address="1.1.1.3/32", status=status_active),
+        ]
 
         cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
             description="Hello World!",
-            autonomous_system=cls.asn,
+            autonomous_system=asn,
             device=device,
         )
 
-        peergroup = models.PeerGroup.objects.create(
-            name="Group 1",
-            role=cls.peeringrole,
+        cls.peergroup = models.PeerGroup.objects.create(
+            name="Group B",
+            role=peeringrole,
             routing_instance=cls.bgp_routing_instance,
-            # vrf=cls.vrf,
-            # router_id=cls.addresses[3],
-            # autonomous_system=cls.asn,
         )
 
-        # Peering #0
+        peering1 = models.Peering.objects.create(status=status_active)
+        peering2 = models.Peering.objects.create(status=status_active)
+        peering3 = models.Peering.objects.create(status=status_active)
+
         models.PeerEndpoint.objects.create(
             routing_instance=cls.bgp_routing_instance,
-            source_ip=cls.addresses[0],
-            peer_group=peergroup,
-            peering=cls.peering[0],
+            source_ip=addresses[0],
+            autonomous_system=asn,
+            peering=peering1,
         )
         models.PeerEndpoint.objects.create(
-            source_ip=cls.addresses[3],
-            autonomous_system=cls.provider_asn,
-            peering=cls.peering[0],
+            routing_instance=cls.bgp_routing_instance,
+            source_ip=addresses[1],
+            autonomous_system=asn,
+            peer_group=cls.peergroup,
+            peering=peering2,
         )
         models.PeerEndpoint.objects.create(
-            source_ip=cls.addresses[2],
-            autonomous_system=cls.provider_asn,
-            peering=cls.peering[3],
-        )
-        # models.PeerEndpoint.objects.create(
-        #     source_ip=cls.addresses[3],
-        #     autonomous_system=cls.provider_asn,
-        #     peering=cls.peering[3]
-        # )
+            source_ip=addresses[2],
+            peer_group=cls.peergroup,
+            enabled=False,
+            peering=peering3,
+        )
+
+    def test_search(self):
+        """Test text search."""
+        self.assertEqual(self.filterset({"q": "Device 1"}, self.queryset).qs.count(), 2)
+        self.assertEqual(self.filterset({"q": "device 1"}, self.queryset).qs.count(), 2)
+
+    def test_id(self):
+        """Test filtering by ID (primary key)."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_enabled(self):
+        """Test filtering by enabled status."""
+        params = {"enabled": True}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_autonomous_system(self):
+        """Test filtering by autonomous system."""
+        params = {"autonomous_system": [4294967295]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_peer_group(self):
+        """Test filtering by peer-group."""
+        params = {"peer_group": [self.peergroup.pk]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
-        # models.PeerEndpoint.objects.create(local_ip=cls.addresses[2], peer_group=peergroup, peering=cls.peering[1])
 
-        cls.create_data = [
-            # Peering #1
-            {
-                "source_ip": cls.addresses[1].pk,
-                "routing_instance": cls.bgp_routing_instance.pk,
-                "peer_group": peergroup.pk,
-                "peering": cls.peering[1].pk,
-            },
-            {
-                "source_ip": cls.addresses[4].pk,
-                "autonomous_system": cls.provider_asn.pk,
-                "peering": cls.peering[1].pk,
-            },
-            {
-                "source_ip": cls.addresses[2].pk,
-                "routing_instance": cls.bgp_routing_instance.pk,
-                "peer_group": peergroup.pk,
-                "peering": cls.peering[1].pk,
-            },
-        ]
+class PeeringTestCase(TestCase):
+    """Test filtering of Peering records."""
 
-        cls.maxDiff = None
-
-
-#     @override_settings(EXEMPT_VIEW_PERMISSIONS=[])
-#     def test_get_object_include_inherited(self):
-#         """Test object retrieval with the `include_inherited` flag."""
-#         instance = self._get_queryset()[0]
-#
-#         # Add object-level permission
-#         obj_perm = ObjectPermission(
-#             name="Test permission",
-#             constraints={"pk": instance.pk},
-#             actions=["view"],
-#         )
-#         obj_perm.save()
-#         obj_perm.users.add(self.user)
-#         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-#
-#         # Retrieve without inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(url, **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         # Properties not set on the instance
-#         self.assertIsNone(response.data["autonomous_system"])
-#         self.assertIsNone(response.data["router_id"])
-#
-#         # Retrieve with inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(f"{url}?include_inherited", **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         # Properties not set on the instance but inheritable from the parent peer-group
-#         self.assertEqual(self.asn.pk, response.data["autonomous_system"])
-#         self.assertEqual(self.addresses[3].pk, response.data["router_id"])
-#
-#         # Retrieve with explictly excluded inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(f"{url}?include_inherited=false", **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         self.assertIsNone(response.data["autonomous_system"])
-#         self.assertIsNone(response.data["router_id"])
-#
-#     def test_invalid_combinations(self):
-#         """Test various invalid combinations of parameters."""
-#         obj_perm = ObjectPermission(name="Test permission", actions=["add"])
-#         obj_perm.save()
-#         obj_perm.users.add(self.user)
-#         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-#
-#         for data, error_key, error_str in (
-#             (
-#                 # Mismatch between local IP's assigned VRF and the explicitly specified VRF
-#                 {
-#                     "local_ip": self.addresses[0].pk,
-#                     "vrf": VRF.objects.create(name="other_vrf").pk,
-#                     "peering": self.peering[2].pk,
-#                 },
-#                 "__all__",
-#                 "VRF other_vrf was specified, but one or more attributes refer instead to Ark B",
-#             ),
-#         ):
-#             response = self.client.post(self._get_list_url(), data, format="json", **self.header)
-#             self.assertHttpStatus(response, status.HTTP_400_BAD_REQUEST)
-#             self.assertIn(error_key, response.data)
-#             self.assertIn(error_str, str(response.data[error_key][0]))
-#
-#         # TODO: lots more negative test possibilities here...
-
-
-class PeeringAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the Peering API."""
-
-    model = models.Peering
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = ["display", "id", "status", "url"]
-    choices_fields = ["status"]
-
-    # Nautobot testing doesn't correctly handle the API representation of a Status as a slug instead of a PK yet.
-    # Nautobot testing also doesn't correctly handle the reverse-relation that is "endpoints"
-    validation_excluded_fields = ["status", "endpoints"]
+    queryset = models.Peering.objects.all()
+    filterset = filters.PeeringFilterSet
 
     @classmethod
-    def setUpTestData(cls):
+    def setUpTestData(cls):  # pylint: disable=too-many-locals
+        """One-time class setup to prepopulate required data for tests."""
         status_active = Status.objects.get(slug="active")
         status_active.content_types.add(ContentType.objects.get_for_model(models.Peering))
+        status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
+
+        status_reserved = Status.objects.get(slug="reserved")
+        status_reserved.content_types.add(ContentType.objects.get_for_model(models.Peering))
 
-        addresses = (
-            IPAddress.objects.create(address="10.1.1.1/24", status=status_active),
-            IPAddress.objects.create(address="10.1.1.2/24", status=status_active),
-            IPAddress.objects.create(address="10.1.2.2/24", status=status_active),
-            IPAddress.objects.create(address="10.1.2.3/24", status=status_active),
-            IPAddress.objects.create(address="10.1.3.3/24", status=status_active),
-            IPAddress.objects.create(address="10.1.3.4/24", status=status_active),
-            IPAddress.objects.create(address="10.1.1.100/24", status=status_active),
+        asn1 = models.AutonomousSystem.objects.create(asn=65000, status=status_active)
+        asn2 = models.AutonomousSystem.objects.create(asn=66000, status=status_active)
+        asn3 = models.AutonomousSystem.objects.create(asn=12345, status=status_active)
+
+        manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
+        devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V", slug="csr1000v")
+        site = Site.objects.create(name="Site 1", slug="site-1")
+        devicerole = DeviceRole.objects.create(name="Router", slug="router", color="ff0000")
+        device1 = Device.objects.create(
+            device_type=devicetype,
+            device_role=devicerole,
+            name="device1",
+            site=site,
+            status=status_active,
+        )
+        # device2 = Device.objects.create(
+        #     device_type=devicetype,
+        #     device_role=devicerole,
+        #     name="device2",
+        #     site=site,
+        #     status=status_active
+        # )
+        cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
+            description="Hello World!",
+            autonomous_system=asn1,
+            device=device1,
         )
 
-        provider = Provider.objects.create(name="Provider", slug="provider")
-        asn = models.AutonomousSystem.objects.create(asn=15521, status=status_active, provider=provider)
+        interfaces_device1 = [
+            Interface.objects.create(device=device1, name="Loopback0"),
+            Interface.objects.create(device=device1, name="Loopback1"),
+            Interface.objects.create(device=device1, name="Loopback2"),
+        ]
+        # interfaces_device2 = [
+        #     Interface.objects.create(device=device2, name="Loopback0"),
+        #     Interface.objects.create(device=device2, name="Loopback1"),
+        #     Interface.objects.create(device=device2, name="Loopback2"),
+        # ]
 
-        # peeringrole_internal = models.PeeringRole.objects.create(name="Internal", slug="internal", color="333333")
-        # peeringrole_external = models.PeeringRole.objects.create(name="External", slug="external", color="0000ff")
+        addresses = [
+            IPAddress.objects.create(
+                address="10.1.1.1/24",
+                status=status_active,
+                assigned_object=interfaces_device1[0],
+            ),
+            IPAddress.objects.create(
+                address="10.1.1.2/24",
+                status=status_active,
+            ),
+            IPAddress.objects.create(
+                address="10.1.1.3/24",
+                status=status_active,
+                assigned_object=interfaces_device1[1],
+            ),
+            IPAddress.objects.create(
+                address="10.1.1.4/24",
+                status=status_reserved,
+            ),
+            IPAddress.objects.create(
+                address="10.1.1.5/24",
+                status=status_active,
+                assigned_object=interfaces_device1[2],
+            ),
+            IPAddress.objects.create(
+                address="10.1.1.6/24",
+                status=status_reserved,
+            ),
+        ]
 
-        peering_1 = models.Peering.objects.create(
-            status=status_active,
+        # peeringrole_internal = models.PeeringRole.objects.create(name="Internal", slug="internal", color="ffffff")
+        # peeringrole_external = models.PeeringRole.objects.create(name="External", slug="external", color="ffffff")
+
+        peerings = [
+            models.Peering.objects.create(status=status_active),
+            models.Peering.objects.create(status=status_active),
+            models.Peering.objects.create(status=status_reserved),
+        ]
+
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[0],
+            peering=peerings[0],
+            autonomous_system=asn1,
         )
-        peering_2 = models.Peering.objects.create(
-            status=status_active,
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[1],
+            peering=peerings[0],
+            autonomous_system=asn1,
         )
-        peering_3 = models.Peering.objects.create(
-            status=status_active,
+
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[2],
+            peering=peerings[1],
+            autonomous_system=asn1,
         )
-        peerendpoints = (
-            models.PeerEndpoint.objects.create(source_ip=addresses[0], autonomous_system=asn, peering=peering_1),
-            models.PeerEndpoint.objects.create(source_ip=addresses[1], autonomous_system=asn, peering=peering_1),
-            models.PeerEndpoint.objects.create(source_ip=addresses[2], autonomous_system=asn, peering=peering_2),
-            models.PeerEndpoint.objects.create(source_ip=addresses[3], autonomous_system=asn, peering=peering_2),
-            models.PeerEndpoint.objects.create(source_ip=addresses[4], autonomous_system=asn, peering=peering_3),
-            models.PeerEndpoint.objects.create(source_ip=addresses[5], autonomous_system=asn, peering=peering_3),
-        )
-
-        peerendpoints[0].peer = peerendpoints[1]
-        peerendpoints[1].peer = peerendpoints[0]
-
-        peerendpoints[2].peer = peerendpoints[3]
-        peerendpoints[3].peer = peerendpoints[2]
-
-        peerendpoints[4].peer = peerendpoints[5]
-        peerendpoints[5].peer = peerendpoints[4]
-
-        cls.create_data = [
-            {
-                "status": "active",
-            },
-            {
-                "status": "active",
-            },
-            {
-                "status": "active",
-            },
-        ]
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[3],
+            peering=peerings[1],
+            autonomous_system=asn2,
+        )
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[4],
+            peering=peerings[2],
+            autonomous_system=asn1,
+        )
+        models.PeerEndpoint.objects.create(
+            source_ip=addresses[5],
+            peering=peerings[2],
+            autonomous_system=asn3,
+        )
+
+    def test_id(self):
+        """Test filtering by id."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    # def test_role(self):
+    #     """Test filtering by role."""
+    #     params = {"role": ["external"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_status(self):
+        """Test filtering by status."""
+        params = {"status": ["active"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_device(self):
+        """Test filtering by device name."""
+        params = {"device": "device1"}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+        # params = {"device": "device2"}
+        # self.assertEqual(self.filterset(params, self.queryset).qs.count(), 0)
+
+        params = {"device": ["device1", "device2"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    # def test_asn(self):
+    #     """Test filtering by asn name."""
+    #     params = {"asn": [65000]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+    #
+    #     params = {"asn": [66000]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+    #
+    #     params = {"asn": [66000, 12345]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    # def test_address(self):
+    #     """Test filtering by device name."""
+    #     params = {"address": ["10.1.1.1"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+    #
+    #     params = {"address": ["10.1.1.1/32"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 0)
+    #
+    #     params = {"address": ["10.1.1.1/24"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+    #
+    #     # Both IP addresses are part of the same Peering so only 1 Peering is expected
+    #     params = {"address": ["10.1.1.1", "10.1.1.2"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+    #
+    #     params = {"address": ["10.1.1.3", "10.1.1.5"]}
+    #     self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+
+class AddressFamilyTestCase(TestCase):
+    """Test filtering of AddressFamily records."""
 
-        cls.bulk_update_data = {
-            "status": "provisioning",
-        }
-
-
-class AddressFamilyAPITestCase(APIViewTestCases.APIViewTestCase):
-    """Test the AddressFamily API."""
-
-    model = models.AddressFamily
-    view_namespace = "plugins-api:nautobot_bgp_models"
-    brief_fields = [
-        "afi_safi",
-        "display",
-        "id",
-        "url",
-    ]
-    choices_fields = ["afi_safi"]
+    queryset = models.AddressFamily.objects.all()
+    filterset = filters.AddressFamilyFilterSet
 
     @classmethod
-    def setUpTestData(cls):  # pylint: disable=too-many-locals
+    def setUpTestData(cls):
         status_active = Status.objects.get(slug="active")
+
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
         devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V", slug="csr1000v")
         site = Site.objects.create(name="Site 1", slug="site-1")
         devicerole = DeviceRole.objects.create(name="Router", slug="router", color="ff0000")
-        device = Device.objects.create(device_type=devicetype, device_role=devicerole, name="Device 1", site=site)
+        device1 = Device.objects.create(
+            device_type=devicetype, device_role=devicerole, name="Device 1", site=site, status=status_active
+        )
+        interface = Interface.objects.create(device=device1, name="Loopback1")
+        address = IPAddress.objects.create(address="1.1.1.1/32", status=status_active, assigned_object=interface)
 
-        asn_8545 = models.AutonomousSystem.objects.create(asn=8545, status=status_active, description="Hi ex PL-IX AS!")
+        peeringrole = models.PeeringRole.objects.create(name="Internal", slug="internal", color="ffffff")
 
-        # provider = Provider.objects.create(name="Provider", slug="provider")
-        # asn_15521 = models.AutonomousSystem.objects.create(
-        #     asn=15521,
-        #     status=status_active,
-        #     description="Hi ex Premium Internet AS!",
-        #     provider=provider,
-        # )
+        asn1 = models.AutonomousSystem.objects.create(asn=65000, status=status_active)
 
-        bgp_routing_instance = models.BGPRoutingInstance.objects.create(
+        cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
             description="Hello World!",
-            autonomous_system=asn_8545,
-            device=device,
+            autonomous_system=asn1,
+            device=device1,
         )
 
-        # interface_1 = Interface.objects.create(device=device, name="Loopback1", type=InterfaceTypeChoices.TYPE_VIRTUAL)
-        # interface_2 = Interface.objects.create(device=device, name="Loopback2", type=InterfaceTypeChoices.TYPE_VIRTUAL)
-
-        # addresses = (
-        #     IPAddress.objects.create(
-        #         address="10.1.1.1/24",
-        #         assigned_object=interface_1,
-        #         status=status_active,
-        #     ),
-        #     IPAddress.objects.create(
-        #         address="10.1.1.2/24",
-        #         status=status_active,
-        #     ),
-        # )
-
-        # peeringrole = models.PeeringRole.objects.create(name="Internal", slug="internal", color="333333")
-        # peergroup = models.PeerGroup.objects.create(
-        #     name="Group 1",
-        #     role=peeringrole,
-        #     routing_instance=bgp_routing_instance,
-        # )
+        cls.peergroup = models.PeerGroup.objects.create(
+            routing_instance=cls.bgp_routing_instance,
+            name="Group B",
+            role=peeringrole,
+        )
 
-        # peering = models.Peering.objects.create(status=status_active)
-        # peerendpoint_1 = models.PeerEndpoint.objects.create(
-        #     routing_instance=bgp_routing_instance,
-        #     source_ip=addresses[0],
-        #     peer_group=peergroup,
-        #     peering=peering,
-        # )
-        # peerendpoint_2 = models.PeerEndpoint.objects.create(
-        #     source_ip=addresses[1],
-        #     autonomous_system=asn_15521,
-        #     peering=peering,
-        # )
+        peering = models.Peering.objects.create(status=status_active)
+        cls.endpoint = models.PeerEndpoint.objects.create(
+            routing_instance=cls.bgp_routing_instance,
+            source_ip=address,
+            peering=peering,
+        )
 
         models.AddressFamily.objects.create(
-            routing_instance=bgp_routing_instance,
+            routing_instance=cls.bgp_routing_instance,
             afi_safi=choices.AFISAFIChoices.AFI_IPV4_UNICAST,
-            export_policy="EXPORT_POLICY",
-            import_policy="IMPORT_POLICY",
         )
+
         models.AddressFamily.objects.create(
-            routing_instance=bgp_routing_instance,
-            afi_safi=choices.AFISAFIChoices.AFI_IPV6_UNICAST,
-            export_policy="EXPORT_POLICY",
-            import_policy="IMPORT_POLICY",
+            routing_instance=cls.bgp_routing_instance,
+            afi_safi=choices.AFISAFIChoices.AFI_IPV4_FLOWSPEC,
         )
+
         models.AddressFamily.objects.create(
-            routing_instance=bgp_routing_instance,
-            afi_safi=choices.AFISAFIChoices.AFI_IPV4_MULTICAST,
+            routing_instance=cls.bgp_routing_instance,
+            afi_safi=choices.AFISAFIChoices.AFI_VPNV4_UNICAST,
         )
 
-        cls.create_data = [
-            {
-                "afi_safi": choices.AFISAFIChoices.AFI_IPV4_FLOWSPEC,
-                "routing_instance": bgp_routing_instance.pk,
-                "import_policy": "IMPORT_ALL",
-                "export_policy": "EXPORT_NONE",
-            },
-            {
-                "afi_safi": choices.AFISAFIChoices.AFI_VPNV4_UNICAST,
-                "routing_instance": bgp_routing_instance.pk,
-            },
-            {
-                "afi_safi": choices.AFISAFIChoices.AFI_VPNV6_UNICAST,
-                "routing_instance": bgp_routing_instance.pk,
-            },
-        ]
-
-        cls.bulk_update_data = {
-            "import_policy": "IMPORT_V4",
-            "export_policy": "EXPORT_V4",
-        }
-
-
-#     @override_settings(EXEMPT_VIEW_PERMISSIONS=[])
-#     def test_get_object_include_inherited(self):
-#         """Test object retrieval with the `include_inherited` flag."""
-#         instance = self._get_queryset().get(peer_endpoint__isnull=False)
-#
-#         # Add object-level permission
-#         obj_perm = ObjectPermission(
-#             name="Test permission",
-#             constraints={"pk": instance.pk},
-#             actions=["view"],
-#         )
-#         obj_perm.save()
-#         obj_perm.users.add(self.user)
-#         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-#
-#         # Retrieve without inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(url, **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         # Properties not set on the instance
-#         self.assertEqual("", response.data["import_policy"])
-#         self.assertEqual("", response.data["export_policy"])
-#
-#         # Retrieve with inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(f"{url}?include_inherited", **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         # Properties not set on the instance but inheritable from the parent address-families
-#         self.assertEqual("IMPORT_POLICY", response.data["import_policy"])
-#         self.assertEqual("EXPORT_POLICY", response.data["export_policy"])
-#
-#         # Retrieve with explictly excluded inheritance
-#         url = self._get_detail_url(instance)
-#         response = self.client.get(f"{url}?include_inherited=false", **self.header)
-#         self.assertHttpStatus(response, status.HTTP_200_OK)
-#         self.assertEqual("", response.data["import_policy"])
-#         self.assertEqual("", response.data["export_policy"])
+    def test_id(self):
+        """Test filtering by id."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_afi_safi(self):
+        """Test filtering by AFI-SAFI."""
+        params = {"afi_safi": ["ipv4_unicast", "vpnv4_unicast"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    # TODO filtering by device/virtualmachine
+    def test_device(self):
+        pass
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_forms.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_models.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_views.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/tests/test_views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 """Unit test automation for Model classes in nautobot_bgp_models."""
 
+from unittest import skip, skipIf
+from packaging import version
+
 from django.contrib.contenttypes.models import ContentType
 from nautobot.circuits.models import Provider
 from nautobot.dcim.models import Device, DeviceRole, DeviceType, Interface, Manufacturer, Site
 from nautobot.extras.models import Status
 from nautobot.ipam.models import IPAddress
 from nautobot.utilities.testing import ViewTestCases
 
 from nautobot_bgp_models import models
 from nautobot_bgp_models.choices import AFISAFIChoices
 
+try:
+    from importlib import metadata
+except ImportError:
+    # Running on pre-3.8 Python; use importlib-metadata package
+    import importlib_metadata as metadata
+
+_NAUTOBOT_VERSION = version.parse(metadata.version("nautobot"))
+# Related to this issue: https://github.com/nautobot/nautobot/issues/2948
+_FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS = [version.parse("1.5.4"), version.parse("1.5.5")]
+
 
 class AutonomousSystemTestCase(ViewTestCases.PrimaryObjectViewTestCase):
     """Test views related to the AutonomousSystem model."""
 
     model = models.AutonomousSystem
 
     test_bulk_import_objects_without_permission = None
     test_bulk_import_objects_with_permission = None
     test_bulk_import_objects_with_constrained_permission = None
 
+    @skip("Route disabled in commit `c97f037f`")
+    def test_bulk_import_objects_with_permission_csv_file(self):
+        pass
+
+    @skip("Route disabled in commit `c97f037f`")
+    def test_get_object_notes(self):
+        pass
+
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):
@@ -67,14 +92,26 @@
 
     model = models.PeeringRole
 
     test_bulk_import_objects_without_permission = None
     test_bulk_import_objects_with_permission = None
     test_bulk_import_objects_with_constrained_permission = None
 
+    @skip("Route disabled in commit `c97f037f`")
+    def test_bulk_import_objects_with_permission_csv_file(self):
+        pass
+
+    @skip("Route disabled in commit `c97f037f`")
+    def test_get_object_notes(self):
+        pass
+
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):
@@ -112,14 +149,18 @@
 ):
     """Test views related to the PeerGroup model."""
 
     model = models.PeerGroup
 
     test_create_object_with_constrained_permission = None  # TODO(mzb): FIXME
 
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):
@@ -163,14 +204,18 @@
     ViewTestCases.ListObjectsViewTestCase,
 ):
     """Test views related to the PeerEndpoint model."""
 
     model = models.PeerEndpoint
     maxDiff = None
 
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):  # pylint: disable=too-many-locals
@@ -250,14 +295,18 @@
     ViewTestCases.ListObjectsViewTestCase,
 ):
     """Test views related to the Peering model."""
 
     model = models.Peering
     maxDiff = None
 
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):
@@ -305,14 +354,18 @@
     ViewTestCases.ListObjectsViewTestCase,
 ):
     """Test views related to the AddressFamily model."""
 
     model = models.AddressFamily
     maxDiff = None
 
+    @skipIf(_NAUTOBOT_VERSION in _FAILING_OBJECT_LIST_NAUTOBOT_VERSIONS, f"Skip Nautobot version {_NAUTOBOT_VERSION}")
+    def test_list_objects_with_permission(self):
+        super().test_list_objects_with_permission()
+
     def _get_base_url(self):
         return "plugins:{}:{}_{{}}".format(  # pylint: disable=consider-using-f-string
             self.model._meta.app_label, self.model._meta.model_name
         )
 
     @classmethod
     def setUpTestData(cls):
```

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/urls.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/views.py` & `nautobot_bgp_models-0.7.1/nautobot_bgp_models/views.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b1/pyproject.toml` & `nautobot_bgp_models-0.7.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-bgp-models"
-version = "v0.7.0-beta.1"
+version = "v0.7.1"
 description = "Nautobot BGP Models Plugin"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-bgp-models"
@@ -16,27 +16,38 @@
 ]
 packages = [
     { include = "nautobot_bgp_models" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-nautobot = "^1.3"
+nautobot = "^1.5.4"
 
 [tool.poetry.dev-dependencies]
 invoke = "*"
 black = "*"
 django-debug-toolbar = "*"
 yamllint = "*"
 bandit = "*"
 pylint = "^2"
 pylint-django = "*"
 pydocstyle = "*"
-flake8 = "*"
+# we need to pin flake8 because of package dependencies that cause it to downgrade and
+# therefore cause issues with linting since older versions do not take .flake8 as config
+flake8 = "^3.9.2"
 coverage = "^5.5"
+# Rendering docs to HTML
+mkdocs = "1.3.1"
+# Material for MkDocs theme
+mkdocs-material = "8.4.2"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
+mkdocstrings = "0.19"
+mkdocstrings-python = "0.7.1"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
```

