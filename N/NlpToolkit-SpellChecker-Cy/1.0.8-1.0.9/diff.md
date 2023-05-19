# Comparing `tmp/NlpToolkit-SpellChecker-Cy-1.0.8.tar.gz` & `tmp/NlpToolkit-SpellChecker-Cy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-SpellChecker-Cy-1.0.8.tar", last modified: Fri Sep 30 17:00:02 2022, max compression
+gzip compressed data, was "dist/NlpToolkit-SpellChecker-Cy-1.0.9.tar", last modified: Tue Oct 11 12:40:05 2022, max compression
```

## Comparing `NlpToolkit-SpellChecker-Cy-1.0.8.tar` & `NlpToolkit-SpellChecker-Cy-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/
--rw-r--r--   0 olcay      (501) staff       (20)    35149 2021-02-09 17:12:05.000000 NlpToolkit-SpellChecker-Cy-1.0.8/LICENSE
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/
--rw-r--r--   0 olcay      (501) staff       (20)     4005 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)      701 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/SOURCES.txt
--rw-r--r--   0 olcay      (501) staff       (20)        1 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/dependency_links.txt
--rw-r--r--   0 olcay      (501) staff       (20)       56 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/requires.txt
--rw-r--r--   0 olcay      (501) staff       (20)       13 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/top_level.txt
--rw-r--r--   0 olcay      (501) staff       (20)     4005 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     3665 2022-04-28 10:59:28.000000 NlpToolkit-SpellChecker-Cy-1.0.8/README.md
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/
--rw-r--r--   0 olcay      (501) staff       (20)   209951 2022-09-26 13:22:32.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/Candidate.c
--rw-r--r--   0 olcay      (501) staff       (20)      127 2022-09-26 11:26:39.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/Candidate.pxd
--rw-r--r--   0 olcay      (501) staff       (20)      306 2022-09-26 13:06:28.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/Candidate.pyx
--rw-r--r--   0 olcay      (501) staff       (20)   479986 2022-09-30 16:32:57.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.c
--rw-r--r--   0 olcay      (501) staff       (20)      602 2022-09-26 13:06:28.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.pxd
--rw-r--r--   0 olcay      (501) staff       (20)    10188 2022-09-30 16:27:40.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      292 2022-09-25 17:27:23.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/Operator.py
--rw-r--r--   0 olcay      (501) staff       (20)   660930 2022-09-30 16:32:57.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.c
--rw-r--r--   0 olcay      (501) staff       (20)     1197 2022-09-26 13:13:45.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.pxd
--rw-r--r--   0 olcay      (501) staff       (20)    14155 2022-09-30 16:21:11.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.pyx
--rw-r--r--   0 olcay      (501) staff       (20)   210961 2022-09-26 13:25:11.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SpellChecker.c
--rw-r--r--   0 olcay      (501) staff       (20)      121 2020-10-07 06:04:50.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SpellChecker.pxd
--rw-r--r--   0 olcay      (501) staff       (20)      364 2020-10-07 06:04:50.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SpellChecker.pyx
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-15 11:11:08.000000 NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)       38 2022-09-30 17:00:02.000000 NlpToolkit-SpellChecker-Cy-1.0.8/setup.cfg
--rw-r--r--   0 olcay      (501) staff       (20)      924 2022-09-30 16:59:19.000000 NlpToolkit-SpellChecker-Cy-1.0.8/setup.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/
+-rw-r--r--   0 olcay      (501) staff       (20)    35149 2021-02-09 17:12:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/LICENSE
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)     4005 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)      701 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       56 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       13 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)     4005 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     3665 2022-04-28 10:59:28.000000 NlpToolkit-SpellChecker-Cy-1.0.9/README.md
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/
+-rw-r--r--   0 olcay      (501) staff       (20)   209951 2022-09-26 13:22:32.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/Candidate.c
+-rw-r--r--   0 olcay      (501) staff       (20)      127 2022-09-26 11:26:39.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/Candidate.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)      306 2022-09-26 13:06:28.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/Candidate.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   477357 2022-10-11 12:39:17.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.c
+-rw-r--r--   0 olcay      (501) staff       (20)      602 2022-09-26 13:06:28.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)    10169 2022-10-11 12:39:16.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)      292 2022-09-25 17:27:23.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/Operator.py
+-rw-r--r--   0 olcay      (501) staff       (20)   653879 2022-09-30 18:21:33.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.c
+-rw-r--r--   0 olcay      (501) staff       (20)     1178 2022-09-30 18:21:08.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)    13908 2022-09-30 18:21:32.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   210961 2022-09-26 13:25:11.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SpellChecker.c
+-rw-r--r--   0 olcay      (501) staff       (20)      121 2020-10-07 06:04:50.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SpellChecker.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)      364 2020-10-07 06:04:50.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SpellChecker.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-15 11:11:08.000000 NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2022-10-11 12:40:05.000000 NlpToolkit-SpellChecker-Cy-1.0.9/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)      924 2022-10-11 12:40:01.000000 NlpToolkit-SpellChecker-Cy-1.0.9/setup.py
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/LICENSE` & `NlpToolkit-SpellChecker-Cy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/PKG-INFO` & `NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NlpToolkit-SpellChecker-Cy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Turkish Spell Checker Library
 Home-page: https://github.com/StarlangSoftware/TurkishSpellChecker-Cy
 Author: olcaytaner
 Author-email: olcay.yildiz@ozyegin.edu.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/NlpToolkit_SpellChecker_Cy.egg-info/SOURCES.txt` & `NlpToolkit-SpellChecker-Cy-1.0.9/NlpToolkit_SpellChecker_Cy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/PKG-INFO` & `NlpToolkit-SpellChecker-Cy-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NlpToolkit-SpellChecker-Cy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Turkish Spell Checker Library
 Home-page: https://github.com/StarlangSoftware/TurkishSpellChecker-Cy
 Author: olcaytaner
 Author-email: olcay.yildiz@ozyegin.edu.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/README.md` & `NlpToolkit-SpellChecker-Cy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/Candidate.c` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/Candidate.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.c` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.c`

 * *Files 1% similar despite different names*

```diff
@@ -1898,15 +1898,15 @@
   struct __pyx_vtabstruct_12SpellChecker_12SpellChecker_SpellChecker __pyx_base;
   PyObject *(*__pyx___generateCandidateList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*candidateList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedMisspellCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   int (*forcedBackwardMergeCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedForwardMergeCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedSplitCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
-  int (*forcedShortcutCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
+  int (*forcedShortcutCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   PyObject *(*loadDictionaries)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, int __pyx_skip_dispatch);
   PyObject *(*getCorrectForm)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*mergedCandidatesList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   PyObject *(*splitCandidatesList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   PyObject *(*getSplitPair)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_vtabptr_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker;
@@ -4334,23 +4334,23 @@
       __pyx_t_1 = 0;
 
       /* "SpellChecker/NGramSpellChecker.pyx":143
  *                 root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 1)
  *                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
  *                 i = i + 1             # <<<<<<<<<<<<<<
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  */
       __pyx_v_i = (__pyx_v_i + 1);
 
       /* "SpellChecker/NGramSpellChecker.pyx":144
  *                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
  *                 i = i + 1
  *                 continue             # <<<<<<<<<<<<<<
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
  */
       goto __pyx_L3_continue;
 
       /* "SpellChecker/NGramSpellChecker.pyx":138
  *                 i = i + 1
  *                 continue
@@ -4359,43 +4359,43 @@
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
  */
     }
 
     /* "SpellChecker/NGramSpellChecker.pyx":145
  *                 i = i + 1
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):             # <<<<<<<<<<<<<<
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):             # <<<<<<<<<<<<<<
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
  *                 root = next_root
  */
     __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->__pyx_base.forcedSplitCheck(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_word, __pyx_v_result, 0) != 0);
     if (!__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
       goto __pyx_L13_bool_binop_done;
     }
-    __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->__pyx_base.forcedShortcutCheck(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_word, __pyx_v_result, __pyx_v_previous_word, 0) != 0);
+    __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->__pyx_base.forcedShortcutCheck(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_word, __pyx_v_result, 0) != 0);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L13_bool_binop_done:;
     if (__pyx_t_5) {
 
       /* "SpellChecker/NGramSpellChecker.pyx":146
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)             # <<<<<<<<<<<<<<
  *                 root = next_root
  *                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
  */
       __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRootForWordAtIndex(__pyx_v_self, __pyx_v_result, (((struct __pyx_vtabstruct_6Corpus_8Sentence_Sentence *)__pyx_v_result->__pyx_vtab)->wordCount(__pyx_v_result, 0) - 1), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF_SET(__pyx_v_previous_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_1));
       __pyx_t_1 = 0;
 
       /* "SpellChecker/NGramSpellChecker.pyx":147
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
  *                 root = next_root             # <<<<<<<<<<<<<<
  *                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
  *                 i = i + 1
  */
       __Pyx_INCREF(((PyObject *)__pyx_v_next_root));
       __Pyx_DECREF_SET(__pyx_v_root, __pyx_v_next_root);
@@ -4429,15 +4429,15 @@
  *                 candidates = self.candidateList(word)
  */
       goto __pyx_L3_continue;
 
       /* "SpellChecker/NGramSpellChecker.pyx":145
  *                 i = i + 1
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):             # <<<<<<<<<<<<<<
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):             # <<<<<<<<<<<<<<
  *                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
  *                 root = next_root
  */
     }
 
     /* "SpellChecker/NGramSpellChecker.pyx":151
  *                 i = i + 1
@@ -4592,15 +4592,15 @@
         }
 
         /* "SpellChecker/NGramSpellChecker.pyx":160
  *                 for candidate in candidates:
  *                     if candidate.getOperator() == Operator.SPELL_CHECK or \
  *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:             # <<<<<<<<<<<<<<
  *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
  */
         __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_candidate->__pyx_base.__pyx_vtab)->getOperator(__pyx_v_candidate, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Operator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_MISSPELLED_REPLACE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
@@ -4622,16 +4622,16 @@
  */
         if (__pyx_t_6) {
 
           /* "SpellChecker/NGramSpellChecker.pyx":161
  *                     if candidate.getOperator() == Operator.SPELL_CHECK or \
  *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
  *                         root = self.checkAnalysisAndSetRoot(candidate.getName())             # <<<<<<<<<<<<<<
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
- *                             and previous_previous_word is not None:
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
+ *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
  */
           __pyx_t_4 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_candidate), 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF_SET(__pyx_v_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2));
