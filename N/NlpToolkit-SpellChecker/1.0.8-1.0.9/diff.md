# Comparing `tmp/NlpToolkit-SpellChecker-1.0.8.tar.gz` & `tmp/NlpToolkit-SpellChecker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-SpellChecker-1.0.8.tar", last modified: Wed Mar 18 13:20:11 2020, max compression
+gzip compressed data, was "dist/NlpToolkit-SpellChecker-1.0.9.tar", last modified: Thu Apr  9 19:08:31 2020, max compression
```

## Comparing `NlpToolkit-SpellChecker-1.0.8.tar` & `NlpToolkit-SpellChecker-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/
--rw-r--r--   0 olcay      (501) staff       (20)      284 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)      375 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/SOURCES.txt
--rw-r--r--   0 olcay      (501) staff       (20)        1 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/dependency_links.txt
--rw-r--r--   0 olcay      (501) staff       (20)       50 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/requires.txt
--rw-r--r--   0 olcay      (501) staff       (20)       13 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/NlpToolkit_SpellChecker.egg-info/top_level.txt
--rw-r--r--   0 olcay      (501) staff       (20)      284 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     3328 2020-03-18 13:19:56.000000 NlpToolkit-SpellChecker-1.0.8/README.md
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/SpellChecker/
--rw-r--r--   0 olcay      (501) staff       (20)     3546 2020-03-18 13:18:26.000000 NlpToolkit-SpellChecker-1.0.8/SpellChecker/NGramSpellChecker.py
--rw-r--r--   0 olcay      (501) staff       (20)     5456 2020-03-18 13:16:48.000000 NlpToolkit-SpellChecker-1.0.8/SpellChecker/SimpleSpellChecker.py
--rw-r--r--   0 olcay      (501) staff       (20)      452 2020-02-17 18:38:08.000000 NlpToolkit-SpellChecker-1.0.8/SpellChecker/SpellChecker.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-15 11:11:08.000000 NlpToolkit-SpellChecker-1.0.8/SpellChecker/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)       38 2020-03-18 13:20:11.000000 NlpToolkit-SpellChecker-1.0.8/setup.cfg
--rw-r--r--   0 olcay      (501) staff       (20)      404 2020-03-18 13:14:03.000000 NlpToolkit-SpellChecker-1.0.8/setup.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)      284 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)      375 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       50 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       13 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/NlpToolkit_SpellChecker.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)      284 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     3328 2020-03-18 13:19:56.000000 NlpToolkit-SpellChecker-1.0.9/README.md
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/SpellChecker/
+-rw-r--r--   0 olcay      (501) staff       (20)     3561 2020-04-09 19:07:48.000000 NlpToolkit-SpellChecker-1.0.9/SpellChecker/NGramSpellChecker.py
+-rw-r--r--   0 olcay      (501) staff       (20)     5456 2020-03-18 13:16:48.000000 NlpToolkit-SpellChecker-1.0.9/SpellChecker/SimpleSpellChecker.py
+-rw-r--r--   0 olcay      (501) staff       (20)      452 2020-02-17 18:38:08.000000 NlpToolkit-SpellChecker-1.0.9/SpellChecker/SpellChecker.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-15 11:11:08.000000 NlpToolkit-SpellChecker-1.0.9/SpellChecker/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2020-04-09 19:08:31.000000 NlpToolkit-SpellChecker-1.0.9/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)      404 2020-04-09 19:07:57.000000 NlpToolkit-SpellChecker-1.0.9/setup.py
```

### Comparing `NlpToolkit-SpellChecker-1.0.8/README.md` & `NlpToolkit-SpellChecker-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-1.0.8/SpellChecker/NGramSpellChecker.py` & `NlpToolkit-SpellChecker-1.0.9/SpellChecker/NGramSpellChecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,9 +73,9 @@
                         bestCandidate = candidate
                         bestRoot = root
                         bestProbability = probability
                 previousRoot = bestRoot
                 result.addWord(Word(bestCandidate))
             else:
                 result.addWord(word)
-                previousRoot = fsmParses.getFsmParse(0).getWord()
+                previousRoot = fsmParses.getParseWithLongestRootWord().getWord()
         return result
```

### Comparing `NlpToolkit-SpellChecker-1.0.8/SpellChecker/SimpleSpellChecker.py` & `NlpToolkit-SpellChecker-1.0.9/SpellChecker/SimpleSpellChecker.py`

 * *Files identical despite different names*

