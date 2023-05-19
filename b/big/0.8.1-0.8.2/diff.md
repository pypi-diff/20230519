# Comparing `tmp/big-0.8.1.tar.gz` & `tmp/big-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "big-0.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `big-0.8.1.tar` & `big-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.8.1/.gitignore
--rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.8.1/LICENSE
--rw-r--r--   0        0        0   144602 2023-05-19 13:23:04.978639 big-0.8.1/README.md
--rw-r--r--   0        0        0     1242 2023-05-19 13:20:37.349392 big-0.8.1/big/__init__.py
--rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.8.1/big/all.py
--rw-r--r--   0        0        0     5705 2023-04-12 21:51:57.504191 big-0.8.1/big/boundinnerclass.py
--rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.8.1/big/builtin.py
--rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.8.1/big/file.py
--rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.8.1/big/graph.py
--rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.8.1/big/heap.py
--rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.8.1/big/itertools.py
--rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.8.1/big/scheduler.py
--rw-r--r--   0        0        0   103073 2023-05-19 13:20:16.529216 big-0.8.1/big/text.py
--rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.8.1/big/time.py
--rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.8.1/requirements.txt
--rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.8.1/resources/experiments/alice.in.wonderland.txt
--rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.8.1/resources/experiments/time_multisplit.py
--rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.8.1/resources/images/big.header.png
--rw-r--r--   0        0        0     2692 2023-04-12 21:51:57.504191 big-0.8.1/test/bigtestlib.py
--rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.8.1/test/grepfile
--rw-r--r--   0        0        0     1422 2023-04-12 21:51:57.504191 big-0.8.1/test/test_all.py
--rw-r--r--   0        0        0     5847 2023-04-12 21:51:57.504191 big-0.8.1/test/test_boundinnerclass.py
--rw-r--r--   0        0        0     6486 2023-04-12 21:51:57.504191 big-0.8.1/test/test_builtin.py
--rw-r--r--   0        0        0     8332 2023-04-12 21:51:57.504191 big-0.8.1/test/test_file.py
--rw-r--r--   0        0        0    12302 2023-04-12 21:51:57.504191 big-0.8.1/test/test_graph.py
--rw-r--r--   0        0        0     4978 2023-04-12 21:51:57.504191 big-0.8.1/test/test_heap.py
--rw-r--r--   0        0        0     3373 2023-04-12 21:51:57.504191 big-0.8.1/test/test_itertools.py
--rw-r--r--   0        0        0    11445 2023-04-12 21:51:57.504191 big-0.8.1/test/test_scheduler.py
--rw-r--r--   0        0        0   115680 2023-05-19 13:19:51.149002 big-0.8.1/test/test_text.py
--rw-r--r--   0        0        0     6069 2023-04-12 21:51:57.508190 big-0.8.1/test/test_time.py
--rw-r--r--   0        0        0   145207 1970-01-01 00:00:00.000000 big-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.8.2/LICENSE
+-rw-r--r--   0        0        0   144931 2023-05-19 14:23:46.881392 big-0.8.2/README.md
+-rw-r--r--   0        0        0     1242 2023-05-19 14:23:58.625491 big-0.8.2/big/__init__.py
+-rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.8.2/big/all.py
+-rw-r--r--   0        0        0     5705 2023-04-12 21:51:57.504191 big-0.8.2/big/boundinnerclass.py
+-rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.8.2/big/builtin.py
+-rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.8.2/big/file.py
+-rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.8.2/big/graph.py
+-rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.8.2/big/heap.py
+-rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.8.2/big/itertools.py
+-rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.8.2/big/scheduler.py
+-rw-r--r--   0        0        0   105102 2023-05-19 14:23:02.781020 big-0.8.2/big/text.py
+-rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.8.2/big/time.py
+-rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.8.2/requirements.txt
+-rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.8.2/resources/experiments/alice.in.wonderland.txt
+-rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.8.2/resources/experiments/time_multisplit.py
+-rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.8.2/resources/images/big.header.png
+-rw-r--r--   0        0        0     2692 2023-04-12 21:51:57.504191 big-0.8.2/test/bigtestlib.py
+-rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.8.2/test/grepfile
+-rw-r--r--   0        0        0     1422 2023-04-12 21:51:57.504191 big-0.8.2/test/test_all.py
+-rw-r--r--   0        0        0     5847 2023-04-12 21:51:57.504191 big-0.8.2/test/test_boundinnerclass.py
+-rw-r--r--   0        0        0     6486 2023-04-12 21:51:57.504191 big-0.8.2/test/test_builtin.py
+-rw-r--r--   0        0        0     8332 2023-04-12 21:51:57.504191 big-0.8.2/test/test_file.py
+-rw-r--r--   0        0        0    12302 2023-04-12 21:51:57.504191 big-0.8.2/test/test_graph.py
+-rw-r--r--   0        0        0     4978 2023-04-12 21:51:57.504191 big-0.8.2/test/test_heap.py
+-rw-r--r--   0        0        0     3373 2023-04-12 21:51:57.504191 big-0.8.2/test/test_itertools.py
+-rw-r--r--   0        0        0    11445 2023-04-12 21:51:57.504191 big-0.8.2/test/test_scheduler.py
+-rw-r--r--   0        0        0   115680 2023-05-19 13:19:51.149002 big-0.8.2/test/test_text.py
+-rw-r--r--   0        0        0     6069 2023-04-12 21:51:57.508190 big-0.8.2/test/test_time.py
+-rw-r--r--   0        0        0   145536 1970-01-01 00:00:00.000000 big-0.8.2/PKG-INFO
```

### Comparing `big-0.8.1/LICENSE` & `big-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `big-0.8.1/README.md` & `big-0.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,20 +93,20 @@
 
 [`big.time`](#bigtime)
 
 [`BoundInnerClass`](#boundinnerclasscls)
 
 [`CycleError`](#cycleerror)
 
-[`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
-
 [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone)
 
 [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone)
 