@@ -4645,17 +4645,17 @@
  *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
  */
         }
 
         /* "SpellChecker/NGramSpellChecker.pyx":162
  *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
  *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \             # <<<<<<<<<<<<<<
- *                             and previous_previous_word is not None:
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:             # <<<<<<<<<<<<<<
  *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
+ *                         if previous_previous_word is not None:
  */
         __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_candidate->__pyx_base.__pyx_vtab)->getOperator(__pyx_v_candidate, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Operator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_BACKWARD_MERGE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
@@ -4666,231 +4666,193 @@
         __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         if (__pyx_t_5) {
         } else {
           __pyx_t_6 = __pyx_t_5;
           goto __pyx_L22_bool_binop_done;
         }
-
-        /* "SpellChecker/NGramSpellChecker.pyx":163
- *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
- *                             and previous_previous_word is not None:             # <<<<<<<<<<<<<<
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- */
         __pyx_t_5 = (((PyObject *)__pyx_v_previous_word) != Py_None);
-
-        /* "SpellChecker/NGramSpellChecker.pyx":162
- *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
- *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \             # <<<<<<<<<<<<<<
- *                             and previous_previous_word is not None:
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- */
         __pyx_t_10 = (__pyx_t_5 != 0);
-        if (__pyx_t_10) {
-        } else {
-          __pyx_t_6 = __pyx_t_10;
-          goto __pyx_L22_bool_binop_done;
-        }
-
-        /* "SpellChecker/NGramSpellChecker.pyx":163
- *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
- *                             and previous_previous_word is not None:             # <<<<<<<<<<<<<<
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- */
-        __pyx_t_10 = (((PyObject *)__pyx_v_previous_previous_word) != Py_None);
-        __pyx_t_5 = (__pyx_t_10 != 0);
-        __pyx_t_6 = __pyx_t_5;
+        __pyx_t_6 = __pyx_t_10;
         __pyx_L22_bool_binop_done:;
-
-        /* "SpellChecker/NGramSpellChecker.pyx":162
- *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
- *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \             # <<<<<<<<<<<<<<
- *                             and previous_previous_word is not None:
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- */
         if (__pyx_t_6) {
 
-          /* "SpellChecker/NGramSpellChecker.pyx":164
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
- *                             and previous_previous_word is not None:
+          /* "SpellChecker/NGramSpellChecker.pyx":163
+ *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
  *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())             # <<<<<<<<<<<<<<
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
+ *                         if previous_previous_word is not None:
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previous_word->__pyx_vtab)->getName(__pyx_v_previous_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previous_word->__pyx_vtab)->getName(__pyx_v_previous_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+          __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+          __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF_SET(__pyx_v_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_1));
           __pyx_t_1 = 0;
 
-          /* "SpellChecker/NGramSpellChecker.pyx":165
- *                             and previous_previous_word is not None:
+          /* "SpellChecker/NGramSpellChecker.pyx":164
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
+ *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
+ *                         if previous_previous_word is not None:             # <<<<<<<<<<<<<<
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
+ */
+          __pyx_t_6 = (((PyObject *)__pyx_v_previous_previous_word) != Py_None);
+          __pyx_t_10 = (__pyx_t_6 != 0);
+          if (__pyx_t_10) {
+
+            /* "SpellChecker/NGramSpellChecker.pyx":165
  *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())             # <<<<<<<<<<<<<<
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
- *                             and next_next_word is not None:
+ *                         if previous_previous_word is not None:
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())             # <<<<<<<<<<<<<<
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
+ *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
  */
-          __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previous_previous_word->__pyx_vtab)->getName(__pyx_v_previous_previous_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_1), 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __Pyx_DECREF_SET(__pyx_v_previous_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2));
-          __pyx_t_2 = 0;
+            __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previous_previous_word->__pyx_vtab)->getName(__pyx_v_previous_previous_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_1);
+            __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_1), 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+            __Pyx_DECREF_SET(__pyx_v_previous_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2));
+            __pyx_t_2 = 0;
+
+            /* "SpellChecker/NGramSpellChecker.pyx":164
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
+ *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
+ *                         if previous_previous_word is not None:             # <<<<<<<<<<<<<<
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
+ */
+          }
 
           /* "SpellChecker/NGramSpellChecker.pyx":162
  *                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
  *                         root = self.checkAnalysisAndSetRoot(candidate.getName())
- *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \             # <<<<<<<<<<<<<<
- *                             and previous_previous_word is not None:
+ *                     if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:             # <<<<<<<<<<<<<<
  *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
+ *                         if previous_previous_word is not None:
  */
         }
 
         /* "SpellChecker/NGramSpellChecker.pyx":166
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \             # <<<<<<<<<<<<<<
- *                             and next_next_word is not None:
+ *                         if previous_previous_word is not None:
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:             # <<<<<<<<<<<<<<
  *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
+ *                         if next_next_word is not None:
  */
         __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_candidate->__pyx_base.__pyx_vtab)->getOperator(__pyx_v_candidate, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FORWARD_MERGE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (__pyx_t_5) {
-        } else {
-          __pyx_t_6 = __pyx_t_5;
-          goto __pyx_L26_bool_binop_done;
-        }
-
-        /* "SpellChecker/NGramSpellChecker.pyx":167
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
- *                             and next_next_word is not None:             # <<<<<<<<<<<<<<
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
- */
-        __pyx_t_5 = (((PyObject *)__pyx_v_next_word) != Py_None);
-
-        /* "SpellChecker/NGramSpellChecker.pyx":166
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \             # <<<<<<<<<<<<<<
- *                             and next_next_word is not None:
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- */
-        __pyx_t_10 = (__pyx_t_5 != 0);
-        if (__pyx_t_10) {
+        if (__pyx_t_6) {
         } else {
-          __pyx_t_6 = __pyx_t_10;
+          __pyx_t_10 = __pyx_t_6;
           goto __pyx_L26_bool_binop_done;
         }
-
-        /* "SpellChecker/NGramSpellChecker.pyx":167
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
- *                             and next_next_word is not None:             # <<<<<<<<<<<<<<
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
- */
-        __pyx_t_10 = (((PyObject *)__pyx_v_next_next_word) != Py_None);
-        __pyx_t_5 = (__pyx_t_10 != 0);
-        __pyx_t_6 = __pyx_t_5;
+        __pyx_t_6 = (((PyObject *)__pyx_v_next_word) != Py_None);
+        __pyx_t_5 = (__pyx_t_6 != 0);
+        __pyx_t_10 = __pyx_t_5;
         __pyx_L26_bool_binop_done:;
+        if (__pyx_t_10) {
 
-        /* "SpellChecker/NGramSpellChecker.pyx":166
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \             # <<<<<<<<<<<<<<
- *                             and next_next_word is not None:
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- */
-        if (__pyx_t_6) {
-
-          /* "SpellChecker/NGramSpellChecker.pyx":168
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
- *                             and next_next_word is not None:
+          /* "SpellChecker/NGramSpellChecker.pyx":167
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
  *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())             # <<<<<<<<<<<<<<
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
- *                     if previous_root is not None:
+ *                         if next_next_word is not None:
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
  */
-          __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_next_word->__pyx_vtab)->getName(__pyx_v_next_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_next_word->__pyx_vtab)->getName(__pyx_v_next_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_4 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF_SET(__pyx_v_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_4));
           __pyx_t_4 = 0;
 
-          /* "SpellChecker/NGramSpellChecker.pyx":169
- *                             and next_next_word is not None:
+          /* "SpellChecker/NGramSpellChecker.pyx":168
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
  *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())             # <<<<<<<<<<<<<<
+ *                         if next_next_word is not None:             # <<<<<<<<<<<<<<
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                     if previous_root is not None:
+ */
+          __pyx_t_10 = (((PyObject *)__pyx_v_next_next_word) != Py_None);
+          __pyx_t_5 = (__pyx_t_10 != 0);
+          if (__pyx_t_5) {
+
+            /* "SpellChecker/NGramSpellChecker.pyx":169
+ *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
+ *                         if next_next_word is not None:
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())             # <<<<<<<<<<<<<<
  *                     if previous_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:
  */
-          __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_next_next_word->__pyx_vtab)->getName(__pyx_v_next_next_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_DECREF_SET(__pyx_v_next_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2));
-          __pyx_t_2 = 0;
+            __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_next_next_word->__pyx_vtab)->getName(__pyx_v_next_next_word, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            __Pyx_DECREF_SET(__pyx_v_next_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2));
+            __pyx_t_2 = 0;
+
+            /* "SpellChecker/NGramSpellChecker.pyx":168
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
+ *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
+ *                         if next_next_word is not None:             # <<<<<<<<<<<<<<
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                     if previous_root is not None:
+ */
+          }
 
           /* "SpellChecker/NGramSpellChecker.pyx":166
- *                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
- *                         previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
- *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \             # <<<<<<<<<<<<<<
- *                             and next_next_word is not None:
+ *                         if previous_previous_word is not None:
+ *                             previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+ *                     if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:             # <<<<<<<<<<<<<<
  *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
+ *                         if next_next_word is not None:
  */
         }
 
         /* "SpellChecker/NGramSpellChecker.pyx":170
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                         if next_next_word is not None:
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
  *                     if previous_root is not None:             # <<<<<<<<<<<<<<
  *                         if candidate.getOperator() == Operator.SPLIT:
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])
  */
