# Comparing `tmp/djangoldp_application-1.1.1.tar.gz` & `tmp/djangoldp_application-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.1.1.tar", last modified: Fri May 19 14:19:14 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.1.2.tar", last modified: Fri May 19 14:58:01 2023, max compression
```

## Comparing `djangoldp_application-1.1.1.tar` & `djangoldp_application-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:19:13.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:19:13.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 14:19:13.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 14:19:13.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 14:19:13.000000 djangoldp_application-1.1.1/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    14085 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5406 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 14:19:11.000000 djangoldp_application-1.1.1/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:19:14.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 14:18:53.000000 djangoldp_application-1.1.1/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    15193 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5406 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-19 14:57:58.000000 djangoldp_application-1.1.2/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:58:01.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-19 14:57:43.000000 djangoldp_application-1.1.2/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.1.1/README.md` & `djangoldp_application-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/setup.cfg` & `djangoldp_application-1.1.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 description = djangoldp application management package
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
 	djangoldp~=2.1
+	djangoldp_branding
 	djangoldp_account~=2.3
 	djangoldp_component
 	djangorestframework-yaml~=2.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_application/__init__.py:__version__
```

### Comparing `djangoldp_application-1.1.1/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.1.2/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/views.py` & `djangoldp_application-1.1.2/djangoldp_application/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .models import Application, Federation
 from django.conf import settings
 from django.core.mail import send_mail
 from django.http import JsonResponse
+from django.template import loader
 from django.utils.translation import ugettext_lazy as _
 from djangoldp_component.models import Component, Package
 from rest_framework import serializers, viewsets
 from rest_framework_yaml.parsers import YAMLParser
 from rest_framework_yaml.renderers import YAMLRenderer
 
 
@@ -54,23 +55,30 @@
 
         federation = []
         for host in application["federation"]:
             federation.append(Federation.objects.get(urlid=host).target.api_url)
 
         serialized = {"apps": {"hosts": {}}}
         serialized["apps"]["hosts"][application["slug"]] = {
-            "graphics": {
-                "client": application["client_url"],
-                "canva": application["repository"],
-            },
+            "graphics": {},
             "data": {"api": application["api_url"], "with": federation},
             "packages": [],
             "components": [],
         }
 
+        if application["client_url"]:
+            serialized["apps"]["hosts"][application["slug"]]["graphics"][
+                "client"
+            ] = application["client_url"]
+
+        if application["repository"]:
+            serialized["apps"]["hosts"][application["slug"]]["graphics"][
+                "canva"
+            ] = application["repository"]
+
         if application["application_title"]:
             serialized["apps"]["hosts"][application["slug"]]["graphics"][
                 "title"
             ] = application["application_title"]
 
         if application["application_logo"]:
             serialized["apps"]["hosts"][application["slug"]]["graphics"][
@@ -273,42 +281,60 @@
 def mark_as_done(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Done"
             deploy.save()
             if deploy.requester:
-                message = _("Woah! Deployment done!")
+                html_message = loader.render_to_string(
+                    'email.html',
+                    {
+                        'on': application.client_url,
+                        'instance': {"summary": "Deployment done"},
+                        'author': deploy.requester.get_full_name(),
+                        'object': _("about your deployment of") + " https://{}".format(application.client_url)
+                    }
+                )
+
                 send_mail(
                     _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
-                    message,
+                    "Deployment done",
                     EMAIL_FROM,
                     [deploy.requester.email],
                     fail_silently=True,
-                    html_message=message
+                    html_message=html_message
                 )
 
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
 
 
 def mark_as_failed(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Failed"
             deploy.save()
             if deploy.requester:
-                message = _("Woah! Deployment failed!")
+                html_message = loader.render_to_string(
+                    'email.html',
+                    {
+                        'on': application.client_url,
+                        'instance': {"summary": "Deployment failed"},
+                        'author': deploy.requester.get_full_name(),
+                        'object': _("about your deployment of") + " https://{}".format(application.client_url)
+                    }
+                )
+
                 send_mail(
                     _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
-                    message,
+                    "Deployment failed",
                     EMAIL_FROM,
                     [deploy.requester.email],
                     fail_silently=True,
-                    html_message=message
+                    html_message=html_message
                 )
 
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
```

### Comparing `djangoldp_application-1.1.1/djangoldp_application/models.py` & `djangoldp_application-1.1.2/djangoldp_application/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/admin.py` & `djangoldp_application-1.1.2/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-1.1.2/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.1/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.1.2/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

