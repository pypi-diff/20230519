# Comparing `tmp/ziafont-0.5.tar.gz` & `tmp/ziafont-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziafont-0.5.tar", last modified: Sun Nov  6 00:24:42 2022, max compression
+gzip compressed data, was "ziafont-0.6.tar", last modified: Fri May 19 20:48:49 2023, max compression
```

## Comparing `ziafont-0.5.tar` & `ziafont-0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:24:42.745016 ziafont-0.5/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2022-10-08 19:00:17.000000 ziafont-0.5/LICENSE.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1624 2022-11-06 00:24:42.745016 ziafont-0.5/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      610 2022-10-16 16:43:16.000000 ziafont-0.5/README.md
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       38 2022-11-06 00:24:42.745016 ziafont-0.5/setup.cfg
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1369 2022-11-06 00:20:43.000000 ziafont-0.5/setup.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:24:42.732016 ziafont-0.5/ziafont/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       77 2022-11-05 23:13:59.000000 ziafont-0.5/ziafont/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3481 2022-11-05 22:53:14.000000 ziafont-0.5/ziafont/cmap.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      534 2022-10-08 19:00:17.000000 ziafont-0.5/ziafont/config.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26315 2022-10-31 01:09:45.000000 ziafont-0.5/ziafont/font.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2707 2022-10-08 20:07:32.000000 ziafont-0.5/ziafont/fontread.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:24:42.744016 ziafont-0.5/ziafont/fonts/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   757076 2022-10-08 19:00:17.000000 ziafont-0.5/ziafont/fonts/DejaVuSans.ttf
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2022-10-08 19:00:17.000000 ziafont-0.5/ziafont/fonts/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1838 2022-10-30 23:23:08.000000 ziafont-0.5/ziafont/fonttypes.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7066 2022-10-26 02:26:13.000000 ziafont-0.5/ziafont/glyph.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    24789 2022-11-05 22:50:44.000000 ziafont-0.5/ziafont/glyphcff.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7307 2022-10-30 03:49:25.000000 ziafont-0.5/ziafont/glyphglyf.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10631 2022-10-29 01:06:03.000000 ziafont-0.5/ziafont/glyphinspect.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15229 2022-10-31 01:12:01.000000 ziafont-0.5/ziafont/gpos.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    25210 2022-10-31 01:16:34.000000 ziafont-0.5/ziafont/gsub.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2022-10-08 19:00:17.000000 ziafont-0.5/ziafont/py.typed
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6342 2022-10-22 21:54:32.000000 ziafont-0.5/ziafont/svgpath.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6616 2022-10-31 01:12:36.000000 ziafont-0.5/ziafont/tables.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2022-11-06 00:24:42.742016 ziafont-0.5/ziafont.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1624 2022-11-06 00:24:42.000000 ziafont-0.5/ziafont.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      518 2022-11-06 00:24:42.000000 ziafont-0.5/ziafont.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2022-11-06 00:24:42.000000 ziafont-0.5/ziafont.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2022-10-08 19:01:25.000000 ziafont-0.5/ziafont.egg-info/not-zip-safe
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2022-11-06 00:24:42.000000 ziafont-0.5/ziafont.egg-info/top_level.txt
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-19 20:48:49.094739 ziafont-0.6/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2023-04-15 17:51:16.000000 ziafont-0.6/LICENSE.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1796 2023-05-19 20:48:49.094739 ziafont-0.6/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      749 2023-05-18 01:38:49.000000 ziafont-0.6/README.md
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-05-13 15:15:45.000000 ziafont-0.6/pyproject.toml
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1151 2023-05-19 20:48:49.094739 ziafont-0.6/setup.cfg
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-19 20:48:49.091739 ziafont-0.6/ziafont/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       77 2023-05-19 20:06:38.000000 ziafont-0.6/ziafont/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3549 2023-05-18 01:40:11.000000 ziafont-0.6/ziafont/cmap.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      579 2023-05-18 01:40:49.000000 ziafont-0.6/ziafont/config.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    26281 2023-05-18 01:48:13.000000 ziafont-0.6/ziafont/font.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2768 2023-05-18 01:48:58.000000 ziafont-0.6/ziafont/fontread.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-19 20:48:49.094739 ziafont-0.6/ziafont/fonts/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   757076 2023-04-15 17:51:16.000000 ziafont-0.6/ziafont/fonts/DejaVuSans.ttf
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:51:16.000000 ziafont-0.6/ziafont/fonts/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1974 2023-05-18 01:49:39.000000 ziafont-0.6/ziafont/fonttypes.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7589 2023-05-18 01:53:56.000000 ziafont-0.6/ziafont/glyph.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    24741 2023-05-18 01:58:08.000000 ziafont-0.6/ziafont/glyphcff.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7293 2023-05-18 02:00:46.000000 ziafont-0.6/ziafont/glyphglyf.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10801 2023-05-18 02:02:52.000000 ziafont-0.6/ziafont/glyphinspect.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15446 2023-05-18 02:06:04.000000 ziafont-0.6/ziafont/gpos.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    25341 2023-05-18 02:10:06.000000 ziafont-0.6/ziafont/gsub.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2023-04-15 17:51:16.000000 ziafont-0.6/ziafont/py.typed
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6410 2023-05-18 02:11:19.000000 ziafont-0.6/ziafont/svgpath.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6616 2023-04-15 17:51:16.000000 ziafont-0.6/ziafont/tables.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-05-19 20:48:49.093739 ziafont-0.6/ziafont.egg-info/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1796 2023-05-19 20:48:49.000000 ziafont-0.6/ziafont.egg-info/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      534 2023-05-19 20:48:49.000000 ziafont-0.6/ziafont.egg-info/SOURCES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-19 20:48:49.000000 ziafont-0.6/ziafont.egg-info/dependency_links.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-05-14 23:10:11.000000 ziafont-0.6/ziafont.egg-info/not-zip-safe
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        8 2023-05-19 20:48:49.000000 ziafont-0.6/ziafont.egg-info/top_level.txt
```

### Comparing `ziafont-0.5/LICENSE.txt` & `ziafont-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ziafont-0.5/README.md` & `ziafont-0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 # ziafont
 
 Ziafont reads TrueType/OpenType font files and draws characters and strings as SVG <path> elements. Unlike the SVG <text> element, the output of Ziafont's SVG will render identically on any system, independent of whether the original font is available.
 
-Ziafont supports fonts with TrueType glyph outlines contained in a "glyf" table in the font (these fonts typically have a .ttf extensions), or fonts with a "CFF " table (typically with a .otf extension). Kerning adjustment is supported if the font has a "GPOS" table.
+Ziafont supports fonts with TrueType glyph outlines contained in a "glyf" table in the font (these fonts typically have a .ttf extensions), or fonts with a "CFF " table (typically with a .otf extension). Kerning adjustment and glyph substitution are supported if the font has a "GPOS" table.
 
