# Comparing `tmp/SAPsim-1.0.9.tar.gz` & `tmp/SAPsim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.9.tar", last modified: Tue May  9 11:21:29 2023, max compression
+gzip compressed data, was "SAPsim-1.1.0.tar", last modified: Fri May 19 17:09:16 2023, max compression
```

## Comparing `SAPsim-1.0.9.tar` & `SAPsim-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:29.818066 SAPsim-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 11:21:21.000000 SAPsim-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-09 11:21:29.818066 SAPsim-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-09 11:21:21.000000 SAPsim-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:29.814066 SAPsim-1.0.9/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:29.814066 SAPsim-1.0.9/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-09 11:21:21.000000 SAPsim-1.0.9/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:29.814066 SAPsim-1.0.9/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-09 11:21:29.000000 SAPsim-1.0.9/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-09 11:21:29.000000 SAPsim-1.0.9/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:21:29.000000 SAPsim-1.0.9/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 11:21:29.000000 SAPsim-1.0.9/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 11:21:29.000000 SAPsim-1.0.9/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-09 11:21:21.000000 SAPsim-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:21:29.818066 SAPsim-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-09 11:21:21.000000 SAPsim-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:29.818066 SAPsim-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/test_SAPsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-09 11:21:21.000000 SAPsim-1.0.9/tests/test_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:16.431325 SAPsim-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 17:09:07.000000 SAPsim-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-19 17:09:16.431325 SAPsim-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-19 17:09:07.000000 SAPsim-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:16.431325 SAPsim-1.1.0/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:16.431325 SAPsim-1.1.0/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-19 17:09:07.000000 SAPsim-1.1.0/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:16.431325 SAPsim-1.1.0/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-19 17:09:16.000000 SAPsim-1.1.0/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-19 17:09:16.000000 SAPsim-1.1.0/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:09:16.000000 SAPsim-1.1.0/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 17:09:16.000000 SAPsim-1.1.0/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 17:09:16.000000 SAPsim-1.1.0/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-19 17:09:07.000000 SAPsim-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:09:16.431325 SAPsim-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 17:09:07.000000 SAPsim-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:16.431325 SAPsim-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/test_SAPsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-19 17:09:07.000000 SAPsim-1.1.0/tests/test_instructions.py
```

### Comparing `SAPsim-1.0.9/LICENSE` & `SAPsim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim/__init__.py` & `SAPsim-1.1.0/SAPsim/__init__.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim/utils/exceptions.py` & `SAPsim-1.1.0/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim/utils/execute.py` & `SAPsim-1.1.0/SAPsim/utils/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,43 +86,50 @@
             * *non_blocking* (``bool``) --
                 * This is used to unit test debug mode of ``run()``, you likely don't have a need for this
                 * If ``True``, then ``run()`` won't block on input
                 * ``input()`` won't be called in debug mode (i.e., don't have to press enter to continue execution)
                 * If this is ``True``, then debug mode will be on even if ``debug`` isn't in kwargs
             * *no_print* (``bool``) --
                 * This is used to save computation time during unit testing
-                * If ``True``, then ``print()`` won't be called, except for error messages
+                * If ``True``, then ``print_RAM()`` and ``print_info()`` won't be called
+                * In debug mode, "Program halted." will still be printed
             * *bits* (``int``) --
