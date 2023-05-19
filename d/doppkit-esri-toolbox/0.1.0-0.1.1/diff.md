# Comparing `tmp/doppkit-esri-toolbox-0.1.0.tar.gz` & `tmp/doppkit-esri-toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-esri-toolbox-0.1.0.tar", last modified: Mon May 15 17:56:09 2023, max compression
+gzip compressed data, was "doppkit-esri-toolbox-0.1.1.tar", last modified: Fri May 19 16:37:26 2023, max compression
```

## Comparing `doppkit-esri-toolbox-0.1.0.tar` & `doppkit-esri-toolbox-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.859118 doppkit-esri-toolbox-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-05-12 21:31:58.000000 doppkit-esri-toolbox-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    13909 2023-05-15 17:56:09.858120 doppkit-esri-toolbox-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-05-12 21:31:58.000000 doppkit-esri-toolbox-0.1.0/README.md
--rw-rw-rw-   0        0        0      973 2023-05-12 21:04:56.000000 doppkit-esri-toolbox-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 17:56:09.859118 doppkit-esri-toolbox-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.802101 doppkit-esri-toolbox-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.823945 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/
--rw-rw-rw-   0        0        0    13909 2023-05-15 17:56:09.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-05-15 17:56:09.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:56:09.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-12 21:05:08.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-15 17:56:09.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 17:56:09.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.824945 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/
--rw-rw-rw-   0        0        0       21 2023-05-15 17:39:12.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.803403 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.829945 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/arcpy/
--rw-rw-rw-   0        0        0     1951 2023-05-12 21:06:28.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.802101 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.849604 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/
--rw-rw-rw-   0        0        0     1208 2023-05-12 18:55:24.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/Fetch_Export_toolbox.xml
--rw-rw-rw-   0        0        0     1225 2023-05-12 18:55:24.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/Subprocess_Sync_toolbox.xml
--rw-rw-rw-   0        0        0      653 2023-05-12 18:55:24.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/toolbox_toolbox.xml
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.855120 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/toolboxes/
--rw-rw-rw-   0        0        0     3174 2023-05-12 21:06:28.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/help/gp/toolboxes/doppkit_wrapper_toolbox.xml
-drwxrwxrwx   0        0        0        0 2023-05-15 17:56:09.856119 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/toolboxes/
--rw-rw-rw-   0        0        0     9045 2023-05-15 17:46:32.000000 doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/toolboxes/doppkit_wrapper_toolbox.pyt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.734407 doppkit-esri-toolbox-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 16:37:26.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.734407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:37:26.738407 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 16:37:12.000000 doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py
```

### Comparing `doppkit-esri-toolbox-0.1.0/LICENSE` & `doppkit-esri-toolbox-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `doppkit-esri-toolbox-0.1.0/PKG-INFO` & `doppkit-esri-toolbox-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,220 +1,282 @@
-Metadata-Version: 2.1
-Name: doppkit-esri-toolbox
-Version: 0.1.0
-Summary: Tool to allow retrival of USACE GRiD data
-Maintainer-email: Ognyan Moore <ogi@hobu.co>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: homepage, https://github.com/hobuinc/doppkit-esri-toolbox
-Project-URL: repository, https://github.com/hobuinc/doppkit-esri-toolbox
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-# doppkit-esri-toolbox
-ArcGIS Pro Toolbox to Interact with GRID
+Metadata-Version: 2.1
+Name: doppkit-esri-toolbox
+Version: 0.1.1
+Summary: Tool to allow retrival of USACE GRiD data
+Maintainer-email: Ognyan Moore <ogi@hobu.co>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: homepage, https://github.com/hobuinc/doppkit-esri-toolbox
+Project-URL: repository, https://github.com/hobuinc/doppkit-esri-toolbox
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# doppkit-esri-toolbox
+
+ArcGIS Pro Toolbox to Interact with GRiD.  The toolbox provides ArcGIS users to interact with the doppkit utility to
+retrieve exports from GRiD.
+
+## Installation
+
+Installation of the doppkit toolkit into ArcGIS pro can be done via the following steps:
+
+1. Clone the default python environment that ESRI provides.
+
+    ![clone_environment](docs/images/arcgis_clone_environment.png)
+
+2. Name your new environment to something that you will recognize
+
+    ![name_new_environment](docs/images/new_environment.png)
+
+3. Activate the newly created environment
+    
+    ![activate](docs/images/activate.png)
+
+4. Close ArcGIS Pro, and open the Python Command Prompt
+    
+    ![python_command_prompt](docs/images/python_command_prompt.png)
+
+5. Install the toolbox by running `pip install doppkit-esri-toolbox`
+    
+    ```doscon
+    (doppkit) C:\Users\ogi\AppData\Local\ESRI\conda\envs\doppkit> pip install doppkit-esri-toolbox
+    ```
+
+    If users do not have access to https://pypi.org, but have the wheel and its dependencies
+    stored in a directory, they can install from that directory itself.
+
+    ```doscon
+    (doppkit) C:\Users\ogi\AppData\Local\ESRI\conda\envs\doppkit>pip install ^
+        --find-links <path-to-directory> ^
+        doppkit-esri-toolbox
+    ```
+
+6. Start ArcGIS in the Geoprocessing tab, look at the list of toolboxes and find GRiD Sync
+    
+    ![find_toolbox](docs/images/toolbox.png)
+
+7. When the toolbox is loaded, it is ready for use
+    
+    ![toolbox_loaded](docs/images/toolbox_loaded.png)
+
+## Dependencies
+
+* ArcGIS Pro 3.0+ 
+* doppkit
+* aiofiles
+* httpx
+* werkzeug
+* click
+* rich
+
+## License
+
+Apache v2.0
+
+
+
```