-        __pyx_t_6 = (((PyObject *)__pyx_v_previous_root) != Py_None);
-        __pyx_t_5 = (__pyx_t_6 != 0);
-        if (__pyx_t_5) {
+        __pyx_t_5 = (((PyObject *)__pyx_v_previous_root) != Py_None);
+        __pyx_t_10 = (__pyx_t_5 != 0);
+        if (__pyx_t_10) {
 
           /* "SpellChecker/NGramSpellChecker.pyx":171
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
  *                     if previous_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:             # <<<<<<<<<<<<<<
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])
  *                         previous_probability = self.getProbability(previous_root.getName(), root.getName())
  */
           __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_candidate->__pyx_base.__pyx_vtab)->getOperator(__pyx_v_candidate, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
@@ -4898,17 +4860,17 @@
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_SPLIT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
+          __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (__pyx_t_5) {
+          if (__pyx_t_10) {
 
             /* "SpellChecker/NGramSpellChecker.pyx":172
  *                     if previous_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])             # <<<<<<<<<<<<<<
  *                         previous_probability = self.getProbability(previous_root.getName(), root.getName())
  *                     else:
@@ -4929,15 +4891,15 @@
             __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->checkAnalysisAndSetRoot(__pyx_v_self, ((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_DECREF_SET(__pyx_v_root, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_1));
             __pyx_t_1 = 0;
 
             /* "SpellChecker/NGramSpellChecker.pyx":171
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
  *                     if previous_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:             # <<<<<<<<<<<<<<
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])
  *                         previous_probability = self.getProbability(previous_root.getName(), root.getName())
  */
           }
 
@@ -4953,16 +4915,16 @@
           __pyx_t_4 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_root->__pyx_vtab)->getName(__pyx_v_root, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_v_previous_probability = ((struct __pyx_vtabstruct_12SpellChecker_17NGramSpellChecker_NGramSpellChecker *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_vtab)->getProbability(__pyx_v_self, ((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_4), 0);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
           /* "SpellChecker/NGramSpellChecker.pyx":170
- *                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
- *                         next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+ *                         if next_next_word is not None:
+ *                             next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
  *                     if previous_root is not None:             # <<<<<<<<<<<<<<
  *                         if candidate.getOperator() == Operator.SPLIT:
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])
  */
           goto __pyx_L29;
         }
 
@@ -4981,17 +4943,17 @@
         /* "SpellChecker/NGramSpellChecker.pyx":176
  *                     else:
  *                         previous_probability = 0.0
  *                     if next_root is not None:             # <<<<<<<<<<<<<<
  *                         if candidate.getOperator() == Operator.SPLIT:
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[1])
  */
-        __pyx_t_5 = (((PyObject *)__pyx_v_next_root) != Py_None);
-        __pyx_t_6 = (__pyx_t_5 != 0);
-        if (__pyx_t_6) {
+        __pyx_t_10 = (((PyObject *)__pyx_v_next_root) != Py_None);
+        __pyx_t_5 = (__pyx_t_10 != 0);
+        if (__pyx_t_5) {
 
           /* "SpellChecker/NGramSpellChecker.pyx":177
  *                         previous_probability = 0.0
  *                     if next_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:             # <<<<<<<<<<<<<<
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[1])
  *                         next_probability = self.getProbability(root.getName(), next_root.getName())
@@ -5002,17 +4964,17 @@
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SPLIT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (__pyx_t_6) {
+          if (__pyx_t_5) {
 
             /* "SpellChecker/NGramSpellChecker.pyx":178
  *                     if next_root is not None:
  *                         if candidate.getOperator() == Operator.SPLIT:
  *                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[1])             # <<<<<<<<<<<<<<
  *                         next_probability = self.getProbability(root.getName(), next_root.getName())
  *                     else:
@@ -5092,16 +5054,16 @@
         __pyx_t_11 = __pyx_v_next_probability;
         __pyx_t_12 = __pyx_v_previous_probability;
         if (((__pyx_t_11 > __pyx_t_12) != 0)) {
           __pyx_t_13 = __pyx_t_11;
         } else {
           __pyx_t_13 = __pyx_t_12;
         }
-        __pyx_t_6 = ((__pyx_t_13 > __pyx_v_best_probability) != 0);
-        if (__pyx_t_6) {
+        __pyx_t_5 = ((__pyx_t_13 > __pyx_v_best_probability) != 0);
+        if (__pyx_t_5) {
 
           /* "SpellChecker/NGramSpellChecker.pyx":183
  *                         next_probability = 0.0
  *                     if max(previous_probability, next_probability) > best_probability:
  *                         best_candidate = candidate             # <<<<<<<<<<<<<<
  *                         best_root = root
  *                         best_probability = max(previous_probability, next_probability)
@@ -5167,17 +5129,17 @@
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FORWARD_MERGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (__pyx_t_6) {
+      if (__pyx_t_5) {
 
         /* "SpellChecker/NGramSpellChecker.pyx":187
  *                         best_probability = max(previous_probability, next_probability)
  *                 if best_candidate.getOperator() == Operator.FORWARD_MERGE:
  *                     i = i + 1             # <<<<<<<<<<<<<<
  *                 if best_candidate.getName() == Operator.BACKWARD_MERGE:
  *                     result.replaceWord(i - 1, Word(best_candidate.getName()))
@@ -5203,18 +5165,18 @@
       __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_best_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_best_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BACKWARD_MERGE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_t_3, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_t_3, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
+      if (__pyx_t_5) {
 
         /* "SpellChecker/NGramSpellChecker.pyx":189
  *                     i = i + 1
  *                 if best_candidate.getName() == Operator.BACKWARD_MERGE:
  *                     result.replaceWord(i - 1, Word(best_candidate.getName()))             # <<<<<<<<<<<<<<
  *                 else:
  *                     if best_candidate.getName() == Operator.SPLIT:
@@ -5250,18 +5212,18 @@
         __pyx_t_3 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_best_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_best_candidate), 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SPLIT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_t_2, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_t_2, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (__pyx_t_6) {
+        if (__pyx_t_5) {
 
           /* "SpellChecker/NGramSpellChecker.pyx":192
  *                 else:
  *                     if best_candidate.getName() == Operator.SPLIT:
  *                         self.addSplitWords(best_candidate.getName(), result)             # <<<<<<<<<<<<<<
  *                     else:
  *                         result.addWord(Word(best_candidate.getName()))
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.pxd` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.pxd`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/NGramSpellChecker.pyx` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/NGramSpellChecker.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if self.forcedForwardMergeCheck(word, result, next_word):
                 i = i + 1
                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
                 root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 1)
                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
                 i = i + 1
                 continue
-            if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+            if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
                 previous_root = self.checkAnalysisAndSetRootForWordAtIndex(result, result.wordCount() - 1)
                 root = next_root
                 next_root = self.checkAnalysisAndSetRootForWordAtIndex(sentence, i + 2)
                 i = i + 1
                 continue
             if root is None:
                 candidates = self.candidateList(word)
@@ -155,22 +155,22 @@
                 best_candidate = Candidate(word.getName(), Operator.NO_CHANGE)
                 best_root = word
                 best_probability = self.__threshold
                 for candidate in candidates:
                     if candidate.getOperator() == Operator.SPELL_CHECK or \
                             candidate.getOperator() == Operator.MISSPELLED_REPLACE:
                         root = self.checkAnalysisAndSetRoot(candidate.getName())
-                    if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None \
-                            and previous_previous_word is not None:
+                    if candidate.getOperator() == Operator.BACKWARD_MERGE and previous_word is not None:
                         root = self.checkAnalysisAndSetRoot(previous_word.getName() + word.getName())
-                        previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
-                    if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None \
-                            and next_next_word is not None:
+                        if previous_previous_word is not None:
+                            previous_root = self.checkAnalysisAndSetRoot(previous_previous_word.getName())
+                    if candidate.getOperator() == Operator.FORWARD_MERGE and next_word is not None:
                         root = self.checkAnalysisAndSetRoot(word.getName() + next_word.getName())
-                        next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
+                        if next_next_word is not None:
+                            next_root = self.checkAnalysisAndSetRoot(next_next_word.getName())
                     if previous_root is not None:
                         if candidate.getOperator() == Operator.SPLIT:
                             root = self.checkAnalysisAndSetRoot(candidate.getName().split(" ")[0])
                         previous_probability = self.getProbability(previous_root.getName(), root.getName())
                     else:
                         previous_probability = 0.0
                     if next_root is not None:
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.c` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.c`

 * *Files 1% similar despite different names*

```diff
@@ -1699,15 +1699,15 @@
   struct __pyx_vtabstruct_12SpellChecker_12SpellChecker_SpellChecker __pyx_base;
   PyObject *(*__pyx___generateCandidateList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*candidateList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedMisspellCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   int (*forcedBackwardMergeCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedForwardMergeCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*forcedSplitCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
-  int (*forcedShortcutCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
+  int (*forcedShortcutCheck)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   PyObject *(*loadDictionaries)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, int __pyx_skip_dispatch);
   PyObject *(*getCorrectForm)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, PyObject *, int __pyx_skip_dispatch);
   PyObject *(*mergedCandidatesList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   PyObject *(*splitCandidatesList)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   PyObject *(*getSplitPair)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_vtabptr_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker;
@@ -2249,15 +2249,15 @@
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker___generateCandidateList(CYTHON_UNUSED struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, PyObject *__pyx_v_word, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_candidateList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, int __pyx_skip_dispatch); /* proto*/
 static struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_spellCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_sentence, int __pyx_skip_dispatch); /* proto*/
 static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedMisspellCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, int __pyx_skip_dispatch); /* proto*/
 static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedBackwardMergeCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord, int __pyx_skip_dispatch); /* proto*/
 static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedForwardMergeCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_nextWord, int __pyx_skip_dispatch); /* proto*/
 static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedSplitCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, int __pyx_skip_dispatch); /* proto*/
-static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord, int __pyx_skip_dispatch); /* proto*/
+static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_loadDictionaries(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getCorrectForm(CYTHON_UNUSED struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, PyObject *__pyx_v_wordName, PyObject *__pyx_v_dictionary, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_mergedCandidatesList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_nextWord, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_splitCandidatesList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getSplitPair(CYTHON_UNUSED struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from 'Dictionary.Word' */
@@ -2378,15 +2378,14 @@
 static const char __pyx_k_open[] = "open";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_utf8[] = "utf8";
 static const char __pyx_k_volt[] = "volt";
 static const char __pyx_k_watt[] = "watt";
 static const char __pyx_k_word[] = "word";
-static const char __pyx_k_0_9_2[] = "[0-9]+";
 static const char __pyx_k_SPLIT[] = "SPLIT";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_litre[] = "litre";
 static const char __pyx_k_metre[] = "metre";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_split[] = "split";
 static const char __pyx_k_strip[] = "strip";
@@ -2451,15 +2450,14 @@
 static const char __pyx_k_forcedForwardMergeCheck[] = "forcedForwardMergeCheck";
 static const char __pyx_k_forcedBackwardMergeCheck[] = "forcedBackwardMergeCheck";
 static const char __pyx_k_pyx_unpickle_SimpleSpellChecke[] = "__pyx_unpickle_SimpleSpellChecker";
 static const char __pyx_k_SpellChecker_SimpleSpellChecker[] = "SpellChecker.SimpleSpellChecker";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x16[] = "Incompatible checksums (%s vs 0x162cce2 = (__merged_words, __split_words, fsm))";
 static PyObject *__pyx_kp_u_;
 static PyObject *__pyx_kp_u_0_9;
-static PyObject *__pyx_kp_u_0_9_2;
 static PyObject *__pyx_n_s_BACKWARD_MERGE;
 static PyObject *__pyx_n_s_FORWARD_MERGE;
 static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x16;
 static PyObject *__pyx_n_s_LETTERS;
 static PyObject *__pyx_n_s_LOWERCASE_LETTERS;
 static PyObject *__pyx_n_s_MISSPELLED_REPLACE;
 static PyObject *__pyx_n_s_Operator;
@@ -2581,15 +2579,15 @@
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_4candidateList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_6spellCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_sentence); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_8forcedMisspellCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_10forcedBackwardMergeCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_12forcedForwardMergeCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_nextWord); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_14addSplitWords(CYTHON_UNUSED struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, PyObject *__pyx_v_multiWord, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_16forcedSplitCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result); /* proto */
-static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord); /* proto */
+static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_20loadDictionaries(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_22getCorrectForm(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, PyObject *__pyx_v_wordName, PyObject *__pyx_v_dictionary); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_24mergedCandidatesList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_nextWord); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_26splitCandidatesList(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_28getSplitPair(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_30__reduce_cython__(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_32__setstate_cython__(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
@@ -4013,23 +4011,23 @@
     if (__pyx_t_5) {
 
       /* "SpellChecker/SimpleSpellChecker.pyx":148
  *                 continue
  *             if self.forcedForwardMergeCheck(word, result, next_word):
  *                 i = i + 2             # <<<<<<<<<<<<<<
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  */
       __pyx_v_i = (__pyx_v_i + 2);
 
       /* "SpellChecker/SimpleSpellChecker.pyx":149
  *             if self.forcedForwardMergeCheck(word, result, next_word):
  *                 i = i + 2
  *                 continue             # <<<<<<<<<<<<<<
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 i = i + 1
  */
       goto __pyx_L3_continue;
 
       /* "SpellChecker/SimpleSpellChecker.pyx":147
  *                 i = i + 1
  *                 continue
@@ -4038,51 +4036,51 @@
  *                 continue
  */
     }
 
     /* "SpellChecker/SimpleSpellChecker.pyx":150
  *                 i = i + 2
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):             # <<<<<<<<<<<<<<
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):             # <<<<<<<<<<<<<<
  *                 i = i + 1
  *                 continue
  */
     __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self->__pyx_base.__pyx_vtab)->forcedSplitCheck(__pyx_v_self, __pyx_v_word, __pyx_v_result, 0) != 0);
     if (!__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
       goto __pyx_L12_bool_binop_done;
     }
-    __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self->__pyx_base.__pyx_vtab)->forcedShortcutCheck(__pyx_v_self, __pyx_v_word, __pyx_v_result, __pyx_v_previous_word, 0) != 0);
+    __pyx_t_6 = (((struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self->__pyx_base.__pyx_vtab)->forcedShortcutCheck(__pyx_v_self, __pyx_v_word, __pyx_v_result, 0) != 0);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_5) {
 
       /* "SpellChecker/SimpleSpellChecker.pyx":151
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 i = i + 1             # <<<<<<<<<<<<<<
  *                 continue
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(word.getName())
  */
       __pyx_v_i = (__pyx_v_i + 1);
 
       /* "SpellChecker/SimpleSpellChecker.pyx":152
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
  *                 i = i + 1
  *                 continue             # <<<<<<<<<<<<<<
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(word.getName())
  *             if fsm_parse_list.size() == 0:
  */
       goto __pyx_L3_continue;
 
       /* "SpellChecker/SimpleSpellChecker.pyx":150
  *                 i = i + 2
  *                 continue
- *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):             # <<<<<<<<<<<<<<
+ *             if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):             # <<<<<<<<<<<<<<
  *                 i = i + 1
  *                 continue
  */
     }
 
     /* "SpellChecker/SimpleSpellChecker.pyx":153
  *                 i = i + 1
@@ -6095,15 +6093,15 @@
   }
 
   /* "SpellChecker/SimpleSpellChecker.pyx":222
  *             self.addSplitWords(forced_replacement, result)
  *             return True
  *         return False             # <<<<<<<<<<<<<<
  * 
- *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result, Word previousWord):
+ *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
   /* "SpellChecker/SimpleSpellChecker.pyx":216
  *         result.addWord(Word(words[1]))
  * 
@@ -6222,21 +6220,21 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "SpellChecker/SimpleSpellChecker.pyx":224
  *         return False
  * 
- *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result, Word previousWord):             # <<<<<<<<<<<<<<
+ *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result):             # <<<<<<<<<<<<<<
  *         cdef str shortcut_regex, forced_replacement
  *         cdef int i
  */
 
 static PyObject *__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_19forcedShortcutCheck(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord, int __pyx_skip_dispatch) {
+static int __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, int __pyx_skip_dispatch) {
   PyObject *__pyx_v_shortcut_regex = 0;
   PyObject *__pyx_v_forced_replacement = 0;
   int __pyx_v_i;
   PyObject *__pyx_v_compiled_expression = NULL;
   PyObject *__pyx_v_pair = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -6245,16 +6243,14 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  int __pyx_t_10;
-  int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("forcedShortcutCheck", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
@@ -6278,43 +6274,40 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_3)) {
-          PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_result), ((PyObject *)__pyx_v_previousWord)};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+          PyObject *__pyx_temp[3] = {__pyx_t_4, ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_result)};
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-          PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_result), ((PyObject *)__pyx_v_previousWord)};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+          PyObject *__pyx_temp[3] = {__pyx_t_4, ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_result)};
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 224, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 224, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_4) {
             __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
           }
           __Pyx_INCREF(((PyObject *)__pyx_v_word));
           __Pyx_GIVEREF(((PyObject *)__pyx_v_word));
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, ((PyObject *)__pyx_v_word));
           __Pyx_INCREF(((PyObject *)__pyx_v_result));
           __Pyx_GIVEREF(((PyObject *)__pyx_v_result));
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, ((PyObject *)__pyx_v_result));
-          __Pyx_INCREF(((PyObject *)__pyx_v_previousWord));
-          __Pyx_GIVEREF(((PyObject *)__pyx_v_previousWord));
-          PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, ((PyObject *)__pyx_v_previousWord));
           __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -6370,15 +6363,15 @@
     __pyx_v_i = __pyx_t_5;
 
     /* "SpellChecker/SimpleSpellChecker.pyx":229
  *         shortcut_regex = "[0-9]+(" + self.__shortcuts[0]
  *         for i in range(1, len(self.__shortcuts)):
  *             shortcut_regex = shortcut_regex + "|" + self.__shortcuts[i]             # <<<<<<<<<<<<<<
  *         shortcut_regex = shortcut_regex + ")"
- *         compiled_expression = re.compile("[0-9]+")
+ *         compiled_expression = re.compile(shortcut_regex)
  */
     __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_shortcut_regex, __pyx_kp_u__3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_shortcuts); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -6392,28 +6385,28 @@
     __pyx_t_2 = 0;
   }
 
   /* "SpellChecker/SimpleSpellChecker.pyx":230
  *         for i in range(1, len(self.__shortcuts)):
  *             shortcut_regex = shortcut_regex + "|" + self.__shortcuts[i]
  *         shortcut_regex = shortcut_regex + ")"             # <<<<<<<<<<<<<<
- *         compiled_expression = re.compile("[0-9]+")
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):
+ *         compiled_expression = re.compile(shortcut_regex)
+ *         if compiled_expression.fullmatch(word.getName()):
  */
   __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_shortcut_regex, __pyx_kp_u__4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF_SET(__pyx_v_shortcut_regex, ((PyObject*)__pyx_t_2));
   __pyx_t_2 = 0;
 
   /* "SpellChecker/SimpleSpellChecker.pyx":231
  *             shortcut_regex = shortcut_regex + "|" + self.__shortcuts[i]
  *         shortcut_regex = shortcut_regex + ")"
- *         compiled_expression = re.compile("[0-9]+")             # <<<<<<<<<<<<<<
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):
- *             result.addWord(word)
+ *         compiled_expression = re.compile(shortcut_regex)             # <<<<<<<<<<<<<<
+ *         if compiled_expression.fullmatch(word.getName()):
+ *             pair = self.getSplitPair(word)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
@@ -6422,248 +6415,142 @@
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_u_0_9_2) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_0_9_2);
+  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_shortcut_regex) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_shortcut_regex);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_compiled_expression = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "SpellChecker/SimpleSpellChecker.pyx":232
  *         shortcut_regex = shortcut_regex + ")"
- *         compiled_expression = re.compile("[0-9]+")
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):             # <<<<<<<<<<<<<<
- *             result.addWord(word)
- *             return True
- */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_shortcuts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_10 = (__Pyx_PySequence_ContainsTF(__pyx_t_2, __pyx_t_1, Py_EQ)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_11 = (__pyx_t_10 != 0);
-  if (__pyx_t_11) {
-  } else {
-    __pyx_t_7 = __pyx_t_11;
-    goto __pyx_L6_bool_binop_done;
-  }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_compiled_expression, __pyx_n_s_fullmatch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previousWord->__pyx_vtab)->getName(__pyx_v_previousWord, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __pyx_t_11;
-  __pyx_L6_bool_binop_done:;
-  if (__pyx_t_7) {
-
-    /* "SpellChecker/SimpleSpellChecker.pyx":233
- *         compiled_expression = re.compile("[0-9]+")
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):
- *             result.addWord(word)             # <<<<<<<<<<<<<<
- *             return True
- *         compiled_expression = re.compile(shortcut_regex)
- */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_6Corpus_8Sentence_Sentence *)__pyx_v_result->__pyx_vtab)->addWord(__pyx_v_result, __pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "SpellChecker/SimpleSpellChecker.pyx":234
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):
- *             result.addWord(word)
- *             return True             # <<<<<<<<<<<<<<
- *         compiled_expression = re.compile(shortcut_regex)
- *         if compiled_expression.fullmatch(word.getName()):
- */
-    __pyx_r = 1;
-    goto __pyx_L0;
-
-    /* "SpellChecker/SimpleSpellChecker.pyx":232
- *         shortcut_regex = shortcut_regex + ")"
- *         compiled_expression = re.compile("[0-9]+")
- *         if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):             # <<<<<<<<<<<<<<
- *             result.addWord(word)
- *             return True
- */
-  }
-
-  /* "SpellChecker/SimpleSpellChecker.pyx":235
- *             result.addWord(word)
- *             return True
- *         compiled_expression = re.compile(shortcut_regex)             # <<<<<<<<<<<<<<
- *         if compiled_expression.fullmatch(word.getName()):
- *             pair = self.getSplitPair(word)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_shortcut_regex) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_shortcut_regex);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF_SET(__pyx_v_compiled_expression, __pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "SpellChecker/SimpleSpellChecker.pyx":236
- *             return True
  *         compiled_expression = re.compile(shortcut_regex)
  *         if compiled_expression.fullmatch(word.getName()):             # <<<<<<<<<<<<<<
  *             pair = self.getSplitPair(word)
  *             forced_replacement = pair[0] + " " + pair[1]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_compiled_expression, __pyx_n_s_fullmatch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_compiled_expression, __pyx_n_s_fullmatch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
+  __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_7) {
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":237
+    /* "SpellChecker/SimpleSpellChecker.pyx":233
  *         compiled_expression = re.compile(shortcut_regex)
  *         if compiled_expression.fullmatch(word.getName()):
  *             pair = self.getSplitPair(word)             # <<<<<<<<<<<<<<
  *             forced_replacement = pair[0] + " " + pair[1]
  *             result.addWord(Word(forced_replacement))
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self->__pyx_base.__pyx_vtab)->getSplitPair(__pyx_v_self, __pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_v_pair = ((PyObject*)__pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self->__pyx_base.__pyx_vtab)->getSplitPair(__pyx_v_self, __pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_v_pair = ((PyObject*)__pyx_t_2);
+    __pyx_t_2 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":238
+    /* "SpellChecker/SimpleSpellChecker.pyx":234
  *         if compiled_expression.fullmatch(word.getName()):
  *             pair = self.getSplitPair(word)
  *             forced_replacement = pair[0] + " " + pair[1]             # <<<<<<<<<<<<<<
  *             result.addWord(Word(forced_replacement))
  *             return True
  */
     if (unlikely(__pyx_v_pair == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 238, __pyx_L1_error)
+      __PYX_ERR(0, 234, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt_Tuple(__pyx_v_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(__pyx_v_pair == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 238, __pyx_L1_error)
+      __PYX_ERR(0, 234, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_pair, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt_Tuple(__pyx_v_pair, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 238, __pyx_L1_error)
-    __pyx_v_forced_replacement = ((PyObject*)__pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_v_forced_replacement = ((PyObject*)__pyx_t_3);
+    __pyx_t_3 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":239
+    /* "SpellChecker/SimpleSpellChecker.pyx":235
  *             pair = self.getSplitPair(word)
  *             forced_replacement = pair[0] + " " + pair[1]
  *             result.addWord(Word(forced_replacement))             # <<<<<<<<<<<<<<
  *             return True
  *         return False
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10Dictionary_4Word_Word), __pyx_v_forced_replacement); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10Dictionary_4Word_Word), __pyx_v_forced_replacement); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = ((struct __pyx_vtabstruct_6Corpus_8Sentence_Sentence *)__pyx_v_result->__pyx_vtab)->addWord(__pyx_v_result, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_3), 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = ((struct __pyx_vtabstruct_6Corpus_8Sentence_Sentence *)__pyx_v_result->__pyx_vtab)->addWord(__pyx_v_result, ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_t_2), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":240
+    /* "SpellChecker/SimpleSpellChecker.pyx":236
  *             forced_replacement = pair[0] + " " + pair[1]
  *             result.addWord(Word(forced_replacement))
  *             return True             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":236
- *             return True
+    /* "SpellChecker/SimpleSpellChecker.pyx":232
+ *         shortcut_regex = shortcut_regex + ")"
  *         compiled_expression = re.compile(shortcut_regex)
  *         if compiled_expression.fullmatch(word.getName()):             # <<<<<<<<<<<<<<
  *             pair = self.getSplitPair(word)
  *             forced_replacement = pair[0] + " " + pair[1]
  */
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":241
+  /* "SpellChecker/SimpleSpellChecker.pyx":237
  *             result.addWord(Word(forced_replacement))
  *             return True
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     cpdef loadDictionaries(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
   /* "SpellChecker/SimpleSpellChecker.pyx":224
  *         return False
  * 
- *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result, Word previousWord):             # <<<<<<<<<<<<<<
+ *     cpdef bint forcedShortcutCheck(self, Word word, Sentence result):             # <<<<<<<<<<<<<<
  *         cdef str shortcut_regex, forced_replacement
  *         cdef int i
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -6683,30 +6570,27 @@
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_19forcedShortcutCheck(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_19forcedShortcutCheck(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word = 0;
   struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result = 0;
-  struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("forcedShortcutCheck (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_word,&__pyx_n_s_result,&__pyx_n_s_previousWord,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_word,&__pyx_n_s_result,0};
+    PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -6715,69 +6599,60 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_word)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("forcedShortcutCheck", 1, 3, 3, 1); __PYX_ERR(0, 224, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_previousWord)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("forcedShortcutCheck", 1, 3, 3, 2); __PYX_ERR(0, 224, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("forcedShortcutCheck", 1, 2, 2, 1); __PYX_ERR(0, 224, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "forcedShortcutCheck") < 0)) __PYX_ERR(0, 224, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_word = ((struct __pyx_obj_10Dictionary_4Word_Word *)values[0]);
     __pyx_v_result = ((struct __pyx_obj_6Corpus_8Sentence_Sentence *)values[1]);
-    __pyx_v_previousWord = ((struct __pyx_obj_10Dictionary_4Word_Word *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("forcedShortcutCheck", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 224, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("forcedShortcutCheck", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 224, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("SpellChecker.SimpleSpellChecker.SimpleSpellChecker.forcedShortcutCheck", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 224, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result), __pyx_ptype_6Corpus_8Sentence_Sentence, 1, "result", 0))) __PYX_ERR(0, 224, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_previousWord), __pyx_ptype_10Dictionary_4Word_Word, 1, "previousWord", 0))) __PYX_ERR(0, 224, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_word, __pyx_v_result, __pyx_v_previousWord);
+  __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_word, __pyx_v_result);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_previousWord) {
+static PyObject *__pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_18forcedShortcutCheck(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *__pyx_v_self, struct __pyx_obj_10Dictionary_4Word_Word *__pyx_v_word, struct __pyx_obj_6Corpus_8Sentence_Sentence *__pyx_v_result) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("forcedShortcutCheck", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(__pyx_v_self, __pyx_v_word, __pyx_v_result, __pyx_v_previousWord, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck(__pyx_v_self, __pyx_v_word, __pyx_v_result, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6786,15 +6661,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SpellChecker/SimpleSpellChecker.pyx":243
+/* "SpellChecker/SimpleSpellChecker.pyx":239
  *         return False
  * 
  *     cpdef loadDictionaries(self):             # <<<<<<<<<<<<<<
  *         cdef str line
  *         cdef list items, lines
  */
 
@@ -6822,15 +6697,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_loadDictionaries); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_loadDictionaries); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_21loadDictionaries)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6839,15 +6714,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -6860,27 +6735,27 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":246
+  /* "SpellChecker/SimpleSpellChecker.pyx":242
  *         cdef str line
  *         cdef list items, lines
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/merged.txt'), "r", encoding="utf8")             # <<<<<<<<<<<<<<
  *         lines = input_file.readlines()
  *         for line in lines:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pkg_resources); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pkg_resources); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_resource_filename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_resource_filename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -6889,236 +6764,236 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_kp_u_data_merged_txt};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_kp_u_data_merged_txt};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_t_2);
     __Pyx_INCREF(__pyx_kp_u_data_merged_txt);
     __Pyx_GIVEREF(__pyx_kp_u_data_merged_txt);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_kp_u_data_merged_txt);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_r);
   __Pyx_GIVEREF(__pyx_n_u_r);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_n_u_r);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_n_u_utf8) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_n_u_utf8) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_input_file = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":247
+  /* "SpellChecker/SimpleSpellChecker.pyx":243
  *         cdef list items, lines
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/merged.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()             # <<<<<<<<<<<<<<
  *         for line in lines:
  *             items = line.strip().split(" ")
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_readlines); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_readlines); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_6 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(PyList_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 247, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 243, __pyx_L1_error)
   __pyx_v_lines = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":248
+  /* "SpellChecker/SimpleSpellChecker.pyx":244
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/merged.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()
  *         for line in lines:             # <<<<<<<<<<<<<<
  *             items = line.strip().split(" ")
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]
  */
   if (unlikely(__pyx_v_lines == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 248, __pyx_L1_error)
+    __PYX_ERR(0, 244, __pyx_L1_error)
   }
   __pyx_t_6 = __pyx_v_lines; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
   for (;;) {
     if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 248, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_line, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":249
+    /* "SpellChecker/SimpleSpellChecker.pyx":245
  *         lines = input_file.readlines()
  *         for line in lines:
  *             items = line.strip().split(" ")             # <<<<<<<<<<<<<<
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]
  *         input_file.close()
  */
-    __pyx_t_3 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_strip, __pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_strip, __pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u__2) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u__2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 249, __pyx_L1_error)
+    if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 245, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_items, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":250
+    /* "SpellChecker/SimpleSpellChecker.pyx":246
  *         for line in lines:
  *             items = line.strip().split(" ")
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]             # <<<<<<<<<<<<<<
  *         input_file.close()
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")
  */
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 250, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_items, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_items, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_self->__pyx___merged_words == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 250, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 250, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_items, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_items, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 250, __pyx_L1_error)
+      __PYX_ERR(0, 246, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_self->__pyx___merged_words, __pyx_t_4, __pyx_t_1) < 0)) __PYX_ERR(0, 250, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->__pyx___merged_words, __pyx_t_4, __pyx_t_1) < 0)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":248
+    /* "SpellChecker/SimpleSpellChecker.pyx":244
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/merged.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()
  *         for line in lines:             # <<<<<<<<<<<<<<
  *             items = line.strip().split(" ")
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":251
+  /* "SpellChecker/SimpleSpellChecker.pyx":247
  *             items = line.strip().split(" ")
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]
  *         input_file.close()             # <<<<<<<<<<<<<<
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":252
+  /* "SpellChecker/SimpleSpellChecker.pyx":248
  *             self.__merged_words[items[0] + " " + items[1]] = items[2]
  *         input_file.close()
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")             # <<<<<<<<<<<<<<
  *         lines = input_file.readlines()
  *         for line in lines:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pkg_resources); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pkg_resources); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_resource_filename); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_resource_filename); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7127,224 +7002,224 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_t_1, __pyx_kp_u_data_split_txt};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_t_1, __pyx_kp_u_data_split_txt};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   {
-    __pyx_t_3 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_5, __pyx_t_1);
     __Pyx_INCREF(__pyx_kp_u_data_split_txt);
     __Pyx_GIVEREF(__pyx_kp_u_data_split_txt);
     PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_5, __pyx_kp_u_data_split_txt);
     __pyx_t_1 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __Pyx_INCREF(__pyx_n_u_r);
   __Pyx_GIVEREF(__pyx_n_u_r);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_r);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_encoding, __pyx_n_u_utf8) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_encoding, __pyx_n_u_utf8) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF_SET(__pyx_v_input_file, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":253
+  /* "SpellChecker/SimpleSpellChecker.pyx":249
  *         input_file.close()
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()             # <<<<<<<<<<<<<<
  *         for line in lines:
  *             items = line.strip().split(" ")
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_readlines); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_readlines); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(PyList_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_lines, ((PyObject*)__pyx_t_3));
   __pyx_t_3 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":254
+  /* "SpellChecker/SimpleSpellChecker.pyx":250
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()
  *         for line in lines:             # <<<<<<<<<<<<<<
  *             items = line.strip().split(" ")
  *             self.__split_words[items[0]] = items[1] + " " + items[2]
  */
   if (unlikely(__pyx_v_lines == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 254, __pyx_L1_error)
+    __PYX_ERR(0, 250, __pyx_L1_error)
   }
   __pyx_t_3 = __pyx_v_lines; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
   for (;;) {
     if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 250, __pyx_L1_error)
     #else