-Documentation is available at [readthedocs](https://ziafont.readthedocs.io)
+Documentation is available at [readthedocs](https://ziafont.readthedocs.io). There is also an [online demo](https://cdelker.github.io/pyscript/ziafont.html) of Glyph rendering using Ziafont.
```

### Comparing `ziafont-0.5/ziafont/cmap.py` & `ziafont-0.6/ziafont/cmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         self.glyphmap = {}
         for startid, start in enumerate(self.startcodes):
             for i in range(start, self.endcodes[startid]+1):
                 self.glyphmap[i] = self.glyphstarts[startid] + (i-start)
 
         self.glyphmap_r: Optional[dict[int, set[str]]] = None  # Build on demand
-                
+
     def __repr__(self):
         return f'<Cmap Format 12: {self.platform} id={self.platformid}'
 
     def glyphid(self, char: str) -> int:
         ''' Get glyph index from a character '''
         charid = ord(char)
         return self.glyphmap.get(charid, 0)       
@@ -54,15 +54,18 @@
         self.iddeltas = iddeltas
         self.glyphidarray = glyphidarray
 
         self.glyphmap = {}
         for seg, startcode in enumerate(self.startcodes):
             for i in range(startcode, self.endcodes[seg]+1):
                 if self.idrangeoffset[seg] != 0:
-                    idx = seg - len(self.startcodes) + self.idrangeoffset[seg]//2 + i - self.startcodes[seg]
+                    idx = (seg 
+                           - len(self.startcodes)
+                           + self.idrangeoffset[seg]//2
+                           + i - self.startcodes[seg])
                     gid = self.glyphidarray[idx]
                     gid = self.iddeltas[seg] + gid if gid > 0 else 0
                 else:
                     gid = (self.iddeltas[seg] + i) % 0x10000
                 self.glyphmap[i] = gid
 
         self.glyphmap_r: Optional[dict[int, set[str]]] = None  # Build on demand
```

### Comparing `ziafont-0.5/ziafont/font.py` & `ziafont-0.6/ziafont/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 ''' Read font file and write glyphs to SVG '''
 
 from __future__ import annotations
 from typing import Literal, Union, Optional, Sequence, Dict
-import sys
-import os
 import math
 from pathlib import Path
 from collections import namedtuple
 import importlib.resources as pkg_resources
 import xml.etree.ElementTree as ET
-import warnings
 
 from .config import config
 from .fontread import FontReader
 from . import gpos
 from . import gsub
 from .cmap import Cmap12, Cmap4
 from .glyph import SimpleGlyph, CompoundGlyph
 from .glyphcff import read_glyph_cff, CFF
 from .glyphglyf import read_glyph_glyf
 from .glyphinspect import ShowGlyphs
-from .fonttypes import AdvanceWidth, Layout, Header, Table, FontInfo, FontNames, Symbols, FontFeatures
+from .fonttypes import (AdvanceWidth, Layout, Header, Table,
+                        FontInfo, FontNames, Symbols, FontFeatures)
 from .svgpath import fmt
 
 
 class Font:
     ''' Class to read/parse a OpenType/TTF and write glyphs to SVG
 
         Args:
@@ -40,14 +38,15 @@
         else:
             with pkg_resources.path('ziafont.fonts', 'DejaVuSans.ttf') as p:
                 self.fname = p
 
         with open(self.fname, 'rb') as f:
             self.fontfile = FontReader(f.read())
 
+        self.tables = {}
         self.features = FontFeatures()
         self.info = self._loadfont()  # Load in all the font metadata
         self._glyphs: Dict[int, Union[SimpleGlyph, CompoundGlyph]] = {}
         self._glyphids: Dict[str, int] = {}
 
     def _loadfont(self) -> FontInfo:
         ''' Read font metadata '''
@@ -287,21 +286,21 @@
     def languages(self, script='DFLT'):
         ''' Get list of languages in the script '''
         langs = set()
         if self.gpos:
             s = self.gpos.scripts.get(script, None)
             if s is not None:
                 langs = langs.union(set(s.languages.keys()))
-            
+
         if self.gsub:
             s = self.gsub.scripts.get(script, None)
             if s is not None:
                 langs = langs.union(set(s.languages.keys()))
         return list(langs)
-       
+
     def language(self, script, language):
         ''' Set script/language to use '''
         if script not in self.scripts():
             raise ValueError(f'Script {script} not defined in font')
 
         if language not in self.languages(script):
             raise ValueError(f'Language {language} not defined in font')
@@ -316,15 +315,15 @@
     def glyphindex(self, char: str) -> int:
         ''' Get index of character glyph '''
         gid = self._glyphids.get(char)
         if gid is None:
             gid = self.cmap.glyphid(char)  # type: ignore
             self._glyphids[char] = gid
         return gid
-            
+
     def glyph(self, char: str) -> SimpleGlyph:
         ''' Get the Glyph for the character '''
         index = self.glyphindex(char)        # Glyph Number
         return self.glyph_fromid(index)
 
     def glyph_fromid(self, glyphid: int) -> Union[SimpleGlyph, CompoundGlyph]:
         ''' Read a glyph from the "glyf" table
@@ -357,21 +356,21 @@
 
     def getsize(self, s) -> tuple[float, float]:
         ''' Calculate width and height (including ascent/descent) of string '''
         txt = Text(s, self)
         return txt.getsize()
 
     def text(self, s: str,
-             size: float=None,
-             linespacing: float=1,
-             halign: Literal['left', 'center', 'right']='left',
-             valign: Literal['base', 'center', 'top']='base',
-             color: str=None,
-             rotation: float=0,
-             rotation_mode: str='anchor'):
+             size: float = None,
+             linespacing: float = 1,
+             halign: Literal['left', 'center', 'right'] = 'left',
+             valign: Literal['base', 'center', 'top'] = 'base',
+             color: str = None,
+             rotation: float = 0,
+             rotation_mode: str = 'anchor'):
         ''' Create a Text object using this font
 
             Args:
                 s: String to convert.
                 size: Font size in points
                 linespacing: Space between lines
                 halign: Horizontal Alignment
@@ -403,16 +402,18 @@
             halign: Horizontal Alignment
             valign: Vertical Alignment
             rotation: Rotation angle in degrees
             rotation_mode: Either 'default' or 'anchor', to
                 mimic Matplotlib behavoir. See:
                 https://matplotlib.org/stable/gallery/text_labels_and_annotations/demo_text_rotation_mode.html
     '''
-    def __init__(self, s: Union[str, Sequence[int]],  font: Union[str, Font] = None,
-                 size: float = None, linespacing: float = 1,
+    def __init__(self, s: Union[str, Sequence[int]],
+                 font: Union[str, Font] = None,
+                 size: float = None,
+                 linespacing: float = 1,
                  halign: Literal['left', 'center', 'right'] = 'left',
                  valign: Literal['base', 'center', 'top'] = 'base',
                  color: str = None,
                  rotation: float = 0,
                  rotation_mode: str = 'anchor'):
         self.str = s
         self.halign = halign
@@ -553,15 +554,15 @@
             gidlines = [self.str]  # Single line
         return gidlines
 
     def _buildstring(self) -> Symbols:
         ''' Create symbols and svg word in a <g> group tag, for placing in an svg '''
         scale = self.size / self.font.info.layout.unitsperem
         lineheight = self.size * self.linespacing
-        
+
         gidlines = self.str_to_gids()
         yvals = [i*lineheight for i in range(len(gidlines))]  # valign == 'base'
 
         # Generate symbols and calculate x positions using left alignment
         symbols: list[ET.Element] = []  # <symbol> elements
         linewidths: list[float] = []
         xadvance = 0.
@@ -574,30 +575,30 @@
 
             glyphs = [self.font.glyph_fromid(gid) for gid in glyphids]
             x = 0
             xmin = min(xmin, glyphs[0].bbox.xmin*scale)
             for gidx, glyph in enumerate(glyphs):
                 if glyph.id not in [s.attrib['id'] for s in symbols]:
                     symbols.append(glyph.svgsymbol())
-                                
+
                 prevglyph = glyphs[gidx-1] if gidx-1 >= 0 else None
                 nextglyph = glyphs[gidx+1] if gidx+1 < len(glyphs) else None
                 if self.font.gpos and prevglyph:
                     # Attach marks
                     placexy = self.font.gpos.placemark(prevglyph.index, glyph.index)
                     if placexy:
                         if not placexy.mkmk:  # Relative to base glyph
                             dx = dy = 0
                         dx += (placexy.dx - xadvance) * scale
                         dy += -placexy.dy * scale
                     else:
                         dx = dy = 0
                 else:
                     dx = dy = 0  # Don't reset, may need these for mark-to-mark p[
-                        
+
                 lineglyphs.append((glyph, x+dx, dy))                
                 xadvance = glyph.advance(nextglyph)
                 x += xadvance * scale
 
             if glyph.bbox.xmax > xadvance:
                 # Make linewidth a bit wider to grab right edge
                 # that extends beyond advance width
```

### Comparing `ziafont-0.5/ziafont/fontread.py` & `ziafont-0.6/ziafont/fontread.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,61 +5,63 @@
 from io import BytesIO
 
 
 class FontReader(BytesIO):
     ''' Class for reading from Font File '''
     # TTF/OTF is big-endian (>)
 
-    def readuint32(self, offset: int=None) -> int:
+    def readuint32(self, offset: int = None) -> int:
         ''' Read 32-bit unsigned integer '''
         if offset:
             self.seek(offset)
         return struct.unpack('>I', self.read(4))[0]
 
-    def readuint24(self, offset: int=None) -> int:
+    def readuint24(self, offset: int = None) -> int:
         ''' Read 24-bit unsigned integer '''
         if offset:
             self.seek(offset)
         return int.from_bytes(self.read(3), 'big')
-    
-    def readuint16(self, offset: int=None) -> int:
+
+    def readuint16(self, offset: int = None) -> int:
         ''' Read 16-bit unsigned integer '''
         if offset:
             self.seek(offset)
         return struct.unpack('>H', self.read(2))[0]
 
-    def readuint8(self, offset: int=None) -> int:
+    def readuint8(self, offset: int = None) -> int:
         ''' Read 8-bit unsigned integer '''
         if offset:
             self.seek(offset)
         return struct.unpack('>B', self.read(1))[0]
 
-    def readint8(self, offset: int=None) -> int:
+    def readint8(self, offset: int = None) -> int:
         ''' Read 8-bit signed integer '''
         if offset:
             self.seek(offset)
         return struct.unpack('>b', self.read(1))[0]
 
-    def readdate(self, offset: int=None) -> datetime:
+    def readdate(self, offset: int = None) -> datetime:
         ''' Read datetime '''
         if offset:
             self.seek(offset)
         mtime = self.readuint32() * 0x100000000 + self.readuint32()
         fontepoch = datetime(1904, 1, 1)
         mdate = fontepoch + timedelta(seconds=mtime)
         return mdate
 
-    def readint16(self, offset: int=None) -> int:
+    def readint16(self, offset: int = None) -> int:
         ''' Read 16-bit signed integer '''
         if offset:
             self.seek(offset)
         return struct.unpack('>h', self.read(2))[0]
 
-    def readshort(self, offset: int=None) -> float:
+    def readshort(self, offset: int = None) -> float:
         ''' Read "short" fixed point number (S1.14) '''
+        if offset:
+            self.seek(offset)
         x = self.readint16()
         return float(x) * 2**-14
 
     def readvaluerecord(self, fmt: int) -> dict:
         ''' Read a GPOS "ValueRecord" into a dictionary. Zero values will be omitted. '''
         record = {}
         if fmt & 0x0001:
```

### Comparing `ziafont-0.5/ziafont/fonts/DejaVuSans.ttf` & `ziafont-0.6/ziafont/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `ziafont-0.5/ziafont/fonttypes.py` & `ziafont-0.6/ziafont/fonttypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 Table = namedtuple('Table', ['checksum', 'offset', 'length'])
 BBox = namedtuple('BBox', ['xmin', 'xmax', 'ymin', 'ymax'])
 AdvanceWidth = namedtuple('AdvanceWidth', ['width', 'leftsidebearing'])
 Header = namedtuple(
     'Header', ['version', 'revision', 'checksumadjust', 'magic', 'flags',
                'created', 'modified', 'macstyle', 'lowestrecppem',
-               'directionhint', 'indextolocformat', 'glyphdataformat', 'numlonghormetrics', 'numglyphs'])
-FontNames = namedtuple('FontNames', ['copyright', 'family', 'subfamily', 'unique', 'name', 'nameversion',
-                       'postscript', 'trademark', 'manufacturer', 'designer',
-                       'description', 'vendorurl', 'designerurl', 'license', 'LicenseURL'])
+               'directionhint', 'indextolocformat', 'glyphdataformat',
+               'numlonghormetrics', 'numglyphs'])
+FontNames = namedtuple('FontNames', ['copyright', 'family', 'subfamily', 'unique',
+                                     'name', 'nameversion', 'postscript', 'trademark',
+                                     'manufacturer', 'designer', 'description', 'vendorurl',
+                                     'designerurl', 'license', 'LicenseURL'])
 Layout = namedtuple(
     'Layout', ['unitsperem', 'xmin', 'xmax', 'ymin', 'ymax',
                'ascent', 'descent', 'advwidthmax',
                'minleftbearing', 'minrightbearing'])
 FontInfo = namedtuple(
     'FontInfo', ['filename', 'names', 'header', 'layout'])
 
@@ -31,8 +33,9 @@
     calt: bool = True   # Contextual alternatives
     clig: bool = True   # Contextual ligatures
     salt: bool = False  # Stylistic alternatives (apply all or nothing)
     dlig: bool = False  # Discretionary ligatures
     hlig: bool = False  # Historical ligatures
     c2sc: bool = False  # Small Capitals from Capitals
     frac: bool = False  # Fractions
-    zero: bool = False  # Zeros with slash
+    zero: bool = False  # Zeros with slash
+    ssty: bool = False  # Math script style alternates
```

### Comparing `ziafont-0.5/ziafont/glyph.py` & `ziafont-0.6/ziafont/glyph.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,133 +14,137 @@
 
 if TYPE_CHECKING:
     from .font import Font
 
 
 class SimpleGlyph:
     ''' Simple Glyph '''
-    dfltsize = 12   # Draw <symbols> in this point size
+    DFLT_SIZE_PT = 12   # Draw <symbols> in this point size
 
     def __init__(self, index: int, operators: Sequence[SVGOpType],
                  bbox: BBox, font: Font):
         self.index = index
         self.operators = operators
         self.bbox = bbox
         self.path = SimpleNamespace()
         self.path.bbox = bbox  # Only for backward-compatibility
         self.font = font
         basename, _ = os.path.splitext(os.path.basename(self.font.info.filename))
         basename = ''.join(c for c in basename if c.isalnum())
         self.id = f'{basename}_{index}'
-        self.emscale = self.dfltsize / self.font.info.layout.unitsperem
+        self._points_per_unit = self.DFLT_SIZE_PT / self.font.info.layout.unitsperem
 
     def _repr_svg_(self):
         return ET.tostring(self.svgxml(), encoding='unicode')
 
     @property
     def char(self) -> set[str]:
         ''' Get set of unicode character represented by this glyph '''
         if self.font.cmap:
             return self.font.cmap.char(self.index)
         return set()
-    
-    def place(self, x: float, y: float, fontsize: float) -> Optional[ET.Element]:
+
+    def funits_to_points(self, value: float, scale_factor: float = 1) -> float:
+        ''' Convert font units to points '''
+        return value * self._points_per_unit * scale_factor
+
+    def place(self, x: float, y: float, point_size: float) -> Optional[ET.Element]:
         ''' Get <use> svg tag translated/scaled to the right position '''
-        fntscale = (fontsize/self.dfltsize)
-        yshift = self.font.info.layout.ymax * self.emscale * fntscale
+        scale_factor = point_size / self.DFLT_SIZE_PT
+        yshift = self.funits_to_points(
+            max(self.bbox.ymax, self.font.info.layout.ymax), scale_factor)
         elm: Optional[ET.Element]
         if config.svg2:
             elm = ET.Element('use')
             elm.attrib['href'] = f'#{self.id}'
-            dx = min(self.bbox.xmin * self.emscale * fntscale, 0)
-            elm.attrib['transform'] = f'translate({fmt(x+dx)} {fmt(y-yshift)}) scale({fmt(fntscale)})'
+            dx = min(self.funits_to_points(self.bbox.xmin, scale_factor), 0)
+            elm.attrib['transform'] = (f'translate({fmt(x+dx)} '
+                                       f'{fmt(y-yshift)}) scale({fmt(scale_factor)})')
         else:
-            elm = self.svgpath(x0=x, y0=y, scale=fntscale)
+            elm = self.svgpath(x0=x, y0=y, scale_factor=scale_factor)
         return elm
 
-    def advance(self, nextchr=None):
+    def advance(self, nextchr=None) -> float:
         ''' Get advance width in glyph units, including kerning if nextchr is defined '''
         if nextchr:
             nextchr = nextchr.index
         return self.font.advance(self.index, nextchr)
 
-    def svgpath(self, x0: float = 0, y0: float = 0, scale: float = 1) -> Optional[ET.Element]:
+    def svgpath(self, x0: float = 0, y0: float = 0, scale_factor: float = 1) -> Optional[ET.Element]:
         ''' Get svg <path> element for glyph, normalized to 12-point font '''
-        emscale = self.emscale * scale
         path = ''
-        for i, op in enumerate(self.operators):
-            segment = op.path(x0, y0, scale=emscale)
+        for operator in self.operators:
+            segment = operator.path(x0, y0, scale=self.funits_to_points(1, scale_factor))
             if segment[0] == 'M' and path != '':
                 path += 'Z '  # Close intermediate segments
             path += segment
         if path == '':
             return None  # Don't return empty path
         path += 'Z '
         return ET.Element('path', attrib={'d': path})
 
     def svgsymbol(self) -> ET.Element:
         ''' Get svg <symbol> element for this glyph, scaled to 12-point font '''
-        xmin = min(self.bbox.xmin * self.emscale, 0)
-        xmax = self.bbox.xmax * self.emscale
+        xmin = min(self.funits_to_points(self.bbox.xmin), 0)
+        xmax = self.funits_to_points(self.bbox.xmax)
         width = xmax-xmin
-        ymax = max(self.font.info.layout.ymax, self.bbox.ymax) * self.emscale
-        ymin = min(self.font.info.layout.ymin, self.bbox.ymin) * self.emscale
+        ymax = self.funits_to_points(max(self.font.info.layout.ymax, self.bbox.ymax))
+        ymin = self.funits_to_points(min(self.font.info.layout.ymin, self.bbox.ymin))
         height = ymax - ymin
 
         sym = ET.Element('symbol')
         sym.attrib['id'] = self.id
         sym.attrib['width'] = fmt(width)
         sym.attrib['height'] = fmt(height)
         sym.attrib['viewBox'] = f'{fmt(xmin)} {fmt(-ymax)} {fmt(width)} {fmt(height)}'
-        path = self.svgpath()
-        if path is not None:
+        if (path := self.svgpath()) is not None:
             sym.append(path)
         return sym
 
-    def svg(self, fontsize: float = None) -> str:
+    def svg(self, point_size: float = None) -> str:
         ''' Get SVG as string '''
-        return ET.tostring(self.svgxml(fontsize), encoding='unicode')
+        return ET.tostring(self.svgxml(point_size), encoding='unicode')
 
-    def svgxml(self, fontsize: float = None) -> ET.Element:
+    def svgxml(self, point_size: float = None) -> ET.Element:
         ''' Standalong SVG '''
-        fontsize = fontsize if fontsize else config.fontsize
-        scale = fontsize / self.font.info.layout.unitsperem
+        point_size = point_size if point_size else config.fontsize
+        scale_factor = point_size / self.DFLT_SIZE_PT
 
         # Width varies by character, but height is constant for the whole font
         # View should include whole character, even if it goes negative/outside the advwidth
-        xmin = min(self.bbox.xmin * scale, 0)
-        xmax = self.bbox.xmax * scale
-        ymin = min(self.bbox.ymin, self.font.info.layout.ymin) * scale
+        xmin = self.funits_to_points(min(self.bbox.xmin, 0), scale_factor)
+        xmax = self.funits_to_points(self.bbox.xmax, scale_factor)
+        ymin = self.funits_to_points(min(self.bbox.ymin, self.font.info.layout.ymin), scale_factor)
 
         # ymax can go above font's ymax for extended (ie math) glyphs
-        ymax = max(self.bbox.ymax, self.font.info.layout.ymax) * scale
+        ymax = self.funits_to_points(max(self.bbox.ymax, self.font.info.layout.ymax), scale_factor)
         width = xmax - xmin
         height = ymax - ymin
         base = ymax
-        scale = fontsize/self.dfltsize
 
         svg = ET.Element('svg')
         svg.attrib['width'] = fmt(width)
         svg.attrib['height'] = fmt(height)
         svg.attrib['xmlns'] = 'http://www.w3.org/2000/svg'
         svg.attrib['viewBox'] = f'{fmt(xmin)} 0 {fmt(width)} {fmt(height)}'
         if not config.svg2:
             svg.attrib['xmlns:xlink'] = 'http://www.w3.org/1999/xlink'
-            elm = self.svgpath(x0=0, y0=base, scale=scale)
+            elm = self.svgpath(x0=0, y0=base, scale_factor=scale_factor)
             if elm is not None:
                 svg.append(elm)
         else:
             symbol = self.svgsymbol()
             svg.append(symbol)
             g = ET.SubElement(svg, 'use')
             g.attrib['href'] = f'#{self.id}'
-            g.attrib['transform'] = f'translate({fmt(xmin)}, {fmt(base-ymax)}) scale({fmt(scale)})'
+            g.attrib['transform'] = (f'translate({fmt(xmin)}, '
+                                     f'{fmt(base-ymax)}) scale({fmt(scale_factor)})')
         return svg
 
-    def test(self, pxwidth: float=400, pxheight: float=400) -> InspectGlyph:
+    def test(self, pxwidth: float = 400, pxheight: float = 400) -> InspectGlyph:
         ''' Get Glyph Test representation showing vertices and borders '''
         return InspectGlyph(self, pxwidth, pxheight)
 
     def describe(self) -> DescribeGlyph:
         ''' Get Glyph Test representation showing vertices and borders '''
         return DescribeGlyph(self)
 
@@ -160,18 +164,17 @@
             if xform.match:
                 raise NotImplementedError('Compound glyph match transform')
 
             m0 = max(abs(xform.a), abs(xform.b))
             n0 = max(abs(xform.c), abs(xform.d))
             m = 2*m0 if abs(abs(xform.a)-abs(xform.c)) <= 33/65536 else m0
             n = 2*n0 if abs(abs(xform.b)-abs(xform.d)) <= 33/65536 else n0
-            for op in glyph.operators:
-                xoperators.append(op.xform(xform.a, xform.b, xform.c,
-                                           xform.d, xform.e, xform.f, m, n))
+            for operator in glyph.operators:
+                xoperators.append(operator.xform(xform.a, xform.b, xform.c,
+                                                 xform.d, xform.e, xform.f, m, n))
         return xoperators
 
 
-
 class EmptyGlyph(SimpleGlyph):
     ''' Glyph with no contours (like a space) '''
     def __init__(self, index: int, font: Font):
         super().__init__(index, [], BBox(0, 0, 0, 0), font)
```

### Comparing `ziafont-0.5/ziafont/glyphcff.py` & `ziafont-0.6/ziafont/glyphcff.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,27 +123,27 @@
         elif op == Operator.HMOVETO:
             p = p + Point(value[0], 0)
             operators.append(Moveto(p))
         elif op == Operator.VMOVETO:
             p = p + Point(0, value[0])
             operators.append(Moveto(p))
         elif op == Operator.HLINETO:
-            for i in range(len(value)):
+            for i, val in enumerate(value):
                 if (i % 2) == 0:  # Alternate Horizontal and Vertical lines
-                    p = p + Point(value[i], 0)
+                    p = p + Point(val, 0)
                 else:
-                    p = p + Point(0, value[i])
+                    p = p + Point(0, val)
                 operators.append(Lineto(p))
 
         elif op == Operator.VLINETO:
-            for i in range(len(value)):
+            for i, val in enumerate(value):
                 if (i % 2) == 0:  # Alternate Horizontal and Vertical lines
-                    p = p + Point(0, value[i])
+                    p = p + Point(0, val)
                 else:
-                    p = p + Point(value[i], 0)
+                    p = p + Point(val, 0)
                 operators.append(Lineto(p))
 
         elif op == Operator.RLINETO:
             for dx, dy in zip(value[::2], value[1::2]):
                 p = p + Point(dx, dy)
                 operators.append(Lineto(p))
 
@@ -305,27 +305,27 @@
             operators.append(Cubic(p1, p2, p3))
             operators.append(Cubic(p4, p5, p))
 
         elif op == Operator.FLEX1:
             dx1, dy1, dx2, dy2, dx3, dy3, dx4, dy4, dx5, dy5, d6, *_ = value
             dx = dx1+dx2+dx3+dx4+dx5
             dy = dy1+dy2+dy3+dy4+dy5
-            
+
             p1 = p + Point(dx1, dy1)
             p2 = p1 + Point(dx2, dy2)
             p3 = p2 + Point(dx3, dy3)
             p4 = p3 + Point(dx4, dy4)
             p5 = p4 + Point(dx5, dy5)
             if abs(dx) > abs(dy):
                 p = p5 + Point(d6, 0)
             else:
                 p = p5 + Point(0, d6)
             operators.append(Cubic(p1, p2, p3))
             operators.append(Cubic(p4, p5, p))
-            
+
         elif op == Operator.HFLEX:
             dx1, dx2, dy2, dx3, dx4, dx5, dx6, *_ = value
             p1 = p + Point(dx1, 0)
             p2 = p1 + Point(dx2, dy2)
             p3 = p2 + Point(dx3, 0)
             p4 = p3 + Point(dx4, 0)
             p5 = p4 + Point(dx5, 0)
@@ -370,17 +370,17 @@
 
         self.stack: list[float] = []
         self.operators: list[Union[Operator, int]] = []
         self.operands: list[list[float]] = []
         self.nhints = 0
         self.readcharstr(buf)
 
-    def append(self, op: Operator):
+    def append(self, operator: Operator):
         ''' Append an operator, and clear the stack '''
-        self.operators.append(op)
+        self.operators.append(operator)
         self.operands.append(self.stack)
         self.stack = []
 
     def addwidth(self):
         ''' Add width operator '''
         self.operators.append(Operator.WIDTH)
         self.operands.append([self.stack[0]])
@@ -400,16 +400,16 @@
                 nbytes = 1
                 if buf[0] == 12:
                     key = struct.unpack_from('>H', buf)[0]
                     nbytes = 2
 
                 try:
                     key = Operator(key)
-                except ValueError:
-                    raise NotImplementedError(f'Unimplemented KEY {key}')
+                except ValueError as exc:
+                    raise NotImplementedError(f'Unimplemented KEY {key}') from exc
 
                 if len(self.operators) == 0:
                     # First operator can have extra width parameter.
                     # have to deduce its presence based on the
                     # operator and number of values in stack
                     if key in [Operator.CNTRMASK, Operator.ENDCHAR] and self.lenstack == 1:
                         self.addwidth()
@@ -440,23 +440,24 @@
                     subchstr = sublist[idx]
                     self.stack = self.stack[:-1]  # remove sub# from stack
                     self.readcharstr(subchstr)
                     buf = buf[nbytes:]
                     continue
 
                 elif key in [Operator.HINTMASK, Operator.CNTRMASK]:
-                    if (len(self.operators) > 0 and self.operators[-1] == Operator.HSTEMHM and
-                        self.lenstack > 0):
+                    if (len(self.operators) > 0
+                            and self.operators[-1] == Operator.HSTEMHM
+                            and self.lenstack > 0):
                         # Implied VSTEM operator
                         self.nhints += self.lenstack // 2
                         self.append(Operator.VSTEMHM)
-                    elif (len(self.operators) == 0 or 
-                          (len(self.operators) == 1 and self.operators[0] == Operator.WIDTH)):
+                    elif (len(self.operators) == 0
+                            or (len(self.operators) == 1 and self.operators[0] == Operator.WIDTH)):
                         self.nhints += self.lenstack // 2
-                        self.append(Operator.VSTEMHM) ## ??
+                        self.append(Operator.VSTEMHM)
                     # N-bits for the N hint masks just read in
                     hintbytes = self.nhints + 7 >> 3
                     self.stack = list(buf[1:hintbytes+1])
                     nbytes = hintbytes+1
 
                 elif key in [Operator.HSTEM, Operator.HSTEMHM,
                              Operator.VSTEM, Operator.VSTEMHM]:
@@ -479,16 +480,14 @@
                 self.stack.append(-(buf[0]-251)*256 - buf[1] - 108)
                 nbytes = 2
             elif buf[0] == 255:
                 self.stack.append(struct.unpack_from('>l', buf[1:])[0] / 0x10000)
                 nbytes = 5
             else:
                 raise ValueError('Bad encoding byte: ' + str(buf[0]))
-                self.stack.append(None)
-                nbytes = 1
 
             buf = buf[nbytes:]
 
 
 def readdict(buf: bytes) -> dict:
     ''' Read a CFF dictionary structure from the buffer '''
     data: dict[Union[int, str], Union[None, list[float], float]] = {}
```

### Comparing `ziafont-0.5/ziafont/glyphglyf.py` & `ziafont-0.6/ziafont/glyphglyf.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
             yval += fontfile.readint16()
         # else: yval stays the same
         yvals.append(yval)
 
     points = []
     controls = []
     start = 0
-    for i in range(len(ends)):
-        stop = ends[i] + 1
+    for end in ends:
+        stop = end + 1
         points.append([Point(x, y) for x, y in zip(xvals[start:stop], yvals[start:stop])])
         controls.append(ctvals[start:stop])
         start = stop
 
     operators: list[SVGOpType] = []
     for p, c in zip(points, controls):
         npoints = len(p)
```

### Comparing `ziafont-0.5/ziafont/glyphinspect.py` & `ziafont-0.6/ziafont/glyphinspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def svg(self) -> str:
         ''' Glyph SVG string '''
         return ET.tostring(self.svgxml(), encoding='unicode')
 
     def svgxml(self) -> ET.Element:
         ''' Glyph svg as XML element tree '''
         # Draw glyph at 1:1 scale in glyph units
-        height = (self.font.info.layout.ymax - self.font.info.layout.ymin)
+        height = self.font.info.layout.ymax - self.font.info.layout.ymin
         width = height * self.pxwidth/self.pxheight
 
         # vertical positions
         ymargin = height / 20
         height *= 1.1
         bot = height - ymargin
         baseline = height + self.font.info.layout.ymin - ymargin
@@ -86,21 +86,23 @@
             path.set('opacity', '.5')
             path.set('vector-effect', 'non-scaling-stroke')
         vline(x0, 'gray')
         vline(x1, 'gray')
 
         # Ticks
         z = ET.SubElement(svg, 'path')
-        z.set('d', f'M {fmt(x0-tick)} {fmt(baseline)} L {fmt(x0)} {fmt(baseline)} {fmt(x0)} {fmt(baseline+tick)}')
+        z.set('d', (f'M {fmt(x0-tick)} {fmt(baseline)} '
+                    f'L {fmt(x0)} {fmt(baseline)} {fmt(x0)} {fmt(baseline+tick)}'))
         z.set('stroke', '#444444')
         z.set('stroke-width', '4px')
         z.set('fill', 'none')
         z.set('vector-effect', 'non-scaling-stroke')
         z = ET.SubElement(svg, 'path')
-        z.set('d', f'M {fmt(x1+tick)} {fmt(baseline)} L {fmt(x1)} {fmt(baseline)} {fmt(x1)} {fmt(baseline+tick)}')
+        z.set('d', (f'M {fmt(x1+tick)} {fmt(baseline)} '
+                    f'L {fmt(x1)} {fmt(baseline)} {fmt(x1)} {fmt(baseline+tick)}'))
         z.set('stroke', '#444444')
         z.set('stroke-width', '4px')
         z.set('fill', 'none')
         z.set('vector-effect', 'non-scaling-stroke')
         text = ET.SubElement(svg, 'text')
         text.set('x', fmt(x0))
         text.set('y', fmt(baseline+tick+100))
@@ -114,15 +116,15 @@
         text.set('font-size', txtsize)
         text.set('text-anchor', 'middle')
         text.set('alignment-baseline', 'top')
         text.text = str(int(xadvance))
 
         # Glyph Outline
         g = self.glyph.svgpath(x0=x0, y0=baseline,
-                               scale=1./self.glyph.emscale)  # type: ignore
+                               scale_factor=1/self.glyph._points_per_unit)  # type: ignore
         if g is not None:
             g.set('fill', 'lightgray')
             g.set('stroke', 'black')
             g.set('stroke-width', '2px')
             g.set('vector-effect', 'non-scaling-stroke')
             svg.append(g)
 
@@ -220,75 +222,75 @@
         for i in range(self.font.info.header.numglyphs):
             glyph = self.font.glyph_fromid(i)
             if x + glyph.advance() * scale > self.pxwidth:
                 y += lineheight
                 x = 0
             if x == 0 and glyph.bbox.xmin < 0:
                 x = glyph.bbox.xmin * scale
-            g = glyph.svgpath(x0=x, y0=y, scale=self.size/glyph.dfltsize)
+            g = glyph.svgpath(x0=x, y0=y, scale_factor=self.size/glyph.DFLT_SIZE_PT)
             if g is not None:
                 svg.append(g)
             x += glyph.advance() * scale
 
         height = y + lineheight/2
         svg.set('viewBox', f'0 0 {fmt(self.pxwidth)} {fmt(height)}')
         svg.set('height', fmt(height))
         return svg
 
-    
-    
+
 class ShowLookup4:
+    ''' Show items in Lookup Table type 4 '''
     def __init__(self, lookup, font, size: float=36, pxwidth: int=400):
         self.lookup = lookup
         self.font = font
         self.size = size
         self.pxwidth = pxwidth
         self.linespacing = 1.25
-    
+
     def _repr_svg_(self):
         ''' Jupyter representation '''
         return self.svg()
 
     def svg(self) -> str:
         ''' Glyph SVG string '''
         return ET.tostring(self.svgxml(), encoding='unicode')
 
     def svgxml(self) -> ET.Element:
+        ''' Get SVG as XML tree '''
         lineheight = self.size * self.linespacing
         scale = self.size / self.font.info.layout.unitsperem
 
         svg = ET.Element('svg')
         svg.set('xmlns', 'http://www.w3.org/2000/svg')
         svg.set('width', fmt(self.pxwidth))
 
         y = lineheight
-        
         for subtable in self.lookup.subtables:
             assert subtable.covtable.format == 1
             for covidx, startglyph in enumerate(subtable.covtable.glyphs):
                 ligset = subtable.ligsets[covidx]
                 for nextglyphs, repl in ligset.items():
                     origglyphs = [startglyph] + list(nextglyphs)
 
                     x = 0
                     for gid in origglyphs:
                         glyph = self.font.glyph_fromid(gid)
-                        g = glyph.svgpath(x0=x, y0=y, scale=self.size/glyph.dfltsize)
+                        g = glyph.svgpath(x0=x, y0=y, scale_factor=self.size/glyph.DFLT_SIZE_PT)
                         if g is not None:
                             svg.append(g)
                         x += glyph.advance() * scale
                     x += 20
                     glyph = self.font.glyph('-')
                     svg.append(glyph.svgpath(x0=x, y0=y,
-                                             scale=self.size/glyph.dfltsize))
+                                             scale_factor=self.size/glyph.DFLT_SIZE_PT))
                     x += glyph.advance() * scale
                     x += 20
 
                     glyph = self.font.glyph_fromid(repl)
