# Comparing `tmp/mwxlib-0.83.4-py3-none-any.whl.zip` & `tmp/mwxlib-0.83.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161800 bytes, number of entries: 22
+Zip file size: 161826 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73243 b- defN 23-May-17 15:10 mwx/framework.py
+-rw-rw-rw-  2.0 fat    73366 b- defN 23-May-18 23:31 mwx/framework.py
 -rw-rw-rw-  2.0 fat    69534 b- defN 23-May-17 15:10 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138127 b- defN 23-May-17 04:56 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat   137969 b- defN 23-May-18 23:32 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37351 b- defN 23-May-16 17:41 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/RECORD
-22 files, 614093 bytes uncompressed, 159298 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-18 23:35 mwxlib-0.83.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-18 23:35 mwxlib-0.83.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 23:35 mwxlib-0.83.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-18 23:35 mwxlib-0.83.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-18 23:35 mwxlib-0.83.5.dist-info/RECORD
+22 files, 614058 bytes uncompressed, 159324 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.83.4.dist-info/LICENSE
+Filename: mwxlib-0.83.5.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.83.4.dist-info/METADATA
+Filename: mwxlib-0.83.5.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.83.4.dist-info/WHEEL
+Filename: mwxlib-0.83.5.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.83.4.dist-info/top_level.txt
+Filename: mwxlib-0.83.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.83.4.dist-info/RECORD
+Filename: mwxlib-0.83.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.83.4"
+__version__ = "0.83.5"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -1235,15 +1235,18 @@
                 ## "self._mgr.GetPane('watcher').FloatingPosition(self.Position)",
                 "self._mgr.Update()\n",
             )))
     
     def _load_file(self, bookname, filename, lineno):
         try:
             book = getattr(self, bookname)
-            book.load_file(filename, lineno)
+            if re.match(r"https?://[\w/:%#\$&\?()~.=+-]+", filename):
+                book.load_url(filename, lineno)
+            else:
+                book.load_file(filename, lineno)
         except Exception:
             pass
     
     def Init(self):
         msg = "#! Opened: <{}>\r\n".format(datetime.datetime.now())
         self.add_history(msg)
         self.add_log(msg)
@@ -1505,16 +1508,15 @@
                 self.debugger.interactive_shell = shell
         elif isinstance(obj, str):
             try:
                 shell = self.debugger.interactive_shell
                 self.debugger.interactive_shell = self.current_shell
                 self.debugger.editor = self.Log # set default logger
                 filename = "<string>"
-                buf = self.Log.find_buffer(filename)\
-                  or self.Log.create_buffer(filename)
+                buf = self.Log.find_buffer(filename) or self.Log.create_buffer(filename)
                 with buf.off_readonly():
                     buf.Text = obj
                 self.debugger.run(obj)
             finally:
                 self.debugger.interactive_shell = shell
         elif hasattr(obj, '__dict__'):
             self.message("Building locals info list...")
