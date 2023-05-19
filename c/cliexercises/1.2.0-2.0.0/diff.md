# Comparing `tmp/cliexercises-1.2.0.tar.gz` & `tmp/cliexercises-2.0.0.tar.gz`

## Comparing `cliexercises-1.2.0.tar` & `cliexercises-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,45 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/__init__.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/app_guide.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/cli_exercises.css
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/cli_exercises.py
--rw-r--r--   0        0        0    13766 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/questions.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/user_progress.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/anchors.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/blocks.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/colors.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/duplicates.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/file_size.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/fruits.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/greeting.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/ip.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/nums_1.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/nums_2.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/purchases.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/range.txt
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/table.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/timings.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/varying_fields.csv
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 cliexercises-1.2.0/LICENSE
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 cliexercises-1.2.0/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 cliexercises-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cliexercises-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/app_guide.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/cli_exercises.css
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/cli_exercises.py
+-rw-r--r--   0        0        0    27383 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/questions.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/user_progress.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/.hidden
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/anchors.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/blocks.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/c1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/c2.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/code.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/colors.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/duplicates.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/file_size.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/fruits.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/fun.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/greeting.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/hex.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/ip.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/lines.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/multi_empty_lines.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/names.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/nums_1.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/nums_2.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/purchases.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/range.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/replace.txt
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/scores.csv
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/shopping_feb.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/shopping_jan.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/table.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/timings.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/twos.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/varying_fields.csv
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/backups/color list.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/backups/dot_files/.bash_aliases
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/backups/dot_files/.inputrc
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cliexercises-2.0.0/src/cliexercises/sample_input/backups/text/ip.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 cliexercises-2.0.0/LICENSE
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 cliexercises-2.0.0/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cliexercises-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cliexercises-2.0.0/PKG-INFO
```

### Comparing `cliexercises-1.2.0/src/cliexercises/app_guide.md` & `cliexercises-2.0.0/src/cliexercises/app_guide.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Linux CLI Text Processing Exercises
 
-This TUI application includes 40 questions to test your CLI text processing skills. These problems have been adapted from my [Computing from the Command Line](https://github.com/learnbyexample/cli-computing) ebook.
+This TUI application includes 60+ questions to test your CLI text processing skills. These problems have been adapted from my [Command Line](https://learnbyexample.github.io/books/) ebooks.
 
 ### Input command box
 
 You can type the command in the input box and press the **Enter** key to execute. For example, `grep 'sky' ip.txt` to display lines containing `sky` from the `ip.txt` file.
 
 `/bin/sh` is the shell interpreting the commands (`subprocess` module's default setting). So, features like `echo {1..3}` (brace expansion) and `grep $'\t' file.txt` (ANSI-C quoting) won't work.
 
@@ -60,11 +60,11 @@
 
 If you close the application and open it again, the first unsolved question will be displayed (i.e. already solved questions are skipped).
 
 Using **Ctrl+s** *won't* trigger the save logic — you'll have to type and execute the command to be considered for saving the changes.
 
 Once you have solved a question, only a different correct solution can override the previously saved command.
 
-### Computing from the Command Line
+### Ebooks
 
-The exercise questions in this app have been adapted from my ebook: [https://github.com/learnbyexample/cli-computing](https://github.com/learnbyexample/cli-computing)
+The exercise questions in this app have been adapted from my CLI ebooks: [https://learnbyexample.github.io/books/](https://learnbyexample.github.io/books/)
```

### Comparing `cliexercises-1.2.0/src/cliexercises/cli_exercises.css` & `cliexercises-2.0.0/src/cliexercises/cli_exercises.css`

 * *Files identical despite different names*

### Comparing `cliexercises-1.2.0/src/cliexercises/cli_exercises.py` & `cliexercises-2.0.0/src/cliexercises/cli_exercises.py`

 * *Files identical despite different names*

### Comparing `cliexercises-1.2.0/LICENSE` & `cliexercises-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliexercises-1.2.0/README.md` & `cliexercises-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Linux CLI Text Processing Exercises
 
-This TUI application includes 40 questions to test your CLI text processing skills.
+This TUI application includes 60+ questions to test your CLI text processing skills.
 
 > **Note:** This application is intended for exercises based on Linux CLI tools. You might still be able to solve the exercises on other platforms, but I'm not sure if it works.
 
 # Screenshot
 
 ![Sample question](https://raw.githubusercontent.com/learnbyexample/TUI-apps/main/CLI-Exercises/cli_exercises.png)
```

### Comparing `cliexercises-1.2.0/pyproject.toml` & `cliexercises-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "cliexercises"
-version = "1.2.0"
+version = "2.0.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
-description = "40 beginner to intermediate level questions on CLI text processing tasks"
+description = "60+ beginner to intermediate level questions on CLI text processing tasks"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `cliexercises-1.2.0/PKG-INFO` & `cliexercises-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cliexercises
-Version: 1.2.0
-Summary: 40 beginner to intermediate level questions on CLI text processing tasks
+Version: 2.0.0
+Summary: 60+ beginner to intermediate level questions on CLI text processing tasks
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/CLI-Exercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: textual>=0.24.1
 Description-Content-Type: text/markdown
 
 # Linux CLI Text Processing Exercises
 
-This TUI application includes 40 questions to test your CLI text processing skills.
+This TUI application includes 60+ questions to test your CLI text processing skills.
 
 > **Note:** This application is intended for exercises based on Linux CLI tools. You might still be able to solve the exercises on other platforms, but I'm not sure if it works.
 
 # Screenshot
 
 ![Sample question](https://raw.githubusercontent.com/learnbyexample/TUI-apps/main/CLI-Exercises/cli_exercises.png)
```