-    __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     #endif
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 254, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_line, ((PyObject*)__pyx_t_6));
     __pyx_t_6 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":255
+    /* "SpellChecker/SimpleSpellChecker.pyx":251
  *         lines = input_file.readlines()
  *         for line in lines:
  *             items = line.strip().split(" ")             # <<<<<<<<<<<<<<
  *             self.__split_words[items[0]] = items[1] + " " + items[2]
  *         input_file.close()
  */
-    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_strip, __pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_strip, __pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_kp_u__2) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u__2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(PyList_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 255, __pyx_L1_error)
+    if (!(likely(PyList_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_items, ((PyObject*)__pyx_t_6));
     __pyx_t_6 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":256
+    /* "SpellChecker/SimpleSpellChecker.pyx":252
  *         for line in lines:
  *             items = line.strip().split(" ")
  *             self.__split_words[items[0]] = items[1] + " " + items[2]             # <<<<<<<<<<<<<<
  *         input_file.close()
  * 
  */
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 256, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 256, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 2, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v_self->__pyx___split_words == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 256, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_items == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 256, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_items, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(PyDict_SetItem(__pyx_v_self->__pyx___split_words, __pyx_t_6, __pyx_t_4) < 0)) __PYX_ERR(0, 256, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->__pyx___split_words, __pyx_t_6, __pyx_t_4) < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":254
+    /* "SpellChecker/SimpleSpellChecker.pyx":250
  *         input_file = open(pkg_resources.resource_filename(__name__, 'data/split.txt'), "r", encoding="utf8")
  *         lines = input_file.readlines()
  *         for line in lines:             # <<<<<<<<<<<<<<
  *             items = line.strip().split(" ")
  *             self.__split_words[items[0]] = items[1] + " " + items[2]
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":257
+  /* "SpellChecker/SimpleSpellChecker.pyx":253
  *             items = line.strip().split(" ")
  *             self.__split_words[items[0]] = items[1] + " " + items[2]
  *         input_file.close()             # <<<<<<<<<<<<<<
  * 
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_input_file, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 257, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":243
+  /* "SpellChecker/SimpleSpellChecker.pyx":239
  *         return False
  * 
  *     cpdef loadDictionaries(self):             # <<<<<<<<<<<<<<
  *         cdef str line
  *         cdef list items, lines
  */
 
@@ -7387,15 +7262,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("loadDictionaries", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_loadDictionaries(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_loadDictionaries(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7404,15 +7279,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SpellChecker/SimpleSpellChecker.pyx":259
+/* "SpellChecker/SimpleSpellChecker.pyx":255
  *         input_file.close()
  * 
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):             # <<<<<<<<<<<<<<
  *         if wordName in dictionary:
  *             return dictionary[wordName]
  */
 
@@ -7437,15 +7312,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getCorrectForm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getCorrectForm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_23getCorrectForm)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -7457,45 +7332,45 @@
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_wordName, __pyx_v_dictionary};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_wordName, __pyx_v_dictionary};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_4) {
             __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
           }
           __Pyx_INCREF(__pyx_v_wordName);
           __Pyx_GIVEREF(__pyx_v_wordName);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_wordName);
           __Pyx_INCREF(__pyx_v_dictionary);
           __Pyx_GIVEREF(__pyx_v_dictionary);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_dictionary);
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 259, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 255, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -7506,70 +7381,70 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":260
+  /* "SpellChecker/SimpleSpellChecker.pyx":256
  * 
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):
  *         if wordName in dictionary:             # <<<<<<<<<<<<<<
  *             return dictionary[wordName]
  *         return ""
  */
   if (unlikely(__pyx_v_dictionary == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 260, __pyx_L1_error)
+    __PYX_ERR(0, 256, __pyx_L1_error)
   }
