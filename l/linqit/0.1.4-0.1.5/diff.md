# Comparing `tmp/linqit-0.1.4.tar.gz` & `tmp/linqit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linqit-0.1.4.tar", last modified: Thu Jun  3 09:10:08 2021, max compression
+gzip compressed data, was "linqit-0.1.5.tar", last modified: Fri May 19 10:06:10 2023, max compression
```

## Comparing `linqit-0.1.4.tar` & `linqit-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 avilumelsky   (501) staff       (20)        0 2021-06-03 09:10:08.406356 linqit-0.1.4/
--rw-r--r--   0 avilumelsky   (501) staff       (20)    11357 2020-11-04 13:28:13.000000 linqit-0.1.4/LICENSE
--rw-r--r--   0 avilumelsky   (501) staff       (20)     4560 2021-06-03 09:10:08.406068 linqit-0.1.4/PKG-INFO
--rw-r--r--   0 avilumelsky   (501) staff       (20)     3912 2021-06-03 08:58:53.000000 linqit-0.1.4/README.md
-drwxr-xr-x   0 avilumelsky   (501) staff       (20)        0 2021-06-03 09:10:08.403895 linqit-0.1.4/linqit/
--rw-r--r--   0 avilumelsky   (501) staff       (20)     7733 2021-06-03 08:58:53.000000 linqit-0.1.4/linqit/__init__.py
-drwxr-xr-x   0 avilumelsky   (501) staff       (20)        0 2021-06-03 09:10:08.405002 linqit-0.1.4/linqit.egg-info/
--rw-r--r--   0 avilumelsky   (501) staff       (20)     4560 2021-06-03 09:10:08.000000 linqit-0.1.4/linqit.egg-info/PKG-INFO
--rw-r--r--   0 avilumelsky   (501) staff       (20)      202 2021-06-03 09:10:08.000000 linqit-0.1.4/linqit.egg-info/SOURCES.txt
--rw-r--r--   0 avilumelsky   (501) staff       (20)        1 2021-06-03 09:10:08.000000 linqit-0.1.4/linqit.egg-info/dependency_links.txt
--rw-r--r--   0 avilumelsky   (501) staff       (20)       13 2021-06-03 09:10:08.000000 linqit-0.1.4/linqit.egg-info/top_level.txt
--rw-r--r--   0 avilumelsky   (501) staff       (20)       38 2021-06-03 09:10:08.406446 linqit-0.1.4/setup.cfg
--rw-r--r--   0 avilumelsky   (501) staff       (20)      845 2021-06-03 09:09:23.000000 linqit-0.1.4/setup.py
-drwxr-xr-x   0 avilumelsky   (501) staff       (20)        0 2021-06-03 09:10:08.405674 linqit-0.1.4/tests/
--rw-r--r--   0 avilumelsky   (501) staff       (20)        0 2020-11-04 13:28:13.000000 linqit-0.1.4/tests/__init__.py
--rw-r--r--   0 avilumelsky   (501) staff       (20)    10192 2021-06-03 08:58:53.000000 linqit-0.1.4/tests/test_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:06:10.471026 linqit-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 10:05:54.000000 linqit-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-19 10:06:10.471026 linqit-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-19 10:05:54.000000 linqit-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:06:10.467026 linqit-0.1.5/linqit/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 10:05:54.000000 linqit-0.1.5/linqit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-05-19 10:05:54.000000 linqit-0.1.5/linqit/linq_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:06:10.471026 linqit-0.1.5/linqit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-19 10:06:10.000000 linqit-0.1.5/linqit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 10:06:10.000000 linqit-0.1.5/linqit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:06:10.000000 linqit-0.1.5/linqit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 10:06:10.000000 linqit-0.1.5/linqit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:06:10.471026 linqit-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-19 10:05:54.000000 linqit-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:06:10.471026 linqit-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:05:54.000000 linqit-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-05-19 10:05:54.000000 linqit-0.1.5/tests/test_list.py
```

### Comparing `linqit-0.1.4/LICENSE` & `linqit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linqit-0.1.4/PKG-INFO` & `linqit-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: linqit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extends python's list builtin with fun, robust functionality - .NET's Language Integrated Queries (Linq) and more. Write clean code with powerful syntax.
 Home-page: https://github.com/avilum/linqit
 Author: Avi Lumelsky
 Author-email: noticetheg@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linqit!
 Extends python's list builtin with fun, robust functionality - .NET's Language Integrated Queries (Linq) and more.<br>
 Write clean code with powerful syntax.<br><br>
 ```shell script
 pip install linqit
 ```
