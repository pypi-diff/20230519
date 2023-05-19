# Comparing `tmp/alignmeet-1.0.8.tar.gz` & `tmp/alignmeet-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/alignmeet/alignmeet/dist/tmpciw92sdm/alignmeet-1.0.8.tar", last modified: Wed Mar 29 05:42:06 2023, max compression
+gzip compressed data, was "alignmeet-1.0.9.tar", last modified: Fri May 19 08:19:11 2023, max compression
```

## Comparing `alignmeet-1.0.8.tar` & `alignmeet-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     8470 2023-03-29 05:41:56.000000 alignmeet-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      276 2023-03-29 05:42:06.000000 alignmeet-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-29 05:42:06.000000 alignmeet-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet/icons/
--rw-r--r--   0 runner    (1001) docker     (116)      521 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/plus.png
--rw-r--r--   0 runner    (1001) docker     (116)      628 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-stop-090.png
--rw-r--r--   0 runner    (1001) docker     (116)      742 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-return.png
--rw-r--r--   0 runner    (1001) docker     (116)      708 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-return-180-left.png
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-circle-315.png
--rw-r--r--   0 runner    (1001) docker     (116)      457 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/layout-split-vertical.png
--rw-r--r--   0 runner    (1001) docker     (116)      737 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-split-270.png
--rw-r--r--   0 runner    (1001) docker     (116)      667 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/arrow-stop-270.png
--rw-r--r--   0 runner    (1001) docker     (116)      401 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/icons/layout-join-vertical.png
--rw-r--r--   0 runner    (1001) docker     (116)     4439 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2971 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (116)     7131 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/player.py
--rw-r--r--   0 runner    (1001) docker     (116)      360 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/combobox.py
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/dialog_act.py
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/htmldelegate.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4979 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3169 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/autoalign.py
--rw-r--r--   0 runner    (1001) docker     (116)     4576 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/problems.py
--rw-r--r--   0 runner    (1001) docker     (116)    24331 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/annotation.py
--rw-r--r--   0 runner    (1001) docker     (116)    19626 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)      512 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/clickslider.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet/minutes/
--rw-r--r--   0 runner    (1001) docker     (116)     1070 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/minutes/minutes_editor.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/minutes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4624 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/minutes/minutes_model.py
--rw-r--r--   0 runner    (1001) docker     (116)    13260 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/minutes/minutes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet/transcripts/
--rw-r--r--   0 runner    (1001) docker     (116)    19349 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/transcripts.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2632 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/speaker_editor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4905 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/dialog_act_editor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4586 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/dialog_act_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2023-03-29 05:41:56.000000 alignmeet-1.0.8/alignmeet/transcripts/transcript.py
--rw-r--r--   0 runner    (1001) docker     (116)      793 2023-03-29 05:41:56.000000 alignmeet-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      276 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       53 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1219 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-29 05:42:06.000000 alignmeet-1.0.8/alignmeet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-03-29 05:41:56.000000 alignmeet-1.0.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.878692 alignmeet-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 08:18:56.000000 alignmeet-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-19 08:19:11.878692 alignmeet-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-19 08:18:56.000000 alignmeet-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.874691 alignmeet-1.0.9/alignmeet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19712 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/autoalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/clickslider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/dialog_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/htmldelegate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.878692 alignmeet-1.0.9/alignmeet/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-circle-315.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-return-180-left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-return.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-split-270.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-stop-090.png
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/arrow-stop-270.png
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/layout-join-vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/layout-split-vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/icons/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.878692 alignmeet-1.0.9/alignmeet/minutes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/minutes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/minutes/minutes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/minutes/minutes_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/minutes/minutes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.878692 alignmeet-1.0.9/alignmeet/transcripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/dialog_act_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/dialog_act_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/speaker_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/transcript.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-05-19 08:18:56.000000 alignmeet-1.0.9/alignmeet/transcripts/transcripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:19:11.878692 alignmeet-1.0.9/alignmeet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 08:19:11.000000 alignmeet-1.0.9/alignmeet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 08:19:11.878692 alignmeet-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-19 08:18:56.000000 alignmeet-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `alignmeet-1.0.8/README.md` & `alignmeet-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/plus.png` & `alignmeet-1.0.9/alignmeet/icons/plus.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-stop-090.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-stop-090.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-return.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-return.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-return-180-left.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-return-180-left.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-circle-315.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-circle-315.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-split-270.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-split-270.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/icons/arrow-stop-270.png` & `alignmeet-1.0.9/alignmeet/icons/arrow-stop-270.png`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/__main__.py` & `alignmeet-1.0.9/alignmeet/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         else:
             assert False
         embeds = e.embed(a._das if type == TR else a._minutes)
         return embeds
     
     parser = argparse.ArgumentParser(prog='Alignmeet', description="Annotation Tool for Meeting Minuting", epilog="Or run without arguments for annotation GUI.")
     group = parser.add_mutually_exclusive_group()
