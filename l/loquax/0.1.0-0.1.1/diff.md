# Comparing `tmp/loquax-0.1.0.tar.gz` & `tmp/loquax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loquax-0.1.0.tar", last modified: Fri May 19 19:40:23 2023, max compression
+gzip compressed data, was "loquax-0.1.1.tar", last modified: Fri May 19 19:48:07 2023, max compression
```

## Comparing `loquax-0.1.0.tar` & `loquax-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.815751 loquax-0.1.0/
--rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.0/LICENSE
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1787 2023-05-19 19:40:23.815498 loquax-0.1.0/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1235 2023-05-19 19:38:53.000000 loquax-0.1.0/README.md
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.809024 loquax-0.1.0/loquax/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/__init__.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.812409 loquax-0.1.0/loquax/abstractions/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/abstractions/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/abstractions/constants.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     9273 2023-05-19 19:38:53.000000 loquax-0.1.0/loquax/abstractions/linguistic_entities.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1080 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/abstractions/phonology.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/abstractions/syllabification.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.813264 loquax-0.1.0/loquax/languages/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/languages/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/languages/latin.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.814577 loquax-0.1.0/loquax/text_processing/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/text_processing/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.0/loquax/text_processing/commons.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2758 2023-05-19 19:37:17.000000 loquax-0.1.0/loquax/text_processing/processing.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:40:23.810418 loquax-0.1.0/loquax.egg-info/
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1787 2023-05-19 19:40:23.000000 loquax-0.1.0/loquax.egg-info/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)      521 2023-05-19 19:40:23.000000 loquax-0.1.0/loquax.egg-info/SOURCES.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-19 19:40:23.000000 loquax-0.1.0/loquax.egg-info/dependency_links.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-19 19:40:23.000000 loquax-0.1.0/loquax.egg-info/top_level.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.0/pyproject.toml
--rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-19 19:40:23.815845 loquax-0.1.0/setup.cfg
--rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-19 13:53:25.000000 loquax-0.1.0/setup.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.034247 loquax-0.1.1/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.1/LICENSE
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:48:07.033959 loquax-0.1.1/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1520 2023-05-19 19:42:27.000000 loquax-0.1.1/README.md
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.025905 loquax-0.1.1/loquax/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/__init__.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.030645 loquax-0.1.1/loquax/abstractions/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/constants.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     9211 2023-05-19 19:42:43.000000 loquax-0.1.1/loquax/abstractions/linguistic_entities.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1080 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/phonology.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/syllabification.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.031658 loquax-0.1.1/loquax/languages/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/languages/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/languages/latin.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.033226 loquax-0.1.1/loquax/text_processing/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/text_processing/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/text_processing/commons.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2758 2023-05-19 19:37:17.000000 loquax-0.1.1/loquax/text_processing/processing.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.027658 loquax-0.1.1/loquax.egg-info/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      521 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/top_level.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.1/pyproject.toml
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-19 19:48:07.034341 loquax-0.1.1/setup.cfg
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-19 19:47:55.000000 loquax-0.1.1/setup.py
```

### Comparing `loquax-0.1.0/LICENSE` & `loquax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/PKG-INFO` & `loquax-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -17,21 +17,33 @@
 
 <h1 align="center">loquax</h1>
 <p align="center">
 </p>
 <p align="center">A <i><a href="https://en.wikipedia.org/wiki/Classical_antiquity" target="_blank">Classical</a></i> Phonology framework</p>
 <p align="center">
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+  <a href="https://codecov.io/gh/mattlianje/loquax" >
+    <img src="https://codecov.io/gh/mattlianje/loquax/branch/main/graph/badge.svg?token=EBMEFP40QL"/>
+  </a>
+</p>
+
+<p align="center">
+Loquax, (Latin for "chatty"), is an <b><i>extensible</i></b> Python library for analyzing and manipulating phonology of endangered & extinct languages. With hobbyists and academia in mind, it provides functionality for:
 </p>
 
-Loquax, (Latin for "chatty"), is an _**extensible**_ Python library for analyzing and manipulating phonology of endangered & extinct languages. It provides functionality for:
 
 - **Syllabification:** Break down words into their fundamental phonetic components.
 - **Phoneme Analysis:** Understand the unique sounds and their roles within words.
 - **Morphological Transformations:** Observe and manipulate the structure of words.
 - **IPA Transliteration:** Convert text into the International Phonetic Alphabet for universal comprehension.
 - **Scansion:** Analyze the rhythm of verse in classical poetry, and syllable weight in general.
 - **Extensibility:** Build and customize your own language rules for unique or theoretical languages.
 
-Loquax is a zero-dependency tool, using functional style Python 3.10+ features to revive the sounds of the past, one phoneme at a time. 
+<p align="center">
+... 
+</p>
+<p align="center">
+Its a zero-dependency framework, using functional style Python 3.10+ features to revive the sounds of the past, one phoneme at a time.
+</p>
+
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.0 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.1 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
                              ****** loquax ******
                         A Classical Phonology framework
