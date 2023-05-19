# Comparing `tmp/netbox-cisco-maintenance-0.0.5.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.5.tar", last modified: Thu May 18 16:55:04 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.6.tar", last modified: Fri May 19 07:41:36 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.5.tar` & `netbox-cisco-maintenance-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.395743 netbox-cisco-maintenance-0.0.5/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 16:55:04.395743 netbox-cisco-maintenance-0.0.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.387742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      657 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.391742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.391742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19763 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/commands/sync_eox_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.391742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
--rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3180 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.387742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.391742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)     1286 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.395743 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 16:55:04.387742 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 16:55:04.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1331 2023-05-18 16:55:04.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 16:55:04.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 16:55:04.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-18 16:55:04.000000 netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 16:55:04.395743 netbox-cisco-maintenance-0.0.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-18 16:54:44.000000 netbox-cisco-maintenance-0.0.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20186 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/sync_eox_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1535 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      582 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3325 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.517048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1524 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1331 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.5/LICENSE` & `netbox-cisco-maintenance-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/PKG-INFO` & `netbox-cisco-maintenance-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.5/README.md` & `netbox-cisco-maintenance-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/__init__.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/management/commands/sync_eox_data.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/sync_eox_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         parser.add_argument(
             "--manufacturer",
             action="store_true",
             default="Cisco",
             help="Manufacturer name (default: Cisco)",
         )
 
-    # Updates a single device with current EoX Data
-    def update_device_eox_data(self, device):
+    # Updates a single device with current SNI coverage summary data
+    def update_device_sni_summary_data(self, device):
         self.stdout.write(self.style.SUCCESS("Trying to update device %s" % device["sr_no"]))
 
         # Get the device object from NetBox
         try:
             d = Device.objects.get(serial=device["sr_no"])
         except MultipleObjectsReturned:
             # Error if netbox has multiple SN's and skip updating
@@ -56,14 +56,29 @@
 
         # Check if the Coverage in the CiscoSupport object equals API answer. If not, change it
         if ds.is_covered != covered:
             ds.is_covered = covered
             value_changed = True
 
         try:
+            if not device["service_line_descr"]:
+                self.stdout.write(self.style.NOTICE("%s has no service_line_descr" % device["sr_no"]))
+            else:
+                service_line_descr = device["service_line_descr"]
+                self.stdout.write(
+                    self.style.SUCCESS("%s - service_line_descr: %s" % (device["sr_no"], service_line_descr))
+                )
+
+                if ds.service_line_descr != service_line_descr:
+                    ds.service_line_descr = service_line_descr
+                    value_changed = True
+        except KeyError:
+            self.stdout.write(self.style.NOTICE("%s has no service_line_descr" % device["sr_no"]))
+
+        try:
             if not device["warranty_end_date"]:
                 self.stdout.write(self.style.NOTICE("%s has no warranty_end_date" % device["sr_no"]))
             else:
                 warranty_end_date_string = device["warranty_end_date"]
                 warranty_end_date = datetime.strptime(warranty_end_date_string, "%Y-%m-%d").date()
                 self.stdout.write(
                     self.style.SUCCESS("%s - warranty_end_date: %s" % (device["sr_no"], warranty_end_date))
@@ -384,20 +399,14 @@
         for pid in product_ids:
             url = (
                 f"https://apix.cisco.com/supporttools/eox/rest/5/EOXByProductID/1/{pid}?responseencoding=json"
             )
             api_call_response = requests.get(url=url, headers=api_call_headers, verify=False)
             self.stdout.write(self.style.SUCCESS("Call " + url))
 
-            ## debug API answer to text file
-            ## sanatize file name
-            # filename = django.utils.text.get_valid_filename("%s.json" % pid)
-            # with open('/source/netbox_cisco_maintenance/api-answer/%s' % filename, 'w') as outfile:
-            #    outfile.write(api_call_response.text)
-
             # Validate response from Cisco
             if api_call_response.status_code == 200:
                 # Deserialize JSON API Response into Python object "data"
                 data = json.loads(api_call_response.text)
 
                 # Call our Device Type Update method for that particular PID
                 self.update_device_type_eox_data(pid, data)
@@ -432,14 +441,14 @@
             if api_call_response.status_code == 200:
                 # Deserialize JSON API Response into Python object "data"
                 data = json.loads(api_call_response.text)
 
                 # Iterate through all serial numbers included in the API response
                 for device in data["serial_numbers"]:
                     # Call our Device Update method for that particular Device
-                    self.update_device_eox_data(device)
+                    self.update_device_sni_summary_data(device)
 
                 i += 1
 
             else:
                 # Show an error
                 self.stdout.write(self.style.ERROR("API Error: " + api_call_response.text))
```

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0001_initial.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                 ("end_of_sw_maintenance_releases", models.DateField()),
                 ("end_of_security_vul_support_date", models.DateField()),
                 ("end_of_routine_failure_analysis_date", models.DateField()),
                 ("end_of_service_contract_renewal", models.DateField()),
                 ("last_date_of_support", models.DateField()),
                 ("end_of_svc_attach_date", models.DateField()),
                 ("coverage_end_date", models.DateField()),
+                ("service_line_descr", models.DateField()),
                 ("warranty_end_date", models.DateField()),
                 (
                     "device",
                     models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to="dcim.device"),
                 ),
             ],
             options={
```

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/models.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,18 @@
     def __str__(self):
         return "%s Support" % self.device
 
     coverage_end_date = models.DateField(
         help_text="End date of the contract coverage for the specifed serial number", blank=True, null=True
     )
 
+    service_line_descr = models.TextField(
+        help_text="Service description for the specified serial number", blank=True, null=True
+    )
+
     warranty_end_date = models.DateField(
         help_text="End date of the warranty for the specified serial number", blank=True, null=True
     )
 
     is_covered = models.BooleanField(
         help_text="Indicates whether the specified serial number is covered by a service contract",
         default=False,
```

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/template_content.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,18 @@
         <div class="card-body">
             <table class="table table-hover panel-body attr-table">
                 <tbody>
                     <tr >
                         <td style="width: 40%">Is Covered by Contract?</td>
                         <td><i class="mdi {% if cisco_device_support.is_covered %}mdi-check-bold text-success{% else %}mdi-close-thick text-danger{% endif %}"></i></td>
                     </tr>
+                    <tr {{ cisco_device_support.service_line_descr }}>
+                        <td>Service Contract Description</td>
+                        <td>{{ cisco_device_support.service_line_descr }}</td>
+                    </tr>
                     <tr {{ cisco_device_support.coverage_end_date|expiration_class }}>
                         <td>End of Contract Coverage Date</td>
                         <td>{{ cisco_device_support.coverage_end_date }}</td>
                     </tr>
                     <tr {{ cisco_device_support.warranty_end_date|expiration_class }}>
                         <td>End of Warranty Date</td>
                         <td>{{ cisco_device_support.warranty_end_date }}</td>
```

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.5/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.5/setup.py` & `netbox-cisco-maintenance-0.0.6/setup.py`

 * *Files identical despite different names*

