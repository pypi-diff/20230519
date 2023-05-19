# Comparing `tmp/etdd-0.0.2.tar.gz` & `tmp/etdd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etdd-0.0.2.tar", last modified: Fri May 12 19:48:17 2023, max compression
+gzip compressed data, was "etdd-0.0.5.tar", last modified: Fri May 12 20:21:16 2023, max compression
```

## Comparing `etdd-0.0.2.tar` & `etdd-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.133427 etdd-0.0.2/
--rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 11:06:48.129529 etdd-0.0.2/PKG-INFO
--rwxr-xr-x   0 user      (1000)     1001        3 2023-05-19 08:37:42.000000 etdd-0.0.2/README.md
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.025036 etdd-0.0.2/etdd/
--rwxr-xr-x   0 user      (1000)     1001       27 2023-05-02 08:16:07.000000 etdd-0.0.2/etdd/__init__.py
--rwxr-xr-x   0 user      (1000)     1001    14882 2023-05-19 11:04:47.000000 etdd-0.0.2/etdd/core.py
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.109018 etdd-0.0.2/etdd.egg-info/
--rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/PKG-INFO
--rwxr-xr-x   0 user      (1000)     1001      187 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/SOURCES.txt
--rwxr-xr-x   0 user      (1000)     1001        1 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/dependency_links.txt
--rwxr-xr-x   0 user      (1000)     1001       67 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/requires.txt
--rwxr-xr-x   0 user      (1000)     1001        5 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/top_level.txt
--rwxr-xr-x   0 user      (1000)     1001       38 2023-05-19 11:06:48.134401 etdd-0.0.2/setup.cfg
--rwxr-xr-x   0 user      (1000)     1001      997 2023-05-19 11:06:17.000000 etdd-0.0.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:21:16.952452 etdd-0.0.5/
+-rw-r--r--   0 user      (1000) user      (1000)      613 2023-05-12 20:21:16.952452 etdd-0.0.5/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)        3 2023-05-12 20:15:11.000000 etdd-0.0.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:21:16.952452 etdd-0.0.5/etdd/
+-rwxr-xr-x   0 user      (1000) user      (1000)       27 2023-05-12 20:15:11.000000 etdd-0.0.5/etdd/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    15624 2023-05-12 20:18:20.000000 etdd-0.0.5/etdd/core.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-12 20:21:16.952452 etdd-0.0.5/etdd.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      613 2023-05-12 20:21:16.000000 etdd-0.0.5/etdd.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      187 2023-05-12 20:21:16.000000 etdd-0.0.5/etdd.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-12 20:21:16.000000 etdd-0.0.5/etdd.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-05-12 20:21:16.000000 etdd-0.0.5/etdd.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2023-05-12 20:21:16.000000 etdd-0.0.5/etdd.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-12 20:21:16.952452 etdd-0.0.5/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      997 2023-05-12 20:21:06.000000 etdd-0.0.5/setup.py
```

### Comparing `etdd-0.0.2/PKG-INFO` & `etdd-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.2
+Version: 0.0.5
 Summary: extend TDD framework
 Home-page: UNKNOWN
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Description: Opa
 Platform: UNKNOWN
```

### Comparing `etdd-0.0.2/etdd/core.py` & `etdd-0.0.5/etdd/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,15 +185,31 @@
         self.tests.append(test)
         if cmakelists != "":
             test.templates["cmakelists"] = cmakelists
         if main != "":
             test.templates["main"] = main
         return test
 
+    def info(self):
+        bash_exec(self.project, "where cmake")
+        bash_exec(self.project, "where gcc")
+        bash_exec(self.project, "where g++")
+        bash_exec(self.project, "where mingw32-make")
+        bash_exec(self.project, "where git")
+        bash_exec(self.project, "where doxygen")
+        bash_exec(self.project, "where lizard")
+        bash_exec(self.project, "where gcovr")
+        bash_exec(self.project, "where dot")
+        pause()
+
     def doxygen(self):
+        print("opa")
+        doxygen_file = self.project / "Doxyfile"
+        if not doxygen_file.exists():
+            bash_exec(self.project, "doxygen -g")    
         bash_exec(self.project, "doxygen")
         pause()
 
     def installCPPUTest(self, version="v4.0"):
         tmp_path = self.project / "tmp";
         os.makedirs(tmp_path, exist_ok=True)
         cpputest_path = tmp_path / "cpputest"
@@ -201,24 +217,25 @@
             print("Downloading and compiling the CPPUTest in {}".format(tmp_path))
             bash_exec_check(tmp_path, "git clone --depth 1 https://github.com/cpputest/cpputest".format(version))
 
         build_path = cpputest_path / "build-mingw" 
         install_path_abs = Path(tmp_path/"cpputest_mingw").resolve()
         os.makedirs(build_path, exist_ok=True)
         bash_exec_check(build_path, 'cmake -G "MinGW Makefiles" -DCMAKE_INSTALL_PREFIX={} ..'.format(install_path_abs))
-        bash_exec_check(build_path, "make")
-        bash_exec_check(build_path, "make install")
+        bash_exec_check(build_path, "mingw32-make")
+        bash_exec_check(build_path, "mingw32-make install")
         pause()
 
     def menu(self):
         menu = ConsoleMenu("eTDD is C++ unit test framework. (%s)" % ("opa"),
                             "Choose test packag/es variant.", show_exit_option=False)
         menu.append_item( ExitItem("Auf wiedersehen!!", menu=None, menu_char='q') )
-        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.installCPPUTest, [], menu_char='i') )
+        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.installCPPUTest, [], menu_char='c') )
         menu.append_item( FunctionItem("Documentation", self.doxygen, [], menu_char='d') )
+        menu.append_item( FunctionItem("Information", self.info, [], menu_char='i') )
 
         count = 1
         for test in self.tests:
             menu.append_item( FunctionItem(test.name, test.run_in_loop, [], menu_char=str(count))  )
             count += 1
         menu.show()
 
@@ -367,17 +384,17 @@
 
     def configure(self):
         os.makedirs(self.build, exist_ok=True)
         bash_exec_check(self.build, 'cmake -G "{}" ..'.format(self.tdd.makefile))
 
     def make(self, debug=False):
         if debug:
-            bash_exec_check(self.build, 'make VERBOSE=1')
+            bash_exec_check(self.build, 'mingw32-make VERBOSE=1')
         else:
-            bash_exec_check(self.build, 'make')
+            bash_exec_check(self.build, 'mingw32-make')
 
     def exec(self):
         if os.name == 'nt':
             bash_exec_check(self.build, 'TestApp')
         else:
             bash_exec_check(self.build, './TestApp')
```

### Comparing `etdd-0.0.2/etdd.egg-info/PKG-INFO` & `etdd-0.0.5/etdd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.2
+Version: 0.0.5
 Summary: extend TDD framework
 Home-page: UNKNOWN
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Description: Opa
 Platform: UNKNOWN
```

### Comparing `etdd-0.0.2/setup.py` & `etdd-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='etdd',
-    version='0.0.2',
+    version='0.0.5',
     description='extend TDD framework',
     packages=['etdd'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