-                              [Code_style:_black]
-Loquax, (Latin for "chatty"), is an _**extensible**_ Python library for
-analyzing and manipulating phonology of endangered & extinct languages. It
-provides functionality for: - **Syllabification:** Break down words into their
-fundamental phonetic components. - **Phoneme Analysis:** Understand the unique
-sounds and their roles within words. - **Morphological Transformations:**
-Observe and manipulate the structure of words. - **IPA Transliteration:**
-Convert text into the International Phonetic Alphabet for universal
-comprehension. - **Scansion:** Analyze the rhythm of verse in classical poetry,
-and syllable weight in general. - **Extensibility:** Build and customize your
-own language rules for unique or theoretical languages. Loquax is a zero-
-dependency tool, using functional style Python 3.10+ features to revive the
-sounds of the past, one phoneme at a time.
+[Code_style:_black] [https://codecov.io/gh/mattlianje/loquax/branch/main/graph/
+                          badge.svg?token=EBMEFP40QL]
+Loquax, (Latin for "chatty"), is an extensible Python library for analyzing and
+ manipulating phonology of endangered & extinct languages. With hobbyists and
+               academia in mind, it provides functionality for:
+- **Syllabification:** Break down words into their fundamental phonetic
+components. - **Phoneme Analysis:** Understand the unique sounds and their
+roles within words. - **Morphological Transformations:** Observe and manipulate
+the structure of words. - **IPA Transliteration:** Convert text into the
+International Phonetic Alphabet for universal comprehension. - **Scansion:**
+Analyze the rhythm of verse in classical poetry, and syllable weight in
+general. - **Extensibility:** Build and customize your own language rules for
+unique or theoretical languages.
+                                      ...
+ Its a zero-dependency framework, using functional style Python 3.10+ features
+           to revive the sounds of the past, one phoneme at a time.
```

### Comparing `loquax-0.1.0/loquax/abstractions/constants.py` & `loquax-0.1.1/loquax/abstractions/constants.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax/abstractions/linguistic_entities.py` & `loquax-0.1.1/loquax/abstractions/linguistic_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def matches(self, units: List[T]) -> bool:
         if len(units) < len(self.rules):
             return False
 
         return all(
             rule.matches(unit)
-            for rule, unit in zip(self.rules, units[-len(self.rules):])
+            for rule, unit in zip(self.rules, units[-len(self.rules) :])
         )
 
 
 @dataclass
 class Morphism(Generic[T]):
     """
     Represents a transformation applied to units in a sequence based on
@@ -71,29 +71,29 @@
     target: Rule[T]
     transformation: Union[Callable[[T], T], T]
     prefix: Optional[RuleSequence[T]] = None
     suffix: Optional[RuleSequence[T]] = None
 
     def matches(self, units: List[T], index: int) -> bool:
         return (
-                (
-                    self.prefix.matches(
-                        units[max(0, index - len(self.prefix.rules)): index]
-                    )
-                    if self.prefix
-                    else True
+            (
+                self.prefix.matches(
+                    units[max(0, index - len(self.prefix.rules)) : index]
                 )
-                and self.target.matches(units[index])
-                and (
-                    self.suffix.matches(
-                        units[index + 1: index + 1 + len(self.suffix.rules)]
-                    )
-                    if self.suffix
-                    else True
+                if self.prefix
+                else True
+            )
+            and self.target.matches(units[index])
+            and (
+                self.suffix.matches(
+                    units[index + 1 : index + 1 + len(self.suffix.rules)]
                 )
+                if self.suffix
+                else True
+            )
         )
 
     def apply(self, units: List[T]) -> List[T]:
         return [
             (
                 self.transformation(unit)
                 if callable(self.transformation)
@@ -124,25 +124,25 @@
     Represents a store for phoneme rules that are used in syllabification.
     These rules help to determine how to split a sequence of phonemes into syllables.
     """
 
     rules: List[RuleSequence["Phoneme"]]
 
     def apply_all(
-            self, phonemes: List["Phoneme"]
+        self, phonemes: List["Phoneme"]
     ) -> Tuple[List["Phoneme"], List["Phoneme"]]:
         if not phonemes:
             return [], []
 
         matching_rule = next(
             (
                 rule
                 for rule in self.rules
                 if len(rule.rules) <= len(phonemes)
-                   and rule.matches(phonemes[-len(rule.rules):])
+                and rule.matches(phonemes[-len(rule.rules) :])
             ),
             None,
         )
 
         if matching_rule is None:
             return [], []
 
@@ -271,15 +271,15 @@
             return self.phonemes[:first_vowel_index]
         return self.phonemes
 
     @property
     def coda(self) -> Optional[List[Phoneme]]:
         first_vowel_index = self._find_first_vowel_index()
         if first_vowel_index is not None:
