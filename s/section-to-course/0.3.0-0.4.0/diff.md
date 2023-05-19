# Comparing `tmp/section-to-course-0.3.0.tar.gz` & `tmp/section-to-course-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "section-to-course-0.3.0.tar", last modified: Mon May 15 15:00:23 2023, max compression
+gzip compressed data, was "section-to-course-0.4.0.tar", last modified: Fri May 19 08:08:52 2023, max compression
```

## Comparing `section-to-course-0.3.0.tar` & `section-to-course-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-15 15:00:16.000000 section-to-course-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-15 15:00:16.000000 section-to-course-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-15 15:00:16.000000 section-to-course-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-05-15 15:00:23.911131 section-to-course-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-05-15 15:00:16.000000 section-to-course-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-15 15:00:16.000000 section-to-course-0.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-15 15:00:16.000000 section-to-course-0.3.0/requirements/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4820 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/commands/section_to_course.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/settings/common.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.903130 section-to-course-0.3.0/section_to_course/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.903130 section-to-course-0.3.0/section_to_course/static/section_to_course/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/static/section_to_course/js/
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/static/section_to_course/js/admin-tools.js
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-15 15:00:23.911131 section-to-course-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5320 2023-05-15 15:00:16.000000 section-to-course-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-19 08:08:48.000000 section-to-course-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-19 08:08:48.000000 section-to-course-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-19 08:08:48.000000 section-to-course-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8056 2023-05-19 08:08:52.529371 section-to-course-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-05-19 08:08:48.000000 section-to-course-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.525371 section-to-course-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-19 08:08:48.000000 section-to-course-0.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-19 08:08:48.000000 section-to-course-0.4.0/requirements/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.525371 section-to-course-0.4.0/section_to_course/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13797 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4814 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/management/commands/section_to_course.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/settings/common.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.525371 section-to-course-0.4.0/section_to_course/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.525371 section-to-course-0.4.0/section_to_course/static/section_to_course/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.529371 section-to-course-0.4.0/section_to_course/static/section_to_course/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/static/section_to_course/js/admin-tools.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-19 08:08:48.000000 section-to-course-0.4.0/section_to_course/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 08:08:52.525371 section-to-course-0.4.0/section_to_course.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8056 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-19 08:08:52.000000 section-to-course-0.4.0/section_to_course.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-19 08:08:52.529371 section-to-course-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5320 2023-05-19 08:08:48.000000 section-to-course-0.4.0/setup.py
```

### Comparing `section-to-course-0.3.0/CHANGELOG.rst` & `section-to-course-0.4.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Change Log
 ##########
 
 ..
    All enhancements and patches to section_to_course will be documented
-   in this file.  It adheres to the structure of https://keepachangelog.com/ ,
+   in this file. It adheres to the structure of https://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+
+[0.4.0] - 2023-05-18
+********************
+
+Changed
+=======
+
+* Removed course autocomplete for performance reasons. Source courses must now be specified by course key pasted into the source course ID field.
+
+Added
+=====
+
+* Github integration-tests action.
 
 [0.3.0] - 2023-05-12
 ********************
 
 Changed
 =======
```

### Comparing `section-to-course-0.3.0/LICENSE.txt` & `section-to-course-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/PKG-INFO` & `section-to-course-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: section-to-course
-Version: 0.3.0
+Version: 0.4.0
 Summary: Factors sections from Open edX courses into their own new course.
 Home-page: https://github.com/open-craft/section-to-course
 Author: OpenCraft
 Author-email: help@opencraft.com
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -168,26 +168,38 @@
 
 
 Change Log
 ##########
 
 ..
    All enhancements and patches to section_to_course will be documented
-   in this file.  It adheres to the structure of https://keepachangelog.com/ ,
+   in this file. It adheres to the structure of https://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+
+[0.4.0] - 2023-05-18
+********************
+
+Changed
+=======
+
+* Removed course autocomplete for performance reasons. Source courses must now be specified by course key pasted into the source course ID field.
+
+Added
+=====
+
+* Github integration-tests action.
 
 [0.3.0] - 2023-05-12
 ********************
 
 Changed
 =======
```

### Comparing `section-to-course-0.3.0/README.rst` & `section-to-course-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/requirements/constraints.txt` & `section-to-course-0.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/admin.py` & `section-to-course-0.4.0/section_to_course/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,26 +72,14 @@
             'data-allow-clear': json.dumps(not self.is_required),
             'data-placeholder': '',  # Allows clearing of the input.
             'class': attrs['class'] + (' ' if attrs['class'] else '') + 'admin-autocomplete',
         })
         return attrs
 
 
