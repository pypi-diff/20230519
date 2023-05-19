# Comparing `tmp/etdd-0.0.1.tar.gz` & `tmp/etdd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etdd-0.0.1.tar", last modified: Fri May 12 17:24:01 2023, max compression
+gzip compressed data, was "etdd-0.0.2.tar", last modified: Fri May 12 19:48:17 2023, max compression
```

## Comparing `etdd-0.0.1.tar` & `etdd-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 08:42:32.112244 etdd-0.0.1/
--rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 08:42:32.108337 etdd-0.0.1/PKG-INFO
--rwxr-xr-x   0 user      (1000)     1001        3 2023-05-19 08:37:42.000000 etdd-0.0.1/README.md
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 08:42:31.979867 etdd-0.0.1/etdd/
--rwxr-xr-x   0 user      (1000)     1001       27 2023-05-02 08:16:07.000000 etdd-0.0.1/etdd/__init__.py
--rwxr-xr-x   0 user      (1000)     1001    14695 2023-05-19 08:35:55.000000 etdd-0.0.1/etdd/core.py
-drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 08:42:32.091736 etdd-0.0.1/etdd.egg-info/
--rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 08:42:31.000000 etdd-0.0.1/etdd.egg-info/PKG-INFO
--rwxr-xr-x   0 user      (1000)     1001      187 2023-05-19 08:42:31.000000 etdd-0.0.1/etdd.egg-info/SOURCES.txt
--rwxr-xr-x   0 user      (1000)     1001        1 2023-05-19 08:42:31.000000 etdd-0.0.1/etdd.egg-info/dependency_links.txt
--rwxr-xr-x   0 user      (1000)     1001       62 2023-05-19 08:42:31.000000 etdd-0.0.1/etdd.egg-info/requires.txt
--rwxr-xr-x   0 user      (1000)     1001        5 2023-05-19 08:42:31.000000 etdd-0.0.1/etdd.egg-info/top_level.txt
--rwxr-xr-x   0 user      (1000)     1001       38 2023-05-19 08:42:32.113218 etdd-0.0.1/setup.cfg
--rwxr-xr-x   0 user      (1000)     1001      979 2023-05-19 08:41:39.000000 etdd-0.0.1/setup.py
+drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.133427 etdd-0.0.2/
+-rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 11:06:48.129529 etdd-0.0.2/PKG-INFO
+-rwxr-xr-x   0 user      (1000)     1001        3 2023-05-19 08:37:42.000000 etdd-0.0.2/README.md
+drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.025036 etdd-0.0.2/etdd/
+-rwxr-xr-x   0 user      (1000)     1001       27 2023-05-02 08:16:07.000000 etdd-0.0.2/etdd/__init__.py
+-rwxr-xr-x   0 user      (1000)     1001    14882 2023-05-19 11:04:47.000000 etdd-0.0.2/etdd/core.py
+drwxr-xr-x   0 user      (1000)     1001        0 2023-05-19 11:06:48.109018 etdd-0.0.2/etdd.egg-info/
+-rwxr-xr-x   0 user      (1000)     1001      613 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/PKG-INFO
+-rwxr-xr-x   0 user      (1000)     1001      187 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/SOURCES.txt
+-rwxr-xr-x   0 user      (1000)     1001        1 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/dependency_links.txt
+-rwxr-xr-x   0 user      (1000)     1001       67 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/requires.txt
+-rwxr-xr-x   0 user      (1000)     1001        5 2023-05-19 11:06:47.000000 etdd-0.0.2/etdd.egg-info/top_level.txt
+-rwxr-xr-x   0 user      (1000)     1001       38 2023-05-19 11:06:48.134401 etdd-0.0.2/setup.cfg
+-rwxr-xr-x   0 user      (1000)     1001      997 2023-05-19 11:06:17.000000 etdd-0.0.2/setup.py
```

### Comparing `etdd-0.0.1/PKG-INFO` & `etdd-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.1
+Version: 0.0.2
 Summary: extend TDD framework
 Home-page: UNKNOWN
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Description: Opa
 Platform: UNKNOWN