-            return self.phonemes[first_vowel_index + 1:]
+            return self.phonemes[first_vowel_index + 1 :]
         return None
 
     @property
     def val(self) -> str:
         return "".join([phoneme.val for phoneme in self.phonemes])
 
     def _find_first_vowel_index(self) -> Optional[int]:
```

### Comparing `loquax-0.1.0/loquax/abstractions/phonology.py` & `loquax-0.1.1/loquax/abstractions/phonology.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax/abstractions/syllabification.py` & `loquax-0.1.1/loquax/abstractions/syllabification.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax/languages/latin.py` & `loquax-0.1.1/loquax/languages/latin.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax/text_processing/commons.py` & `loquax-0.1.1/loquax/text_processing/commons.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax/text_processing/processing.py` & `loquax-0.1.1/loquax/text_processing/processing.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/loquax.egg-info/PKG-INFO` & `loquax-0.1.1/loquax.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -17,21 +17,33 @@
 
 <h1 align="center">loquax</h1>
 <p align="center">
 </p>
 <p align="center">A <i><a href="https://en.wikipedia.org/wiki/Classical_antiquity" target="_blank">Classical</a></i> Phonology framework</p>
 <p align="center">
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+  <a href="https://codecov.io/gh/mattlianje/loquax" >
+    <img src="https://codecov.io/gh/mattlianje/loquax/branch/main/graph/badge.svg?token=EBMEFP40QL"/>
+  </a>
+</p>
+
+<p align="center">
+Loquax, (Latin for "chatty"), is an <b><i>extensible</i></b> Python library for analyzing and manipulating phonology of endangered & extinct languages. With hobbyists and academia in mind, it provides functionality for:
 </p>
 
-Loquax, (Latin for "chatty"), is an _**extensible**_ Python library for analyzing and manipulating phonology of endangered & extinct languages. It provides functionality for:
 
 - **Syllabification:** Break down words into their fundamental phonetic components.
 - **Phoneme Analysis:** Understand the unique sounds and their roles within words.
 - **Morphological Transformations:** Observe and manipulate the structure of words.
 - **IPA Transliteration:** Convert text into the International Phonetic Alphabet for universal comprehension.
 - **Scansion:** Analyze the rhythm of verse in classical poetry, and syllable weight in general.
 - **Extensibility:** Build and customize your own language rules for unique or theoretical languages.
 
-Loquax is a zero-dependency tool, using functional style Python 3.10+ features to revive the sounds of the past, one phoneme at a time. 
+<p align="center">
+... 
+</p>
+<p align="center">
+Its a zero-dependency framework, using functional style Python 3.10+ features to revive the sounds of the past, one phoneme at a time.
+</p>
+
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.0 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.1 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
                              ****** loquax ******
                         A Classical Phonology framework
-                              [Code_style:_black]
-Loquax, (Latin for "chatty"), is an _**extensible**_ Python library for
-analyzing and manipulating phonology of endangered & extinct languages. It
-provides functionality for: - **Syllabification:** Break down words into their
-fundamental phonetic components. - **Phoneme Analysis:** Understand the unique
-sounds and their roles within words. - **Morphological Transformations:**
-Observe and manipulate the structure of words. - **IPA Transliteration:**
-Convert text into the International Phonetic Alphabet for universal
-comprehension. - **Scansion:** Analyze the rhythm of verse in classical poetry,
-and syllable weight in general. - **Extensibility:** Build and customize your
-own language rules for unique or theoretical languages. Loquax is a zero-
-dependency tool, using functional style Python 3.10+ features to revive the
-sounds of the past, one phoneme at a time.
+[Code_style:_black] [https://codecov.io/gh/mattlianje/loquax/branch/main/graph/
+                          badge.svg?token=EBMEFP40QL]
+Loquax, (Latin for "chatty"), is an extensible Python library for analyzing and
+ manipulating phonology of endangered & extinct languages. With hobbyists and
+               academia in mind, it provides functionality for:
+- **Syllabification:** Break down words into their fundamental phonetic
+components. - **Phoneme Analysis:** Understand the unique sounds and their
+roles within words. - **Morphological Transformations:** Observe and manipulate
+the structure of words. - **IPA Transliteration:** Convert text into the
+International Phonetic Alphabet for universal comprehension. - **Scansion:**
+Analyze the rhythm of verse in classical poetry, and syllable weight in
+general. - **Extensibility:** Build and customize your own language rules for
+unique or theoretical languages.
+                                      ...
+ Its a zero-dependency framework, using functional style Python 3.10+ features
+           to revive the sounds of the past, one phoneme at a time.
```

### Comparing `loquax-0.1.0/loquax.egg-info/SOURCES.txt` & `loquax-0.1.1/loquax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loquax-0.1.0/setup.py` & `loquax-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loquax",
-    version="0.1.0",
+    version="0.1.1",
     author="Matthieu Court",
     author_email="matthieu.court@protonmail.com",
     description="A Classical Phonology framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattlianje/loquax",
     packages=find_packages(exclude=['tests', 'tests.*']),
```