-Stop using loops, complex conditions, list comperhension and filters.<br>
+<center>
+<img src="https://img.shields.io/badge/Test Coverage-96%25-brightgreen">
+</center>
+<br>
+
+
+Stop using loops, complex conditions, list comprehension and filters.<br>
 Doesn't it looks better? <br>
 ```python
 from seven_dwwarfs import Grumpy, Happy, Sleepy, Bashful, Sneezy, Dopey, Doc
 from linqit import List
 
 # Go ahead and fill the list with whatever you want... like a list of <Programmer> objects.
 programmers = List()
@@ -85,32 +89,32 @@
 
 class Person():
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
     def __repr__(self):
-        return 'Person(name="{}", age={})'.format(self.name, self.age)
+        return f'Person(name="{self.name}", age={self.age})')
 
 
 # Creating a list of people
 avi, bill, bob, harry = Person('Avi', 23), Person('Bill', 41), Person('Bob', 77), Person('Harry', 55)
 
 people = List(avi, bill, bob, harry)
 ```
 
 ## Use LINQ selections, write cleaner code
 ```python
-old_people = people.where(lambda p: p.age > 23) # It's a joke! :) [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
-old_people.first()                                              # <Person name="Bill" age="41">
-old_people.last()                                               # <Person name="Harry" age="55">
-old_people.any(lambda p: p.name.lower().startswith('b'))        # True
-old_people.where(age=55)                         # [<Person name="Harry" age="55">]
-old_people.skip(3).any()                                        # False
-old_people.skip(2).first()                                      # <Person name="Harry" age="55">
+people = people.where(lambda p: p.age > 23) # [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
+people.first()                                              # <Person name="Bill" age="41">
+people.last()                                               # <Person name="Harry" age="55">
+people.any(lambda p: p.name.lower().startswith('b'))        # True
+people.where(age=55)                         # [<Person name="Harry" age="55">]
+people.skip(3).any()                                        # False
+people.skip(2).first()                                      # <Person name="Harry" age="55">
 
 # Isn't it better than "for", "if", "else", "filter", "map" and list comprehensions in the middle of your code?
 
 ```
 ## More selections
 ```python
 new_kids_in_town = [Person('Chris', 18), Person('Danny', 16), Person('John', 17)]
@@ -128,8 +132,19 @@
 teenagers_names = teenagers.name                                # ['Chris', 'Danny', 'John']
 teenagers_names.take(2).except_for(lambda n: n == 'Danny')      # ['Chris']
 teenagers.age.min                                               # 16
 teenagers.age.avg                                               # 17
 teenagers.age.max                                               # 18
 ```
 
-
+# Test Coverage
+```python
+➜  linqit git:(master) ✗ coverage report                    
+Name                  Stmts   Miss  Cover
+-----------------------------------------
+linqit/__init__.py        2      0   100%
+linqit/linq_list.py     101     11    89%
+tests/__init__.py         0      0   100%
+tests/test_list.py      203      0   100%
+-----------------------------------------
+TOTAL                   306     11    96%
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linqit-0.1.4/README.md` & `linqit-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Linqit!
 Extends python's list builtin with fun, robust functionality - .NET's Language Integrated Queries (Linq) and more.<br>
 Write clean code with powerful syntax.<br><br>
 ```shell script
 pip install linqit
 ```
-Stop using loops, complex conditions, list comperhension and filters.<br>
+<center>
+<img src="https://img.shields.io/badge/Test Coverage-96%25-brightgreen">
+</center>
+<br>
+
+
+Stop using loops, complex conditions, list comprehension and filters.<br>
 Doesn't it looks better? <br>
 ```python
 from seven_dwwarfs import Grumpy, Happy, Sleepy, Bashful, Sneezy, Dopey, Doc
 from linqit import List
 
 # Go ahead and fill the list with whatever you want... like a list of <Programmer> objects.
 programmers = List()
@@ -68,32 +74,32 @@
 
 class Person():
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
     def __repr__(self):
-        return 'Person(name="{}", age={})'.format(self.name, self.age)
+        return f'Person(name="{self.name}", age={self.age})')
 
 
 # Creating a list of people
 avi, bill, bob, harry = Person('Avi', 23), Person('Bill', 41), Person('Bob', 77), Person('Harry', 55)
 
 people = List(avi, bill, bob, harry)
 ```
 
 ## Use LINQ selections, write cleaner code
 ```python
-old_people = people.where(lambda p: p.age > 23) # It's a joke! :) [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
-old_people.first()                                              # <Person name="Bill" age="41">
-old_people.last()                                               # <Person name="Harry" age="55">
-old_people.any(lambda p: p.name.lower().startswith('b'))        # True
-old_people.where(age=55)                         # [<Person name="Harry" age="55">]
-old_people.skip(3).any()                                        # False
-old_people.skip(2).first()                                      # <Person name="Harry" age="55">
+people = people.where(lambda p: p.age > 23) # [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
+people.first()                                              # <Person name="Bill" age="41">
+people.last()                                               # <Person name="Harry" age="55">
+people.any(lambda p: p.name.lower().startswith('b'))        # True
+people.where(age=55)                         # [<Person name="Harry" age="55">]
+people.skip(3).any()                                        # False
+people.skip(2).first()                                      # <Person name="Harry" age="55">
 
 # Isn't it better than "for", "if", "else", "filter", "map" and list comprehensions in the middle of your code?
 
 ```
 ## More selections
 ```python
 new_kids_in_town = [Person('Chris', 18), Person('Danny', 16), Person('John', 17)]