### Comparing `doppkit-esri-toolbox-0.1.0/pyproject.toml` & `doppkit-esri-toolbox-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[project]
-name = "doppkit-esri-toolbox"
-dynamic = ["version", "readme"]
-requires-python = ">=3.9"
-license = { file="LICENSE" }
-description = "Tool to allow retrival of USACE GRiD data"
-dependencies = [
-    "doppkit"
-]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Intended Audience :: Information Technology",
-  "Intended Audience :: Science/Research",
-  "License :: OSI Approved :: Apache Software License",
-  "Topic :: Scientific/Engineering :: GIS",
-]
-maintainers = [
-    { name = "Ognyan Moore", email = "ogi@hobu.co" },
-]
-
-[project.urls]
-homepage = "https://github.com/hobuinc/doppkit-esri-toolbox"
-repository = "https://github.com/hobuinc/doppkit-esri-toolbox"
-
-[tool.setuptools]
-package-dir = {"" =  "src"}
-zip-safe = false
-
-[tool.setuptools.dynamic]
-version = { attr = "doppkit_toolbox.__version__" }
-readme = { file = ["README.md"] }
-
-[build-system]
-requires = ["setuptools>=64.0"]
+[project]
+name = "doppkit-esri-toolbox"
+dynamic = ["version", "readme"]
+requires-python = ">=3.9"
+license = { file="LICENSE" }
+description = "Tool to allow retrival of USACE GRiD data"
+dependencies = [
+    "doppkit"
+]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Intended Audience :: Information Technology",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: Apache Software License",
+  "Topic :: Scientific/Engineering :: GIS",
+]
+maintainers = [
+    { name = "Ognyan Moore", email = "ogi@hobu.co" },
+]
+
+[project.urls]
+homepage = "https://github.com/hobuinc/doppkit-esri-toolbox"
+repository = "https://github.com/hobuinc/doppkit-esri-toolbox"
+
+[tool.setuptools]
+package-dir = {"" =  "src"}
+zip-safe = false
+
+[tool.setuptools.dynamic]
+version = { attr = "doppkit_toolbox.__version__" }
+readme = { file = "README.md", content-type = "text/markdown" }
+
+[build-system]
+requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `doppkit-esri-toolbox-0.1.0/src/doppkit_esri_toolbox.egg-info/PKG-INFO` & `doppkit-esri-toolbox-0.1.1/src/doppkit_esri_toolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,220 +1,282 @@
-Metadata-Version: 2.1
-Name: doppkit-esri-toolbox
-Version: 0.1.0
-Summary: Tool to allow retrival of USACE GRiD data
-Maintainer-email: Ognyan Moore <ogi@hobu.co>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: homepage, https://github.com/hobuinc/doppkit-esri-toolbox
-Project-URL: repository, https://github.com/hobuinc/doppkit-esri-toolbox
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-# doppkit-esri-toolbox
-ArcGIS Pro Toolbox to Interact with GRID
+Metadata-Version: 2.1
+Name: doppkit-esri-toolbox
+Version: 0.1.1
+Summary: Tool to allow retrival of USACE GRiD data
+Maintainer-email: Ognyan Moore <ogi@hobu.co>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: homepage, https://github.com/hobuinc/doppkit-esri-toolbox
+Project-URL: repository, https://github.com/hobuinc/doppkit-esri-toolbox
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# doppkit-esri-toolbox
+
+ArcGIS Pro Toolbox to Interact with GRiD.  The toolbox provides ArcGIS users to interact with the doppkit utility to
+retrieve exports from GRiD.
+
+## Installation
+
+Installation of the doppkit toolkit into ArcGIS pro can be done via the following steps:
+
+1. Clone the default python environment that ESRI provides.
+
+    ![clone_environment](docs/images/arcgis_clone_environment.png)
+
+2. Name your new environment to something that you will recognize
+
+    ![name_new_environment](docs/images/new_environment.png)
+
+3. Activate the newly created environment
+    
+    ![activate](docs/images/activate.png)
+
+4. Close ArcGIS Pro, and open the Python Command Prompt
+    
+    ![python_command_prompt](docs/images/python_command_prompt.png)
+
+5. Install the toolbox by running `pip install doppkit-esri-toolbox`
+    
+    ```doscon
+    (doppkit) C:\Users\ogi\AppData\Local\ESRI\conda\envs\doppkit> pip install doppkit-esri-toolbox
+    ```
+
+    If users do not have access to https://pypi.org, but have the wheel and its dependencies
+    stored in a directory, they can install from that directory itself.
+
+    ```doscon
+    (doppkit) C:\Users\ogi\AppData\Local\ESRI\conda\envs\doppkit>pip install ^
+        --find-links <path-to-directory> ^
+        doppkit-esri-toolbox
+    ```
+
+6. Start ArcGIS in the Geoprocessing tab, look at the list of toolboxes and find GRiD Sync
+    
+    ![find_toolbox](docs/images/toolbox.png)
+
+7. When the toolbox is loaded, it is ready for use
+    
+    ![toolbox_loaded](docs/images/toolbox_loaded.png)
+
+## Dependencies
+
+* ArcGIS Pro 3.0+ 
+* doppkit
+* aiofiles
+* httpx
+* werkzeug
+* click
+* rich
+
+## License
+
+Apache v2.0
+
+
+
```

### Comparing `doppkit-esri-toolbox-0.1.0/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py` & `doppkit-esri-toolbox-0.1.1/src/doppkit_toolbox/esri/arcpy/doppkit_wrapper_toolbox.py`

 * *Files identical despite different names*