+    group.add_argument('--autoembed', dest='autoembed', action='store_true', help='Run GUI with autoembed.')
     group.add_argument('-et', dest='et', metavar='Filename', type=str, nargs='+', help='Generate embeddings for given transcripts.')
     group.add_argument('-em', dest='em', metavar='Filename', type=str, nargs='+', help='Generate embeddings for given minutes files.')
     group.add_argument('-a', '--align', dest='a', metavar=('Minutes_Embed', 'Transcript_Embed'), type=str, nargs=2, help='Generate alignment based on given file embeddings.')
     parser.add_argument('--thr', type=float, help="Threshold for alignment (0.0 to 1.0).", required=False, default=0.5)
     parser.add_argument('-nf', '--not-final', dest='final', action='store_false' , help="Store alignment as tentative (to be confirmed by hand in GUI).")
     args=parser.parse_args()
     
@@ -98,13 +99,15 @@
     else:
         app = QApplication(sys.argv)
         app.setStyle("Fusion")    
 
 
         Settings.apply_settings()
         a = Annotations()
+        a.setAutoembed(args.autoembed)
+            
         a.show()
 
         exit(app.exec_())
 
 if __name__ == '__main__':
     main()
```

### Comparing `alignmeet-1.0.8/alignmeet/evaluation.py` & `alignmeet-1.0.9/alignmeet/evaluation.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/player.py` & `alignmeet-1.0.9/alignmeet/player.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/dialog_act.py` & `alignmeet-1.0.9/alignmeet/dialog_act.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/htmldelegate.py` & `alignmeet-1.0.9/alignmeet/htmldelegate.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/settings.py` & `alignmeet-1.0.9/alignmeet/settings.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/autoalign.py` & `alignmeet-1.0.9/alignmeet/autoalign.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 class Embedder:
     def __init__(self, model = 'stsb-mpnet-base-v2'):
         self.model_name = model
         self.model = SentenceTransformer(model)
         
     def embed(self, lines):
+        return
         embeds = self.model.encode([l.text for l in lines])
         return embeds
     
     @staticmethod
     def saveEmbed(embeds, filename):
         with open(filename, 'wb') as f:
             pickle.dump(embeds, f)
```

### Comparing `alignmeet-1.0.8/alignmeet/problems.py` & `alignmeet-1.0.9/alignmeet/problems.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/annotation.py` & `alignmeet-1.0.9/alignmeet/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
             super().__init__()
             self.annotation = annotation
             self.filename = filename
             
         def run(self):
             e = Embedder()
             embeds = e.embed(self.annotation._minutes)
-            self.finished.emit(list(embeds), self.filename)
+            if embeds:
+                self.finished.emit(list(embeds), self.filename)
             
 class TranscriptEmbedThread(QThread):
         finished = Signal(list, str)
         def __init__(self, annotation, filename):
             super().__init__()
             self.annotation = annotation
             self.filename = filename