-class CourseAutocompleteSelect(ArbitraryAutocompleteSelect):
-    """
-    Widget which will autocomplete course IDs.
-    """
-
-    def get_url(self):
-        """
-        Get the URL for the course autocomplete function.
-        """
-        return reverse('section_to_course:course_autocomplete')
-
-
 class SectionAutocompleteSelect(ArbitraryAutocompleteSelect):
     """
     Widget which will autocomplete section IDs.
     """
 
     def __init__(self, *args, course_field=None, **kwargs):
         """
@@ -155,15 +143,14 @@
 class CreateSectionToCourseLink(forms.ModelForm):
     """
     Form for creating a new section to course link.
     """
 
     source_course_id = forms.CharField(
         max_length=127,
-        widget=CourseAutocompleteSelect('source_course_id'),
     )
     source_section_id = forms.CharField(
         max_length=255,
         widget=SectionAutocompleteSelect(
             'source_section_id',
             course_field='source_course_id',
         ),
```

### Comparing `section-to-course-0.3.0/section_to_course/api/views.py` & `section-to-course-0.4.0/section_to_course/api/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,18 @@
 from opaque_keys import InvalidKeyError
 from opaque_keys.edx.keys import CourseKey
 from rest_framework import status
 from rest_framework.permissions import IsAdminUser
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from ..compat import course_exists, get_course_outline, modulestore
+from ..compat import course_exists, get_course_outline
 from ..models import SectionToCourseLink
 
 
-class CourseAutocomplete(APIView):
-    """
-    Autocomplete API endpoint for courses.
-    """
-
-    permission_classes = [IsAdminUser]
-
-    def get(self, request):
-        """
-        Get all courses and match a search term against them.
-        """
-        self.check_permissions(request)
-        section_courses = set(SectionToCourseLink.objects.values_list('destination_course_id', flat=True))
-        all_courses = [
-            {'id': str(course.id), 'text': f'{course.display_name} ({course.id})'}
-            for course in modulestore().get_courses()
-            if course.id not in section_courses
-        ]
-        term = request.GET.get('term', '').lower()
-        courses = [
-            entry for entry in all_courses
-            if entry['id'].lower().startswith(term) or entry['text'].lower().startswith(term)
-        ]
-        return Response(data={'results': courses}, status=status.HTTP_200_OK)
-
-
 class SectionAutocomplete(APIView):
     """
     Autocomplete API endpoint for course sections.
     """
 
     permission_classes = [IsAdminUser]
```

### Comparing `section-to-course-0.3.0/section_to_course/apps.py` & `section-to-course-0.4.0/section_to_course/apps.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/compat.py` & `section-to-course-0.4.0/section_to_course/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     return modulestore().has_course(course_key)
 
 
 def get_course(course_key: CourseLocator):
     """
     Get a course from the modulestore.
     """
-    return modulestore().get_course(course_key)
+    return get_course_outline(course_key)
 
 
 def modulestore():
     """
     Get the modulestore function from upstream.
     """
     from xmodule.modulestore.django import modulestore as upstream_modulestore
```

### Comparing `section-to-course-0.3.0/section_to_course/management/commands/section_to_course.py` & `section-to-course-0.4.0/section_to_course/management/commands/section_to_course.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/migrations/0001_initial.py` & `section-to-course-0.4.0/section_to_course/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/models.py` & `section-to-course-0.4.0/section_to_course/models.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/static/section_to_course/js/admin-tools.js` & `section-to-course-0.4.0/section_to_course/static/section_to_course/js/admin-tools.js`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course/utils.py` & `section-to-course-0.4.0/section_to_course/utils.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/section_to_course.egg-info/PKG-INFO` & `section-to-course-0.4.0/section_to_course.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: section-to-course
-Version: 0.3.0
+Version: 0.4.0
 Summary: Factors sections from Open edX courses into their own new course.
 Home-page: https://github.com/open-craft/section-to-course
 Author: OpenCraft
 Author-email: help@opencraft.com
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -168,26 +168,38 @@
 
 
 Change Log
 ##########
 
 ..
    All enhancements and patches to section_to_course will be documented
-   in this file.  It adheres to the structure of https://keepachangelog.com/ ,
+   in this file. It adheres to the structure of https://keepachangelog.com/ ,
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+
+[0.4.0] - 2023-05-18
+********************
+
+Changed
+=======
+
+* Removed course autocomplete for performance reasons. Source courses must now be specified by course key pasted into the source course ID field.
+
+Added
+=====
+
+* Github integration-tests action.
 
 [0.3.0] - 2023-05-12
 ********************
 
 Changed
 =======
```

### Comparing `section-to-course-0.3.0/section_to_course.egg-info/SOURCES.txt` & `section-to-course-0.4.0/section_to_course.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.3.0/setup.py` & `section-to-course-0.4.0/setup.py`

 * *Files identical despite different names*