-                    g = glyph.svgpath(x0=x, y0=y, scale=self.size/glyph.dfltsize)
+                    g = glyph.svgpath(x0=x, y0=y, scale_factor=self.size/glyph.DFLT_SIZE_PT)
                     g.set('fill', 'red')
                     svg.append(g)
                     y += lineheight
 
         svg.set('viewBox', f'0 0 {fmt(self.pxwidth)} {fmt(y + lineheight/2)}')
         svg.set('height', fmt(y + lineheight/2))
-        return svg
+        return svg
```

### Comparing `ziafont-0.5/ziafont/gpos.py` & `ziafont-0.6/ziafont/gpos.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.vermajor = self.fontfile.readuint16()
         self.verminor = self.fontfile.readuint16()
         scriptofst = self.fontfile.readuint16()
         featureofst = self.fontfile.readuint16()
         lookupofst = self.fontfile.readuint16()
         if self.verminor > 0:
             self.variationofst = self.fontfile.readuint32()
-            logging.warn('GPOS has feature variations - unimplemented')
+            logging.warning('GPOS has feature variations - unimplemented')
 
         # Read scripts
         scriptlisttableloc = self.ofst + scriptofst
         scriptcnt = self.fontfile.readuint16(scriptlisttableloc)
         self.scripts = {}
         for i in range(scriptcnt):
             tag = self.fontfile.read(4).decode()
