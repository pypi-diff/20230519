# Comparing `tmp/big-0.8.tar.gz` & `tmp/big-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "big-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `big-0.8.tar` & `big-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.8/.gitignore
--rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.8/LICENSE
--rw-r--r--   0        0        0   142096 2023-05-18 12:33:28.374029 big-0.8/README.md
--rw-r--r--   0        0        0     1240 2023-05-18 12:31:45.441153 big-0.8/big/__init__.py
--rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.8/big/all.py
--rw-r--r--   0        0        0     5705 2023-04-12 21:51:57.504191 big-0.8/big/boundinnerclass.py
--rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.8/big/builtin.py
--rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.8/big/file.py
--rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.8/big/graph.py
--rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.8/big/heap.py
--rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.8/big/itertools.py
--rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.8/big/scheduler.py
--rw-r--r--   0        0        0    95441 2023-05-18 12:28:37.491552 big-0.8/big/text.py
--rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.8/big/time.py
--rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.8/pyproject.toml
--rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.8/requirements.txt
--rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.8/resources/experiments/alice.in.wonderland.txt
--rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.8/resources/experiments/time_multisplit.py
--rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.8/resources/images/big.header.png
--rw-r--r--   0        0        0     2692 2023-04-12 21:51:57.504191 big-0.8/test/bigtestlib.py
--rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.8/test/grepfile
--rw-r--r--   0        0        0     1422 2023-04-12 21:51:57.504191 big-0.8/test/test_all.py
--rw-r--r--   0        0        0     5847 2023-04-12 21:51:57.504191 big-0.8/test/test_boundinnerclass.py
--rw-r--r--   0        0        0     6486 2023-04-12 21:51:57.504191 big-0.8/test/test_builtin.py
--rw-r--r--   0        0        0     8332 2023-04-12 21:51:57.504191 big-0.8/test/test_file.py
--rw-r--r--   0        0        0    12302 2023-04-12 21:51:57.504191 big-0.8/test/test_graph.py
--rw-r--r--   0        0        0     4978 2023-04-12 21:51:57.504191 big-0.8/test/test_heap.py
--rw-r--r--   0        0        0     3373 2023-04-12 21:51:57.504191 big-0.8/test/test_itertools.py
--rw-r--r--   0        0        0    11445 2023-04-12 21:51:57.504191 big-0.8/test/test_scheduler.py
--rw-r--r--   0        0        0   111989 2023-05-18 11:26:19.367687 big-0.8/test/test_text.py
--rw-r--r--   0        0        0     6069 2023-04-12 21:51:57.508190 big-0.8/test/test_time.py
--rw-r--r--   0        0        0   142699 1970-01-01 00:00:00.000000 big-0.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.8.1/LICENSE
+-rw-r--r--   0        0        0   144602 2023-05-19 13:23:04.978639 big-0.8.1/README.md
+-rw-r--r--   0        0        0     1242 2023-05-19 13:20:37.349392 big-0.8.1/big/__init__.py
+-rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.8.1/big/all.py
+-rw-r--r--   0        0        0     5705 2023-04-12 21:51:57.504191 big-0.8.1/big/boundinnerclass.py
+-rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.8.1/big/builtin.py
+-rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.8.1/big/file.py
+-rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.8.1/big/graph.py
+-rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.8.1/big/heap.py
+-rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.8.1/big/itertools.py
+-rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.8.1/big/scheduler.py
+-rw-r--r--   0        0        0   103073 2023-05-19 13:20:16.529216 big-0.8.1/big/text.py
+-rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.8.1/big/time.py
+-rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.8.1/requirements.txt
+-rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.8.1/resources/experiments/alice.in.wonderland.txt
+-rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.8.1/resources/experiments/time_multisplit.py
+-rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.8.1/resources/images/big.header.png
+-rw-r--r--   0        0        0     2692 2023-04-12 21:51:57.504191 big-0.8.1/test/bigtestlib.py
+-rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.8.1/test/grepfile
+-rw-r--r--   0        0        0     1422 2023-04-12 21:51:57.504191 big-0.8.1/test/test_all.py
+-rw-r--r--   0        0        0     5847 2023-04-12 21:51:57.504191 big-0.8.1/test/test_boundinnerclass.py
+-rw-r--r--   0        0        0     6486 2023-04-12 21:51:57.504191 big-0.8.1/test/test_builtin.py
+-rw-r--r--   0        0        0     8332 2023-04-12 21:51:57.504191 big-0.8.1/test/test_file.py
+-rw-r--r--   0        0        0    12302 2023-04-12 21:51:57.504191 big-0.8.1/test/test_graph.py
+-rw-r--r--   0        0        0     4978 2023-04-12 21:51:57.504191 big-0.8.1/test/test_heap.py
+-rw-r--r--   0        0        0     3373 2023-04-12 21:51:57.504191 big-0.8.1/test/test_itertools.py
+-rw-r--r--   0        0        0    11445 2023-04-12 21:51:57.504191 big-0.8.1/test/test_scheduler.py
+-rw-r--r--   0        0        0   115680 2023-05-19 13:19:51.149002 big-0.8.1/test/test_text.py
+-rw-r--r--   0        0        0     6069 2023-04-12 21:51:57.508190 big-0.8.1/test/test_time.py
+-rw-r--r--   0        0        0   145207 1970-01-01 00:00:00.000000 big-0.8.1/PKG-INFO
```

### Comparing `big-0.8/LICENSE` & `big-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `big-0.8/README.md` & `big-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 
 [`big.time`](#bigtime)
 
 [`BoundInnerClass`](#boundinnerclasscls)
 
 [`CycleError`](#cycleerror)
 
+[`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+
 [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone)
 
 [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone)
 
 [`Event(scheduler, event, time, priority, sequence)`](#eventscheduler-event-time-priority-sequence)
 
 [`Event.cancel()`](#eventcancel)
@@ -173,14 +175,16 @@
 
 [`newlines`](#newlines)
 
 [`newlines_without_dos`](#newlines)
 
 [`normalize_whitespace(s, separators=None, replacement=None)`](#normalize_whitespaces-separatorsNone-replacementnone)
 
+[`parse_delimiters(s, delimiters=None)`](#parse_delimiterss-delimitersNone)
+
 [`parse_timestamp_3339Z(s, *, timezone=None)`](#parse_timestamp_3339zs--timezonenone)
 
 [`PushbackIterator(iterable=None)`](#pushbackiteratoriterablenone)
 
 [`PushbackIterator.next(default=None)`](#pushbackiteratornextdefaultnone)
 
 [`PushbackIterator.push(o)`](#pushbackiteratorpusho)
@@ -1038,14 +1042,28 @@
 These functions will check that all such arguments
 are of the same type.
 
 Subclasses of `str` and `bytes` will also work; anywhere you
 should pass in a `str`, you can also pass in a subclass of
 `str`, and likewise for `bytes`.
 
+#### `Delimiter(open, close, *, backslash=False, nested=True)`
+
+> Class representing a delimiter for
+> [`parse_delimiters(s, delimiters=None)`.](#parse_delimiterss-delimitersNone)
+>
+> `open` is the opening delimiter character, can be `str` or `bytes`, must be length 1.
+>
+> `close` is the closing delimiter character, must be the same type as `open`, and length 1.
+>
+> `backslash` is a boolean: when inside this delimiter, can you escape delimiters
+> with a backslash?  (You usually can inside single or double quotes.)
+>
+> `nested` is a boolean: must other delimiters nest in this delimiter?
+> (Delimiters don't usually need to be nested inside single and double quotes.)
 
 #### `gently_title(s, *, apostrophes=None, double_quotes=None)`
 
 > Uppercase the first character of every word in `s`.
 > Leave the other letters alone.  s should be `str` or `bytes`.
 >
 > (For the purposes of this algorithm, words are
@@ -1589,14 +1607,50 @@
 > a replacement string consisting of a single space character.
 >
 > Leading or trailing runs of separator characters will
 > be replaced with the replacement string, e.g.:
 >
 >     normalize_whitespace("   a    b   c") == " a b c"
 
+#### `parse_delimiters(s, delimiters=None)`
+
+> Parses a string containing nesting delimiters.
+> Raises an exception if mismatched delimiters are detected.
+>
+> `s` may be `str` or `bytes`.
+>
+> `delimiters` may be either `None` or an iterable containing
+> either
+> [`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+> objects or objects matching `s` (`str` or `bytes`).
+> Entries in the `delimiters` iterable which are `str` or `bytes`
+> should be exactly two characters long; these will be used
+> as the `open` and `close` arguments for a new `Delimiter` object.
+>
+> If `delimiters` is `None`, `parse_delimiters` uses a default
+> value matching these pairs of delimiters:
+>
+>     () [] {} "" ''
+>
+> The quote mark delimiters enable backslash quoting and disable nesting.
+>
+> Yields 3-tuples containing strings:
+>     (text, open, close)
+> where `text` is the text before the next opening or closing delimiter,
+> `open` is the trailing opening delimiter,
+> and `close` is the trailing closing delimiter.
+> At least one of these three strings will always be non-empty.
+> If `open` is non-empty, `close` will be empty, and vice-versa.
+> If `s` does not end with a closing delimiter, in the final tuple
+> yielded, both `open` and `close` will be empty strings.
+>
+> You can only specify a particular character as an opening delimiter
+> once, though you may reuse a particular character as a closing
+> delimiter multiple times.
+
 #### `re_partition(text, pattern, count=1, *, flags=0, reverse=False)`
 
 > Like `str.partition`, but `pattern` is matched as a regular expression.
 >
 > `text` can be a string or a bytes object.
 >
 > `pattern` can be a string, bytes, or `re.Pattern` object.
@@ -3284,14 +3338,21 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
+**0.8.1**
+
+* Added
+  [`parse_delimiters`](#parse_delimiterss-delimitersNone)
+  and
+  [`Delimiter(open, close, *, backslash=False, nested=True)`.](delimiteropen-close--backslash-nested)
+
 **0.8**
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
     for how it works.
```

### Comparing `big-0.8/big/__init__.py` & `big-0.8.1/big/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-__version__ = "0.8"
+__version__ = "0.8.1"
```

### Comparing `big-0.8/big/all.py` & `big-0.8.1/big/all.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/boundinnerclass.py` & `big-0.8.1/big/boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/builtin.py` & `big-0.8.1/big/builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/file.py` & `big-0.8.1/big/file.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/graph.py` & `big-0.8.1/big/graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/heap.py` & `big-0.8.1/big/heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/itertools.py` & `big-0.8.1/big/itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/scheduler.py` & `big-0.8.1/big/scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8/big/text.py` & `big-0.8.1/big/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1607,14 +1607,238 @@
 
     # flush the remainder of the string we were building,
     # in whatever condition it's in.
     if text:
         yield in_quote, empty_join(text)
 
 
+
+
+@_export
+class Delimiter:
+    """
+    Class representing a delimiter for parse_delimiters.
+
+    open is the opening delimiter character, can be str or bytes, must be length 1.
+    close is the closing delimiter character, must be the same type as open, and length 1.
+    backslash is a boolean: when inside this delimiter, can you escape delimiters
+       with a backslash?  (You usually can inside single or double quotes.)
+    nested is a boolean: must other delimiters nest in this delimiter?
+       (Delimiters don't usually need to be nested inside single and double quotes.)
+    """
+    def __init__(self, open, close, *, backslash=False, nested=True):
+        if isinstance(open, bytes):
+            t = bytes
+        else:
+            t = str
+        if not (isinstance(open, t) and isinstance(close, t)):
+            raise TypeError(f"open={open!r} and close={close!r}, they must be the same type, either str or bytes")
+
+        self.open = open
+        self.close = close
+        self.backslash = backslash
+        self.nested = nested
+
+    def __repr__(self):
+        return f"Delimiter(open={self.open!r}, close={self.close!r}, backslash={self.backslash}, nested={self.nested})"
+
+delimiter_parentheses = "()"
+_export_name('delimiter_parentheses')
+
+delimiter_square_brackets = "[]"
+_export_name('delimiter_square_brackets')
+
+delimiter_curly_braces = "{}"
+_export_name('delimiter_curly_braces')
+
+delimiter_angle_brackets = "<>"
+_export_name('delimiter_angle_brackets')
+
+delimiter_single_quote = Delimiter("'", "'", backslash=True, nested=False)
+_export_name('delimiter_single_quote')
+
+delimiter_double_quotes = Delimiter('"', '"', backslash=True, nested=False)
+_export_name('delimiter_double_quotes')
+
+parse_delimiters_default_delimiters = (
+    delimiter_parentheses,
+    delimiter_square_brackets,
+    delimiter_curly_braces,
+    delimiter_single_quote,
+    delimiter_double_quotes,
+    )
+_export_name('parse_delimiters_default_delimiters')
+
+parse_delimiters_default_delimiters_bytes = (
+    b'()',
+    b'[]',
+    b'{}',
+    Delimiter(b"'", b"'", backslash=True, nested=False),
+    Delimiter(b'"', b'"', backslash=True, nested=False),
+    )
+_export_name('parse_delimiters_default_delimiters_bytes')
+
+
+# break the rules
+_base_delimiter = Delimiter('a', 'b')
+_base_delimiter.open = _base_delimiter.close = None
+
+@_export
+def parse_delimiters(s, delimiters=None):
+    """
+    Parses a string containing nesting delimiters.
+    Raises an exception if mismatched delimiters are detected.
+
+    s may be str or bytes.
+
+    delimiters may be either None or an iterable containing
+    either Delimiter objects or objects matching s (str or bytes).
+    Entries in the delimiters iterable which are str or bytes
+    should be exactly two characters long; these will be used
+    as the open and close arguments for a new Delimiter object.
+
+    If delimiters is None, parse_delimiters uses a default
+    value matching these pairs of delimiters:
+        () [] {} "" ''
+    The quote mark delimiters enable backslash quoting and disable nesting.
+
+    Yields 3-tuples containing strings:
+        (text, open, close)
+    where text is the text before the next opening or closing delimiter,
+    open is the trailing opening delimiter,
+    and close is the trailing closing delimiter.
+    At least one of these three strings will always be non-empty.
+    If open is non-empty, close will be empty, and vice-versa.
+    If s does not end with a closing delimiter, in the final tuple
+    yielded, both open and close will be empty strings.
+
+    You can only specify a particular character as an opening delimiter
+    once, though you may reuse a particular character as a closing
+    delimiter multiple times.
+    """
+    if isinstance(s, bytes):
+        s_type = bytes
+        if delimiters is None:
+            delimiters = parse_delimiters_default_delimiters_bytes
+        backslash_character = b'\\'
+        disallowed_delimiters = backslash_character
+        empty = b''
+    else:
+        s_type = str
+        if delimiters is None:
+            delimiters = parse_delimiters_default_delimiters
+        backslash_character = '\\'
+        disallowed_delimiters = backslash_character
+        empty = ''
+
+    if not delimiters:
+        raise ValueError("invalid delimiters")
+    # convert
+    delimiters2 = []
+    for d in delimiters:
+        if isinstance(d, Delimiter):
+            delimiters2.append(d)
+            continue
+        if isinstance(d, s_type):
+            if not len(d) == 2:
+                raise ValueError(f"illegal delimiter string {d!r}, must be 2 characters long")
+            delimiters2.append(Delimiter(d[0:1], d[1:2]))
+            continue
+        raise TypeError(f"invalid delimiter {d!r}")
+
+    delimiters = delimiters2
+    # early-detect errors
+
+    # scan for disallowed
+    delimiter_characters = {d.open for d in delimiters} | {d.close for d in delimiters}
+    disallowed = {disallowed_delimiters}
+    illegal_delimiters = disallowed & delimiter_characters
+    if illegal_delimiters:
+        raise ValueError("illegal delimiters used: " + "".join(illegal_delimiters))
+
+    # closers is a set of closing delimiters *only*.
+    # if open and close delimiters are the same (e.g. quote marks)
+    # it shouldn't go in closers.
+    seen = set()
+    repeated = []
+    closers = set()
+    for d in delimiters:
+        if d.open in seen:
+            repeated.append(d.open)
+        seen.add(d.open)
+        if d.close != d.open:
+            closers.add(d.close)
+
+    if repeated:
+        raise ValueError("these opening delimiters were used multiple times: " + " ".join(repeated))
+
+    def parse_delimiters(s, delimiters):
+        open_to_delimiter = {d.open: d for d in delimiters}
+
+        text = []
+        append = text.append
+        def flush(open, close):
+            s = empty.join(text)
+            text.clear()
+            assert s or open or close
+            return s, open, close
+
+        # d stores the *current* delimiter
+        # d is not in stack.
+        d = _base_delimiter
+        stack = []
+        backslash = d.backslash
+        nested = d.nested
+        close = None
+        quoted = False
+
+        for i, c in enumerate(_iterate_over_bytes(s)):
+            if quoted:
+                append(c)
+                quoted = False
+                continue
+            if c == close:
+                yield flush(empty, c)
+                d = stack.pop()
+                backslash = d.backslash
+                nested = d.nested
+                close = d.close
+                continue
+            if nested:
+                if c in closers:
+                    # this is a closing delimiter,
+                    # but it doesn't match.
+                    # (if it did, we'd have handled it
+                    #  in "if c == close" above.)
+                    raise ValueError(f"mismatched closing delimiter at s[{i}]: expected {close}, got {c}")
+                next_d = open_to_delimiter.get(c)
+                if next_d:
+                    yield flush(c, empty)
+                    stack.append(d)
+                    d = next_d
+                    backslash = d.backslash
+                    nested = d.nested
+                    close = d.close
+                    continue
+            if backslash and (c == backslash_character):
+                quoted = True
+            append(c)
+
+        if len(stack):
+            stack.pop(0)
+            stack.append(d)
+            raise ValueError("s does not close all opened delimiters, needs " + " ".join(d.close for d in reversed(stack)))
+
+        if text:
+            yield flush(empty, empty)
+
+    return parse_delimiters(s, delimiters)
+
+
+
 @_export
 class LineInfo:
     """
     The second object yielded by a lines iterator,
     containing metadata about the line.
     You can add your own fields by passing them in
     via **kwargs; you can also add new attributes
```

### Comparing `big-0.8/big/time.py` & `big-0.8.1/big/time.py`

 * *Files identical despite different names*

### Comparing `big-0.8/pyproject.toml` & `big-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `big-0.8/resources/experiments/alice.in.wonderland.txt` & `big-0.8.1/resources/experiments/alice.in.wonderland.txt`

 * *Files identical despite different names*

### Comparing `big-0.8/resources/experiments/time_multisplit.py` & `big-0.8.1/resources/experiments/time_multisplit.py`

 * *Files identical despite different names*

### Comparing `big-0.8/resources/images/big.header.png` & `big-0.8.1/resources/images/big.header.png`

 * *Files identical despite different names*

### Comparing `big-0.8/test/bigtestlib.py` & `big-0.8.1/test/bigtestlib.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_all.py` & `big-0.8.1/test/test_all.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_boundinnerclass.py` & `big-0.8.1/test/test_boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_builtin.py` & `big-0.8.1/test/test_builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_file.py` & `big-0.8.1/test/test_file.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_graph.py` & `big-0.8.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_heap.py` & `big-0.8.1/test/test_heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_itertools.py` & `big-0.8.1/test/test_itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_scheduler.py` & `big-0.8.1/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8/test/test_text.py` & `big-0.8.1/test/test_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -6015,986 +6015,1216 @@
 000177e0: 2020 2020 2020 2020 2028 5472 7565 2c20           (True, 
 000177f0: 2722 2227 292c 0a20 2020 2020 2020 2020  '""'),.         
 00017800: 2020 2020 2020 2028 4661 6c73 652c 2027         (False, '
 00017810: 2069 7420 6b69 6e64 6120 776f 726b 7320   it kinda works 
 00017820: 616e 7977 6179 2127 292c 0a20 2020 2020  anyway!'),.     
 00017830: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
 00017840: 2020 2020 2020 7472 6970 6c65 5f71 756f        triple_quo
-00017850: 7465 733d 4661 6c73 6529 0a0a 0a20 2020  tes=False)...   
-00017860: 2064 6566 2074 6573 745f 6c69 6e65 7328   def test_lines(
-00017870: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
-00017880: 6566 2074 6573 7428 692c 2065 7870 6563  ef test(i, expec
-00017890: 7465 6429 3a0a 2020 2020 2020 2020 2020  ted):.          
-000178a0: 2020 676f 7420 3d20 6c69 7374 2869 290a    got = list(i).
-000178b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000178c0: 2e61 7373 6572 7445 7175 616c 2867 6f74  .assertEqual(got
-000178d0: 2c20 6578 7065 6374 6564 290a 0a20 2020  , expected)..   
-000178e0: 2020 2020 204c 4920 3d20 6269 672e 4c69       LI = big.Li
-000178f0: 6e65 496e 666f 0a0a 2020 2020 2020 2020  neInfo..        
-00017900: 6465 6620 4c28 6c69 6e65 2c20 6c69 6e65  def L(line, line
-00017910: 5f6e 756d 6265 722c 2063 6f6c 756d 6e5f  _number, column_
-00017920: 6e75 6d62 6572 3d31 2c20 2a2a 6b77 6172  number=1, **kwar
-00017930: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
-00017940: 2069 6e66 6f20 3d20 6269 672e 4c69 6e65   info = big.Line
-00017950: 496e 666f 286c 696e 652c 206c 696e 655f  Info(line, line_
-00017960: 6e75 6d62 6572 2c20 636f 6c75 6d6e 5f6e  number, column_n
-00017970: 756d 6265 722c 202a 2a6b 7761 7267 7329  umber, **kwargs)
-00017980: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00017990: 7572 6e20 2869 6e66 6f2c 206c 696e 6529  urn (info, line)
-000179a0: 0a0a 2020 2020 2020 2020 7465 7374 2862  ..        test(b
-000179b0: 6967 2e6c 696e 6573 2822 615c 6e62 5c6e  ig.lines("a\nb\n
-000179c0: 635c 6e64 5c6e 655c 6e22 292c 0a20 2020  c\nd\ne\n"),.   
-000179d0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-000179e0: 2020 2020 2020 2028 4c49 2827 6127 2c20         (LI('a', 
-000179f0: 312c 2031 292c 2027 6127 292c 0a20 2020  1, 1), 'a'),.   
-00017a00: 2020 2020 2020 2020 2028 4c49 2827 6227           (LI('b'
-00017a10: 2c20 322c 2031 292c 2027 6227 292c 0a20  , 2, 1), 'b'),. 
-00017a20: 2020 2020 2020 2020 2020 2028 4c49 2827             (LI('
-00017a30: 6327 2c20 332c 2031 292c 2027 6327 292c  c', 3, 1), 'c'),
-00017a40: 0a20 2020 2020 2020 2020 2020 2028 4c49  .            (LI
-00017a50: 2827 6427 2c20 342c 2031 292c 2027 6427  ('d', 4, 1), 'd'
-00017a60: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00017a70: 4c49 2827 6527 2c20 352c 2031 292c 2027  LI('e', 5, 1), '
-00017a80: 6527 292c 0a20 2020 2020 2020 2020 2020  e'),.           
-00017a90: 2028 4c49 2827 272c 2020 362c 2031 292c   (LI('',  6, 1),
-00017aa0: 2027 2729 2c0a 2020 2020 2020 2020 2020   ''),.          
-00017ab0: 2020 5d29 0a0a 2020 2020 2020 2020 6c69    ])..        li
-00017ac0: 6e65 7320 3d20 5b27 6669 7273 7420 6c69  nes = ['first li
-00017ad0: 6e65 272c 2027 5c74 7365 636f 6e64 206c  ne', '\tsecond l
-00017ae0: 696e 6527 2c20 2774 6869 7264 206c 696e  ine', 'third lin
-00017af0: 6527 5d0a 2020 2020 2020 2020 7465 7374  e'].        test
-00017b00: 2862 6967 2e6c 696e 6573 5f73 7472 6970  (big.lines_strip
-00017b10: 2862 6967 2e6c 696e 6573 286c 696e 6573  (big.lines(lines
-00017b20: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00017b30: 5b0a 2020 2020 2020 2020 2020 2020 284c  [.            (L
-00017b40: 4928 2766 6972 7374 206c 696e 6527 2c20  I('first line', 
-00017b50: 312c 2031 292c 2027 6669 7273 7420 6c69  1, 1), 'first li
-00017b60: 6e65 2729 2c0a 2020 2020 2020 2020 2020  ne'),.          
-00017b70: 2020 284c 4928 275c 7473 6563 6f6e 6420    (LI('\tsecond 
-00017b80: 6c69 6e65 272c 2032 2c20 392c 206c 6561  line', 2, 9, lea
-00017b90: 6469 6e67 3d27 5c74 2729 2c20 2773 6563  ding='\t'), 'sec
-00017ba0: 6f6e 6420 6c69 6e65 2729 2c0a 2020 2020  ond line'),.    
-00017bb0: 2020 2020 2020 2020 284c 4928 2774 6869          (LI('thi
-00017bc0: 7264 206c 696e 6527 2c20 332c 2031 292c  rd line', 3, 1),
-00017bd0: 2027 7468 6972 6420 6c69 6e65 2729 2c0a   'third line'),.
-00017be0: 2020 2020 2020 2020 2020 2020 5d29 0a0a              ])..
-00017bf0: 2020 2020 2020 2020 7465 7374 2862 6967          test(big
-00017c00: 2e6c 696e 6573 5f66 696c 7465 725f 636f  .lines_filter_co
-00017c10: 6d6d 656e 745f 6c69 6e65 7328 6269 672e  mment_lines(big.
-00017c20: 6c69 6e65 7328 2222 220a 2020 2020 2320  lines(""".    # 
-00017c30: 636f 6d6d 656e 740a 2020 2020 6120 3d20  comment.    a = 
-00017c40: 620a 2020 2020 2f2f 2061 6e6f 7468 6572  b.    // another
-00017c50: 2063 6f6d 6d65 6e74 0a20 2020 2063 203d   comment.    c =
-00017c60: 2064 0a20 2020 202f 206e 6f74 2061 2063   d.    / not a c
-00017c70: 6f6d 6d65 6e74 0a20 2020 202f 2f2f 2069  omment.    /// i
-00017c80: 7320 6120 636f 6d6d 656e 7421 0a20 2020  s a comment!.   
-00017c90: 2023 2320 616e 6f74 6865 7220 636f 6d6d   ## another comm
-00017ca0: 656e 7421 0a20 2020 2023 2120 6120 7468  ent!.    #! a th
-00017cb0: 6972 6420 636f 6d6d 656e 7421 0a22 2222  ird comment!."""
-00017cc0: 2e6c 7374 7269 7028 275c 6e27 2929 2c20  .lstrip('\n')), 
-00017cd0: 2827 2327 2c20 272f 2f27 2929 2c0a 2020  ('#', '//')),.  
-00017ce0: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
-00017cf0: 2020 2020 2020 2020 284c 4928 2720 2020          (LI('   
-00017d00: 2061 203d 2062 272c 2020 2020 2020 2020   a = b',        
-00017d10: 2020 2032 2c20 3129 2c20 2720 2020 2061     2, 1), '    a
-00017d20: 203d 2062 2729 2c0a 2020 2020 2020 2020   = b'),.        
-00017d30: 2020 2020 284c 4928 2720 2020 2063 203d      (LI('    c =
-00017d40: 2064 272c 2020 2020 2020 2020 2020 2034   d',           4
-00017d50: 2c20 3129 2c20 2720 2020 2063 203d 2064  , 1), '    c = d
-00017d60: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00017d70: 284c 4928 2720 2020 202f 206e 6f74 2061  (LI('    / not a
-00017d80: 2063 6f6d 6d65 6e74 272c 2035 2c20 3129   comment', 5, 1)
-00017d90: 2c20 2720 2020 202f 206e 6f74 2061 2063  , '    / not a c
-00017da0: 6f6d 6d65 6e74 2729 2c0a 2020 2020 2020  omment'),.      
-00017db0: 2020 2020 2020 284c 4928 2727 2c20 2020        (LI('',   
-00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dd0: 2039 2c20 3129 2c20 2727 292c 0a20 2020   9, 1), ''),.   
-00017de0: 2020 2020 2020 2020 205d 290a 0a20 2020           ])..   
-00017df0: 2020 2020 2074 6573 7428 6269 672e 6c69       test(big.li
-00017e00: 6e65 735f 6669 6c74 6572 5f63 6f6d 6d65  nes_filter_comme
-00017e10: 6e74 5f6c 696e 6573 2862 6967 2e6c 696e  nt_lines(big.lin
-00017e20: 6573 2862 2261 5c6e 2320 6967 6e6f 7265  es(b"a\n# ignore
-00017e30: 645c 6e20 6322 292c 2062 2723 2729 2c0a  d\n c"), b'#'),.
-00017e40: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-00017e50: 2020 2020 2020 2020 2020 4c28 6227 6127            L(b'a'
-00017e60: 2c20 3129 2c0a 2020 2020 2020 2020 2020  , 1),.          
-00017e70: 2020 4c28 6227 2063 272c 2033 292c 0a20    L(b' c', 3),. 
-00017e80: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00017e90: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00017ea0: 2020 2020 7465 7374 2862 6967 2e6c 696e      test(big.lin
-00017eb0: 6573 5f63 6f6e 7461 696e 696e 6728 6269  es_containing(bi
-00017ec0: 672e 6c69 6e65 7328 2222 220a 6865 6c6c  g.lines(""".hell
-00017ed0: 6f20 796f 6c6b 730a 7768 6174 2064 6f20  o yolks.what do 
-00017ee0: 796f 7520 6861 7665 2074 6f20 7361 792c  you have to say,
-00017ef0: 2063 6861 6d70 3f0a 6920 6c69 6b65 2065   champ?.i like e
-00017f00: 6767 732e 0a74 6865 7920 646f 6e27 7420  ggs..they don't 
-00017f10: 6861 7665 2074 6f20 6265 2066 616e 6379  have to be fancy
-00017f20: 2e0a 7369 6d70 6c65 2073 6372 616d 626c  ..simple scrambl
-00017f30: 6564 2065 6767 7320 6172 6520 6a75 7374  ed eggs are just
-00017f40: 2066 696e 652e 0a6e 6567 6761 746f 7279   fine..neggatory
-00017f50: 210a 7768 6f6f 7073 2c20 4920 6d65 616e  !.whoops, I mean
-00017f60: 742c 206e 6567 6174 6f72 792e 0a22 2222  t, negatory.."""
-00017f70: 5b31 3a5d 292c 2022 6567 6722 292c 0a20  [1:]), "egg"),. 
-00017f80: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-00017f90: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
-00017fa0: 2827 6920 6c69 6b65 2065 6767 732e 272c  ('i like eggs.',
-00017fb0: 2033 2c20 3129 2c20 2769 206c 696b 6520   3, 1), 'i like 
-00017fc0: 6567 6773 2e27 292c 0a20 2020 2020 2020  eggs.'),.       
-00017fd0: 2020 2020 2020 2020 2028 4c49 2827 7369           (LI('si
-00017fe0: 6d70 6c65 2073 6372 616d 626c 6564 2065  mple scrambled e
-00017ff0: 6767 7320 6172 6520 6a75 7374 2066 696e  ggs are just fin
-00018000: 652e 272c 2035 2c20 3129 2c20 2773 696d  e.', 5, 1), 'sim
-00018010: 706c 6520 7363 7261 6d62 6c65 6420 6567  ple scrambled eg
-00018020: 6773 2061 7265 206a 7573 7420 6669 6e65  gs are just fine
-00018030: 2e27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-00018040: 2020 2020 2028 4c49 2827 6e65 6767 6174       (LI('neggat
-00018050: 6f72 7921 272c 2036 2c20 3129 2c20 276e  ory!', 6, 1), 'n
-00018060: 6567 6761 746f 7279 2127 292c 0a20 2020  eggatory!'),.   
-00018070: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00018080: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00018090: 2020 7465 7374 2862 6967 2e6c 696e 6573    test(big.lines
-000180a0: 5f63 6f6e 7461 696e 696e 6728 6269 672e  _containing(big.
-000180b0: 6c69 6e65 7328 2222 220a 6865 6c6c 6f20  lines(""".hello 
-000180c0: 796f 6c6b 730a 7768 6174 2064 6f20 796f  yolks.what do yo
-000180d0: 7520 6861 7665 2074 6f20 7361 792c 2063  u have to say, c
-000180e0: 6861 6d70 3f0a 6920 6c69 6b65 2065 6767  hamp?.i like egg
-000180f0: 732e 0a74 6865 7920 646f 6e27 7420 6861  s..they don't ha
-00018100: 7665 2074 6f20 6265 2066 616e 6379 2e0a  ve to be fancy..
-00018110: 7369 6d70 6c65 2073 6372 616d 626c 6564  simple scrambled
-00018120: 2065 6767 7320 6172 6520 6a75 7374 2066   eggs are just f
-00018130: 696e 652e 0a6e 6567 6761 746f 7279 210a  ine..neggatory!.
-00018140: 7768 6f6f 7073 2c20 4920 6d65 616e 742c  whoops, I meant,
-00018150: 206e 6567 6174 6f72 792e 0a22 2222 5b31   negatory.."""[1
-00018160: 3a5d 292c 2022 6567 6722 2c20 696e 7665  :]), "egg", inve
-00018170: 7274 3d54 7275 6529 2c0a 2020 2020 2020  rt=True),.      
-00018180: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00018190: 2020 2020 2020 2020 284c 4928 2768 656c          (LI('hel
-000181a0: 6c6f 2079 6f6c 6b73 272c 2031 2c20 3129  lo yolks', 1, 1)
-000181b0: 2c20 2768 656c 6c6f 2079 6f6c 6b73 2729  , 'hello yolks')
-000181c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000181d0: 2020 284c 4928 2777 6861 7420 646f 2079    (LI('what do y
-000181e0: 6f75 2068 6176 6520 746f 2073 6179 2c20  ou have to say, 
-000181f0: 6368 616d 703f 272c 2032 2c20 3129 2c20  champ?', 2, 1), 
-00018200: 2777 6861 7420 646f 2079 6f75 2068 6176  'what do you hav
-00018210: 6520 746f 2073 6179 2c20 6368 616d 703f  e to say, champ?
-00018220: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00018230: 2020 2020 284c 4928 2274 6865 7920 646f      (LI("they do
-00018240: 6e27 7420 6861 7665 2074 6f20 6265 2066  n't have to be f
-00018250: 616e 6379 2e22 2c20 342c 2031 292c 2022  ancy.", 4, 1), "
-00018260: 7468 6579 2064 6f6e 2774 2068 6176 6520  they don't have 
-00018270: 746f 2062 6520 6661 6e63 792e 2229 2c0a  to be fancy."),.
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 284c 4928 2777 686f 6f70 732c 2049 206d  (LI('whoops, I m
-000182a0: 6561 6e74 2c20 6e65 6761 746f 7279 2e27  eant, negatory.'
-000182b0: 2c20 372c 2031 292c 2027 7768 6f6f 7073  , 7, 1), 'whoops
-000182c0: 2c20 4920 6d65 616e 742c 206e 6567 6174  , I meant, negat
-000182d0: 6f72 792e 2729 2c0a 2020 2020 2020 2020  ory.'),.        
-000182e0: 2020 2020 2020 2020 284c 4928 2727 2c20          (LI('', 
-000182f0: 382c 2031 292c 2027 2729 2c0a 2020 2020  8, 1), ''),.    
-00018300: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00018310: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00018320: 2074 6573 7428 6269 672e 6c69 6e65 735f   test(big.lines_
-00018330: 6772 6570 2862 6967 2e6c 696e 6573 2822  grep(big.lines("
-00018340: 2222 0a68 656c 6c6f 2079 6f6c 6b73 0a77  "".hello yolks.w
-00018350: 6861 7420 646f 2079 6f75 2068 6176 6520  hat do you have 
-00018360: 746f 2073 6179 2c20 6368 616d 703f 0a69  to say, champ?.i
-00018370: 206c 696b 6520 6567 6773 2e0a 7468 6579   like eggs..they
-00018380: 2064 6f6e 2774 2068 6176 6520 746f 2062   don't have to b
-00018390: 6520 6661 6e63 792e 0a73 696d 706c 6520  e fancy..simple 
-000183a0: 7363 7261 6d62 6c65 6420 6567 6773 2061  scrambled eggs a
-000183b0: 7265 206a 7573 7420 6669 6e65 2e0a 6e65  re just fine..ne
-000183c0: 6767 6174 6f72 7921 0a77 686f 6f70 732c  ggatory!.whoops,
-000183d0: 2049 206d 6561 6e74 2c20 6e65 6761 746f   I meant, negato
-000183e0: 7279 2e0a 2222 225b 313a 5d29 2c20 2265  ry.."""[1:]), "e
-000183f0: 672b 2229 2c0a 2020 2020 2020 2020 2020  g+"),.          
-00018400: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00018410: 2020 2020 284c 4928 2769 206c 696b 6520      (LI('i like 
-00018420: 6567 6773 2e27 2c20 332c 2031 292c 2027  eggs.', 3, 1), '
-00018430: 6920 6c69 6b65 2065 6767 732e 2729 2c0a  i like eggs.'),.
-00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 284c 4928 2773 696d 706c 6520 7363 7261  (LI('simple scra
-00018460: 6d62 6c65 6420 6567 6773 2061 7265 206a  mbled eggs are j
-00018470: 7573 7420 6669 6e65 2e27 2c20 352c 2031  ust fine.', 5, 1
-00018480: 292c 2027 7369 6d70 6c65 2073 6372 616d  ), 'simple scram
-00018490: 626c 6564 2065 6767 7320 6172 6520 6a75  bled eggs are ju
-000184a0: 7374 2066 696e 652e 2729 2c0a 2020 2020  st fine.'),.    
-000184b0: 2020 2020 2020 2020 2020 2020 284c 4928              (LI(
-000184c0: 276e 6567 6761 746f 7279 2127 2c20 362c  'neggatory!', 6,
-000184d0: 2031 292c 2027 6e65 6767 6174 6f72 7921   1), 'neggatory!
-000184e0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000184f0: 2020 2020 284c 4928 2777 686f 6f70 732c      (LI('whoops,
-00018500: 2049 206d 6561 6e74 2c20 6e65 6761 746f   I meant, negato
-00018510: 7279 2e27 2c20 372c 2031 292c 2027 7768  ry.', 7, 1), 'wh
-00018520: 6f6f 7073 2c20 4920 6d65 616e 742c 206e  oops, I meant, n
-00018530: 6567 6174 6f72 792e 2729 2c0a 2020 2020  egatory.'),.    
-00018540: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00018550: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00018560: 2074 6573 7428 6269 672e 6c69 6e65 735f   test(big.lines_
-00018570: 6772 6570 2862 6967 2e6c 696e 6573 2822  grep(big.lines("
-00018580: 2222 0a68 656c 6c6f 2079 6f6c 6b73 0a77  "".hello yolks.w
-00018590: 6861 7420 646f 2079 6f75 2068 6176 6520  hat do you have 
-000185a0: 746f 2073 6179 2c20 6368 616d 703f 0a69  to say, champ?.i
-000185b0: 206c 696b 6520 6567 6773 2e0a 7468 6579   like eggs..they
-000185c0: 2064 6f6e 2774 2068 6176 6520 746f 2062   don't have to b
-000185d0: 6520 6661 6e63 792e 0a73 696d 706c 6520  e fancy..simple 
-000185e0: 7363 7261 6d62 6c65 6420 6567 6773 2061  scrambled eggs a
-000185f0: 7265 206a 7573 7420 6669 6e65 2e0a 6e65  re just fine..ne
-00018600: 6767 6174 6f72 7921 0a77 686f 6f70 732c  ggatory!.whoops,
-00018610: 2049 206d 6561 6e74 2c20 6e65 6761 746f   I meant, negato
-00018620: 7279 2e0a 2222 225b 313a 5d29 2c20 2265  ry.."""[1:]), "e
-00018630: 672b 222c 2069 6e76 6572 743d 5472 7565  g+", invert=True
-00018640: 292c 0a20 2020 2020 2020 2020 2020 205b  ),.            [
-00018650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018660: 2028 4c49 2827 6865 6c6c 6f20 796f 6c6b   (LI('hello yolk
-00018670: 7327 2c20 312c 2031 292c 2027 6865 6c6c  s', 1, 1), 'hell
-00018680: 6f20 796f 6c6b 7327 292c 0a20 2020 2020  o yolks'),.     
-00018690: 2020 2020 2020 2020 2020 2028 4c49 2827             (LI('
-000186a0: 7768 6174 2064 6f20 796f 7520 6861 7665  what do you have
-000186b0: 2074 6f20 7361 792c 2063 6861 6d70 3f27   to say, champ?'
-000186c0: 2c20 322c 2031 292c 2027 7768 6174 2064  , 2, 1), 'what d
-000186d0: 6f20 796f 7520 6861 7665 2074 6f20 7361  o you have to sa
-000186e0: 792c 2063 6861 6d70 3f27 292c 0a20 2020  y, champ?'),.   
-000186f0: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
-00018700: 2822 7468 6579 2064 6f6e 2774 2068 6176  ("they don't hav
-00018710: 6520 746f 2062 6520 6661 6e63 792e 222c  e to be fancy.",
-00018720: 2034 2c20 3129 2c20 2274 6865 7920 646f   4, 1), "they do
-00018730: 6e27 7420 6861 7665 2074 6f20 6265 2066  n't have to be f
-00018740: 616e 6379 2e22 292c 0a20 2020 2020 2020  ancy."),.       
-00018750: 2020 2020 2020 2020 2028 4c49 2827 272c           (LI('',
-00018760: 2038 2c20 3129 2c20 2727 292c 0a20 2020   8, 1), ''),.   
-00018770: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00018780: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00018790: 2020 7465 7374 2862 6967 2e6c 696e 6573    test(big.lines
-000187a0: 5f73 6f72 7428 6269 672e 6c69 6e65 7328  _sort(big.lines(
-000187b0: 2222 220a 636f 726d 6f72 616e 740a 6669  """.cormorant.fi
-000187c0: 7265 666f 780a 616c 6c69 6761 746f 720a  refox.alligator.
-000187d0: 6469 706c 6f64 6f63 7573 0a65 6c65 7068  diplodocus.eleph
-000187e0: 616e 740a 6769 7261 6666 650a 6261 7272  ant.giraffe.barr
-000187f0: 6163 7564 610a 6875 6d6d 696e 6762 6972  acuda.hummingbir
-00018800: 640a 2222 225b 313a 2d31 5d29 292c 0a20  d."""[1:-1])),. 
-00018810: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-00018820: 2020 2020 2020 2020 2020 2020 204c 2827               L('
-00018830: 616c 6c69 6761 746f 7227 2c20 3329 2c0a  alligator', 3),.
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 4c28 2762 6172 7261 6375 6461 272c 2037  L('barracuda', 7
-00018860: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00018870: 2020 204c 2827 636f 726d 6f72 616e 7427     L('cormorant'
-00018880: 2c20 3129 2c0a 2020 2020 2020 2020 2020  , 1),.          
-00018890: 2020 2020 2020 4c28 2764 6970 6c6f 646f        L('diplodo
-000188a0: 6375 7327 2c20 3429 2c0a 2020 2020 2020  cus', 4),.      
-000188b0: 2020 2020 2020 2020 2020 4c28 2765 6c65            L('ele
-000188c0: 7068 616e 7427 2c20 3529 2c0a 2020 2020  phant', 5),.    
-000188d0: 2020 2020 2020 2020 2020 2020 4c28 2766              L('f
-000188e0: 6972 6566 6f78 272c 2032 292c 0a20 2020  irefox', 2),.   
-000188f0: 2020 2020 2020 2020 2020 2020 204c 2827               L('
-00018900: 6769 7261 6666 6527 2c20 3629 2c0a 2020  giraffe', 6),.  
-00018910: 2020 2020 2020 2020 2020 2020 2020 4c28                L(
-00018920: 2768 756d 6d69 6e67 6269 7264 272c 2038  'hummingbird', 8
-00018930: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
-00018940: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00018950: 2020 2020 2020 2020 7465 7374 2862 6967          test(big
-00018960: 2e6c 696e 6573 5f73 6f72 7428 6269 672e  .lines_sort(big.
-00018970: 6c69 6e65 7328 2222 220a 636f 726d 6f72  lines(""".cormor
-00018980: 616e 740a 6669 7265 666f 780a 616c 6c69  ant.firefox.alli
-00018990: 6761 746f 720a 6469 706c 6f64 6f63 7573  gator.diplodocus
-000189a0: 0a65 6c65 7068 616e 740a 6769 7261 6666  .elephant.giraff
-000189b0: 650a 6261 7272 6163 7564 610a 6875 6d6d  e.barracuda.humm
-000189c0: 696e 6762 6972 640a 2222 225b 313a 2d31  ingbird."""[1:-1
-000189d0: 5d29 2c20 7265 7665 7273 653d 5472 7565  ]), reverse=True
-000189e0: 292c 0a20 2020 2020 2020 2020 2020 205b  ),.            [
-000189f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a00: 204c 2827 6875 6d6d 696e 6762 6972 6427   L('hummingbird'
-00018a10: 2c20 3829 2c0a 2020 2020 2020 2020 2020  , 8),.          
-00018a20: 2020 2020 2020 4c28 2767 6972 6166 6665        L('giraffe
-00018a30: 272c 2036 292c 0a20 2020 2020 2020 2020  ', 6),.         
-00018a40: 2020 2020 2020 204c 2827 6669 7265 666f         L('firefo
-00018a50: 7827 2c20 3229 2c0a 2020 2020 2020 2020  x', 2),.        
-00018a60: 2020 2020 2020 2020 4c28 2765 6c65 7068          L('eleph
-00018a70: 616e 7427 2c20 3529 2c0a 2020 2020 2020  ant', 5),.      
-00018a80: 2020 2020 2020 2020 2020 4c28 2764 6970            L('dip
-00018a90: 6c6f 646f 6375 7327 2c20 3429 2c0a 2020  lodocus', 4),.  
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 4c28                L(
-00018ab0: 2763 6f72 6d6f 7261 6e74 272c 2031 292c  'cormorant', 1),
-00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ad0: 204c 2827 6261 7272 6163 7564 6127 2c20   L('barracuda', 
-00018ae0: 3729 2c0a 2020 2020 2020 2020 2020 2020  7),.            
-00018af0: 2020 2020 4c28 2761 6c6c 6967 6174 6f72      L('alligator
-00018b00: 272c 2033 292c 0a20 2020 2020 2020 2020  ', 3),.         
-00018b10: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00018b20: 2029 0a0a 2020 2020 2020 2020 7465 7374   )..        test
-00018b30: 2862 6967 2e6c 696e 6573 5f72 7374 7269  (big.lines_rstri
-00018b40: 7028 6269 672e 6c69 6e65 7328 0a22 2020  p(big.lines(."  
-00018b50: 2020 6120 3d20 6220 205c 6e22 0a22 2020    a = b  \n"."  
-00018b60: 2020 6320 3d20 6420 2020 2020 5c6e 220a    c = d     \n".
-00018b70: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00018b80: 5b0a 2020 2020 2020 2020 2020 2020 284c  [.            (L
-00018b90: 4928 2720 2020 2061 203d 2062 2020 272c  I('    a = b  ',
-00018ba0: 2020 2020 312c 2031 292c 2027 2020 2020      1, 1), '    
-00018bb0: 6120 3d20 6227 292c 0a20 2020 2020 2020  a = b'),.       
-00018bc0: 2020 2020 2028 4c49 2827 2020 2020 6320       (LI('    c 
-00018bd0: 3d20 6420 2020 2020 272c 2032 2c20 3129  = d     ', 2, 1)
-00018be0: 2c20 2720 2020 2063 203d 2064 2729 2c0a  , '    c = d'),.
-00018bf0: 2020 2020 2020 2020 2020 2020 284c 4928              (LI(
-00018c00: 2727 2c20 2020 2020 2020 2020 2020 2020  '',             
-00018c10: 2020 332c 2031 292c 2027 2729 2c0a 2020    3, 1), ''),.  
-00018c20: 2020 2020 2020 2020 2020 5d29 0a0a 2020            ])..  
-00018c30: 2020 2020 2020 7465 7374 2862 6967 2e6c        test(big.l
-00018c40: 696e 6573 5f73 7472 6970 2862 6967 2e6c  ines_strip(big.l
-00018c50: 696e 6573 280a 2220 2020 2061 203d 2062  ines(."    a = b
-00018c60: 2020 5c6e 220a 2220 2020 2063 203d 2064    \n"."    c = d
-00018c70: 2020 2020 205c 6e22 0a29 292c 0a20 2020       \n".)),.   
-00018c80: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00018c90: 2020 2020 2020 2028 4c49 2827 2020 2020         (LI('    
-00018ca0: 6120 3d20 6220 2027 2c20 2020 2031 2c20  a = b  ',    1, 
-00018cb0: 352c 206c 6561 6469 6e67 3d27 2020 2020  5, leading='    
-00018cc0: 2729 2c20 2761 203d 2062 2729 2c0a 2020  '), 'a = b'),.  
-00018cd0: 2020 2020 2020 2020 2020 284c 4928 2720            (LI(' 
-00018ce0: 2020 2063 203d 2064 2020 2020 2027 2c20     c = d     ', 
-00018cf0: 322c 2035 2c20 6c65 6164 696e 673d 2720  2, 5, leading=' 
-00018d00: 2020 2027 292c 2027 6320 3d20 6427 292c     '), 'c = d'),
-00018d10: 0a20 2020 2020 2020 2020 2020 2028 4c49  .            (LI
-00018d20: 2827 272c 2020 2020 2020 2020 2020 2020  ('',            
-00018d30: 2020 2033 2c20 3129 2c20 2727 292c 0a20     3, 1), ''),. 
-00018d40: 2020 2020 2020 2020 2020 205d 290a 0a20             ]).. 
-00018d50: 2020 2020 2020 2074 6573 7428 6269 672e         test(big.
-00018d60: 6c69 6e65 735f 6669 6c74 6572 5f65 6d70  lines_filter_emp
-00018d70: 7479 5f6c 696e 6573 2862 6967 2e6c 696e  ty_lines(big.lin
-00018d80: 6573 2822 2222 0a0a 2020 2020 6120 3d20  es("""..    a = 
-00018d90: 620a 0a0a 2020 2020 6320 3d20 640a 0a22  b...    c = d.."
-00018da0: 2222 5b31 3a5d 2929 2c0a 2020 2020 2020  ""[1:])),.      
-00018db0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00018dc0: 2020 2020 284c 4928 2720 2020 2061 203d      (LI('    a =
-00018dd0: 2062 272c 2032 2c20 3129 2c20 2720 2020   b', 2, 1), '   
-00018de0: 2061 203d 2062 2729 2c0a 2020 2020 2020   a = b'),.      
-00018df0: 2020 2020 2020 284c 4928 2720 2020 2063        (LI('    c
-00018e00: 203d 2064 272c 2035 2c20 3129 2c20 2720   = d', 5, 1), ' 
-00018e10: 2020 2063 203d 2064 2729 2c0a 2020 2020     c = d'),.    
-00018e20: 2020 2020 2020 2020 5d29 0a0a 2020 2020          ])..    
-00018e30: 2020 2020 7465 7374 2862 6967 2e6c 696e      test(big.lin
-00018e40: 6573 5f63 6f6e 7665 7274 5f74 6162 735f  es_convert_tabs_
-00018e50: 746f 5f73 7061 6365 7328 6269 672e 6c69  to_spaces(big.li
-00018e60: 6e65 7328 0a20 2020 2020 2020 2020 2020  nes(.           
-00018e70: 2022 5c74 6669 7273 7420 6c69 6e65 5c6e   "\tfirst line\n
-00018e80: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
-00018e90: 745c 7473 6563 6f6e 6420 6c69 6e65 5c6e  t\tsecond line\n
-00018ea0: 220a 2020 2020 2020 2020 2020 2020 2220  ".            " 
-00018eb0: 205c 7474 6869 7264 206c 696e 655c 6e22   \tthird line\n"
-00018ec0: 2c0a 2020 2020 2020 2020 2020 2020 7461  ,.            ta
-00018ed0: 625f 7769 6474 683d 3829 292c 0a20 2020  b_width=8)),.   
-00018ee0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00018ef0: 2020 2020 2020 2020 2020 2028 4c49 2822             (LI("
-00018f00: 5c74 6669 7273 7420 6c69 6e65 222c 2031  \tfirst line", 1
-00018f10: 2c20 3129 2c20 2220 2020 2020 2020 2066  , 1), "        f
-00018f20: 6972 7374 206c 696e 6522 292c 0a20 2020  irst line"),.   
-00018f30: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
-00018f40: 2822 5c74 5c74 7365 636f 6e64 206c 696e  ("\t\tsecond lin
-00018f50: 6522 2c20 322c 2031 292c 2022 2020 2020  e", 2, 1), "    
-00018f60: 2020 2020 2020 2020 2020 2020 7365 636f              seco
-00018f70: 6e64 206c 696e 6522 292c 0a20 2020 2020  nd line"),.     
-00018f80: 2020 2020 2020 2020 2020 2028 4c49 2822             (LI("
-00018f90: 2020 5c74 7468 6972 6420 6c69 6e65 222c    \tthird line",
-00018fa0: 2033 2c20 3129 2c20 2220 2020 2020 2020   3, 1), "       
-00018fb0: 2074 6869 7264 206c 696e 6522 292c 0a20   third line"),. 
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00018fd0: 4c49 2822 222c 2034 2c20 3129 2c20 2222  LI("", 4, 1), ""
-00018fe0: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
-00018ff0: 290a 0a20 2020 2020 2020 2074 6573 7428  )..        test(
-00019000: 6269 672e 6c69 6e65 735f 7374 7269 705f  big.lines_strip_
-00019010: 636f 6d6d 656e 7473 2862 6967 2e6c 696e  comments(big.lin
-00019020: 6573 2822 2222 0a66 6f72 2078 2069 6e20  es(""".for x in 
-00019030: 7261 6e67 6528 3529 3a20 2320 7468 6973  range(5): # this
-00019040: 2069 7320 6120 636f 6d6d 656e 740a 2020   is a comment.  
-00019050: 2020 7072 696e 7428 2223 2074 6869 7320    print("# this 
-00019060: 6973 2071 756f 7465 6422 2c20 7829 0a20  is quoted", x). 
-00019070: 2020 2070 7269 6e74 2822 2229 2023 2074     print("") # t
-00019080: 6869 7320 2263 6f6d 6d65 6e74 2220 6973  his "comment" is
-00019090: 2075 7365 6c65 7373 0a20 2020 2070 7269   useless.    pri
-000190a0: 6e74 286e 6f5f 636f 6d6d 656e 7473 5f6f  nt(no_comments_o
-000190b0: 725f 7175 6f74 6573 5f6f 6e5f 7468 6973  r_quotes_on_this
-000190c0: 5f6c 696e 6529 0a22 2222 5b31 3a5d 292c  _line)."""[1:]),
-000190d0: 2028 2223 222c 2022 2f2f 2229 292c 0a20   ("#", "//")),. 
-000190e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-000190f0: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
-00019100: 286c 696e 653d 2766 6f72 2078 2069 6e20  (line='for x in 
-00019110: 7261 6e67 6528 3529 3a20 2320 7468 6973  range(5): # this
-00019120: 2069 7320 6120 636f 6d6d 656e 7427 2c20   is a comment', 
-00019130: 6c69 6e65 5f6e 756d 6265 723d 312c 2063  line_number=1, c
-00019140: 6f6c 756d 6e5f 6e75 6d62 6572 3d31 2c20  olumn_number=1, 
-00019150: 636f 6d6d 656e 743d 2723 2074 6869 7320  comment='# this 
-00019160: 6973 2061 2063 6f6d 6d65 6e74 2729 2c0a  is a comment'),.
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 2020 2020 2766 6f72 2078 2069 6e20 7261      'for x in ra
-00019190: 6e67 6528 3529 3a27 292c 0a20 2020 2020  nge(5):'),.     
-000191a0: 2020 2020 2020 2020 2020 2028 4c49 286c             (LI(l
-000191b0: 696e 653d 2720 2020 2070 7269 6e74 2822  ine='    print("
-000191c0: 2320 7468 6973 2069 7320 7175 6f74 6564  # this is quoted
-000191d0: 222c 2078 2927 2c20 6c69 6e65 5f6e 756d  ", x)', line_num
-000191e0: 6265 723d 322c 2063 6f6c 756d 6e5f 6e75  ber=2, column_nu
-000191f0: 6d62 6572 3d31 2c20 636f 6d6d 656e 743d  mber=1, comment=
-00019200: 2727 292c 0a20 2020 2020 2020 2020 2020  ''),.           
-00019210: 2020 2020 2020 2020 2027 2020 2020 7072           '    pr
-00019220: 696e 7428 2223 2074 6869 7320 6973 2071  int("# this is q
-00019230: 756f 7465 6422 2c20 7829 2729 2c0a 2020  uoted", x)'),.  
-00019240: 2020 2020 2020 2020 2020 2020 2020 284c                (L
-00019250: 4928 6c69 6e65 3d27 2020 2020 7072 696e  I(line='    prin
-00019260: 7428 2222 2920 2320 7468 6973 2022 636f  t("") # this "co
-00019270: 6d6d 656e 7422 2069 7320 7573 656c 6573  mment" is useles
-00019280: 7327 2c20 6c69 6e65 5f6e 756d 6265 723d  s', line_number=
-00019290: 332c 2063 6f6c 756d 6e5f 6e75 6d62 6572  3, column_number
-000192a0: 3d31 2c20 636f 6d6d 656e 743d 2723 2074  =1, comment='# t
-000192b0: 6869 7320 2263 6f6d 6d65 6e74 2220 6973  his "comment" is
-000192c0: 2075 7365 6c65 7373 2729 2c0a 2020 2020   useless'),.    
-000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192e0: 2720 2020 2070 7269 6e74 2822 2229 2729  '    print("")')
-000192f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019300: 2020 284c 4928 6c69 6e65 3d27 2020 2020    (LI(line='    
-00019310: 7072 696e 7428 6e6f 5f63 6f6d 6d65 6e74  print(no_comment
-00019320: 735f 6f72 5f71 756f 7465 735f 6f6e 5f74  s_or_quotes_on_t
-00019330: 6869 735f 6c69 6e65 2927 2c20 6c69 6e65  his_line)', line
-00019340: 5f6e 756d 6265 723d 342c 2063 6f6c 756d  _number=4, colum
-00019350: 6e5f 6e75 6d62 6572 3d31 2c20 636f 6d6d  n_number=1, comm
-00019360: 656e 743d 2727 292c 0a20 2020 2020 2020  ent=''),.       
-00019370: 2020 2020 2020 2020 2020 2020 2027 2020               '  
-00019380: 2020 7072 696e 7428 6e6f 5f63 6f6d 6d65    print(no_comme
-00019390: 6e74 735f 6f72 5f71 756f 7465 735f 6f6e  nts_or_quotes_on
-000193a0: 5f74 6869 735f 6c69 6e65 2927 292c 0a20  _this_line)'),. 
-000193b0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000193c0: 4c49 286c 696e 653d 2727 2c20 6c69 6e65  LI(line='', line
-000193d0: 5f6e 756d 6265 723d 352c 2063 6f6c 756d  _number=5, colum
-000193e0: 6e5f 6e75 6d62 6572 3d31 2c20 636f 6d6d  n_number=1, comm
-000193f0: 656e 743d 2727 292c 0a20 2020 2020 2020  ent=''),.       
-00019400: 2020 2020 2020 2020 2020 2020 2027 2729               '')
-00019410: 0a20 2020 2020 2020 2020 2020 205d 290a  .            ]).
-00019420: 0a20 2020 2020 2020 2074 6573 7428 6269  .        test(bi
-00019430: 672e 6c69 6e65 735f 7374 7269 705f 636f  g.lines_strip_co
-00019440: 6d6d 656e 7473 2862 6967 2e6c 696e 6573  mments(big.lines
-00019450: 2822 2222 0a66 6f72 2078 2069 6e20 7261  (""".for x in ra
-00019460: 6e67 6528 3529 3a20 2320 7468 6973 2069  nge(5): # this i
-00019470: 7320 6120 636f 6d6d 656e 740a 2020 2020  s a comment.    
-00019480: 7072 696e 7428 2223 2074 6869 7320 6973  print("# this is
-00019490: 2071 756f 7465 6422 2c20 7829 0a20 2020   quoted", x).   
-000194a0: 2070 7269 6e74 2822 2229 2023 2074 6869   print("") # thi
-000194b0: 7320 2263 6f6d 6d65 6e74 2220 6973 2075  s "comment" is u
-000194c0: 7365 6c65 7373 0a20 2020 2070 7269 6e74  seless.    print
-000194d0: 286e 6f5f 636f 6d6d 656e 7473 5f6f 725f  (no_comments_or_
-000194e0: 7175 6f74 6573 5f6f 6e5f 7468 6973 5f6c  quotes_on_this_l
-000194f0: 696e 6529 0a22 2222 5b31 3a5d 292c 2028  ine)."""[1:]), (
-00019500: 2223 222c 2022 2f2f 2229 2c20 7175 6f74  "#", "//"), quot
-00019510: 6573 3d4e 6f6e 6529 2c0a 2020 2020 2020  es=None),.      
-00019520: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00019530: 2020 2020 2020 2020 284c 4928 6c69 6e65          (LI(line
-00019540: 3d27 666f 7220 7820 696e 2072 616e 6765  ='for x in range
-00019550: 2835 293a 2023 2074 6869 7320 6973 2061  (5): # this is a
-00019560: 2063 6f6d 6d65 6e74 272c 206c 696e 655f   comment', line_
-00019570: 6e75 6d62 6572 3d31 2c20 636f 6c75 6d6e  number=1, column
-00019580: 5f6e 756d 6265 723d 312c 2063 6f6d 6d65  _number=1, comme
-00019590: 6e74 3d27 2320 7468 6973 2069 7320 6120  nt='# this is a 
-000195a0: 636f 6d6d 656e 7427 292c 0a20 2020 2020  comment'),.     
-000195b0: 2020 2020 2020 2020 2020 2020 2027 666f               'fo
-000195c0: 7220 7820 696e 2072 616e 6765 2835 293a  r x in range(5):
-000195d0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000195e0: 2020 2020 284c 4928 6c69 6e65 3d27 2020      (LI(line='  
-000195f0: 2020 7072 696e 7428 2223 2074 6869 7320    print("# this 
-00019600: 6973 2071 756f 7465 6422 2c20 7829 272c  is quoted", x)',
-00019610: 206c 696e 655f 6e75 6d62 6572 3d32 2c20   line_number=2, 
-00019620: 636f 6c75 6d6e 5f6e 756d 6265 723d 312c  column_number=1,
-00019630: 2063 6f6d 6d65 6e74 3d27 2320 7468 6973   comment='# this
-00019640: 2069 7320 7175 6f74 6564 222c 2078 2927   is quoted", x)'
-00019650: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00019660: 2020 2020 2020 2027 2020 2020 7072 696e         '    prin
-00019670: 7428 2227 292c 0a20 2020 2020 2020 2020  t("'),.         
-00019680: 2020 2020 2020 2028 4c49 286c 696e 653d         (LI(line=
-00019690: 2720 2020 2070 7269 6e74 2822 2229 2023  '    print("") #
-000196a0: 2074 6869 7320 2263 6f6d 6d65 6e74 2220   this "comment" 
-000196b0: 6973 2075 7365 6c65 7373 272c 206c 696e  is useless', lin
-000196c0: 655f 6e75 6d62 6572 3d33 2c20 636f 6c75  e_number=3, colu
-000196d0: 6d6e 5f6e 756d 6265 723d 312c 2063 6f6d  mn_number=1, com
-000196e0: 6d65 6e74 3d27 2320 7468 6973 2022 636f  ment='# this "co
-000196f0: 6d6d 656e 7422 2069 7320 7573 656c 6573  mment" is useles
-00019700: 7327 292c 0a20 2020 2020 2020 2020 2020  s'),.           
-00019710: 2020 2020 2020 2020 2027 2020 2020 7072           '    pr
-00019720: 696e 7428 2222 2927 292c 0a20 2020 2020  int("")'),.     
-00019730: 2020 2020 2020 2020 2020 2028 4c49 286c             (LI(l
-00019740: 696e 653d 2720 2020 2070 7269 6e74 286e  ine='    print(n
-00019750: 6f5f 636f 6d6d 656e 7473 5f6f 725f 7175  o_comments_or_qu
-00019760: 6f74 6573 5f6f 6e5f 7468 6973 5f6c 696e  otes_on_this_lin
-00019770: 6529 272c 206c 696e 655f 6e75 6d62 6572  e)', line_number
-00019780: 3d34 2c20 636f 6c75 6d6e 5f6e 756d 6265  =4, column_numbe
-00019790: 723d 312c 2063 6f6d 6d65 6e74 3d27 2729  r=1, comment='')
-000197a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000197b0: 2020 2020 2020 2720 2020 2070 7269 6e74        '    print
-000197c0: 286e 6f5f 636f 6d6d 656e 7473 5f6f 725f  (no_comments_or_
-000197d0: 7175 6f74 6573 5f6f 6e5f 7468 6973 5f6c  quotes_on_this_l
-000197e0: 696e 6529 2729 2c0a 2020 2020 2020 2020  ine)'),.        
-000197f0: 2020 2020 2020 2020 284c 4928 6c69 6e65          (LI(line
-00019800: 3d27 272c 206c 696e 655f 6e75 6d62 6572  ='', line_number
-00019810: 3d35 2c20 636f 6c75 6d6e 5f6e 756d 6265  =5, column_numbe
-00019820: 723d 312c 2063 6f6d 6d65 6e74 3d27 2729  r=1, comment='')
-00019830: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019840: 2020 2020 2020 2727 292c 0a20 2020 2020        ''),.     
-00019850: 2020 2020 2020 205d 290a 0a20 2020 2020         ])..     
-00019860: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-00019870: 6572 7452 6169 7365 7328 5661 6c75 6545  ertRaises(ValueE
-00019880: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-00019890: 2020 2074 6573 7428 6269 672e 6c69 6e65     test(big.line
-000198a0: 735f 7374 7269 705f 636f 6d6d 656e 7473  s_strip_comments
-000198b0: 2862 6967 2e6c 696e 6573 2822 615c 6e62  (big.lines("a\nb
-000198c0: 5c6e 2229 2c20 4e6f 6e65 292c 205b 5d29  \n"), None), [])
-000198d0: 0a0a 2020 2020 2020 2020 7465 7374 2862  ..        test(b
-000198e0: 6967 2e6c 696e 6573 5f73 7472 6970 5f63  ig.lines_strip_c
-000198f0: 6f6d 6d65 6e74 7328 6269 672e 6c69 6e65  omments(big.line
-00019900: 7328 6222 615c 6e62 2320 6967 6e6f 7265  s(b"a\nb# ignore
-00019910: 645c 6e20 6322 292c 2062 2723 2729 2c0a  d\n c"), b'#'),.
-00019920: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-00019930: 2020 2020 2020 2020 2020 4c28 6227 6127            L(b'a'
-00019940: 2c20 312c 2063 6f6d 6d65 6e74 3d62 2727  , 1, comment=b''
-00019950: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00019960: 4c49 2862 2762 2320 6967 6e6f 7265 6427  LI(b'b# ignored'
-00019970: 2c20 322c 2031 2c20 636f 6d6d 656e 743d  , 2, 1, comment=
-00019980: 6227 2320 6967 6e6f 7265 6427 292c 2062  b'# ignored'), b
-00019990: 2762 2729 2c0a 2020 2020 2020 2020 2020  'b'),.          
-000199a0: 2020 4c28 6227 2063 272c 2033 2c20 636f    L(b' c', 3, co
-000199b0: 6d6d 656e 743d 6227 2729 2c0a 2020 2020  mment=b''),.    
-000199c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000199d0: 2020 2020 2020 290a 0a0a 2020 2020 2020        )...      
-000199e0: 2020 7465 7374 2862 6967 2e6c 696e 6573    test(big.lines
-000199f0: 5f66 696c 7465 725f 656d 7074 795f 6c69  _filter_empty_li
-00019a00: 6e65 7328 6269 672e 6c69 6e65 735f 6669  nes(big.lines_fi
-00019a10: 6c74 6572 5f63 6f6d 6d65 6e74 5f6c 696e  lter_comment_lin
-00019a20: 6573 2862 6967 2e6c 696e 6573 5f73 7472  es(big.lines_str
-00019a30: 6970 2862 6967 2e6c 696e 6573 280a 2220  ip(big.lines(." 
-00019a40: 2020 5c6e 2220 2b0a 2220 2020 2061 203d    \n" +."    a =
-00019a50: 2062 205c 6e22 202b 0a22 2020 205c 6e22   b \n" +."   \n"
-00019a60: 202b 0a22 2020 2020 2320 636f 6d6d 656e   +."    # commen
-00019a70: 7420 6c69 6e65 205c 6e22 202b 0a22 2020  t line \n" +."  
-00019a80: 2020 5c6e 2220 2b0a 2220 2020 205c 6e22    \n" +."    \n"
-00019a90: 202b 0a22 2020 2020 6320 3d20 6420 205c   +."    c = d  \
-00019aa0: 6e22 202b 0a22 2020 2020 205c 6e22 2929  n" +."     \n"))
-00019ab0: 2c20 2723 2729 292c 0a20 2020 2020 2020  , '#')),.       
-00019ac0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00019ad0: 2020 2028 4c49 2827 2020 2020 6120 3d20     (LI('    a = 
-00019ae0: 6220 272c 2020 322c 2035 2c20 6c65 6164  b ',  2, 5, lead
-00019af0: 696e 673d 2720 2020 2027 292c 2027 6120  ing='    '), 'a 
-00019b00: 3d20 6227 292c 0a20 2020 2020 2020 2020  = b'),.         
-00019b10: 2020 2028 4c49 2827 2020 2020 6320 3d20     (LI('    c = 
-00019b20: 6420 2027 2c20 372c 2035 2c20 6c65 6164  d  ', 7, 5, lead
-00019b30: 696e 673d 2720 2020 2027 292c 2027 6320  ing='    '), 'c 
-00019b40: 3d20 6427 292c 0a20 2020 2020 2020 2020  = d'),.         
-00019b50: 2020 205d 290a 0a0a 2020 2020 6465 6620     ])...    def 
-00019b60: 7465 7374 5f6c 696e 6573 5f73 7472 6970  test_lines_strip
-00019b70: 5f69 6e64 656e 7428 7365 6c66 293a 0a20  _indent(self):. 
-00019b80: 2020 2020 2020 2064 6566 2074 6573 7428         def test(
-00019b90: 6c69 6e65 732c 2065 7870 6563 7465 642c  lines, expected,
-00019ba0: 202a 2c20 7461 625f 7769 6474 683d 3829   *, tab_width=8)
-00019bb0: 3a0a 2020 2020 2020 2020 2020 2020 676f  :.            go
-00019bc0: 7420 3d20 6c69 7374 2862 6967 2e6c 696e  t = list(big.lin
-00019bd0: 6573 5f73 7472 6970 5f69 6e64 656e 7428  es_strip_indent(
-00019be0: 6269 672e 6c69 6e65 7328 6c69 6e65 732c  big.lines(lines,
-00019bf0: 2074 6162 5f77 6964 7468 3d74 6162 5f77   tab_width=tab_w
-00019c00: 6964 7468 2929 290a 2020 2020 2020 2020  idth))).        
-00019c10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00019c20: 7175 616c 2867 6f74 2c20 6578 7065 6374  qual(got, expect
-00019c30: 6564 290a 0a0a 2020 2020 2020 2020 4c69  ed)...        Li
-00019c40: 6e65 496e 666f 203d 2062 6967 2e74 6578  neInfo = big.tex
-00019c50: 742e 4c69 6e65 496e 666f 0a0a 2020 2020  t.LineInfo..    
-00019c60: 2020 2020 6c69 6e65 7320 3d20 2222 220a      lines = """.
-00019c70: 6c65 6674 206d 6172 6769 6e0a 6966 2033  left margin.if 3
-00019c80: 3a0a 2020 2020 7465 7874 0a65 6c73 653a  :.    text.else:
-00019c90: 0a20 2020 2069 6620 313a 0a20 2020 2020  .    if 1:.     
-00019ca0: 2020 2020 206f 7468 6572 2074 6578 740a       other text.
-00019cb0: 2020 2020 2020 2020 2020 6f74 6865 7220            other 
-00019cc0: 7465 7874 0a20 2020 206d 6f72 6520 7465  text.    more te
-00019cd0: 7874 0a20 2020 2020 2064 6966 6665 7265  xt.      differe
-00019ce0: 6e74 2069 6e64 656e 740a 2020 2020 6f75  nt indent.    ou
-00019cf0: 7464 656e 740a 6f75 7464 656e 740a 2020  tdent.outdent.  
-00019d00: 6e65 7720 696e 6465 6e74 0a6f 7574 6465  new indent.outde
-00019d10: 6e74 0a22 2222 0a0a 2020 2020 2020 2020  nt."""..        
-00019d20: 6578 7065 6374 6564 203d 205b 0a20 2020  expected = [.   
-00019d30: 2020 2020 2020 2020 2028 4c69 6e65 496e           (LineIn
-00019d40: 666f 286c 696e 653d 2727 2c20 6c69 6e65  fo(line='', line
-00019d50: 5f6e 756d 6265 723d 312c 2063 6f6c 756d  _number=1, colum
-00019d60: 6e5f 6e75 6d62 6572 3d31 2c20 696e 6465  n_number=1, inde
-00019d70: 6e74 3d30 2c20 6c65 6164 696e 673d 2727  nt=0, leading=''
-00019d80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00019d90: 2020 2027 2729 2c0a 2020 2020 2020 2020     ''),.        
-00019da0: 2020 2020 284c 696e 6549 6e66 6f28 6c69      (LineInfo(li
-00019db0: 6e65 3d27 6c65 6674 206d 6172 6769 6e27  ne='left margin'
-00019dc0: 2c20 6c69 6e65 5f6e 756d 6265 723d 322c  , line_number=2,
-00019dd0: 2063 6f6c 756d 6e5f 6e75 6d62 6572 3d31   column_number=1
-00019de0: 2c20 696e 6465 6e74 3d30 2c20 6c65 6164  , indent=0, lead
-00019df0: 696e 673d 2727 292c 0a20 2020 2020 2020  ing=''),.       
-00019e00: 2020 2020 2020 2020 2027 6c65 6674 206d           'left m
-00019e10: 6172 6769 6e27 292c 0a20 2020 2020 2020  argin'),.       
-00019e20: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
-00019e30: 696e 653d 2769 6620 333a 272c 206c 696e  ine='if 3:', lin
-00019e40: 655f 6e75 6d62 6572 3d33 2c20 636f 6c75  e_number=3, colu
-00019e50: 6d6e 5f6e 756d 6265 723d 312c 2069 6e64  mn_number=1, ind
-00019e60: 656e 743d 302c 206c 6561 6469 6e67 3d27  ent=0, leading='
-00019e70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00019e80: 2020 2020 2769 6620 333a 2729 2c0a 2020      'if 3:'),.  
-00019e90: 2020 2020 2020 2020 2020 284c 696e 6549            (LineI
-00019ea0: 6e66 6f28 6c69 6e65 3d27 2020 2020 7465  nfo(line='    te
-00019eb0: 7874 272c 206c 696e 655f 6e75 6d62 6572  xt', line_number
-00019ec0: 3d34 2c20 636f 6c75 6d6e 5f6e 756d 6265  =4, column_numbe
-00019ed0: 723d 352c 2069 6e64 656e 743d 312c 206c  r=5, indent=1, l
-00019ee0: 6561 6469 6e67 3d27 2020 2020 2729 2c0a  eading='    '),.
-00019ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f00: 2774 6578 7427 292c 0a20 2020 2020 2020  'text'),.       
-00019f10: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
-00019f20: 696e 653d 2765 6c73 653a 272c 206c 696e  ine='else:', lin
-00019f30: 655f 6e75 6d62 6572 3d35 2c20 636f 6c75  e_number=5, colu
-00019f40: 6d6e 5f6e 756d 6265 723d 312c 2069 6e64  mn_number=1, ind
-00019f50: 656e 743d 302c 206c 6561 6469 6e67 3d27  ent=0, leading='
-00019f60: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00019f70: 2020 2020 2765 6c73 653a 2729 2c0a 2020      'else:'),.  
-00019f80: 2020 2020 2020 2020 2020 284c 696e 6549            (LineI
-00019f90: 6e66 6f28 6c69 6e65 3d27 2020 2020 6966  nfo(line='    if
-00019fa0: 2031 3a27 2c20 6c69 6e65 5f6e 756d 6265   1:', line_numbe
-00019fb0: 723d 362c 2063 6f6c 756d 6e5f 6e75 6d62  r=6, column_numb
-00019fc0: 6572 3d35 2c20 696e 6465 6e74 3d31 2c20  er=5, indent=1, 
-00019fd0: 6c65 6164 696e 673d 2720 2020 2027 292c  leading='    '),
-00019fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ff0: 2027 6966 2031 3a27 292c 0a20 2020 2020   'if 1:'),.     
-0001a000: 2020 2020 2020 2028 4c69 6e65 496e 666f         (LineInfo
-0001a010: 286c 696e 653d 2720 2020 2020 2020 2020  (line='         
-0001a020: 206f 7468 6572 2074 6578 7427 2c20 6c69   other text', li
-0001a030: 6e65 5f6e 756d 6265 723d 372c 2063 6f6c  ne_number=7, col
-0001a040: 756d 6e5f 6e75 6d62 6572 3d31 312c 2069  umn_number=11, i
-0001a050: 6e64 656e 743d 322c 206c 6561 6469 6e67  ndent=2, leading
-0001a060: 3d27 2020 2020 2020 2020 2020 2729 2c0a  ='          '),.
+00017850: 7465 733d 4661 6c73 6529 0a0a 2020 2020  tes=False)..    
+00017860: 6465 6620 7465 7374 5f70 6172 7365 5f64  def test_parse_d
+00017870: 656c 696d 6974 6572 7328 7365 6c66 293a  elimiters(self):
+00017880: 0a0a 2020 2020 2020 2020 6465 6620 7465  ..        def te
+00017890: 7374 2873 2c20 6578 7065 6374 6564 2c20  st(s, expected, 
+000178a0: 2a2c 2064 656c 696d 6974 6572 733d 4e6f  *, delimiters=No
+000178b0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+000178c0: 2065 6d70 7479 203d 2027 270a 2020 2020   empty = ''.    
+000178d0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+000178e0: 2072 616e 6765 2832 293a 0a20 2020 2020   range(2):.     
+000178f0: 2020 2020 2020 2020 2020 2067 6f74 203d             got =
+00017900: 2074 7570 6c65 2862 6967 2e70 6172 7365   tuple(big.parse
+00017910: 5f64 656c 696d 6974 6572 7328 732c 2064  _delimiters(s, d
+00017920: 656c 696d 6974 6572 733d 6465 6c69 6d69  elimiters=delimi
+00017930: 7465 7273 2929 0a0a 2020 2020 2020 2020  ters))..        
+00017940: 2020 2020 2020 2020 666c 6174 7465 6e65          flattene
+00017950: 6420 3d20 5b5d 0a20 2020 2020 2020 2020  d = [].         
+00017960: 2020 2020 2020 2066 6f72 2074 2069 6e20         for t in 
+00017970: 676f 743a 0a20 2020 2020 2020 2020 2020  got:.           
+00017980: 2020 2020 2020 2020 2066 6c61 7474 656e           flatten
+00017990: 6564 2e65 7874 656e 6428 7429 0a20 2020  ed.extend(t).   
+000179a0: 2020 2020 2020 2020 2020 2020 2073 3220               s2 
+000179b0: 3d20 656d 7074 792e 6a6f 696e 2866 6c61  = empty.join(fla
+000179c0: 7474 656e 6564 290a 2020 2020 2020 2020  ttened).        
+000179d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000179e0: 6572 7445 7175 616c 2873 2c20 7332 290a  ertEqual(s, s2).
+000179f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a00: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00017a10: 6c28 6578 7065 6374 6564 2c20 676f 7429  l(expected, got)
+00017a20: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017a30: 2020 6966 206e 6f74 2069 3a0a 2020 2020    if not i:.    
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a50: 7320 3d20 746f 5f62 7974 6573 2873 290a  s = to_bytes(s).
+00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a70: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
+00017a80: 6f5f 6279 7465 7328 6578 7065 6374 6564  o_bytes(expected
+00017a90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017aa0: 2020 2020 2020 656d 7074 7920 3d20 6227        empty = b'
+00017ab0: 270a 0a20 2020 2020 2020 2074 6573 7428  '..        test(
+00017ac0: 2761 5b78 5d20 3d20 666f 6f28 2268 6f77  'a[x] = foo("how
+00017ad0: 6479 2028 666f 6c6b 7329 5c5c 6e22 2c20  dy (folks)\\n", 
+00017ae0: 7b31 3a32 2c20 333a 347d 2927 2c0a 2020  {1:2, 3:4})',.  
+00017af0: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
+00017b00: 2020 2020 2020 2020 2020 2020 2827 6127              ('a'
+00017b10: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+00017b20: 2027 5b27 2c20 2027 2729 2c0a 2020 2020   '[',  ''),.    
+00017b30: 2020 2020 2020 2020 2020 2020 2827 7827              ('x'
+00017b40: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+00017b50: 2020 2727 2c20 275d 2729 2c0a 2020 2020    '', ']'),.    
+00017b60: 2020 2020 2020 2020 2020 2020 2827 203d              (' =
+00017b70: 2066 6f6f 272c 2020 2020 2020 2020 2020   foo',          
+00017b80: 2027 2827 2c20 2027 2729 2c0a 2020 2020   '(',  ''),.    
+00017b90: 2020 2020 2020 2020 2020 2020 2827 272c              ('',
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bb0: 2027 2227 2c20 2027 2729 2c0a 2020 2020   '"',  ''),.    
+00017bc0: 2020 2020 2020 2020 2020 2020 2827 686f              ('ho
+00017bd0: 7764 7920 2866 6f6c 6b73 295c 5c6e 272c  wdy (folks)\\n',
+00017be0: 2020 2727 2c20 2722 2729 2c0a 2020 2020    '', '"'),.    
+00017bf0: 2020 2020 2020 2020 2020 2020 2827 2c20              (', 
+00017c00: 272c 2020 2020 2020 2020 2020 2020 2020  ',              
+00017c10: 2027 7b27 2c20 2027 2729 2c0a 2020 2020   '{',  ''),.    
+00017c20: 2020 2020 2020 2020 2020 2020 2827 313a              ('1:
+00017c30: 322c 2033 3a34 272c 2020 2020 2020 2020  2, 3:4',        
+00017c40: 2020 2727 2c20 277d 2729 2c0a 2020 2020    '', '}'),.    
+00017c50: 2020 2020 2020 2020 2020 2020 2827 272c              ('',
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c70: 2020 2727 2c20 2729 2729 2c0a 2020 2020    '', ')'),.    
+00017c80: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00017c90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00017ca0: 2020 7465 7374 2827 615b 5b5b 7a5d 5d5d    test('a[[[z]]]
+00017cb0: 7b7b 7b7b 717d 7d7d 7d5b 7b5b 7b5b 7b5b  {{{{q}}}}[{[{[{[
+00017cc0: 7b7a 7d5d 7d5d 7d5d 7d5d 2127 2c0a 2020  {z}]}]}]}]!',.  
+00017cd0: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
+00017ce0: 2020 2020 2020 2020 2020 2020 2827 6127              ('a'
+00017cf0: 2c20 275b 272c 2020 2727 292c 0a20 2020  , '[',  ''),.   
+00017d00: 2020 2020 2020 2020 2020 2020 2028 2727               (''
+00017d10: 2c20 2027 5b27 2c20 2027 2729 2c0a 2020  ,  '[',  ''),.  
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2827                ('
+00017d30: 272c 2020 275b 272c 2020 2727 292c 0a20  ',  '[',  ''),. 
+00017d40: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00017d50: 277a 272c 2020 2727 2c20 275d 2729 2c0a  'z',  '', ']'),.
+00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d70: 2827 272c 2020 2027 272c 2027 5d27 292c  ('',   '', ']'),
+00017d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d90: 2028 2727 2c20 2020 2727 2c20 275d 2729   ('',   '', ']')
+00017da0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017db0: 2020 2827 272c 2020 277b 272c 2020 2727    ('',  '{',  ''
+00017dc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00017dd0: 2020 2028 2727 2c20 2027 7b27 2c20 2027     ('',  '{',  '
+00017de0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00017df0: 2020 2020 2827 272c 2020 277b 272c 2020      ('',  '{',  
+00017e00: 2727 292c 0a20 2020 2020 2020 2020 2020  ''),.           
+00017e10: 2020 2020 2028 2727 2c20 2027 7b27 2c20       ('',  '{', 
+00017e20: 2027 2729 2c0a 2020 2020 2020 2020 2020   ''),.          
+00017e30: 2020 2020 2020 2827 7127 2c20 2027 272c        ('q',  '',
+00017e40: 2027 7d27 292c 0a20 2020 2020 2020 2020   '}'),.         
+00017e50: 2020 2020 2020 2028 2727 2c20 2020 2727         ('',   ''
+00017e60: 2c20 277d 2729 2c0a 2020 2020 2020 2020  , '}'),.        
+00017e70: 2020 2020 2020 2020 2827 272c 2020 2027          ('',   '
+00017e80: 272c 2027 7d27 292c 0a20 2020 2020 2020  ', '}'),.       
+00017e90: 2020 2020 2020 2020 2028 2727 2c20 2020           ('',   
+00017ea0: 2727 2c20 277d 2729 2c0a 2020 2020 2020  '', '}'),.      
+00017eb0: 2020 2020 2020 2020 2020 2827 272c 2020            ('',  
+00017ec0: 275b 272c 2020 2727 292c 0a20 2020 2020  '[',  ''),.     
+00017ed0: 2020 2020 2020 2020 2020 2028 2727 2c20             ('', 
+00017ee0: 2027 7b27 2c20 2027 2729 2c0a 2020 2020   '{',  ''),.    
+00017ef0: 2020 2020 2020 2020 2020 2020 2827 272c              ('',
+00017f00: 2020 275b 272c 2020 2727 292c 0a20 2020    '[',  ''),.   
+00017f10: 2020 2020 2020 2020 2020 2020 2028 2727               (''
+00017f20: 2c20 2027 7b27 2c20 2027 2729 2c0a 2020  ,  '{',  ''),.  
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2827                ('
+00017f40: 272c 2020 275b 272c 2020 2727 292c 0a20  ',  '[',  ''),. 
+00017f50: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00017f60: 2727 2c20 2027 7b27 2c20 2027 2729 2c0a  '',  '{',  ''),.
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 2827 272c 2020 275b 272c 2020 2727 292c  ('',  '[',  ''),
+00017f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017fa0: 2028 2727 2c20 2027 7b27 2c20 2027 2729   ('',  '{',  '')
+00017fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017fc0: 2020 2827 7a27 2c20 2027 272c 2027 7d27    ('z',  '', '}'
+00017fd0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00017fe0: 2020 2028 2727 2c20 2020 2727 2c20 275d     ('',   '', ']
+00017ff0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00018000: 2020 2020 2827 272c 2020 2027 272c 2027      ('',   '', '
+00018010: 7d27 292c 0a20 2020 2020 2020 2020 2020  }'),.           
+00018020: 2020 2020 2028 2727 2c20 2020 2727 2c20       ('',   '', 
+00018030: 275d 2729 2c0a 2020 2020 2020 2020 2020  ']'),.          
+00018040: 2020 2020 2020 2827 272c 2020 2027 272c        ('',   '',
+00018050: 2027 7d27 292c 0a20 2020 2020 2020 2020   '}'),.         
+00018060: 2020 2020 2020 2028 2727 2c20 2020 2727         ('',   ''
+00018070: 2c20 275d 2729 2c0a 2020 2020 2020 2020  , ']'),.        
+00018080: 2020 2020 2020 2020 2827 272c 2020 2027          ('',   '
+00018090: 272c 2027 7d27 292c 0a20 2020 2020 2020  ', '}'),.       
+000180a0: 2020 2020 2020 2020 2028 2727 2c20 2020           ('',   
+000180b0: 2727 2c20 275d 2729 2c0a 2020 2020 2020  '', ']'),.      
+000180c0: 2020 2020 2020 2020 2020 2827 2127 2c20            ('!', 
+000180d0: 2027 272c 2020 2727 292c 0a20 2020 2020   '',  ''),.     
+000180e0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000180f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00018100: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+00018110: 7452 6169 7365 7328 5661 6c75 6545 7272  tRaises(ValueErr
+00018120: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00018130: 2074 6573 7428 2761 5b33 2927 2c20 4e6f   test('a[3)', No
+00018140: 6e65 290a 2020 2020 2020 2020 7769 7468  ne).        with
+00018150: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00018160: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00018170: 2020 2020 2020 2020 2020 2020 7465 7374              test
+00018180: 2827 617b 335d 272c 204e 6f6e 6529 0a20  ('a{3]', None). 
+00018190: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000181a0: 2e61 7373 6572 7452 6169 7365 7328 5661  .assertRaises(Va
+000181b0: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+000181c0: 2020 2020 2020 2074 6573 7428 2761 2833         test('a(3
+000181d0: 7d27 2c20 4e6f 6e65 290a 0a20 2020 2020  }', None)..     
+000181e0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+000181f0: 6572 7452 6169 7365 7328 5661 6c75 6545  ertRaises(ValueE
+00018200: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+00018210: 2020 2074 6573 7428 2764 656c 696d 6974     test('delimit
+00018220: 6572 7320 6973 2065 6d70 7479 272c 204e  ers is empty', N
+00018230: 6f6e 652c 2064 656c 696d 6974 6572 733d  one, delimiters=
+00018240: 5b5d 290a 2020 2020 2020 2020 7769 7468  []).        with
+00018250: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00018260: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00018270: 2020 2020 2020 2020 2020 2020 7465 7374              test
+00018280: 2827 6465 6c69 6d69 7465 7220 6973 2061  ('delimiter is a
+00018290: 6263 2028 6875 6821 2927 2c20 4e6f 6e65  bc (huh!)', None
+000182a0: 2c20 6465 6c69 6d69 7465 7273 3d5b 2728  , delimiters=['(
+000182b0: 2927 2c20 2761 6263 275d 290a 2020 2020  )', 'abc']).    
+000182c0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+000182d0: 7365 7274 5261 6973 6573 2854 7970 6545  sertRaises(TypeE
+000182e0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+000182f0: 2020 2074 6573 7428 2764 656c 696d 6974     test('delimit
+00018300: 6572 7320 636f 6e74 6169 6e73 2033 272c  ers contains 3',
+00018310: 204e 6f6e 652c 2064 656c 696d 6974 6572   None, delimiter
+00018320: 733d 5b27 7b7d 272c 2033 5d29 0a20 2020  s=['{}', 3]).   
+00018330: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00018340: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
+00018350: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+00018360: 2020 2020 2074 6573 7428 2764 656c 696d       test('delim
+00018370: 6974 6572 7320 636f 6e74 6169 6e73 2061  iters contains a
+00018380: 203c 6261 636b 736c 6173 683e 272c 204e   <backslash>', N
+00018390: 6f6e 652c 2064 656c 696d 6974 6572 733d  one, delimiters=
+000183a0: 5b27 3c3e 272c 2027 5c5c 2f27 5d29 0a20  ['<>', '\\/']). 
+000183b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000183c0: 2e61 7373 6572 7452 6169 7365 7328 5661  .assertRaises(Va
+000183d0: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+000183e0: 2020 2020 2020 2074 6573 7428 2764 656c         test('del
+000183f0: 696d 6974 6572 7320 636f 6e74 6169 6e73  imiters contains
+00018400: 203c 616e 676c 653e 203c 6272 6163 6b65   <angle> <bracke
+00018410: 7473 3e20 3c74 7769 6365 3e27 2c20 4e6f  ts> <twice>', No
+00018420: 6e65 2c20 6465 6c69 6d69 7465 7273 3d5b  ne, delimiters=[
+00018430: 273c 3e27 2c20 273c 3e27 5d29 0a0a 2020  '<>', '<>'])..  
+00018440: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00018450: 6173 7365 7274 5261 6973 6573 2856 616c  assertRaises(Val
+00018460: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
+00018470: 2020 2020 2020 7465 7374 2827 756e 636c        test('uncl
+00018480: 6f73 6564 5f70 6172 656e 2861 5b33 5d27  osed_paren(a[3]'
+00018490: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+000184a0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+000184b0: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
+000184c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000184d0: 7465 7374 2827 785b 335d 203d 2075 6e63  test('x[3] = unc
+000184e0: 6c6f 7365 645f 6375 726c 797b 272c 204e  losed_curly{', N
+000184f0: 6f6e 6529 0a20 2020 2020 2020 2077 6974  one).        wit
+00018500: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+00018510: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
+00018520: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
+00018530: 7428 2766 6f6f 2861 5b31 5d2c 207b 615b  t('foo(a[1], {a[
+00018540: 325d 3a20 3333 7d29 203d 2075 6e63 6c6f  2]: 33}) = unclo
+00018550: 7365 645f 7371 7561 7265 5b35 3527 2c20  sed_square[55', 
+00018560: 4e6f 6e65 290a 2020 2020 2020 2020 7769  None).        wi
+00018570: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+00018580: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+00018590: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+000185a0: 7374 2827 2275 6e74 6572 6d69 6e61 7465  st('"unterminate
+000185b0: 6420 7374 7269 6e67 5c5c 272c 204e 6f6e  d string\\', Non
+000185c0: 6529 0a20 2020 2020 2020 2077 6974 6820  e).        with 
+000185d0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+000185e0: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
+000185f0: 2020 2020 2020 2020 2020 2074 6573 7428             test(
+00018600: 276f 7065 6e5f 6576 6572 7974 6869 6e67  'open_everything
+00018610: 2820 7b20 615b 3335 2022 666f 6f27 2c20  ( { a[35 "foo', 
+00018620: 4e6f 6e65 290a 0a20 2020 2020 2020 2077  None)..        w
+00018630: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00018640: 6169 7365 7328 5479 7065 4572 726f 7229  aises(TypeError)
+00018650: 3a0a 2020 2020 2020 2020 2020 2020 6269  :.            bi
+00018660: 672e 4465 6c69 6d69 7465 7228 2728 272c  g.Delimiter('(',
+00018670: 2062 2729 2729 0a20 2020 2020 2020 2077   b')').        w
+00018680: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00018690: 6169 7365 7328 5479 7065 4572 726f 7229  aises(TypeError)
+000186a0: 3a0a 2020 2020 2020 2020 2020 2020 6269  :.            bi
+000186b0: 672e 4465 6c69 6d69 7465 7228 6227 2827  g.Delimiter(b'('
+000186c0: 2c20 2729 2729 0a0a 2020 2020 6465 6620  , ')')..    def 
+000186d0: 7465 7374 5f6c 696e 6573 2873 656c 6629  test_lines(self)
+000186e0: 3a0a 2020 2020 2020 2020 6465 6620 7465  :.        def te
+000186f0: 7374 2869 2c20 6578 7065 6374 6564 293a  st(i, expected):
+00018700: 0a20 2020 2020 2020 2020 2020 2067 6f74  .            got
+00018710: 203d 206c 6973 7428 6929 0a20 2020 2020   = list(i).     
+00018720: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00018730: 7274 4571 7561 6c28 676f 742c 2065 7870  rtEqual(got, exp
+00018740: 6563 7465 6429 0a0a 2020 2020 2020 2020  ected)..        
+00018750: 4c49 203d 2062 6967 2e4c 696e 6549 6e66  LI = big.LineInf
+00018760: 6f0a 0a20 2020 2020 2020 2064 6566 204c  o..        def L
+00018770: 286c 696e 652c 206c 696e 655f 6e75 6d62  (line, line_numb
+00018780: 6572 2c20 636f 6c75 6d6e 5f6e 756d 6265  er, column_numbe
+00018790: 723d 312c 202a 2a6b 7761 7267 7329 3a0a  r=1, **kwargs):.
+000187a0: 2020 2020 2020 2020 2020 2020 696e 666f              info
+000187b0: 203d 2062 6967 2e4c 696e 6549 6e66 6f28   = big.LineInfo(
+000187c0: 6c69 6e65 2c20 6c69 6e65 5f6e 756d 6265  line, line_numbe
+000187d0: 722c 2063 6f6c 756d 6e5f 6e75 6d62 6572  r, column_number
+000187e0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+000187f0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00018800: 696e 666f 2c20 6c69 6e65 290a 0a20 2020  info, line)..   
+00018810: 2020 2020 2074 6573 7428 6269 672e 6c69       test(big.li
+00018820: 6e65 7328 2261 5c6e 625c 6e63 5c6e 645c  nes("a\nb\nc\nd\
+00018830: 6e65 5c6e 2229 2c0a 2020 2020 2020 2020  ne\n"),.        
+00018840: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00018850: 2020 284c 4928 2761 272c 2031 2c20 3129    (LI('a', 1, 1)
+00018860: 2c20 2761 2729 2c0a 2020 2020 2020 2020  , 'a'),.        
+00018870: 2020 2020 284c 4928 2762 272c 2032 2c20      (LI('b', 2, 
+00018880: 3129 2c20 2762 2729 2c0a 2020 2020 2020  1), 'b'),.      
+00018890: 2020 2020 2020 284c 4928 2763 272c 2033        (LI('c', 3
+000188a0: 2c20 3129 2c20 2763 2729 2c0a 2020 2020  , 1), 'c'),.    
+000188b0: 2020 2020 2020 2020 284c 4928 2764 272c          (LI('d',
+000188c0: 2034 2c20 3129 2c20 2764 2729 2c0a 2020   4, 1), 'd'),.  
+000188d0: 2020 2020 2020 2020 2020 284c 4928 2765            (LI('e
+000188e0: 272c 2035 2c20 3129 2c20 2765 2729 2c0a  ', 5, 1), 'e'),.
+000188f0: 2020 2020 2020 2020 2020 2020 284c 4928              (LI(
+00018900: 2727 2c20 2036 2c20 3129 2c20 2727 292c  '',  6, 1), ''),
+00018910: 0a20 2020 2020 2020 2020 2020 205d 290a  .            ]).
+00018920: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+00018930: 205b 2766 6972 7374 206c 696e 6527 2c20   ['first line', 
+00018940: 275c 7473 6563 6f6e 6420 6c69 6e65 272c  '\tsecond line',
+00018950: 2027 7468 6972 6420 6c69 6e65 275d 0a20   'third line']. 
+00018960: 2020 2020 2020 2074 6573 7428 6269 672e         test(big.
+00018970: 6c69 6e65 735f 7374 7269 7028 6269 672e  lines_strip(big.
+00018980: 6c69 6e65 7328 6c69 6e65 7329 292c 0a20  lines(lines)),. 
+00018990: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+000189a0: 2020 2020 2020 2020 2028 4c49 2827 6669           (LI('fi
+000189b0: 7273 7420 6c69 6e65 272c 2031 2c20 3129  rst line', 1, 1)
+000189c0: 2c20 2766 6972 7374 206c 696e 6527 292c  , 'first line'),
+000189d0: 0a20 2020 2020 2020 2020 2020 2028 4c49  .            (LI
+000189e0: 2827 5c74 7365 636f 6e64 206c 696e 6527  ('\tsecond line'
+000189f0: 2c20 322c 2039 2c20 6c65 6164 696e 673d  , 2, 9, leading=
+00018a00: 275c 7427 292c 2027 7365 636f 6e64 206c  '\t'), 'second l
+00018a10: 696e 6527 292c 0a20 2020 2020 2020 2020  ine'),.         
+00018a20: 2020 2028 4c49 2827 7468 6972 6420 6c69     (LI('third li
+00018a30: 6e65 272c 2033 2c20 3129 2c20 2774 6869  ne', 3, 1), 'thi
+00018a40: 7264 206c 696e 6527 292c 0a20 2020 2020  rd line'),.     
+00018a50: 2020 2020 2020 205d 290a 0a20 2020 2020         ])..     
+00018a60: 2020 2074 6573 7428 6269 672e 6c69 6e65     test(big.line
+00018a70: 735f 6669 6c74 6572 5f63 6f6d 6d65 6e74  s_filter_comment
+00018a80: 5f6c 696e 6573 2862 6967 2e6c 696e 6573  _lines(big.lines
+00018a90: 2822 2222 0a20 2020 2023 2063 6f6d 6d65  (""".    # comme
+00018aa0: 6e74 0a20 2020 2061 203d 2062 0a20 2020  nt.    a = b.   
+00018ab0: 202f 2f20 616e 6f74 6865 7220 636f 6d6d   // another comm
+00018ac0: 656e 740a 2020 2020 6320 3d20 640a 2020  ent.    c = d.  
+00018ad0: 2020 2f20 6e6f 7420 6120 636f 6d6d 656e    / not a commen
+00018ae0: 740a 2020 2020 2f2f 2f20 6973 2061 2063  t.    /// is a c
+00018af0: 6f6d 6d65 6e74 210a 2020 2020 2323 2061  omment!.    ## a
+00018b00: 6e6f 7468 6572 2063 6f6d 6d65 6e74 210a  nother comment!.
+00018b10: 2020 2020 2321 2061 2074 6869 7264 2063      #! a third c
+00018b20: 6f6d 6d65 6e74 210a 2222 222e 6c73 7472  omment!.""".lstr
+00018b30: 6970 2827 5c6e 2729 292c 2028 2723 272c  ip('\n')), ('#',
+00018b40: 2027 2f2f 2729 292c 0a20 2020 2020 2020   '//')),.       
+00018b50: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00018b60: 2020 2028 4c49 2827 2020 2020 6120 3d20     (LI('    a = 
+00018b70: 6227 2c20 2020 2020 2020 2020 2020 322c  b',           2,
+00018b80: 2031 292c 2027 2020 2020 6120 3d20 6227   1), '    a = b'
+00018b90: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00018ba0: 4c49 2827 2020 2020 6320 3d20 6427 2c20  LI('    c = d', 
+00018bb0: 2020 2020 2020 2020 2020 342c 2031 292c            4, 1),
+00018bc0: 2027 2020 2020 6320 3d20 6427 292c 0a20   '    c = d'),. 
+00018bd0: 2020 2020 2020 2020 2020 2028 4c49 2827             (LI('
+00018be0: 2020 2020 2f20 6e6f 7420 6120 636f 6d6d      / not a comm
+00018bf0: 656e 7427 2c20 352c 2031 292c 2027 2020  ent', 5, 1), '  
+00018c00: 2020 2f20 6e6f 7420 6120 636f 6d6d 656e    / not a commen
+00018c10: 7427 292c 0a20 2020 2020 2020 2020 2020  t'),.           
+00018c20: 2028 4c49 2827 272c 2020 2020 2020 2020   (LI('',        
+00018c30: 2020 2020 2020 2020 2020 2020 392c 2031              9, 1
+00018c40: 292c 2027 2729 2c0a 2020 2020 2020 2020  ), ''),.        
+00018c50: 2020 2020 5d29 0a0a 2020 2020 2020 2020      ])..        
+00018c60: 7465 7374 2862 6967 2e6c 696e 6573 5f66  test(big.lines_f
+00018c70: 696c 7465 725f 636f 6d6d 656e 745f 6c69  ilter_comment_li
+00018c80: 6e65 7328 6269 672e 6c69 6e65 7328 6222  nes(big.lines(b"
+00018c90: 615c 6e23 2069 676e 6f72 6564 5c6e 2063  a\n# ignored\n c
+00018ca0: 2229 2c20 6227 2327 292c 0a20 2020 2020  "), b'#'),.     
+00018cb0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00018cc0: 2020 2020 204c 2862 2761 272c 2031 292c       L(b'a', 1),
+00018cd0: 0a20 2020 2020 2020 2020 2020 204c 2862  .            L(b
+00018ce0: 2720 6327 2c20 3329 2c0a 2020 2020 2020  ' c', 3),.      
+00018cf0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00018d00: 2020 2020 290a 0a20 2020 2020 2020 2074      )..        t
+00018d10: 6573 7428 6269 672e 6c69 6e65 735f 636f  est(big.lines_co
+00018d20: 6e74 6169 6e69 6e67 2862 6967 2e6c 696e  ntaining(big.lin
+00018d30: 6573 2822 2222 0a68 656c 6c6f 2079 6f6c  es(""".hello yol
+00018d40: 6b73 0a77 6861 7420 646f 2079 6f75 2068  ks.what do you h
+00018d50: 6176 6520 746f 2073 6179 2c20 6368 616d  ave to say, cham
+00018d60: 703f 0a69 206c 696b 6520 6567 6773 2e0a  p?.i like eggs..
+00018d70: 7468 6579 2064 6f6e 2774 2068 6176 6520  they don't have 
+00018d80: 746f 2062 6520 6661 6e63 792e 0a73 696d  to be fancy..sim
+00018d90: 706c 6520 7363 7261 6d62 6c65 6420 6567  ple scrambled eg
+00018da0: 6773 2061 7265 206a 7573 7420 6669 6e65  gs are just fine
+00018db0: 2e0a 6e65 6767 6174 6f72 7921 0a77 686f  ..neggatory!.who
+00018dc0: 6f70 732c 2049 206d 6561 6e74 2c20 6e65  ops, I meant, ne
+00018dd0: 6761 746f 7279 2e0a 2222 225b 313a 5d29  gatory.."""[1:])
+00018de0: 2c20 2265 6767 2229 2c0a 2020 2020 2020  , "egg"),.      
+00018df0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00018e00: 2020 2020 2020 2020 284c 4928 2769 206c          (LI('i l
+00018e10: 696b 6520 6567 6773 2e27 2c20 332c 2031  ike eggs.', 3, 1
+00018e20: 292c 2027 6920 6c69 6b65 2065 6767 732e  ), 'i like eggs.
+00018e30: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00018e40: 2020 2020 284c 4928 2773 696d 706c 6520      (LI('simple 
+00018e50: 7363 7261 6d62 6c65 6420 6567 6773 2061  scrambled eggs a
+00018e60: 7265 206a 7573 7420 6669 6e65 2e27 2c20  re just fine.', 
+00018e70: 352c 2031 292c 2027 7369 6d70 6c65 2073  5, 1), 'simple s
+00018e80: 6372 616d 626c 6564 2065 6767 7320 6172  crambled eggs ar
+00018e90: 6520 6a75 7374 2066 696e 652e 2729 2c0a  e just fine.'),.
+00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018eb0: 284c 4928 276e 6567 6761 746f 7279 2127  (LI('neggatory!'
+00018ec0: 2c20 362c 2031 292c 2027 6e65 6767 6174  , 6, 1), 'neggat
+00018ed0: 6f72 7921 2729 2c0a 2020 2020 2020 2020  ory!'),.        
+00018ee0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00018ef0: 2020 290a 0a20 2020 2020 2020 2074 6573    )..        tes
+00018f00: 7428 6269 672e 6c69 6e65 735f 636f 6e74  t(big.lines_cont
+00018f10: 6169 6e69 6e67 2862 6967 2e6c 696e 6573  aining(big.lines
+00018f20: 2822 2222 0a68 656c 6c6f 2079 6f6c 6b73  (""".hello yolks
+00018f30: 0a77 6861 7420 646f 2079 6f75 2068 6176  .what do you hav
+00018f40: 6520 746f 2073 6179 2c20 6368 616d 703f  e to say, champ?
+00018f50: 0a69 206c 696b 6520 6567 6773 2e0a 7468  .i like eggs..th
+00018f60: 6579 2064 6f6e 2774 2068 6176 6520 746f  ey don't have to
+00018f70: 2062 6520 6661 6e63 792e 0a73 696d 706c   be fancy..simpl
+00018f80: 6520 7363 7261 6d62 6c65 6420 6567 6773  e scrambled eggs
+00018f90: 2061 7265 206a 7573 7420 6669 6e65 2e0a   are just fine..
+00018fa0: 6e65 6767 6174 6f72 7921 0a77 686f 6f70  neggatory!.whoop
+00018fb0: 732c 2049 206d 6561 6e74 2c20 6e65 6761  s, I meant, nega
+00018fc0: 746f 7279 2e0a 2222 225b 313a 5d29 2c20  tory.."""[1:]), 
+00018fd0: 2265 6767 222c 2069 6e76 6572 743d 5472  "egg", invert=Tr
+00018fe0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+00018ff0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00019000: 2020 2028 4c49 2827 6865 6c6c 6f20 796f     (LI('hello yo
+00019010: 6c6b 7327 2c20 312c 2031 292c 2027 6865  lks', 1, 1), 'he
+00019020: 6c6c 6f20 796f 6c6b 7327 292c 0a20 2020  llo yolks'),.   
+00019030: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
+00019040: 2827 7768 6174 2064 6f20 796f 7520 6861  ('what do you ha
+00019050: 7665 2074 6f20 7361 792c 2063 6861 6d70  ve to say, champ
+00019060: 3f27 2c20 322c 2031 292c 2027 7768 6174  ?', 2, 1), 'what
+00019070: 2064 6f20 796f 7520 6861 7665 2074 6f20   do you have to 
+00019080: 7361 792c 2063 6861 6d70 3f27 292c 0a20  say, champ?'),. 
+00019090: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000190a0: 4c49 2822 7468 6579 2064 6f6e 2774 2068  LI("they don't h
+000190b0: 6176 6520 746f 2062 6520 6661 6e63 792e  ave to be fancy.
+000190c0: 222c 2034 2c20 3129 2c20 2274 6865 7920  ", 4, 1), "they 
+000190d0: 646f 6e27 7420 6861 7665 2074 6f20 6265  don't have to be
+000190e0: 2066 616e 6379 2e22 292c 0a20 2020 2020   fancy."),.     
+000190f0: 2020 2020 2020 2020 2020 2028 4c49 2827             (LI('
+00019100: 7768 6f6f 7073 2c20 4920 6d65 616e 742c  whoops, I meant,
+00019110: 206e 6567 6174 6f72 792e 272c 2037 2c20   negatory.', 7, 
+00019120: 3129 2c20 2777 686f 6f70 732c 2049 206d  1), 'whoops, I m
+00019130: 6561 6e74 2c20 6e65 6761 746f 7279 2e27  eant, negatory.'
+00019140: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00019150: 2020 2028 4c49 2827 272c 2038 2c20 3129     (LI('', 8, 1)
+00019160: 2c20 2727 292c 0a20 2020 2020 2020 2020  , ''),.         
+00019170: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00019180: 2029 0a0a 2020 2020 2020 2020 7465 7374   )..        test
+00019190: 2862 6967 2e6c 696e 6573 5f67 7265 7028  (big.lines_grep(
+000191a0: 6269 672e 6c69 6e65 7328 2222 220a 6865  big.lines(""".he
+000191b0: 6c6c 6f20 796f 6c6b 730a 7768 6174 2064  llo yolks.what d
+000191c0: 6f20 796f 7520 6861 7665 2074 6f20 7361  o you have to sa
+000191d0: 792c 2063 6861 6d70 3f0a 6920 6c69 6b65  y, champ?.i like
+000191e0: 2065 6767 732e 0a74 6865 7920 646f 6e27   eggs..they don'
+000191f0: 7420 6861 7665 2074 6f20 6265 2066 616e  t have to be fan
+00019200: 6379 2e0a 7369 6d70 6c65 2073 6372 616d  cy..simple scram
+00019210: 626c 6564 2065 6767 7320 6172 6520 6a75  bled eggs are ju
+00019220: 7374 2066 696e 652e 0a6e 6567 6761 746f  st fine..neggato
+00019230: 7279 210a 7768 6f6f 7073 2c20 4920 6d65  ry!.whoops, I me
+00019240: 616e 742c 206e 6567 6174 6f72 792e 0a22  ant, negatory.."
+00019250: 2222 5b31 3a5d 292c 2022 6567 2b22 292c  ""[1:]), "eg+"),
+00019260: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+00019270: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00019280: 4c49 2827 6920 6c69 6b65 2065 6767 732e  LI('i like eggs.
+00019290: 272c 2033 2c20 3129 2c20 2769 206c 696b  ', 3, 1), 'i lik
+000192a0: 6520 6567 6773 2e27 292c 0a20 2020 2020  e eggs.'),.     
+000192b0: 2020 2020 2020 2020 2020 2028 4c49 2827             (LI('
+000192c0: 7369 6d70 6c65 2073 6372 616d 626c 6564  simple scrambled
+000192d0: 2065 6767 7320 6172 6520 6a75 7374 2066   eggs are just f
+000192e0: 696e 652e 272c 2035 2c20 3129 2c20 2773  ine.', 5, 1), 's
+000192f0: 696d 706c 6520 7363 7261 6d62 6c65 6420  imple scrambled 
+00019300: 6567 6773 2061 7265 206a 7573 7420 6669  eggs are just fi
+00019310: 6e65 2e27 292c 0a20 2020 2020 2020 2020  ne.'),.         
+00019320: 2020 2020 2020 2028 4c49 2827 6e65 6767         (LI('negg
+00019330: 6174 6f72 7921 272c 2036 2c20 3129 2c20  atory!', 6, 1), 
+00019340: 276e 6567 6761 746f 7279 2127 292c 0a20  'neggatory!'),. 
+00019350: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00019360: 4c49 2827 7768 6f6f 7073 2c20 4920 6d65  LI('whoops, I me
+00019370: 616e 742c 206e 6567 6174 6f72 792e 272c  ant, negatory.',
+00019380: 2037 2c20 3129 2c20 2777 686f 6f70 732c   7, 1), 'whoops,
+00019390: 2049 206d 6561 6e74 2c20 6e65 6761 746f   I meant, negato
+000193a0: 7279 2e27 292c 0a20 2020 2020 2020 2020  ry.'),.         
+000193b0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+000193c0: 2029 0a0a 2020 2020 2020 2020 7465 7374   )..        test
+000193d0: 2862 6967 2e6c 696e 6573 5f67 7265 7028  (big.lines_grep(
+000193e0: 6269 672e 6c69 6e65 7328 2222 220a 6865  big.lines(""".he
+000193f0: 6c6c 6f20 796f 6c6b 730a 7768 6174 2064  llo yolks.what d
+00019400: 6f20 796f 7520 6861 7665 2074 6f20 7361  o you have to sa
+00019410: 792c 2063 6861 6d70 3f0a 6920 6c69 6b65  y, champ?.i like
+00019420: 2065 6767 732e 0a74 6865 7920 646f 6e27   eggs..they don'
+00019430: 7420 6861 7665 2074 6f20 6265 2066 616e  t have to be fan
+00019440: 6379 2e0a 7369 6d70 6c65 2073 6372 616d  cy..simple scram
+00019450: 626c 6564 2065 6767 7320 6172 6520 6a75  bled eggs are ju
+00019460: 7374 2066 696e 652e 0a6e 6567 6761 746f  st fine..neggato
+00019470: 7279 210a 7768 6f6f 7073 2c20 4920 6d65  ry!.whoops, I me
+00019480: 616e 742c 206e 6567 6174 6f72 792e 0a22  ant, negatory.."
+00019490: 2222 5b31 3a5d 292c 2022 6567 2b22 2c20  ""[1:]), "eg+", 
+000194a0: 696e 7665 7274 3d54 7275 6529 2c0a 2020  invert=True),.  
+000194b0: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+000194c0: 2020 2020 2020 2020 2020 2020 284c 4928              (LI(
+000194d0: 2768 656c 6c6f 2079 6f6c 6b73 272c 2031  'hello yolks', 1
+000194e0: 2c20 3129 2c20 2768 656c 6c6f 2079 6f6c  , 1), 'hello yol
+000194f0: 6b73 2729 2c0a 2020 2020 2020 2020 2020  ks'),.          
+00019500: 2020 2020 2020 284c 4928 2777 6861 7420        (LI('what 
+00019510: 646f 2079 6f75 2068 6176 6520 746f 2073  do you have to s
+00019520: 6179 2c20 6368 616d 703f 272c 2032 2c20  ay, champ?', 2, 
+00019530: 3129 2c20 2777 6861 7420 646f 2079 6f75  1), 'what do you
+00019540: 2068 6176 6520 746f 2073 6179 2c20 6368   have to say, ch
+00019550: 616d 703f 2729 2c0a 2020 2020 2020 2020  amp?'),.        
+00019560: 2020 2020 2020 2020 284c 4928 2274 6865          (LI("the
+00019570: 7920 646f 6e27 7420 6861 7665 2074 6f20  y don't have to 
+00019580: 6265 2066 616e 6379 2e22 2c20 342c 2031  be fancy.", 4, 1
+00019590: 292c 2022 7468 6579 2064 6f6e 2774 2068  ), "they don't h
+000195a0: 6176 6520 746f 2062 6520 6661 6e63 792e  ave to be fancy.
+000195b0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000195c0: 2020 2020 284c 4928 2727 2c20 382c 2031      (LI('', 8, 1
+000195d0: 292c 2027 2729 2c0a 2020 2020 2020 2020  ), ''),.        
+000195e0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000195f0: 2020 290a 0a20 2020 2020 2020 2074 6573    )..        tes
+00019600: 7428 6269 672e 6c69 6e65 735f 736f 7274  t(big.lines_sort
+00019610: 2862 6967 2e6c 696e 6573 2822 2222 0a63  (big.lines(""".c
+00019620: 6f72 6d6f 7261 6e74 0a66 6972 6566 6f78  ormorant.firefox
+00019630: 0a61 6c6c 6967 6174 6f72 0a64 6970 6c6f  .alligator.diplo
+00019640: 646f 6375 730a 656c 6570 6861 6e74 0a67  docus.elephant.g
+00019650: 6972 6166 6665 0a62 6172 7261 6375 6461  iraffe.barracuda
+00019660: 0a68 756d 6d69 6e67 6269 7264 0a22 2222  .hummingbird."""
+00019670: 5b31 3a2d 315d 2929 2c0a 2020 2020 2020  [1:-1])),.      
+00019680: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00019690: 2020 2020 2020 2020 4c28 2761 6c6c 6967          L('allig
+000196a0: 6174 6f72 272c 2033 292c 0a20 2020 2020  ator', 3),.     
+000196b0: 2020 2020 2020 2020 2020 204c 2827 6261             L('ba
+000196c0: 7272 6163 7564 6127 2c20 3729 2c0a 2020  rracuda', 7),.  
+000196d0: 2020 2020 2020 2020 2020 2020 2020 4c28                L(
+000196e0: 2763 6f72 6d6f 7261 6e74 272c 2031 292c  'cormorant', 1),
+000196f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019700: 204c 2827 6469 706c 6f64 6f63 7573 272c   L('diplodocus',
+00019710: 2034 292c 0a20 2020 2020 2020 2020 2020   4),.           
+00019720: 2020 2020 204c 2827 656c 6570 6861 6e74       L('elephant
+00019730: 272c 2035 292c 0a20 2020 2020 2020 2020  ', 5),.         
+00019740: 2020 2020 2020 204c 2827 6669 7265 666f         L('firefo
+00019750: 7827 2c20 3229 2c0a 2020 2020 2020 2020  x', 2),.        
+00019760: 2020 2020 2020 2020 4c28 2767 6972 6166          L('giraf
+00019770: 6665 272c 2036 292c 0a20 2020 2020 2020  fe', 6),.       
+00019780: 2020 2020 2020 2020 204c 2827 6875 6d6d           L('humm
+00019790: 696e 6762 6972 6427 2c20 3829 2c0a 2020  ingbird', 8),.  
+000197a0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+000197b0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000197c0: 2020 2074 6573 7428 6269 672e 6c69 6e65     test(big.line
+000197d0: 735f 736f 7274 2862 6967 2e6c 696e 6573  s_sort(big.lines
+000197e0: 2822 2222 0a63 6f72 6d6f 7261 6e74 0a66  (""".cormorant.f
+000197f0: 6972 6566 6f78 0a61 6c6c 6967 6174 6f72  irefox.alligator
+00019800: 0a64 6970 6c6f 646f 6375 730a 656c 6570  .diplodocus.elep
+00019810: 6861 6e74 0a67 6972 6166 6665 0a62 6172  hant.giraffe.bar
+00019820: 7261 6375 6461 0a68 756d 6d69 6e67 6269  racuda.hummingbi
+00019830: 7264 0a22 2222 5b31 3a2d 315d 292c 2072  rd."""[1:-1]), r
+00019840: 6576 6572 7365 3d54 7275 6529 2c0a 2020  everse=True),.  
+00019850: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00019860: 2020 2020 2020 2020 2020 2020 4c28 2768              L('h
+00019870: 756d 6d69 6e67 6269 7264 272c 2038 292c  ummingbird', 8),
+00019880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019890: 204c 2827 6769 7261 6666 6527 2c20 3629   L('giraffe', 6)
+000198a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000198b0: 2020 4c28 2766 6972 6566 6f78 272c 2032    L('firefox', 2
+000198c0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000198d0: 2020 204c 2827 656c 6570 6861 6e74 272c     L('elephant',
+000198e0: 2035 292c 0a20 2020 2020 2020 2020 2020   5),.           
+000198f0: 2020 2020 204c 2827 6469 706c 6f64 6f63       L('diplodoc
+00019900: 7573 272c 2034 292c 0a20 2020 2020 2020  us', 4),.       
+00019910: 2020 2020 2020 2020 204c 2827 636f 726d           L('corm
+00019920: 6f72 616e 7427 2c20 3129 2c0a 2020 2020  orant', 1),.    
+00019930: 2020 2020 2020 2020 2020 2020 4c28 2762              L('b
+00019940: 6172 7261 6375 6461 272c 2037 292c 0a20  arracuda', 7),. 
+00019950: 2020 2020 2020 2020 2020 2020 2020 204c                 L
+00019960: 2827 616c 6c69 6761 746f 7227 2c20 3329  ('alligator', 3)
+00019970: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
+00019980: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00019990: 2020 2020 2020 2074 6573 7428 6269 672e         test(big.
+000199a0: 6c69 6e65 735f 7273 7472 6970 2862 6967  lines_rstrip(big
+000199b0: 2e6c 696e 6573 280a 2220 2020 2061 203d  .lines(."    a =
+000199c0: 2062 2020 5c6e 220a 2220 2020 2063 203d   b  \n"."    c =
+000199d0: 2064 2020 2020 205c 6e22 0a29 292c 0a20   d     \n".)),. 
+000199e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+000199f0: 2020 2020 2020 2020 2028 4c49 2827 2020           (LI('  
+00019a00: 2020 6120 3d20 6220 2027 2c20 2020 2031    a = b  ',    1
+00019a10: 2c20 3129 2c20 2720 2020 2061 203d 2062  , 1), '    a = b
+00019a20: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00019a30: 284c 4928 2720 2020 2063 203d 2064 2020  (LI('    c = d  
+00019a40: 2020 2027 2c20 322c 2031 292c 2027 2020     ', 2, 1), '  
+00019a50: 2020 6320 3d20 6427 292c 0a20 2020 2020    c = d'),.     
+00019a60: 2020 2020 2020 2028 4c49 2827 272c 2020         (LI('',  
+00019a70: 2020 2020 2020 2020 2020 2020 2033 2c20               3, 
+00019a80: 3129 2c20 2727 292c 0a20 2020 2020 2020  1), ''),.       
+00019a90: 2020 2020 205d 290a 0a20 2020 2020 2020       ])..       
+00019aa0: 2074 6573 7428 6269 672e 6c69 6e65 735f   test(big.lines_
+00019ab0: 7374 7269 7028 6269 672e 6c69 6e65 7328  strip(big.lines(
+00019ac0: 0a22 2020 2020 6120 3d20 6220 205c 6e22  ."    a = b  \n"
+00019ad0: 0a22 2020 2020 6320 3d20 6420 2020 2020  ."    c = d     
+00019ae0: 5c6e 220a 2929 2c0a 2020 2020 2020 2020  \n".)),.        
+00019af0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00019b00: 2020 284c 4928 2720 2020 2061 203d 2062    (LI('    a = b
+00019b10: 2020 272c 2020 2020 312c 2035 2c20 6c65    ',    1, 5, le
+00019b20: 6164 696e 673d 2720 2020 2027 292c 2027  ading='    '), '
+00019b30: 6120 3d20 6227 292c 0a20 2020 2020 2020  a = b'),.       
+00019b40: 2020 2020 2028 4c49 2827 2020 2020 6320       (LI('    c 
+00019b50: 3d20 6420 2020 2020 272c 2032 2c20 352c  = d     ', 2, 5,
+00019b60: 206c 6561 6469 6e67 3d27 2020 2020 2729   leading='    ')
+00019b70: 2c20 2763 203d 2064 2729 2c0a 2020 2020  , 'c = d'),.    
+00019b80: 2020 2020 2020 2020 284c 4928 2727 2c20          (LI('', 
+00019b90: 2020 2020 2020 2020 2020 2020 2020 332c                3,
+00019ba0: 2031 292c 2027 2729 2c0a 2020 2020 2020   1), ''),.      
+00019bb0: 2020 2020 2020 5d29 0a0a 2020 2020 2020        ])..      
+00019bc0: 2020 7465 7374 2862 6967 2e6c 696e 6573    test(big.lines
+00019bd0: 5f66 696c 7465 725f 656d 7074 795f 6c69  _filter_empty_li
+00019be0: 6e65 7328 6269 672e 6c69 6e65 7328 2222  nes(big.lines(""
+00019bf0: 220a 0a20 2020 2061 203d 2062 0a0a 0a20  "..    a = b... 
+00019c00: 2020 2063 203d 2064 0a0a 2222 225b 313a     c = d.."""[1:
+00019c10: 5d29 292c 0a20 2020 2020 2020 2020 2020  ])),.           
+00019c20: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
+00019c30: 4c49 2827 2020 2020 6120 3d20 6227 2c20  LI('    a = b', 
+00019c40: 322c 2031 292c 2027 2020 2020 6120 3d20  2, 1), '    a = 
+00019c50: 6227 292c 0a20 2020 2020 2020 2020 2020  b'),.           
+00019c60: 2028 4c49 2827 2020 2020 6320 3d20 6427   (LI('    c = d'
+00019c70: 2c20 352c 2031 292c 2027 2020 2020 6320  , 5, 1), '    c 
+00019c80: 3d20 6427 292c 0a20 2020 2020 2020 2020  = d'),.         
+00019c90: 2020 205d 290a 0a20 2020 2020 2020 2074     ])..        t
+00019ca0: 6573 7428 6269 672e 6c69 6e65 735f 636f  est(big.lines_co
+00019cb0: 6e76 6572 745f 7461 6273 5f74 6f5f 7370  nvert_tabs_to_sp
+00019cc0: 6163 6573 2862 6967 2e6c 696e 6573 280a  aces(big.lines(.
+00019cd0: 2020 2020 2020 2020 2020 2020 225c 7466              "\tf
+00019ce0: 6972 7374 206c 696e 655c 6e22 0a20 2020  irst line\n".   
+00019cf0: 2020 2020 2020 2020 2022 5c74 5c74 7365           "\t\tse
+00019d00: 636f 6e64 206c 696e 655c 6e22 0a20 2020  cond line\n".   
+00019d10: 2020 2020 2020 2020 2022 2020 5c74 7468           "  \tth
+00019d20: 6972 6420 6c69 6e65 5c6e 222c 0a20 2020  ird line\n",.   
+00019d30: 2020 2020 2020 2020 2074 6162 5f77 6964           tab_wid
+00019d40: 7468 3d38 2929 2c0a 2020 2020 2020 2020  th=8)),.        
+00019d50: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00019d60: 2020 2020 2020 284c 4928 225c 7466 6972        (LI("\tfir
+00019d70: 7374 206c 696e 6522 2c20 312c 2031 292c  st line", 1, 1),
+00019d80: 2022 2020 2020 2020 2020 6669 7273 7420   "        first 
+00019d90: 6c69 6e65 2229 2c0a 2020 2020 2020 2020  line"),.        
+00019da0: 2020 2020 2020 2020 284c 4928 225c 745c          (LI("\t\
+00019db0: 7473 6563 6f6e 6420 6c69 6e65 222c 2032  tsecond line", 2
+00019dc0: 2c20 3129 2c20 2220 2020 2020 2020 2020  , 1), "         
+00019dd0: 2020 2020 2020 2073 6563 6f6e 6420 6c69         second li
+00019de0: 6e65 2229 2c0a 2020 2020 2020 2020 2020  ne"),.          
+00019df0: 2020 2020 2020 284c 4928 2220 205c 7474        (LI("  \tt
+00019e00: 6869 7264 206c 696e 6522 2c20 332c 2031  hird line", 3, 1
+00019e10: 292c 2022 2020 2020 2020 2020 7468 6972  ), "        thir
+00019e20: 6420 6c69 6e65 2229 2c0a 2020 2020 2020  d line"),.      
+00019e30: 2020 2020 2020 2020 2020 284c 4928 2222            (LI(""
+00019e40: 2c20 342c 2031 292c 2022 2229 2c0a 2020  , 4, 1), ""),.  
+00019e50: 2020 2020 2020 2020 2020 5d29 0a0a 2020            ])..  
+00019e60: 2020 2020 2020 7465 7374 2862 6967 2e6c        test(big.l
+00019e70: 696e 6573 5f73 7472 6970 5f63 6f6d 6d65  ines_strip_comme
+00019e80: 6e74 7328 6269 672e 6c69 6e65 7328 2222  nts(big.lines(""
+00019e90: 220a 666f 7220 7820 696e 2072 616e 6765  ".for x in range
+00019ea0: 2835 293a 2023 2074 6869 7320 6973 2061  (5): # this is a
+00019eb0: 2063 6f6d 6d65 6e74 0a20 2020 2070 7269   comment.    pri
+00019ec0: 6e74 2822 2320 7468 6973 2069 7320 7175  nt("# this is qu
+00019ed0: 6f74 6564 222c 2078 290a 2020 2020 7072  oted", x).    pr
+00019ee0: 696e 7428 2222 2920 2320 7468 6973 2022  int("") # this "
+00019ef0: 636f 6d6d 656e 7422 2069 7320 7573 656c  comment" is usel
+00019f00: 6573 730a 2020 2020 7072 696e 7428 6e6f  ess.    print(no
+00019f10: 5f63 6f6d 6d65 6e74 735f 6f72 5f71 756f  _comments_or_quo
+00019f20: 7465 735f 6f6e 5f74 6869 735f 6c69 6e65  tes_on_this_line
+00019f30: 290a 2222 225b 313a 5d29 2c20 2822 2322  )."""[1:]), ("#"
+00019f40: 2c20 222f 2f22 2929 2c0a 2020 2020 2020  , "//")),.      
+00019f50: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00019f60: 2020 2020 2020 2020 284c 4928 6c69 6e65          (LI(line
+00019f70: 3d27 666f 7220 7820 696e 2072 616e 6765  ='for x in range
+00019f80: 2835 293a 2023 2074 6869 7320 6973 2061  (5): # this is a
+00019f90: 2063 6f6d 6d65 6e74 272c 206c 696e 655f   comment', line_
+00019fa0: 6e75 6d62 6572 3d31 2c20 636f 6c75 6d6e  number=1, column
+00019fb0: 5f6e 756d 6265 723d 312c 2063 6f6d 6d65  _number=1, comme
+00019fc0: 6e74 3d27 2320 7468 6973 2069 7320 6120  nt='# this is a 
+00019fd0: 636f 6d6d 656e 7427 292c 0a20 2020 2020  comment'),.     
+00019fe0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00019ff0: 666f 7220 7820 696e 2072 616e 6765 2835  for x in range(5
+0001a000: 293a 2729 2c0a 2020 2020 2020 2020 2020  ):'),.          
+0001a010: 2020 2020 2020 284c 4928 6c69 6e65 3d27        (LI(line='
+0001a020: 2020 2020 7072 696e 7428 2223 2074 6869      print("# thi
+0001a030: 7320 6973 2071 756f 7465 6422 2c20 7829  s is quoted", x)
+0001a040: 272c 206c 696e 655f 6e75 6d62 6572 3d32  ', line_number=2
+0001a050: 2c20 636f 6c75 6d6e 5f6e 756d 6265 723d  , column_number=
+0001a060: 312c 2063 6f6d 6d65 6e74 3d27 2729 2c0a  1, comment=''),.
 0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a080: 276f 7468 6572 2074 6578 7427 292c 0a20  'other text'),. 
-0001a090: 2020 2020 2020 2020 2020 2028 4c69 6e65             (Line
-0001a0a0: 496e 666f 286c 696e 653d 2720 2020 2020  Info(line='     
-0001a0b0: 2020 2020 206f 7468 6572 2074 6578 7427       other text'
-0001a0c0: 2c20 6c69 6e65 5f6e 756d 6265 723d 382c  , line_number=8,
-0001a0d0: 2063 6f6c 756d 6e5f 6e75 6d62 6572 3d31   column_number=1
-0001a0e0: 312c 2069 6e64 656e 743d 322c 206c 6561  1, indent=2, lea
-0001a0f0: 6469 6e67 3d27 2020 2020 2020 2020 2020  ding='          
-0001a100: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0001a110: 2020 2020 276f 7468 6572 2074 6578 7427      'other text'
-0001a120: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001a130: 4c69 6e65 496e 666f 286c 696e 653d 2720  LineInfo(line=' 
-0001a140: 2020 206d 6f72 6520 7465 7874 272c 206c     more text', l
-0001a150: 696e 655f 6e75 6d62 6572 3d39 2c20 636f  ine_number=9, co
-0001a160: 6c75 6d6e 5f6e 756d 6265 723d 352c 2069  lumn_number=5, i
-0001a170: 6e64 656e 743d 312c 206c 6561 6469 6e67  ndent=1, leading
-0001a180: 3d27 2020 2020 2729 2c0a 2020 2020 2020  ='    '),.      
-0001a190: 2020 2020 2020 2020 2020 276d 6f72 6520            'more 
-0001a1a0: 7465 7874 2729 2c0a 2020 2020 2020 2020  text'),.        
-0001a1b0: 2020 2020 284c 696e 6549 6e66 6f28 6c69      (LineInfo(li
-0001a1c0: 6e65 3d27 2020 2020 2020 6469 6666 6572  ne='      differ
-0001a1d0: 656e 7420 696e 6465 6e74 272c 206c 696e  ent indent', lin
-0001a1e0: 655f 6e75 6d62 6572 3d31 302c 2063 6f6c  e_number=10, col
-0001a1f0: 756d 6e5f 6e75 6d62 6572 3d37 2c20 696e  umn_number=7, in
-0001a200: 6465 6e74 3d32 2c20 6c65 6164 696e 673d  dent=2, leading=
-0001a210: 2720 2020 2020 2027 292c 0a20 2020 2020  '      '),.     
-0001a220: 2020 2020 2020 2020 2020 2027 6469 6666             'diff
-0001a230: 6572 656e 7420 696e 6465 6e74 2729 2c0a  erent indent'),.
-0001a240: 2020 2020 2020 2020 2020 2020 284c 696e              (Lin
-0001a250: 6549 6e66 6f28 6c69 6e65 3d27 2020 2020  eInfo(line='    
-0001a260: 6f75 7464 656e 7427 2c20 6c69 6e65 5f6e  outdent', line_n
-0001a270: 756d 6265 723d 3131 2c20 636f 6c75 6d6e  umber=11, column
-0001a280: 5f6e 756d 6265 723d 352c 2069 6e64 656e  _number=5, inden
-0001a290: 743d 312c 206c 6561 6469 6e67 3d27 2020  t=1, leading='  
-0001a2a0: 2020 2729 2c0a 2020 2020 2020 2020 2020    '),.          
-0001a2b0: 2020 2020 2020 276f 7574 6465 6e74 2729        'outdent')
-0001a2c0: 2c0a 2020 2020 2020 2020 2020 2020 284c  ,.            (L
-0001a2d0: 696e 6549 6e66 6f28 6c69 6e65 3d27 6f75  ineInfo(line='ou
-0001a2e0: 7464 656e 7427 2c20 6c69 6e65 5f6e 756d  tdent', line_num
-0001a2f0: 6265 723d 3132 2c20 636f 6c75 6d6e 5f6e  ber=12, column_n
-0001a300: 756d 6265 723d 312c 2069 6e64 656e 743d  umber=1, indent=
-0001a310: 302c 206c 6561 6469 6e67 3d27 2729 2c0a  0, leading=''),.
-0001a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a330: 276f 7574 6465 6e74 2729 2c0a 2020 2020  'outdent'),.    
-0001a340: 2020 2020 2020 2020 284c 696e 6549 6e66          (LineInf
-0001a350: 6f28 6c69 6e65 3d27 2020 6e65 7720 696e  o(line='  new in
-0001a360: 6465 6e74 272c 206c 696e 655f 6e75 6d62  dent', line_numb
-0001a370: 6572 3d31 332c 2063 6f6c 756d 6e5f 6e75  er=13, column_nu
-0001a380: 6d62 6572 3d33 2c20 696e 6465 6e74 3d31  mber=3, indent=1
-0001a390: 2c20 6c65 6164 696e 673d 2720 2027 292c  , leading='  '),
-0001a3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a3b0: 2027 6e65 7720 696e 6465 6e74 2729 2c0a   'new indent'),.
-0001a3c0: 2020 2020 2020 2020 2020 2020 284c 696e              (Lin
-0001a3d0: 6549 6e66 6f28 6c69 6e65 3d27 6f75 7464  eInfo(line='outd
-0001a3e0: 656e 7427 2c20 6c69 6e65 5f6e 756d 6265  ent', line_numbe
-0001a3f0: 723d 3134 2c20 636f 6c75 6d6e 5f6e 756d  r=14, column_num
-0001a400: 6265 723d 312c 2069 6e64 656e 743d 302c  ber=1, indent=0,
-0001a410: 206c 6561 6469 6e67 3d27 2729 2c0a 2020   leading=''),.  
-0001a420: 2020 2020 2020 2020 2020 2020 2020 276f                'o
-0001a430: 7574 6465 6e74 2729 2c0a 2020 2020 2020  utdent'),.      
-0001a440: 2020 2020 2020 284c 696e 6549 6e66 6f28        (LineInfo(
-0001a450: 6c69 6e65 3d27 272c 206c 696e 655f 6e75  line='', line_nu
-0001a460: 6d62 6572 3d31 352c 2063 6f6c 756d 6e5f  mber=15, column_
-0001a470: 6e75 6d62 6572 3d31 2c20 696e 6465 6e74  number=1, indent
-0001a480: 3d30 2c20 6c65 6164 696e 673d 2727 292c  =0, leading=''),
-0001a490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a4a0: 2027 2729 2c0a 2020 2020 2020 2020 2020   ''),.          
-0001a4b0: 2020 5d0a 0a20 2020 2020 2020 2074 6573    ]..        tes
-0001a4c0: 7428 6c69 6e65 732c 2065 7870 6563 7465  t(lines, expecte
-0001a4d0: 6429 0a0a 0a20 2020 2020 2020 2023 230a  d)...        ##.
-0001a4e0: 2020 2020 2020 2020 2323 2074 6573 7420          ## test 
-0001a4f0: 7461 6220 746f 2073 7061 6365 730a 2020  tab to spaces.  
-0001a500: 2020 2020 2020 2323 0a0a 2020 2020 2020        ##..      
-0001a510: 2020 6c69 6e65 7320 3d20 280a 2020 2020    lines = (.    
-0001a520: 2020 2020 226c 6566 7420 6d61 7267 696e      "left margin
-0001a530: 5c6e 220a 2020 2020 2020 2020 225c 7465  \n".        "\te
-0001a540: 6967 6874 5c6e 220a 2020 2020 2020 2020  ight\n".        
-0001a550: 2220 205c 7420 2020 2074 7765 6c76 655c  "  \t    twelve\
-0001a560: 6e22 0a20 2020 2020 2020 2022 2020 2020  n".        "    
-0001a570: 2020 2020 6569 6768 7420 6973 2065 6e6f      eight is eno
-0001a580: 7567 685c 6e22 0a20 2020 2020 2020 2029  ugh\n".        )
-0001a590: 0a0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
-0001a5a0: 6564 203d 205b 0a20 2020 2020 2020 2020  ed = [.         
-0001a5b0: 2020 2028 4c69 6e65 496e 666f 286c 696e     (LineInfo(lin
-0001a5c0: 653d 276c 6566 7420 6d61 7267 696e 272c  e='left margin',
-0001a5d0: 206c 696e 655f 6e75 6d62 6572 3d31 2c20   line_number=1, 
-0001a5e0: 636f 6c75 6d6e 5f6e 756d 6265 723d 312c  column_number=1,
-0001a5f0: 2069 6e64 656e 743d 302c 206c 6561 6469   indent=0, leadi
-0001a600: 6e67 3d27 2729 2c0a 2020 2020 2020 2020  ng=''),.        
-0001a610: 2020 2020 2020 2020 276c 6566 7420 6d61          'left ma
-0001a620: 7267 696e 2729 2c0a 2020 2020 2020 2020  rgin'),.        
-0001a630: 2020 2020 284c 696e 6549 6e66 6f28 6c69      (LineInfo(li
-0001a640: 6e65 3d27 5c74 6569 6768 7427 2c20 6c69  ne='\teight', li
-0001a650: 6e65 5f6e 756d 6265 723d 322c 2063 6f6c  ne_number=2, col
-0001a660: 756d 6e5f 6e75 6d62 6572 3d39 2c20 696e  umn_number=9, in
-0001a670: 6465 6e74 3d31 2c20 6c65 6164 696e 673d  dent=1, leading=
-0001a680: 275c 7427 292c 0a20 2020 2020 2020 2020  '\t'),.         
-0001a690: 2020 2020 2020 2027 6569 6768 7427 292c         'eight'),
-0001a6a0: 0a20 2020 2020 2020 2020 2020 2028 4c69  .            (Li
-0001a6b0: 6e65 496e 666f 286c 696e 653d 2720 205c  neInfo(line='  \
-0001a6c0: 7420 2020 2074 7765 6c76 6527 2c20 6c69  t    twelve', li
-0001a6d0: 6e65 5f6e 756d 6265 723d 332c 2063 6f6c  ne_number=3, col
-0001a6e0: 756d 6e5f 6e75 6d62 6572 3d31 332c 2069  umn_number=13, i
-0001a6f0: 6e64 656e 743d 322c 206c 6561 6469 6e67  ndent=2, leading
-0001a700: 3d27 2020 5c74 2020 2020 2729 2c0a 2020  ='  \t    '),.  
-0001a710: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0001a720: 7765 6c76 6527 292c 0a20 2020 2020 2020  welve'),.       
-0001a730: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
-0001a740: 696e 653d 2720 2020 2020 2020 2065 6967  ine='        eig
-0001a750: 6874 2069 7320 656e 6f75 6768 272c 206c  ht is enough', l
-0001a760: 696e 655f 6e75 6d62 6572 3d34 2c20 636f  ine_number=4, co
-0001a770: 6c75 6d6e 5f6e 756d 6265 723d 392c 2069  lumn_number=9, i
-0001a780: 6e64 656e 743d 312c 206c 6561 6469 6e67  ndent=1, leading
-0001a790: 3d27 2020 2020 2020 2020 2729 2c0a 2020  ='        '),.  
-0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2765                'e
-0001a7b0: 6967 6874 2069 7320 656e 6f75 6768 2729  ight is enough')
-0001a7c0: 2c0a 2020 2020 2020 2020 2020 2020 284c  ,.            (L
-0001a7d0: 696e 6549 6e66 6f28 6c69 6e65 3d27 272c  ineInfo(line='',
-0001a7e0: 206c 696e 655f 6e75 6d62 6572 3d35 2c20   line_number=5, 
-0001a7f0: 636f 6c75 6d6e 5f6e 756d 6265 723d 312c  column_number=1,
-0001a800: 2069 6e64 656e 743d 302c 206c 6561 6469   indent=0, leadi
-0001a810: 6e67 3d27 2729 2c0a 2020 2020 2020 2020  ng=''),.        
-0001a820: 2020 2020 2020 2020 2727 290a 2020 2020          '').    
-0001a830: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
-0001a840: 2020 2074 6573 7428 6c69 6e65 732c 2065     test(lines, e
-0001a850: 7870 6563 7465 6429 0a0a 2020 2020 2020  xpected)..      
-0001a860: 2020 6c69 6e65 7320 3d20 280a 2020 2020    lines = (.    
-0001a870: 2020 2020 2020 2020 226c 6566 7420 6d61          "left ma
-0001a880: 7267 696e 5c6e 220a 2020 2020 2020 2020  rgin\n".        
-0001a890: 2020 2020 225c 7466 6f75 725c 6e22 0a20      "\tfour\n". 
-0001a8a0: 2020 2020 2020 2020 2020 2022 2020 5c74             "  \t
-0001a8b0: 2020 2020 6569 6768 745c 6e22 0a20 2020      eight\n".   
-0001a8c0: 2020 2020 2020 2020 2022 2020 5c74 5c74           "  \t\t
-0001a8d0: 6669 6775 7265 2065 6967 6874 2069 7320  figure eight is 
-0001a8e0: 646f 7562 6c65 2066 6f75 725c 6e22 0a20  double four\n". 
-0001a8f0: 2020 2020 2020 2020 2020 2022 2020 2020             "    
-0001a900: 6669 6775 7265 2066 6f75 7220 6973 2068  figure four is h
-0001a910: 616c 6620 6f66 2065 6967 6874 5c6e 220a  alf of eight\n".
-0001a920: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0001a930: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
-0001a940: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0001a950: 284c 696e 6549 6e66 6f28 6c69 6e65 3d27  (LineInfo(line='
-0001a960: 6c65 6674 206d 6172 6769 6e27 2c20 6c69  left margin', li
-0001a970: 6e65 5f6e 756d 6265 723d 312c 2063 6f6c  ne_number=1, col
-0001a980: 756d 6e5f 6e75 6d62 6572 3d31 2c20 696e  umn_number=1, in
-0001a990: 6465 6e74 3d30 2c20 6c65 6164 696e 673d  dent=0, leading=
-0001a9a0: 2727 292c 0a20 2020 2020 2020 2020 2020  ''),.           
-0001a9b0: 2020 2020 2027 6c65 6674 206d 6172 6769       'left margi
-0001a9c0: 6e27 292c 0a20 2020 2020 2020 2020 2020  n'),.           
-0001a9d0: 2028 4c69 6e65 496e 666f 286c 696e 653d   (LineInfo(line=
-0001a9e0: 275c 7466 6f75 7227 2c20 6c69 6e65 5f6e  '\tfour', line_n
-0001a9f0: 756d 6265 723d 322c 2063 6f6c 756d 6e5f  umber=2, column_
-0001aa00: 6e75 6d62 6572 3d35 2c20 696e 6465 6e74  number=5, indent
-0001aa10: 3d31 2c20 6c65 6164 696e 673d 275c 7427  =1, leading='\t'
-0001aa20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001aa30: 2020 2027 666f 7572 2729 2c0a 2020 2020     'four'),.    
-0001aa40: 2020 2020 2020 2020 284c 696e 6549 6e66          (LineInf
-0001aa50: 6f28 6c69 6e65 3d27 2020 5c74 2020 2020  o(line='  \t    
-0001aa60: 6569 6768 7427 2c20 6c69 6e65 5f6e 756d  eight', line_num
-0001aa70: 6265 723d 332c 2063 6f6c 756d 6e5f 6e75  ber=3, column_nu
-0001aa80: 6d62 6572 3d39 2c20 696e 6465 6e74 3d32  mber=9, indent=2
-0001aa90: 2c20 6c65 6164 696e 673d 2720 205c 7420  , leading='  \t 
-0001aaa0: 2020 2027 292c 0a20 2020 2020 2020 2020     '),.         
-0001aab0: 2020 2020 2020 2027 6569 6768 7427 292c         'eight'),
-0001aac0: 0a20 2020 2020 2020 2020 2020 2028 4c69  .            (Li
-0001aad0: 6e65 496e 666f 286c 696e 653d 2720 205c  neInfo(line='  \
-0001aae0: 745c 7466 6967 7572 6520 6569 6768 7420  t\tfigure eight 
-0001aaf0: 6973 2064 6f75 626c 6520 666f 7572 272c  is double four',
-0001ab00: 206c 696e 655f 6e75 6d62 6572 3d34 2c20   line_number=4, 
-0001ab10: 636f 6c75 6d6e 5f6e 756d 6265 723d 392c  column_number=9,
-0001ab20: 2069 6e64 656e 743d 322c 206c 6561 6469   indent=2, leadi
-0001ab30: 6e67 3d27 2020 5c74 5c74 2729 2c0a 2020  ng='  \t\t'),.  
-0001ab40: 2020 2020 2020 2020 2020 2020 2020 2766                'f
-0001ab50: 6967 7572 6520 6569 6768 7420 6973 2064  igure eight is d
-0001ab60: 6f75 626c 6520 666f 7572 2729 2c0a 2020  ouble four'),.  
-0001ab70: 2020 2020 2020 2020 2020 284c 696e 6549            (LineI
-0001ab80: 6e66 6f28 6c69 6e65 3d27 2020 2020 6669  nfo(line='    fi
-0001ab90: 6775 7265 2066 6f75 7220 6973 2068 616c  gure four is hal
-0001aba0: 6620 6f66 2065 6967 6874 272c 206c 696e  f of eight', lin
-0001abb0: 655f 6e75 6d62 6572 3d35 2c20 636f 6c75  e_number=5, colu
-0001abc0: 6d6e 5f6e 756d 6265 723d 352c 2069 6e64  mn_number=5, ind
-0001abd0: 656e 743d 312c 206c 6561 6469 6e67 3d27  ent=1, leading='
-0001abe0: 2020 2020 2729 2c0a 2020 2020 2020 2020      '),.        
-0001abf0: 2020 2020 2020 2020 2766 6967 7572 6520          'figure 
-0001ac00: 666f 7572 2069 7320 6861 6c66 206f 6620  four is half of 
-0001ac10: 6569 6768 7427 292c 0a20 2020 2020 2020  eight'),.       
-0001ac20: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
-0001ac30: 696e 653d 2727 2c20 6c69 6e65 5f6e 756d  ine='', line_num
-0001ac40: 6265 723d 362c 2063 6f6c 756d 6e5f 6e75  ber=6, column_nu
-0001ac50: 6d62 6572 3d31 2c20 696e 6465 6e74 3d30  mber=1, indent=0
-0001ac60: 2c20 6c65 6164 696e 673d 2727 292c 0a20  , leading=''),. 
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001ac80: 2729 5d0a 0a20 2020 2020 2020 2074 6573  ')]..        tes
-0001ac90: 7428 6c69 6e65 732c 2065 7870 6563 7465  t(lines, expecte
-0001aca0: 642c 2074 6162 5f77 6964 7468 3d34 290a  d, tab_width=4).
-0001acb0: 0a20 2020 2020 2020 2023 230a 2020 2020  .        ##.    
-0001acc0: 2020 2020 2323 2074 6573 7420 7261 6973      ## test rais
-0001acd0: 696e 6720 666f 7220 696c 6c65 6761 6c20  ing for illegal 
-0001ace0: 6f75 7464 656e 7473 0a20 2020 2020 2020  outdents.       
-0001acf0: 2023 230a 0a20 2020 2020 2020 2023 2077   ##..        # w
-0001ad00: 6865 6e20 6974 2773 2062 6574 7765 656e  hen it's between
-0001ad10: 2074 776f 2065 7869 7374 696e 6720 696e   two existing in
-0001ad20: 6465 6e74 730a 2020 2020 2020 2020 6c69  dents.        li
-0001ad30: 6e65 7320 3d20 280a 2020 2020 2020 2020  nes = (.        
-0001ad40: 2020 2020 226c 6566 7420 6d61 7267 696e      "left margin
-0001ad50: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-0001ad60: 225c 7466 6f75 725c 6e22 0a20 2020 2020  "\tfour\n".     
-0001ad70: 2020 2020 2020 2022 2020 5c74 2020 2020         "  \t    
-0001ad80: 6569 6768 745c 6e22 0a20 2020 2020 2020  eight\n".       
-0001ad90: 2020 2020 2022 2020 2020 2020 7369 783f       "      six?
-0001ada0: 215c 6e22 0a20 2020 2020 2020 2020 2020  !\n".           
-0001adb0: 2022 6c65 6674 206d 6172 6769 6e20 6167   "left margin ag
-0001adc0: 6169 6e5c 6e22 0a20 2020 2020 2020 2020  ain\n".         
-0001add0: 2020 2029 0a0a 2020 2020 2020 2020 7769     )..        wi
-0001ade0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-0001adf0: 6973 6573 2849 6e64 656e 7461 7469 6f6e  ises(Indentation
-0001ae00: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-0001ae10: 2020 2020 7465 7374 286c 696e 6573 2c20      test(lines, 
-0001ae20: 5b5d 2c20 7461 625f 7769 6474 683d 3429  [], tab_width=4)
-0001ae30: 0a0a 0a20 2020 2020 2020 2023 2077 6865  ...        # whe
-0001ae40: 6e20 6974 2773 206c 6573 7320 7468 616e  n it's less than
-0001ae50: 2074 6865 2066 6972 7374 2069 6e64 656e   the first inden
-0001ae60: 740a 2020 2020 2020 2020 6c69 6e65 7320  t.        lines 
-0001ae70: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001ae80: 226c 6566 7420 6d61 7267 696e 5c6e 220a  "left margin\n".
-0001ae90: 2020 2020 2020 2020 2020 2020 225c 7466              "\tf
-0001aea0: 6f75 725c 6e22 0a20 2020 2020 2020 2020  our\n".         
-0001aeb0: 2020 2022 2020 5c74 2020 2020 6569 6768     "  \t    eigh
-0001aec0: 745c 6e22 0a20 2020 2020 2020 2020 2020  t\n".           
-0001aed0: 2022 2020 7477 6f3f 215c 6e22 0a20 2020   "  two?!\n".   
-0001aee0: 2020 2020 2020 2020 2022 6c65 6674 206d           "left m
-0001aef0: 6172 6769 6e20 6167 6169 6e5c 6e22 0a20  argin again\n". 
-0001af00: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0001af10: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0001af20: 6173 7365 7274 5261 6973 6573 2849 6e64  assertRaises(Ind
-0001af30: 656e 7461 7469 6f6e 4572 726f 7229 3a0a  entationError):.
-0001af40: 2020 2020 2020 2020 2020 2020 7465 7374              test
-0001af50: 286c 696e 6573 2c20 5b5d 2c20 7461 625f  (lines, [], tab_
-0001af60: 7769 6474 683d 3429 0a0a 2020 2020 2020  width=4)..      
-0001af70: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-0001af80: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
-0001af90: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0001afa0: 2020 7465 7374 2822 6669 7273 7420 6c69    test("first li
-0001afb0: 6e65 5c6e 2020 5c75 3330 3030 2020 7365  ne\n  \u3000  se
-0001afc0: 636f 6e64 206c 696e 655c 6e74 6869 7264  cond line\nthird
-0001afd0: 206c 696e 655c 6e22 2c20 5b5d 290a 0a20   line\n", []).. 
-0001afe0: 2020 2064 6566 2074 6573 745f 6c69 6e65     def test_line
-0001aff0: 735f 6d69 7363 2873 656c 6629 3a0a 2020  s_misc(self):.  
-0001b000: 2020 2020 2020 2323 2072 6570 720a 2020        ## repr.  
-0001b010: 2020 2020 2020 6c69 203d 2062 6967 2e4c        li = big.L
-0001b020: 696e 6549 6e66 6f28 2727 2c20 312c 2031  ineInfo('', 1, 1
-0001b030: 2c20 696e 6465 6e74 3d30 290a 2020 2020  , indent=0).    
-0001b040: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001b050: 7175 616c 2872 6570 7228 6c69 292c 2022  qual(repr(li), "
-0001b060: 4c69 6e65 496e 666f 286c 696e 653d 2727  LineInfo(line=''
-0001b070: 2c20 6c69 6e65 5f6e 756d 6265 723d 312c  , line_number=1,
-0001b080: 2063 6f6c 756d 6e5f 6e75 6d62 6572 3d31   column_number=1
-0001b090: 2c20 696e 6465 6e74 3d30 2922 290a 0a20  , indent=0)").. 
-0001b0a0: 2020 2020 2020 2023 2320 6572 726f 7220         ## error 
-0001b0b0: 6861 6e64 6c69 6e67 0a20 2020 2020 2020  handling.       
-0001b0c0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-0001b0d0: 7452 6169 7365 7328 5479 7065 4572 726f  tRaises(TypeErro
-0001b0e0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0001b0f0: 6269 672e 6c69 6e65 7328 2222 2c20 6c69  big.lines("", li
-0001b100: 6e65 5f6e 756d 6265 723d 6d61 7468 2e70  ne_number=math.p
-0001b110: 6929 0a20 2020 2020 2020 2077 6974 6820  i).        with 
-0001b120: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-0001b130: 7328 5479 7065 4572 726f 7229 3a0a 2020  s(TypeError):.  
-0001b140: 2020 2020 2020 2020 2020 6269 672e 6c69            big.li
-0001b150: 6e65 7328 2222 2c20 636f 6c75 6d6e 5f6e  nes("", column_n
-0001b160: 756d 6265 723d 6d61 7468 2e70 6929 0a20  umber=math.pi). 
-0001b170: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0001b180: 2e61 7373 6572 7452 6169 7365 7328 5479  .assertRaises(Ty
-0001b190: 7065 4572 726f 7229 3a0a 2020 2020 2020  peError):.      
-0001b1a0: 2020 2020 2020 6269 672e 6c69 6e65 7328        big.lines(
-0001b1b0: 2222 2c20 7461 625f 7769 6474 683d 6d61  "", tab_width=ma
-0001b1c0: 7468 2e70 6929 0a0a 2020 2020 2020 2020  th.pi)..        
-0001b1d0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-0001b1e0: 5261 6973 6573 2854 7970 6545 7272 6f72  Raises(TypeError
-0001b1f0: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
-0001b200: 6967 2e4c 696e 6549 6e66 6f28 6d61 7468  ig.LineInfo(math
-0001b210: 2e70 692c 2031 2c20 3129 0a20 2020 2020  .pi, 1, 1).     
-0001b220: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-0001b230: 6572 7452 6169 7365 7328 5479 7065 4572  ertRaises(TypeEr
-0001b240: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0001b250: 2020 6269 672e 4c69 6e65 496e 666f 2827    big.LineInfo('
-0001b260: 272c 206d 6174 682e 7069 2c20 3129 0a20  ', math.pi, 1). 
-0001b270: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0001b280: 2e61 7373 6572 7452 6169 7365 7328 5479  .assertRaises(Ty
-0001b290: 7065 4572 726f 7229 3a0a 2020 2020 2020  peError):.      
-0001b2a0: 2020 2020 2020 6269 672e 4c69 6e65 496e        big.LineIn
-0001b2b0: 666f 2827 272c 2031 2c20 6d61 7468 2e70  fo('', 1, math.p
-0001b2c0: 6929 0a0a 2020 2020 2020 2020 7769 7468  i)..        with
-0001b2d0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-0001b2e0: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
-0001b2f0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-0001b300: 2862 6967 2e6c 696e 6573 5f66 696c 7465  (big.lines_filte
-0001b310: 725f 636f 6d6d 656e 745f 6c69 6e65 7328  r_comment_lines(
-0001b320: 2222 2c20 5b5d 2929 0a20 2020 2020 2020  "", [])).       
-0001b330: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-0001b340: 7452 6169 7365 7328 5479 7065 4572 726f  tRaises(TypeErro
-0001b350: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0001b360: 6c69 7374 2862 6967 2e6c 696e 6573 5f66  list(big.lines_f
-0001b370: 696c 7465 725f 636f 6d6d 656e 745f 6c69  ilter_comment_li
-0001b380: 6e65 7328 2222 2c20 6d61 7468 2e70 6929  nes("", math.pi)
-0001b390: 290a 0a20 2020 2020 2020 2023 2320 7465  )..        ## te
-0001b3a0: 7374 206b 7761 7267 730a 2020 2020 2020  st kwargs.      
-0001b3b0: 2020 6920 3d20 6269 672e 6c69 6e65 7328    i = big.lines(
-0001b3c0: 2727 2c20 7175 6172 6b3d 3232 290a 2020  '', quark=22).  
-0001b3d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001b3e0: 7454 7275 6528 6861 7361 7474 7228 692c  tTrue(hasattr(i,
-0001b3f0: 2027 7175 6172 6b27 2929 0a20 2020 2020   'quark')).     
-0001b400: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001b410: 7561 6c28 6765 7461 7474 7228 692c 2027  ual(getattr(i, '
-0001b420: 7175 6172 6b27 292c 2032 3229 0a0a 2020  quark'), 22)..  
-0001b430: 2020 2020 2020 696e 666f 203d 2062 6967        info = big
-0001b440: 2e4c 696e 6549 6e66 6f28 2727 2c20 312c  .LineInfo('', 1,
-0001b450: 2031 2c20 7175 6172 6b3d 3335 290a 2020   1, quark=35).  
-0001b460: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001b470: 7454 7275 6528 6861 7361 7474 7228 696e  tTrue(hasattr(in
-0001b480: 666f 2c20 2771 7561 726b 2729 290a 2020  fo, 'quark')).  
-0001b490: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001b4a0: 7445 7175 616c 2867 6574 6174 7472 2869  tEqual(getattr(i
-0001b4b0: 6e66 6f2c 2027 7175 6172 6b27 292c 2033  nfo, 'quark'), 3
-0001b4c0: 3529 0a0a 0a69 6d70 6f72 7420 6269 6774  5)...import bigt
-0001b4d0: 6573 746c 6962 0a0a 6465 6620 7275 6e5f  estlib..def run_
-0001b4e0: 7465 7374 7328 293a 0a20 2020 2062 6967  tests():.    big
-0001b4f0: 7465 7374 6c69 622e 7275 6e28 6e61 6d65  testlib.run(name
-0001b500: 3d22 6269 672e 7465 7874 222c 206d 6f64  ="big.text", mod
-0001b510: 756c 653d 5f5f 6e61 6d65 5f5f 290a 0a69  ule=__name__)..i
-0001b520: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
-0001b530: 5f6d 6169 6e5f 5f22 3a20 2320 7072 6167  _main__": # prag
-0001b540: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-0001b550: 2072 756e 5f74 6573 7473 2829 0a20 2020   run_tests().   
-0001b560: 2062 6967 7465 7374 6c69 622e 6669 6e69   bigtestlib.fini
-0001b570: 7368 2829 0a                             sh().
+0001a080: 2020 2020 2720 2020 2070 7269 6e74 2822      '    print("
+0001a090: 2320 7468 6973 2069 7320 7175 6f74 6564  # this is quoted
+0001a0a0: 222c 2078 2927 292c 0a20 2020 2020 2020  ", x)'),.       
+0001a0b0: 2020 2020 2020 2020 2028 4c49 286c 696e           (LI(lin
+0001a0c0: 653d 2720 2020 2070 7269 6e74 2822 2229  e='    print("")
+0001a0d0: 2023 2074 6869 7320 2263 6f6d 6d65 6e74   # this "comment
+0001a0e0: 2220 6973 2075 7365 6c65 7373 272c 206c  " is useless', l
+0001a0f0: 696e 655f 6e75 6d62 6572 3d33 2c20 636f  ine_number=3, co
+0001a100: 6c75 6d6e 5f6e 756d 6265 723d 312c 2063  lumn_number=1, c
+0001a110: 6f6d 6d65 6e74 3d27 2320 7468 6973 2022  omment='# this "
+0001a120: 636f 6d6d 656e 7422 2069 7320 7573 656c  comment" is usel
+0001a130: 6573 7327 292c 0a20 2020 2020 2020 2020  ess'),.         
+0001a140: 2020 2020 2020 2020 2020 2027 2020 2020             '    
+0001a150: 7072 696e 7428 2222 2927 292c 0a20 2020  print("")'),.   
+0001a160: 2020 2020 2020 2020 2020 2020 2028 4c49               (LI
+0001a170: 286c 696e 653d 2720 2020 2070 7269 6e74  (line='    print
+0001a180: 286e 6f5f 636f 6d6d 656e 7473 5f6f 725f  (no_comments_or_
+0001a190: 7175 6f74 6573 5f6f 6e5f 7468 6973 5f6c  quotes_on_this_l
+0001a1a0: 696e 6529 272c 206c 696e 655f 6e75 6d62  ine)', line_numb
+0001a1b0: 6572 3d34 2c20 636f 6c75 6d6e 5f6e 756d  er=4, column_num
+0001a1c0: 6265 723d 312c 2063 6f6d 6d65 6e74 3d27  ber=1, comment='
+0001a1d0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001a1e0: 2020 2020 2020 2020 2720 2020 2070 7269          '    pri
+0001a1f0: 6e74 286e 6f5f 636f 6d6d 656e 7473 5f6f  nt(no_comments_o
+0001a200: 725f 7175 6f74 6573 5f6f 6e5f 7468 6973  r_quotes_on_this
+0001a210: 5f6c 696e 6529 2729 2c0a 2020 2020 2020  _line)'),.      
+0001a220: 2020 2020 2020 2020 2020 284c 4928 6c69            (LI(li
+0001a230: 6e65 3d27 272c 206c 696e 655f 6e75 6d62  ne='', line_numb
+0001a240: 6572 3d35 2c20 636f 6c75 6d6e 5f6e 756d  er=5, column_num
+0001a250: 6265 723d 312c 2063 6f6d 6d65 6e74 3d27  ber=1, comment='
+0001a260: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001a270: 2020 2020 2020 2020 2727 290a 2020 2020          '').    
+0001a280: 2020 2020 2020 2020 5d29 0a0a 2020 2020          ])..    
+0001a290: 2020 2020 7465 7374 2862 6967 2e6c 696e      test(big.lin
+0001a2a0: 6573 5f73 7472 6970 5f63 6f6d 6d65 6e74  es_strip_comment
+0001a2b0: 7328 6269 672e 6c69 6e65 7328 2222 220a  s(big.lines(""".
+0001a2c0: 666f 7220 7820 696e 2072 616e 6765 2835  for x in range(5
+0001a2d0: 293a 2023 2074 6869 7320 6973 2061 2063  ): # this is a c
+0001a2e0: 6f6d 6d65 6e74 0a20 2020 2070 7269 6e74  omment.    print
+0001a2f0: 2822 2320 7468 6973 2069 7320 7175 6f74  ("# this is quot
+0001a300: 6564 222c 2078 290a 2020 2020 7072 696e  ed", x).    prin
+0001a310: 7428 2222 2920 2320 7468 6973 2022 636f  t("") # this "co
+0001a320: 6d6d 656e 7422 2069 7320 7573 656c 6573  mment" is useles
+0001a330: 730a 2020 2020 7072 696e 7428 6e6f 5f63  s.    print(no_c
+0001a340: 6f6d 6d65 6e74 735f 6f72 5f71 756f 7465  omments_or_quote
+0001a350: 735f 6f6e 5f74 6869 735f 6c69 6e65 290a  s_on_this_line).
+0001a360: 2222 225b 313a 5d29 2c20 2822 2322 2c20  """[1:]), ("#", 
+0001a370: 222f 2f22 292c 2071 756f 7465 733d 4e6f  "//"), quotes=No
+0001a380: 6e65 292c 0a20 2020 2020 2020 2020 2020  ne),.           
+0001a390: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0001a3a0: 2020 2028 4c49 286c 696e 653d 2766 6f72     (LI(line='for
+0001a3b0: 2078 2069 6e20 7261 6e67 6528 3529 3a20   x in range(5): 
+0001a3c0: 2320 7468 6973 2069 7320 6120 636f 6d6d  # this is a comm
+0001a3d0: 656e 7427 2c20 6c69 6e65 5f6e 756d 6265  ent', line_numbe
+0001a3e0: 723d 312c 2063 6f6c 756d 6e5f 6e75 6d62  r=1, column_numb
+0001a3f0: 6572 3d31 2c20 636f 6d6d 656e 743d 2723  er=1, comment='#
+0001a400: 2074 6869 7320 6973 2061 2063 6f6d 6d65   this is a comme
+0001a410: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
+0001a420: 2020 2020 2020 2020 2766 6f72 2078 2069          'for x i
+0001a430: 6e20 7261 6e67 6528 3529 3a27 292c 0a20  n range(5):'),. 
+0001a440: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001a450: 4c49 286c 696e 653d 2720 2020 2070 7269  LI(line='    pri
+0001a460: 6e74 2822 2320 7468 6973 2069 7320 7175  nt("# this is qu
+0001a470: 6f74 6564 222c 2078 2927 2c20 6c69 6e65  oted", x)', line
+0001a480: 5f6e 756d 6265 723d 322c 2063 6f6c 756d  _number=2, colum
+0001a490: 6e5f 6e75 6d62 6572 3d31 2c20 636f 6d6d  n_number=1, comm
+0001a4a0: 656e 743d 2723 2074 6869 7320 6973 2071  ent='# this is q
+0001a4b0: 756f 7465 6422 2c20 7829 2729 2c0a 2020  uoted", x)'),.  
+0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4d0: 2020 2720 2020 2070 7269 6e74 2822 2729    '    print("')
+0001a4e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a4f0: 2020 284c 4928 6c69 6e65 3d27 2020 2020    (LI(line='    
+0001a500: 7072 696e 7428 2222 2920 2320 7468 6973  print("") # this
+0001a510: 2022 636f 6d6d 656e 7422 2069 7320 7573   "comment" is us
+0001a520: 656c 6573 7327 2c20 6c69 6e65 5f6e 756d  eless', line_num
+0001a530: 6265 723d 332c 2063 6f6c 756d 6e5f 6e75  ber=3, column_nu
+0001a540: 6d62 6572 3d31 2c20 636f 6d6d 656e 743d  mber=1, comment=
+0001a550: 2723 2074 6869 7320 2263 6f6d 6d65 6e74  '# this "comment
+0001a560: 2220 6973 2075 7365 6c65 7373 2729 2c0a  " is useless'),.
+0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a580: 2020 2020 2720 2020 2070 7269 6e74 2822      '    print("
+0001a590: 2229 2729 2c0a 2020 2020 2020 2020 2020  ")'),.          
+0001a5a0: 2020 2020 2020 284c 4928 6c69 6e65 3d27        (LI(line='
+0001a5b0: 2020 2020 7072 696e 7428 6e6f 5f63 6f6d      print(no_com
+0001a5c0: 6d65 6e74 735f 6f72 5f71 756f 7465 735f  ments_or_quotes_
+0001a5d0: 6f6e 5f74 6869 735f 6c69 6e65 2927 2c20  on_this_line)', 
+0001a5e0: 6c69 6e65 5f6e 756d 6265 723d 342c 2063  line_number=4, c
+0001a5f0: 6f6c 756d 6e5f 6e75 6d62 6572 3d31 2c20  olumn_number=1, 
+0001a600: 636f 6d6d 656e 743d 2727 292c 0a20 2020  comment=''),.   
+0001a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a620: 2027 2020 2020 7072 696e 7428 6e6f 5f63   '    print(no_c
+0001a630: 6f6d 6d65 6e74 735f 6f72 5f71 756f 7465  omments_or_quote
+0001a640: 735f 6f6e 5f74 6869 735f 6c69 6e65 2927  s_on_this_line)'
+0001a650: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001a660: 2020 2028 4c49 286c 696e 653d 2727 2c20     (LI(line='', 
+0001a670: 6c69 6e65 5f6e 756d 6265 723d 352c 2063  line_number=5, c
+0001a680: 6f6c 756d 6e5f 6e75 6d62 6572 3d31 2c20  olumn_number=1, 
+0001a690: 636f 6d6d 656e 743d 2727 292c 0a20 2020  comment=''),.   
+0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6b0: 2027 2729 2c0a 2020 2020 2020 2020 2020   ''),.          
+0001a6c0: 2020 5d29 0a0a 2020 2020 2020 2020 7769    ])..        wi
+0001a6d0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0001a6e0: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+0001a6f0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+0001a700: 7374 2862 6967 2e6c 696e 6573 5f73 7472  st(big.lines_str
+0001a710: 6970 5f63 6f6d 6d65 6e74 7328 6269 672e  ip_comments(big.
+0001a720: 6c69 6e65 7328 2261 5c6e 625c 6e22 292c  lines("a\nb\n"),
+0001a730: 204e 6f6e 6529 2c20 5b5d 290a 0a20 2020   None), [])..   
+0001a740: 2020 2020 2074 6573 7428 6269 672e 6c69       test(big.li
+0001a750: 6e65 735f 7374 7269 705f 636f 6d6d 656e  nes_strip_commen
+0001a760: 7473 2862 6967 2e6c 696e 6573 2862 2261  ts(big.lines(b"a
+0001a770: 5c6e 6223 2069 676e 6f72 6564 5c6e 2063  \nb# ignored\n c
+0001a780: 2229 2c20 6227 2327 292c 0a20 2020 2020  "), b'#'),.     
+0001a790: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+0001a7a0: 2020 2020 204c 2862 2761 272c 2031 2c20       L(b'a', 1, 
+0001a7b0: 636f 6d6d 656e 743d 6227 2729 2c0a 2020  comment=b''),.  
+0001a7c0: 2020 2020 2020 2020 2020 284c 4928 6227            (LI(b'
+0001a7d0: 6223 2069 676e 6f72 6564 272c 2032 2c20  b# ignored', 2, 
+0001a7e0: 312c 2063 6f6d 6d65 6e74 3d62 2723 2069  1, comment=b'# i
+0001a7f0: 676e 6f72 6564 2729 2c20 6227 6227 292c  gnored'), b'b'),
+0001a800: 0a20 2020 2020 2020 2020 2020 204c 2862  .            L(b
+0001a810: 2720 6327 2c20 332c 2063 6f6d 6d65 6e74  ' c', 3, comment
+0001a820: 3d62 2727 292c 0a20 2020 2020 2020 2020  =b''),.         
+0001a830: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+0001a840: 2029 0a0a 0a20 2020 2020 2020 2074 6573   )...        tes
+0001a850: 7428 6269 672e 6c69 6e65 735f 6669 6c74  t(big.lines_filt
+0001a860: 6572 5f65 6d70 7479 5f6c 696e 6573 2862  er_empty_lines(b
+0001a870: 6967 2e6c 696e 6573 5f66 696c 7465 725f  ig.lines_filter_
+0001a880: 636f 6d6d 656e 745f 6c69 6e65 7328 6269  comment_lines(bi
+0001a890: 672e 6c69 6e65 735f 7374 7269 7028 6269  g.lines_strip(bi
+0001a8a0: 672e 6c69 6e65 7328 0a22 2020 205c 6e22  g.lines(."   \n"
+0001a8b0: 202b 0a22 2020 2020 6120 3d20 6220 5c6e   +."    a = b \n
+0001a8c0: 2220 2b0a 2220 2020 5c6e 2220 2b0a 2220  " +."   \n" +." 
+0001a8d0: 2020 2023 2063 6f6d 6d65 6e74 206c 696e     # comment lin
+0001a8e0: 6520 5c6e 2220 2b0a 2220 2020 205c 6e22  e \n" +."    \n"
+0001a8f0: 202b 0a22 2020 2020 5c6e 2220 2b0a 2220   +."    \n" +." 
+0001a900: 2020 2063 203d 2064 2020 5c6e 2220 2b0a     c = d  \n" +.
+0001a910: 2220 2020 2020 5c6e 2229 292c 2027 2327  "     \n")), '#'
+0001a920: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+0001a930: 5b0a 2020 2020 2020 2020 2020 2020 284c  [.            (L
+0001a940: 4928 2720 2020 2061 203d 2062 2027 2c20  I('    a = b ', 
+0001a950: 2032 2c20 352c 206c 6561 6469 6e67 3d27   2, 5, leading='
+0001a960: 2020 2020 2729 2c20 2761 203d 2062 2729      '), 'a = b')
+0001a970: 2c0a 2020 2020 2020 2020 2020 2020 284c  ,.            (L
+0001a980: 4928 2720 2020 2063 203d 2064 2020 272c  I('    c = d  ',
+0001a990: 2037 2c20 352c 206c 6561 6469 6e67 3d27   7, 5, leading='
+0001a9a0: 2020 2020 2729 2c20 2763 203d 2064 2729      '), 'c = d')
+0001a9b0: 2c0a 2020 2020 2020 2020 2020 2020 5d29  ,.            ])
+0001a9c0: 0a0a 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
+0001a9d0: 6c69 6e65 735f 7374 7269 705f 696e 6465  lines_strip_inde
+0001a9e0: 6e74 2873 656c 6629 3a0a 2020 2020 2020  nt(self):.      
+0001a9f0: 2020 6465 6620 7465 7374 286c 696e 6573    def test(lines
+0001aa00: 2c20 6578 7065 6374 6564 2c20 2a2c 2074  , expected, *, t
+0001aa10: 6162 5f77 6964 7468 3d38 293a 0a20 2020  ab_width=8):.   
+0001aa20: 2020 2020 2020 2020 2067 6f74 203d 206c           got = l
+0001aa30: 6973 7428 6269 672e 6c69 6e65 735f 7374  ist(big.lines_st
+0001aa40: 7269 705f 696e 6465 6e74 2862 6967 2e6c  rip_indent(big.l
+0001aa50: 696e 6573 286c 696e 6573 2c20 7461 625f  ines(lines, tab_
+0001aa60: 7769 6474 683d 7461 625f 7769 6474 6829  width=tab_width)
+0001aa70: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+0001aa80: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001aa90: 676f 742c 2065 7870 6563 7465 6429 0a0a  got, expected)..
+0001aaa0: 0a20 2020 2020 2020 204c 696e 6549 6e66  .        LineInf
+0001aab0: 6f20 3d20 6269 672e 7465 7874 2e4c 696e  o = big.text.Lin
+0001aac0: 6549 6e66 6f0a 0a20 2020 2020 2020 206c  eInfo..        l
+0001aad0: 696e 6573 203d 2022 2222 0a6c 6566 7420  ines = """.left 
+0001aae0: 6d61 7267 696e 0a69 6620 333a 0a20 2020  margin.if 3:.   
+0001aaf0: 2074 6578 740a 656c 7365 3a0a 2020 2020   text.else:.    
+0001ab00: 6966 2031 3a0a 2020 2020 2020 2020 2020  if 1:.          
+0001ab10: 6f74 6865 7220 7465 7874 0a20 2020 2020  other text.     
+0001ab20: 2020 2020 206f 7468 6572 2074 6578 740a       other text.
+0001ab30: 2020 2020 6d6f 7265 2074 6578 740a 2020      more text.  
+0001ab40: 2020 2020 6469 6666 6572 656e 7420 696e      different in
+0001ab50: 6465 6e74 0a20 2020 206f 7574 6465 6e74  dent.    outdent
+0001ab60: 0a6f 7574 6465 6e74 0a20 206e 6577 2069  .outdent.  new i
+0001ab70: 6e64 656e 740a 6f75 7464 656e 740a 2222  ndent.outdent.""
+0001ab80: 220a 0a20 2020 2020 2020 2065 7870 6563  "..        expec
+0001ab90: 7465 6420 3d20 5b0a 2020 2020 2020 2020  ted = [.        
+0001aba0: 2020 2020 284c 696e 6549 6e66 6f28 6c69      (LineInfo(li
+0001abb0: 6e65 3d27 272c 206c 696e 655f 6e75 6d62  ne='', line_numb
+0001abc0: 6572 3d31 2c20 636f 6c75 6d6e 5f6e 756d  er=1, column_num
+0001abd0: 6265 723d 312c 2069 6e64 656e 743d 302c  ber=1, indent=0,
+0001abe0: 206c 6561 6469 6e67 3d27 2729 2c0a 2020   leading=''),.  
+0001abf0: 2020 2020 2020 2020 2020 2020 2020 2727                ''
+0001ac00: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001ac10: 4c69 6e65 496e 666f 286c 696e 653d 276c  LineInfo(line='l
+0001ac20: 6566 7420 6d61 7267 696e 272c 206c 696e  eft margin', lin
+0001ac30: 655f 6e75 6d62 6572 3d32 2c20 636f 6c75  e_number=2, colu
+0001ac40: 6d6e 5f6e 756d 6265 723d 312c 2069 6e64  mn_number=1, ind
+0001ac50: 656e 743d 302c 206c 6561 6469 6e67 3d27  ent=0, leading='
+0001ac60: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001ac70: 2020 2020 276c 6566 7420 6d61 7267 696e      'left margin
+0001ac80: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001ac90: 284c 696e 6549 6e66 6f28 6c69 6e65 3d27  (LineInfo(line='
+0001aca0: 6966 2033 3a27 2c20 6c69 6e65 5f6e 756d  if 3:', line_num
+0001acb0: 6265 723d 332c 2063 6f6c 756d 6e5f 6e75  ber=3, column_nu
+0001acc0: 6d62 6572 3d31 2c20 696e 6465 6e74 3d30  mber=1, indent=0
+0001acd0: 2c20 6c65 6164 696e 673d 2727 292c 0a20  , leading=''),. 
+0001ace0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001acf0: 6966 2033 3a27 292c 0a20 2020 2020 2020  if 3:'),.       
+0001ad00: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
+0001ad10: 696e 653d 2720 2020 2074 6578 7427 2c20  ine='    text', 
+0001ad20: 6c69 6e65 5f6e 756d 6265 723d 342c 2063  line_number=4, c
+0001ad30: 6f6c 756d 6e5f 6e75 6d62 6572 3d35 2c20  olumn_number=5, 
+0001ad40: 696e 6465 6e74 3d31 2c20 6c65 6164 696e  indent=1, leadin
+0001ad50: 673d 2720 2020 2027 292c 0a20 2020 2020  g='    '),.     
+0001ad60: 2020 2020 2020 2020 2020 2027 7465 7874             'text
+0001ad70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001ad80: 284c 696e 6549 6e66 6f28 6c69 6e65 3d27  (LineInfo(line='
+0001ad90: 656c 7365 3a27 2c20 6c69 6e65 5f6e 756d  else:', line_num
+0001ada0: 6265 723d 352c 2063 6f6c 756d 6e5f 6e75  ber=5, column_nu
+0001adb0: 6d62 6572 3d31 2c20 696e 6465 6e74 3d30  mber=1, indent=0
+0001adc0: 2c20 6c65 6164 696e 673d 2727 292c 0a20  , leading=''),. 
+0001add0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001ade0: 656c 7365 3a27 292c 0a20 2020 2020 2020  else:'),.       
+0001adf0: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
+0001ae00: 696e 653d 2720 2020 2069 6620 313a 272c  ine='    if 1:',
+0001ae10: 206c 696e 655f 6e75 6d62 6572 3d36 2c20   line_number=6, 
+0001ae20: 636f 6c75 6d6e 5f6e 756d 6265 723d 352c  column_number=5,
+0001ae30: 2069 6e64 656e 743d 312c 206c 6561 6469   indent=1, leadi
+0001ae40: 6e67 3d27 2020 2020 2729 2c0a 2020 2020  ng='    '),.    
+0001ae50: 2020 2020 2020 2020 2020 2020 2769 6620              'if 
+0001ae60: 313a 2729 2c0a 2020 2020 2020 2020 2020  1:'),.          
+0001ae70: 2020 284c 696e 6549 6e66 6f28 6c69 6e65    (LineInfo(line
+0001ae80: 3d27 2020 2020 2020 2020 2020 6f74 6865  ='          othe
+0001ae90: 7220 7465 7874 272c 206c 696e 655f 6e75  r text', line_nu
+0001aea0: 6d62 6572 3d37 2c20 636f 6c75 6d6e 5f6e  mber=7, column_n
+0001aeb0: 756d 6265 723d 3131 2c20 696e 6465 6e74  umber=11, indent
+0001aec0: 3d32 2c20 6c65 6164 696e 673d 2720 2020  =2, leading='   
+0001aed0: 2020 2020 2020 2027 292c 0a20 2020 2020         '),.     
+0001aee0: 2020 2020 2020 2020 2020 2027 6f74 6865             'othe
+0001aef0: 7220 7465 7874 2729 2c0a 2020 2020 2020  r text'),.      
+0001af00: 2020 2020 2020 284c 696e 6549 6e66 6f28        (LineInfo(
+0001af10: 6c69 6e65 3d27 2020 2020 2020 2020 2020  line='          
+0001af20: 6f74 6865 7220 7465 7874 272c 206c 696e  other text', lin
+0001af30: 655f 6e75 6d62 6572 3d38 2c20 636f 6c75  e_number=8, colu
+0001af40: 6d6e 5f6e 756d 6265 723d 3131 2c20 696e  mn_number=11, in
+0001af50: 6465 6e74 3d32 2c20 6c65 6164 696e 673d  dent=2, leading=
+0001af60: 2720 2020 2020 2020 2020 2027 292c 0a20  '          '),. 
+0001af70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001af80: 6f74 6865 7220 7465 7874 2729 2c0a 2020  other text'),.  
+0001af90: 2020 2020 2020 2020 2020 284c 696e 6549            (LineI
+0001afa0: 6e66 6f28 6c69 6e65 3d27 2020 2020 6d6f  nfo(line='    mo
+0001afb0: 7265 2074 6578 7427 2c20 6c69 6e65 5f6e  re text', line_n
+0001afc0: 756d 6265 723d 392c 2063 6f6c 756d 6e5f  umber=9, column_
+0001afd0: 6e75 6d62 6572 3d35 2c20 696e 6465 6e74  number=5, indent
+0001afe0: 3d31 2c20 6c65 6164 696e 673d 2720 2020  =1, leading='   
+0001aff0: 2027 292c 0a20 2020 2020 2020 2020 2020   '),.           
+0001b000: 2020 2020 2027 6d6f 7265 2074 6578 7427       'more text'
+0001b010: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001b020: 4c69 6e65 496e 666f 286c 696e 653d 2720  LineInfo(line=' 
+0001b030: 2020 2020 2064 6966 6665 7265 6e74 2069       different i
+0001b040: 6e64 656e 7427 2c20 6c69 6e65 5f6e 756d  ndent', line_num
+0001b050: 6265 723d 3130 2c20 636f 6c75 6d6e 5f6e  ber=10, column_n
+0001b060: 756d 6265 723d 372c 2069 6e64 656e 743d  umber=7, indent=
+0001b070: 322c 206c 6561 6469 6e67 3d27 2020 2020  2, leading='    
+0001b080: 2020 2729 2c0a 2020 2020 2020 2020 2020    '),.          
+0001b090: 2020 2020 2020 2764 6966 6665 7265 6e74        'different
+0001b0a0: 2069 6e64 656e 7427 292c 0a20 2020 2020   indent'),.     
+0001b0b0: 2020 2020 2020 2028 4c69 6e65 496e 666f         (LineInfo
+0001b0c0: 286c 696e 653d 2720 2020 206f 7574 6465  (line='    outde
+0001b0d0: 6e74 272c 206c 696e 655f 6e75 6d62 6572  nt', line_number
+0001b0e0: 3d31 312c 2063 6f6c 756d 6e5f 6e75 6d62  =11, column_numb
+0001b0f0: 6572 3d35 2c20 696e 6465 6e74 3d31 2c20  er=5, indent=1, 
+0001b100: 6c65 6164 696e 673d 2720 2020 2027 292c  leading='    '),
+0001b110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b120: 2027 6f75 7464 656e 7427 292c 0a20 2020   'outdent'),.   
+0001b130: 2020 2020 2020 2020 2028 4c69 6e65 496e           (LineIn
+0001b140: 666f 286c 696e 653d 276f 7574 6465 6e74  fo(line='outdent
+0001b150: 272c 206c 696e 655f 6e75 6d62 6572 3d31  ', line_number=1
+0001b160: 322c 2063 6f6c 756d 6e5f 6e75 6d62 6572  2, column_number
+0001b170: 3d31 2c20 696e 6465 6e74 3d30 2c20 6c65  =1, indent=0, le
+0001b180: 6164 696e 673d 2727 292c 0a20 2020 2020  ading=''),.     
+0001b190: 2020 2020 2020 2020 2020 2027 6f75 7464             'outd
+0001b1a0: 656e 7427 292c 0a20 2020 2020 2020 2020  ent'),.         
+0001b1b0: 2020 2028 4c69 6e65 496e 666f 286c 696e     (LineInfo(lin
+0001b1c0: 653d 2720 206e 6577 2069 6e64 656e 7427  e='  new indent'
+0001b1d0: 2c20 6c69 6e65 5f6e 756d 6265 723d 3133  , line_number=13
+0001b1e0: 2c20 636f 6c75 6d6e 5f6e 756d 6265 723d  , column_number=
+0001b1f0: 332c 2069 6e64 656e 743d 312c 206c 6561  3, indent=1, lea
+0001b200: 6469 6e67 3d27 2020 2729 2c0a 2020 2020  ding='  '),.    
+0001b210: 2020 2020 2020 2020 2020 2020 276e 6577              'new
+0001b220: 2069 6e64 656e 7427 292c 0a20 2020 2020   indent'),.     
+0001b230: 2020 2020 2020 2028 4c69 6e65 496e 666f         (LineInfo
+0001b240: 286c 696e 653d 276f 7574 6465 6e74 272c  (line='outdent',
+0001b250: 206c 696e 655f 6e75 6d62 6572 3d31 342c   line_number=14,
+0001b260: 2063 6f6c 756d 6e5f 6e75 6d62 6572 3d31   column_number=1
+0001b270: 2c20 696e 6465 6e74 3d30 2c20 6c65 6164  , indent=0, lead
+0001b280: 696e 673d 2727 292c 0a20 2020 2020 2020  ing=''),.       
+0001b290: 2020 2020 2020 2020 2027 6f75 7464 656e           'outden
+0001b2a0: 7427 292c 0a20 2020 2020 2020 2020 2020  t'),.           
+0001b2b0: 2028 4c69 6e65 496e 666f 286c 696e 653d   (LineInfo(line=
+0001b2c0: 2727 2c20 6c69 6e65 5f6e 756d 6265 723d  '', line_number=
+0001b2d0: 3135 2c20 636f 6c75 6d6e 5f6e 756d 6265  15, column_numbe
+0001b2e0: 723d 312c 2069 6e64 656e 743d 302c 206c  r=1, indent=0, l
+0001b2f0: 6561 6469 6e67 3d27 2729 2c0a 2020 2020  eading=''),.    
+0001b300: 2020 2020 2020 2020 2020 2020 2727 292c              ''),
+0001b310: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
+0001b320: 2020 2020 2020 2020 7465 7374 286c 696e          test(lin
+0001b330: 6573 2c20 6578 7065 6374 6564 290a 0a0a  es, expected)...
+0001b340: 2020 2020 2020 2020 2323 0a20 2020 2020          ##.     
+0001b350: 2020 2023 2320 7465 7374 2074 6162 2074     ## test tab t
+0001b360: 6f20 7370 6163 6573 0a20 2020 2020 2020  o spaces.       
+0001b370: 2023 230a 0a20 2020 2020 2020 206c 696e   ##..        lin
+0001b380: 6573 203d 2028 0a20 2020 2020 2020 2022  es = (.        "
+0001b390: 6c65 6674 206d 6172 6769 6e5c 6e22 0a20  left margin\n". 
+0001b3a0: 2020 2020 2020 2022 5c74 6569 6768 745c         "\teight\
+0001b3b0: 6e22 0a20 2020 2020 2020 2022 2020 5c74  n".        "  \t
+0001b3c0: 2020 2020 7477 656c 7665 5c6e 220a 2020      twelve\n".  
+0001b3d0: 2020 2020 2020 2220 2020 2020 2020 2065        "        e
+0001b3e0: 6967 6874 2069 7320 656e 6f75 6768 5c6e  ight is enough\n
+0001b3f0: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
+0001b400: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+0001b410: 5b0a 2020 2020 2020 2020 2020 2020 284c  [.            (L
+0001b420: 696e 6549 6e66 6f28 6c69 6e65 3d27 6c65  ineInfo(line='le
+0001b430: 6674 206d 6172 6769 6e27 2c20 6c69 6e65  ft margin', line
+0001b440: 5f6e 756d 6265 723d 312c 2063 6f6c 756d  _number=1, colum
+0001b450: 6e5f 6e75 6d62 6572 3d31 2c20 696e 6465  n_number=1, inde
+0001b460: 6e74 3d30 2c20 6c65 6164 696e 673d 2727  nt=0, leading=''
+0001b470: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001b480: 2020 2027 6c65 6674 206d 6172 6769 6e27     'left margin'
+0001b490: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001b4a0: 4c69 6e65 496e 666f 286c 696e 653d 275c  LineInfo(line='\
+0001b4b0: 7465 6967 6874 272c 206c 696e 655f 6e75  teight', line_nu
+0001b4c0: 6d62 6572 3d32 2c20 636f 6c75 6d6e 5f6e  mber=2, column_n
+0001b4d0: 756d 6265 723d 392c 2069 6e64 656e 743d  umber=9, indent=
+0001b4e0: 312c 206c 6561 6469 6e67 3d27 5c74 2729  1, leading='\t')
+0001b4f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b500: 2020 2765 6967 6874 2729 2c0a 2020 2020    'eight'),.    
+0001b510: 2020 2020 2020 2020 284c 696e 6549 6e66          (LineInf
+0001b520: 6f28 6c69 6e65 3d27 2020 5c74 2020 2020  o(line='  \t    
+0001b530: 7477 656c 7665 272c 206c 696e 655f 6e75  twelve', line_nu
+0001b540: 6d62 6572 3d33 2c20 636f 6c75 6d6e 5f6e  mber=3, column_n
+0001b550: 756d 6265 723d 3133 2c20 696e 6465 6e74  umber=13, indent
+0001b560: 3d32 2c20 6c65 6164 696e 673d 2720 205c  =2, leading='  \
+0001b570: 7420 2020 2027 292c 0a20 2020 2020 2020  t    '),.       
+0001b580: 2020 2020 2020 2020 2027 7477 656c 7665           'twelve
+0001b590: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001b5a0: 284c 696e 6549 6e66 6f28 6c69 6e65 3d27  (LineInfo(line='
+0001b5b0: 2020 2020 2020 2020 6569 6768 7420 6973          eight is
+0001b5c0: 2065 6e6f 7567 6827 2c20 6c69 6e65 5f6e   enough', line_n
+0001b5d0: 756d 6265 723d 342c 2063 6f6c 756d 6e5f  umber=4, column_
+0001b5e0: 6e75 6d62 6572 3d39 2c20 696e 6465 6e74  number=9, indent
+0001b5f0: 3d31 2c20 6c65 6164 696e 673d 2720 2020  =1, leading='   
+0001b600: 2020 2020 2027 292c 0a20 2020 2020 2020       '),.       
+0001b610: 2020 2020 2020 2020 2027 6569 6768 7420           'eight 
+0001b620: 6973 2065 6e6f 7567 6827 292c 0a20 2020  is enough'),.   
+0001b630: 2020 2020 2020 2020 2028 4c69 6e65 496e           (LineIn
+0001b640: 666f 286c 696e 653d 2727 2c20 6c69 6e65  fo(line='', line
+0001b650: 5f6e 756d 6265 723d 352c 2063 6f6c 756d  _number=5, colum
+0001b660: 6e5f 6e75 6d62 6572 3d31 2c20 696e 6465  n_number=1, inde
+0001b670: 6e74 3d30 2c20 6c65 6164 696e 673d 2727  nt=0, leading=''
+0001b680: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001b690: 2020 2027 2729 0a20 2020 2020 2020 2020     '').         
+0001b6a0: 2020 205d 0a0a 2020 2020 2020 2020 7465     ]..        te
+0001b6b0: 7374 286c 696e 6573 2c20 6578 7065 6374  st(lines, expect
+0001b6c0: 6564 290a 0a20 2020 2020 2020 206c 696e  ed)..        lin
+0001b6d0: 6573 203d 2028 0a20 2020 2020 2020 2020  es = (.         
+0001b6e0: 2020 2022 6c65 6674 206d 6172 6769 6e5c     "left margin\
+0001b6f0: 6e22 0a20 2020 2020 2020 2020 2020 2022  n".            "
+0001b700: 5c74 666f 7572 5c6e 220a 2020 2020 2020  \tfour\n".      
+0001b710: 2020 2020 2020 2220 205c 7420 2020 2065        "  \t    e
+0001b720: 6967 6874 5c6e 220a 2020 2020 2020 2020  ight\n".        
+0001b730: 2020 2020 2220 205c 745c 7466 6967 7572      "  \t\tfigur
+0001b740: 6520 6569 6768 7420 6973 2064 6f75 626c  e eight is doubl
+0001b750: 6520 666f 7572 5c6e 220a 2020 2020 2020  e four\n".      
+0001b760: 2020 2020 2020 2220 2020 2066 6967 7572        "    figur
+0001b770: 6520 666f 7572 2069 7320 6861 6c66 206f  e four is half o
+0001b780: 6620 6569 6768 745c 6e22 0a20 2020 2020  f eight\n".     
+0001b790: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0001b7a0: 2020 6578 7065 6374 6564 203d 205b 0a20    expected = [. 
+0001b7b0: 2020 2020 2020 2020 2020 2028 4c69 6e65             (Line
+0001b7c0: 496e 666f 286c 696e 653d 276c 6566 7420  Info(line='left 
+0001b7d0: 6d61 7267 696e 272c 206c 696e 655f 6e75  margin', line_nu
+0001b7e0: 6d62 6572 3d31 2c20 636f 6c75 6d6e 5f6e  mber=1, column_n
+0001b7f0: 756d 6265 723d 312c 2069 6e64 656e 743d  umber=1, indent=
+0001b800: 302c 206c 6561 6469 6e67 3d27 2729 2c0a  0, leading=''),.
+0001b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b820: 276c 6566 7420 6d61 7267 696e 2729 2c0a  'left margin'),.
+0001b830: 2020 2020 2020 2020 2020 2020 284c 696e              (Lin
+0001b840: 6549 6e66 6f28 6c69 6e65 3d27 5c74 666f  eInfo(line='\tfo
+0001b850: 7572 272c 206c 696e 655f 6e75 6d62 6572  ur', line_number
+0001b860: 3d32 2c20 636f 6c75 6d6e 5f6e 756d 6265  =2, column_numbe
+0001b870: 723d 352c 2069 6e64 656e 743d 312c 206c  r=5, indent=1, l
+0001b880: 6561 6469 6e67 3d27 5c74 2729 2c0a 2020  eading='\t'),.  
+0001b890: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+0001b8a0: 6f75 7227 292c 0a20 2020 2020 2020 2020  our'),.         
+0001b8b0: 2020 2028 4c69 6e65 496e 666f 286c 696e     (LineInfo(lin
+0001b8c0: 653d 2720 205c 7420 2020 2065 6967 6874  e='  \t    eight
+0001b8d0: 272c 206c 696e 655f 6e75 6d62 6572 3d33  ', line_number=3
+0001b8e0: 2c20 636f 6c75 6d6e 5f6e 756d 6265 723d  , column_number=
+0001b8f0: 392c 2069 6e64 656e 743d 322c 206c 6561  9, indent=2, lea
+0001b900: 6469 6e67 3d27 2020 5c74 2020 2020 2729  ding='  \t    ')
+0001b910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b920: 2020 2765 6967 6874 2729 2c0a 2020 2020    'eight'),.    
+0001b930: 2020 2020 2020 2020 284c 696e 6549 6e66          (LineInf
+0001b940: 6f28 6c69 6e65 3d27 2020 5c74 5c74 6669  o(line='  \t\tfi
+0001b950: 6775 7265 2065 6967 6874 2069 7320 646f  gure eight is do
+0001b960: 7562 6c65 2066 6f75 7227 2c20 6c69 6e65  uble four', line
+0001b970: 5f6e 756d 6265 723d 342c 2063 6f6c 756d  _number=4, colum
+0001b980: 6e5f 6e75 6d62 6572 3d39 2c20 696e 6465  n_number=9, inde
+0001b990: 6e74 3d32 2c20 6c65 6164 696e 673d 2720  nt=2, leading=' 
+0001b9a0: 205c 745c 7427 292c 0a20 2020 2020 2020   \t\t'),.       
+0001b9b0: 2020 2020 2020 2020 2027 6669 6775 7265           'figure
+0001b9c0: 2065 6967 6874 2069 7320 646f 7562 6c65   eight is double
+0001b9d0: 2066 6f75 7227 292c 0a20 2020 2020 2020   four'),.       
+0001b9e0: 2020 2020 2028 4c69 6e65 496e 666f 286c       (LineInfo(l
+0001b9f0: 696e 653d 2720 2020 2066 6967 7572 6520  ine='    figure 
+0001ba00: 666f 7572 2069 7320 6861 6c66 206f 6620  four is half of 
+0001ba10: 6569 6768 7427 2c20 6c69 6e65 5f6e 756d  eight', line_num
+0001ba20: 6265 723d 352c 2063 6f6c 756d 6e5f 6e75  ber=5, column_nu
+0001ba30: 6d62 6572 3d35 2c20 696e 6465 6e74 3d31  mber=5, indent=1
+0001ba40: 2c20 6c65 6164 696e 673d 2720 2020 2027  , leading='    '
+0001ba50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001ba60: 2020 2027 6669 6775 7265 2066 6f75 7220     'figure four 
+0001ba70: 6973 2068 616c 6620 6f66 2065 6967 6874  is half of eight
+0001ba80: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001ba90: 284c 696e 6549 6e66 6f28 6c69 6e65 3d27  (LineInfo(line='
+0001baa0: 272c 206c 696e 655f 6e75 6d62 6572 3d36  ', line_number=6
+0001bab0: 2c20 636f 6c75 6d6e 5f6e 756d 6265 723d  , column_number=
+0001bac0: 312c 2069 6e64 656e 743d 302c 206c 6561  1, indent=0, lea
+0001bad0: 6469 6e67 3d27 2729 2c0a 2020 2020 2020  ding=''),.      
+0001bae0: 2020 2020 2020 2020 2020 2727 295d 0a0a            '')]..
+0001baf0: 2020 2020 2020 2020 7465 7374 286c 696e          test(lin
+0001bb00: 6573 2c20 6578 7065 6374 6564 2c20 7461  es, expected, ta
+0001bb10: 625f 7769 6474 683d 3429 0a0a 2020 2020  b_width=4)..    
+0001bb20: 2020 2020 2323 0a20 2020 2020 2020 2023      ##.        #
+0001bb30: 2320 7465 7374 2072 6169 7369 6e67 2066  # test raising f
+0001bb40: 6f72 2069 6c6c 6567 616c 206f 7574 6465  or illegal outde
+0001bb50: 6e74 730a 2020 2020 2020 2020 2323 0a0a  nts.        ##..
+0001bb60: 2020 2020 2020 2020 2320 7768 656e 2069          # when i
+0001bb70: 7427 7320 6265 7477 6565 6e20 7477 6f20  t's between two 
+0001bb80: 6578 6973 7469 6e67 2069 6e64 656e 7473  existing indents
+0001bb90: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+0001bba0: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+0001bbb0: 6c65 6674 206d 6172 6769 6e5c 6e22 0a20  left margin\n". 
+0001bbc0: 2020 2020 2020 2020 2020 2022 5c74 666f             "\tfo
+0001bbd0: 7572 5c6e 220a 2020 2020 2020 2020 2020  ur\n".          
+0001bbe0: 2020 2220 205c 7420 2020 2065 6967 6874    "  \t    eight
+0001bbf0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+0001bc00: 2220 2020 2020 2073 6978 3f21 5c6e 220a  "      six?!\n".
+0001bc10: 2020 2020 2020 2020 2020 2020 226c 6566              "lef
+0001bc20: 7420 6d61 7267 696e 2061 6761 696e 5c6e  t margin again\n
+0001bc30: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0001bc40: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0001bc50: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+0001bc60: 496e 6465 6e74 6174 696f 6e45 7272 6f72  IndentationError
+0001bc70: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+0001bc80: 6573 7428 6c69 6e65 732c 205b 5d2c 2074  est(lines, [], t
+0001bc90: 6162 5f77 6964 7468 3d34 290a 0a0a 2020  ab_width=4)...  
+0001bca0: 2020 2020 2020 2320 7768 656e 2069 7427        # when it'
+0001bcb0: 7320 6c65 7373 2074 6861 6e20 7468 6520  s less than the 
+0001bcc0: 6669 7273 7420 696e 6465 6e74 0a20 2020  first indent.   
+0001bcd0: 2020 2020 206c 696e 6573 203d 2028 0a20       lines = (. 
+0001bce0: 2020 2020 2020 2020 2020 2022 6c65 6674             "left
+0001bcf0: 206d 6172 6769 6e5c 6e22 0a20 2020 2020   margin\n".     
+0001bd00: 2020 2020 2020 2022 5c74 666f 7572 5c6e         "\tfour\n
+0001bd10: 220a 2020 2020 2020 2020 2020 2020 2220  ".            " 
+0001bd20: 205c 7420 2020 2065 6967 6874 5c6e 220a   \t    eight\n".
+0001bd30: 2020 2020 2020 2020 2020 2020 2220 2074              "  t
+0001bd40: 776f 3f21 5c6e 220a 2020 2020 2020 2020  wo?!\n".        
+0001bd50: 2020 2020 226c 6566 7420 6d61 7267 696e      "left margin
+0001bd60: 2061 6761 696e 5c6e 220a 2020 2020 2020   again\n".      
+0001bd70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001bd80: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+0001bd90: 7452 6169 7365 7328 496e 6465 6e74 6174  tRaises(Indentat
+0001bda0: 696f 6e45 7272 6f72 293a 0a20 2020 2020  ionError):.     
+0001bdb0: 2020 2020 2020 2074 6573 7428 6c69 6e65         test(line
+0001bdc0: 732c 205b 5d2c 2074 6162 5f77 6964 7468  s, [], tab_width
+0001bdd0: 3d34 290a 0a20 2020 2020 2020 2077 6974  =4)..        wit
+0001bde0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+0001bdf0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
+0001be00: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
+0001be10: 7428 2266 6972 7374 206c 696e 655c 6e20  t("first line\n 
+0001be20: 205c 7533 3030 3020 2073 6563 6f6e 6420   \u3000  second 
+0001be30: 6c69 6e65 5c6e 7468 6972 6420 6c69 6e65  line\nthird line
+0001be40: 5c6e 222c 205b 5d29 0a0a 2020 2020 6465  \n", [])..    de
+0001be50: 6620 7465 7374 5f6c 696e 6573 5f6d 6973  f test_lines_mis
+0001be60: 6328 7365 6c66 293a 0a20 2020 2020 2020  c(self):.       
+0001be70: 2023 2320 7265 7072 0a20 2020 2020 2020   ## repr.       
+0001be80: 206c 6920 3d20 6269 672e 4c69 6e65 496e   li = big.LineIn
+0001be90: 666f 2827 272c 2031 2c20 312c 2069 6e64  fo('', 1, 1, ind
+0001bea0: 656e 743d 3029 0a20 2020 2020 2020 2073  ent=0).        s
+0001beb0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001bec0: 7265 7072 286c 6929 2c20 224c 696e 6549  repr(li), "LineI
+0001bed0: 6e66 6f28 6c69 6e65 3d27 272c 206c 696e  nfo(line='', lin
+0001bee0: 655f 6e75 6d62 6572 3d31 2c20 636f 6c75  e_number=1, colu
+0001bef0: 6d6e 5f6e 756d 6265 723d 312c 2069 6e64  mn_number=1, ind
+0001bf00: 656e 743d 3029 2229 0a0a 2020 2020 2020  ent=0)")..      
+0001bf10: 2020 2323 2065 7272 6f72 2068 616e 646c    ## error handl
+0001bf20: 696e 670a 2020 2020 2020 2020 7769 7468  ing.        with
+0001bf30: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0001bf40: 6573 2854 7970 6545 7272 6f72 293a 0a20  es(TypeError):. 
+0001bf50: 2020 2020 2020 2020 2020 2062 6967 2e6c             big.l
+0001bf60: 696e 6573 2822 222c 206c 696e 655f 6e75  ines("", line_nu
+0001bf70: 6d62 6572 3d6d 6174 682e 7069 290a 2020  mber=math.pi).  
+0001bf80: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0001bf90: 6173 7365 7274 5261 6973 6573 2854 7970  assertRaises(Typ
+0001bfa0: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+0001bfb0: 2020 2020 2062 6967 2e6c 696e 6573 2822       big.lines("
+0001bfc0: 222c 2063 6f6c 756d 6e5f 6e75 6d62 6572  ", column_number
+0001bfd0: 3d6d 6174 682e 7069 290a 2020 2020 2020  =math.pi).      
+0001bfe0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0001bff0: 7274 5261 6973 6573 2854 7970 6545 7272  rtRaises(TypeErr
+0001c000: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0001c010: 2062 6967 2e6c 696e 6573 2822 222c 2074   big.lines("", t
+0001c020: 6162 5f77 6964 7468 3d6d 6174 682e 7069  ab_width=math.pi
+0001c030: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+0001c040: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+0001c050: 7328 5479 7065 4572 726f 7229 3a0a 2020  s(TypeError):.  
+0001c060: 2020 2020 2020 2020 2020 6269 672e 4c69            big.Li
+0001c070: 6e65 496e 666f 286d 6174 682e 7069 2c20  neInfo(math.pi, 
+0001c080: 312c 2031 290a 2020 2020 2020 2020 7769  1, 1).        wi
+0001c090: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0001c0a0: 6973 6573 2854 7970 6545 7272 6f72 293a  ises(TypeError):
+0001c0b0: 0a20 2020 2020 2020 2020 2020 2062 6967  .            big
+0001c0c0: 2e4c 696e 6549 6e66 6f28 2727 2c20 6d61  .LineInfo('', ma
+0001c0d0: 7468 2e70 692c 2031 290a 2020 2020 2020  th.pi, 1).      
+0001c0e0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0001c0f0: 7274 5261 6973 6573 2854 7970 6545 7272  rtRaises(TypeErr
+0001c100: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0001c110: 2062 6967 2e4c 696e 6549 6e66 6f28 2727   big.LineInfo(''
+0001c120: 2c20 312c 206d 6174 682e 7069 290a 0a20  , 1, math.pi).. 
+0001c130: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0001c140: 2e61 7373 6572 7452 6169 7365 7328 5661  .assertRaises(Va
+0001c150: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+0001c160: 2020 2020 2020 206c 6973 7428 6269 672e         list(big.
+0001c170: 6c69 6e65 735f 6669 6c74 6572 5f63 6f6d  lines_filter_com
+0001c180: 6d65 6e74 5f6c 696e 6573 2822 222c 205b  ment_lines("", [
+0001c190: 5d29 290a 2020 2020 2020 2020 7769 7468  ])).        with
+0001c1a0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0001c1b0: 6573 2854 7970 6545 7272 6f72 293a 0a20  es(TypeError):. 
+0001c1c0: 2020 2020 2020 2020 2020 206c 6973 7428             list(
+0001c1d0: 6269 672e 6c69 6e65 735f 6669 6c74 6572  big.lines_filter
+0001c1e0: 5f63 6f6d 6d65 6e74 5f6c 696e 6573 2822  _comment_lines("
+0001c1f0: 222c 206d 6174 682e 7069 2929 0a0a 2020  ", math.pi))..  
+0001c200: 2020 2020 2020 2323 2074 6573 7420 6b77        ## test kw
+0001c210: 6172 6773 0a20 2020 2020 2020 2069 203d  args.        i =
+0001c220: 2062 6967 2e6c 696e 6573 2827 272c 2071   big.lines('', q
+0001c230: 7561 726b 3d32 3229 0a20 2020 2020 2020  uark=22).       
+0001c240: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0001c250: 2868 6173 6174 7472 2869 2c20 2771 7561  (hasattr(i, 'qua
+0001c260: 726b 2729 290a 2020 2020 2020 2020 7365  rk')).        se
+0001c270: 6c66 2e61 7373 6572 7445 7175 616c 2867  lf.assertEqual(g
+0001c280: 6574 6174 7472 2869 2c20 2771 7561 726b  etattr(i, 'quark
+0001c290: 2729 2c20 3232 290a 0a20 2020 2020 2020  '), 22)..       
+0001c2a0: 2069 6e66 6f20 3d20 6269 672e 4c69 6e65   info = big.Line
+0001c2b0: 496e 666f 2827 272c 2031 2c20 312c 2071  Info('', 1, 1, q
+0001c2c0: 7561 726b 3d33 3529 0a20 2020 2020 2020  uark=35).       
+0001c2d0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0001c2e0: 2868 6173 6174 7472 2869 6e66 6f2c 2027  (hasattr(info, '
+0001c2f0: 7175 6172 6b27 2929 0a20 2020 2020 2020  quark')).       
+0001c300: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001c310: 6c28 6765 7461 7474 7228 696e 666f 2c20  l(getattr(info, 
+0001c320: 2771 7561 726b 2729 2c20 3335 290a 0a0a  'quark'), 35)...
+0001c330: 696d 706f 7274 2062 6967 7465 7374 6c69  import bigtestli
+0001c340: 620a 0a64 6566 2072 756e 5f74 6573 7473  b..def run_tests
+0001c350: 2829 3a0a 2020 2020 6269 6774 6573 746c  ():.    bigtestl
+0001c360: 6962 2e72 756e 286e 616d 653d 2262 6967  ib.run(name="big
+0001c370: 2e74 6578 7422 2c20 6d6f 6475 6c65 3d5f  .text", module=_
+0001c380: 5f6e 616d 655f 5f29 0a0a 6966 205f 5f6e  _name__)..if __n
+0001c390: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+0001c3a0: 5f5f 223a 2023 2070 7261 676d 613a 206e  __": # pragma: n
+0001c3b0: 6f20 636f 7665 720a 2020 2020 7275 6e5f  o cover.    run_
+0001c3c0: 7465 7374 7328 290a 2020 2020 6269 6774  tests().    bigt
+0001c3d0: 6573 746c 6962 2e66 696e 6973 6828 290a  estlib.finish().
```

### Comparing `big-0.8/test/test_time.py` & `big-0.8.1/test/test_time.py`

 * *Files identical despite different names*

### Comparing `big-0.8/PKG-INFO` & `big-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: big
-Version: 0.8
+Version: 0.8.1
 Summary: The big package is a grab-bag of cool code for use in your programs.
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -109,14 +109,16 @@
 
 [`big.time`](#bigtime)
 
 [`BoundInnerClass`](#boundinnerclasscls)
 
 [`CycleError`](#cycleerror)
 
+[`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+
 [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone)
 
 [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone)
 
 [`Event(scheduler, event, time, priority, sequence)`](#eventscheduler-event-time-priority-sequence)
 
 [`Event.cancel()`](#eventcancel)
@@ -189,14 +191,16 @@
 
 [`newlines`](#newlines)
 
 [`newlines_without_dos`](#newlines)
 
 [`normalize_whitespace(s, separators=None, replacement=None)`](#normalize_whitespaces-separatorsNone-replacementnone)
 
+[`parse_delimiters(s, delimiters=None)`](#parse_delimiterss-delimitersNone)
+
 [`parse_timestamp_3339Z(s, *, timezone=None)`](#parse_timestamp_3339zs--timezonenone)
 
 [`PushbackIterator(iterable=None)`](#pushbackiteratoriterablenone)
 
 [`PushbackIterator.next(default=None)`](#pushbackiteratornextdefaultnone)
 
 [`PushbackIterator.push(o)`](#pushbackiteratorpusho)
@@ -1054,14 +1058,28 @@
 These functions will check that all such arguments
 are of the same type.
 
 Subclasses of `str` and `bytes` will also work; anywhere you
 should pass in a `str`, you can also pass in a subclass of
 `str`, and likewise for `bytes`.
 
+#### `Delimiter(open, close, *, backslash=False, nested=True)`
+
+> Class representing a delimiter for
+> [`parse_delimiters(s, delimiters=None)`.](#parse_delimiterss-delimitersNone)
+>
+> `open` is the opening delimiter character, can be `str` or `bytes`, must be length 1.
+>
+> `close` is the closing delimiter character, must be the same type as `open`, and length 1.
+>
+> `backslash` is a boolean: when inside this delimiter, can you escape delimiters
+> with a backslash?  (You usually can inside single or double quotes.)
+>
+> `nested` is a boolean: must other delimiters nest in this delimiter?
+> (Delimiters don't usually need to be nested inside single and double quotes.)
 
 #### `gently_title(s, *, apostrophes=None, double_quotes=None)`
 
 > Uppercase the first character of every word in `s`.
 > Leave the other letters alone.  s should be `str` or `bytes`.
 >
 > (For the purposes of this algorithm, words are
@@ -1605,14 +1623,50 @@
 > a replacement string consisting of a single space character.
 >
 > Leading or trailing runs of separator characters will
 > be replaced with the replacement string, e.g.:
 >
 >     normalize_whitespace("   a    b   c") == " a b c"
 
+#### `parse_delimiters(s, delimiters=None)`
+
+> Parses a string containing nesting delimiters.
+> Raises an exception if mismatched delimiters are detected.
+>
+> `s` may be `str` or `bytes`.
+>
+> `delimiters` may be either `None` or an iterable containing
+> either
+> [`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+> objects or objects matching `s` (`str` or `bytes`).
+> Entries in the `delimiters` iterable which are `str` or `bytes`
+> should be exactly two characters long; these will be used
+> as the `open` and `close` arguments for a new `Delimiter` object.
+>
+> If `delimiters` is `None`, `parse_delimiters` uses a default
+> value matching these pairs of delimiters:
+>
+>     () [] {} "" ''
+>
+> The quote mark delimiters enable backslash quoting and disable nesting.
+>
+> Yields 3-tuples containing strings:
+>     (text, open, close)
+> where `text` is the text before the next opening or closing delimiter,
+> `open` is the trailing opening delimiter,
+> and `close` is the trailing closing delimiter.
+> At least one of these three strings will always be non-empty.
+> If `open` is non-empty, `close` will be empty, and vice-versa.
+> If `s` does not end with a closing delimiter, in the final tuple
+> yielded, both `open` and `close` will be empty strings.
+>
+> You can only specify a particular character as an opening delimiter
+> once, though you may reuse a particular character as a closing
+> delimiter multiple times.
+
 #### `re_partition(text, pattern, count=1, *, flags=0, reverse=False)`
 
 > Like `str.partition`, but `pattern` is matched as a regular expression.
 >
 > `text` can be a string or a bytes object.
 >
 > `pattern` can be a string, bytes, or `re.Pattern` object.
@@ -3300,14 +3354,21 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
+**0.8.1**
+
+* Added
+  [`parse_delimiters`](#parse_delimiterss-delimitersNone)
+  and
+  [`Delimiter(open, close, *, backslash=False, nested=True)`.](delimiteropen-close--backslash-nested)
+
 **0.8**
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
     for how it works.
```