+[`Delimiter(open, close, *, backslash=False, nested=True)`](#delimiteropen-close--backslashfalse-nestedtrue)
+
 [`Event(scheduler, event, time, priority, sequence)`](#eventscheduler-event-time-priority-sequence)
 
 [`Event.cancel()`](#eventcancel)
 
 [`fgrep(path, text, *, encoding=None, enumerate=False, case_insensitive=False)`](#fgreppath-text--encodingnone-enumeratefalse-case_insensitivefalse)
 
 [`file_mtime(path)`](#file_mtimepath)
@@ -1012,15 +1012,15 @@
 All the functions in `big.text` will work with either
 `str` or `bytes` objects, except the three
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 functions.  When working with `bytes`,
 by default the functions will only work with ASCII
 characters.
 
-## Support for bytes and str
+#### Support for bytes and str
 
 The **big** text functions all support both `str` and `bytes`.
 The functions all automatically detect whether you passed in
 `str` or `bytes`  using an
 intentionally simple and predictable process, as follows:
 
 At the start of each function, it'll test its first "string"
@@ -1045,15 +1045,15 @@
 Subclasses of `str` and `bytes` will also work; anywhere you
 should pass in a `str`, you can also pass in a subclass of
 `str`, and likewise for `bytes`.
 
 #### `Delimiter(open, close, *, backslash=False, nested=True)`
 
 > Class representing a delimiter for
-> [`parse_delimiters(s, delimiters=None)`.](#parse_delimiterss-delimitersNone)
+> [`parse_delimiters`.](#parse_delimiterss-delimitersNone)
 >
 > `open` is the opening delimiter character, can be `str` or `bytes`, must be length 1.
 >
 > `close` is the closing delimiter character, must be the same type as `open`, and length 1.
 >
 > `backslash` is a boolean: when inside this delimiter, can you escape delimiters
 > with a backslash?  (You usually can inside single or double quotes.)
@@ -1616,29 +1616,31 @@
 > Parses a string containing nesting delimiters.
 > Raises an exception if mismatched delimiters are detected.
 >
 > `s` may be `str` or `bytes`.
 >
 > `delimiters` may be either `None` or an iterable containing
 > either
-> [`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+> [`Delimiter`](#delimiteropen-close--backslashfalse-nestedtrue)
 > objects or objects matching `s` (`str` or `bytes`).
 > Entries in the `delimiters` iterable which are `str` or `bytes`
 > should be exactly two characters long; these will be used
 > as the `open` and `close` arguments for a new `Delimiter` object.
 >
 > If `delimiters` is `None`, `parse_delimiters` uses a default
 > value matching these pairs of delimiters:
 >
 >     () [] {} "" ''
 >
 > The quote mark delimiters enable backslash quoting and disable nesting.
 >
 > Yields 3-tuples containing strings:
+>
 >     (text, open, close)
+>
 > where `text` is the text before the next opening or closing delimiter,
 > `open` is the trailing opening delimiter,
 > and `close` is the trailing closing delimiter.
 > At least one of these three strings will always be non-empty.
 > If `open` is non-empty, `close` will be empty, and vice-versa.
 > If `s` does not end with a closing delimiter, in the final tuple
 > yielded, both `open` and `close` will be empty strings.
@@ -3338,20 +3340,30 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
+**0.8.2**
+
+* Convert all iterator functions to use my new approach:
+  instead of checking arguments inside the iterator,
+  the function you call checks arguments, then has a
+  nested iterator function which it runs and returns the
+  result.  This means bad inputs raise their exceptions
+  at the call site where the iterator is constructed,
+  rather than when the first value is yielded by the iterator!
+
 **0.8.1**
 
 * Added
   [`parse_delimiters`](#parse_delimiterss-delimitersNone)
   and
-  [`Delimiter(open, close, *, backslash=False, nested=True)`.](delimiteropen-close--backslash-nested)
+  [`Delimiter`.](#delimiteropen-close--backslashfalse-nestedtrue)
 
 **0.8**
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
```

### Comparing `big-0.8.1/big/__init__.py` & `big-0.8.2/big/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
```

### Comparing `big-0.8.1/big/all.py` & `big-0.8.2/big/all.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/boundinnerclass.py` & `big-0.8.2/big/boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/builtin.py` & `big-0.8.2/big/builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/file.py` & `big-0.8.2/big/file.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/graph.py` & `big-0.8.2/big/graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/heap.py` & `big-0.8.2/big/heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/itertools.py` & `big-0.8.2/big/itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/scheduler.py` & `big-0.8.2/big/scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/big/text.py` & `big-0.8.2/big/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,241 +177,243 @@
     the flags you passed in.
 
     string should be the same type as pattern (or pattern.pattern).
     """
     if not isinstance_re_pattern(pattern):
         pattern = re.compile(pattern, flags=flags)
 
-    # matches are found by re.search *going forwards.*
-    # but what we need here is the *reverse* matches.
-    #
-    # consider this call:
-    #    re_rpartition('abcdefgh', '(abcdef|efg|ab|b|c|d)', count=4)
-    #
-    # re.finditer with that string and pattern yields one match:
-    #    'abcdef'
-    # but reverse searching, e.g. with
-    # regex.finditer(flags=regex.REVERSE), yields four matches:
-    #    'efg', 'd', 'c', 'ab'
-    #
-    # so what we do is: we ask re.finditer for all the forward
-    # matches.  then, for every match it found, we check every
-    # overlapping character to see if there's a different match
-    # there that we might prefer.  if we prefer one of those,
-    # we yield that--but we keep around the other matches,
-    # because one of those (or a truncated version of it) might
-    # also work.
-
-
-    # matches and overlapping_matches are lists of 3-tuples of:
-    #    (end_pos, -start_pos, match)
-    # if we sort the list, the last element will be the correct
-    # last match in "reverse" order.  see
-    #    https://en.wikipedia.org/wiki/Schwartzian_transform
-    #
-    # matches contains the list of matches we got directly from
-    # re.finditer(), reversed.  since this was found using re in
-    # "forward" order, we need to check every match in this list
-    # for potential overlapping matches.
-    matches = [(match.end(), -match.start(), match) for match in pattern.finditer(string)]
-    if not matches:
-        # print(f"no matches at all! exiting immediately.")
-        return
-
-    # Does this pattern match zero-length strings?
-    zero_length_match = pattern.match(string, 0, 0)
-    if zero_length_match:
-        # This pattern matches zero-length strings.
-        # Since the rules are a little different for
-        # zero-length strings when in reverse mode,
-        # we need to doctor the match results a little.
-
-        # These seem to be the rules:
+    def reversed_re_finditer(pattern, string):
+        # matches are found by re.search *going forwards.*
+        # but what we need here is the *reverse* matches.
         #
-        # In forwards mode, we consider two matches to overlap
-        # if they start at the same position, or if they have
-        # any characters in common.  There's an implicit
-        # zero-length string at the beginning and end of every
-        # string, so if the pattern matches against a zero-length
-        # string at the start or end, and there isn't another
-        # (longer) match that starts at that position, we'll
-        # yield these matches too.  Since only a zero-length
-        # match can start at position len(string), we'll always
-        # yield a zero-length match starting and ending at
-        # position length(string) if the pattern matches there.
+        # consider this call:
+        #    re_rpartition('abcdefgh', '(abcdef|efg|ab|b|c|d)', count=4)
         #
-        # In reverse mode, we consider two matches to overlap
-        # if they end at the same position, or if they have any
-        # characters in common with any other match.  There's an
-        # implicit zero-length string at the beginning and end of
-        # every string, so if the pattern matches a zero-length
-        # string at the start or end, and there isn't another
-        # (longer) match that ends at that position, we'll yield
-        # these matches too.  Since only a zero-length match can
-        # end at position 0, we'll always yield a zero-length
-        # match starting and ending at position 0 if the pattern
-        # matches there.
-
-        # We need to ensure that, for every non-zero-length match,
-        # if the pattern matches a zero-length string starting at
-        # the same position, we have that zero-length match in
-        # matches too.
+        # re.finditer with that string and pattern yields one match:
+        #    'abcdef'
+        # but reverse searching, e.g. with
+        # regex.finditer(flags=regex.REVERSE), yields four matches:
+        #    'efg', 'd', 'c', 'ab'
         #
-        # So specifically we're going to do this:
-        #
-        # for every match m in matches:
-        #   if m has nonzero length,
-        #     and the pattern matches a zero-length string
-        #       starting at m,
-        #     ensure that the zero-length match is also in matches.
-        #   elif m has zero length,
-        #     if we've already ensured that a zero-length
-        #     match starting at m.start() is in matches,
-        #     discard m.
-
-        zeroes = set()
-        new_matches = []
-        append = new_matches.append
-        last_start = -1
-        for t in matches:
-            match = t[2]
-            start, end = match.span()
-
-            if start not in zeroes:
-                if (start == end):
-                    append(t)
-                    zeroes.add(start)
-                    continue
+        # so what we do is: we ask re.finditer for all the forward
+        # matches.  then, for every match it found, we check every
+        # overlapping character to see if there's a different match
+        # there that we might prefer.  if we prefer one of those,
+        # we yield that--but we keep around the other matches,
+        # because one of those (or a truncated version of it) might
+        # also work.
 
-                zero_match = pattern.match(string, start, start)
-                if zero_match:
-                    t_zero_length = (start, -start, zero_match)
-                    append(t_zero_length)
-                zeroes.add(start)
-            append(t)
-        # del zeroes
-        matches = new_matches
-
-    matches.sort()
-
-    # overlapping_matches is a list of the possibly-viable
-    # overlapping matches we found from checking a match
-    # we got from "matches".
-    overlapping_matches = []
 
-    result = []
-    match = None
+        # matches and overlapping_matches are lists of 3-tuples of:
+        #    (end_pos, -start_pos, match)
+        # if we sort the list, the last element will be the correct
+        # last match in "reverse" order.  see
+        #    https://en.wikipedia.org/wiki/Schwartzian_transform
+        #
+        # matches contains the list of matches we got directly from
+        # re.finditer(), reversed.  since this was found using re in
+        # "forward" order, we need to check every match in this list
+        # for potential overlapping matches.
+        matches = [(match.end(), -match.start(), match) for match in pattern.finditer(string)]
+        if not matches:
+            # print(f"no matches at all! exiting immediately.")
+            return
 
-    # We truncate each match at the start
-    # of the previously yielded match.
-    #
-    # The initial value allows the initial match
-    # to extend all the way to the end of the string.
-    previous_match_start = len(string)
-
-    # cache some method lookups
-    pattern_match = pattern.match
-    append = overlapping_matches.append
-
-    while True:
-        if overlapping_matches:
-            # overlapping_matches contains the overlapping
-            # matches found *last* time around, before we
-            # yielded the most recent match.
-            #
-            # The thing is, some of these matches might overlap that match.
-            # But we only yield *non*-overlapping matches.  So we need to
-            # filter the matches in overlapping_matches accordingly.
-
-            truncated_matches = []
-            # (overlapping_matches will be set to truncated_matches in a few lines)
-            append = truncated_matches.append
-
-            for t in overlapping_matches:
-                end, negated_start, match = t
-                start = -negated_start
-                if start > previous_match_start:
-                    # This match starts *after* the previous match started.
-                    # All matches starting at this position are no longer
-                    # viable.  Throw away the match.
-                    continue
-                if end <= previous_match_start:
-                    # This match ends *before* the previous match started.
-                    # In other words, this match is still 100% viable.
-                    # Keep it, we don't need to change it at all.
-                    append(t)
-                    continue
+        # Does this pattern match zero-length strings?
+        zero_length_match = pattern.match(string, 0, 0)
+        if zero_length_match:
+            # This pattern matches zero-length strings.
+            # Since the rules are a little different for
+            # zero-length strings when in reverse mode,
+            # we need to doctor the match results a little.
 
-                # This match starts before the previous match started,
-                # but ends after the previous match start.
-                # In other words, it overlaps the previous match.
-                #
-                # So this match is itself no longer viable.  But!
-                # There might be a *different* match starting at this
-                # position in the string.  So we do a fresh re.match here,
-                # stopping at the start of the previously yielded match.
-                # (That's the third parameter, "endpos".)
-
-                match = pattern_match(string, start, previous_match_start)
-                if match:
-                    append((match.end(), -start, match))
-
-            overlapping_matches = truncated_matches
-
-        if (not overlapping_matches) and matches:
-            # We don't currently have any pre-screened
-            # overlapping matches we can use.
+            # These seem to be the rules:
+            #
+            # In forwards mode, we consider two matches to overlap
+            # if they start at the same position, or if they have
+            # any characters in common.  There's an implicit
+            # zero-length string at the beginning and end of every
+            # string, so if the pattern matches against a zero-length
+            # string at the start or end, and there isn't another
+            # (longer) match that starts at that position, we'll
+            # yield these matches too.  Since only a zero-length
+            # match can start at position len(string), we'll always
+            # yield a zero-length match starting and ending at
+            # position length(string) if the pattern matches there.
             #
-            # But we *do* have a match (or matches) found in forwards mode.
-            # Grab the next one that's still viable.
+            # In reverse mode, we consider two matches to overlap
+            # if they end at the same position, or if they have any
+            # characters in common with any other match.  There's an
+            # implicit zero-length string at the beginning and end of
+            # every string, so if the pattern matches a zero-length
+            # string at the start or end, and there isn't another
+            # (longer) match that ends at that position, we'll yield
+            # these matches too.  Since only a zero-length match can
+            # end at position 0, we'll always yield a zero-length
+            # match starting and ending at position 0 if the pattern
+            # matches there.
+
+            # We need to ensure that, for every non-zero-length match,
+            # if the pattern matches a zero-length string starting at
+            # the same position, we have that zero-length match in
+            # matches too.
+            #
+            # So specifically we're going to do this:
+            #
+            # for every match m in matches:
+            #   if m has nonzero length,
+            #     and the pattern matches a zero-length string
+            #       starting at m,
+            #     ensure that the zero-length match is also in matches.
+            #   elif m has zero length,
+            #     if we've already ensured that a zero-length
+            #     match starting at m.start() is in matches,
+            #     discard m.
+
+            zeroes = set()
+            new_matches = []
+            append = new_matches.append
+            last_start = -1
+            for t in matches:
+                match = t[2]
+                start, end = match.span()
+
+                if start not in zeroes:
+                    if (start == end):
+                        append(t)
+                        zeroes.add(start)
+                        continue
+
+                    zero_match = pattern.match(string, start, start)
+                    if zero_match:
+                        t_zero_length = (start, -start, zero_match)
+                        append(t_zero_length)
+                    zeroes.add(start)
+                append(t)
+            # del zeroes
+            matches = new_matches
+
+        matches.sort()
+
+        # overlapping_matches is a list of the possibly-viable
+        # overlapping matches we found from checking a match
+        # we got from "matches".
+        overlapping_matches = []
 
-            scan_for_overlapping_matches = False
-            while matches:
-                t = matches.pop()
-                end, negated_start, match = t
-                start = -negated_start
-                if end <= previous_match_start:
-                    assert start <= previous_match_start
-                    append(t)
-                    start += 1
-                    scan_for_overlapping_matches = True
-                    break
+        result = []
+        match = None
 
-            if scan_for_overlapping_matches:
-                # We scan every** position inside the match for an
-                # overlapping match.  All the matches we find go in
-                # overlapping_matches, then we sort it and yield
-                # the last one.
-                #
-                # ** We don't actually need to check the *first* position,
-                #    "start", because we already know what we'll find:
-                #    the match that we got from re.finditer() and
-                #    scanned for overlaps.
+        # We truncate each match at the start
+        # of the previously yielded match.
+        #
+        # The initial value allows the initial match
+        # to extend all the way to the end of the string.
+        previous_match_start = len(string)
+
+        # cache some method lookups
+        pattern_match = pattern.match
+        append = overlapping_matches.append
+
+        while True:
+            if overlapping_matches:
+                # overlapping_matches contains the overlapping
+                # matches found *last* time around, before we
+                # yielded the most recent match.
                 #
-                # As mentioned, the match we got from finditer
-                # is viable here, so add it to the list.
+                # The thing is, some of these matches might overlap that match.
+                # But we only yield *non*-overlapping matches.  So we need to
+                # filter the matches in overlapping_matches accordingly.
+
+                truncated_matches = []
+                # (overlapping_matches will be set to truncated_matches in a few lines)
+                append = truncated_matches.append
+
+                for t in overlapping_matches:
+                    end, negated_start, match = t
+                    start = -negated_start
+                    if start > previous_match_start:
+                        # This match starts *after* the previous match started.
+                        # All matches starting at this position are no longer
+                        # viable.  Throw away the match.
+                        continue
+                    if end <= previous_match_start:
+                        # This match ends *before* the previous match started.
+                        # In other words, this match is still 100% viable.
+                        # Keep it, we don't need to change it at all.
+                        append(t)
+                        continue
+
+                    # This match starts before the previous match started,
+                    # but ends after the previous match start.
+                    # In other words, it overlaps the previous match.
+                    #
+                    # So this match is itself no longer viable.  But!
+                    # There might be a *different* match starting at this
+                    # position in the string.  So we do a fresh re.match here,
+                    # stopping at the start of the previously yielded match.
+                    # (That's the third parameter, "endpos".)
 
-                end = min(end, previous_match_start)
-                for pos in range(start, end):
-                    match = pattern_match(string, pos, previous_match_start)
+                    match = pattern_match(string, start, previous_match_start)
                     if match:
-                        # print(f"  found {match=}")
-                        append((match.end(), -pos, match))
+                        append((match.end(), -start, match))
 
-        if not overlapping_matches:
-            # matches and overlapping matches are both empty.
-            # We've exhausted the matches.  Stop iterating.
-            return
+                overlapping_matches = truncated_matches
+
+            if (not overlapping_matches) and matches:
+                # We don't currently have any pre-screened
+                # overlapping matches we can use.
+                #
+                # But we *do* have a match (or matches) found in forwards mode.
+                # Grab the next one that's still viable.
 
-        # overlapping_matches is now guaranteed current and non-empty.
-        # We sort it so the rightmost match is last, and yield that.
-        overlapping_matches.sort()
-        match = overlapping_matches.pop()[2]
-        previous_match_start = match.start()
-        yield match
+                scan_for_overlapping_matches = False
+                while matches:
+                    t = matches.pop()
+                    end, negated_start, match = t
+                    start = -negated_start
+                    if end <= previous_match_start:
+                        assert start <= previous_match_start
+                        append(t)
+                        start += 1
+                        scan_for_overlapping_matches = True
+                        break
+
+                if scan_for_overlapping_matches:
+                    # We scan every** position inside the match for an
+                    # overlapping match.  All the matches we find go in
+                    # overlapping_matches, then we sort it and yield
+                    # the last one.
+                    #
+                    # ** We don't actually need to check the *first* position,
+                    #    "start", because we already know what we'll find:
+                    #    the match that we got from re.finditer() and
+                    #    scanned for overlaps.
+                    #
+                    # As mentioned, the match we got from finditer
+                    # is viable here, so add it to the list.
+
+                    end = min(end, previous_match_start)
+                    for pos in range(start, end):
+                        match = pattern_match(string, pos, previous_match_start)
+                        if match:
+                            # print(f"  found {match=}")
+                            append((match.end(), -pos, match))
+
+            if not overlapping_matches:
+                # matches and overlapping matches are both empty.
+                # We've exhausted the matches.  Stop iterating.
+                return
+
+            # overlapping_matches is now guaranteed current and non-empty.
+            # We sort it so the rightmost match is last, and yield that.
+            overlapping_matches.sort()
+            match = overlapping_matches.pop()[2]
+            previous_match_start = match.start()
+            yield match
+    return reversed_re_finditer(pattern, string)
 
 
 @_export
 def re_rpartition(s, pattern, count=1, *, flags=0):
     """
     Like str.rpartition, but pattern is matched as a regular expression.
 
@@ -998,122 +1000,125 @@
             right = strip != LEFT
         s = multistrip(s, separators, left=left, right=right)
         if not s:
             # oops! all separators!
             # this will make us exit early, just a few lines down from here.
             maxsplit = 0
 
-    if maxsplit == None:
-        maxsplit = -1
-    elif maxsplit == 0:
-        if keep == ALTERNATING:
-            yield s
-        elif keep == AS_PAIRS:
-            yield (s, empty)
-        else:
-            yield s
-        return
+    def multisplit(s, separators, keep, maxsplit, reverse, separate, strip):
+        if maxsplit == None:
+            maxsplit = -1
+        elif maxsplit == 0:
+            if keep == ALTERNATING:
+                yield s
+            elif keep == AS_PAIRS:
+                yield (s, empty)
+            else:
+                yield s
+            return
 
-    # convert maxsplit for use with re.split.
-    #
-    # re.split interprets maxsplit slightly differently:
-    #   its maxsplit==0 means "allow all splits".
-    #   its maxsplit==1 means "only allow one split".
-    #
-    # (re.split doesn't have a way to express
-    #  "don't split" with its maxsplit parameter,
-    #  which is why we handled it already.)
-    re_split_maxsplit = 0 if maxsplit == -1 else maxsplit
-
-    if reverse:
-        # if reverse is true, when separators overlap,
-        # we need to prefer the rightmost one rather than
-        # the leftmost one.  how do we do *that*?
-        # Eric Smith had the brainstorm: reverse the string
-        # and the separators, split, and reverse the output
-        # and the strings in the output.
-        s = _multisplit_reversed(s, 's')
-        separators = tuple(separators)
-        s2 = _reversed_builtin_separators.get(separators, None)
-        if s2 != None:
-            separators = s2
-        else:
-            separators = _multisplit_reversed(separators, 'separators')
+        # convert maxsplit for use with re.split.
+        #
+        # re.split interprets maxsplit slightly differently:
+        #   its maxsplit==0 means "allow all splits".
+        #   its maxsplit==1 means "only allow one split".
+        #
+        # (re.split doesn't have a way to express
+        #  "don't split" with its maxsplit parameter,
+        #  which is why we handled it already.)
+        re_split_maxsplit = 0 if maxsplit == -1 else maxsplit
 
-    pattern = _separators_to_re(separators, is_bytes, keep=separators_to_re_keep, separate=separate)
-    # print("PATTERN", pattern, f"{separators_to_re_keep=} {separate=}")
+        if reverse:
+            # if reverse is true, when separators overlap,
+            # we need to prefer the rightmost one rather than
+            # the leftmost one.  how do we do *that*?
+            # Eric Smith had the brainstorm: reverse the string
+            # and the separators, split, and reverse the output
+            # and the strings in the output.
+            s = _multisplit_reversed(s, 's')
+            separators = tuple(separators)
+            s2 = _reversed_builtin_separators.get(separators, None)
+            if s2 != None:
+                separators = s2
+            else:
+                separators = _multisplit_reversed(separators, 'separators')
 
-    l = re.split(pattern, s, re_split_maxsplit)
-    assert l
-    # print("S", repr(s), "L", l, f"{re_split_maxsplit=}")
-
-    if strip == PROGRESSIVE:
-        # l alternates nonsep and sep strings.
-        # it's always an odd length, starting and ending with nonsep.
-        length = len(l)
-        assert length & 1
-
-        desired_length = 1 + (2*maxsplit)
-
-        # dang! this is complicated!
-        # maxsplit has to extend *past* the last nonsep
-        # for us to strip on the far side.
-        #  ' a b c   '.split(None, maxsplit=2) => ['a', 'b', 'c   ']
-        #  ' a b c   '.split(None, maxsplit=3) => ['a', 'b', 'c']
-        for i in range(length - 1, 0, -2):
-            nonsep = l[i]
-            if nonsep:
-                last_non_empty_nonsep = i
-                break
-        else:
-            last_non_empty_nonsep = 0
+        pattern = _separators_to_re(separators, is_bytes, keep=separators_to_re_keep, separate=separate)
+        # print("PATTERN", pattern, f"{separators_to_re_keep=} {separate=}")
 
-        if desired_length > (last_non_empty_nonsep + 2):
-            # strip!
-            l = l[:last_non_empty_nonsep + 1]
-            desired_length = length = last_non_empty_nonsep
+        l = re.split(pattern, s, re_split_maxsplit)
+        assert l
+        # print("S", repr(s), "L", l, f"{re_split_maxsplit=}")
+
+        if strip == PROGRESSIVE:
+            # l alternates nonsep and sep strings.
+            # it's always an odd length, starting and ending with nonsep.
+            length = len(l)
+            assert length & 1
+
+            desired_length = 1 + (2*maxsplit)
+
+            # dang! this is complicated!
+            # maxsplit has to extend *past* the last nonsep
+            # for us to strip on the far side.
+            #  ' a b c   '.split(None, maxsplit=2) => ['a', 'b', 'c   ']
+            #  ' a b c   '.split(None, maxsplit=3) => ['a', 'b', 'c']
+            for i in range(length - 1, 0, -2):
+                nonsep = l[i]
+                if nonsep:
+                    last_non_empty_nonsep = i
+                    break
+            else:
+                last_non_empty_nonsep = 0
+
+            if desired_length > (last_non_empty_nonsep + 2):
+                # strip!
+                l = l[:last_non_empty_nonsep + 1]
+                desired_length = length = last_non_empty_nonsep
+
+            if not keep:
+                for i in range(len(l) - 2, 0, -2):
+                    del l[i]
+
+        if reverse:
+            l = _multisplit_reversed(l, 'l')
+            l.reverse()
 
         if not keep:
-            for i in range(len(l) - 2, 0, -2):
-                del l[i]
+            l.reverse()
+            while l:
+                yield l.pop()
+            return
 
-    if reverse:
-        l = _multisplit_reversed(l, 'l')
-        l.reverse()
+        # from here on out, we're 'keep'-ing the separator strings.
+        # (we're returning the separator strings in one form or another.)
 
-    if not keep:
-        l.reverse()
-        while l:
-            yield l.pop()
-        return
+        if keep == ALTERNATING:
+            l.reverse()
+            while l:
+                yield l.pop()
+            return
 
-    # from here on out, we're 'keep'-ing the separator strings.
-    # (we're returning the separator strings in one form or another.)
+        if (len(l) % 2) == 1:
+            l.append(empty)
 
-    if keep == ALTERNATING:
+        previous = None
         l.reverse()
         while l:
-            yield l.pop()
-        return
+            o = l.pop()
+            if previous is None:
+                previous = o
+                continue
+            if keep == AS_PAIRS:
+                yield (previous, o)
+            else:
+                yield previous + o
+            previous = None
 
-    if (len(l) % 2) == 1:
-        l.append(empty)
-
-    previous = None
-    l.reverse()
-    while l:
-        o = l.pop()
-        if previous is None:
-            previous = o
-            continue
-        if keep == AS_PAIRS:
-            yield (previous, o)
-        else:
-            yield previous + o
-        previous = None
+    return multisplit(s, separators, keep, maxsplit, reverse, separate, strip)
 
 
 @_export
 def multipartition(s, separators, count=1, *, reverse=False, separate=True):
     """
     Like str.partition, but supports partitioning based on multiple separator
     strings, and can partition more than once.
@@ -1607,16 +1612,14 @@
 
     # flush the remainder of the string we were building,
     # in whatever condition it's in.
     if text:
         yield in_quote, empty_join(text)
 
 
-
-
 @_export
 class Delimiter:
     """
     Class representing a delimiter for parse_delimiters.
 
     open is the opening delimiter character, can be str or bytes, must be length 1.
     close is the closing delimiter character, must be the same type as open, and length 1.
@@ -1634,15 +1637,15 @@
             raise TypeError(f"open={open!r} and close={close!r}, they must be the same type, either str or bytes")
 
         self.open = open
         self.close = close
         self.backslash = backslash
         self.nested = nested
 
-    def __repr__(self):
+    def __repr__(self): # pragma: no cover
         return f"Delimiter(open={self.open!r}, close={self.close!r}, backslash={self.backslash}, nested={self.nested})"
 
 delimiter_parentheses = "()"
 _export_name('delimiter_parentheses')
 
 delimiter_square_brackets = "[]"
 _export_name('delimiter_square_brackets')
@@ -2021,19 +2024,22 @@
         comment_separators_is_bytes = True
     else:
         comment_separators_is_bytes = isinstance(comment_separators[0], bytes)
     comment_separators = tuple(comment_separators)
 
     comment_pattern = _separators_to_re(comment_separators, comment_separators_is_bytes, separate=False, keep=False)
     comment_re = re.compile(comment_pattern)
-    for info, line in li:
-        s = line.lstrip()
-        if comment_re.match(s):
-            continue
-        yield (info, line)
+
+    def lines_filter_comment_lines(li, comment_re):
+        for info, line in li:
+            s = line.lstrip()
+            if comment_re.match(s):
+                continue
+            yield (info, line)
+    return lines_filter_comment_lines(li, comment_re)
 
 
 @_export
 def lines_containing(li, s, *, invert=False):
     """
     A lines modifier function.  Only yields lines
     that contain s.  (Filters out lines that
@@ -2071,22 +2077,28 @@
 
     (In older versions of Python, re.Pattern was a private type called
     re._pattern_type.)
     """
     if not isinstance_re_pattern(pattern):
         pattern = re.compile(pattern, flags=flags)
     search = pattern.search
+
     if invert:
+        def lines_grep(li, search):
+            for t in li:
+                if not search(t[1]):
+                    yield t
+            return
+        return lines_grep(li, search)
+
+    def lines_grep(li, search):
         for t in li:
-            if not search(t[1]):
+            if search(t[1]):
                 yield t
-        return
-    for t in li:
-        if search(t[1]):
-            yield t
+    return lines_grep(li, search)
 
 @_export
 def lines_sort(li, *, reverse=False):
     """
     A lines modifier function.  Sorts all
     input lines before yielding them.
 
@@ -2156,43 +2168,47 @@
     else:
         empty = ''
     empty_join = empty.join
 
     comment_pattern = __separators_to_re(comment_separators, separators_is_bytes=comment_separators_is_bytes, separate=True, keep=True)
     re_comment = re.compile(comment_pattern)
     split = re_comment.split
-    for info, line in li:
-        if quotes:
-            i = split_quoted_strings(line, quotes, backslash=backslash, triple_quotes=triple_quotes)
-        else:
-            i = ((False, line),)
-        segments = []
-        append = segments.append
-        comment = []
-        for is_quoted, segment in i:
-            if comment:
-                comment.append(segment)
-                continue
-            if is_quoted:
-                append(segment)
-                continue
-            fields = split(segment, maxsplit=1)
-            leading = fields[0]
-            if len(fields) == 1:
+
+
+    def lines_strip_comments(li, split, quotes, backslash, rstrip, triple_quotes):
+        for info, line in li:
+            if quotes:
+                i = split_quoted_strings(line, quotes, backslash=backslash, triple_quotes=triple_quotes)
+            else:
+                i = ((False, line),)
+            segments = []
+            append = segments.append
+            comment = []
+            for is_quoted, segment in i:
+                if comment:
+                    comment.append(segment)
+                    continue
+                if is_quoted:
+                    append(segment)
+                    continue
+                fields = split(segment, maxsplit=1)
+                leading = fields[0]
+                if len(fields) == 1:
+                    append(leading)
+                    continue
+                # found a comment marker in an unquoted segment!
+                if rstrip:
+                    leading = leading.rstrip()
                 append(leading)
-                continue
-            # found a comment marker in an unquoted segment!
-            if rstrip:
-                leading = leading.rstrip()
-            append(leading)
-            comment = fields[1:]
+                comment = fields[1:]
 
-        info.comment = empty_join(comment)
-        line = empty_join(segments)
-        yield (info, line)
+            info.comment = empty_join(comment)
+            line = empty_join(segments)
+            yield (info, line)
+    return lines_strip_comments(li, split, quotes, backslash, rstrip, triple_quotes)
 
 @_export
 def lines_convert_tabs_to_spaces(li):
     """
     A lines modifier function.  Converts tabs to spaces for the lines
     of a "lines iterator", using the tab_width passed in to lines.
```

### Comparing `big-0.8.1/big/time.py` & `big-0.8.2/big/time.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/pyproject.toml` & `big-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `big-0.8.1/resources/experiments/alice.in.wonderland.txt` & `big-0.8.2/resources/experiments/alice.in.wonderland.txt`

 * *Files identical despite different names*

### Comparing `big-0.8.1/resources/experiments/time_multisplit.py` & `big-0.8.2/resources/experiments/time_multisplit.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/resources/images/big.header.png` & `big-0.8.2/resources/images/big.header.png`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/bigtestlib.py` & `big-0.8.2/test/bigtestlib.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_all.py` & `big-0.8.2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_boundinnerclass.py` & `big-0.8.2/test/test_boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_builtin.py` & `big-0.8.2/test/test_builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_file.py` & `big-0.8.2/test/test_file.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_graph.py` & `big-0.8.2/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_heap.py` & `big-0.8.2/test/test_heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_itertools.py` & `big-0.8.2/test/test_itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_scheduler.py` & `big-0.8.2/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_text.py` & `big-0.8.2/test/test_text.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/test/test_time.py` & `big-0.8.2/test/test_time.py`

 * *Files identical despite different names*

### Comparing `big-0.8.1/PKG-INFO` & `big-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: big
-Version: 0.8.1
+Version: 0.8.2
 Summary: The big package is a grab-bag of cool code for use in your programs.
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -109,20 +109,20 @@
 
 [`big.time`](#bigtime)
 
 [`BoundInnerClass`](#boundinnerclasscls)
 
 [`CycleError`](#cycleerror)
 
-[`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
-
 [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone)
 
 [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone)
 
+[`Delimiter(open, close, *, backslash=False, nested=True)`](#delimiteropen-close--backslashfalse-nestedtrue)
+
 [`Event(scheduler, event, time, priority, sequence)`](#eventscheduler-event-time-priority-sequence)
 
 [`Event.cancel()`](#eventcancel)
 
 [`fgrep(path, text, *, encoding=None, enumerate=False, case_insensitive=False)`](#fgreppath-text--encodingnone-enumeratefalse-case_insensitivefalse)
 
 [`file_mtime(path)`](#file_mtimepath)
@@ -1028,15 +1028,15 @@
 All the functions in `big.text` will work with either
 `str` or `bytes` objects, except the three
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 functions.  When working with `bytes`,
 by default the functions will only work with ASCII
 characters.
 
-## Support for bytes and str
+#### Support for bytes and str
 
 The **big** text functions all support both `str` and `bytes`.
 The functions all automatically detect whether you passed in
 `str` or `bytes`  using an
 intentionally simple and predictable process, as follows:
 
 At the start of each function, it'll test its first "string"
@@ -1061,15 +1061,15 @@
 Subclasses of `str` and `bytes` will also work; anywhere you
 should pass in a `str`, you can also pass in a subclass of
 `str`, and likewise for `bytes`.
 
 #### `Delimiter(open, close, *, backslash=False, nested=True)`
 
 > Class representing a delimiter for
-> [`parse_delimiters(s, delimiters=None)`.](#parse_delimiterss-delimitersNone)
+> [`parse_delimiters`.](#parse_delimiterss-delimitersNone)
 >
 > `open` is the opening delimiter character, can be `str` or `bytes`, must be length 1.
 >
 > `close` is the closing delimiter character, must be the same type as `open`, and length 1.
 >
 > `backslash` is a boolean: when inside this delimiter, can you escape delimiters
 > with a backslash?  (You usually can inside single or double quotes.)
@@ -1632,29 +1632,31 @@
 > Parses a string containing nesting delimiters.
 > Raises an exception if mismatched delimiters are detected.
 >
 > `s` may be `str` or `bytes`.
 >
 > `delimiters` may be either `None` or an iterable containing
 > either
-> [`Delimiter(open, close, *, backslash=False, nested=True)`](delimiteropen-close--backslash-nested)
+> [`Delimiter`](#delimiteropen-close--backslashfalse-nestedtrue)
 > objects or objects matching `s` (`str` or `bytes`).
 > Entries in the `delimiters` iterable which are `str` or `bytes`
 > should be exactly two characters long; these will be used
 > as the `open` and `close` arguments for a new `Delimiter` object.
 >
 > If `delimiters` is `None`, `parse_delimiters` uses a default
 > value matching these pairs of delimiters:
 >
 >     () [] {} "" ''
 >
 > The quote mark delimiters enable backslash quoting and disable nesting.
 >
 > Yields 3-tuples containing strings:
+>
 >     (text, open, close)
+>
 > where `text` is the text before the next opening or closing delimiter,
 > `open` is the trailing opening delimiter,
 > and `close` is the trailing closing delimiter.
 > At least one of these three strings will always be non-empty.
 > If `open` is non-empty, `close` will be empty, and vice-versa.
 > If `s` does not end with a closing delimiter, in the final tuple
 > yielded, both `open` and `close` will be empty strings.
@@ -3354,20 +3356,30 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
+**0.8.2**
+
+* Convert all iterator functions to use my new approach:
+  instead of checking arguments inside the iterator,
+  the function you call checks arguments, then has a
+  nested iterator function which it runs and returns the
+  result.  This means bad inputs raise their exceptions
+  at the call site where the iterator is constructed,
+  rather than when the first value is yielded by the iterator!
+
 **0.8.1**
 
 * Added
   [`parse_delimiters`](#parse_delimiterss-delimitersNone)
   and
-  [`Delimiter(open, close, *, backslash=False, nested=True)`.](delimiteropen-close--backslash-nested)
+  [`Delimiter`.](#delimiteropen-close--backslashfalse-nestedtrue)
 
 **0.8**
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
```