-                * Number of bits in unsigned registers
+                * You probably don't have a need for this
+                * Number of bits in registers
                 * Default value in ``global_vars`` is 8
                 * 8 is also the maximum value since everything in RAM should fit in a byte
 
     :return: ``None`` or program state if ``return_state``
     :rtype: ``Union[None, dict[str, Any]]``
     """
     if not isinstance(prog_path, str):
         raise TypeError("Required parameter prog_path must be a str.")
-    if "debug" in kwargs and not isinstance(kwargs["debug"], bool):
-        raise TypeError("Keyword argument debug must be a bool.")
+    debug: bool = False
+    if "debug" in kwargs:
+        if not isinstance(kwargs["debug"], bool):
+            raise TypeError("Keyword argument debug must be a bool.")
+        debug = kwargs["debug"]
     # Not initializing it causes some syntax warnings but better than initializing it
     change: dict[int, int]
     if "change" in kwargs:
         change = kwargs["change"]
         if not isinstance(change, dict):
             raise TypeError("Keyword argument change must be a dict[int, int].")
         if not all(isinstance(key, int) for key in change.keys()) or not all(
             isinstance(value, int) for value in change.values()
         ):
             raise TypeError("Keyword argument change must be a dict[int, int].")
     if "table_format" in kwargs and not isinstance(kwargs["table_format"], str):
         raise TypeError("Keyword argument table_format must be a str.")
     if "return_state" in kwargs and not isinstance(kwargs["return_state"], bool):
         raise TypeError("Keyword argument return_state must be a bool.")
-    if "non_blocking" in kwargs and not isinstance(kwargs["non_blocking"], bool):
-        raise TypeError("Keyword argument non_blocking must be a bool.")
+    if "non_blocking" in kwargs:
+        if not isinstance(kwargs["non_blocking"], bool):
+            raise TypeError("Keyword argument non_blocking must be a bool.")
+        debug = True
     if "no_print" in kwargs and not isinstance(kwargs["no_print"], bool):
         raise TypeError("Keyword argument no_print must be a bool.")
     if "bits" in kwargs and not isinstance(kwargs["bits"], int):
         raise TypeError("Keyword argument bits must be an int.")
 
     path: Path = Path(prog_path)
     if not path.suffix == ".csv":
@@ -151,15 +158,15 @@
         if unmapped_addrs_changed:
             print(
                 f"WARNING: You attempted to change the following address(es) not mapped in the CSV: {', '.join(list(map(str, unmapped_addrs_changed)))}.\nThis is likely unintentional, but they are now mapped, and the program will continue.",
                 file=sys.stderr,
             )
     if "table_format" in kwargs:
         global_vars.table_format = kwargs["table_format"]
-    if kwargs.get("debug") or kwargs.get("non_blocking"):
+    if debug:
         if not kwargs.get("no_print"):
             print(f"Initial state of simulation of {prog_path}")
             helpers.print_RAM()
             helpers.print_info()
             print("Debug mode: press Enter to execute next instruction ( > ).")
         if not kwargs.get("non_blocking"):
             input()
@@ -179,15 +186,14 @@
                 input()
         print("Program halted.")
     else:
         execute_full_speed()
         if not kwargs.get("no_print"):
             helpers.print_RAM()
             helpers.print_info()
-            print("Program halted.")
 
     if kwargs.get("return_state"):
         return helpers.get_state()
 
 
 @is_documented_by(
     run,
```

### Comparing `SAPsim-1.0.9/SAPsim/utils/global_vars.py` & `SAPsim-1.1.0/SAPsim/utils/global_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 If changing anything in this file, also modify ``SAPsim/__init__.py`` and ``helpers.print_info``."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from bidict import bidict
 
-RAM = {}
+RAM: dict[int, int] = {}
 """``dict[int, int]`` mapping ``PC``:``byte``, where ``byte`` can be instruction or data (indistinguishable, mostly)"""
 PC: int = 0
 """Program counter that indexes into ``RAM``, default value 0"""
 A: int = 0
 """Register A, default value 0"""
 B: int = 0
 """Register B, default value 0"""
@@ -46,16 +46,16 @@
         "JC": 7,
         "JZ": 8,
         "OUT": 14,
         "HLT": 15,
     }
 )
 
-"""Bidirectional dictionary mapping ``str mnemonic : int opcode``.
+"""Bidirectional mapping ``str mnemonic : int opcode``.
 
 Use ``MNEMONIC_TO_OPCODE.inverse[opcode]`` to get mnemonic from opcode.
 
 All mnemonics in this dict are in all caps."""
 
 table_format: str = "simple_outline"
-"""Tabulate ``table_fmt`` arg to customize pretty-printing. Defaults to ``simple_outline``, see all options: https://github.com/astanin/python-tabulate#table-
-                        format"""
+"""Tabulate ``table_fmt`` kwarg to customize pretty-printing. Defaults to ``simple_outline``,
+see all options: https://github.com/astanin/python-tabulate#table-format"""
```

### Comparing `SAPsim-1.0.9/SAPsim/utils/helpers.py` & `SAPsim-1.1.0/SAPsim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim/utils/instructions.py` & `SAPsim-1.1.0/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim/utils/parser.py` & `SAPsim-1.1.0/SAPsim/utils/parser.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.1.0/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/pyproject.toml` & `SAPsim-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "SAPsim"
 authors = [
     { name="Jesse Wei", email="jesse@cs.unc.edu" },
 ]
 description = "Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
```

### Comparing `SAPsim-1.0.9/setup.py` & `SAPsim-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Check https://pypi.org/project/SAPsim/ for latest version number
-    version="1.0.9",
+    version="1.1.0",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.9/tests/test_SAPsim.py` & `SAPsim-1.1.0/tests/test_SAPsim.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/tests/test_example_progs.py` & `SAPsim-1.1.0/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/tests/test_exceptions.py` & `SAPsim-1.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/tests/test_helpers.py` & `SAPsim-1.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.9/tests/test_instructions.py` & `SAPsim-1.1.0/tests/test_instructions.py`

 * *Files identical despite different names*