@@ -94,22 +94,23 @@
         ''' Return dx, dy postition wrt original mark position '''
         features = self.features_active()
         for feat in ['mark', 'mkmk']:
             if feat in features:
                 for lookup in features[feat]:
                     for subtable in lookup.subtables:
                         if not hasattr(subtable, 'anchor'):
-                            logging.debug(f'skipping unimplemented placemark subtable {subtable}')
+                            logging.debug('skipping unimplemented placemark subtable %s', subtable)
                             continue
 
                         anchors = subtable.anchor(base, mark)
                         if anchors is not None:
                             dx = anchors.base.x - anchors.mark.x
                             dy = anchors.base.y - anchors.mark.y
-                            logging.debug(f'Positioning Mark {mark} on {base}: ({dx}, {dy})')
+                            logging.debug('Positioning Mark %s on %s: (%s, %s)',
+                                          mark, base, dx, dy)
                             mkmk = isinstance(subtable, MarkToMarkSubtable)
                             return PlaceMark(dx, dy, mkmk)   # Use first one found
         return None
 
     def __repr__(self):
         return f'<GPOS Table v{self.vermajor}.{self.verminor}>'
 
@@ -135,15 +136,17 @@
         self.tableofsts = []
         for i in range(subtablecnt):
             self.tableofsts.append(self.fontfile.readuint16())
         self.markfilterset = None
         if self.flag & USE_MARK_FILTERING_SET:
             self.markfilterset = self.fontfile.readuint16()
 