@@ -110,7 +116,20 @@
 ages = people.age                                               # [23, 41, 77, 55, 18, 17]
 teenagers_names = teenagers.name                                # ['Chris', 'Danny', 'John']
 teenagers_names.take(2).except_for(lambda n: n == 'Danny')      # ['Chris']
 teenagers.age.min                                               # 16
 teenagers.age.avg                                               # 17
 teenagers.age.max                                               # 18
 ```
+
+# Test Coverage
+```python
+➜  linqit git:(master) ✗ coverage report                    
+Name                  Stmts   Miss  Cover
+-----------------------------------------
+linqit/__init__.py        2      0   100%
+linqit/linq_list.py     101     11    89%
+tests/__init__.py         0      0   100%
+tests/test_list.py      203      0   100%
+-----------------------------------------
+TOTAL                   306     11    96%
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linqit-0.1.4/linqit.egg-info/PKG-INFO` & `linqit-0.1.5/linqit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: linqit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extends python's list builtin with fun, robust functionality - .NET's Language Integrated Queries (Linq) and more. Write clean code with powerful syntax.
 Home-page: https://github.com/avilum/linqit
 Author: Avi Lumelsky
 Author-email: noticetheg@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linqit!
 Extends python's list builtin with fun, robust functionality - .NET's Language Integrated Queries (Linq) and more.<br>
 Write clean code with powerful syntax.<br><br>
 ```shell script
 pip install linqit
 ```
-Stop using loops, complex conditions, list comperhension and filters.<br>
+<center>
+<img src="https://img.shields.io/badge/Test Coverage-96%25-brightgreen">
+</center>
+<br>
+
+
+Stop using loops, complex conditions, list comprehension and filters.<br>
 Doesn't it looks better? <br>
 ```python
 from seven_dwwarfs import Grumpy, Happy, Sleepy, Bashful, Sneezy, Dopey, Doc
 from linqit import List
 
 # Go ahead and fill the list with whatever you want... like a list of <Programmer> objects.
 programmers = List()
@@ -85,32 +89,32 @@
 
 class Person():
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
     def __repr__(self):
-        return 'Person(name="{}", age={})'.format(self.name, self.age)
+        return f'Person(name="{self.name}", age={self.age})')
 
 
 # Creating a list of people
 avi, bill, bob, harry = Person('Avi', 23), Person('Bill', 41), Person('Bob', 77), Person('Harry', 55)
 
 people = List(avi, bill, bob, harry)
 ```
 
 ## Use LINQ selections, write cleaner code
 ```python
-old_people = people.where(lambda p: p.age > 23) # It's a joke! :) [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
-old_people.first()                                              # <Person name="Bill" age="41">
-old_people.last()                                               # <Person name="Harry" age="55">
-old_people.any(lambda p: p.name.lower().startswith('b'))        # True
-old_people.where(age=55)                         # [<Person name="Harry" age="55">]
-old_people.skip(3).any()                                        # False
-old_people.skip(2).first()                                      # <Person name="Harry" age="55">
+people = people.where(lambda p: p.age > 23) # [<Person name="Bill" age="41">, <Person name="Bob" age="77">, <Person name="Harry" age="55">]
+people.first()                                              # <Person name="Bill" age="41">
+people.last()                                               # <Person name="Harry" age="55">
+people.any(lambda p: p.name.lower().startswith('b'))        # True
+people.where(age=55)                         # [<Person name="Harry" age="55">]
+people.skip(3).any()                                        # False
+people.skip(2).first()                                      # <Person name="Harry" age="55">
 
 # Isn't it better than "for", "if", "else", "filter", "map" and list comprehensions in the middle of your code?
 
 ```
 ## More selections
 ```python
 new_kids_in_town = [Person('Chris', 18), Person('Danny', 16), Person('John', 17)]
@@ -128,8 +132,19 @@
 teenagers_names = teenagers.name                                # ['Chris', 'Danny', 'John']
 teenagers_names.take(2).except_for(lambda n: n == 'Danny')      # ['Chris']
 teenagers.age.min                                               # 16
 teenagers.age.avg                                               # 17
 teenagers.age.max                                               # 18
 ```
 
-
+# Test Coverage
+```python
+➜  linqit git:(master) ✗ coverage report                    
+Name                  Stmts   Miss  Cover
+-----------------------------------------
+linqit/__init__.py        2      0   100%
+linqit/linq_list.py     101     11    89%
+tests/__init__.py         0      0   100%
+tests/test_list.py      203      0   100%
+-----------------------------------------
+TOTAL                   306     11    96%
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linqit-0.1.4/setup.py` & `linqit-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="linqit",
-    version="0.1.4",
+    version="0.1.5",
     author="Avi Lumelsky",
     author_email="noticetheg@gmail.com",
     description="Extends python's list builtin with fun, robust functionality - "
-                ".NET's Language Integrated Queries (Linq) and more. Write clean code with powerful syntax.",
+    ".NET's Language Integrated Queries (Linq) and more. Write clean code with powerful syntax.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/avilum/linqit",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=2.7,>=3.6',
+    python_requires=">=2.7,>=3.6",
 )
```

