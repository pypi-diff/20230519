# Comparing `tmp/arithmetic-dice-roller-0.2.4.tar.gz` & `tmp/arithmetic-dice-roller-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetic-dice-roller-0.2.4.tar", last modified: Tue Dec 13 12:20:40 2022, max compression
+gzip compressed data, was "arithmetic-dice-roller-0.3.0.tar", last modified: Fri May 19 08:31:05 2023, max compression
```

## Comparing `arithmetic-dice-roller-0.2.4.tar` & `arithmetic-dice-roller-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2022-12-13 12:20:40.090977 arithmetic-dice-roller-0.2.4/
--rw-r--r--   0 damax     (1000) damax     (1000)     4593 2022-12-13 12:20:40.090977 arithmetic-dice-roller-0.2.4/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)     4054 2022-03-02 13:20:22.000000 arithmetic-dice-roller-0.2.4/README.md
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2022-12-13 12:20:40.090977 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/
--rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/__init__.py
--rw-r--r--   0 damax     (1000) damax     (1000)     1956 2022-12-13 12:06:00.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/__main__.py
--rw-r--r--   0 damax     (1000) damax     (1000)    11804 2022-12-13 12:06:00.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/roller.py
-drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2022-12-13 12:20:40.090977 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/
--rw-r--r--   0 damax     (1000) damax     (1000)     4593 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/PKG-INFO
--rw-r--r--   0 damax     (1000) damax     (1000)      399 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/SOURCES.txt
--rw-r--r--   0 damax     (1000) damax     (1000)        1 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/dependency_links.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       80 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/entry_points.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       12 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/requires.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       23 2022-12-13 12:20:40.000000 arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/top_level.txt
--rw-r--r--   0 damax     (1000) damax     (1000)       38 2022-12-13 12:20:40.090977 arithmetic-dice-roller-0.2.4/setup.cfg
--rw-r--r--   0 damax     (1000) damax     (1000)     1712 2022-12-13 12:14:57.000000 arithmetic-dice-roller-0.2.4/setup.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)     4054 2022-03-02 13:20:22.000000 arithmetic-dice-roller-0.3.0/README.md
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/
+-rw-r--r--   0 damax     (1000) damax     (1000)        0 2021-11-05 13:05:11.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__init__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)     1956 2022-12-13 12:06:00.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__main__.py
+-rw-r--r--   0 damax     (1000) damax     (1000)    11783 2023-05-19 08:28:18.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/roller.py
+drwxr-xr-x   0 damax     (1000) damax     (1000)        0 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/
+-rw-r--r--   0 damax     (1000) damax     (1000)     4593 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/PKG-INFO
+-rw-r--r--   0 damax     (1000) damax     (1000)      399 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/SOURCES.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)        1 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/dependency_links.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       80 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/entry_points.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       12 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/requires.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       23 2023-05-19 08:31:05.000000 arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/top_level.txt
+-rw-r--r--   0 damax     (1000) damax     (1000)       38 2023-05-19 08:31:05.150281 arithmetic-dice-roller-0.3.0/setup.cfg
+-rw-r--r--   0 damax     (1000) damax     (1000)     1712 2023-05-19 08:29:08.000000 arithmetic-dice-roller-0.3.0/setup.py
```

### Comparing `arithmetic-dice-roller-0.2.4/PKG-INFO` & `arithmetic-dice-roller-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.2.4
+Version: 0.3.0
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
 [![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3100/)
```

### Comparing `arithmetic-dice-roller-0.2.4/README.md` & `arithmetic-dice-roller-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/__main__.py` & `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/__main__.py`

 * *Files identical despite different names*

### Comparing `arithmetic-dice-roller-0.2.4/arithmetic_dice_roller/roller.py` & `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller/roller.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,55 +132,55 @@
         Parse dice substrings following the syntax and roll them.
         :param expression: the expression to parse
         :return: tuple of the expression with evaluated rolls and the list of rolls
         """
         # Find all the dice substrings that follow dice syntax
         dice_groups = self.__dice_regex.findall(expression)
         rolls = []
-        for dice_groups in dice_groups:
+        for dice_group in dice_groups:
             # Parse number and type of dice
-            dice_amount = 1 if not dice_groups[1] else int(dice_groups[1])
+            dice_amount = 1 if not dice_group[1] else int(dice_group[1])
             is_fudge = False
-            match dice_groups[2].lower():
+            match dice_group[2].lower():
                 # Fudge
                 case 'f':
                     dice_type = range(-1, 2)
                     is_fudge = True
                 # Percentage
                 case '%':
                     dice_type = range(1, 101)
                 # All the others
                 case _:
-                    dice_type = range(1, int(dice_groups[2]) + 1)
+                    dice_type = range(1, int(dice_group[2]) + 1)
             # Operators that need to check each roll after it has been evaluated
-            if dice_groups[3] in ['R', 'r', '!']:
-                comparison_operator = self.__comparison_operators[dice_groups[4]]
-                if not dice_groups[5]:
-                    if dice_groups[3] == '!':
+            if dice_group[3] in ['R', 'r', '!']:
+                comparison_operator = self.__comparison_operators[dice_group[4]]
+                if not dice_group[5]:
+                    if dice_group[3] == '!':
                         comparison_value = 4 if is_fudge else dice_type.stop - 1
                     else:
                         comparison_value = -4 if is_fudge else 1
                 else:
-                    comparison_value = int(dice_groups[5])
+                    comparison_value = int(dice_group[5])
                 rolls.append(self.__reroll(dice_amount, dice_type, is_fudge,
-                                           dice_groups[3], comparison_operator, comparison_value))
+                                           dice_group[3], comparison_operator, comparison_value))
             else:
                 # In all the other cases all the rolls are immediately evaluated
                 results = []
                 if is_fudge:
                     rolls.append([0, [[0, random_choices(dice_type, k=4)] for _ in range(0, dice_amount)]])
                     for i, roll in enumerate(rolls[-1][1]):
                         results.append(sum(roll[1]))
                         rolls[-1][1][i][0] = results[-1]
                 else:
                     rolls.append([0, random_choices(dice_type, k=dice_amount)])
                     results = rolls[-1][1]
                 # Operators that modify the result after having evaluated all the rolls
-                keep_drop_amount = 1 if not dice_groups[5] else int(dice_groups[5])
-                match dice_groups[3]:
+                keep_drop_amount = 1 if not dice_group[5] else int(dice_group[5])
+                match dice_group[3]:
                     # Keep highest
                     case 'K':
                         rolls[-1][0] = sum(nlargest(keep_drop_amount, results))
                     # Keep lowest
                     case 'k':
                         rolls[-1][0] = sum(nsmallest(keep_drop_amount, results))
                     # Drop highest
@@ -188,26 +188,26 @@
                         rolls[-1][0] = sum(nsmallest(dice_amount - keep_drop_amount, results))
                     # Drop lowest
                     case 'x':
                         rolls[-1][0] = sum(nlargest(dice_amount - keep_drop_amount, results))
                     # Successes/failures or none
                     case _:
                         # Count successes?
-                        if dice_groups[6]:
-                            comparison_operator = self.__comparison_operators[dice_groups[6]]
-                            rolls[-1][0] = sum(map(lambda r: comparison_operator(r, int(dice_groups[7])), results))
+                        if dice_group[6]:
+                            comparison_operator = self.__comparison_operators[dice_group[6]]
+                            rolls[-1][0] = sum(map(lambda r: comparison_operator(r, int(dice_group[7])), results))
                             # Count failures?
-                            if dice_groups[8]:
-                                comparison_operator = self.__comparison_operators[dice_groups[8]]
-                                rolls[-1][0] -= sum(map(lambda r: comparison_operator(r, int(dice_groups[9])), results))
+                            if dice_group[8]:
+                                comparison_operator = self.__comparison_operators[dice_group[8]]
+                                rolls[-1][0] -= sum(map(lambda r: comparison_operator(r, int(dice_group[9])), results))
                                 if rolls[-1][0] < 0:
                                     rolls[-1][0] = 0
                         else:
                             rolls[-1][0] = sum(results)
-            rolls[-1].insert(0, dice_groups[0])
+            rolls[-1].insert(0, dice_group[0])
         return self.__dice_regex.sub('{}', expression).format(*[roll[1] for roll in rolls]), rolls
 
     @staticmethod
     def __reroll(dice_amount, dice_type, is_fudge, dice_operator, comparison_operator, comparison_value):
         """
         Roll with operators that need to check each single result.
         :param dice_amount: the amount of dice to roll
```

### Comparing `arithmetic-dice-roller-0.2.4/arithmetic_dice_roller.egg-info/PKG-INFO` & `arithmetic-dice-roller-0.3.0/arithmetic_dice_roller.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arithmetic-dice-roller
-Version: 0.2.4
+Version: 0.3.0
 Summary: A handy dice roller with extended notation and arithmetic expressions management.
 Home-page: https://github.com/massimopavoni/arithmetic-dice-roller
 Author: Massimo Pavoni
 Author-email: maspavoni@gmail.com
 Platform: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # arithmetic-dice-roller
 [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/massimopavoni/arithmetic-dice-roller?include_prereleases)](https://github.com/massimopavoni/arithmetic-dice-roller/releases)
 [![PyPI Package](https://img.shields.io/pypi/v/arithmetic-dice-roller)](https://pypi.org/project/arithmetic-dice-roller/)
 [![GitHub License](https://img.shields.io/github/license/massimopavoni/arithmetic-dice-roller)](https://github.com/massimopavoni/arithmetic-dice-roller/blob/main/LICENSE)
 [![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/massimopavoni/arithmetic-dice-roller)](https://www.python.org/downloads/release/python-3100/)
```

### Comparing `arithmetic-dice-roller-0.2.4/setup.py` & `arithmetic-dice-roller-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from setuptools import setup, find_packages
 
 README = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='arithmetic-dice-roller',
-    version='0.2.4',
+    version='0.3.0',
     description="A handy dice roller with extended notation and arithmetic expressions management.",
     long_description=README,
     long_description_content_type="text/markdown",
     author='Massimo Pavoni',
     author_email='maspavoni@gmail.com',
     url='https://github.com/massimopavoni/arithmetic-dice-roller',
     license_files='LICENSE',
@@ -36,15 +36,15 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Operating System :: OS Independent"
     ],
     platforms=['OS Independent'],
     packages=find_packages(),
     include_package_data=True,
-    python_requires='>=3.10',
-    install_requires=['sympy>=1.11'],
+    python_requires='>=3.11',
+    install_requires=['sympy>=1.12'],
     entry_points={
         'console_scripts': [
             'arithmetic-dice-roller=arithmetic_dice_roller.__main__:main'
         ]
     }
 )
```

