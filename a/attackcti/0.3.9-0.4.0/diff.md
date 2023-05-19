# Comparing `tmp/attackcti-0.3.9.tar.gz` & `tmp/attackcti-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attackcti-0.3.9.tar", last modified: Thu Apr 13 01:25:20 2023, max compression
+gzip compressed data, was "attackcti-0.4.0.tar", last modified: Fri May 19 15:52:37 2023, max compression
```

## Comparing `attackcti-0.3.9.tar` & `attackcti-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.887669 attackcti-0.3.9/
--rw-rw-rw-   0        0        0     1546 2021-05-14 02:44:16.000000 attackcti-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     5265 2023-04-13 01:25:20.887669 attackcti-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2022-01-19 04:33:51.000000 attackcti-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.858364 attackcti-0.3.9/attackcti/
--rw-rw-rw-   0        0        0       62 2021-05-14 02:44:16.000000 attackcti-0.3.9/attackcti/__init__.py
--rw-rw-rw-   0        0        0    92732 2023-04-13 01:23:17.000000 attackcti-0.3.9/attackcti/attack_api.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:25:20.886669 attackcti-0.3.9/attackcti.egg-info/
--rw-rw-rw-   0        0        0     5265 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 01:25:20.000000 attackcti-0.3.9/attackcti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 01:25:20.889672 attackcti-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-04-13 01:24:52.000000 attackcti-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 15:52:37.906401 attackcti-0.4.0/
+-rw-rw-rw-   0        0        0     1546 2023-05-19 15:48:17.000000 attackcti-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4648 2023-05-19 15:52:37.906401 attackcti-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3522 2023-05-19 15:48:17.000000 attackcti-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 15:52:37.874689 attackcti-0.4.0/attackcti/
+-rw-rw-rw-   0        0        0       62 2023-05-19 15:48:17.000000 attackcti-0.4.0/attackcti/__init__.py
+-rw-rw-rw-   0        0        0    95074 2023-05-19 15:50:05.000000 attackcti-0.4.0/attackcti/attack_api.py
+drwxrwxrwx   0        0        0        0 2023-05-19 15:52:37.905392 attackcti-0.4.0/attackcti.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-05-19 15:52:37.000000 attackcti-0.4.0/attackcti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 15:52:37.000000 attackcti-0.4.0/attackcti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 15:52:37.000000 attackcti-0.4.0/attackcti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-19 15:52:37.000000 attackcti-0.4.0/attackcti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 15:52:37.000000 attackcti-0.4.0/attackcti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-19 15:52:37.908409 attackcti-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-05-19 15:50:24.000000 attackcti-0.4.0/setup.py
```

### Comparing `attackcti-0.3.9/LICENSE` & `attackcti-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attackcti-0.3.9/PKG-INFO` & `attackcti-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,102 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.3.9
+Version: 0.4.0
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
-Description: # ATT&CK Python Client
-        
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
-        [![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
-        [![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
-        [![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
-        
-        A Python module to access up-to-date ATT&CK content available in [STIX](https://oasis-open.github.io/cti-documentation/stix/intro) via a public [TAXII](https://oasis-open.github.io/cti-documentation/taxii/intro) server. This project leverages python classes and functions from the [cti-python-stix2](https://github.com/oasis-open/cti-python-stix2) and [cti-taxii-client](https://github.com/oasis-open/cti-taxii-client) libraries developed by MITRE.
-        
-        ## Goals
-        
-        * Provide an easy way to access and interact with up-to-date ATT&CK content available in STIX via public TAXII server.
-        * Allow security analysts to quickly explore ATT&CK content and apply it in their daily operations.
-        * Allow the integration of ATT&CK content with other platforms to host up to date information from the framework.
-        * Help security analysts during the transition from the old ATT&CK MediaWiki API to the STIX/TAXII 2.0 API.
-        * Learn STIX2 and TAXII Client Python libraries
-        
-        ## Documentation
-        
-        ### [https://attackcti.com](https://attackcti.com)
-        
-        ## Current Status: Production/Stable
-        
-        The project is currently in a Production/Stable stage, which means that the current main functions are more stable. I would love to get your feedback to make it a better project.
-        
-        ## Resources
-        
-        * [MITRE CTI](https://github.com/mitre/cti)
-        * [OASIS CTI TAXII Client](https://github.com/oasis-open/cti-taxii-client)
-        * [OASIS CTI Python STIX2](https://github.com/oasis-open/cti-python-stix2)
-        * [MITRE ATT&CK Framework](https://attack.mitre.org/wiki/Main_Page)
-        * [ATT&CK MediaWiki API](https://attack.mitre.org/wiki/Using_the_API)
-        * [Invoke-ATTACKAPI](https://github.com/Cyb3rWard0g/Invoke-ATTACKAPI)
-        * [Mitre-Attack-API](https://github.com/annamcabee/Mitre-Attack-API)
-        
-        ### Requirements
-        
-        - Python >= 3.0
-        - stix2 >= 2.1.0
-        - taxii2-client >= 2.3.0
-        - six >= 1.16.0
-        
-        ### Installation
-        
-        You can install it via pip:
-        
-        ```
-        pip install attackcti
-        ```
-        
-        Or you can also do the following:
-        
-        ```
-        git clone https://github.com/OTRF/ATTACK-Python-Client
-        cd ATTACK-Python-Client
-        pip install .
-        ```
-        
-        ## Contribution
-        
-        * Now that the project is more stable, It would be great to get your feedback and hopefully get more contributions to the project. Let us know if you have any features in mind. We would love to collaborate to make them happen in the project.
-        * Check our basic contribution guidelines and submit an issue with your ideas.
-        * Be concise but clear when adding a title and description to your feature proposal.
-        * One pull request per issue.
-        * Select one or more labels when you submit an issue.
-        * Make sure you are in the correct branch [Master].
-        * Try to avoid sizeable changes unless warranted.
-        * Be patient and polite as the project is still relatively small, which is why we would appreciate your help where possible.
-        
-        ## Author
-        
-        * Roberto Rodriguez [@Cyb3rWard0g](https://twitter.com/Cyb3rWard0g)
-        
-        ## Official Committers
-        
-        * Jose Luis Rodriguez [@Cyb3rPandaH](https://twitter.com/Cyb3rPandaH)
-        
 Keywords: threat hunting dfir cti cyber threat intelligence mitre att&ck
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ATT&CK Python Client
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
+[![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
+[![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
+[![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
+
+A Python module to access up-to-date ATT&CK content available in [STIX](https://oasis-open.github.io/cti-documentation/stix/intro) via a public [TAXII](https://oasis-open.github.io/cti-documentation/taxii/intro) server. This project leverages python classes and functions from the [cti-python-stix2](https://github.com/oasis-open/cti-python-stix2) and [cti-taxii-client](https://github.com/oasis-open/cti-taxii-client) libraries developed by MITRE.
+
+## Goals
+
+* Provide an easy way to access and interact with up-to-date ATT&CK content available in STIX via public TAXII server.
+* Allow security analysts to quickly explore ATT&CK content and apply it in their daily operations.
+* Allow the integration of ATT&CK content with other platforms to host up to date information from the framework.
+* Help security analysts during the transition from the old ATT&CK MediaWiki API to the STIX/TAXII 2.0 API.
+* Learn STIX2 and TAXII Client Python libraries
+
+## Documentation
+
+### [https://attackcti.com](https://attackcti.com)
+
+## Current Status: Production/Stable
+
+The project is currently in a Production/Stable stage, which means that the current main functions are more stable. I would love to get your feedback to make it a better project.
+
+## Resources
+
+* [MITRE CTI](https://github.com/mitre/cti)
+* [OASIS CTI TAXII Client](https://github.com/oasis-open/cti-taxii-client)
+* [OASIS CTI Python STIX2](https://github.com/oasis-open/cti-python-stix2)
+* [MITRE ATT&CK Framework](https://attack.mitre.org/wiki/Main_Page)
+* [ATT&CK MediaWiki API](https://attack.mitre.org/wiki/Using_the_API)
+* [Invoke-ATTACKAPI](https://github.com/Cyb3rWard0g/Invoke-ATTACKAPI)
+* [Mitre-Attack-API](https://github.com/annamcabee/Mitre-Attack-API)
+
+### Requirements
+
+- Python >= 3.0
+- stix2 >= 2.1.0
+- taxii2-client >= 2.3.0
+- six >= 1.16.0
+
+### Installation
+
+You can install it via pip:
+
+```
+pip install attackcti
+```
+
+Or you can also do the following:
+
+```
+git clone https://github.com/OTRF/ATTACK-Python-Client
+cd ATTACK-Python-Client
+pip install .
+```
+
+## Contribution
+
+* Now that the project is more stable, It would be great to get your feedback and hopefully get more contributions to the project. Let us know if you have any features in mind. We would love to collaborate to make them happen in the project.
+* Check our basic contribution guidelines and submit an issue with your ideas.
+* Be concise but clear when adding a title and description to your feature proposal.
+* One pull request per issue.
+* Select one or more labels when you submit an issue.
+* Make sure you are in the correct branch [Master].
+* Try to avoid sizeable changes unless warranted.
+* Be patient and polite as the project is still relatively small, which is why we would appreciate your help where possible.
+
+## Author
+
+* Roberto Rodriguez [@Cyb3rWard0g](https://twitter.com/Cyb3rWard0g)
+
+## Official Committers
+
+* Jose Luis Rodriguez [@Cyb3rPandaH](https://twitter.com/Cyb3rPandaH)
```

### Comparing `attackcti-0.3.9/README.md` & `attackcti-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `attackcti-0.3.9/attackcti/attack_api.py` & `attackcti-0.4.0/attackcti/attack_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
         if skip_revoked_deprecated:
             enterprise_campaigns = self.remove_revoked_deprecated(enterprise_campaigns)
         
         if not stix_format:
             enterprise_campaigns = self.translate_stix_objects(enterprise_campaigns)
         return enterprise_campaigns
 
-    def get_enterprise_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, enrich_data_sources = False, stix_format=True):
+    def get_enterprise_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, enrich_data_sources=False, stix_format=True):
         """ Extracts all the available techniques STIX objects in the Enterprise ATT&CK matrix
 
         Args:
             skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects. 
             include_subtechniques (bool): default True. Include techniques and sub-techniques STIX objects.
             enrich_data_sources (bool): default False. Adds data component and data source context to each technqiue.
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
@@ -665,18 +665,20 @@
         Returns:
             List of STIX objects
         
         """
 
         mobile_filter_objects = {
             "techniques": self.get_mobile_techniques,
+            "data-component": self.get_mobile_data_components,
             "mitigations": self.get_mobile_mitigations,
             "groups": self.get_mobile_groups,
             "malware": self.get_mobile_malware,
             "tools": self.get_mobile_tools,
+            "data-source": self.get_mobile_data_sources,
             "relationships": self.get_mobile_relationships,
             "tactics": self.get_mobile_tactics,
             "matrix": Filter("type", "=", "x-mitre-matrix"),
             "identity": Filter("type", "=", "identity"),
             "marking-definition": Filter("type", "=", "marking-definition"),
             "campaigns": self.get_mobile_campaigns
         }
@@ -703,20 +705,21 @@
         if skip_revoked_deprecated:
             mobile_campaigns = self.remove_revoked_deprecated(mobile_campaigns)
 
         if not stix_format:
             mobile_campaigns = self.translate_stix_objects(mobile_campaigns)
         return mobile_campaigns
 
-    def get_mobile_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, stix_format=True):
+    def get_mobile_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, enrich_data_sources=False, stix_format=True):
         """  Extracts all the available techniques STIX objects in the Mobile ATT&CK matrix
 
         Args:
             skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects. 
             include_subtechniques (bool): default True. Include techniques and sub-techniques STIX objects.
+            enrich_data_sources (bool): default False. Adds data component and data source context to each technqiue.
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         
         Returns:
             List of STIX objects
         """
 
         if include_subtechniques:
@@ -725,19 +728,36 @@
             mobile_techniques = self.TC_MOBILE_SOURCE.query([
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
             ])
 
         if skip_revoked_deprecated:
             mobile_techniques = self.remove_revoked_deprecated(mobile_techniques)
+        
+        if enrich_data_sources:
+            mobile_techniques = self.enrich_techniques_data_sources(mobile_techniques)
 
         if not stix_format:
             mobile_techniques = self.translate_stix_objects(mobile_techniques)
         return mobile_techniques
     
+    def get_mobile_data_components(self, stix_format=True):
+        """ Extracts all the available data components STIX objects in the Mobile ATT&CK matrix
+
+        Args:
+            stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
+        
+        Returns:
+            List of STIX objects
+        """
+        mobile_data_components = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-data-component"))
+        if not stix_format:
+            mobile_data_components = self.translate_stix_objects(mobile_data_components)
+        return mobile_data_components
+    
     def get_mobile_mitigations(self, stix_format=True):
         """ Extracts all the available mitigations STIX objects in the Mobile ATT&CK matrix
 
         Args:
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         
         Returns:
@@ -824,14 +844,31 @@
             List of STIX objects
         
         """
         mobile_tactics = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-tactic"))
         if not stix_format:
             mobile_tactics = self.translate_stix_objects(mobile_tactics)
         return mobile_tactics
+
+    def get_mobile_data_sources(self, include_data_components=False, stix_format=True):
+        """ Extracts all the available data source STIX objects availalbe in the Mobile ATT&CK matrix. This function filters all STIX objects by the type x-mitre-data-source.
+
+        Args:
+            stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
+        
+        Returns:
+            List of STIX objects
+        """
+        mobile_data_sources = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-data-source"))
+        if include_data_components:
+            for ds in mobile_data_sources:
+                ds['data_components']= self.get_data_components_by_data_source(ds)
+        if not stix_format:
+            mobile_data_sources = self.translate_stix_objects(mobile_data_sources)
+        return mobile_data_sources
     
     # ******** ICS ATT&CK Technology Domain *******
     def get_ics(self, stix_format=True):
         """ Extracts all the available STIX objects in the ICS ATT&CK matrix
 
         Args:
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
@@ -878,20 +915,21 @@
         if skip_revoked_deprecated:
             ics_campaigns = self.remove_revoked_deprecated(ics_campaigns)
 
         if not stix_format:
             ics_campaigns = self.translate_stix_objects(ics_campaigns)
         return ics_campaigns
 
-    def get_ics_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, stix_format=True):
+    def get_ics_techniques(self, skip_revoked_deprecated=True, include_subtechniques=True, enrich_data_sources=False, stix_format=True):
         """ Extracts all the available techniques STIX objects in the ICS ATT&CK matrix
 
         Args:
             skip_revoked_deprecated (bool): default True. Skip revoked and deprecated STIX objects. 
             include_subtechniques (bool): default True. Include techniques and sub-techniques STIX objects.
+            enrich_data_sources (bool): default False. Adds data component and data source context to each technqiue.
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         
         Returns:
             List of STIX objects
         
         """
 
@@ -902,14 +940,17 @@
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
             ])
 
         if skip_revoked_deprecated:
             ics_techniques = self.remove_revoked_deprecated(ics_techniques)
         
+        if enrich_data_sources:
+            ics_techniques = self.enrich_techniques_data_sources(ics_techniques)
+        
         if not stix_format:
             ics_techniques = self.translate_stix_objects(ics_techniques)
         return ics_techniques
 
     def get_ics_data_components(self, stix_format=True):
         """ Extracts all the available data components STIX objects in the ICS ATT&CK matrix
 
@@ -1154,18 +1195,18 @@
         """ Extracts all the available data components STIX objects across all ATT&CK matrices
         Args:
             skip_revoked_deprecated (bool): removes revoked or deprecated STIX objects from relationships and techniques. Default: Set to True.
             stix_format (bool):  Returns results in original STIX format or friendly syntax (e.g. 'attack-pattern' or 'technique')
         """
         enterprise_data_components = self.get_enterprise_data_components()
         ics_data_components = self.get_ics_data_components()
-        '''mobile_data_components = self.get_mobile_data_components()
+        mobile_data_components = self.get_mobile_data_components()
         for mdc in mobile_data_components:
             if mdc not in enterprise_data_components:
-                enterprise_data_components.append(mdc)'''
+                enterprise_data_components.append(mdc)
         for idc in ics_data_components:
             if idc not in enterprise_data_components:
                 enterprise_data_components.append(idc)
         
         if skip_revoked_deprecated:
             enterprise_data_components = self.remove_revoked_deprecated(enterprise_data_components)
         
@@ -1262,17 +1303,21 @@
         
         Returns:
             List of STIX objects
         
         """
         enterprise_data_sources = self.get_enterprise_data_sources(include_data_components)
         ics_data_sources = self.get_ics_data_sources(include_data_components)
-        for ds in ics_data_sources:
-            if ds not in enterprise_data_sources:
-                enterprise_data_sources.append(ds)
+        mobile_data_sources = self.get_mobile_data_sources(include_data_components)
+        for mds in mobile_data_sources:
+            if mds not in enterprise_data_sources:
+                enterprise_data_sources.append(mds)
+        for ids in ics_data_sources:
+            if ids not in enterprise_data_sources:
+                enterprise_data_sources.append(ids)
         '''
         if include_data_components:
             data_sources = self.get_enterprise_data_sources(include_data_components=True)
         else:
             data_sources = self.get_enterprise_data_sources()'''
 
         if not stix_format:
@@ -1965,22 +2010,21 @@
 
         # Create Data Sources and Data Components lookup tables
         ds_lookup = {ds['id']:ds for ds in data_sources}
         dc_lookup = {dc['id']:dc for dc in data_components}
 
         # https://stix2.readthedocs.io/en/latest/guide/versioning.html
         for i in range(len(stix_object)):
-            if 'x_mitre_data_sources' in stix_object[i].keys():
-                technique_ds = dict()
-                for rl in relationships:
-                    if stix_object[i]['id'] == rl['target_ref']:
-                        dc = dc_lookup[rl['source_ref']]
-                        dc_ds_ref = dc['x_mitre_data_source_ref']
-                        if dc_ds_ref not in technique_ds.keys():
-                            technique_ds[dc_ds_ref] = ds_lookup[dc_ds_ref].copy()
-                            technique_ds[dc_ds_ref]['data_components'] = list()
-                        if dc not in technique_ds[dc_ds_ref]['data_components']:
-                            technique_ds[dc_ds_ref]['data_components'].append(dc)
-                if technique_ds:
-                    new_data_sources = [ v for v in technique_ds.values()]
-                    stix_object[i] = stix_object[i].new_version(x_mitre_data_sources = new_data_sources)
+            technique_ds = dict()
+            for rl in relationships:
+                if stix_object[i]['id'] == rl['target_ref']:
+                    dc = dc_lookup[rl['source_ref']]
+                    dc_ds_ref = dc['x_mitre_data_source_ref']
+                    if dc_ds_ref not in technique_ds.keys():
+                        technique_ds[dc_ds_ref] = ds_lookup[dc_ds_ref].copy()
+                        technique_ds[dc_ds_ref]['data_components'] = list()
+                    if dc not in technique_ds[dc_ds_ref]['data_components']:
+                        technique_ds[dc_ds_ref]['data_components'].append(dc)
+            if technique_ds:
+                new_data_sources = [ v for v in technique_ds.values()]
+                stix_object[i] = stix_object[i].new_version(x_mitre_data_sources = new_data_sources)
         return stix_object
```

### Comparing `attackcti-0.3.9/attackcti.egg-info/PKG-INFO` & `attackcti-0.4.0/attackcti.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,102 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.3.9
+Version: 0.4.0
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
-Description: # ATT&CK Python Client
-        
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
-        [![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
-        [![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
-        [![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
-        
-        A Python module to access up-to-date ATT&CK content available in [STIX](https://oasis-open.github.io/cti-documentation/stix/intro) via a public [TAXII](https://oasis-open.github.io/cti-documentation/taxii/intro) server. This project leverages python classes and functions from the [cti-python-stix2](https://github.com/oasis-open/cti-python-stix2) and [cti-taxii-client](https://github.com/oasis-open/cti-taxii-client) libraries developed by MITRE.
-        
-        ## Goals
-        
-        * Provide an easy way to access and interact with up-to-date ATT&CK content available in STIX via public TAXII server.
-        * Allow security analysts to quickly explore ATT&CK content and apply it in their daily operations.
-        * Allow the integration of ATT&CK content with other platforms to host up to date information from the framework.
-        * Help security analysts during the transition from the old ATT&CK MediaWiki API to the STIX/TAXII 2.0 API.
-        * Learn STIX2 and TAXII Client Python libraries
-        
-        ## Documentation
-        
-        ### [https://attackcti.com](https://attackcti.com)
-        
-        ## Current Status: Production/Stable
-        
-        The project is currently in a Production/Stable stage, which means that the current main functions are more stable. I would love to get your feedback to make it a better project.
-        
-        ## Resources
-        
-        * [MITRE CTI](https://github.com/mitre/cti)
-        * [OASIS CTI TAXII Client](https://github.com/oasis-open/cti-taxii-client)
-        * [OASIS CTI Python STIX2](https://github.com/oasis-open/cti-python-stix2)
-        * [MITRE ATT&CK Framework](https://attack.mitre.org/wiki/Main_Page)
-        * [ATT&CK MediaWiki API](https://attack.mitre.org/wiki/Using_the_API)
-        * [Invoke-ATTACKAPI](https://github.com/Cyb3rWard0g/Invoke-ATTACKAPI)
-        * [Mitre-Attack-API](https://github.com/annamcabee/Mitre-Attack-API)
-        
-        ### Requirements
-        
-        - Python >= 3.0
-        - stix2 >= 2.1.0
-        - taxii2-client >= 2.3.0
-        - six >= 1.16.0
-        
-        ### Installation
-        
-        You can install it via pip:
-        
-        ```
-        pip install attackcti
-        ```
-        
-        Or you can also do the following:
-        
-        ```
-        git clone https://github.com/OTRF/ATTACK-Python-Client
-        cd ATTACK-Python-Client
-        pip install .
-        ```
-        
-        ## Contribution
-        
-        * Now that the project is more stable, It would be great to get your feedback and hopefully get more contributions to the project. Let us know if you have any features in mind. We would love to collaborate to make them happen in the project.
-        * Check our basic contribution guidelines and submit an issue with your ideas.
-        * Be concise but clear when adding a title and description to your feature proposal.
-        * One pull request per issue.
-        * Select one or more labels when you submit an issue.
-        * Make sure you are in the correct branch [Master].
-        * Try to avoid sizeable changes unless warranted.
-        * Be patient and polite as the project is still relatively small, which is why we would appreciate your help where possible.
-        
-        ## Author
-        
-        * Roberto Rodriguez [@Cyb3rWard0g](https://twitter.com/Cyb3rWard0g)
-        
-        ## Official Committers
-        
-        * Jose Luis Rodriguez [@Cyb3rPandaH](https://twitter.com/Cyb3rPandaH)
-        
 Keywords: threat hunting dfir cti cyber threat intelligence mitre att&ck
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ATT&CK Python Client
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
+[![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
+[![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
+[![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
+
+A Python module to access up-to-date ATT&CK content available in [STIX](https://oasis-open.github.io/cti-documentation/stix/intro) via a public [TAXII](https://oasis-open.github.io/cti-documentation/taxii/intro) server. This project leverages python classes and functions from the [cti-python-stix2](https://github.com/oasis-open/cti-python-stix2) and [cti-taxii-client](https://github.com/oasis-open/cti-taxii-client) libraries developed by MITRE.
+
+## Goals
+
+* Provide an easy way to access and interact with up-to-date ATT&CK content available in STIX via public TAXII server.
+* Allow security analysts to quickly explore ATT&CK content and apply it in their daily operations.
+* Allow the integration of ATT&CK content with other platforms to host up to date information from the framework.
+* Help security analysts during the transition from the old ATT&CK MediaWiki API to the STIX/TAXII 2.0 API.
+* Learn STIX2 and TAXII Client Python libraries
+
+## Documentation
+
+### [https://attackcti.com](https://attackcti.com)
+
+## Current Status: Production/Stable
+
+The project is currently in a Production/Stable stage, which means that the current main functions are more stable. I would love to get your feedback to make it a better project.
+
+## Resources
+
+* [MITRE CTI](https://github.com/mitre/cti)
+* [OASIS CTI TAXII Client](https://github.com/oasis-open/cti-taxii-client)
+* [OASIS CTI Python STIX2](https://github.com/oasis-open/cti-python-stix2)
+* [MITRE ATT&CK Framework](https://attack.mitre.org/wiki/Main_Page)
+* [ATT&CK MediaWiki API](https://attack.mitre.org/wiki/Using_the_API)
+* [Invoke-ATTACKAPI](https://github.com/Cyb3rWard0g/Invoke-ATTACKAPI)
+* [Mitre-Attack-API](https://github.com/annamcabee/Mitre-Attack-API)
+
+### Requirements
+
+- Python >= 3.0
+- stix2 >= 2.1.0
+- taxii2-client >= 2.3.0
+- six >= 1.16.0
+
+### Installation
+
+You can install it via pip:
+
+```
+pip install attackcti
+```
+
+Or you can also do the following:
+
+```
+git clone https://github.com/OTRF/ATTACK-Python-Client
+cd ATTACK-Python-Client
+pip install .
+```
+
+## Contribution
+
+* Now that the project is more stable, It would be great to get your feedback and hopefully get more contributions to the project. Let us know if you have any features in mind. We would love to collaborate to make them happen in the project.
+* Check our basic contribution guidelines and submit an issue with your ideas.
+* Be concise but clear when adding a title and description to your feature proposal.
+* One pull request per issue.
+* Select one or more labels when you submit an issue.
+* Make sure you are in the correct branch [Master].
+* Try to avoid sizeable changes unless warranted.
+* Be patient and polite as the project is still relatively small, which is why we would appreciate your help where possible.
+
+## Author
+
+* Roberto Rodriguez [@Cyb3rWard0g](https://twitter.com/Cyb3rWard0g)
+
+## Official Committers
+
+* Jose Luis Rodriguez [@Cyb3rPandaH](https://twitter.com/Cyb3rPandaH)
```

### Comparing `attackcti-0.3.9/setup.py` & `attackcti-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md')as f:
     long_description = f.read()
 
 setup(
     name="attackcti",
-    version="0.3.9",
+    version="0.4.0",
     author="Roberto Rodriguez",
     description="MITRE ATTACK CTI Python Libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OTRF/ATTACK-Python-Client",
     project_urls={
         "Documentation": "https://attackcti.com",
```

