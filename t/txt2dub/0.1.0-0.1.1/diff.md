# Comparing `tmp/txt2dub-0.1.0.tar.gz` & `tmp/txt2dub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2dub-0.1.0.tar", max compression
+gzip compressed data, was "txt2dub-0.1.1.tar", max compression
```

## Comparing `txt2dub-0.1.0.tar` & `txt2dub-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1085 2023-05-06 01:45:13.483547 txt2dub-0.1.0/LICENSE
--rw-r--r--   0        0        0      552 2023-05-18 14:24:43.459741 txt2dub-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2134 2023-05-18 14:24:43.457743 txt2dub-0.1.0/README.md
--rw-r--r--   0        0        0       22 2023-05-18 14:24:43.460741 txt2dub-0.1.0/txt2dub/__init__.py
--rw-r--r--   0        0        0       28 2023-05-18 14:24:43.461740 txt2dub-0.1.0/txt2dub/__main__.py
--rw-r--r--   0        0        0     6390 2023-05-18 14:24:43.461740 txt2dub-0.1.0/txt2dub/app.py
--rw-r--r--   0        0        0      151 2023-05-18 14:24:43.462739 txt2dub-0.1.0/txt2dub/models/__init__.py
--rw-r--r--   0        0        0      671 2023-05-18 14:24:43.463739 txt2dub-0.1.0/txt2dub/models/base.py
--rw-r--r--   0        0        0     6879 2023-05-18 14:24:43.463739 txt2dub-0.1.0/txt2dub/models/script.py
--rw-r--r--   0        0        0        0 2023-05-09 00:54:47.921658 txt2dub-0.1.0/txt2dub/screens/__init__.py
--rw-r--r--   0        0        0      265 2023-05-18 14:24:43.464738 txt2dub-0.1.0/txt2dub/screens/file/__init__.py
--rw-r--r--   0        0        0     8515 2023-05-18 14:24:43.464738 txt2dub-0.1.0/txt2dub/screens/file/screen.py
--rw-r--r--   0        0        0     1321 2023-05-18 14:24:43.465737 txt2dub-0.1.0/txt2dub/screens/file/widgets.py
--rw-r--r--   0        0        0       62 2023-05-18 14:24:43.465737 txt2dub-0.1.0/txt2dub/screens/script/__init__.py
--rw-r--r--   0        0        0     1470 2023-05-18 14:24:43.466737 txt2dub-0.1.0/txt2dub/screens/script/messages.py
--rw-r--r--   0        0        0    25548 2023-05-18 14:24:43.467736 txt2dub-0.1.0/txt2dub/screens/script/screen.py
--rw-r--r--   0        0        0    16904 2023-05-18 14:24:43.468736 txt2dub-0.1.0/txt2dub/screens/script/widgets.py
--rw-r--r--   0        0        0        0 2023-05-18 14:24:43.468736 txt2dub-0.1.0/txt2dub/services/__init__.py
--rw-r--r--   0        0        0     2076 2023-05-18 14:24:43.469737 txt2dub-0.1.0/txt2dub/services/actions.py
--rw-r--r--   0        0        0     3110 2023-05-18 14:24:43.469737 txt2dub-0.1.0/txt2dub/services/tts.py
--rw-r--r--   0        0        0     5595 2023-05-18 14:24:43.470737 txt2dub-0.1.0/txt2dub/styles/app.css
--rw-r--r--   0        0        0        0 2023-05-18 14:24:43.470737 txt2dub-0.1.0/txt2dub/tts/__init__.py
--rw-r--r--   0        0        0      104 2023-05-18 14:24:43.471736 txt2dub-0.1.0/txt2dub/tts/__main__.py
--rw-r--r--   0        0        0     4971 2023-05-18 14:24:43.471736 txt2dub-0.1.0/txt2dub/tts/interpreter.py
--rw-r--r--   0        0        0        0 2023-05-07 00:47:14.411074 txt2dub-0.1.0/txt2dub/widgets/__init__.py
--rw-r--r--   0        0        0      784 2023-05-18 14:24:43.472735 txt2dub-0.1.0/txt2dub/widgets/base.py
--rw-r--r--   0        0        0      479 2023-05-07 00:51:34.735297 txt2dub-0.1.0/txt2dub/widgets/logo.py
--rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 txt2dub-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-06 01:45:13.483547 txt2dub-0.1.1/LICENSE
+-rw-r--r--   0        0        0      611 2023-05-19 01:48:49.871969 txt2dub-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2891 2023-05-19 01:48:49.866974 txt2dub-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-19 01:48:49.871969 txt2dub-0.1.1/txt2dub/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-18 14:24:43.461740 txt2dub-0.1.1/txt2dub/__main__.py
+-rw-r--r--   0        0        0     6390 2023-05-18 14:24:43.461740 txt2dub-0.1.1/txt2dub/app.py
+-rw-r--r--   0        0        0      151 2023-05-18 14:24:43.462739 txt2dub-0.1.1/txt2dub/models/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-18 14:24:43.463739 txt2dub-0.1.1/txt2dub/models/base.py
+-rw-r--r--   0        0        0     6879 2023-05-18 14:24:43.463739 txt2dub-0.1.1/txt2dub/models/script.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:54:47.921658 txt2dub-0.1.1/txt2dub/screens/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-18 14:24:43.464738 txt2dub-0.1.1/txt2dub/screens/file/__init__.py
+-rw-r--r--   0        0        0     8515 2023-05-18 14:24:43.464738 txt2dub-0.1.1/txt2dub/screens/file/screen.py
+-rw-r--r--   0        0        0     1321 2023-05-18 14:24:43.465737 txt2dub-0.1.1/txt2dub/screens/file/widgets.py
+-rw-r--r--   0        0        0       62 2023-05-18 14:24:43.465737 txt2dub-0.1.1/txt2dub/screens/script/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-18 14:24:43.466737 txt2dub-0.1.1/txt2dub/screens/script/messages.py
+-rw-r--r--   0        0        0    25548 2023-05-18 14:24:43.467736 txt2dub-0.1.1/txt2dub/screens/script/screen.py
+-rw-r--r--   0        0        0    16904 2023-05-18 14:24:43.468736 txt2dub-0.1.1/txt2dub/screens/script/widgets.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:24:43.468736 txt2dub-0.1.1/txt2dub/services/__init__.py
+-rw-r--r--   0        0        0     2076 2023-05-18 14:24:43.469737 txt2dub-0.1.1/txt2dub/services/actions.py
+-rw-r--r--   0        0        0     3110 2023-05-18 14:24:43.469737 txt2dub-0.1.1/txt2dub/services/tts.py
+-rw-r--r--   0        0        0     5690 2023-05-19 01:48:49.872969 txt2dub-0.1.1/txt2dub/styles/app.css
+-rw-r--r--   0        0        0        0 2023-05-18 14:24:43.470737 txt2dub-0.1.1/txt2dub/tts/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-18 14:24:43.471736 txt2dub-0.1.1/txt2dub/tts/__main__.py
+-rw-r--r--   0        0        0     4971 2023-05-18 14:24:43.471736 txt2dub-0.1.1/txt2dub/tts/interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-07 00:47:14.411074 txt2dub-0.1.1/txt2dub/widgets/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-18 14:24:43.472735 txt2dub-0.1.1/txt2dub/widgets/base.py
+-rw-r--r--   0        0        0      479 2023-05-07 00:51:34.735297 txt2dub-0.1.1/txt2dub/widgets/logo.py
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 txt2dub-0.1.1/PKG-INFO
```

### Comparing `txt2dub-0.1.0/LICENSE` & `txt2dub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/pyproject.toml` & `txt2dub-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "txt2dub"
-version = "0.1.0"
-description = "A terminal UI application for editing voiceover scripts and generating text to speech performances."
+version = "0.1.1"
+homepage = "https://github.com/NotYourDadsMath/txt2dub"
+description = "A text-based UI application for editing voiceover scripts and generating text to speech performances."
 authors = ["Mike Kibbel", "Not Your Dad's Math"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyttsx3 = "^2.90"
-textual = "^0.24.1"
+textual = "^0.25.0"
 
 [tool.poetry.group.dev.dependencies]
 textual-dev = "^0.0.2"
 
 [tool.poetry.scripts]
 txt2dub = "txt2dub.app:run"
```

### Comparing `txt2dub-0.1.0/README.md` & `txt2dub-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 txt2dub
 =======
 
-Write and edit voiceover scripts and generate text-to-speech performances in a text-based user interface.
+A text-based UI application for editing voiceover scripts and generating text to speech performances.
 
 ## What is `txt2dub` for?
 
 `txt2dub` is a video content creation tool for writing scripts and generating overdub performances as MP3 files that can be imported into your video editing software. This supports a workflow for arranging video assets on your timeline based on the voice performance's timing. You can record your own voiceovers to replace the robotic text-to-speech performance, or you can keep the placeholders if that's the style you're targeting.
 
+![Screenshot of txt2dub being used to edit a script with a quote from Frank Herbert's Dune](https://raw.githubusercontent.com/NotYourDadsMath/txt2dub/main/images/txt2dub-editing.png)
+
+
+This is how it looks to edit a script in `txt2dub`. As you type each script line is played aloud by the text-to-speech system. You can play back a line, reorder lines or insert new lines anywhere in the script. You can set the voice performer and the rate of speech for each line in the script. You can undo or redo actions without limit. You can also play back the whole script starting from the selected line.
+
+![Screenshot of txt2dub home screen](https://raw.githubusercontent.com/NotYourDadsMath/txt2dub/main/images/txt2dub-home-screen.png)
+
+And here is the home screen.
+
 ## Who is `txt2dub` for?
 
 `txt2dub` is designed to be easily installable on the major desktop platforms (Windows, Mac and Linux) without programming skills. More detailed installation instructions will be posted soon. For those familiar with Python, you can install `txt2dub` in a virtual environment or globally with:
 
 ```bash
 pip install txt2dub
 ```
```

### Comparing `txt2dub-0.1.0/txt2dub/app.py` & `txt2dub-0.1.1/txt2dub/app.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/models/base.py` & `txt2dub-0.1.1/txt2dub/models/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/models/script.py` & `txt2dub-0.1.1/txt2dub/models/script.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/screens/file/screen.py` & `txt2dub-0.1.1/txt2dub/screens/file/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/screens/file/widgets.py` & `txt2dub-0.1.1/txt2dub/screens/file/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/screens/script/messages.py` & `txt2dub-0.1.1/txt2dub/screens/script/messages.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/screens/script/screen.py` & `txt2dub-0.1.1/txt2dub/screens/script/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/screens/script/widgets.py` & `txt2dub-0.1.1/txt2dub/screens/script/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/services/actions.py` & `txt2dub-0.1.1/txt2dub/services/actions.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/services/tts.py` & `txt2dub-0.1.1/txt2dub/services/tts.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/styles/app.css` & `txt2dub-0.1.1/txt2dub/styles/app.css`

 * *Files 7% similar despite different names*

```diff
@@ -123,14 +123,16 @@
     border-bottom: hkey $panel-darken-1;
 }
 .toolbar.bottom {
     dock: bottom;
     padding-bottom: 1;
     border: none;
     border-top: hkey $panel;
+    /* HACK: auto height broke for bottom docked toolbars in textual@0.25.0. */
+    height: 5;
 }
 
 .toolbar .row {
     layout: horizontal;
     align-horizontal: center;
     width: auto;
     height: auto;
```

### Comparing `txt2dub-0.1.0/txt2dub/tts/interpreter.py` & `txt2dub-0.1.1/txt2dub/tts/interpreter.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/txt2dub/widgets/base.py` & `txt2dub-0.1.1/txt2dub/widgets/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.0/PKG-INFO` & `txt2dub-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: txt2dub
-Version: 0.1.0
-Summary: A terminal UI application for editing voiceover scripts and generating text to speech performances.
+Version: 0.1.1
+Summary: A text-based UI application for editing voiceover scripts and generating text to speech performances.
+Home-page: https://github.com/NotYourDadsMath/txt2dub
 License: MIT
 Author: Mike Kibbel
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyttsx3 (>=2.90,<3.0)
-Requires-Dist: textual (>=0.24.1,<0.25.0)
+Requires-Dist: textual (>=0.25.0,<0.26.0)
 Description-Content-Type: text/markdown
 
 txt2dub
 =======
 
-Write and edit voiceover scripts and generate text-to-speech performances in a text-based user interface.
+A text-based UI application for editing voiceover scripts and generating text to speech performances.
 
 ## What is `txt2dub` for?
 
 `txt2dub` is a video content creation tool for writing scripts and generating overdub performances as MP3 files that can be imported into your video editing software. This supports a workflow for arranging video assets on your timeline based on the voice performance's timing. You can record your own voiceovers to replace the robotic text-to-speech performance, or you can keep the placeholders if that's the style you're targeting.
 
+![Screenshot of txt2dub being used to edit a script with a quote from Frank Herbert's Dune](https://raw.githubusercontent.com/NotYourDadsMath/txt2dub/main/images/txt2dub-editing.png)
+
+
+This is how it looks to edit a script in `txt2dub`. As you type each script line is played aloud by the text-to-speech system. You can play back a line, reorder lines or insert new lines anywhere in the script. You can set the voice performer and the rate of speech for each line in the script. You can undo or redo actions without limit. You can also play back the whole script starting from the selected line.
+
+![Screenshot of txt2dub home screen](https://raw.githubusercontent.com/NotYourDadsMath/txt2dub/main/images/txt2dub-home-screen.png)
+
+And here is the home screen.
+
 ## Who is `txt2dub` for?
 
 `txt2dub` is designed to be easily installable on the major desktop platforms (Windows, Mac and Linux) without programming skills. More detailed installation instructions will be posted soon. For those familiar with Python, you can install `txt2dub` in a virtual environment or globally with:
 
 ```bash
 pip install txt2dub
 ```
```

