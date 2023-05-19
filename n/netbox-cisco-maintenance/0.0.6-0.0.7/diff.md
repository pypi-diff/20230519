# Comparing `tmp/netbox-cisco-maintenance-0.0.6.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.6.tar", last modified: Fri May 19 07:41:36 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.7.tar", last modified: Fri May 19 08:09:20 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.6.tar` & `netbox-cisco-maintenance-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20186 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/sync_eox_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1535 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
--rw-r--r--   0 vsts      (1001) docker     (123)      582 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3325 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.517048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)     1524 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1331 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-19 07:41:36.000000 netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-19 07:41:36.521048 netbox-cisco-maintenance-0.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-19 07:41:19.000000 netbox-cisco-maintenance-0.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.929705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20186 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/commands/sync_eox_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3325 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.929705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1524 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-19 08:09:20.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1331 2023-05-19 08:09:20.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 08:09:20.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 08:09:20.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-19 08:09:20.000000 netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-19 08:09:20.933705 netbox-cisco-maintenance-0.0.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-19 08:08:53.000000 netbox-cisco-maintenance-0.0.7/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.6/LICENSE` & `netbox-cisco-maintenance-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/PKG-INFO` & `netbox-cisco-maintenance-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.6
+Version: 0.0.7
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.6/README.md` & `netbox-cisco-maintenance-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/__init__.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/admin.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/management/commands/sync_eox_data.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/management/commands/sync_eox_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0001_initial.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                 ("end_of_sw_maintenance_releases", models.DateField()),
                 ("end_of_security_vul_support_date", models.DateField()),
                 ("end_of_routine_failure_analysis_date", models.DateField()),
                 ("end_of_service_contract_renewal", models.DateField()),
                 ("last_date_of_support", models.DateField()),
                 ("end_of_svc_attach_date", models.DateField()),
                 ("coverage_end_date", models.DateField()),
-                ("service_line_descr", models.DateField()),
                 ("warranty_end_date", models.DateField()),
                 (
                     "device",
                     models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to="dcim.device"),
                 ),
             ],
             options={
```

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/models.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/template_content.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templates/netbox_cisco_maintenance/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.6
+Version: 0.0.7
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.6/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.7/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.6/setup.py` & `netbox-cisco-maintenance-0.0.7/setup.py`

 * *Files identical despite different names*