```

### Comparing `etdd-0.0.1/etdd/core.py` & `etdd-0.0.2/etdd/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,430 +1,446 @@
-# =======================================================================================
-#  Header
-# =======================================================================================
-
-import os
-import jinja2
-import shutil
-import re
-import time
-from pathlib import Path
-from consolemenu import ConsoleMenu
-from consolemenu.items import ExitItem
-from consolemenu.items import FunctionItem
-import readchar
-import threading
-
-# =======================================================================================
-#  Templates
-# =======================================================================================
-
-std_cmake_template = """project({{name}})
-cmake_minimum_required(VERSION 3.00)
-
-SET(PROJECT_DIR {{project_dir}})
-SET(CPPCHECK_LIB "${PROJECT_DIR}/tmp/cpputest_mingw")
-
-{% for var_name,var_value in cmake.items() -%}
-SET({{var_name}} "{{var_value}}")
-{% endfor %}
-
-add_executable(TestApp
-    {% for file in sut_code -%}
-        {{file}}        
-    {% endfor %}
-    {{code}}
-	main.cpp
-	)
-
-include_directories(
-    ${CMAKE_SOURCE_DIR}
-    {% for dir in includes -%}
-        ${PROJECT_DIR}/{{dir}}
-    {% endfor %}
-	${CPPCHECK_LIB}/include
-    )
-
-{% if os_name == 'nt' %}
-    find_library(testlib NAMES CppUTest PATHS ${CPPCHECK_LIB}/lib/)
-    find_library(testlibext NAMES CppUTestExt PATHS ${CPPCHECK_LIB}/lib/)
-    target_link_libraries(TestApp ${testlib} ${testlibext})
-{% else %}
-    target_link_libraries(TestApp CppUTest CppUTestExt)
-{% endif %}
-"""
-
-std_main_template = """
-#include "CppUTest/CommandLineTestRunner.h"
-#include "CppUTest/TestPlugin.h"
-#include "CppUTest/TestRegistry.h"
-#include "CppUTestExt/IEEE754ExceptionsPlugin.h"
-#include "CppUTestExt/MockSupportPlugin.h"
-
-int main(int ac, char** av)
-{
-    return CommandLineTestRunner::RunAllTests(ac, av);
-}
-"""
-
-main_template22 = """
-#include "CppUTest/CommandLineTestRunner.h"
-#include "CppUTest/TestPlugin.h"
-#include "CppUTest/TestRegistry.h"
-#include "CppUTestExt/IEEE754ExceptionsPlugin.h"
-#include "CppUTestExt/MockSupportPlugin.h"
-
-class MyDummyComparator : public MockNamedValueComparator
-{
-public:
-    virtual bool isEqual(const void* object1, const void* object2)
-    {
-        return object1 == object2;
-    }
-
-    virtual SimpleString valueToString(const void* object)
-    {
-        return StringFrom(object);
-    }
-};
-
-int main(int ac, char** av)
-{
-    MyDummyComparator dummyComparator;
-    MockSupportPlugin mockPlugin;
-    IEEE754ExceptionsPlugin ieee754Plugin;
-
-    mockPlugin.installComparator("MyDummyType", dummyComparator);
-    TestRegistry::getCurrentRegistry()->installPlugin(&mockPlugin);
-    TestRegistry::getCurrentRegistry()->installPlugin(&ieee754Plugin);
-    return CommandLineTestRunner::RunAllTests(ac, av);
-}
-"""
-
-# =======================================================================================
-#  Functions
-# =======================================================================================
-
-def interrupt(signum, frame):
-    print("aqui")
-    raise Exception("")
-
-def bash_exec(root, cmd):
-    saved_path = os.getcwd()
-    os.chdir(root)
-    print(cmd)
-    os.system(cmd)
-    os.chdir(saved_path)
-
-def bash_exec_check(root, cmd):
-    saved_path = os.getcwd()
-    os.chdir(root)
-    print(cmd)
-    error = os.system(cmd)
-    if error != 0:
-        os.chdir(saved_path)
-        raise(Exception("Error in {}".format(cmd)))
-    os.chdir(saved_path)
-
-def pause():
-    if os.name == 'nt':
-        os.system("pause")
-    else:
-        input('Press <ENTER> to continue')
-
-# =======================================================================================
-#  KeyboardThread
-# =======================================================================================
-
-class KeyboardThread(threading.Thread):
-    b_keyPressed: bool
-
-    def __init__(self):
-        threading.Thread.__init__(self, name="KeyPressThread")
-        self.b_keyPressed = False
-        self.start()
-
-    def run(self):
-        while(True):
-            int_key = readchar.readchar()
-            print("KeyPress -> Finishing threads.")
-            break
-
-        self.b_keyPressed = True
-        pass
-
-    def isAnyKeyPressed(self):
-        return(self.b_keyPressed)
-
-# =======================================================================================
-#  TDD
-# =======================================================================================
-
-class TDD:
-    def __init__(self, cmakelists=std_cmake_template, main=std_main_template):
-        std_gcc_flags = "-g -O0 -coverage -lgcov " # keep one space after the flags
-
-        self.project = Path(".")
-        self.tests = []
-        self.includes = []
-        self.cmake = {"CMAKE_C_FLAGS": std_gcc_flags, "CMAKE_CXX_FLAGS": std_gcc_flags}
-        self.templates = {"cmakelists": cmakelists, "main": main}
-        self.run_test_func = None
-        if os.name == 'nt':
-            self.makefile = "MinGW Makefiles"
-        else:
-            self.makefile = "Unix Makefiles"
-    
-    def test(self, test_file, cmakelists="", main=""):
-        test = Test(test_file, self)
-        self.tests.append(test)
-        if cmakelists != "":
-            test.templates["cmakelists"] = cmakelists
-        if main != "":
-            test.templates["main"] = main
-        return test
-
-    def doxygen(self):
-        bash_exec(self.project, "doxygen")
-        pause()
-
-    def installCPPUTest(self, version="v4.0"):
-        tmp_path = self.project / "tmp";
-        os.makedirs(tmp_path, exist_ok=True)
-        cpputest_path = tmp_path / "cpputest"
-        if not cpputest_path.exists():
-            print("Downloading and compiling the CPPUTest in {}".format(tmp_path))
-            bash_exec_check(tmp_path, "git clone --depth 1 https://github.com/cpputest/cpputest".format(version))
-
-        build_path = cpputest_path / "build-mingw" 
-        install_path_abs = Path(tmp_path/"cpputest_mingw").resolve()
-        os.makedirs(build_path, exist_ok=True)
-        bash_exec_check(build_path, 'cmake -G "MinGW Makefiles" -DCMAKE_INSTALL_PREFIX={} ..'.format(install_path_abs))
-        bash_exec_check(build_path, "make")
-        bash_exec_check(build_path, "make install")
-        pause()
-
-    def menu(self):
-        menu = ConsoleMenu("eTDD is C++ unit test framework. (%s)" % ("opa"),
-                            "Choose test packag/es variant.", show_exit_option=False)
-        menu.append_item( ExitItem("Auf wiedersehen!!", menu=None, menu_char='q') )
-        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.installCPPUTest, [], menu_char='i') )
-        menu.append_item( FunctionItem("Documentation", self.doxygen, [], menu_char='d') )
-
-        count = 1
-        for test in self.tests:
-            menu.append_item( FunctionItem(test.name, test.run_in_loop, [], menu_char=str(count))  )
-            count += 1
-        menu.show()
-
-    def download_from_git(self, repo):
-        name = Path(repo).stem
-        project_path = Path(".") / name
-        if not project_path.exists():
-            bash_exec_check(self.project, "git clone {}".format(repo))
-
-    def run_test(self, func):
-        self.run_test_func = func
-
-# =======================================================================================
-#  Test
-# =======================================================================================
-
-class Test:
-    def __init__(self, test_file: str, tdd: TDD):
-        self.name = Path(test_file).stem
-        self.code = test_file
-        self.sut = []
-        self.files = []
-        self.home = Path("tmp") / self.name
-        self.build = self.home / "build"
-        self.tdd = tdd
-        self.cmake = self.tdd.cmake.copy()
-        self.includes = []
-        self.gentest_count = 0
-        self.templates = {}
-        self.__timestamp = {}
-
-    def __get_template(self, template_name) -> str:
-        if template_name in self.templates:
-            return self.templates[template_name]
-        if template_name in self.tdd.templates:
-            return self.tdd.templates[template_name]
-        raise( Exception("template {} not found".format(template_name)) )
-
-    def __copy_files_from_project(self, list: []):
-        # Copy the files
-        project_path = Path(self.tdd.project)
-        for file in list:
-            print("copying the file {}".format(file))
-            filename = Path(file).name
-            shutil.copyfile( project_path / file, self.home / filename )
-            self.__timestamp[file] = os.path.getmtime(file)
-
-    def set_SUT(self, list_files, put_to_compile=True):
-        self.sut = list_files
-
-    def generate(self, template_text, filename, **data):
-        rtemplate = jinja2.Environment().from_string(template_text)
-        rendered = rtemplate.render(**data)
-        with open(self.home / filename, "w") as fd:
-            fd.write(rendered)
-
-    def generate_test_from(self, code_file):
-        with open(code_file, "r") as fd:
-            text = fd.read()
-
-        # find blocks defined by /** <multi line text> */
-        group_list = re.findall("/\*\*([\S\s]*?)\*/", text)
-        for group in group_list:
-            tests = re.findall("@test (.*)", group)
-            for test in tests:
-                self.gentest_count += 1
-                test_code = "TEST(klog, test_{}) {{\n".format(self.gentest_count)
-                test_code += test
-                test_code += "\n}"
-
-    def split_code(self, code_file) -> [str]:
-        with open(code_file, "r") as fd:
-            text = fd.read()
-
-        # find blocks like /** @code <path/filename> <code> */
-        group_list = re.findall("/\*\*[ ]*@code ([a-zA-Z_][a-zA-Z0-9_./]+)([\S\s/]*?)\*/", text)
-
-        # save each block in a new file
-        retval = []
-        for group in group_list:
-            filename = group[0]
-
-            # case there is a path before the file name
-            filename_path = Path(filename)
-            if len(filename_path.parents) > 1:
-                os.makedirs(self.home/filename_path.parent, exist_ok=True)
-
-            # create the file
-            code = group[1]
-            with open(self.home / filename, "w") as fd:
-                print("generating from {} file {}".format(code_file.name, filename))
-                fd.write(code)
-            # Put the new file in the vector to compile
-            file_suffix = Path(filename).suffix
-            retval.append(filename)
-
-        # return list of filenames created. Example ["file1.h", "file2.c", ...]
-        return retval
-
-    def copy(self):
-        code_name = Path(self.code).name
-        project_path = Path(self.tdd.project)
-        test_sut_code = []
-
-        # Create test directory and generate the main.cpp
-        tmp_test_main_path = self.home / Path(self.code).name
-        os.makedirs(self.home, exist_ok=True)
-        main_template = self.__get_template("main")
-        self.generate(main_template, "main.cpp")
-        shutil.copyfile( project_path / self.code, tmp_test_main_path)
-
-        # split files defined inside the test code
-        gen_files = self.split_code(tmp_test_main_path)
-        for filename in gen_files:
-            file_suffix = Path(filename).suffix
-            if file_suffix == '.c' or file_suffix == '.cpp':
-                test_sut_code.append(filename)
-
-        # Copy the SUT files
-        self.__copy_files_from_project(self.sut);
-
-        # Copy the other files
-        self.__copy_files_from_project(self.files);
-
-        # Merge the includes directories from TDD and Test
-        includes = []
-        includes += self.tdd.includes
-        includes += self.includes
-
-        # Merge the test and TDD cmake variables
-        # cmake = self.tdd.cmake.copy()
-        # cmake.update(self.cmake)
-
-        # Generate the CMakelists.txt
-        cmake_template = self.__get_template("cmakelists")
-        project_dir = str(self.tdd.project.resolve()).replace("\\","\\\\")
-        self.generate(cmake_template, "CMakeLists.txt", name=self.name, project_dir=project_dir, code=code_name, sut_code=test_sut_code, os_name=os.name, includes=includes, cmake=self.cmake)
-
-    def configure(self):
-        os.makedirs(self.build, exist_ok=True)
-        bash_exec_check(self.build, 'cmake -G "{}" ..'.format(self.tdd.makefile))
-
-    def make(self, debug=False):
-        if debug:
-            bash_exec_check(self.build, 'make VERBOSE=1')
-        else:
-            bash_exec_check(self.build, 'make')
-
-    def exec(self):
-        if os.name == 'nt':
-            bash_exec_check(self.build, 'TestApp')
-        else:
-            bash_exec_check(self.build, './TestApp')
-
-    def cppcheck(self):
-        # cppcheck
-        pass
-
-    def clean(self):
-        bash_exec(self.build, "make clean")
-
-    def coverage(self):
-        """
-            # gcovr --object-directory CMakeFiles\TestApp.dir\mingw_tmp_single -r ..\mingw_tmp_single\ -f "\.\./mingw_tmp_single/Calculator.cpp" -b --txt cov_vypis.txt --html cov\cov_html.html --html-details cov\coverage_details.html
-        """
-        bash_exec(self.home, 'gcovr')
-
-    def complexity(self):
-        files = []
-        for file in self.sut:
-            files.append( Path(file).name )
-        files_str = ' '.join(files)
-        bash_exec(self.home, "lizard {}".format(files_str))
-
-    def run(self):
-        if self.tdd.run_test_func != None:           
-            self.tdd.run_test_func(self)
-            self.clean()
-        else:
-            self.copy()
-            self.cppcheck()
-            self.configure()
-            self.make()
-            self.exec()
-            self.coverage()
-            self.clean()
-
-    def run_in_loop(self):
-        keyboard = KeyboardThread()
-        while(True):
-            # Run the Test
-            self.run()
-
-            # Check changes on files or keyboard event
-            while(True):
-                if self.is_changed_files():
-                    break;
-                if keyboard.isAnyKeyPressed():
-                    return 0
-                time.sleep(1)
-
-    def is_changed_files(self):
-        for file,time in self.__timestamp.items():
-            new_time = os.path.getmtime(file)
-            if ( new_time > time ):
-                print(file, time, new_time)
-                return True
-        return False
-
-    def pause(self):
-        if os.name == 'nt':
-            os.system("pause")
-        else:
-            input('Press <ENTER> to continue')
-
+# =======================================================================================
+#  Header
+# =======================================================================================
+
+import os
+import jinja2
+import shutil
+import re
+import time
+import glob
+import readchar
+import threading
+from pathlib import Path
+from consolemenu import ConsoleMenu
+from consolemenu.items import ExitItem
+from consolemenu.items import FunctionItem
+from colorama import Fore, Style
+
+# =======================================================================================
+#  Templates
+# =======================================================================================
+
+std_cmake_template = """project({{name}})
+cmake_minimum_required(VERSION 3.00)
+
+SET(PROJECT_DIR {{project_dir}})
+SET(CPPCHECK_LIB "${PROJECT_DIR}/tmp/cpputest_mingw")
+
+{% for var_name,var_value in cmake.items() -%}
+SET({{var_name}} "{{var_value}}")
+{% endfor %}
+
+add_executable(TestApp
+    {% for file in compile -%}
+    {{file}}        
+    {% endfor %}
+    {{code}}
+	main.cpp
+	)
+
+include_directories(
+    ${CMAKE_SOURCE_DIR}
+    {% for dir in includes -%}
+        ${PROJECT_DIR}/{{dir}}
+    {% endfor %}
+	${CPPCHECK_LIB}/include
+    )
+
+{% if os_name == 'nt' %}
+    find_library(testlib NAMES CppUTest PATHS ${CPPCHECK_LIB}/lib/)
+    find_library(testlibext NAMES CppUTestExt PATHS ${CPPCHECK_LIB}/lib/)
+    target_link_libraries(TestApp ${testlib} ${testlibext})
+{% else %}
+    target_link_libraries(TestApp CppUTest CppUTestExt)
+{% endif %}
+"""
+
+std_main_template = """
+#include "CppUTest/CommandLineTestRunner.h"
+#include "CppUTest/TestPlugin.h"
+#include "CppUTest/TestRegistry.h"
+#include "CppUTestExt/IEEE754ExceptionsPlugin.h"
+#include "CppUTestExt/MockSupportPlugin.h"
+
+int main(int ac, char** av)
+{
+    return CommandLineTestRunner::RunAllTests(ac, av);
+}
+"""
+
+main_template22 = """
+#include "CppUTest/CommandLineTestRunner.h"
+#include "CppUTest/TestPlugin.h"
+#include "CppUTest/TestRegistry.h"
+#include "CppUTestExt/IEEE754ExceptionsPlugin.h"
+#include "CppUTestExt/MockSupportPlugin.h"
+
+class MyDummyComparator : public MockNamedValueComparator
+{
+public:
+    virtual bool isEqual(const void* object1, const void* object2)
+    {
+        return object1 == object2;
+    }
+
+    virtual SimpleString valueToString(const void* object)
+    {
+        return StringFrom(object);
+    }
+};
+
+int main(int ac, char** av)
+{
+    MyDummyComparator dummyComparator;
+    MockSupportPlugin mockPlugin;
+    IEEE754ExceptionsPlugin ieee754Plugin;
+
+    mockPlugin.installComparator("MyDummyType", dummyComparator);
+    TestRegistry::getCurrentRegistry()->installPlugin(&mockPlugin);
+    TestRegistry::getCurrentRegistry()->installPlugin(&ieee754Plugin);
+    return CommandLineTestRunner::RunAllTests(ac, av);
+}
+"""
+
+# =======================================================================================
+#  Functions
+# =======================================================================================
+
+def interrupt(signum, frame):
+    print("aqui")
+    raise Exception("")
+
+def bash_exec(root, cmd):
+    saved_path = os.getcwd()
+    os.chdir(root)
+    print(f"\n{Fore.YELLOW}# {cmd}{Style.RESET_ALL}")
+    os.system(cmd)
+    os.chdir(saved_path)
+
+def bash_exec_check(root, cmd):
+    saved_path = os.getcwd()
+    os.chdir(root)
+    print(f"\n{Fore.YELLOW}# {cmd}{Style.RESET_ALL}")
+    error = os.system(cmd)
+    if error != 0:
+        os.chdir(saved_path)
+        raise(Exception("Error in {}".format(cmd)))
+    os.chdir(saved_path)
+
+def pause():
+    if os.name == 'nt':
+        os.system("pause")
+    else:
+        input('Press <ENTER> to continue')
+
+# =======================================================================================
+#  KeyboardThread
+# =======================================================================================
+
+class KeyboardThread(threading.Thread):
+    b_keyPressed: bool
+
+    def __init__(self):
+        threading.Thread.__init__(self, name="KeyPressThread")
+        self.b_keyPressed = False
+        self.start()
+
+    def run(self):
+        while(True):
+            int_key = readchar.readchar()
+            print("KeyPress -> Finishing threads.")
+            break
+
+        self.b_keyPressed = True
+        pass
+
+    def isAnyKeyPressed(self):
+        return(self.b_keyPressed)
+
+# =======================================================================================
+#  TDD
+# =======================================================================================
+
+class TDD:
+    def __init__(self, cmakelists=std_cmake_template, main=std_main_template):
+        std_gcc_flags = "-g -O0 -coverage -lgcov " # keep one space after the flags
+
+        self.project = Path(".")
+        self.tests = []
+        self.includes = []
+        self.cmake = {"CMAKE_C_FLAGS": std_gcc_flags, "CMAKE_CXX_FLAGS": std_gcc_flags}
+        self.templates = {"cmakelists": cmakelists, "main": main}
+        self.run_test_func = None
+        if os.name == 'nt':
+            self.makefile = "MinGW Makefiles"
+        else:
+            self.makefile = "Unix Makefiles"
+    
+    def test(self, test_file, name="", cmakelists="", main=""):
+        test_name = name
+        if test_name == "":
+            test_name = Path(test_file).stem
+        
+        test = Test(test_file, self, test_name)
+        self.tests.append(test)
+        if cmakelists != "":
+            test.templates["cmakelists"] = cmakelists
+        if main != "":
+            test.templates["main"] = main
+        return test
+
+    def doxygen(self):
+        bash_exec(self.project, "doxygen")
+        pause()
+
+    def installCPPUTest(self, version="v4.0"):
+        tmp_path = self.project / "tmp";
+        os.makedirs(tmp_path, exist_ok=True)
+        cpputest_path = tmp_path / "cpputest"
+        if not cpputest_path.exists():
+            print("Downloading and compiling the CPPUTest in {}".format(tmp_path))
+            bash_exec_check(tmp_path, "git clone --depth 1 https://github.com/cpputest/cpputest".format(version))
+
+        build_path = cpputest_path / "build-mingw" 
+        install_path_abs = Path(tmp_path/"cpputest_mingw").resolve()
+        os.makedirs(build_path, exist_ok=True)
+        bash_exec_check(build_path, 'cmake -G "MinGW Makefiles" -DCMAKE_INSTALL_PREFIX={} ..'.format(install_path_abs))
+        bash_exec_check(build_path, "make")
+        bash_exec_check(build_path, "make install")
+        pause()
+
+    def menu(self):
+        menu = ConsoleMenu("eTDD is C++ unit test framework. (%s)" % ("opa"),
+                            "Choose test packag/es variant.", show_exit_option=False)
+        menu.append_item( ExitItem("Auf wiedersehen!!", menu=None, menu_char='q') )
+        menu.append_item( FunctionItem("Install CppUTest on ./tmp", self.installCPPUTest, [], menu_char='i') )
+        menu.append_item( FunctionItem("Documentation", self.doxygen, [], menu_char='d') )
+
+        count = 1
+        for test in self.tests:
+            menu.append_item( FunctionItem(test.name, test.run_in_loop, [], menu_char=str(count))  )
+            count += 1
+        menu.show()
+
+    def download_from_git(self, repo):
+        name = Path(repo).stem
+        project_path = Path(".") / name
+        if not project_path.exists():
+            bash_exec_check(self.project, "git clone {}".format(repo))
+
+    def run_test(self, func):
+        self.run_test_func = func
+
+# =======================================================================================
+#  Test
+# =======================================================================================
+
+class Test:
+    def __init__(self, test_file: str, tdd: TDD, name: str):
+        self.name = name
+        self.code = test_file
+        self.sut = []
+        self.files = []
+        self.home = Path("tmp") / self.name
+        self.build = self.home / "build"
+        self.tdd = tdd
+        self.cmake = self.tdd.cmake.copy()
+        self.includes = []
+        self.compile = []
+        self.gentest_count = 0
+        self.templates = {}
+        self.__timestamp = {}
+
+    def __get_template(self, template_name) -> str:
+        if template_name in self.templates:
+            return self.templates[template_name]
+        if template_name in self.tdd.templates:
+            return self.tdd.templates[template_name]
+        raise( Exception("template {} not found".format(template_name)) )
+
+    def __copy_files_from_project(self, list: []):
+        # Copy the files
+        project_path = Path(self.tdd.project)
+        for file in list:
+            if file.find("*") > 0:
+                test = str(project_path / file)
+                list_files = glob.glob(test)
+                self.__copy_files_from_project(list_files)
+            else:
+                print("copying the file {}".format(file))
+                filename = Path(file).name
+                shutil.copyfile( project_path / file, self.home / filename )
+                self.__timestamp[file] = os.path.getmtime(file)
+
+    def set_SUT(self, list_files, put_to_compile=True):
+        self.sut = list_files
+
+    def generate(self, template_text, filename, **data):
+        rtemplate = jinja2.Environment().from_string(template_text)
+        rendered = rtemplate.render(**data)
+        with open(self.home / filename, "w") as fd:
+            fd.write(rendered)
+
+    def generate_test_from(self, code_file):
+        with open(code_file, "r") as fd:
+            text = fd.read()
+
+        # find blocks defined by /** <multi line text> */
+        group_list = re.findall("/\*\*([\S\s]*?)\*/", text)
+        for group in group_list:
+            tests = re.findall("@test (.*)", group)
+            for test in tests:
+                self.gentest_count += 1
+                test_code = "TEST(klog, test_{}) {{\n".format(self.gentest_count)
+                test_code += test
+                test_code += "\n}"
+
+    def split_code(self, code_file) -> [str]:
+        with open(code_file, "r") as fd:
+            text = fd.read()
+
+        # find blocks like /** @code <path/filename> <code> */
+        group_list = re.findall("/\*\*[ ]*@code ([a-zA-Z_][a-zA-Z0-9_./]+)([\S\s/]*?)\*/", text)
+
+        # save each block in a new file
+        retval = []
+        for group in group_list:
+            filename = group[0]
+
+            # case there is a path before the file name
+            filename_path = Path(filename)
+            if len(filename_path.parents) > 1:
+                os.makedirs(self.home/filename_path.parent, exist_ok=True)
+
+            # create the file
+            code = group[1]
+            with open(self.home / filename, "w") as fd:
+                print("generating from {} file {}".format(code_file.name, filename))
+                fd.write(code)
+            # Put the new file in the vector to compile
+            file_suffix = Path(filename).suffix
+            retval.append(filename)
+
+        # return list of filenames created. Example ["file1.h", "file2.c", ...]
+        return retval
+
+    def copy(self):
+        print(f"\n{Fore.YELLOW}Copying the files {Style.RESET_ALL}")
+
+        code_name = Path(self.code).name
+        project_path = Path(self.tdd.project)
+        test_sut_code = []
+
+        # Create test directory and generate the main.cpp
+        tmp_test_main_path = self.home / Path(self.code).name
+        os.makedirs(self.home, exist_ok=True)
+        main_template = self.__get_template("main")
+        self.generate(main_template, "main.cpp")
+        shutil.copyfile( project_path / self.code, tmp_test_main_path)
+
+        # split files defined inside the test code
+        gen_files = self.split_code(tmp_test_main_path)
+        for filename in gen_files:
+            file_suffix = Path(filename).suffix
+            if file_suffix == '.c' or file_suffix == '.cpp':
+                test_sut_code.append(filename)
+
+        # Copy the SUT files
+        self.__copy_files_from_project(self.sut);
+
+        # Copy the other files
+        self.__copy_files_from_project(self.files);
+
+        # Merge the includes directories from TDD and Test
+        includes = []
+        includes += self.tdd.includes
+        includes += self.includes
+
+        # Merge the test and TDD cmake variables
+        # cmake = self.tdd.cmake.copy()
+        # cmake.update(self.cmake)
+
+        # Generate the CMakelists.txt
+        cmake_template = self.__get_template("cmakelists")
+        project_dir = str(self.tdd.project.resolve()).replace("\\","\\\\")
+        self.generate(cmake_template, "CMakeLists.txt", name=self.name, project_dir=project_dir, code=code_name, sut_code=test_sut_code, os_name=os.name, includes=includes, cmake=self.cmake, compile=self.compile)
+
+    def configure(self):
+        os.makedirs(self.build, exist_ok=True)
+        bash_exec_check(self.build, 'cmake -G "{}" ..'.format(self.tdd.makefile))
+
+    def make(self, debug=False):
+        if debug:
+            bash_exec_check(self.build, 'make VERBOSE=1')
+        else:
+            bash_exec_check(self.build, 'make')
+
+    def exec(self):
+        if os.name == 'nt':
+            bash_exec_check(self.build, 'TestApp')
+        else:
+            bash_exec_check(self.build, './TestApp')
+
+    def cppcheck(self):
+        # cppcheck
+        pass
+
+    def clean(self):
+        bash_exec(self.build, "make clean")
+
+    def coverage(self):
+        """
+            # gcovr --object-directory CMakeFiles\TestApp.dir\mingw_tmp_single -r ..\mingw_tmp_single\ -f "\.\./mingw_tmp_single/Calculator.cpp" -b --txt cov_vypis.txt --html cov\cov_html.html --html-details cov\coverage_details.html
+        """
+        bash_exec(self.home, 'gcovr')
+
+    def complexity(self):
+        files = []
+        for file in self.sut:
+            files.append( Path(file).name )
+        files_str = ' '.join(files)
+        bash_exec(self.home, "lizard {}".format(files_str))
+
+    def run(self):
+        if self.tdd.run_test_func != None:           
+            self.tdd.run_test_func(self)
+            self.clean()
+        else:
+            self.copy()
+            self.cppcheck()
+            self.configure()
+            self.make()
+            self.exec()
+            self.coverage()
+            self.clean()
+
+    def run_in_loop(self):
+        keyboard = KeyboardThread()
+        while(True):
+            # Run the Test
+            self.run()
+
+            # Check changes on files or keyboard event
+            while(True):
+                if self.is_changed_files():
+                    os.system('cls')
+                    break;
+                if keyboard.isAnyKeyPressed():
+                    return 0
+                time.sleep(1)
+
+    def is_changed_files(self):
+        for file,time in self.__timestamp.items():
+            new_time = os.path.getmtime(file)
+            if ( new_time > time ):
+                print(file, time, new_time)
+                return True
+        return False
+
+    def pause(self):
+        if os.name == 'nt':
+            os.system("pause")
+        else:
+            input('Press <ENTER> to continue')
+
+
```

### Comparing `etdd-0.0.1/etdd.egg-info/PKG-INFO` & `etdd-0.0.2/etdd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etdd
-Version: 0.0.1
+Version: 0.0.2
 Summary: extend TDD framework
 Home-page: UNKNOWN
 Author: Milan Neubert, Felipe Bombardelli
 Author-email: felipebombardelli@gmail.com
 License: UNKNOWN
 Description: Opa
 Platform: UNKNOWN
```

### Comparing `etdd-0.0.1/setup.py` & `etdd-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='etdd',
-    version='0.0.1',
+    version='0.0.2',
     description='extend TDD framework',
     packages=['etdd'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
@@ -26,9 +26,10 @@
         'pathlib'
         , 'jinja2'
         , 'colorama'
         , 'tabulate'
         , 'lizard'
         , 'console-menu' # 0.8.0
         , 'readchar'
+        , 'glob'
     ]
 )
```

