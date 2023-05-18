# Comparing `tmp/pygments-ansi-color-0.2.0.tar.gz` & `tmp/pygments-ansi-color-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments-ansi-color-0.2.0.tar", last modified: Wed Feb 22 19:04:07 2023, max compression
+gzip compressed data, was "pygments-ansi-color-0.3.0.tar", last modified: Thu May 18 22:44:10 2023, max compression
```

## Comparing `pygments-ansi-color-0.2.0.tar` & `pygments-ansi-color-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-02-22 19:04:07.579060 pygments-ansi-color-0.2.0/
--rw-r--r--   0 ckuehl    (3119) users      (100)      552 2018-02-01 19:03:51.000000 pygments-ansi-color-0.2.0/LICENSE
--rw-r--r--   0 ckuehl    (3119) users      (100)      501 2023-02-22 19:04:07.579060 pygments-ansi-color-0.2.0/PKG-INFO
--rw-r--r--   0 ckuehl    (3119) users      (100)     4653 2023-02-22 19:02:35.000000 pygments-ansi-color-0.2.0/README.md
-drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-02-22 19:04:07.579060 pygments-ansi-color-0.2.0/pygments_ansi_color/
--rw-r--r--   0 ckuehl    (3119) users      (100)    10704 2023-02-22 19:02:35.000000 pygments-ansi-color-0.2.0/pygments_ansi_color/__init__.py
--rw-r--r--   0 ckuehl    (3119) users      (100)        0 2023-02-22 19:01:57.000000 pygments-ansi-color-0.2.0/pygments_ansi_color/py.typed
-drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-02-22 19:04:07.579060 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/
--rw-r--r--   0 ckuehl    (3119) users      (100)      501 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/PKG-INFO
--rw-r--r--   0 ckuehl    (3119) users      (100)      347 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/SOURCES.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)        1 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/dependency_links.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       67 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/entry_points.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       16 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/requires.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       20 2023-02-22 19:04:07.000000 pygments-ansi-color-0.2.0/pygments_ansi_color.egg-info/top_level.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       38 2023-02-22 19:04:07.579060 pygments-ansi-color-0.2.0/setup.cfg
--rw-r--r--   0 ckuehl    (3119) users      (100)      769 2023-02-22 19:03:18.000000 pygments-ansi-color-0.2.0/setup.py
+drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2023-05-18 22:44:10.293005 pygments-ansi-color-0.3.0/
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      552 2017-09-12 07:06:01.000000 pygments-ansi-color-0.3.0/LICENSE
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      471 2023-05-18 22:44:10.293005 pygments-ansi-color-0.3.0/PKG-INFO
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     6045 2023-05-18 22:43:09.000000 pygments-ansi-color-0.3.0/README.md
+drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2023-05-18 22:44:10.293005 pygments-ansi-color-0.3.0/pygments_ansi_color/
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)    11301 2023-05-18 22:43:09.000000 pygments-ansi-color-0.3.0/pygments_ansi_color/__init__.py
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)        0 2022-09-13 23:40:01.000000 pygments-ansi-color-0.3.0/pygments_ansi_color/py.typed
+drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2023-05-18 22:44:10.293005 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      471 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/PKG-INFO
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      347 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)        1 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       66 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/entry_points.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       16 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/requires.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       20 2023-05-18 22:44:10.000000 pygments-ansi-color-0.3.0/pygments_ansi_color.egg-info/top_level.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       38 2023-05-18 22:44:10.293005 pygments-ansi-color-0.3.0/setup.cfg
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      819 2023-05-18 22:43:42.000000 pygments-ansi-color-0.3.0/setup.py
```

### Comparing `pygments-ansi-color-0.2.0/LICENSE` & `pygments-ansi-color-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments-ansi-color-0.2.0/README.md` & `pygments-ansi-color-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,117 @@
 pygments-ansi-color