-        self.subtables: list[Union[PairAdjustmentSubtable, MarkToBaseSubtable, MarkToMarkSubtable]] = []
+        self.subtables: list[Union[PairAdjustmentSubtable,
+                                   MarkToBaseSubtable,
+                                   MarkToMarkSubtable]] = []
         for tblofst in self.tableofsts:
             if self.type == 9:  # Extension table - converts to another type
                 fmt = self.fontfile.readuint16(self.ofst + tblofst)
                 assert fmt == 1
                 self.type = self.fontfile.readuint16()
                 tblofst += self.fontfile.readuint32()
 
@@ -153,15 +156,15 @@
             elif self.type == 4:  # Mark-to-base
                 self.subtables.append(MarkToBaseSubtable(
                         tblofst + self.ofst, self.fontfile))
             elif self.type == 6:  # Mark-to-mark
                 self.subtables.append(MarkToMarkSubtable(
                         tblofst + self.ofst, self.fontfile))
             else:
-                logging.debug(f'Unimplemented GPOS Lookup Type {self.type}')
+                logging.debug('Unimplemented GPOS Lookup Type %s', self.type)
 
         self.fontfile.seek(fileptr)  # Put file pointer back
 
     def __repr__(self):
         return f'<GPOSLookup Type {self.type} {hex(self.ofst)}>'
 
 