-  __pyx_t_7 = (__Pyx_PyDict_ContainsTF(__pyx_v_wordName, __pyx_v_dictionary, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_7 = (__Pyx_PyDict_ContainsTF(__pyx_v_wordName, __pyx_v_dictionary, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 256, __pyx_L1_error)
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":261
+    /* "SpellChecker/SimpleSpellChecker.pyx":257
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):
  *         if wordName in dictionary:
  *             return dictionary[wordName]             # <<<<<<<<<<<<<<
  *         return ""
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_dictionary == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 261, __pyx_L1_error)
+      __PYX_ERR(0, 257, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_dictionary, __pyx_v_wordName); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_dictionary, __pyx_v_wordName); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 261, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 257, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":260
+    /* "SpellChecker/SimpleSpellChecker.pyx":256
  * 
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):
  *         if wordName in dictionary:             # <<<<<<<<<<<<<<
  *             return dictionary[wordName]
  *         return ""
  */
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":262
+  /* "SpellChecker/SimpleSpellChecker.pyx":258
  *         if wordName in dictionary:
  *             return dictionary[wordName]
  *         return ""             # <<<<<<<<<<<<<<
  * 
  *     cpdef list mergedCandidatesList(self, Word previousWord, Word word, Word nextWord):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_kp_u_);
   __pyx_r = __pyx_kp_u_;
   goto __pyx_L0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":259
+  /* "SpellChecker/SimpleSpellChecker.pyx":255
  *         input_file.close()
  * 
  *     cpdef str getCorrectForm(self, str wordName, dict dictionary):             # <<<<<<<<<<<<<<
  *         if wordName in dictionary:
  *             return dictionary[wordName]
  */
 
@@ -7618,39 +7493,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_wordName)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dictionary)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("getCorrectForm", 1, 2, 2, 1); __PYX_ERR(0, 259, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("getCorrectForm", 1, 2, 2, 1); __PYX_ERR(0, 255, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getCorrectForm") < 0)) __PYX_ERR(0, 259, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getCorrectForm") < 0)) __PYX_ERR(0, 255, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_wordName = ((PyObject*)values[0]);
     __pyx_v_dictionary = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getCorrectForm", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 259, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getCorrectForm", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 255, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("SpellChecker.SimpleSpellChecker.SimpleSpellChecker.getCorrectForm", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_wordName), (&PyUnicode_Type), 1, "wordName", 1))) __PYX_ERR(0, 259, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dictionary), (&PyDict_Type), 1, "dictionary", 1))) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_wordName), (&PyUnicode_Type), 1, "wordName", 1))) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dictionary), (&PyDict_Type), 1, "dictionary", 1))) __PYX_ERR(0, 255, __pyx_L1_error)
   __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_22getCorrectForm(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_wordName, __pyx_v_dictionary);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7663,15 +7538,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getCorrectForm", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getCorrectForm(__pyx_v_self, __pyx_v_wordName, __pyx_v_dictionary, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getCorrectForm(__pyx_v_self, __pyx_v_wordName, __pyx_v_dictionary, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7680,15 +7555,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SpellChecker/SimpleSpellChecker.pyx":264