@@ -127,17 +128,18 @@
         self._relevance = 1.0
         
         self.tr_thread = None
         self.min_thread = None
         self.tr_embed_done = False
         self.min_embed_done = False
         
-        
         self.threshold = 0.5 #for autoalign
 
+        self.remarks_backup = None
+
         if undo:
             self.undo_stack = QUndoStack(self) # stores QUndoCommands (user actions) that can be undone/redone
             self.undo_view = QUndoView(self.undo_stack)
 
     def show_edit_history(self):
         self.undo_view.show()
 
@@ -275,30 +277,30 @@
                 data.append(DialogAct(*s))
 
         self._das = data
         
         if os.path.exists(full_path + '.embed'):
             embeds = Embedder.loadEmbed(full_path + '.embed')
             self.finalize_tr_embed(embeds, full_path, False)
-        else:
+        elif self.annotations.autoembed:
             if self.tr_thread:
                 self.tr_thread.terminate()
             self.tr_thread = TranscriptEmbedThread(self, full_path)
             self.tr_thread.finished.connect(self.finalize_tr_embed)
             self.tr_thread.start()
         
         self.open_annotation()
         self.open_evaluation()
         self.modified = False
 
     def open_minutes(self, file):
         self.min_embed_done = False
         if self.annotations:
             self.annotations.autoalignAction.setEnabled(False)
-        self._prevent()
+        #self._prevent()
         self._minutes_file = file
         full_path = path.normpath(path.join(self._path, MINUTES_FOLDER, file))
         if not os.path.exists(full_path):
             full_path = path.normpath(path.join(self._path, file))
         data = []
         try:
             with open(full_path, 'r', encoding='utf-8') as f:
@@ -308,27 +310,30 @@
         except:
             pass
         self._minutes = data
         
         if os.path.exists(full_path + '.embed'):
             embeds = Embedder.loadEmbed(full_path + '.embed')
             self.finalize_min_embed(embeds, full_path, False)
-        else:
+        elif self.annotations.autoembed:
             if self.min_thread:
                 self.min_thread.terminate()
             self.min_thread = MinuteEmbedThread(self, full_path)
             self.min_thread.finished.connect(self.finalize_min_embed)
             self.min_thread.start()
         
         self._make_minutes_index_map()
         self.open_annotation()
         self.open_evaluation()
         self.modified = False
 
     def open_annotation(self):
