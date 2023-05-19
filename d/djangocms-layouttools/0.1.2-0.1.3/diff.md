# Comparing `tmp/djangocms-layouttools-0.1.2.tar.gz` & `tmp/djangocms-layouttools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-layouttools-0.1.2.tar", last modified: Tue Jan 12 07:04:15 2021, max compression
+gzip compressed data, was "djangocms-layouttools-0.1.3.tar", last modified: Fri May 19 16:54:51 2023, max compression
```

## Comparing `djangocms-layouttools-0.1.2.tar` & `djangocms-layouttools-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.992563 djangocms-layouttools-0.1.2/
--rw-r--r--   0 russmo     (501) staff       (20)     1090 2018-03-01 00:34:30.000000 djangocms-layouttools-0.1.2/LICENSE.txt
--rw-r--r--   0 russmo     (501) staff       (20)      166 2018-03-06 20:48:10.000000 djangocms-layouttools-0.1.2/MANIFEST.in
--rw-r--r--   0 russmo     (501) staff       (20)     3889 2021-01-12 07:04:15.992770 djangocms-layouttools-0.1.2/PKG-INFO
--rw-r--r--   0 russmo     (501) staff       (20)     1996 2021-01-12 06:57:13.000000 djangocms-layouttools-0.1.2/README.rst
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.985955 djangocms-layouttools-0.1.2/djangocms_layouttools/
--rw-r--r--   0 russmo     (501) staff       (20)       46 2021-01-12 06:35:52.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)      624 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/admin.py
--rw-r--r--   0 russmo     (501) staff       (20)      185 2018-03-06 20:47:21.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/apps.py
--rw-r--r--   0 russmo     (501) staff       (20)     1213 2018-03-06 20:40:22.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/cms_plugins.py
--rw-r--r--   0 russmo     (501) staff       (20)      240 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/fields.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.990204 djangocms-layouttools-0.1.2/djangocms_layouttools/migrations/
--rw-r--r--   0 russmo     (501) staff       (20)     3768 2018-03-13 17:56:36.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/migrations/0001_initial.py
--rw-r--r--   0 russmo     (501) staff       (20)        0 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/migrations/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)     4550 2021-01-12 06:32:31.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/models.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.978298 djangocms-layouttools-0.1.2/djangocms_layouttools/templates/
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.990602 djangocms-layouttools-0.1.2/djangocms_layouttools/templates/djangocms_layouttools/
--rw-r--r--   0 russmo     (501) staff       (20)      953 2018-03-05 20:05:37.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/templates/djangocms_layouttools/section.html
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.992219 djangocms-layouttools-0.1.2/djangocms_layouttools/tests/
--rw-r--r--   0 russmo     (501) staff       (20)       24 2018-03-01 20:48:06.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/tests/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)      460 2018-03-01 20:49:29.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/tests/settings.py
--rw-r--r--   0 russmo     (501) staff       (20)      673 2018-03-01 23:37:26.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/tests/tests_models.py
--rw-r--r--   0 russmo     (501) staff       (20)       63 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.2/djangocms_layouttools/views.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2021-01-12 07:04:15.989210 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/
--rw-r--r--   0 russmo     (501) staff       (20)     3889 2021-01-12 07:04:15.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/PKG-INFO
--rw-r--r--   0 russmo     (501) staff       (20)      833 2021-01-12 07:04:15.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/SOURCES.txt
--rw-r--r--   0 russmo     (501) staff       (20)        1 2021-01-12 07:04:15.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/dependency_links.txt
--rw-r--r--   0 russmo     (501) staff       (20)        1 2018-03-06 20:50:50.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/not-zip-safe
--rw-r--r--   0 russmo     (501) staff       (20)       72 2021-01-12 07:04:15.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/requires.txt
--rw-r--r--   0 russmo     (501) staff       (20)       22 2021-01-12 07:04:15.000000 djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/top_level.txt
--rw-r--r--   0 russmo     (501) staff       (20)      172 2021-01-12 07:04:15.993469 djangocms-layouttools-0.1.2/setup.cfg
--rw-r--r--   0 russmo     (501) staff       (20)     1753 2021-01-12 07:04:03.000000 djangocms-layouttools-0.1.2/setup.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.601999 djangocms-layouttools-0.1.3/
+-rw-r--r--   0 russmo     (501) staff       (20)     1090 2018-03-01 00:34:30.000000 djangocms-layouttools-0.1.3/LICENSE.txt
+-rw-r--r--   0 russmo     (501) staff       (20)      166 2018-03-06 20:48:10.000000 djangocms-layouttools-0.1.3/MANIFEST.in
+-rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 16:54:51.602080 djangocms-layouttools-0.1.3/PKG-INFO
+-rw-r--r--   0 russmo     (501) staff       (20)     1996 2021-01-12 06:57:13.000000 djangocms-layouttools-0.1.3/README.rst
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.591039 djangocms-layouttools-0.1.3/djangocms_layouttools/
+-rw-r--r--   0 russmo     (501) staff       (20)       46 2023-05-19 16:50:16.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)      624 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/admin.py
+-rw-r--r--   0 russmo     (501) staff       (20)      235 2023-05-19 16:47:54.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/apps.py
+-rw-r--r--   0 russmo     (501) staff       (20)     1213 2018-03-06 20:40:22.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/cms_plugins.py
+-rw-r--r--   0 russmo     (501) staff       (20)      240 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/fields.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.600253 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/
+-rw-r--r--   0 russmo     (501) staff       (20)     3768 2018-03-13 17:56:36.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/0001_initial.py
+-rw-r--r--   0 russmo     (501) staff       (20)        0 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)     4550 2021-01-12 06:32:31.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/models.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.585148 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.600415 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/
+-rw-r--r--   0 russmo     (501) staff       (20)      953 2018-03-05 20:05:37.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/section.html
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.601835 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/
+-rw-r--r--   0 russmo     (501) staff       (20)       24 2018-03-01 20:48:06.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)      460 2018-03-01 20:49:29.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/settings.py
+-rw-r--r--   0 russmo     (501) staff       (20)      673 2018-03-01 23:37:26.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/tests_models.py
+-rw-r--r--   0 russmo     (501) staff       (20)       63 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/views.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.599496 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/
+-rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/PKG-INFO
+-rw-r--r--   0 russmo     (501) staff       (20)      833 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/SOURCES.txt
+-rw-r--r--   0 russmo     (501) staff       (20)        1 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/dependency_links.txt
+-rw-r--r--   0 russmo     (501) staff       (20)        1 2018-03-06 20:50:50.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/not-zip-safe
+-rw-r--r--   0 russmo     (501) staff       (20)       72 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/requires.txt
+-rw-r--r--   0 russmo     (501) staff       (20)       22 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/top_level.txt
+-rw-r--r--   0 russmo     (501) staff       (20)      172 2023-05-19 16:54:51.603000 djangocms-layouttools-0.1.3/setup.cfg
+-rw-r--r--   0 russmo     (501) staff       (20)     1753 2021-01-12 07:04:03.000000 djangocms-layouttools-0.1.3/setup.py
```

### Comparing `djangocms-layouttools-0.1.2/LICENSE.txt` & `djangocms-layouttools-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/PKG-INFO` & `djangocms-layouttools-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,15 @@
 Metadata-Version: 2.1
 Name: djangocms-layouttools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adds layout Section and other plugins to django CMS.
 Home-page: https://github.com/mci/djangocms-layouttools
 Author: Russell Moffitt, Marine Conservation Institute
 Author-email: Russell.Moffitt@marine-conservation.org
 License: MIT