+/* "SpellChecker/SimpleSpellChecker.pyx":260
  *         return ""
  * 
  *     cpdef list mergedCandidatesList(self, Word previousWord, Word word, Word nextWord):             # <<<<<<<<<<<<<<
  *         cdef list merged_candidates
  *         cdef Candidate backward_merge_candidate, forward_merge_candidate
  */
 
@@ -7719,15 +7594,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mergedCandidatesList); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mergedCandidatesList); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_25mergedCandidatesList)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -7739,48 +7614,48 @@
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_v_previousWord), ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_nextWord)};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_v_previousWord), ((PyObject *)__pyx_v_word), ((PyObject *)__pyx_v_nextWord)};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_4) {
             __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
           }
           __Pyx_INCREF(((PyObject *)__pyx_v_previousWord));
           __Pyx_GIVEREF(((PyObject *)__pyx_v_previousWord));
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, ((PyObject *)__pyx_v_previousWord));
           __Pyx_INCREF(((PyObject *)__pyx_v_word));
           __Pyx_GIVEREF(((PyObject *)__pyx_v_word));
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, ((PyObject *)__pyx_v_word));
           __Pyx_INCREF(((PyObject *)__pyx_v_nextWord));
           __Pyx_GIVEREF(((PyObject *)__pyx_v_nextWord));
           PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, ((PyObject *)__pyx_v_nextWord));
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 264, __pyx_L1_error)
+        if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 260, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -7791,280 +7666,280 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":268
+  /* "SpellChecker/SimpleSpellChecker.pyx":264
  *         cdef Candidate backward_merge_candidate, forward_merge_candidate
  *         cdef FsmParseList fsm_parse_list
  *         merged_candidates = []             # <<<<<<<<<<<<<<
  *         backward_merge_candidate = None
  *         if previousWord is not None:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_merged_candidates = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":269
+  /* "SpellChecker/SimpleSpellChecker.pyx":265
  *         cdef FsmParseList fsm_parse_list
  *         merged_candidates = []
  *         backward_merge_candidate = None             # <<<<<<<<<<<<<<
  *         if previousWord is not None:
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_backward_merge_candidate = ((struct __pyx_obj_12SpellChecker_9Candidate_Candidate *)Py_None);
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":270
+  /* "SpellChecker/SimpleSpellChecker.pyx":266
  *         merged_candidates = []
  *         backward_merge_candidate = None
  *         if previousWord is not None:             # <<<<<<<<<<<<<<
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  */
   __pyx_t_7 = (((PyObject *)__pyx_v_previousWord) != Py_None);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":271
+    /* "SpellChecker/SimpleSpellChecker.pyx":267
  *         backward_merge_candidate = None
  *         if previousWord is not None:
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)             # <<<<<<<<<<<<<<
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  *             if fsm_parse_list.size() != 0:
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previousWord->__pyx_vtab)->getName(__pyx_v_previousWord, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_previousWord->__pyx_vtab)->getName(__pyx_v_previousWord, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BACKWARD_MERGE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BACKWARD_MERGE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
     __pyx_t_3 = 0;
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_backward_merge_candidate, ((struct __pyx_obj_12SpellChecker_9Candidate_Candidate *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":272
+    /* "SpellChecker/SimpleSpellChecker.pyx":268
  *         if previousWord is not None:
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())             # <<<<<<<<<<<<<<
  *             if fsm_parse_list.size() != 0:
  *                 merged_candidates.append(backward_merge_candidate)
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_backward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_backward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_backward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_backward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 272, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 268, __pyx_L1_error)
     __pyx_v_fsm_parse_list = ((struct __pyx_obj_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":273
+    /* "SpellChecker/SimpleSpellChecker.pyx":269
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  *             if fsm_parse_list.size() != 0:             # <<<<<<<<<<<<<<
  *                 merged_candidates.append(backward_merge_candidate)
  *         if nextWord is not None:
  */
     __pyx_t_8 = ((((struct __pyx_vtabstruct_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_v_fsm_parse_list->__pyx_vtab)->size(__pyx_v_fsm_parse_list, 0) != 0) != 0);
     if (__pyx_t_8) {
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":274
+      /* "SpellChecker/SimpleSpellChecker.pyx":270
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  *             if fsm_parse_list.size() != 0:
  *                 merged_candidates.append(backward_merge_candidate)             # <<<<<<<<<<<<<<
  *         if nextWord is not None:
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_merged_candidates, ((PyObject *)__pyx_v_backward_merge_candidate)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 274, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_merged_candidates, ((PyObject *)__pyx_v_backward_merge_candidate)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 270, __pyx_L1_error)
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":273
+      /* "SpellChecker/SimpleSpellChecker.pyx":269
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  *             if fsm_parse_list.size() != 0:             # <<<<<<<<<<<<<<
  *                 merged_candidates.append(backward_merge_candidate)
  *         if nextWord is not None:
  */
     }
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":270
+    /* "SpellChecker/SimpleSpellChecker.pyx":266
  *         merged_candidates = []
  *         backward_merge_candidate = None
  *         if previousWord is not None:             # <<<<<<<<<<<<<<
  *             backward_merge_candidate = Candidate(previousWord.getName() + word.getName(), Operator.BACKWARD_MERGE)
  *             fsm_parse_list = self.fsm.morphologicalAnalysis(backward_merge_candidate.getName())
  */
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":275
+  /* "SpellChecker/SimpleSpellChecker.pyx":271
  *             if fsm_parse_list.size() != 0:
  *                 merged_candidates.append(backward_merge_candidate)
  *         if nextWord is not None:             # <<<<<<<<<<<<<<
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  */
   __pyx_t_8 = (((PyObject *)__pyx_v_nextWord) != Py_None);
   __pyx_t_7 = (__pyx_t_8 != 0);
   if (__pyx_t_7) {
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":276
+    /* "SpellChecker/SimpleSpellChecker.pyx":272
  *                 merged_candidates.append(backward_merge_candidate)
  *         if nextWord is not None:
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)             # <<<<<<<<<<<<<<
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_nextWord->__pyx_vtab)->getName(__pyx_v_nextWord, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_nextWord->__pyx_vtab)->getName(__pyx_v_nextWord, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FORWARD_MERGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FORWARD_MERGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_forward_merge_candidate = ((struct __pyx_obj_12SpellChecker_9Candidate_Candidate *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":277
+    /* "SpellChecker/SimpleSpellChecker.pyx":273
  *         if nextWord is not None:
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():             # <<<<<<<<<<<<<<
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  *                 if fsm_parse_list.size() != 0:
  */
     __pyx_t_8 = (((PyObject *)__pyx_v_backward_merge_candidate) == Py_None);
     __pyx_t_10 = (__pyx_t_8 != 0);
     if (!__pyx_t_10) {
     } else {
       __pyx_t_7 = __pyx_t_10;
       goto __pyx_L7_bool_binop_done;
     }
-    __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_backward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_backward_merge_candidate), 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_backward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_backward_merge_candidate), 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_forward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_forward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_forward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_forward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_10 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_t_1, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_10 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_t_1, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_8 = (__pyx_t_10 != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":278
+      /* "SpellChecker/SimpleSpellChecker.pyx":274
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())             # <<<<<<<<<<<<<<
  *                 if fsm_parse_list.size() != 0:
  *                     merged_candidates.append(forward_merge_candidate)
  */
-      __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_forward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_forward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_12SpellChecker_9Candidate_Candidate *)__pyx_v_forward_merge_candidate->__pyx_base.__pyx_vtab)->__pyx_base.getName(((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_forward_merge_candidate), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 278, __pyx_L1_error)
+      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 274, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_fsm_parse_list, ((struct __pyx_obj_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":279
+      /* "SpellChecker/SimpleSpellChecker.pyx":275
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  *                 if fsm_parse_list.size() != 0:             # <<<<<<<<<<<<<<
  *                     merged_candidates.append(forward_merge_candidate)
  *         return merged_candidates
  */
       __pyx_t_7 = ((((struct __pyx_vtabstruct_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_v_fsm_parse_list->__pyx_vtab)->size(__pyx_v_fsm_parse_list, 0) != 0) != 0);
       if (__pyx_t_7) {
 
-        /* "SpellChecker/SimpleSpellChecker.pyx":280
+        /* "SpellChecker/SimpleSpellChecker.pyx":276
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  *                 if fsm_parse_list.size() != 0:
  *                     merged_candidates.append(forward_merge_candidate)             # <<<<<<<<<<<<<<
  *         return merged_candidates
  * 
  */
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_merged_candidates, ((PyObject *)__pyx_v_forward_merge_candidate)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 280, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_merged_candidates, ((PyObject *)__pyx_v_forward_merge_candidate)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 276, __pyx_L1_error)
 
-        /* "SpellChecker/SimpleSpellChecker.pyx":279
+        /* "SpellChecker/SimpleSpellChecker.pyx":275
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  *                 if fsm_parse_list.size() != 0:             # <<<<<<<<<<<<<<
  *                     merged_candidates.append(forward_merge_candidate)
  *         return merged_candidates
  */
       }
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":277
+      /* "SpellChecker/SimpleSpellChecker.pyx":273
  *         if nextWord is not None:
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():             # <<<<<<<<<<<<<<
  *                 fsm_parse_list = self.fsm.morphologicalAnalysis(forward_merge_candidate.getName())
  *                 if fsm_parse_list.size() != 0:
  */
     }
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":275
+    /* "SpellChecker/SimpleSpellChecker.pyx":271
  *             if fsm_parse_list.size() != 0:
  *                 merged_candidates.append(backward_merge_candidate)
  *         if nextWord is not None:             # <<<<<<<<<<<<<<
  *             forward_merge_candidate = Candidate(word.getName() + nextWord.getName(), Operator.FORWARD_MERGE)
  *             if backward_merge_candidate is None or backward_merge_candidate.getName() != forward_merge_candidate.getName():
  */
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":281
+  /* "SpellChecker/SimpleSpellChecker.pyx":277
  *                 if fsm_parse_list.size() != 0:
  *                     merged_candidates.append(forward_merge_candidate)
  *         return merged_candidates             # <<<<<<<<<<<<<<
  * 
  *     cpdef list splitCandidatesList(self, Word word):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_merged_candidates);
   __pyx_r = __pyx_v_merged_candidates;
   goto __pyx_L0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":264
+  /* "SpellChecker/SimpleSpellChecker.pyx":260
  *         return ""
  * 
  *     cpdef list mergedCandidatesList(self, Word previousWord, Word word, Word nextWord):             # <<<<<<<<<<<<<<
  *         cdef list merged_candidates
  *         cdef Candidate backward_merge_candidate, forward_merge_candidate
  */
 
@@ -8120,48 +7995,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_previousWord)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_word)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, 1); __PYX_ERR(0, 264, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, 1); __PYX_ERR(0, 260, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nextWord)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, 2); __PYX_ERR(0, 264, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, 2); __PYX_ERR(0, 260, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "mergedCandidatesList") < 0)) __PYX_ERR(0, 264, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "mergedCandidatesList") < 0)) __PYX_ERR(0, 260, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_previousWord = ((struct __pyx_obj_10Dictionary_4Word_Word *)values[0]);
     __pyx_v_word = ((struct __pyx_obj_10Dictionary_4Word_Word *)values[1]);
     __pyx_v_nextWord = ((struct __pyx_obj_10Dictionary_4Word_Word *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 264, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("mergedCandidatesList", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 260, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("SpellChecker.SimpleSpellChecker.SimpleSpellChecker.mergedCandidatesList", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_previousWord), __pyx_ptype_10Dictionary_4Word_Word, 1, "previousWord", 0))) __PYX_ERR(0, 264, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 264, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_nextWord), __pyx_ptype_10Dictionary_4Word_Word, 1, "nextWord", 0))) __PYX_ERR(0, 264, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_previousWord), __pyx_ptype_10Dictionary_4Word_Word, 1, "previousWord", 0))) __PYX_ERR(0, 260, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 260, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_nextWord), __pyx_ptype_10Dictionary_4Word_Word, 1, "nextWord", 0))) __PYX_ERR(0, 260, __pyx_L1_error)
   __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_24mergedCandidatesList(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), __pyx_v_previousWord, __pyx_v_word, __pyx_v_nextWord);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8174,15 +8049,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mergedCandidatesList", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_mergedCandidatesList(__pyx_v_self, __pyx_v_previousWord, __pyx_v_word, __pyx_v_nextWord, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_mergedCandidatesList(__pyx_v_self, __pyx_v_previousWord, __pyx_v_word, __pyx_v_nextWord, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8191,15 +8066,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SpellChecker/SimpleSpellChecker.pyx":283