+        if not self._das == []:
+            self.remarks_backup = [d.problem for d in self._das]
+        
         for d in self._das:
             d.problem = None
             d.minute = None
         annotations_path = path.normpath(path.join(self._path, ANNOTATIONS_FOLDER))
         annotations_prefix = '' if os.path.exists(annotations_path) else 'alignment+'
         af = "{}{}+{}".format(
             annotations_prefix,
@@ -369,14 +374,24 @@
                     d.problem = problem
                     d.is_final = final
                     try:
                         d.minute = self._minutes[minute]
                     except:
                         d.minute = None
             self.problems_changed.emit()
+            
+    def copy_problems_if_none_presend(self):
+        if not self.remarks_backup or not len(self._das) == len(self.remarks_backup):
+            return
+        untouched = set([d.problem == None for d in self._das])
+        if True in untouched and not False in untouched:
+            for i, d in enumerate(self._das):
+                d.problem = self.remarks_backup[i]
+            self.problems_changed.emit()
+            self.modified = True
 
     def open_evaluation(self):
         self._adequacy = 1.0
         self._grammaticality = 1.0
         self._fluency = 1.0
         self._relevance = 1.0
         evaluation_path = path.normpath(path.join(self._path, EVALUATIONS_FOLDER))
@@ -455,15 +470,15 @@
         full_path = path.normpath(full_path)
         with open(full_path, 'w', encoding='utf-8') as f:
             for idx, da in enumerate(self._das):
                 if da.minute != None or da.problem != None:
                     midx = self.minutes_index_map[da.minute]
                     if isinstance(da.problem, str):
                         problem = f'0:{da.problem}'
-                    elif da.problem:
+                    elif not da.problem is None:
                         problem = da.problem + 1
                     else:
                         problem = None
                     f.write('{} {}{} {}\n'.format(
                         idx + 1,
                         midx + 1 if midx is not None else midx,
                         '?' if not da.is_final else '',
```

### Comparing `alignmeet-1.0.8/alignmeet/annotations.py` & `alignmeet-1.0.9/alignmeet/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
         self.setWindowTitle("Annotations")
         self.folder = None
         self._gui_setup()
         self.setAttribute(Qt.WA_DeleteOnClose)
         self.is_git = False
         self.new_problem = ''
+        
+    def setAutoembed(self, autoembed):
+        self.autoembed = autoembed
 
     def _gui_setup(self):
         layout = QHBoxLayout()
 
         splitter = QSplitter(Qt.Horizontal)
         panel_right = QWidget(self)
         layout.addWidget(splitter)
```

### Comparing `alignmeet-1.0.8/alignmeet/clickslider.py` & `alignmeet-1.0.9/alignmeet/clickslider.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/minutes/minutes_editor.py` & `alignmeet-1.0.9/alignmeet/minutes/minutes_editor.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/minutes/minutes_model.py` & `alignmeet-1.0.9/alignmeet/minutes/minutes_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     return m.fluency
                 if j == 4:
                     return m.relevance
         elif role == Qt.BackgroundRole:
             if self.annotation.is_minute_visible(m):
                 return self.annotation.get_minute_color(m)
         elif role == Qt.ForegroundRole:
-            if self.annotation.is_minute_visible(m):                
+            if self.annotation.is_minute_visible(m):
                 return self.annotation.get_minute_text_color(m)
         else:
             return None
 
     def flags(self, index):
         i = index.row()
         j = index.column()
```

### Comparing `alignmeet-1.0.8/alignmeet/minutes/minutes.py` & `alignmeet-1.0.9/alignmeet/minutes/minutes.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,16 @@
         self.right.setEnabled(s and not self._evaluation_mode)
         if s or self._evaluation_mode:
             self.minutes_view.setEditTriggers(QAbstractItemView.AllEditTriggers)
         else:
             self.minutes_view.setEditTriggers(QAbstractItemView.NoEditTriggers)
 
     def _minute_selected(self, m):
-        if self._evaluation_mode:
-            return
+    #     if self._evaluation_mode:
+    #         return
         if self.edit.isChecked():
             self.deleteAction.setEnabled(True)
             return
         m = self.annotation.get_minute(m)
         self.annotation.set_minute(m)
 
     @Slot(bool)
@@ -255,14 +255,15 @@
         selection = self.minutes_view.selectionModel()
         return list(set([i.row() for i in selection.selectedIndexes()]))
         
     @Slot()
     def _minutes_changed(self):
         self.annotation.undo_stack.clear()
         self.annotation.open_minutes(self.minutes_ver.currentText())
+        self.annotation.copy_problems_if_none_presend()
         self.annotation.problems_changed.emit()
 
 class TableView(Transcript):
     minute_selected = Signal(int)
 
     def __init__(self, parent):
         super(TableView, self).__init__(parent)
```

### Comparing `alignmeet-1.0.8/alignmeet/transcripts/transcripts.py` & `alignmeet-1.0.9/alignmeet/transcripts/transcripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,31 +89,31 @@
         self.resetAction = QAction('Reset minutes', transcript)
         self.resetAction.setShortcuts(['Ctrl+m'])
         self.resetAction.setToolTip('Reset minutes (Ctrl+m)')
         self.resetAction.triggered.connect(self._reset_triggered)
         transcript.addAction(self.resetAction)
         self.toolbar.addAction(self.resetAction)
         
-        self.resetpAction = QAction('Reset problems', transcript)
+        self.resetpAction = QAction('Reset remarks', transcript)
         self.resetpAction.setShortcuts(['Ctrl+p'])
-        self.resetpAction.setToolTip('Reset problems (Ctrl+p)')
+        self.resetpAction.setToolTip('Reset remarks (Ctrl+p)')
         self.resetpAction.triggered.connect(self._resetp_triggered)
         transcript.addAction(self.resetpAction)
         self.toolbar.addAction(self.resetpAction)
 
         empty = QWidget()
         empty.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
         self.toolbar.addWidget(empty)
 
         self.edit = QCheckBox("edit transcript")
         self.edit.setChecked(True)
         self.edit.stateChanged.connect(self._editation)
         # parse_layout.addStretch()
 
-        self.problems = QCheckBox('show problems')
+        self.problems = QCheckBox('show remarks')
         self.problems.setChecked(True)
 
         self.toolbar.addWidget(self.edit)
         self.toolbar.addWidget(self.problems)
 
 
         layout.addWidget(transcript)
```

### Comparing `alignmeet-1.0.8/alignmeet/transcripts/speaker_editor.py` & `alignmeet-1.0.9/alignmeet/transcripts/speaker_editor.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/transcripts/dialog_act_editor.py` & `alignmeet-1.0.9/alignmeet/transcripts/dialog_act_editor.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/alignmeet/transcripts/dialog_act_model.py` & `alignmeet-1.0.9/alignmeet/transcripts/dialog_act_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class DAModel(QtCore.QAbstractTableModel): 
     def __init__(self, annotation : Annotation, parent=None, *args): 
         super(DAModel, self).__init__()
         self.annotation = annotation
         self.annotation.modified_changed.connect(self.update)
         self.setHeaderData(0, Qt.Horizontal, "Speaker")
         self.setHeaderData(1, Qt.Horizontal, "Transcript")
-        self.setHeaderData(2, Qt.Horizontal, "Problem")
+        self.setHeaderData(2, Qt.Horizontal, "Remark")
         self.highlight = None
     
     @Slot()
     def update(self):
         self.layoutAboutToBeChanged.emit()
         self.layoutChanged.emit()
 
@@ -29,17 +29,17 @@
 
     def headerData(self, index, orientation, role):
         if role == Qt.DisplayRole:
             if orientation == Qt.Horizontal:
                 if index == 0:
                     return 'Speaker'
                 elif index == 1:
-                    return 'Dialog Act'
+                    return 'Transcript'
                 else:
-                    return 'Problem'
+                    return 'Remark'
             elif orientation == Qt.Vertical:
                 if self.annotation.das_count() > index:
                     d = self.annotation.get_dialog_act(index)
                     if d.time_valid():
                         return '{:2d}:{:2.1f} - {:2d}:{:2.1f}'.format(
                             int(d.start // 60),
                             d.start - (d.start // 60) * 60,
```

### Comparing `alignmeet-1.0.8/alignmeet/transcripts/transcript.py` & `alignmeet-1.0.9/alignmeet/transcripts/transcript.py`

 * *Files identical despite different names*

### Comparing `alignmeet-1.0.8/setup.py` & `alignmeet-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os.path
 from setuptools import find_packages, setup
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-#with open(os.path.join(HERE, "README.md")) as fid:
-#    README = fid.read()
+with open(os.path.join(HERE, "README.md")) as fid:
+    README = fid.read()
     
 setup(
     name="alignmeet",
-    version="1.0.8",
+    version="1.0.9",
     description="A Comprehensive Tool for Meeting Alignment, Annotation and Evaluation",
-#    long_description=README,
-#    long_description_content_type="text/markdown",
+    long_description=README,
+    long_description_content_type="text/markdown",
     url="https://github.com/ELITR/alignmeet",
     author="Peter Polak",
     author_email="polak@ufal.mff.cuni.cz",
     license="TBD",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

### Comparing `alignmeet-1.0.8/alignmeet.egg-info/SOURCES.txt` & `alignmeet-1.0.9/alignmeet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