@@ -248,28 +251,30 @@
         return v1, v2
 
     def __repr__(self):
         return f'<PairAdjustmentSubtable {hex(self.ofst)}>'
 
 
 def read_markarray_table(ofst, fontfile):
+    ''' Read MarkArray table from font file '''
     cnt = fontfile.readuint16(ofst)
     MarkRecord = namedtuple('MarkRecord', ['markclass', 'anchortable'])
     markrecords = []
     for i in range(cnt):
         markclass = fontfile.readuint16()
         anchorofst = fontfile.readuint16()
         ptr = fontfile.tell()
         anchortable = read_anchortable(ofst+anchorofst, fontfile)
         markrecords.append(MarkRecord(markclass, anchortable))
         ptr = fontfile.seek(ptr)
     return markrecords
 
 
 def read_anchortable(ofst, fontfile):
+    ''' Read anchor table from font file '''
     Anchor = namedtuple('Anchor', ['x', 'y', 'anchorpoint', 'xofst', 'yofst'])
     fmt = fontfile.readuint16(ofst)
     point = None
     xofst = yofst = None
     x = fontfile.readint16()
     y = fontfile.readint16()
     if fmt == 2:
```

### Comparing `ziafont-0.5/ziafont/gsub.py` & `ziafont-0.6/ziafont/gsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 
 
 ChainedSeqRule = namedtuple('ChainedSeqRule', ['backtrack', 'input', 'lookahead', 'sequence'])
 SequenceLookupRecord = namedtuple('SequenceLookupRecord', ['sequenceindex', 'lookupindex'])
 
 
 class LookupSubtable:
