# Comparing `tmp/phonebox_plugin-0.0.5b1.tar.gz` & `tmp/phonebox_plugin-0.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonebox_plugin-0.0.5b1.tar", last modified: Tue Apr 18 18:52:08 2023, max compression
+gzip compressed data, was "phonebox_plugin-0.0.6b1.tar", last modified: Fri May 19 14:11:05 2023, max compression
```

## Comparing `phonebox_plugin-0.0.5b1.tar` & `phonebox_plugin-0.0.6b1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.091702 phonebox_plugin-0.0.5b1/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1066 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/LICENSE
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      123 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/MANIFEST.in
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-04-18 18:52:08.091521 phonebox_plugin-0.0.5b1/PKG-INFO
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4870 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/README.md
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.085919 phonebox_plugin-0.0.5b1/phonebox_plugin/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      493 2023-04-18 18:35:42.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/__init__.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      205 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/admin.py
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.087617 phonebox_plugin-0.0.5b1/phonebox_plugin/api/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       35 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/__init__.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      707 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/nested_serializers.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1148 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/serializers.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      256 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/urls.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      780 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/views.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      556 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/choices.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3293 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/filters.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)    10187 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/forms.py
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.088544 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1982 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0001_initial.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      376 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0002_alter_number_id.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2337 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0003_voicecircuit.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/__init__.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4882 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/models.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      331 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/navigation.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1402 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/tables.py
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.082665 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.091305 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4360 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5176 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      734 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1913 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1910 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4327 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4466 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3263 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      254 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/tags_panel.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6570 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6980 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      775 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2038 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2035 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1595 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/urls.py
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4507 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/views.py
-drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.086585 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/PKG-INFO
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1811 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        1 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       16 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/top_level.txt
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       38 2023-04-18 18:52:08.091748 phonebox_plugin-0.0.5b1/setup.cfg
--rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1107 2023-04-18 18:35:25.000000 phonebox_plugin-0.0.5b1/setup.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.891046 phonebox_plugin-0.0.6b1/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1066 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/LICENSE
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      123 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/MANIFEST.in
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-05-19 14:11:05.890874 phonebox_plugin-0.0.6b1/PKG-INFO
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4870 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/README.md
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.885624 phonebox_plugin-0.0.6b1/phonebox_plugin/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      493 2023-05-18 14:23:47.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      205 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/admin.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.887228 phonebox_plugin-0.0.6b1/phonebox_plugin/api/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       35 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/api/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      707 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/api/nested_serializers.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1148 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/api/serializers.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      256 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/api/urls.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      780 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/api/views.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      556 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/choices.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3293 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/filters.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)    10688 2023-05-18 14:23:47.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/forms.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.887953 phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1982 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/0001_initial.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      376 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/0002_alter_number_id.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2337 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/0003_voicecircuit.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4882 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/models.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      331 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/navigation.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1402 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/tables.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.882683 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.890645 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_number.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4360 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5176 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      734 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1913 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1910 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4327 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/number.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4466 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3263 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      254 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/tags_panel.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6570 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6980 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      775 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2038 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2035 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1595 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/urls.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4507 2023-05-17 12:52:34.000000 phonebox_plugin-0.0.6b1/phonebox_plugin/views.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-05-19 14:11:05.886230 phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-05-19 14:11:05.000000 phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1811 2023-05-19 14:11:05.000000 phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        1 2023-05-19 14:11:05.000000 phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       16 2023-05-19 14:11:05.000000 phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/top_level.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       38 2023-05-19 14:11:05.891088 phonebox_plugin-0.0.6b1/setup.cfg
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1107 2023-05-18 14:23:47.000000 phonebox_plugin-0.0.6b1/setup.py
```

### Comparing `phonebox_plugin-0.0.5b1/LICENSE` & `phonebox_plugin-0.0.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/PKG-INFO` & `phonebox_plugin-0.0.6b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phonebox_plugin
-Version: 0.0.5b1
+Version: 0.0.6b1
 Summary: A phone numbers management plugin for NetBox.
 Home-page: https://github.com/iDebugAll/phonebox-plugin.git
-Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz
+Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.6-beta.1.tar.gz
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
 Keywords: netbox,netbox-plugin,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `phonebox_plugin-0.0.5b1/README.md` & `phonebox_plugin-0.0.6b1/README.md`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/api/nested_serializers.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/api/serializers.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/api/views.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/choices.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/choices.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/filters.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/filters.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/forms.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from django import forms
-from utilities.forms import (
-    BootstrapMixin, DynamicModelMultipleChoiceField, DynamicModelChoiceField,
-    TagFilterField, BulkEditForm, CSVModelForm, CSVModelChoiceField
-)
+from django.conf import settings
+from packaging import version
 from tenancy.models import Tenant
 from dcim.models import Region, Site, Device, Interface
 from virtualization.models import VirtualMachine, VMInterface
 from circuits.models import Provider
 from extras.models import Tag
 from .models import Number, VoiceCircuit
 from .choices import VoiceCircuitTypeChoices
 
+NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
+if NETBOX_CURRENT_VERSION < version.parse("3.5"):
+    from utilities.forms import (
+        BootstrapMixin, DynamicModelMultipleChoiceField, DynamicModelChoiceField,
+        TagFilterField, BulkEditForm, CSVModelForm, CSVModelChoiceField
+    )
+else:
+    from utilities.forms import BootstrapMixin, BulkEditForm, CSVModelForm
+    from utilities.forms.fields import (
+        DynamicModelMultipleChoiceField, DynamicModelChoiceField,
+        TagFilterField, CSVModelChoiceField
+    )
 
 class AddRemoveTagsForm(forms.Form):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Add add/remove tags fields
@@ -49,15 +59,18 @@
     )
     provider = DynamicModelMultipleChoiceField(
         queryset=Provider.objects.all(),
         to_field_name='id',
         required=False,
         null_option='None',
     )
-    tag = TagFilterField(model)
+    tags = DynamicModelMultipleChoiceField(
+        queryset=Tag.objects.all(),
+        required=False
+    )
 
 
 class NumberEditForm(forms.ModelForm):
 
     number = forms.CharField(
         required=True,
         widget=forms.TextInput(
```

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0001_initial.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0003_voicecircuit.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/migrations/0003_voicecircuit.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/models.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/models.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/tables.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_number.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/number.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html` & `phonebox_plugin-0.0.6b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/urls.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin/views.py` & `phonebox_plugin-0.0.6b1/phonebox_plugin/views.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/PKG-INFO` & `phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phonebox-plugin
-Version: 0.0.5b1
+Version: 0.0.6b1
 Summary: A phone numbers management plugin for NetBox.
 Home-page: https://github.com/iDebugAll/phonebox-plugin.git
-Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz
+Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.6-beta.1.tar.gz
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
 Keywords: netbox,netbox-plugin,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/SOURCES.txt` & `phonebox_plugin-0.0.6b1/phonebox_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.5b1/setup.py` & `phonebox_plugin-0.0.6b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from os import path
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='phonebox_plugin',
-    version='v0.0.5-beta.1',
+    version='v0.0.6-beta.1',
     url='https://github.com/iDebugAll/phonebox-plugin.git',
-    download_url='https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz',
+    download_url='https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.6-beta.1.tar.gz',
     description='A phone numbers management plugin for NetBox.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Igor Korotchenkov',
     author_email='iDebugAll@gmail.com',
     install_requires=[],
     packages=find_packages(),
```

