# Comparing `tmp/crossmark-jotform-api-0.3.1.tar.gz` & `tmp/crossmark-jotform-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.3.1.tar", last modified: Tue May 16 18:36:04 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.3.2.tar", last modified: Thu May 18 22:11:55 2023, max compression
```

## Comparing `crossmark-jotform-api-0.3.1.tar` & `crossmark-jotform-api-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.826363 crossmark-jotform-api-0.3.1/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-05-16 18:36:04.825364 crossmark-jotform-api-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.1/README.md
--rw-rw-rw-   0        0        0      789 2023-05-16 18:34:10.000000 crossmark-jotform-api-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 18:36:04.826363 crossmark-jotform-api-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.795361 crossmark-jotform-api-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.806360 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12969 2023-05-16 18:34:02.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.823363 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2770 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.824361 crossmark-jotform-api-0.3.1/test/
--rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.1/test/test_jotform_class.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.2/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-18 22:10:35.000000 crossmark-jotform-api-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.282965 crossmark-jotform-api-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.287957 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12736 2023-05-18 21:09:04.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.300955 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2770 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.301956 crossmark-jotform-api-0.3.2/test/
+-rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.2/test/test_jotform_class.py
```

### Comparing `crossmark-jotform-api-0.3.1/LICENSE` & `crossmark-jotform-api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.1/PKG-INFO` & `crossmark-jotform-api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.3.1/README.md` & `crossmark-jotform-api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.1/pyproject.toml` & `crossmark-jotform-api-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/jotForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,18 +222,15 @@
         self.new = submission_object['new']
         self.flag = submission_object['flag']
         self.notes = submission_object['notes']
         self.updated_at = submission_object['updated_at']
         self.answers = submission_object['answers']
         self.answers_arr = self.set_answers(self.answers)
         self.case_id = self.get_answer_by_text('CASE')['answer']
-        self.editor = self.get_answer_by_text('EDITOR')['answer']
-        self.status = self.get_answer_by_text('STATUS')['answer']
         self.store = self.get_answer_by_text('STORE')['answer']
-        self.GUID = self.get_answer_by_text('GUID')['answer']
         self.client = self.get_answer_by_text('CLIENT')['answer']
         self.emails = self.get_emails()
 
     def set_answers(self, answers):
         answers_arr = []
         for key, value in answers.items():
             if 'name' in value:
@@ -323,20 +320,18 @@
 
     def to_dict(self):
         return {
             'id': self.id,
             'form_id': self.form_id,
             'ip': self.ip,
             'created_at': self.get_day_from_date(self.created_at),
-            'status': self.status,
+            'status': self.get_answer_by_text('STATUS')['answer'],
             'new': self.new,
             'flag': self.flag,
             'notes': self.notes,
             'updated_at': self.updated_at,
             'case_id': self.case_id,
-            'editor': self.editor,
             'store': self.store,
             'store_number': self.get_store_number_from_store(self.store),
-            'GUID': self.GUID,
             'client': self.client,
             'emails': self.get_emails(),
         }
```

### Comparing `crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