---------
+-------------------
 
 [![Build Status](https://travis-ci.org/chriskuehl/pygments-ansi-color.svg?branch=master)](https://travis-ci.org/chriskuehl/pygments-ansi-color)
 [![Coverage Status](https://coveralls.io/repos/github/chriskuehl/pygments-ansi-color/badge.svg?branch=master)](https://coveralls.io/github/chriskuehl/pygments-ansi-color?branch=master)
 [![PyPI version](https://badge.fury.io/py/pygments-ansi-color.svg)](https://pypi.python.org/pypi/pygments-ansi-color)
 
 An ANSI color-code highlighting lexer for Pygments.
 
 ![](https://i.fluffy.cc/nHPkL3gfBtj5Kt4H3RR51T9TJLh6rtv2.png)
 
 
-### Usage
+### Basic usage
 
-1. `pip install pygments-ansi-color`
+1. Install `pygments-ansi-color`:
 
-2. Configure your Pygments style with the appropriate color tokens. It's
-   necessary to add additional tokens because existing Pygments lexers are
-   built around contextual tokens (think "Comment" or "String") rather than
-   actual colors.
+   ```shell-session
+   $ pip install pygments-ansi-color
+   ```
 
-   In the case of ANSI escape sequences, colors have no context beyond the
-   color themselves; we'd always want a "red" rendered as "red", regardless of
-   your particular theme.
+2. `pygments-ansi-color` is not magic (yet?), so you need to [choose an exising
+   Pygments style](https://pygments.org/styles/), which will be used as a base
+   for your own style.
+
+   For example, let's choose `pygments.styles.xcode.XcodeStyle`, which looks
+   great to use. And then we will augment this reference style with
+   `pygments-ansi-color`'s color tokens thanks to the `color_tokens` function,
+   to make our final `MyStyle` custom style.
 
-   Here's an example:
+   Here is how the code looks like:
 
    ```python
    from pygments_ansi_color import color_tokens
 
-   # Note: You can use different background colors for improved readability.
-   fg_colors = bg_colors = {
-       'Black': '#000000',
-       'Red': '#EF2929',
-       'Green': '#8AE234',
-       'Yellow': '#FCE94F',
-       'Blue': '#3465A4',
-       'Magenta': '#c509c5',
-       'Cyan': '#34E2E2',
-       'White': '#F5F5F5',
-       'BrightBlack': '#676767',
-       'BrightRed': '#FF6D67',
-       'BrightGreen': '#5FF967',
-       'BrightYellow': '#FEFB67',
-       'BrightBlue': '#6871FF',
-       'BrightMagenta': '#FF76FF',
-       'BrightCyan': '#5FFDFF',
-       'BrightWhite': '#FEFFFF',
-   }
    class MyStyle(pygments.styles.xcode.XcodeStyle):
        styles = dict(pygments.styles.xcode.XcodeStyle.styles)
-       styles.update(color_tokens(fg_colors, bg_colors))
+       styles.update(color_tokens())
    ```
 
-3. Render your code!
+   That's all the custom code you need to integrate with `pygments-ansi-color`.
+
+3. Now you can highlight your content with the dedicated ANSI lexer and your
+   custom style, with the Pygments regular API:
 
    ```python
    import pygments
    import pygments.formatters
    import pygments.lexers
 
    lexer = pygments.lexers.get_lexer_by_name('ansi-color')
    formatter = pygments.formatters.HtmlFormatter(style=MyStyle)
    print(pygments.highlight('your text', lexer, formatter))
    ```
 
+### Design
+
+We had to configure above a custom Pygments style with the appropriate color
+tokens. That's because existing Pygments lexers are built around contextual
+tokens (think `Comment` or `Punctuation`) rather than actual colors.
+
+In the case of ANSI escape sequences, colors have no context beyond the color
+themselves; we'd always want a `red` rendered as `red`, regardless of your
+particular theme.
+
+
+### Custom theme
+
+By default, `pygments-ansi-color` maps ANSI codes to its own set of colors.
+They have been carefully crafted for readability, and are [loosely based on the
+color scheme used by iTerm2
+](https://github.com/chriskuehl/pygments-ansi-color/pull/27#discussion_r1113790011).
+
+Default colors are hard-coded by the `pygments_ansi_color.DEFAULT_STYLE`
+constant as such:
+- `Black`: `#000000`
+- `Red`: `#ef2929`
+- `Green`: `#8ae234`
+- `Yellow`: `#fce94f`
+- `Blue`: `#3465a4`
+- `Magenta`: `#c509c5`
+- `Cyan`: `#34e2e2`
+- `White`: `#f5f5f5`
+- `BrightBlack`: `#676767`
+- `BrightRed`: `#ff6d67`
+- `BrightGreen`: `#5ff967`
+- `BrightYellow`: `#fefb67`
+- `BrightBlue`: `#6871ff`
+- `BrightMagenta`: `#ff76ff`
+- `BrightCyan`: `#5ffdff`
+- `BrightWhite`: `#feffff`
+
+Still, you may want to use your own colors, to tweak the rendering to your
+background color, or to match your own theme.
+
+For that you can override each color individually, by passing them as
+arguments to the `color_tokens` function:
+
+```python
+from pygments_ansi_color import color_tokens
+
+class MyStyle(pygments.styles.xcode.XcodeStyle):
+   styles = dict(pygments.styles.xcode.XcodeStyle.styles)
+   styles.update(color_tokens(
+      fg_colors={'Cyan': '#00ffff', 'BrightCyan': '#00ffff'},
+      bg_colors={'BrightWhite': '#000000'},
+   ))
+```
+
 
-### Example
+### Used by
 
 You can see an example [on fluffy][fluffy-example], the project that this lexer
 was originally developed for.
 
 The colors are defined as part of your Pygments style and can be changed.
 
 
@@ -97,15 +139,15 @@
 you need only 1 + 265 + 265 = 531 CSS classes to support all possibilities.
 
 If you'd like to enable 256-color support, you'll need to do two things:
 
 1. When calling `color_tokens`, pass `enable_256color=True`:
 
    ```python
-   styles.update(color_tokens(fg_colors, bg_colors, enable_256color=True))
+   styles.update(color_tokens(enable_256color=True))
    ```
 
    This change is what causes your CSS to have the appropriate classes in it.
 
 2. When constructing your formatter, use the `ExtendedColorHtmlFormatterMixin`
    mixin, like this:
```

### Comparing `pygments-ansi-color-0.2.0/pygments_ansi_color/__init__.py` & `pygments-ansi-color-0.3.0/pygments_ansi_color/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,17 +91,37 @@
     else:
         token = Color
         for component in components:
             token = getattr(token, component)
         return token
 
 
+DEFAULT_STYLE = {
+    'Black': '#000000',
+    'Red': '#ef2929',
+    'Green': '#8ae234',
+    'Yellow': '#fce94f',
+    'Blue': '#3465a4',
+    'Magenta': '#c509c5',
+    'Cyan': '#34e2e2',
+    'White': '#f5f5f5',
+    'BrightBlack': '#676767',
+    'BrightRed': '#ff6d67',
+    'BrightGreen': '#5ff967',
+    'BrightYellow': '#fefb67',
+    'BrightBlue': '#6871ff',
+    'BrightMagenta': '#ff76ff',
+    'BrightCyan': '#5ffdff',
+    'BrightWhite': '#feffff',
+}
+
+
 def color_tokens(
-    fg_colors: dict[str, str],
-    bg_colors: dict[str, str],
+    fg_colors: dict[str, str] = DEFAULT_STYLE,
+    bg_colors: dict[str, str] = DEFAULT_STYLE,
     enable_256color: bool = False,
 ) -> dict[pygments.token._TokenType, str]:
     """Return color tokens for a given set of colors.
 
     Pygments doesn't have a generic "color" token; instead everything is
     contextual (e.g. "comment" or "variable"). That doesn't make sense for us,
     where the colors actually *are* what we care about.
@@ -118,38 +138,39 @@
     but enable the use of 256-color in text. The reason this is optional and
     non-default is that it requires patching the Pygments formatter you're
     using, using the ExtendedColorHtmlFormatterMixin provided by this file.
     For more details on why and how, see the README.
 
     Usage:
 
-        fg_colors = bg_colors = {
-            'Black': '#000000',
-            'Red': '#EF2929',
-            'Green': '#8AE234',
-            'Yellow': '#FCE94F',
-            'Blue': '#3465A4',
-            'Magenta': '#c509c5',
-            'Cyan': '#34E2E2',
-            'White': '#F5F5F5',
-            'BrightBlack': '#676767',
-            'BrightRed': '#FF6D67',
-            'BrightGreen': '#5FF967',
-            'BrightYellow': '#FEFB67',
-            'BrightBlue': '#6871FF',
-            'BrightMagenta': '#FF76FF',
-            'BrightCyan': '#5FFDFF',
-            'BrightWhite': '#FEFFFF',
-        }
-        class MyStyle(pygments.styles.SomeStyle):
-            styles = dict(pygments.styles.SomeStyle.styles)
-            styles.update(color_tokens(fg_colors, bg_colors))
+        .. code-block:: python
+            from pygments_ansi_color import color_tokens
+
+            class MyStyle(pygments.styles.SomeStyle):
+                styles = dict(pygments.styles.SomeStyle.styles)
+                styles.update(color_tokens())
     """
     styles: dict[pygments.token._TokenType, str] = {}
 
+    # Validates custom color IDs.
+    if not set(fg_colors).issubset(DEFAULT_STYLE):  # pragma: no cover (trivial)
+        raise ValueError(
+            f'Unrecognized {set(fg_colors).difference(DEFAULT_STYLE)}'
+            ' foreground color',
+        )
+    if not set(bg_colors).issubset(DEFAULT_STYLE):  # pragma: no cover (trivial)
+        raise ValueError(
+            f'Unrecognized {set(bg_colors).difference(DEFAULT_STYLE)}'
+            ' background color',
+        )
+
+    # Merge the default colors with the user-provided colors.
+    fg_colors = {**DEFAULT_STYLE, **fg_colors}
+    bg_colors = {**DEFAULT_STYLE, **bg_colors}
+
     if enable_256color:
         styles[pygments.token.Token.C.Bold] = 'bold'
         styles[pygments.token.Token.C.Faint] = ''
         for i, color in _256_colors.items():
             styles[getattr(pygments.token.Token.C, f'C{i}')] = color
             styles[getattr(pygments.token.Token.C, f'BGC{i}')] = f'bg:{color}'
```

### Comparing `pygments-ansi-color-0.2.0/setup.py` & `pygments-ansi-color-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from setuptools import setup
 
 
 setup(
     name='pygments-ansi-color',
-    version='0.2.0',
+    version='0.3.0',
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.7',
     install_requires=['pygments!=2.7.3'],
     packages=['pygments_ansi_color'],
     package_data={
         'pygments_ansi_color': ['py.typed'],
     },
```