```

## mwx/nutshell.py

```diff
@@ -1381,15 +1381,14 @@
 
 class Buffer(EditWindow, EditorInterface):
     """Python code buffer.
     
     Attributes:
         name     : buffer-name (basename)
         filename : buffer-file-name
-        codename : code-file-name (e.g. '<scratch>')
         code     : code object
     """
     STYLE = {
         stc.STC_STYLE_DEFAULT     : "fore:#7f7f7f,back:#ffffb8,size:9,face:MS Gothic",
         stc.STC_STYLE_LINENUMBER  : "fore:#000000,back:#ffffb8,size:9",
         stc.STC_STYLE_BRACELIGHT  : "fore:#000000,back:#ffffb8,bold",
         stc.STC_STYLE_BRACEBAD    : "fore:#000000,back:#ff0000,bold",
@@ -1457,23 +1456,24 @@
             return os.path.getmtime(f) - self.__mtime
         elif f and re.match(r"https?://[\w/:%#\$&\?()~.=+-]+", f):
             return -1
     
     @property
     def caption(self):
         prefix = ''
-        if self.mtdelta is not None:
+        dt = self.mtdelta
+        if dt is not None:
             if self.IsModified():
                 prefix += '*'
-            if self.mtdelta > 0:
+            if dt > 0:
                 prefix += '!'
-            elif self.mtdelta < 0:
+            elif dt < 0:
                 prefix += '%'
-            if prefix:
-                prefix += ' '
+        if prefix:
+            prefix += ' '
         return prefix + self.name
     
     @property
     def need_buffer_save(self):
         """Returns whether the buffer should be saved.
         The file has been modified internally.
         """
@@ -1498,15 +1498,14 @@
     
     def __init__(self, parent, filename=None, **kwargs):
         EditWindow.__init__(self, parent, **kwargs)
         EditorInterface.__init__(self)
         
         self.parent = parent
         self.filename = filename
-        self.codename = ''
         self.code = None
         
         self.Bind(stc.EVT_STC_UPDATEUI, self.OnUpdate) # skip to brace matching
         
         self.Bind(stc.EVT_STC_SAVEPOINTLEFT, self.OnSavePointLeft)
         self.Bind(stc.EVT_STC_SAVEPOINTREACHED, self.OnSavePointReached)
         
@@ -1693,15 +1692,14 @@
                 self.EnsureVisible(lx) # expand if folded
                 self.EnsureCaretVisible()
                 self.AnnotationSetStyle(lx, stc.STC_STYLE_ANNOTATION)
                 self.AnnotationSetText(lx, msg)
             self.message("- {!r}".format(e))
             ## print(msg, file=sys.__stderr__)
         else:
-            self.codename = filename
             self.code = code
             del self.pointer # Reset pointer (debugger hook point).
             del self.red_arrow
             self.handler('py_region_executed', self)
             self.message("Evaluated {!r} successfully".format(filename))
             self.AnnotationClearAll()
     
@@ -1883,21 +1881,16 @@
     def buffer(self):
         """Returns the currently selected page or None."""
         return self.CurrentPage
     
     def find_buffer(self, f):
         """Find buffer with specified f:filename or code."""
         for buf in self.all_buffers:
-            if f is buf or f in buf: # check code
+            if f is buf or f in buf or f == buf.filename: # check code
                 return buf
-            elif isinstance(f, str):
-                if buf.code and f == buf.codename:
-                    return buf
-                if f == buf.filename:
-                    return buf
     
     def create_buffer(self, filename, index=None):
         """Create a new buffer (internal use only)."""
         try:
             self.Freeze()
             buf = Buffer(self, filename)
             self.set_attributes(buf, **self.defaultBufferStyle)
@@ -1946,15 +1939,15 @@
     ## File I/O
     ## --------------------------------
     wildcards = [
         "PY files (*.py)|*.py",
         "ALL files (*.*)|*.*",
     ]
     
-    def load_url(self, url, *args, **kwargs):
+    def load_url(self, url, lineno=0):
         import requests
         if wx.MessageBox( # Confirm URL load.
                 "You are loading URL contents.\n\n"
                f"{url!r}\n"
                 "Continue loading?",
                 "Load URL",
                 style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
@@ -1963,15 +1956,15 @@
         try:
             res = requests.get(url)
         except Exception as e:
             self.post_message("Failed to load URL: {}".format(e))
             return None
         if res.status_code == 200: # success
             buf = self.find_buffer(url) or self.create_buffer(url)
-            buf._load_textfile(res.text, url)
+            buf._load_textfile(res.text, url, lineno)
             self.swap_page(buf)
             return True
         return False
     
     def load_cache(self, filename, lineno=0, globals=None):
         """Load a file from cache using linecache.
         Note:
@@ -2039,32 +2032,38 @@
         except Exception as e:
             self.post_message("Failed to save {!r}: {}".format(buf.name, e))
             return False
     
     def load_buffer(self, buf=None):
         """Confirm the load with the dialog."""
         buf = buf or self.buffer
-        if buf.mtdelta is None:
+        dt = buf.mtdelta
+        if dt is None:
             self.post_message("No filename.")
             return None
-        if buf.mtdelta == 0 and not buf.IsModified():
+        elif dt == 0 and not buf.IsModified():
             self.post_message("No need to load.")
             return None
-        return self.load_file(buf, buf.markline+1)
+        elif dt < 0:
+            return self.load_url(buf.filename, buf.markline+1)
+        else:
+            return self.load_file(buf, buf.markline+1)
     
     def save_buffer(self, buf=None):
         """Confirm the save with the dialog."""
         buf = buf or self.buffer
-        if buf.mtdelta is None:
+        dt = buf.mtdelta
+        if dt is None:
             self.post_message("No filename.")
             return None
-        if buf.mtdelta == 0 and not buf.IsModified():
+        elif dt == 0 and not buf.IsModified():
             self.post_message("No need to save.")
             return None
-        return self.save_file(buf.filename, buf)
+        else:
+            return self.save_file(buf.filename, buf)
     
     def save_buffer_as(self, buf=None):
         """Confirm the saveas with the dialog."""
         buf = buf or self.buffer
         name = re.sub("[\\/:*?\"<>|]", '', buf.name)
         with wx.FileDialog(self, "Save buffer as",
                 defaultFile=name,
```

## Comparing `mwxlib-0.83.4.dist-info/LICENSE` & `mwxlib-0.83.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.83.4.dist-info/METADATA` & `mwxlib-0.83.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.83.4
+Version: 0.83.5
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.83.4.dist-info/RECORD` & `mwxlib-0.83.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=7hnSimA3bKDgTct29l6Hqpq7BCKqCeOjZJ6JQ1xjh7I,43445
-mwx/framework.py,sha256=_WT2Pod18b2CFYuJTNnglpWph-A4NWdPLFCmyKFzb78,73243
+mwx/framework.py,sha256=vmU8YOwbYLhmZSgK6pU68SzMntPv2v25E7KhXJTacL8,73366
 mwx/graphman.py,sha256=Edw2pZKghWGkbR_AV9PDWQpZz6q8XstTL5Q-xDrAce4,69534
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=h_aFij_7ksG2DXuYCaGmjtlcl122vZnwbMTv21Mprcg,27606
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=gKIDIFEji9x8ypPUdWmroUvPs0dTyoPg-zMnrvdJArA,138127
+mwx/nutshell.py,sha256=yDQxLhlIpGxcfOHHv0O8QvTVIXFj4B9ZSKcx9xF2VN4,137969
 mwx/utilus.py,sha256=q1DZGRNvtzk6Yavlc9XuLWMWgLS236khbiG4wa-hDj0,37351
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.83.4.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.83.4.dist-info/METADATA,sha256=j9WUxZBLCznmBJsIjheewsBQpN15LmpWdnSWP8rWnuI,1893
-mwxlib-0.83.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.83.4.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.83.4.dist-info/RECORD,,
+mwxlib-0.83.5.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.83.5.dist-info/METADATA,sha256=Tdlk8BlhUz_n9bEXZ-eYLjtsO7Jweh81Oe-rwNOyyOE,1893
+mwxlib-0.83.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.83.5.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.83.5.dist-info/RECORD,,
```