-Description: ================
-        Django CMS LayoutTools
-        ================
-        
-        
-        |pypi| |build| |coverage|
-        
-        **Django CMS LayoutTools** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allows you to design content sections on cms webpages that have specified 
-        container properties (e.g., container-fluid) and css styling such as backgrounds.
-        It uses Bootstrap3 container classes by default, but doesn't necessarily require
-        Bootstrap to be a useful tool for sectioning and styling content. A Section plugin
-        is provided now, but further plugins may be created at a later date.
-        
-        It uses images/files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. See the github repo 
-        `contribution guidelines https://github.com/mci/djangocms-layouttools>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/mci/djangocms-layouttools/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        * Python 2.7, 3.3 or higher
-        * Django 1.8 or higher
-        * Django Filer 1.2.4 or higher
-        
-        Make sure `django Filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-layouttools``
-        * add ``djangocms_layouttools`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_layouttools``
-        
-        
-        Configuration
-        -------------
-        
-        TBD
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-layouttools.svg
-            :target: http://badge.fury.io/py/djangocms-layouttools
-        .. |build| image:: https://travis-ci.org/mci/djangocms-layouttools.svg?branch=master
-            :target: https://travis-ci.org/mci/djangocms-layouttools
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -94,7 +22,79 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+================
+Django CMS LayoutTools
+================
+
+
+|pypi| |build| |coverage|
+
+**Django CMS LayoutTools** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allows you to design content sections on cms webpages that have specified 
+container properties (e.g., container-fluid) and css styling such as backgrounds.
+It uses Bootstrap3 container classes by default, but doesn't necessarily require
+Bootstrap to be a useful tool for sectioning and styling content. A Section plugin
+is provided now, but further plugins may be created at a later date.
+
+It uses images/files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. See the github repo 
+`contribution guidelines https://github.com/mci/djangocms-layouttools>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/mci/djangocms-layouttools/blob/master/setup.py>`_
+file for additional dependencies:
+
+* Python 2.7, 3.3 or higher
+* Django 1.8 or higher
+* Django Filer 1.2.4 or higher
+
+Make sure `django Filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-layouttools``
+* add ``djangocms_layouttools`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_layouttools``
+
+
+Configuration
+-------------
+
+TBD
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-layouttools.svg
+    :target: http://badge.fury.io/py/djangocms-layouttools
+.. |build| image:: https://travis-ci.org/mci/djangocms-layouttools.svg?branch=master
+    :target: https://travis-ci.org/mci/djangocms-layouttools
```

### Comparing `djangocms-layouttools-0.1.2/README.rst` & `djangocms-layouttools-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/admin.py` & `djangocms-layouttools-0.1.3/djangocms_layouttools/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/cms_plugins.py` & `djangocms-layouttools-0.1.3/djangocms_layouttools/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/migrations/0001_initial.py` & `djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/models.py` & `djangocms-layouttools-0.1.3/djangocms_layouttools/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/templates/djangocms_layouttools/section.html` & `djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/section.html`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools/tests/tests_models.py` & `djangocms-layouttools-0.1.3/djangocms_layouttools/tests/tests_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/PKG-INFO` & `djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,15 @@
 Metadata-Version: 2.1
 Name: djangocms-layouttools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adds layout Section and other plugins to django CMS.
 Home-page: https://github.com/mci/djangocms-layouttools
 Author: Russell Moffitt, Marine Conservation Institute
 Author-email: Russell.Moffitt@marine-conservation.org
 License: MIT
-Description: ================
-        Django CMS LayoutTools
-        ================
-        
-        
-        |pypi| |build| |coverage|
-        
-        **Django CMS LayoutTools** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allows you to design content sections on cms webpages that have specified 
-        container properties (e.g., container-fluid) and css styling such as backgrounds.
-        It uses Bootstrap3 container classes by default, but doesn't necessarily require
-        Bootstrap to be a useful tool for sectioning and styling content. A Section plugin
-        is provided now, but further plugins may be created at a later date.
-        
-        It uses images/files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. See the github repo 
-        `contribution guidelines https://github.com/mci/djangocms-layouttools>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/mci/djangocms-layouttools/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        * Python 2.7, 3.3 or higher
-        * Django 1.8 or higher
-        * Django Filer 1.2.4 or higher
-        
-        Make sure `django Filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-layouttools``
-        * add ``djangocms_layouttools`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_layouttools``
-        
-        
-        Configuration
-        -------------
-        
-        TBD
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-layouttools.svg
-            :target: http://badge.fury.io/py/djangocms-layouttools
-        .. |build| image:: https://travis-ci.org/mci/djangocms-layouttools.svg?branch=master
-            :target: https://travis-ci.org/mci/djangocms-layouttools
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -94,7 +22,79 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+================
+Django CMS LayoutTools
+================
+
+
+|pypi| |build| |coverage|
+
+**Django CMS LayoutTools** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allows you to design content sections on cms webpages that have specified 
+container properties (e.g., container-fluid) and css styling such as backgrounds.
+It uses Bootstrap3 container classes by default, but doesn't necessarily require
+Bootstrap to be a useful tool for sectioning and styling content. A Section plugin
+is provided now, but further plugins may be created at a later date.
+
+It uses images/files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. See the github repo 
+`contribution guidelines https://github.com/mci/djangocms-layouttools>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/mci/djangocms-layouttools/blob/master/setup.py>`_
+file for additional dependencies:
+
+* Python 2.7, 3.3 or higher
+* Django 1.8 or higher
+* Django Filer 1.2.4 or higher
+
+Make sure `django Filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-layouttools``
+* add ``djangocms_layouttools`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_layouttools``
+
+
+Configuration
+-------------
+
+TBD
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-layouttools.svg
+    :target: http://badge.fury.io/py/djangocms-layouttools
+.. |build| image:: https://travis-ci.org/mci/djangocms-layouttools.svg?branch=master
+    :target: https://travis-ci.org/mci/djangocms-layouttools
```

### Comparing `djangocms-layouttools-0.1.2/djangocms_layouttools.egg-info/SOURCES.txt` & `djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.2/setup.py` & `djangocms-layouttools-0.1.3/setup.py`

 * *Files identical despite different names*