+/* "SpellChecker/SimpleSpellChecker.pyx":279
  *         return merged_candidates
  * 
  *     cpdef list splitCandidatesList(self, Word word):             # <<<<<<<<<<<<<<
  *         cdef list split_candidates
  *         cdef int i
  */
 
@@ -8232,15 +8107,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_splitCandidatesList); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_splitCandidatesList); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_27splitCandidatesList)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8249,18 +8124,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_word)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_word));
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 283, __pyx_L1_error)
+        if (!(likely(PyList_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 279, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8271,111 +8146,111 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":288
+  /* "SpellChecker/SimpleSpellChecker.pyx":284
  *         cdef str first_part, second_part
  *         cdef FsmParseList fsm_parse_list_first, fsm_parse_list_second
  *         split_candidates = []             # <<<<<<<<<<<<<<
  *         for i in range(4, len(word.getName()) - 3):
  *             first_part = word.getName()[0:i]
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_split_candidates = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":289
+  /* "SpellChecker/SimpleSpellChecker.pyx":285
  *         cdef FsmParseList fsm_parse_list_first, fsm_parse_list_second
  *         split_candidates = []
  *         for i in range(4, len(word.getName()) - 3):             # <<<<<<<<<<<<<<
  *             first_part = word.getName()[0:i]
  *             second_part = word.getName()[i:]
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 289, __pyx_L1_error)
+    __PYX_ERR(0, 285, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = (__pyx_t_5 - 3);
   __pyx_t_5 = __pyx_t_6;
   for (__pyx_t_7 = 4; __pyx_t_7 < __pyx_t_5; __pyx_t_7+=1) {
     __pyx_v_i = __pyx_t_7;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":290
+    /* "SpellChecker/SimpleSpellChecker.pyx":286
  *         split_candidates = []
  *         for i in range(4, len(word.getName()) - 3):
  *             first_part = word.getName()[0:i]             # <<<<<<<<<<<<<<
  *             second_part = word.getName()[i:]
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_t_1 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 290, __pyx_L1_error)
+      __PYX_ERR(0, 286, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyUnicode_Substring(__pyx_t_1, 0, __pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Substring(__pyx_t_1, 0, __pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_first_part, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":291
+    /* "SpellChecker/SimpleSpellChecker.pyx":287
  *         for i in range(4, len(word.getName()) - 3):
  *             first_part = word.getName()[0:i]
  *             second_part = word.getName()[i:]             # <<<<<<<<<<<<<<
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (unlikely(__pyx_t_2 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 291, __pyx_L1_error)
+      __PYX_ERR(0, 287, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_t_2, __pyx_v_i, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_t_2, __pyx_v_i, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_second_part, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":292
+    /* "SpellChecker/SimpleSpellChecker.pyx":288
  *             first_part = word.getName()[0:i]
  *             second_part = word.getName()[i:]
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)             # <<<<<<<<<<<<<<
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_v_first_part, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_v_first_part, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 292, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fsm_parse_list_first, ((struct __pyx_obj_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":293
+    /* "SpellChecker/SimpleSpellChecker.pyx":289
  *             second_part = word.getName()[i:]
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)             # <<<<<<<<<<<<<<
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:
  *                 split_candidates.append(Candidate(first_part + " " + second_part, Operator.SPLIT))
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_v_second_part, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_21MorphologicalAnalysis_24FsmMorphologicalAnalyzer_FsmMorphologicalAnalyzer *)__pyx_v_self->fsm->__pyx_vtab)->morphologicalAnalysis(__pyx_v_self->fsm, __pyx_v_second_part, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 293, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21MorphologicalAnalysis_12FsmParseList_FsmParseList))))) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_fsm_parse_list_second, ((struct __pyx_obj_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":294
+    /* "SpellChecker/SimpleSpellChecker.pyx":290
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:             # <<<<<<<<<<<<<<
  *                 split_candidates.append(Candidate(first_part + " " + second_part, Operator.SPLIT))
  *         return split_candidates
  */
     __pyx_t_9 = ((((struct __pyx_vtabstruct_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_v_fsm_parse_list_first->__pyx_vtab)->size(__pyx_v_fsm_parse_list_first, 0) > 0) != 0);
@@ -8385,68 +8260,68 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_9 = ((((struct __pyx_vtabstruct_21MorphologicalAnalysis_12FsmParseList_FsmParseList *)__pyx_v_fsm_parse_list_second->__pyx_vtab)->size(__pyx_v_fsm_parse_list_second, 0) > 0) != 0);
     __pyx_t_8 = __pyx_t_9;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_8) {
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":295
+      /* "SpellChecker/SimpleSpellChecker.pyx":291
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:
  *                 split_candidates.append(Candidate(first_part + " " + second_part, Operator.SPLIT))             # <<<<<<<<<<<<<<
  *         return split_candidates
  * 
  */
-      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_first_part, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_first_part, __pyx_kp_u__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_v_second_part); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_v_second_part); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Operator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SPLIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SPLIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
       __pyx_t_2 = 0;
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12SpellChecker_9Candidate_Candidate), __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_split_candidates, __pyx_t_3); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_split_candidates, __pyx_t_3); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":294
+      /* "SpellChecker/SimpleSpellChecker.pyx":290
  *             fsm_parse_list_first = self.fsm.morphologicalAnalysis(first_part)
  *             fsm_parse_list_second = self.fsm.morphologicalAnalysis(second_part)
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:             # <<<<<<<<<<<<<<
  *                 split_candidates.append(Candidate(first_part + " " + second_part, Operator.SPLIT))
  *         return split_candidates
  */
     }
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":296
+  /* "SpellChecker/SimpleSpellChecker.pyx":292
  *             if fsm_parse_list_first.size() > 0 and fsm_parse_list_second.size() > 0:
  *                 split_candidates.append(Candidate(first_part + " " + second_part, Operator.SPLIT))
  *         return split_candidates             # <<<<<<<<<<<<<<
  * 
  *     cpdef tuple getSplitPair(self, Word word):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_split_candidates);
   __pyx_r = __pyx_v_split_candidates;
   goto __pyx_L0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":283
+  /* "SpellChecker/SimpleSpellChecker.pyx":279
  *         return merged_candidates
  * 
  *     cpdef list splitCandidatesList(self, Word word):             # <<<<<<<<<<<<<<
  *         cdef list split_candidates
  *         cdef int i
  */
 
@@ -8474,15 +8349,15 @@
 static PyObject *__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_27splitCandidatesList(PyObject *__pyx_v_self, PyObject *__pyx_v_word) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("splitCandidatesList (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 279, __pyx_L1_error)
   __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_26splitCandidatesList(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_word));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8495,15 +8370,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("splitCandidatesList", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_splitCandidatesList(__pyx_v_self, __pyx_v_word, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_splitCandidatesList(__pyx_v_self, __pyx_v_word, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8512,15 +8387,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "SpellChecker/SimpleSpellChecker.pyx":298
+/* "SpellChecker/SimpleSpellChecker.pyx":294
  *         return split_candidates
  * 
  *     cpdef tuple getSplitPair(self, Word word):             # <<<<<<<<<<<<<<
  *         cdef str key, value
  *         cdef int j
  */
 
@@ -8548,15 +8423,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getSplitPair); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_getSplitPair); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_29getSplitPair)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8565,18 +8440,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_word)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_word));
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 298, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 294, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8587,159 +8462,159 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":301
+  /* "SpellChecker/SimpleSpellChecker.pyx":297
  *         cdef str key, value
  *         cdef int j
  *         key = ""             # <<<<<<<<<<<<<<
  *         j = 0
  *         while j < len(word.getName()):
  */
   __Pyx_INCREF(__pyx_kp_u_);
   __pyx_v_key = __pyx_kp_u_;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":302
+  /* "SpellChecker/SimpleSpellChecker.pyx":298
  *         cdef int j
  *         key = ""
  *         j = 0             # <<<<<<<<<<<<<<
  *         while j < len(word.getName()):
  *             if "0" <= word.getName()[j] <= "9":
  */
   __pyx_v_j = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":303
