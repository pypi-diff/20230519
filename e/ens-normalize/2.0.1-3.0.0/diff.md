# Comparing `tmp/ens_normalize-2.0.1.tar.gz` & `tmp/ens_normalize-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ens_normalize-2.0.1.tar", max compression
+gzip compressed data, was "ens_normalize-3.0.0.tar", max compression
```

## Comparing `ens_normalize-2.0.1.tar` & `ens_normalize-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1110 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/LICENSE
--rw-r--r--   0        0        0    12777 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/README.md
--rw-r--r--   0        0        0      582 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/ens_normalize/__init__.py
--rw-r--r--   0        0        0    35437 2023-04-27 15:53:15.749293 ens_normalize-2.0.1/ens_normalize/normalization.py
--rw-r--r--   0        0        0  5153418 2023-04-27 15:53:15.777292 ens_normalize-2.0.1/ens_normalize/spec.pickle
--rw-r--r--   0        0        0      678 2023-04-27 15:53:15.777292 ens_normalize-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    13521 1970-01-01 00:00:00.000000 ens_normalize-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-05-19 19:26:02.034528 ens_normalize-3.0.0/LICENSE
+-rw-r--r--   0        0        0    17091 2023-05-19 19:26:02.034528 ens_normalize-3.0.0/README.md
+-rw-r--r--   0        0        0      571 2023-05-19 19:26:02.034528 ens_normalize-3.0.0/ens_normalize/__init__.py
+-rw-r--r--   0        0        0    36598 2023-05-19 19:26:02.034528 ens_normalize-3.0.0/ens_normalize/normalization.py
+-rw-r--r--   0        0        0  5153418 2023-05-19 19:26:02.054529 ens_normalize-3.0.0/ens_normalize/spec.pickle
+-rw-r--r--   0        0        0      678 2023-05-19 19:26:02.054529 ens_normalize-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17835 1970-01-01 00:00:00.000000 ens_normalize-3.0.0/PKG-INFO
```

### Comparing `ens_normalize-2.0.1/LICENSE` & `ens_normalize-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_normalize-2.0.1/README.md` & `ens_normalize-3.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,153 @@
 # ENS Normalize Python
 
 ![Tests](https://github.com/namehash/ens-normalize-python/actions/workflows/python-app.yml/badge.svg?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/ens-normalize)
 ![Coverage](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/coverage_badge.svg)
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/namehash/ens-normalize-python/blob/main/examples/notebook.ipynb)
 
 * Python implementation of the [ENS Name Normalization Standard](https://github.com/adraffy/ensip-norm/blob/main/draft.md).
-  Thanks to [Adraffy](https://github.com/adraffy) for his leadership in coordinating the definition of this standard with the ENS community.
-* Passes **100%** of the [official validation tests](https://github.com/adraffy/ens-normalize.js/tree/main/validate) (validated automatically with pytest, see below).
+  *  Thanks to [Adraffy](https://github.com/adraffy) for his leadership in coordinating the definition of this standard with the ENS community.
+  *  This library is being maintained by the team at [NameHash](https://namehash.io).
+* Passes **100%** of the [official validation tests](https://github.com/adraffy/ens-normalize.js/tree/main/validate) (validated automatically with pytest on Linux, MacOS, and Windows, see below for details).
 * Passes an [additional suite of further tests](/tools/updater/update-ens.js#L54) for compatibility with the official [Javascript reference implementation](https://github.com/adraffy/ens-normalize.js) and code testing coverage.
 * Based on [JavaScript implementation version 1.9.0](https://github.com/adraffy/ens-normalize.js/tree/4873fbe6393e970e186ab57860cc59cbbb1fa162).
 
 ## Glossary
 
-* name - a full domain name, e.g. `nick.eth`
-* label - a part of a name separated by a dot, e.g. `nick` and `eth` are labels in `nick.eth`
-* normalized name - name that is already in normalized form according to the ENS Normalization Standard
-* normalizable name - name that is normalized or that can be converted into a normalized name using `ens_normalize`
-* disallowed name - name that is not normalized or normalizable
-* curable name - name that may be disallowed but can still be converted into a normalized name using `ens_cure`
-* fatal error - a `DisallowedNameError` object thrown by `ens_normalize` that contains only general information about the error and no possible fixes
-* curable error - a `CurableError` object (inherits from `DisallowedNameError`) thrown by `ens_normalize` that contains information about a possible fix for the error
+**Foundations**
+* **sequence** - a Unicode string containing any number of characters.
+* **label separator** - a full stop character (also known as a period), e.g. `.` .
+* **label** - a sequence of any length (including 0) that does not contain a label separator, e.g.  `abc` or `eth`.
+* **name** - a series of any number of labels (including 0) separated by label separators, e.g. `abc.eth`.
+
+**Names**
+* **normalized name** - a name that is in normalized form according to the ENS Normalization Standard. This means `name == ens_normalize(name)`. A normalized name always contains at least 1 label. All labels in a normalized name always contain a sequence of at least 1 character.
+* **normalizable name** - a name that is normalized or that can be converted into a normalized name using `ens_normalize`.
+* **beautiful name** - a name that is normalizable and is equal to itself when using `ens_beautify`. This means `name == ens_beautify(name)`. For all normalizable names `ens_normalize(ens_beautify(name)) == ens_normalize(name)`.
+* **disallowed name** - a name that is not normalizable. This means `ens_normalize(name)` raises a `DisallowedSequence`.
+* **curable name** - a name that is normalizable, or a name in the subset of disallowed names that can still be converted into a normalized name using `ens_cure`.
+* **empty name** - a name that is the empty string. An empty name is disallowed and not curable.
+* **namehash ready name** - a name that is ready for for use with the ENS `namehash` function. Only normalized and empty names are namehash ready. Empty names represent the ENS namespace root for use with the ENS `namehash` function. Using the ENS `namehash` function on any name that is not namehash ready will return a node that is unreachable by ENS client applications that use a proper implementation of `ens_normalize`.
+
+**Sequences**
+* **unnormalized sequence** - a sequence from a name that is not in normalized form according to the ENS Normalization Standard.
+* **normalization suggestion** - a sequence suggested as an in-place replacement for an unnormalized sequence.
+* **normalizable sequence** - an unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_normalize` and `ens_cure`.
+* **curable sequence** - an unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_cure`.
+* **disallowed sequence** - an unnormalized sequence without any normalization suggestion.
+
+The following Venn diagram is not to scale, but may help to communicate how some of the classifications of names relate to each other conceptually.
+
+![ENS Normalize Venn Diagram](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/docs/ENS_Normalize_-_Venn_Diagram.png  "ENS Normalize Venn Diagram")
 
 ## Usage
 
 The package is available on [pypi](https://pypi.org/project/ens-normalize/)
 
 ```bash
 pip install ens-normalize
 ```
 
+You can also try it in Google Colab\
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/namehash/ens-normalize-python/blob/main/examples/notebook.ipynb)
+
 Normalize an ENS name:
 
 ```python
 from ens_normalize import ens_normalize
 # str -> str
-# raises DisallowedNameError for disallowed names
-# output ready for namehash
+# raises DisallowedSequence for disallowed names
+# output is namehash ready
 ens_normalize('Nick.ETH')
 # 'nick.eth'
-# note: does not enforce .eth TLD 3-character minimum
+# note: ens_normalize does not enforce any constraints that might be applied by a particular registrar. For example, the registrar for names that are a subname of '.eth' enforces a 3-character minimum and this constraint is not enforced by ens_normalize.
 ```
 
-Inspect issues with names that cannot be normalized:
+Inspect issues with disallowed names:
 
 ```python
-from ens_normalize import DisallowedNameError
+from ens_normalize import DisallowedSequence
 # added a hidden "zero width joiner" character
 try:
     ens_normalize('Ni‍ck.ETH')
-# Catch the first normalization error (the name we are attempting to normalize could have more than one error).
-except DisallowedNameError as e:
+# Catch the first disallowed sequence (the name we are attempting to normalize could have more than one).
+except DisallowedSequence as e:
     # error code
     print(e.code)
     # INVISIBLE
 
-    # a message about why the input is disallowed
+    # a message about why the sequence is disallowed
     print(e.general_info)
     # Contains a disallowed invisible character
 
-    if isinstance(e, CurableError):
-        # information about the disallowed substring
-        print(e.disallowed_sequence_info)
+    if isinstance(e, CurableSequence):
+        # information about the curable sequence
+        print(e.sequence_info)
         # 'This invisible character is disallowed'
 
-        # starting index of the disallowed substring in the input string
+        # starting index of the disallowed sequence in the input string
         # (counting in Unicode code points)
         print(e.index)
         # 2
 
-        # the disallowed substring
+        # the disallowed sequence
         # (use repr() to "see" the invisible character)
-        print(repr(e.disallowed))
+        print(repr(e.sequence))
         # '\u200d'
 
-        # a suggestion for fixing the first error (there might be more errors)
+        # a normalization suggestion for fixing the disallowed sequence (there might be more disallowed sequences)
         print(repr(e.suggested))
         # ''
-        # replacing the disallowed substring with this empty string represents that the disallowed substring should be removed
+        # replacing the disallowed sequence with this suggestion (an empty string) represents the idea that the disallowed sequence is suggested to be removed
 
-        # You may be able to fix this error by replacing e.disallowed
-        # with e.suggested in the input string.
-        # Fields index, disallowed_sequence_info, disallowed, and suggested are not None only for fixable errors.
-        # Other errors might be found even after applying this suggestion.
+        # You may be able to fix this disallowed sequence by replacing e.sequence with e.suggested in the input string.
+        # Fields index, sequence_info, sequence, and suggested are available only for curable errors.
+        # Other disallowed sequences might be found even after applying this suggestion.
 ```
 
-You can attempt conversion of disallowed names into normalized names:
+You can attempt conversion of disallowed names into normalized names using `ens_cure`. This algorithm can “cure” many normalization errors that would fail `ens_normalize`. This can be useful in some situations. For example, if a user input fails `ens_normalize`, a user could be prompted with a more helpful error message such as: “Did you mean curedname.eth?”.
+
+Some names are not curable. For example, if it is challenging to provide a specific normalization suggestion that might be needed to replace a disallowed sequence.
+
+Note: This function is *NOT* a part of the ENS Normalization Standard.
 
 ```python
 from ens_normalize import ens_cure
 # input name with disallowed zero width joiner and '?'
 # str -> str
 ens_cure('Ni‍ck?.ETH')
 # 'nick.eth'
 # ZWJ and '?' are removed, no error is raised
-# note: this function is not a part of the ENS Normalization Standard
 
-# note: might still raise DisallowedNameError for certain names, which cannot be cured, e.g.
+# note: might still raise DisallowedSequence for certain names, which cannot be cured, e.g.
 ens_cure('?')
-# DisallowedNameError: The name is empty
+# DisallowedSequence: No valid characters in name
+# reason: '?' would have to be removed which would result in an empty name
+
 ens_cure('0χх0.eth')
-# DisallowedNameError: Contains visually confusing characters that are disallowed
+# DisallowedSequence: Contains visually confusing characters from Cyrillic and Latin scripts
+# reason: it is not clear which character should be removed ('χ' or 'х')
 ```
 
-Format names with fully-qualified emoji:
+Get a beautiful name that is optimized for display:
 
 ```python
 from ens_normalize import ens_beautify
 # works like ens_normalize()
 # output ready for display
 ens_beautify('1⃣2⃣.eth')
 # '1️⃣2️⃣.eth'
 
 # note: normalization is unchanged:
 # ens_normalize(ens_beautify(x)) == ens_normalize(x)
-# note: in addition to beautifying emojis, ens_beautify converts the character 'ξ' (Greek lowercase 'Xi') to 'Ξ' (Greek uppercase 'Xi', a.k.a. the Ethereum symbol) in labels that contain no other Greek characters
+# note: in addition to beautifying emojis with fully-qualified emoji, ens_beautify converts the character 'ξ' (Greek lowercase 'Xi') to 'Ξ' (Greek uppercase 'Xi', a.k.a. the Ethereum symbol) in labels that contain no other Greek characters
 ```
 
-Generate detailed label analysis:
+Generate detailed name analysis:
 
 ```python
 from ens_normalize import ens_tokenize
 # str -> List[Token]
 # always returns a tokenization of the input
 ens_tokenize('Nàme‍🧙‍♂.eth')
 # [TokenMapped(cp=78, cps=[110], type='mapped'),
@@ -134,27 +161,27 @@
 #  TokenStop(cp=46, type='stop'),
 #  TokenValid(cps=[101, 116, 104], type='valid')]
 ```
 
 For a normalizable name, you can find out how the input is transformed during normalization:
 
 ```python
-from ens_normalize import ens_transformations
-# Returns a list of transformations (substring -> string)
+from ens_normalize import ens_normalizations
+# Returns a list of transformations (unnormalized sequence -> normalization suggestion)
 # that have been applied to the input during normalization.
-# NormalizationTransformation has the same fields as CurableError:
+# NormalizableSequence has the same fields as CurableSequence:
 # - code
 # - general_info
-# - disallowed_sequence_info
+# - sequence_info
 # - index
-# - disallowed
+# - sequence
 # - suggested
-ens_transformations('Nàme🧙‍♂️.eth')
-# [NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n"),
-#  NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")]
+ens_normalizations('Nàme🧙‍♂️.eth')
+# [NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n"),
+#  NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")]
 ```
 
 An example normalization workflow:
 
 ```python
 name = 'Nàme🧙‍♂️.eth'
 try:
@@ -162,94 +189,104 @@
     print('Normalized:', normalized)
     # Normalized: nàme🧙‍♂.eth
     # Success!
 
      # was the input transformed by the normalization process?
     if name != normalized:
         # Let's check how the input was changed:
-        for t in ens_transformations(name):
+        for t in ens_normalizations(name):
             print(repr(t)) # use repr() to print more information
-        # NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n")
-        # NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")
-        #                              invisible character inside emoji ^
-except DisallowedNameError as e:
+        # NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n")
+        # NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")
+        #                                     invisible character inside emoji ^
+except DisallowedSequence as e:
     # Even if the name is invalid according to the ENS Normalization Standard,
-    # we can try to automatically remove disallowed characters.
+    # we can try to automatically cure disallowed sequences.
     try:
-        print(ens_cure(name))
-    except DisallowedLabelError as e:
-        # The name cannot be automatically fixed.
-        print('Fatal error:', e)
+        print('Cured:', ens_cure(name))
+    except DisallowedSequence as e:
+        # The name cannot be automatically cured.
+        print('Disallowed name error:', e)
 ```
 
 You can run many of the above functions at once. It is faster than running all of them sequentially.
 
 ```python
 from ens_normalize import ens_process
 # use only the do_* flags you need
 ens_process("Nàme🧙‍♂️1⃣.eth",
     do_normalize=True,
     do_beautify=True,
     do_tokenize=True,
-    do_transformations=True,
+    do_normalizations=True,
     do_cure=True,
 )
 # ENSProcessResult(
 #   normalized='nàme🧙\u200d♂1⃣.eth',
 #   beautified='nàme🧙\u200d♂️1️⃣.eth',
 #   tokens=[...],
 #   cured='nàme🧙\u200d♂1⃣.eth',
 #   cures=[], # This is the list of cures that were applied to the input (in this case, none).
 #   error=None, # This is the exception raised by ens_normalize().
-#               # It is a DisallowedNameError or CurableError if the error is curable.
-#   transformations=[
-#     NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n"),
-#     NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")
+#               # It is a DisallowedSequence or CurableSequence if the error is curable.
+#   normalizations=[
+#     NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n"),
+#     NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")
 #   ])
 ```
 
-## List of all `DisallowedNameError` types
+## Exceptions
 
-For fatal errors (not curable), it is challenging to communicate the normalization error as a problem with a specific substring.
+These Python classes are used by the library to communicate information about unnormalized sequences.
 
-| `DisallowedNameErrorType` | General info |
-| ------------------------- | ------------ |
-| `EMPTY_NAME`   | The name is empty |
-| `NSM_REPEATED` | Contains a repeated non-spacing mark |
-| `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
-| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
+| Exception class               |  `ens_normalize` handling  | `ens_cure` handling       | normalization<br>suggestion  | Inherits From         |
+|-------------------------------|----------------------------|---------------------------|------------------------------|-----------------------|
+| `NormalizableSequence`        |  ✅ automatically resolves | ✅ automatically resolves | ✅ included                  | `CurableSequence`     |
+| `CurableSequence`             |  ❌ throws error           | ✅ automatically resolves | ✅ included                  | `DisallowedSequence`  |
+| `DisallowedSequence`          |  ❌ throws error           | ❌ throws error           | ❌ none                      | `Exception`           |
 
-## List of all `CurableError` types
+### List of all `NormalizableSequence` types
 
-Curable errors contain additional information about the disallowed substring.
+| `NormalizableSequenceType` | General info | Sequence info |
+| --------------------------------- | ------------ | ------------------------ |
+| `IGNORED`    | Contains a disallowed "ignored" character that has been removed | This character is ignored during normalization and has been automatically removed |
+| `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
+| `FE0F`       | Contains a disallowed variant of an emoji which has been replaced by an equivalent normalized emoji | This emoji has been automatically fixed to remove an invisible character |
+| `NFC`        | Contains a disallowed sequence that is not "NFC normalized" which has been replaced by an equivalent normalized sequence | This sequence has been automatically normalized into NFC canonical form |
+
+### List of all `CurableSequence` types
+
+Curable errors contain additional information about the disallowed sequence and a normalization suggestion that might help to cure the name.
 
-| `CurableErrorType` | General info | Disallowed sequence info |
+| `CurableSequenceType` | General info | Sequence info |
 | ------------------ | ------------ | ------------------------ |
 | `UNDERSCORE`  | Contains an underscore in a disallowed position | An underscore is only allowed at the start of a label |
 | `HYPHEN`      | Contains the sequence '--' in a disallowed position | Hyphens are disallowed at the 2nd and 3rd positions of a label |
 | `EMPTY_LABEL` | Contains a disallowed empty label | Empty labels are not allowed, e.g. abc..eth |
 | `CM_START`    | Contains a combining mark in a disallowed position at the start of the label | A combining mark is disallowed at the start of a label |
 | `CM_EMOJI`    | Contains a combining mark in a disallowed position after an emoji | A combining mark is disallowed after an emoji |
 | `DISALLOWED`  | Contains a disallowed character | This character is disallowed |
 | `INVISIBLE`   | Contains a disallowed invisible character | This invisible character is disallowed |
 | `FENCED_LEADING`  | Contains a disallowed character at the start of a label | This character is disallowed at the start of a label |
 | `FENCED_MULTI`    | Contains a disallowed consecutive sequence of characters | Characters in this sequence cannot be placed next to each other |
 | `FENCED_TRAILING` | Contains a disallowed character at the end of a label | This character is disallowed at the end of a label |
 | `CONF_MIXED` | Contains visually confusing characters from multiple scripts ({script1}/{script2}) | This character from the {script1} script is disallowed because it is visually confusing with another character from the {script2} script |
 
-## List of all normalization transformations
+### List of all `DisallowedSequence` types
 
-| `NormalizationTransformationType` | General info | Disallowed sequence info |
-| --------------------------------- | ------------ | ------------------------ |
-| `IGNORED`    | Contains disallowed "ignored" characters that have been removed | This character is ignored during normalization and has been automatically removed |
-| `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
-| `FE0F`       | Contains a disallowed variant of an emoji which has been replaced by an equivalent normalized emoji | This emoji has been automatically fixed to remove an invisible character |
-| `NFC`        | Contains a disallowed sequence that is not "NFC normalized" which has been replaced by an equivalent normalized sequence | This sequence has been automatically normalized into NFC canonical form |
+Disallowed name errors are not considered curable because it may be challenging to suggest a specific normalization suggestion that might resolve the problem.
+
+| `DisallowedSequenceType` | General info |
+| ------------------------- | ------------ |
+| `EMPTY_NAME`   | No valid characters in name |
+| `NSM_REPEATED` | Contains a repeated non-spacing mark |
+| `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
+| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
 
-## Develop
+## Development
 
 ### Update this library to the latest ENS normalization specification *(optional)*
 
 This library uses files defining the normalization standard
 directly from the [official Javascript implementation](https://github.com/adraffy/ens-normalize.js/tree/main/derive).
 When the standard is updated with new characters, this library can
 be updated by running the following steps:
```

### Comparing `ens_normalize-2.0.1/ens_normalize/__init__.py` & `ens_normalize-3.0.0/ens_normalize/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .normalization import (
     ens_process,
     ens_normalize,
     ens_cure,
     ens_beautify,
     ens_tokenize,
-    ens_transformations,
+    ens_normalizations,
     is_ens_normalized,
-    DisallowedNameError,
-    DisallowedNameErrorType,
-    CurableError,
-    CurableErrorType,
-    NormalizationTransformation,
-    NormalizationTransformationType,
+    DisallowedSequence,
+    DisallowedSequenceType,
+    CurableSequence,
+    CurableSequenceType,
+    NormalizableSequence,
+    NormalizableSequenceType,
     TY_VALID,
     TY_MAPPED,
     TY_IGNORED,
     TY_DISALLOWED,
     TY_EMOJI,
     TY_STOP,
     TY_NFC,
```

### Comparing `ens_normalize-2.0.1/ens_normalize/normalization.py` & `ens_normalize-3.0.0/ens_normalize/normalization.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,68 +7,80 @@
 from pyunormalize import NFC, NFD, UNICODE_VERSION
 import warnings
 
 
 SPEC_PICKLE_PATH = os.path.join(os.path.dirname(__file__), 'spec.pickle')
 
 
-class ErrorTypeBase(Enum):
+class DisallowedSequenceTypeBase(Enum):
+    '''
+    Base class for disallowed sequence types.
+    See README: Glossary -> Sequences.
+    '''
+
     def __new__(cls, *args):
         value = len(cls.__members__) + 1
         obj = object.__new__(cls)
         obj._value_ = value
         return obj
 
     def __init__(self, general_info: str):
         self.general_info = general_info
 
     @property
     def code(self) -> str:
         return self.name
 
 
-class CurableErrorTypeBase(Enum):
+class CurableSequenceTypeBase(Enum):
+    '''
+    Base class for curable sequence types.
+    See README: Glossary -> Sequences.
+    '''
+
     def __new__(cls, *args):
         value = len(cls.__members__) + 1
         obj = object.__new__(cls)
         obj._value_ = value
         return obj
 
-    def __init__(self, general_info: str, disallowed_sequence_info: str):
+    def __init__(self, general_info: str, sequence_info: str):
         self.general_info = general_info
-        self.disallowed_sequence_info = disallowed_sequence_info
+        self.sequence_info = sequence_info
 
     @property
     def code(self) -> str:
         return self.name
 
 
-class DisallowedNameErrorType(ErrorTypeBase):
+class DisallowedSequenceType(DisallowedSequenceTypeBase):
     """
-    The name is disallowed and cannot be normalized.
+    The type of a disallowed sequence.
+    See README: Glossary -> Sequences.
     """
 
     # GENERIC ----------------
 
-    EMPTY_NAME = "The name is empty"
+    EMPTY_NAME = "No valid characters in name"
 
     # NSM --------------------
 
     NSM_REPEATED = "Contains a repeated non-spacing mark"
 
     NSM_TOO_MANY = "Contains too many consecutive non-spacing marks"
 
     # CONFUSABLES ----------
 
     CONF_WHOLE = "Contains visually confusing characters from {script1} and {script2} scripts"
 
 
-class CurableErrorType(CurableErrorTypeBase):
+class CurableSequenceType(CurableSequenceTypeBase):
     """
-    The name is disallowed but a cure is available.
+    The type of a curable sequence.
+    See README: Glossary -> Sequences.
     """
 
     # GENERIC ----------------
 
     UNDERSCORE = "Contains an underscore in a disallowed position", \
                  "An underscore is only allowed at the start of a label"
 
@@ -107,17 +119,18 @@
 
     # CONFUSABLES ----------
 
     CONF_MIXED = "Contains visually confusing characters from multiple scripts ({scripts})", \
                  "This character{script1} is disallowed because it is visually confusing with another character{script2}"
 
 
-class NormalizationTransformationType(CurableErrorTypeBase):
+class NormalizableSequenceType(CurableSequenceTypeBase):
     """
-    The label is allowed but contains a sequence which has been automatically transformed into a normalized form.
+    The type of a normalizable sequence.
+    See README: Glossary -> Sequences.
     """
 
     IGNORED   = "Contains disallowed \"ignored\" characters that have been removed", \
                 "This character is ignored during normalization and has been automatically removed"
 
     MAPPED    = "Contains a disallowed character that has been replaced by a normalized sequence", \
                 "This character is disallowed and has been automatically replaced by a normalized sequence"
@@ -125,16 +138,21 @@
     FE0F      = "Contains a disallowed variant of an emoji which has been replaced by an equivalent normalized emoji", \
                 "This emoji has been automatically fixed to remove an invisible character"
 
     NFC       = "Contains a disallowed sequence that is not \"NFC normalized\" which has been replaced by an equivalent normalized sequence", \
                 "This sequence has been automatically normalized into NFC canonical form"
 
 
-class DisallowedNameError(Exception):
-    def __init__(self, type: DisallowedNameErrorType, meta: Dict[str, str] = {}):
+class DisallowedSequence(Exception):
+    '''
+    An unnormalized sequence without any normalization suggestion.
+    See README: Glossary -> Sequences.
+    '''
+
+    def __init__(self, type: DisallowedSequenceType, meta: Dict[str, str] = {}):
         super().__init__(type.general_info)
         self.type = type
         self.meta = meta
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(code="{self.type.code}")'
 
@@ -152,50 +170,60 @@
     def general_info(self) -> str:
         """
         Information about the entire name.
         """
         return self.type.general_info.format(**self.meta)
 
 
-class CurableError(DisallowedNameError):
+class CurableSequence(DisallowedSequence):
+    '''
+    An unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_cure`.
+    See README: Glossary -> Sequences.
+    '''
+
     def __init__(self,
-                 type: CurableErrorType,
+                 type: CurableSequenceType,
                  index: int,
-                 disallowed: str,
+                 sequence: str,
                  suggested: str,
                  meta: Dict[str, str] = {}):
         super().__init__(type, meta)
         self.type = type
         self.index = index
-        self.disallowed = disallowed
+        self.sequence = sequence
         self.suggested = suggested
 
     def __repr__(self) -> str:
-        return f'{self.__class__.__name__}(code="{self.type.code}", index={self.index}, disallowed="{self.disallowed}", suggested="{self.suggested}")'
+        return f'{self.__class__.__name__}(code="{self.type.code}", index={self.index}, sequence="{self.sequence}", suggested="{self.suggested}")'
 
     @property
-    def disallowed_sequence_info(self) -> str:
+    def sequence_info(self) -> str:
         """
         Information about the disallowed sequence.
         """
-        return self.type.disallowed_sequence_info.format(
-            disallowed=self.disallowed,
+        return self.type.sequence_info.format(
+            sequence=self.sequence,
             suggested=self.suggested,
             **self.meta,
         )
 
 
-class NormalizationTransformation(CurableError):
+class NormalizableSequence(CurableSequence):
+    '''
+    An unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_normalize` and `ens_cure`.
+    See README: Glossary -> Sequences.
+    '''
+
     def __init__(self,
-                 type: NormalizationTransformationType,
+                 type: NormalizableSequenceType,
                  index: int,
-                 disallowed: str,
+                 sequence: str,
                  suggested: str,
                  meta: Dict[str, str] = {}):
-        super().__init__(type, index, disallowed, suggested, meta)
+        super().__init__(type, index, sequence, suggested, meta)
         self.type = type
 
 
 TY_VALID = 'valid'
 TY_MAPPED = 'mapped'
 TY_IGNORED = 'ignored'
 TY_DISALLOWED = 'disallowed'
@@ -264,17 +292,17 @@
 
 
 class ENSProcessResult(NamedTuple):
     normalized: Optional[str]
     beautified: Optional[str]
     tokens: Optional[List[Token]]
     cured: Optional[str]
-    cures: Optional[List[CurableError]]
-    error: Optional[DisallowedNameError]
-    transformations: Optional[List[NormalizationTransformation]]
+    cures: Optional[List[CurableSequence]]
+    error: Optional[DisallowedSequence]
+    normalizations: Optional[List[NormalizableSequence]]
 
 
 def str2cps(text: str) -> List[int]:
     """
     Convert text to a list of integer codepoints.
     """
     return [ord(c) for c in text]
@@ -338,22 +366,28 @@
     """
     Create a lookup table for recreating FE0F emojis from non-FE0F emojis.
     """
     return {filter_fe0f(emoji): emoji for emoji in emojis}
 
 
 def compute_valid(groups: List[Dict]) -> Set[int]:
+    '''
+    Compute the set of valid codepoints from the spec.json file.
+    '''
     valid = set()
     for g in groups:
         valid.update(g['V'])
     valid.update(map(ord, NFD(''.join(map(chr, valid)))))
     return valid
 
 
 def read_groups(groups: List[Dict]) -> List[Dict]:
+    '''
+    Read and parse the groups field from the spec.json file.
+    '''
     return [
         {
             'name': g['name'],
             'P': set(g['primary']),
             'Q': set(g['secondary']),
             'V': set(g['primary'] + g['secondary']),
             'M': 'cm' not in g,
@@ -366,26 +400,35 @@
     try:
         return int(x)
     except ValueError:
         return x
 
 
 def dict_keys_to_int(d):
+    '''
+    Recursively convert dictionary keys to integers (for JSON parsing).
+    '''
     if isinstance(d, dict):
         return {try_str_to_int(k): dict_keys_to_int(v) for k, v in d.items()}
     return d
 
 
 def find_group_id(groups, name):
+    '''
+    Find the index of a group by name.
+    '''
     for i, g in enumerate(groups):
         if g['name'] == name:
             return i
 
 
 def group_names_to_ids(groups, whole_map):
+    '''
+    Convert group names to group ids in the whole_map for faster lookup.
+    '''
     for v in whole_map.values():
         if isinstance(v, dict):
             for k in v['M']:
                 for i in range(len(v['M'][k])):
                     id = find_group_id(groups, v['M'][k][i])
                     assert id is not None
                     v['M'][k][i] = id
@@ -502,109 +545,109 @@
                 start = i
         elif token.type != TY_IGNORED:
             start = -1
         i += 1
     return collapse_valid_tokens(tokens)
 
 
-def post_check_empty(name: str) -> Optional[Union[DisallowedNameError, CurableError]]:
+def post_check_empty(name: str) -> Optional[Union[DisallowedSequence, CurableSequence]]:
     if len(name) == 0:
-        return DisallowedNameError(DisallowedNameErrorType.EMPTY_NAME)
+        return DisallowedSequence(DisallowedSequenceType.EMPTY_NAME)
     if name[0] == '.':
-        return CurableError(
-            CurableErrorType.EMPTY_LABEL,
+        return CurableSequence(
+            CurableSequenceType.EMPTY_LABEL,
             index=0,
-            disallowed='.',
+            sequence='.',
             suggested='',
         )
     if name[-1] == '.':
-        return CurableError(
-            CurableErrorType.EMPTY_LABEL,
+        return CurableSequence(
+            CurableSequenceType.EMPTY_LABEL,
             index=len(name) - 1,
-            disallowed='.',
+            sequence='.',
             suggested='',
         )
     i = name.find('..')
     if i >= 0:
-        return CurableError(
-            CurableErrorType.EMPTY_LABEL,
+        return CurableSequence(
+            CurableSequenceType.EMPTY_LABEL,
             index=i,
-            disallowed='..',
+            sequence='..',
             suggested='.',
         )
 
 
-def post_check_underscore(label: str) -> Optional[CurableError]:
+def post_check_underscore(label: str) -> Optional[CurableSequence]:
     in_middle = False
     for i, c in enumerate(label):
         if c != '_':
             in_middle = True
         elif in_middle:
             cnt = 1
             while i + cnt < len(label) and label[i + cnt] == '_':
                 cnt += 1
-            return CurableError(
-                CurableErrorType.UNDERSCORE,
+            return CurableSequence(
+                CurableSequenceType.UNDERSCORE,
                 index=i,
-                disallowed='_' * cnt,
+                sequence='_' * cnt,
                 suggested='',
             )
 
 
-def post_check_hyphen(label: str) -> Optional[CurableError]:
+def post_check_hyphen(label: str) -> Optional[CurableSequence]:
     if len(label) >= 4 and all(ord(cp) < 0x80 for cp in label) and '-' == label[2] == label[3]:
-        return CurableError(
-            CurableErrorType.HYPHEN,
+        return CurableSequence(
+            CurableSequenceType.HYPHEN,
             index=2,
-            disallowed='--',
+            sequence='--',
             suggested='',
         )
 
 
-def post_check_cm_leading_emoji(cps: List[int]) -> Optional[CurableError]:
+def post_check_cm_leading_emoji(cps: List[int]) -> Optional[CurableSequence]:
     for i in range(len(cps)):
         if cps[i] in NORMALIZATION.cm:
             if i == 0:
-                return CurableError(
-                    CurableErrorType.CM_START,
+                return CurableSequence(
+                    CurableSequenceType.CM_START,
                     index=i,
-                    disallowed=chr(cps[i]),
+                    sequence=chr(cps[i]),
                     suggested='',
                 )
             else:
                 prev = cps[i - 1]
                 # emojis were replaced with FE0F
                 if prev == CP_FE0F:
-                    return CurableError(
-                        CurableErrorType.CM_EMOJI,
+                    return CurableSequence(
+                        CurableSequenceType.CM_EMOJI,
                         # we cannot report the emoji because it was replaced with FE0F
                         index=i,
-                        disallowed=chr(cps[i]),
+                        sequence=chr(cps[i]),
                         suggested='',
                     )
 
 
-def make_fenced_error(cps: List[int], start: int, end: int) -> CurableError:
+def make_fenced_error(cps: List[int], start: int, end: int) -> CurableSequence:
     suggested = ''
     if start == 0:
-        type_ = CurableErrorType.FENCED_LEADING
+        type_ = CurableSequenceType.FENCED_LEADING
     elif end == len(cps):
-        type_ = CurableErrorType.FENCED_TRAILING
+        type_ = CurableSequenceType.FENCED_TRAILING
     else:
-        type_ = CurableErrorType.FENCED_MULTI
+        type_ = CurableSequenceType.FENCED_MULTI
         suggested = chr(cps[start])
-    return CurableError(
+    return CurableSequence(
         type_,
         index=start,
-        disallowed=''.join(map(chr, cps[start:end])),
+        sequence=''.join(map(chr, cps[start:end])),
         suggested=suggested,
     )
 
 
-def post_check_fenced(cps: List[int]) -> Optional[CurableError]:
+def post_check_fenced(cps: List[int]) -> Optional[CurableSequence]:
     cp = cps[0]
     prev = NORMALIZATION.fenced.get(cp)
     if prev is not None:
         return make_fenced_error(cps, 0, 1)
 
     n = len(cps)
     last = -1
@@ -616,15 +659,15 @@
                 return make_fenced_error(cps, i - 1, i + 1)
             last = i + 1
 
     if last == n:
         return make_fenced_error(cps, n - 1, n)
 
 
-def post_check_group_whole(cps: List[int], is_greek: List[bool]) -> Optional[Union[DisallowedNameError, CurableError]]:
+def post_check_group_whole(cps: List[int], is_greek: List[bool]) -> Optional[Union[DisallowedSequence, CurableSequence]]:
     cps_no_fe0f = [cp for cp in cps if cp != CP_FE0F]
     unique = set(cps_no_fe0f)
     # we pass cps with fe0f to align error position with the original input
     g, e = determine_group(unique, cps)
     if e is not None:
         return e
     g = g[0]
@@ -633,14 +676,17 @@
     return (
         post_check_group(g, cps_no_fe0f, cps)
         or post_check_whole(g, unique)
     )
 
 
 def meta_for_conf_mixed(g, cp):
+    '''
+    Create metadata for the CONF_MIXED error.
+    '''
     s1 = [g['name'] for g in NORMALIZATION.groups if cp in g['V']]
     s1 = s1[0] if s1 else None
     s2 = g['name']
     if s1 is not None:
         return {
             'scripts': f'{s1}/{s2}',
             'script1': f' from the {s1} script',
@@ -650,72 +696,71 @@
         return {
             'scripts': f'{s2} plus other scripts',
             'script1': '',
             'script2': f' from the {s2} script',
         }
 
 
-def determine_group(unique: Iterable[int], cps: List[int]) -> Tuple[Optional[List[Dict]], Optional[CurableError]]:
+def determine_group(unique: Iterable[int], cps: List[int]) -> Tuple[Optional[List[Dict]], Optional[CurableSequence]]:
     groups = NORMALIZATION.groups
     for cp in unique:
         gs = [g for g in groups if cp in g['V']]
         if len(gs) == 0:
             if groups == NORMALIZATION.groups:
-                return None, CurableError(
-                    CurableErrorType.DISALLOWED,
+                return None, CurableSequence(
+                    CurableSequenceType.DISALLOWED,
                     index=cps.index(cp),
-                    disallowed=chr(cp),
+                    sequence=chr(cp),
                     suggested='',
                 )
             else:
-                return None, CurableError(
-                    CurableErrorType.CONF_MIXED,
+                return None, CurableSequence(
+                    CurableSequenceType.CONF_MIXED,
                     index=cps.index(cp),
-                    disallowed=chr(cp),
+                    sequence=chr(cp),
                     suggested='',
                     meta=meta_for_conf_mixed(groups[0], cp),
                 )
         groups = gs
         if len(groups) == 1:
             break
     return groups, None
 
 
-def post_check_group(g, cps: List[int], input: List[int]) -> Optional[Union[DisallowedNameError, CurableError]]:
+def post_check_group(g, cps: List[int], input: List[int]) -> Optional[Union[DisallowedSequence, CurableSequence]]:
     v, m = g['V'], g['M']
     for cp in cps:
         if cp not in v:
-            return CurableError(
-                CurableErrorType.CONF_MIXED,
+            return CurableSequence(
+                CurableSequenceType.CONF_MIXED,
                 index=input.index(cp),
-                disallowed=chr(cp),
+                sequence=chr(cp),
                 suggested='',
                 meta=meta_for_conf_mixed(g, cp),
             )
     if m:
         decomposed = str2cps(NFD(cps2str(cps)))
         i = 1
         e = len(decomposed)
         while i < e:
             if decomposed[i] in NORMALIZATION.nsm:
                 j = i + 1
                 while j < e and decomposed[j] in NORMALIZATION.nsm:
                     if j - i + 1 > NORMALIZATION.nsm_max:
-                        return DisallowedNameError(DisallowedNameErrorType.NSM_TOO_MANY)
+                        return DisallowedSequence(DisallowedSequenceType.NSM_TOO_MANY)
                     for k in range(i, j):
                         if decomposed[k] == decomposed[j]:
-                            return DisallowedNameError(DisallowedNameErrorType.NSM_REPEATED)
+                            return DisallowedSequence(DisallowedSequenceType.NSM_REPEATED)
                     j += 1
                 i = j
             i += 1
 
 
-def post_check_whole(group, cps: Iterable[int]) -> Optional[DisallowedNameError]:
+def post_check_whole(group, cps: Iterable[int]) -> Optional[DisallowedSequence]:
     # Cannot report error index, operating on unique codepoints.
-    # Not reporting disallowed sequence, see below.
     maker = None
     shared = []
     for cp in cps:
         whole = NORMALIZATION.whole_map.get(cp)
         if whole == 1:
             return None
         if whole is not None:
@@ -728,24 +773,24 @@
                 return None
         else:
             shared.append(cp)
     if maker is not None:
         for g_ind in maker:
             g = NORMALIZATION.groups[g_ind]
             if all(cp in g['V'] for cp in shared):
-                return DisallowedNameError(
-                    DisallowedNameErrorType.CONF_WHOLE,
+                return DisallowedSequence(
+                    DisallowedSequenceType.CONF_WHOLE,
                     meta={
                         'script1': group['name'],
                         'script2': g['name'],
                     },
                 )
 
 
-def post_check(name: str, label_is_greek: List[bool]) -> Optional[Union[DisallowedNameError, CurableError]]:
+def post_check(name: str, label_is_greek: List[bool]) -> Optional[Union[DisallowedSequence, CurableSequence]]:
     # name has emojis replaced with a single FE0F
     e = post_check_empty(name)
     if e is not None:
         return e
     label_offset = 0
     for label in name.split('.'):
         # will be set inside post_check_group_whole
@@ -758,56 +803,56 @@
             or post_check_fenced(cps)
             or post_check_group_whole(cps, is_greek)
         )
         # was this label greek?
         label_is_greek.append(is_greek[0])
         if e is not None:
             # post_checks are called on a single label and need an offset
-            if isinstance(e, CurableError):
+            if isinstance(e, CurableSequence): # or NormalizableSequence because of inheritance
                 e.index = label_offset + e.index if e.index is not None else None
             return e
         label_offset += len(label) + 1
 
     return None
 
 
-def find_normalization_transformations(tokens: List[Token]) -> List[NormalizationTransformation]:
+def find_normalizations(tokens: List[Token]) -> List[NormalizableSequence]:
     warnings = []
     warning = None
     start = 0
     disallowed = None
     suggestion = None
     for tok in tokens:
         if tok.type == TY_MAPPED:
-            warning = NormalizationTransformationType.MAPPED
+            warning = NormalizableSequenceType.MAPPED
             disallowed = chr(tok.cp)
             suggestion = cps2str(tok.cps)
             scanned = 1
         elif tok.type == TY_IGNORED:
-            warning = NormalizationTransformationType.IGNORED
+            warning = NormalizableSequenceType.IGNORED
             disallowed = chr(tok.cp)
             suggestion = ''
             scanned = 1
         elif tok.type == TY_EMOJI:
             if tok.input != tok.cps:
-                warning = NormalizationTransformationType.FE0F
+                warning = NormalizableSequenceType.FE0F
                 disallowed = cps2str(tok.input)
                 suggestion = cps2str(tok.cps)
             scanned = len(tok.input)
         elif tok.type == TY_NFC:
-            warning = NormalizationTransformationType.NFC
+            warning = NormalizableSequenceType.NFC
             disallowed = cps2str(tok.input)
             suggestion = cps2str(tok.cps)
             scanned = len(tok.input)
         elif tok.type == TY_VALID:
             scanned = len(tok.cps)
         else:  # TY_STOP
             scanned = 1
         if warning is not None:
-            warnings.append(NormalizationTransformation(warning, start, disallowed, suggestion))
+            warnings.append(NormalizableSequence(warning, start, disallowed, suggestion))
             warning = None
         start += scanned
     return warnings
 
 
 def tokens2str(tokens: List[Token], emoji_fn: Callable[[TokenEmoji], str] = lambda tok: cps2str(tok.cps)) -> str:
     t = []
@@ -852,35 +897,35 @@
     return ''.join(s)
 
 
 def ens_process(input: str,
                 do_normalize: bool = False,
                 do_beautify: bool = False,
                 do_tokenize: bool = False,
-                do_transformations: bool = False,
+                do_normalizations: bool = False,
                 do_cure: bool = False) -> ENSProcessResult:
     """
     Used to compute
 
     - `ens_normalize`
     - `ens_beautify`
     - `ens_tokenize`
-    - `ens_transformations`
+    - `ens_normalizations`
     - `ens_cure`
 
     in one go.
 
     Returns `ENSProcessResult` with the following fields:
     - `normalized`: normalized name or `None` if input cannot be normalized or `do_normalize` is `False`
     - `beautified`: beautified name or `None` if input cannot be normalized or `do_beautify` is `False`
     - `tokens`: list of `Token` objects or `None` if `do_tokenize` is `False`
     - `cured`: cured name or `None` if input cannot be cured or `do_cure` is `False`
-    - `cures`: list of fixed `CurableError` objects or `None` if input cannot be cured or `do_cure` is `False`
-    - `error`: `DisallowedNameError` or `CurableError` or `None` if input is valid
-    - `transformations`: list of `NormalizationTransformation` objects or `None` if `do_transformations` is `False`
+    - `cures`: list of fixed `CurableSequence` objects or `None` if input cannot be cured or `do_cure` is `False`
+    - `error`: `DisallowedSequence` or `CurableSequence` or `None` if input is valid
+    - `normalizations`: list of `NormalizableSequence` objects or `None` if `do_normalizations` is `False`
     """
     tokens: List[Token] = []
     error = None
 
     input_cur = 0
     emoji_iter = NORMALIZATION.emoji_regex.finditer(input)
     next_emoji_match = next(emoji_iter, None)
@@ -933,39 +978,39 @@
         if mapping is not None:
             tokens.append(TokenMapped(
                 cp = cp,
                 cps = mapping,
             ))
             continue
 
-        error = error or CurableError(
-            CurableErrorType.INVISIBLE
+        error = error or CurableSequence(
+            CurableSequenceType.INVISIBLE
             if c in ('\u200d', '\u200c')
-            else CurableErrorType.DISALLOWED,
+            else CurableSequenceType.DISALLOWED,
             index=input_cur - 1,
-            disallowed=c,
+            sequence=c,
             suggested='',
         )
 
         tokens.append(TokenDisallowed(
             cp = cp,
         ))
 
     tokens = normalize_tokens(tokens)
 
-    transformations = find_normalization_transformations(tokens) if do_transformations else None
+    normalizations = find_normalizations(tokens) if do_normalizations else None
 
     if error is None:
         # run post checks
         emojis_as_fe0f = ''.join(tokens2str(tokens, lambda _: '\uFE0F'))
         # true for each label that is greek
         # will be set by post_check()
         label_is_greek = []
         error = post_check(emojis_as_fe0f, label_is_greek)
-        if isinstance(error, CurableError):
+        if isinstance(error, CurableSequence): # or NormalizableSequence because of inheritance
             offset_err_start(error, tokens)
 
     # else:
         # only the result of post_check() is not input aligned
         # so we do not offset the error set by the input scanning loop
 
     if error is not None:
@@ -979,29 +1024,29 @@
     tokens = tokens if do_tokenize else None
 
     cured = None
     cures = None
     if do_cure:
         try:
             cured, cures = _ens_cure(input)
-        except DisallowedNameError:
+        except DisallowedSequence:
             pass
 
     return ENSProcessResult(
         normalized,
         beautified,
         tokens,
         cured,
         cures,
         error,
-        transformations,
+        normalizations,
     )
 
 
-def offset_err_start(err: Optional[CurableError], tokens: List[Token]):
+def offset_err_start(err: Optional[CurableSequence], tokens: List[Token]):
     """
     Output of post_check() is not input aligned.
     This function offsets the error index (in-place) to match the input characters.
     """
     # index in string that was scanned
     i = 0
     # offset between input and scanned
@@ -1034,54 +1079,54 @@
     err.index += offset
 
 
 def ens_normalize(text: str) -> str:
     """
     Apply ENS normalization to a string.
 
-    Raises DisallowedNameError if the input cannot be normalized.
+    Raises DisallowedSequence if the input cannot be normalized.
     """
     res = ens_process(text, do_normalize=True)
     if res.error is not None:
         raise res.error
     return res.normalized
 
 
-def _ens_cure(text: str) -> Tuple[str, List[CurableError]]:
+def _ens_cure(text: str) -> Tuple[str, List[CurableSequence]]:
     cures = []
     # Protect against infinite loops.
     # The assumption is that n iterations are enough to cure the input (2n just in case).
-    # +1 is for the last iteration that should raise DisallowedNameError.
+    # +1 is for the last iteration that should raise DisallowedSequence.
     # All cures currently implemented remove a character so this assumption seems reasonable.
     for _ in range(2 * len(text) + 1):
         try:
             return ens_normalize(text), cures
-        except CurableError as e:
-            text = text[:e.index] + e.suggested + text[e.index + len(e.disallowed):]
+        except CurableSequence as e:
+            text = text[:e.index] + e.suggested + text[e.index + len(e.sequence):]
             cures.append(e)
-        # DisallowedNameError is not caught here because it is not curable
+        # DisallowedSequence is not caught here because it is not curable
     # this should never happen
-    raise Exception('ens_cure() exceeded max iterations. Please report this as a bug.')
+    raise Exception('ens_cure() exceeded max iterations. Please report this as a bug along with the input string.')
 
 
 def ens_cure(text: str) -> str:
     """
     Apply ENS normalization to a string. If the result is not normalized then this function
     will try to make the input normalized by removing all disallowed characters.
 
-    Raises `DisallowedNameError` if one is encountered and cannot be cured.
+    Raises `DisallowedSequence` if one is encountered and cannot be cured.
     """
     return _ens_cure(text)[0]
 
 
 def ens_beautify(text: str) -> str:
     """
     Apply ENS normalization with beautification to a string.
 
-    Raises DisallowedNameError if the input cannot be normalized.
+    Raises DisallowedSequence if the input cannot be normalized.
     """
     res = ens_process(text, do_beautify=True)
     if res.error is not None:
         raise res.error
     return res.beautified
 
 
@@ -1113,25 +1158,25 @@
     - nfc
         - input: input codepoints
         - cps: output codepoints (after NFC normalization)
     """
     return ens_process(input, do_tokenize=True).tokens
 
 
-def ens_transformations(input: str) -> List[NormalizationTransformation]:
+def ens_normalizations(input: str) -> List[NormalizableSequence]:
     """
-    This function returns a list of `NormalizationTransformation` objects
+    This function returns a list of `NormalizableSequence` objects
     that describe the modifications applied by ENS normalization to the input string.
 
-    Raises DisallowedNameError if the input cannot be normalized.
+    Raises DisallowedSequence if the input cannot be normalized.
     """
-    res = ens_process(input, do_transformations=True)
+    res = ens_process(input, do_normalizations=True)
     if res.error is not None:
         raise res.error
-    return res.transformations
+    return res.normalizations
 
 
 def is_ens_normalized(name: str) -> bool:
     """
     Checks if the input string is already ENS normalized
     (i.e. `ens_normalize(name) == name`).
     """
```

### Comparing `ens_normalize-2.0.1/ens_normalize/spec.pickle` & `ens_normalize-3.0.0/ens_normalize/spec.pickle`

 * *Files identical despite different names*

### Comparing `ens_normalize-2.0.1/pyproject.toml` & `ens_normalize-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ens-normalize"
-version = "2.0.1"
+version = "3.0.0"
 description = "Ethereum Name Service (ENS) Name Normalizer"
 license = "MIT"
 authors = ["Jakub Karbowski <jakub@namehash.io>"]
 maintainers = ["NameHash Team <devops@namehash.io>"]
 homepage = "https://github.com/namehash/ens-normalize-python"
 repository = "https://github.com/namehash/ens-normalize-python"
 readme = "README.md"
```

### Comparing `ens_normalize-2.0.1/PKG-INFO` & `ens_normalize-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ens-normalize
-Version: 2.0.1
+Version: 3.0.0
 Summary: Ethereum Name Service (ENS) Name Normalizer
 Home-page: https://github.com/namehash/ens-normalize-python
 License: MIT
 Author: Jakub Karbowski
 Author-email: jakub@namehash.io
 Maintainer: NameHash Team
 Maintainer-email: devops@namehash.io
@@ -19,128 +19,155 @@
 Description-Content-Type: text/markdown
 
 # ENS Normalize Python
 
 ![Tests](https://github.com/namehash/ens-normalize-python/actions/workflows/python-app.yml/badge.svg?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/ens-normalize)
 ![Coverage](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/coverage_badge.svg)
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/namehash/ens-normalize-python/blob/main/examples/notebook.ipynb)
 
 * Python implementation of the [ENS Name Normalization Standard](https://github.com/adraffy/ensip-norm/blob/main/draft.md).
-  Thanks to [Adraffy](https://github.com/adraffy) for his leadership in coordinating the definition of this standard with the ENS community.
-* Passes **100%** of the [official validation tests](https://github.com/adraffy/ens-normalize.js/tree/main/validate) (validated automatically with pytest, see below).
+  *  Thanks to [Adraffy](https://github.com/adraffy) for his leadership in coordinating the definition of this standard with the ENS community.
+  *  This library is being maintained by the team at [NameHash](https://namehash.io).
+* Passes **100%** of the [official validation tests](https://github.com/adraffy/ens-normalize.js/tree/main/validate) (validated automatically with pytest on Linux, MacOS, and Windows, see below for details).
 * Passes an [additional suite of further tests](/tools/updater/update-ens.js#L54) for compatibility with the official [Javascript reference implementation](https://github.com/adraffy/ens-normalize.js) and code testing coverage.
 * Based on [JavaScript implementation version 1.9.0](https://github.com/adraffy/ens-normalize.js/tree/4873fbe6393e970e186ab57860cc59cbbb1fa162).
 
 ## Glossary
 
-* name - a full domain name, e.g. `nick.eth`
-* label - a part of a name separated by a dot, e.g. `nick` and `eth` are labels in `nick.eth`
-* normalized name - name that is already in normalized form according to the ENS Normalization Standard
-* normalizable name - name that is normalized or that can be converted into a normalized name using `ens_normalize`
-* disallowed name - name that is not normalized or normalizable
-* curable name - name that may be disallowed but can still be converted into a normalized name using `ens_cure`
-* fatal error - a `DisallowedNameError` object thrown by `ens_normalize` that contains only general information about the error and no possible fixes
-* curable error - a `CurableError` object (inherits from `DisallowedNameError`) thrown by `ens_normalize` that contains information about a possible fix for the error
+**Foundations**
+* **sequence** - a Unicode string containing any number of characters.
+* **label separator** - a full stop character (also known as a period), e.g. `.` .
+* **label** - a sequence of any length (including 0) that does not contain a label separator, e.g.  `abc` or `eth`.
+* **name** - a series of any number of labels (including 0) separated by label separators, e.g. `abc.eth`.
+
+**Names**
+* **normalized name** - a name that is in normalized form according to the ENS Normalization Standard. This means `name == ens_normalize(name)`. A normalized name always contains at least 1 label. All labels in a normalized name always contain a sequence of at least 1 character.
+* **normalizable name** - a name that is normalized or that can be converted into a normalized name using `ens_normalize`.
+* **beautiful name** - a name that is normalizable and is equal to itself when using `ens_beautify`. This means `name == ens_beautify(name)`. For all normalizable names `ens_normalize(ens_beautify(name)) == ens_normalize(name)`.
+* **disallowed name** - a name that is not normalizable. This means `ens_normalize(name)` raises a `DisallowedSequence`.
+* **curable name** - a name that is normalizable, or a name in the subset of disallowed names that can still be converted into a normalized name using `ens_cure`.
+* **empty name** - a name that is the empty string. An empty name is disallowed and not curable.
+* **namehash ready name** - a name that is ready for for use with the ENS `namehash` function. Only normalized and empty names are namehash ready. Empty names represent the ENS namespace root for use with the ENS `namehash` function. Using the ENS `namehash` function on any name that is not namehash ready will return a node that is unreachable by ENS client applications that use a proper implementation of `ens_normalize`.
+
+**Sequences**
+* **unnormalized sequence** - a sequence from a name that is not in normalized form according to the ENS Normalization Standard.
+* **normalization suggestion** - a sequence suggested as an in-place replacement for an unnormalized sequence.
+* **normalizable sequence** - an unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_normalize` and `ens_cure`.
+* **curable sequence** - an unnormalized sequence containing a normalization suggestion that is automatically applied using `ens_cure`.
+* **disallowed sequence** - an unnormalized sequence without any normalization suggestion.
+
+The following Venn diagram is not to scale, but may help to communicate how some of the classifications of names relate to each other conceptually.
+
+![ENS Normalize Venn Diagram](https://raw.githubusercontent.com/namehash/ens-normalize-python/main/docs/ENS_Normalize_-_Venn_Diagram.png  "ENS Normalize Venn Diagram")
 
 ## Usage
 
 The package is available on [pypi](https://pypi.org/project/ens-normalize/)
 
 ```bash
 pip install ens-normalize
 ```
 
+You can also try it in Google Colab\
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/namehash/ens-normalize-python/blob/main/examples/notebook.ipynb)
+
 Normalize an ENS name:
 
 ```python
 from ens_normalize import ens_normalize
 # str -> str
-# raises DisallowedNameError for disallowed names
-# output ready for namehash
+# raises DisallowedSequence for disallowed names
+# output is namehash ready
 ens_normalize('Nick.ETH')
 # 'nick.eth'
-# note: does not enforce .eth TLD 3-character minimum
+# note: ens_normalize does not enforce any constraints that might be applied by a particular registrar. For example, the registrar for names that are a subname of '.eth' enforces a 3-character minimum and this constraint is not enforced by ens_normalize.
 ```
 
-Inspect issues with names that cannot be normalized:
+Inspect issues with disallowed names:
 
 ```python
-from ens_normalize import DisallowedNameError
+from ens_normalize import DisallowedSequence
 # added a hidden "zero width joiner" character
 try:
     ens_normalize('Ni‍ck.ETH')
-# Catch the first normalization error (the name we are attempting to normalize could have more than one error).
-except DisallowedNameError as e:
+# Catch the first disallowed sequence (the name we are attempting to normalize could have more than one).
+except DisallowedSequence as e:
     # error code
     print(e.code)
     # INVISIBLE
 
-    # a message about why the input is disallowed
+    # a message about why the sequence is disallowed
     print(e.general_info)
     # Contains a disallowed invisible character
 
-    if isinstance(e, CurableError):
-        # information about the disallowed substring
-        print(e.disallowed_sequence_info)
+    if isinstance(e, CurableSequence):
+        # information about the curable sequence
+        print(e.sequence_info)
         # 'This invisible character is disallowed'
 
-        # starting index of the disallowed substring in the input string
+        # starting index of the disallowed sequence in the input string
         # (counting in Unicode code points)
         print(e.index)
         # 2
 
-        # the disallowed substring
+        # the disallowed sequence
         # (use repr() to "see" the invisible character)
-        print(repr(e.disallowed))
+        print(repr(e.sequence))
         # '\u200d'
 
-        # a suggestion for fixing the first error (there might be more errors)
+        # a normalization suggestion for fixing the disallowed sequence (there might be more disallowed sequences)
         print(repr(e.suggested))
         # ''
-        # replacing the disallowed substring with this empty string represents that the disallowed substring should be removed
+        # replacing the disallowed sequence with this suggestion (an empty string) represents the idea that the disallowed sequence is suggested to be removed
 
-        # You may be able to fix this error by replacing e.disallowed
-        # with e.suggested in the input string.
-        # Fields index, disallowed_sequence_info, disallowed, and suggested are not None only for fixable errors.
-        # Other errors might be found even after applying this suggestion.
+        # You may be able to fix this disallowed sequence by replacing e.sequence with e.suggested in the input string.
+        # Fields index, sequence_info, sequence, and suggested are available only for curable errors.
+        # Other disallowed sequences might be found even after applying this suggestion.
 ```
 
-You can attempt conversion of disallowed names into normalized names:
+You can attempt conversion of disallowed names into normalized names using `ens_cure`. This algorithm can “cure” many normalization errors that would fail `ens_normalize`. This can be useful in some situations. For example, if a user input fails `ens_normalize`, a user could be prompted with a more helpful error message such as: “Did you mean curedname.eth?”.
+
+Some names are not curable. For example, if it is challenging to provide a specific normalization suggestion that might be needed to replace a disallowed sequence.
+
+Note: This function is *NOT* a part of the ENS Normalization Standard.
 
 ```python
 from ens_normalize import ens_cure
 # input name with disallowed zero width joiner and '?'
 # str -> str
 ens_cure('Ni‍ck?.ETH')
 # 'nick.eth'
 # ZWJ and '?' are removed, no error is raised
-# note: this function is not a part of the ENS Normalization Standard
 
-# note: might still raise DisallowedNameError for certain names, which cannot be cured, e.g.
+# note: might still raise DisallowedSequence for certain names, which cannot be cured, e.g.
 ens_cure('?')
-# DisallowedNameError: The name is empty
+# DisallowedSequence: No valid characters in name
+# reason: '?' would have to be removed which would result in an empty name
+
 ens_cure('0χх0.eth')
-# DisallowedNameError: Contains visually confusing characters that are disallowed
+# DisallowedSequence: Contains visually confusing characters from Cyrillic and Latin scripts
+# reason: it is not clear which character should be removed ('χ' or 'х')
 ```
 
-Format names with fully-qualified emoji:
+Get a beautiful name that is optimized for display:
 
 ```python
 from ens_normalize import ens_beautify
 # works like ens_normalize()
 # output ready for display
 ens_beautify('1⃣2⃣.eth')
 # '1️⃣2️⃣.eth'
 
 # note: normalization is unchanged:
 # ens_normalize(ens_beautify(x)) == ens_normalize(x)
-# note: in addition to beautifying emojis, ens_beautify converts the character 'ξ' (Greek lowercase 'Xi') to 'Ξ' (Greek uppercase 'Xi', a.k.a. the Ethereum symbol) in labels that contain no other Greek characters
+# note: in addition to beautifying emojis with fully-qualified emoji, ens_beautify converts the character 'ξ' (Greek lowercase 'Xi') to 'Ξ' (Greek uppercase 'Xi', a.k.a. the Ethereum symbol) in labels that contain no other Greek characters
 ```
 
-Generate detailed label analysis:
+Generate detailed name analysis:
 
 ```python
 from ens_normalize import ens_tokenize
 # str -> List[Token]
 # always returns a tokenization of the input
 ens_tokenize('Nàme‍🧙‍♂.eth')
 # [TokenMapped(cp=78, cps=[110], type='mapped'),
@@ -154,27 +181,27 @@
 #  TokenStop(cp=46, type='stop'),
 #  TokenValid(cps=[101, 116, 104], type='valid')]
 ```
 
 For a normalizable name, you can find out how the input is transformed during normalization:
 
 ```python
-from ens_normalize import ens_transformations
-# Returns a list of transformations (substring -> string)
+from ens_normalize import ens_normalizations
+# Returns a list of transformations (unnormalized sequence -> normalization suggestion)
 # that have been applied to the input during normalization.
-# NormalizationTransformation has the same fields as CurableError:
+# NormalizableSequence has the same fields as CurableSequence:
 # - code
 # - general_info
-# - disallowed_sequence_info
+# - sequence_info
 # - index
-# - disallowed
+# - sequence
 # - suggested
-ens_transformations('Nàme🧙‍♂️.eth')
-# [NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n"),
-#  NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")]
+ens_normalizations('Nàme🧙‍♂️.eth')
+# [NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n"),
+#  NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")]
 ```
 
 An example normalization workflow:
 
 ```python
 name = 'Nàme🧙‍♂️.eth'
 try:
@@ -182,94 +209,104 @@
     print('Normalized:', normalized)
     # Normalized: nàme🧙‍♂.eth
     # Success!
 
      # was the input transformed by the normalization process?
     if name != normalized:
         # Let's check how the input was changed:
-        for t in ens_transformations(name):
+        for t in ens_normalizations(name):
             print(repr(t)) # use repr() to print more information
-        # NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n")
-        # NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")
-        #                              invisible character inside emoji ^
-except DisallowedNameError as e:
+        # NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n")
+        # NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")
+        #                                     invisible character inside emoji ^
+except DisallowedSequence as e:
     # Even if the name is invalid according to the ENS Normalization Standard,
-    # we can try to automatically remove disallowed characters.
+    # we can try to automatically cure disallowed sequences.
     try:
-        print(ens_cure(name))
-    except DisallowedLabelError as e:
-        # The name cannot be automatically fixed.
-        print('Fatal error:', e)
+        print('Cured:', ens_cure(name))
+    except DisallowedSequence as e:
+        # The name cannot be automatically cured.
+        print('Disallowed name error:', e)
 ```
 
 You can run many of the above functions at once. It is faster than running all of them sequentially.
 
 ```python
 from ens_normalize import ens_process
 # use only the do_* flags you need
 ens_process("Nàme🧙‍♂️1⃣.eth",
     do_normalize=True,
     do_beautify=True,
     do_tokenize=True,
-    do_transformations=True,
+    do_normalizations=True,
     do_cure=True,
 )
 # ENSProcessResult(
 #   normalized='nàme🧙\u200d♂1⃣.eth',
 #   beautified='nàme🧙\u200d♂️1️⃣.eth',
 #   tokens=[...],
 #   cured='nàme🧙\u200d♂1⃣.eth',
 #   cures=[], # This is the list of cures that were applied to the input (in this case, none).
 #   error=None, # This is the exception raised by ens_normalize().
-#               # It is a DisallowedNameError or CurableError if the error is curable.
-#   transformations=[
-#     NormalizationTransformation(code="MAPPED", index=0, disallowed="N", suggested="n"),
-#     NormalizationTransformation(code="FE0F", index=4, disallowed="🧙‍♂️", suggested="🧙‍♂")
+#               # It is a DisallowedSequence or CurableSequence if the error is curable.
+#   normalizations=[
+#     NormalizableSequence(code="MAPPED", index=0, sequence="N", suggested="n"),
+#     NormalizableSequence(code="FE0F", index=4, sequence="🧙‍♂️", suggested="🧙‍♂")
 #   ])
 ```
 
-## List of all `DisallowedNameError` types
+## Exceptions
 
-For fatal errors (not curable), it is challenging to communicate the normalization error as a problem with a specific substring.
+These Python classes are used by the library to communicate information about unnormalized sequences.
 
-| `DisallowedNameErrorType` | General info |
-| ------------------------- | ------------ |
-| `EMPTY_NAME`   | The name is empty |
-| `NSM_REPEATED` | Contains a repeated non-spacing mark |
-| `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
-| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
+| Exception class               |  `ens_normalize` handling  | `ens_cure` handling       | normalization<br>suggestion  | Inherits From         |
+|-------------------------------|----------------------------|---------------------------|------------------------------|-----------------------|
+| `NormalizableSequence`        |  ✅ automatically resolves | ✅ automatically resolves | ✅ included                  | `CurableSequence`     |
+| `CurableSequence`             |  ❌ throws error           | ✅ automatically resolves | ✅ included                  | `DisallowedSequence`  |
+| `DisallowedSequence`          |  ❌ throws error           | ❌ throws error           | ❌ none                      | `Exception`           |
 
-## List of all `CurableError` types
+### List of all `NormalizableSequence` types
 
-Curable errors contain additional information about the disallowed substring.
+| `NormalizableSequenceType` | General info | Sequence info |
+| --------------------------------- | ------------ | ------------------------ |
+| `IGNORED`    | Contains a disallowed "ignored" character that has been removed | This character is ignored during normalization and has been automatically removed |
+| `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
+| `FE0F`       | Contains a disallowed variant of an emoji which has been replaced by an equivalent normalized emoji | This emoji has been automatically fixed to remove an invisible character |
+| `NFC`        | Contains a disallowed sequence that is not "NFC normalized" which has been replaced by an equivalent normalized sequence | This sequence has been automatically normalized into NFC canonical form |
+
+### List of all `CurableSequence` types
+
+Curable errors contain additional information about the disallowed sequence and a normalization suggestion that might help to cure the name.
 
-| `CurableErrorType` | General info | Disallowed sequence info |
+| `CurableSequenceType` | General info | Sequence info |
 | ------------------ | ------------ | ------------------------ |
 | `UNDERSCORE`  | Contains an underscore in a disallowed position | An underscore is only allowed at the start of a label |
 | `HYPHEN`      | Contains the sequence '--' in a disallowed position | Hyphens are disallowed at the 2nd and 3rd positions of a label |
 | `EMPTY_LABEL` | Contains a disallowed empty label | Empty labels are not allowed, e.g. abc..eth |
 | `CM_START`    | Contains a combining mark in a disallowed position at the start of the label | A combining mark is disallowed at the start of a label |
 | `CM_EMOJI`    | Contains a combining mark in a disallowed position after an emoji | A combining mark is disallowed after an emoji |
 | `DISALLOWED`  | Contains a disallowed character | This character is disallowed |
 | `INVISIBLE`   | Contains a disallowed invisible character | This invisible character is disallowed |
 | `FENCED_LEADING`  | Contains a disallowed character at the start of a label | This character is disallowed at the start of a label |
 | `FENCED_MULTI`    | Contains a disallowed consecutive sequence of characters | Characters in this sequence cannot be placed next to each other |
 | `FENCED_TRAILING` | Contains a disallowed character at the end of a label | This character is disallowed at the end of a label |
 | `CONF_MIXED` | Contains visually confusing characters from multiple scripts ({script1}/{script2}) | This character from the {script1} script is disallowed because it is visually confusing with another character from the {script2} script |
 
-## List of all normalization transformations
+### List of all `DisallowedSequence` types
 
-| `NormalizationTransformationType` | General info | Disallowed sequence info |
-| --------------------------------- | ------------ | ------------------------ |
-| `IGNORED`    | Contains disallowed "ignored" characters that have been removed | This character is ignored during normalization and has been automatically removed |
-| `MAPPED`     | Contains a disallowed character that has been replaced by a normalized sequence | This character is disallowed and has been automatically replaced by a normalized sequence |
-| `FE0F`       | Contains a disallowed variant of an emoji which has been replaced by an equivalent normalized emoji | This emoji has been automatically fixed to remove an invisible character |
-| `NFC`        | Contains a disallowed sequence that is not "NFC normalized" which has been replaced by an equivalent normalized sequence | This sequence has been automatically normalized into NFC canonical form |
+Disallowed name errors are not considered curable because it may be challenging to suggest a specific normalization suggestion that might resolve the problem.
+
+| `DisallowedSequenceType` | General info |
+| ------------------------- | ------------ |
+| `EMPTY_NAME`   | No valid characters in name |
+| `NSM_REPEATED` | Contains a repeated non-spacing mark |
+| `NSM_TOO_MANY` | Contains too many consecutive non-spacing marks |
+| `CONF_WHOLE` | Contains visually confusing characters from {script1} and {script2} scripts |
 
-## Develop
+## Development
 
 ### Update this library to the latest ENS normalization specification *(optional)*
 
 This library uses files defining the normalization standard
 directly from the [official Javascript implementation](https://github.com/adraffy/ens-normalize.js/tree/main/derive).
 When the standard is updated with new characters, this library can
 be updated by running the following steps:
```