-    ''' Generic/unimplemented GSBU Lookup Sub Table '''
+    ''' Generic/unimplemented GSUB Lookup Sub Table '''
     def __init__(self, ofst: int, fontfile: FontReader):
         self.ofst = ofst
         self.fontfile = fontfile
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
-        logging.debug(f'Glyph substitution from unimplemented GSUB subtable type {self.ofst}')
+        logging.debug('Glyph substitution from unimplemented GSUB subtable type %s', self.ofst)
         return glyphids
 
 
 class LookupSingleSub1(LookupSubtable):
     ''' GSUB Single Glyph Substitution  (LookupType 1, format 1) '''
     def __init__(self, ofst: int, fontfile: FontReader):
         super().__init__(ofst, fontfile)
         self.fmt = fontfile.readuint16(ofst)
         assert self.fmt == 1
         covofst = fontfile.readuint16()
         self.deltagid = fontfile.readint16()
         self.covtable = Coverage(ofst + covofst, fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         for i in range(len(glyphids)):
             covidx = self.covtable.covidx(glyphids[i])
             if covidx is not None:
                 glyphids[i] += self.deltagid
         return glyphids
 
@@ -87,15 +87,15 @@
             subglyphs = []
             for _ in range(glyphcnt):
                 subglyphs.append(fontfile.readuint16())
             self.subglyphids.append(subglyphs)
 
         self.covtable = Coverage(ofst + covofst, fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         newglyphids = []
         for gid in glyphids:
             covidx = self.covtable.covidx(gid)
             if covidx is not None:
                 newglyphids.extend(self.subglyphids[covidx])
             else:
@@ -119,26 +119,26 @@
             cnt = self.fontfile.readuint16(ofst+altofst)
             gids = []
             for i in range(cnt):
                 gids.append(self.fontfile.readuint16())
             self.altglyphs.append(gids)
         self.covtable = Coverage(ofst + covofst, fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         for i in range(len(glyphids)):
             covidx = self.covtable.covidx(glyphids[i])
             if covidx is not None:
 
                 if name == 'rand':
                     glyphids[i] = random.choice(self.altglyphs[covidx])
                 else:
-                    # TODO - user choice!
-                    altgids = ', '.join(str(c) for c in self.altglyphs[covidx])
-                    logging.debug(f'Alternate glyphs for id {glyphids[i]}: {altgids}')
+                    altgids = self.altglyphs[covidx]
+                    # TODO - user choice! return first one for now.
+                    glyphids[i] = altgids[0]
 
         return glyphids
 
 
 class LookupLigatureSub(LookupSubtable):
     ''' Ligature Substitution Subtable (LookupType 4) '''
     def __init__(self, ofst: int, fontfile: FontReader):
@@ -168,15 +168,15 @@
                 compglyphs = []
                 for _ in range(compcount-1):
                     compglyphs.append(self.fontfile.readuint16())
                 ligs[tuple(compglyphs)] = ligglyph
             self.ligsets.append(ligs)
         self.covtable = Coverage(self.ofst+covofst, self.fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         newgids = []
         i = 0
         while i < len(glyphids):
             gid = glyphids[i]
             covidx = self.covtable.covidx(gid)
             if covidx is not None:
@@ -229,15 +229,15 @@
         self.inptCoverage = []
         for iofst in inptofsts:
             self.inptCoverage.append(Coverage(self.ofst+iofst, self.fontfile))
         self.lookaheadCoverage = []
         for lofst in lookofsts:
             self.lookaheadCoverage.append(Coverage(self.ofst+lofst, self.fontfile))
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         ilen = len(self.inptCoverage)
         i = len(self.backCoverage)
         while i < len(glyphids) - len(self.lookaheadCoverage) - ilen + 1:
             covidx = [cov.covidx(glyphids[i+k]) for k, cov in enumerate(self.inptCoverage)]
             if None in covidx:
                 i += 1
@@ -310,33 +310,36 @@
                     ChainedSeqRule(backseq, inputseq, lookaheadseq, sequencelookup))
             self.rules.append(ruleset)
         self.covtable = Coverage(self.ofst+covofst, self.fontfile)
         self.backtrackClass = ClassDef(self.ofst+backtrackofst, self.fontfile)
         self.inputClass = ClassDef(self.ofst+inputofst, self.fontfile)
         self.lookaheadClass = ClassDef(self.ofst+lookaheadofst, self.fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         i = 0
         while i < len(glyphids):
             gid = glyphids[i]
             covidx = self.covtable.covidx(gid)
             if covidx is not None:
                 classid = self.inputClass.get_class(gid)
                 if classid is not None:
                     ruleset = self.rules[classid]
                     for rule in ruleset:
-                        inpt = [self.inputClass.get_class(g) for g in glyphids[i+1:i+1+len(rule.input)]]
+                        inpt = [self.inputClass.get_class(g)
+                                for g in glyphids[i+1:i+1+len(rule.input)]]
                         if inpt != rule.input:
                             continue
-                        backtrack = [self.backtrackClass.get_class(g) for g in glyphids[i-len(rule.backtrack):i]]
+                        backtrack = [self.backtrackClass.get_class(g)
+                                     for g in glyphids[i-len(rule.backtrack):i]]
                         if backtrack[::-1] != rule.backtrack:  # Rule is reverse order
                             continue
                         aheadlen = len(rule.input) + len(rule.lookahead)
-                        lookahead = [self.lookaheadClass.get_class(g) for g in glyphids[i+1+len(rule.input):i+1+aheadlen]]
+                        lookahead = [self.lookaheadClass.get_class(g)
+                                     for g in glyphids[i+1+len(rule.input):i+1+aheadlen]]
 
                         if lookahead != rule.lookahead:
                             continue
 
                         # Match
                         for seqlookup in rule.sequence:
                             glyphids[i+seqlookup.sequenceindex:i+1+len(rule.input)] = \
@@ -388,15 +391,15 @@
                         self.fontfile.readuint16(),   # SequenceIndex
                         self.fontfile.readuint16()))  # LookupListIndex
                 ruleset.append(ChainedSeqRule(
                     backtrackSeq, inputSequence, lookaheadSequence, sequencelookup))
             self.rules.append(ruleset)
         self.covtable = Coverage(self.ofst+covofst, self.fontfile)
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         i = 0
         while i < len(glyphids):
             gid = glyphids[i]
             covidx = self.covtable.covidx(gid)
             if covidx is not None:
                 ruleset = self.rules[covidx]
@@ -447,15 +450,15 @@
         subtablecnt = self.fontfile.readuint16()
         self.tableofsts = []
         for i in range(subtablecnt):
             self.tableofsts.append(self.fontfile.readuint16())
         self.markfilterset = None
         if self.flag & USE_MARK_FILTERING_SET:
             self.markfilterset = self.fontfile.readuint16()
-            
+
         self.subtables: list[LookupSubtable] = []
         for i in range(subtablecnt):
             tblofst = self.ofst+self.tableofsts[i]
             self.fmt = self.fontfile.readuint16(tblofst)
             if self.type == 7:  # Extension Table - turns into another type
                 self.type = self.fontfile.readuint16()
                 extofst = self.fontfile.readuint32()
@@ -469,35 +472,35 @@
                     self.subtables.append(LookupSingleSub2(tblofst, self.fontfile))
 
             elif self.type == 2:  # Multiple sub
                 self.subtables.append(LookupMultipleSub(tblofst, self.fontfile))
 
             elif self.type == 3:  # Alternates lookup
                 self.subtables.append(LookupAlternate(tblofst, self.fontfile))
-                    
+
             elif self.type == 4:  # Ligature sub
                 self.subtables.append(LookupLigatureSub(tblofst, self.fontfile))
 
             elif self.type == 6:  # Chained context sub
                 if self.fmt == 1:
                     self.subtables.append(LookupChainedSub1(tblofst, self.fontfile))
                 elif self.fmt == 2:
                     self.subtables.append(LookupChainedSub2(tblofst, self.fontfile))
                 else:
                     self.subtables.append(LookupChainedSub3(tblofst, self.fontfile))
             else:
-                logging.debug(f'Unimplemented GSUB Lookup Type {self.type}')
+                logging.debug('Unimplemented GSUB Lookup Type %s', self.type)
                 self.subtables.append(LookupSubtable(self.type, self.fontfile))
 
         self.fontfile.seek(fileptr)
 
     def __repr__(self):
         return f'<GSUBLookup Type {self.type}.{self.fmt}>'
 
-    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str=None) -> list[int]:
+    def sub(self, glyphids: list[int], lookups: list[GSUBLookup], name: str = None) -> list[int]:
         ''' Apply glyph substitution to list of glyph ids '''
         for subtable in self.subtables:
             glyphids = subtable.sub(glyphids, lookups, name)
         return glyphids
 
 
 class Gsub:
@@ -511,15 +514,15 @@
         verminor = self.fontfile.readuint16()
         scriptofst = self.fontfile.readuint16()
         featureofst = self.fontfile.readuint16()
         lookupofst = self.fontfile.readuint16()
         featurevariationsofst = None
         if verminor == 1:
             featurevariationsofst = self.fontfile.readuint32()
-            logging.warn('GSUB has feature variations - unimplemented')
+            logging.warning('GSUB has feature variations - unimplemented')
 
         # Read scripts
         scriptlisttableloc = self.ofst + scriptofst
         scriptcnt = self.fontfile.readuint16(scriptlisttableloc)
         self.scripts = {}
         for i in range(scriptcnt):
             tag = self.fontfile.read(4).decode()
@@ -567,20 +570,21 @@
         return self.features.get(self.language.script, {}).get(self.language.language, {})
 
     def sub(self, glyphids: list[int], features: FontFeatures):
         ''' Apply glyph substitution to list of glyph ids. Features
             enable/disable certain substitutions.
         '''
         feattable = self.features_active()
+        
         def apply_feature(name, glyphids):
             tables = feattable.get(name, [])
             for table in tables:
                 newglyphids = table.sub(glyphids.copy(), self.lookups, name)
                 if newglyphids != glyphids:
-                    logging.debug(f'GSUB applied by feature {name} in {table}')
+                    logging.debug('GSUB applied by feature %s in %s', name, table)
                 glyphids = newglyphids
             return glyphids
 
         basicfeatures = ['locl', 'ccmp', 'rlig']
         altfeatures = ['rclt', 'rand']
         if features.calt:
             altfeatures.append('calt')
@@ -596,14 +600,16 @@
             altfeatures.append('frac')
         if features.salt:
             altfeatures.append('salt')
         if features.hlig:
             altfeatures.append('hlig')
         if features.zero:
             altfeatures.append('zero')
+        if features.ssty:
+            altfeatures.append('ssty')
 
         # Run basic features first, in order defined by font
         for feat in feattable.keys():
             if feat in basicfeatures:
                 glyphids = apply_feature(feat, glyphids)
 
         # Then alernate/optional features, in order defined by font
```

### Comparing `ziafont-0.5/ziafont/svgpath.py` & `ziafont-0.6/ziafont/svgpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     def __truediv__(self, i):
         return Point(self.x / i, self.y / i)
 
     def xform(self, a: float, b: float, c: float, d: float,
               e: float, f: float, m: float, n: float) -> Point:
         ''' Apply Transform (for compound glyph) '''
-        x = m * a/m * self.x + c/m * self.y + e
-        y = n * b/n * self.x + d/n * self.y + f
+        x = m * (a/m * self.x + c/m * self.y + e)
+        y = n * (b/n * self.x + d/n * self.y + f)
         return Point(x, y)
 
 
 class Moveto:
     ''' SVG Move To '''
     def __init__(self, p: Point):
         self.p = p
@@ -124,15 +124,16 @@
         self.p2 = p2
 
     def __repr__(self):
         return f'Quad({self.p1.x}, {self.p1.y}; {self.p2.x} {self.p2.y})'
 
     def path(self, x0: float = 0, y0: float = 0, scale: float = 1) -> str:
         ''' Get SVG path '''
-        return f'Q {fmt(x0 + self.p1.x * scale)} {fmt(y0-self.p1.y * scale)} {fmt(x0+self.p2.x * scale)} {fmt(y0-self.p2.y * scale)} '
+        return (f'Q {fmt(x0 + self.p1.x * scale)} {fmt(y0-self.p1.y * scale)} '
+                f'{fmt(x0+self.p2.x * scale)} {fmt(y0-self.p2.y * scale)} ')
 
     def xform(self, a: float, b: float, c: float, d: float,
               e: float, f: float, m: float, n: float) -> Quad:
         ''' Transform the SVG path '''
         return Quad(self.p1.xform(a, b, c, d, e, f, m, n),
                     self.p2.xform(a, b, c, d, e, f, m, n))
 
@@ -168,15 +169,17 @@
         self.p3 = p3
 
     def __repr__(self):
         return f'Cubic({self.p1.x}, {self.p1.y}; {self.p2.x}, {self.p2.y}; {self.p3.x} {self.p3.y})'
 
     def path(self, x0: float = 0, y0: float = 0, scale: float = 1) -> str:
         ''' Get SVG path '''
-        return f'C {fmt(x0+self.p1.x * scale)} {fmt(y0-self.p1.y * scale)} {fmt(x0+self.p2.x * scale)} {fmt(y0-self.p2.y * scale)} {fmt(x0+self.p3.x * scale)} {fmt(y0-self.p3.y * scale)} '
+        return (f'C {fmt(x0+self.p1.x * scale)} {fmt(y0-self.p1.y * scale)} '
+                f'{fmt(x0+self.p2.x * scale)} {fmt(y0-self.p2.y * scale)} '
+                f'{fmt(x0+self.p3.x * scale)} {fmt(y0-self.p3.y * scale)} ')
 
     def xform(self, a: float, b: float, c: float, d: float,
               e: float, f: float, m: float, n: float) -> Cubic:
         ''' Transform the SVG path '''
         return Cubic(self.p1.xform(a, b, c, d, e, f, m, n),
                      self.p2.xform(a, b, c, d, e, f, m, n),
                      self.p3.xform(a, b, c, d, e, f, m, n))
```

### Comparing `ziafont-0.5/ziafont/tables.py` & `ziafont-0.6/ziafont/tables.py`

 * *Files identical despite different names*

### Comparing `ziafont-0.5/ziafont.egg-info/SOURCES.txt` & `ziafont-0.6/ziafont.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 README.md
-setup.py
+pyproject.toml
+setup.cfg
 ziafont/__init__.py
 ziafont/cmap.py
 ziafont/config.py
 ziafont/font.py
 ziafont/fontread.py
 ziafont/fonttypes.py
 ziafont/glyph.py
```