+  /* "SpellChecker/SimpleSpellChecker.pyx":299
  *         key = ""
  *         j = 0
  *         while j < len(word.getName()):             # <<<<<<<<<<<<<<
  *             if "0" <= word.getName()[j] <= "9":
  *                 key = key + word.getName()[j]
  */
   while (1) {
-    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_t_1 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 303, __pyx_L1_error)
+      __PYX_ERR(0, 299, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 303, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = ((__pyx_v_j < __pyx_t_5) != 0);
     if (!__pyx_t_6) break;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":304
+    /* "SpellChecker/SimpleSpellChecker.pyx":300
  *         j = 0
  *         while j < len(word.getName()):
  *             if "0" <= word.getName()[j] <= "9":             # <<<<<<<<<<<<<<
  *                 key = key + word.getName()[j]
  *             else:
  */
-    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_t_1, __pyx_v_j, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_t_1, __pyx_v_j, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = (48 <= __pyx_t_7);
     if (__pyx_t_6) {
       __pyx_t_6 = (__pyx_t_7 <= 57);
     }
     __pyx_t_8 = (__pyx_t_6 != 0);
     if (__pyx_t_8) {
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":305
+      /* "SpellChecker/SimpleSpellChecker.pyx":301
  *         while j < len(word.getName()):
  *             if "0" <= word.getName()[j] <= "9":
  *                 key = key + word.getName()[j]             # <<<<<<<<<<<<<<
  *             else:
  *                 break
  */
-      __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 305, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_t_1, __pyx_v_j, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 305, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_t_1, __pyx_v_j, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 301, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 305, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromOrdinal(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_v_key, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 305, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_v_key, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "SpellChecker/SimpleSpellChecker.pyx":304
+      /* "SpellChecker/SimpleSpellChecker.pyx":300
  *         j = 0
  *         while j < len(word.getName()):
  *             if "0" <= word.getName()[j] <= "9":             # <<<<<<<<<<<<<<
  *                 key = key + word.getName()[j]
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":307
+    /* "SpellChecker/SimpleSpellChecker.pyx":303
  *                 key = key + word.getName()[j]
  *             else:
  *                 break             # <<<<<<<<<<<<<<
  *             j = j + 1
  *         value = word.getName()[j:]
  */
     /*else*/ {
       goto __pyx_L4_break;
     }
     __pyx_L5:;
 
-    /* "SpellChecker/SimpleSpellChecker.pyx":308
+    /* "SpellChecker/SimpleSpellChecker.pyx":304
  *             else:
  *                 break
  *             j = j + 1             # <<<<<<<<<<<<<<
  *         value = word.getName()[j:]
  *         return key, value
  */
     __pyx_v_j = (__pyx_v_j + 1);
   }
   __pyx_L4_break:;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":309
+  /* "SpellChecker/SimpleSpellChecker.pyx":305
  *                 break
  *             j = j + 1
  *         value = word.getName()[j:]             # <<<<<<<<<<<<<<
  *         return key, value
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_10Dictionary_4Word_Word *)__pyx_v_word->__pyx_vtab)->getName(__pyx_v_word, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (unlikely(__pyx_t_2 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 309, __pyx_L1_error)
+    __PYX_ERR(0, 305, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_t_2, __pyx_v_j, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_t_2, __pyx_v_j, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_value = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":310
+  /* "SpellChecker/SimpleSpellChecker.pyx":306
  *             j = j + 1
  *         value = word.getName()[j:]
  *         return key, value             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_key);
   __Pyx_GIVEREF(__pyx_v_key);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_key);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_value);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "SpellChecker/SimpleSpellChecker.pyx":298
+  /* "SpellChecker/SimpleSpellChecker.pyx":294
  *         return split_candidates
  * 
  *     cpdef tuple getSplitPair(self, Word word):             # <<<<<<<<<<<<<<
  *         cdef str key, value
  *         cdef int j
  */
 
@@ -8764,15 +8639,15 @@
 static PyObject *__pyx_pw_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_29getSplitPair(PyObject *__pyx_v_self, PyObject *__pyx_v_word) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getSplitPair (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 298, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_word), __pyx_ptype_10Dictionary_4Word_Word, 1, "word", 0))) __PYX_ERR(0, 294, __pyx_L1_error)
   __pyx_r = __pyx_pf_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_28getSplitPair(((struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *)__pyx_v_self), ((struct __pyx_obj_10Dictionary_4Word_Word *)__pyx_v_word));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8785,15 +8660,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getSplitPair", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getSplitPair(__pyx_v_self, __pyx_v_word, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getSplitPair(__pyx_v_self, __pyx_v_word, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9741,15 +9616,14 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
   {&__pyx_kp_u_0_9, __pyx_k_0_9, sizeof(__pyx_k_0_9), 0, 1, 0, 0},
-  {&__pyx_kp_u_0_9_2, __pyx_k_0_9_2, sizeof(__pyx_k_0_9_2), 0, 1, 0, 0},
   {&__pyx_n_s_BACKWARD_MERGE, __pyx_k_BACKWARD_MERGE, sizeof(__pyx_k_BACKWARD_MERGE), 0, 0, 1, 1},
   {&__pyx_n_s_FORWARD_MERGE, __pyx_k_FORWARD_MERGE, sizeof(__pyx_k_FORWARD_MERGE), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_s_vs_0x16, __pyx_k_Incompatible_checksums_s_vs_0x16, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x16), 0, 0, 1, 0},
   {&__pyx_n_s_LETTERS, __pyx_k_LETTERS, sizeof(__pyx_k_LETTERS), 0, 0, 1, 1},
   {&__pyx_n_s_LOWERCASE_LETTERS, __pyx_k_LOWERCASE_LETTERS, sizeof(__pyx_k_LOWERCASE_LETTERS), 0, 0, 1, 1},
   {&__pyx_n_s_MISSPELLED_REPLACE, __pyx_k_MISSPELLED_REPLACE, sizeof(__pyx_k_MISSPELLED_REPLACE), 0, 0, 1, 1},
   {&__pyx_n_s_Operator, __pyx_k_Operator, sizeof(__pyx_k_Operator), 0, 0, 1, 1},
@@ -9866,15 +9740,15 @@
   {&__pyx_n_u_watt, __pyx_k_watt, sizeof(__pyx_k_watt), 0, 1, 0, 1},
   {&__pyx_n_s_word, __pyx_k_word, sizeof(__pyx_k_word), 0, 0, 1, 1},
   {&__pyx_n_s_wordName, __pyx_k_wordName, sizeof(__pyx_k_wordName), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 59, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 242, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -9956,15 +9830,15 @@
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.__pyx_base.spellCheck = (struct __pyx_obj_6Corpus_8Sentence_Sentence *(*)(struct __pyx_obj_12SpellChecker_12SpellChecker_SpellChecker *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_spellCheck;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.__pyx___generateCandidateList = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker___generateCandidateList;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.candidateList = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_candidateList;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedMisspellCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedMisspellCheck;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedBackwardMergeCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedBackwardMergeCheck;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedForwardMergeCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedForwardMergeCheck;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedSplitCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedSplitCheck;
-  __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedShortcutCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck;
+  __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.forcedShortcutCheck = (int (*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_forcedShortcutCheck;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.loadDictionaries = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_loadDictionaries;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.getCorrectForm = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getCorrectForm;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.mergedCandidatesList = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_mergedCandidatesList;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.splitCandidatesList = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_splitCandidatesList;
   __pyx_vtable_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.getSplitPair = (PyObject *(*)(struct __pyx_obj_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch))__pyx_f_12SpellChecker_18SimpleSpellChecker_18SimpleSpellChecker_getSplitPair;
   __pyx_type_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker.tp_base = __pyx_ptype_12SpellChecker_12SpellChecker_SpellChecker;
   if (PyType_Ready(&__pyx_type_12SpellChecker_18SimpleSpellChecker_SimpleSpellChecker) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.pxd` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     cpdef list __generateCandidateList(self, str word)
     cpdef list candidateList(self, Word word)
     cpdef Sentence spellCheck(self, Sentence sentence)
     cpdef bint forcedMisspellCheck(self, Word word, Sentence result)
     cpdef bint forcedBackwardMergeCheck(self, Word word, Sentence result, Word previousWord)
     cpdef bint forcedForwardMergeCheck(self, Word word, Sentence result, Word nextWord)
     cpdef bint forcedSplitCheck(self, Word word, Sentence result)
-    cpdef bint forcedShortcutCheck(self, Word word, Sentence result, Word previousWord)
+    cpdef bint forcedShortcutCheck(self, Word word, Sentence result)
     cpdef loadDictionaries(self)
     cpdef str getCorrectForm(self, str wordName, dict dictionary)
     cpdef list mergedCandidatesList(self, Word previousWord, Word word, Word nextWord)
     cpdef list splitCandidatesList(self, Word word)
     cpdef tuple getSplitPair(self, Word word)
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SimpleSpellChecker.pyx` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SimpleSpellChecker.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             if self.forcedMisspellCheck(word, result) or \
                     self.forcedBackwardMergeCheck(word, result, previous_word):
                 i = i + 1
                 continue
             if self.forcedForwardMergeCheck(word, result, next_word):
                 i = i + 2
                 continue
-            if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result, previous_word):
+            if self.forcedSplitCheck(word, result) or self.forcedShortcutCheck(word, result):
                 i = i + 1
                 continue
             fsm_parse_list = self.fsm.morphologicalAnalysis(word.getName())
             if fsm_parse_list.size() == 0:
                 candidates = self.candidateList(word)
                 if len(candidates) < 1:
                     candidates.extend(self.mergedCandidatesList(previous_word, word, next_word))
@@ -217,25 +217,21 @@
         cdef str forced_replacement
         forced_replacement = self.getCorrectForm(word.getName(), self.__split_words)
         if forced_replacement != "":
             self.addSplitWords(forced_replacement, result)
             return True
         return False
 
-    cpdef bint forcedShortcutCheck(self, Word word, Sentence result, Word previousWord):
+    cpdef bint forcedShortcutCheck(self, Word word, Sentence result):
         cdef str shortcut_regex, forced_replacement
         cdef int i
         shortcut_regex = "[0-9]+(" + self.__shortcuts[0]
         for i in range(1, len(self.__shortcuts)):
             shortcut_regex = shortcut_regex + "|" + self.__shortcuts[i]
         shortcut_regex = shortcut_regex + ")"
-        compiled_expression = re.compile("[0-9]+")
-        if word.getName() in self.__shortcuts and compiled_expression.fullmatch(previousWord.getName()):
-            result.addWord(word)
-            return True
         compiled_expression = re.compile(shortcut_regex)
         if compiled_expression.fullmatch(word.getName()):
             pair = self.getSplitPair(word)
             forced_replacement = pair[0] + " " + pair[1]
             result.addWord(Word(forced_replacement))
             return True
         return False
```

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/SpellChecker/SpellChecker.c` & `NlpToolkit-SpellChecker-Cy-1.0.9/SpellChecker/SpellChecker.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-SpellChecker-Cy-1.0.8/setup.py` & `NlpToolkit-SpellChecker-Cy-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 from Cython.Build import cythonize
 
 setup(
     ext_modules=cythonize(["SpellChecker/*.pyx"],
                           compiler_directives={'language_level': "3"}),
     name='NlpToolkit-SpellChecker-Cy',
-    version='1.0.8',
+    version='1.0.9',
     packages=['SpellChecker'],
     package_data={'SpellChecker': ['*.pxd', '*.pyx', '*.c'],
                   'SpellChecker.data': ['*.txt']},
     url='https://github.com/StarlangSoftware/TurkishSpellChecker-Cy',
     license='',
     author='olcaytaner',
     author_email='olcay.yildiz@ozyegin.edu.tr',
```

