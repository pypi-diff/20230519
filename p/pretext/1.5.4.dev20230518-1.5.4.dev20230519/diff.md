# Comparing `tmp/pretext-1.5.4.dev20230518.tar.gz` & `tmp/pretext-1.5.4.dev20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.4.dev20230518.tar", max compression
+gzip compressed data, was "pretext-1.5.4.dev20230519.tar", max compression
```

## Comparing `pretext-1.5.4.dev20230518.tar` & `pretext-1.5.4.dev20230519.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/README.md
--rw-r--r--   0        0        0     1440 2023-05-18 06:19:01.989555 pretext-1.5.4.dev20230518/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-05-18 06:19:07.289638 pretext-1.5.4.dev20230518/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-18 06:18:17.924778 pretext-1.5.4.dev20230518/pretext/core/resources.py
--rw-r--r--   0        0        0  1029449 2023-05-18 06:19:07.289638 pretext-1.5.4.dev20230518/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-18 06:18:17.928778 pretext-1.5.4.dev20230518/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-18 06:18:17.928778 pretext-1.5.4.dev20230518/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-18 06:18:17.928778 pretext-1.5.4.dev20230518/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160548 2023-05-18 06:19:07.353639 pretext-1.5.4.dev20230518/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     8054 2023-05-18 06:19:07.341638 pretext-1.5.4.dev20230518/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173747 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     5095 2023-05-18 06:19:07.357639 pretext-1.5.4.dev20230518/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-18 06:19:07.377639 pretext-1.5.4.dev20230518/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8830 2023-05-18 06:19:07.361639 pretext-1.5.4.dev20230518/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-18 06:18:17.928778 pretext-1.5.4.dev20230518/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-18 06:19:01.989555 pretext-1.5.4.dev20230518/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230518/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/README.md
+-rw-r--r--   0        0        0     1440 2023-05-19 06:18:46.027659 pretext-1.5.4.dev20230519/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-05-19 06:18:51.256048 pretext-1.5.4.dev20230519/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/core/resources.py
+-rw-r--r--   0        0        0  1029942 2023-05-19 06:18:51.256048 pretext-1.5.4.dev20230519/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160548 2023-05-19 06:18:51.312051 pretext-1.5.4.dev20230519/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     8054 2023-05-19 06:18:51.300051 pretext-1.5.4.dev20230519/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173747 2023-05-19 06:18:51.332053 pretext-1.5.4.dev20230519/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     5095 2023-05-19 06:18:51.316052 pretext-1.5.4.dev20230519/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8830 2023-05-19 06:18:51.316052 pretext-1.5.4.dev20230519/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-19 06:18:46.027659 pretext-1.5.4.dev20230519/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230519/PKG-INFO
```

### Comparing `pretext-1.5.4.dev20230518/LICENSE` & `pretext-1.5.4.dev20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/README.md` & `pretext-1.5.4.dev20230519/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/__init__.py` & `pretext-1.5.4.dev20230519/pretext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = 'bcd0befbd265c936cb6f8f03591506b80de9e260'
+CORE_COMMIT = '393d7a374feeb73971d9eda9cc2232dab7b68f31'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.4.dev20230518/pretext/build.py` & `pretext-1.5.4.dev20230519/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/cli.py` & `pretext-1.5.4.dev20230519/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/codechat.py` & `pretext-1.5.4.dev20230519/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/config/xml_overlay.py` & `pretext-1.5.4.dev20230519/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/core/pretext.py` & `pretext-1.5.4.dev20230519/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/core/resources.py` & `pretext-1.5.4.dev20230519/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/core/resources.zip` & `pretext-1.5.4.dev20230519/pretext/core/resources.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,142 +1,142 @@
-Zip file size: 1029449 bytes, number of entries: 140
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-18 06:19 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-18 06:19 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx      481 b- defN 23-May-18 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-May-18 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 23-May-18 06:19 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx    18421 b- defN 23-May-18 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-May-18 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx    25290 b- defN 23-May-18 06:19 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   134043 b- defN 23-May-18 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx     1180 b- defN 23-May-18 06:19 schema/README.md
--rw-r--r--  2.0 unx   125135 b- defN 23-May-18 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-May-18 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    34210 b- defN 23-May-18 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-May-18 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-May-18 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-May-18 06:19 schema/build.sh
--rw-r--r--  2.0 unx     1367 b- defN 23-May-18 06:19 pretext/README.md
--rw-r--r--  2.0 unx   172432 b- defN 23-May-18 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-18 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-May-18 06:19 pretext/pretext
--rw-r--r--  2.0 unx        0 b- defN 23-May-18 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx    35449 b- defN 23-May-18 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx     2566 b- defN 23-May-18 06:19 pretext/pretext.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/utilities/
--rw-r--r--  2.0 unx     9787 b- defN 23-May-18 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-May-18 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-18 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-18 06:19 xsl/README.md
--rw-r--r--  2.0 unx   139486 b- defN 23-May-18 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-18 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-18 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-May-18 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-18 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-18 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   261852 b- defN 23-May-18 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-18 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-May-18 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-May-18 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-18 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   540859 b- defN 23-May-18 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-18 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-18 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-18 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-18 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-18 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-18 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-18 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-18 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-18 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   544780 b- defN 23-May-18 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-May-18 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-18 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-18 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    86548 b- defN 23-May-18 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-18 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-18 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-18 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   606187 b- defN 23-May-18 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-18 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-18 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-18 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-18 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-18 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-May-18 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-18 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-18 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-18 06:19 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-May-18 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx    10306 b- defN 23-May-18 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-May-18 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-18 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-May-18 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5800 b- defN 23-May-18 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-18 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-May-18 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-May-18 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-May-18 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16518 b- defN 23-May-18 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-18 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-18 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-18 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-May-18 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-18 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15938 b- defN 23-May-18 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-18 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-18 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-18 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-18 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-May-18 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-18 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-18 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-18 06:19 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-18 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-18 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     1810 b- defN 23-May-18 06:19 xsl/utilities/README.md
--rw-r--r--  2.0 unx    30257 b- defN 23-May-18 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-18 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-May-18 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-18 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-18 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1276 b- defN 23-May-18 06:19 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-18 06:19 css/style_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-18 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-18 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-18 06:19 css/README.md
--rw-r--r--  2.0 unx     1280 b- defN 23-May-18 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-18 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-18 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-18 06:19 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-18 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-18 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-18 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-18 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-18 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-18 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-18 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-18 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-18 06:19 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-18 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-18 06:19 css/epub.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-18 06:19 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-18 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     4021 b- defN 23-May-18 06:19 css/update_css
-140 files, 4812130 bytes uncompressed, 1012121 bytes compressed:  79.0%
+Zip file size: 1029942 bytes, number of entries: 140
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-19 06:18 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-19 06:18 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 06:18 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      481 b- defN 23-May-19 06:18 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-May-19 06:18 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-19 06:18 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-19 06:18 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-May-19 06:18 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-19 06:18 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   134043 b- defN 23-May-19 06:18 schema/pretext.xml
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-19 06:18 schema/README.md
+-rw-r--r--  2.0 unx   125135 b- defN 23-May-19 06:18 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-May-19 06:18 schema/xml.xsd
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-19 06:18 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-May-19 06:18 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-19 06:18 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-19 06:18 schema/build.sh
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-19 06:18 pretext/README.md
+-rw-r--r--  2.0 unx   172432 b- defN 23-May-19 06:18 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-19 06:18 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-May-19 06:18 pretext/pretext
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 06:18 pretext/__init__.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-May-19 06:18 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-19 06:18 pretext/pretext.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/utilities/
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-19 06:18 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-19 06:18 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-19 06:18 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-19 06:18 xsl/README.md
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-19 06:18 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-19 06:18 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-19 06:18 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-19 06:18 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-19 06:18 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-19 06:18 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   261852 b- defN 23-May-19 06:18 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-19 06:18 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-19 06:18 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-May-19 06:18 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-19 06:18 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   540859 b- defN 23-May-19 06:18 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-19 06:18 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-19 06:18 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-19 06:18 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-19 06:18 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-19 06:18 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-19 06:18 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-19 06:18 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-19 06:18 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-19 06:18 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   544780 b- defN 23-May-19 06:18 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-19 06:18 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-19 06:18 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-19 06:18 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    88250 b- defN 23-May-19 06:18 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-19 06:18 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-19 06:18 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-19 06:18 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   606187 b- defN 23-May-19 06:18 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-19 06:18 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-19 06:18 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-19 06:18 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-19 06:18 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-May-19 06:18 xsl/support/README.md
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-19 06:18 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-19 06:18 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-19 06:18 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-May-19 06:18 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-19 06:18 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-19 06:18 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-19 06:18 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-May-19 06:18 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-19 06:18 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-19 06:18 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-19 06:18 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-19 06:18 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-19 06:18 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-19 06:18 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-19 06:18 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-19 06:18 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-19 06:18 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-19 06:18 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-19 06:18 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-19 06:18 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-19 06:18 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-19 06:18 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-19 06:18 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-19 06:18 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-19 06:18 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-19 06:18 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-19 06:18 xsl/utilities/README.md
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-19 06:18 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-19 06:18 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-May-19 06:18 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-19 06:18 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-19 06:18 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-19 06:18 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-19 06:18 css/style_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-19 06:18 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-19 06:18 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-19 06:18 css/README.md
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-19 06:18 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_blue_red.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-19 06:18 css/mathbook-3.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-19 06:18 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-19 06:18 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-19 06:18 css/colors_blue_green.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-19 06:18 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-19 06:18 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-19 06:18 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-19 06:18 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-19 06:18 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-19 06:18 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-19 06:18 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-19 06:18 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-19 06:18 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-19 06:18 css/epub.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-19 06:18 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-19 06:18 css/update_css
+140 files, 4813832 bytes uncompressed, 1012614 bytes compressed:  79.0%
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -1217,14 +1217,20 @@
     <xsl:text>…</xsl:text>
   </xsl:template>
   <!-- Unicode Character 'MIDDLE DOT' (U+00B7) -->
   <!-- Liblouis: 4-16                          -->
   <xsl:template name="midpoint-character">
     <xsl:text>·</xsl:text>
   </xsl:template>
+  <!-- Unicode Character 'SWUNG DASH' (U+2053) -->
+  <!-- instead faking it with                  -->
+  <!-- Unicode Character 'TILDE' (U+007E)      -->
+  <xsl:template name="swungdash-character">
+    <xsl:text>~</xsl:text>
+  </xsl:template>
   <!-- Unicode Character 'PILCROW SIGN' (U+00B6) -->
   <!-- Liblouis: 45-1234                         -->
   <xsl:template name="pilcrow-character">
     <xsl:text>¶</xsl:text>
   </xsl:template>
   <!-- Unicode Character 'SECTION SIGN' (U+00A7) -->
   <!-- Liblouis: 45-234                          -->
@@ -1237,24 +1243,56 @@
     <xsl:text>−</xsl:text>
   </xsl:template>
   <!-- Unicode Character 'MULTIPLICATION SIGN' (U+00D7) -->
   <!-- Liblouis: 5-236                                  -->
   <xsl:template name="times-character">
     <xsl:text>×</xsl:text>
   </xsl:template>
+  <!-- Unicode Character 'FRACTION SLASH' (U+2044) -->
+  <!-- instead faking it with                      -->
+  <!-- Unicode Character 'SOLIDUS' (U+002F)        -->
+  <xsl:template name="solidus-character">
+    <xsl:text>/</xsl:text>
+  </xsl:template>
   <!-- Unicode Character 'DIVISION SIGN' (U+00F7) -->
   <!-- Liblouis: 5-34                             -->
   <xsl:template name="obelus-character">
     <xsl:text>÷</xsl:text>
   </xsl:template>
   <!-- Unicode Character 'PLUS-MINUS SIGN' (U+00B1) -->
   <!-- Liblouis: 456-235                            -->
   <xsl:template name="plusminus-character">
     <xsl:text>±</xsl:text>
   </xsl:template>
+  <!-- Icons -->
+  <!-- Just the four arrows, unsure about the rest -->
+  <!-- Arrows are in liblouis table                -->
+  <xsl:template match="icon">
+    <xsl:choose>
+      <xsl:when test="@name = 'arrow-left'">
+        <xsl:text>←</xsl:text>
+      </xsl:when>
+      <xsl:when test="@name ='arrow-up'">
+        <xsl:text>↑</xsl:text>
+      </xsl:when>
+      <xsl:when test="@name = 'arrow-right'">
+        <xsl:text>→</xsl:text>
+      </xsl:when>
+      <xsl:when test="@name ='arrow-down'">
+        <xsl:text>↓</xsl:text>
+      </xsl:when>
+      <xsl:otherwise>
+        <xsl:message>
+          WARNING:  &quot;icon&quot; with @name attribute value &quot;
+          <xsl:value-of select="@name"/>
+          &quot; does not have an implementation for braille.
+        </xsl:message>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:template>
   <!-- ############ -->
   <!-- Font Changes -->
   <!-- ############ -->
   <!-- Certain PreTeXt groupings in running text naturally yield just  -->
   <!-- a font change.  Braille and liblouis have facilities for italic -->
   <!-- and bold.  This is "internal" markup that eventually gets       -->
   <!-- interpreted by  lxml  in Python.                                -->
@@ -1501,14 +1539,26 @@
   <!-- Containers that have zero metadata (no title, etc.) -->
   <xsl:template match="statement|introduction|conclusion">
     <xsl:apply-templates select="*"/>
   </xsl:template>
   <xsl:template match="description">
     <xsl:apply-templates select="node()"/>
   </xsl:template>
+  <!-- fillin blanks, outside math -->
+  <!-- A fillin inside math will have disappeared on us by now, -->
+  <!-- it was mixed into some LaTeX syntax and has been gobbled -->
+  <!-- up by MathJax by now.  So the conditional here is really -->
+  <!-- moot and not necessary.                                  -->
+  <!-- [BANA, 2016] 10.6.2 and Michael Cantino: an underscore   -->
+  <!-- Seems to translate as a "sign": 46-36 in liblouis table  -->
+  <xsl:template match="fillin[not(parent::m or parent::me or parent::men or parent::mrow)]">
+    <xsl:text>_</xsl:text>
+  </xsl:template>
+  <!-- Fillin blanks, inside math -->
+  <!-- For math see https://nemeth.aphtech.org/lesson3.5 4x U+2824 -->
   <!-- ############ -->
   <!-- EXPERIMENTAL -->
   <!-- ############ -->
   <!-- A paragraph without "displays" is straightforward and -->
   <!-- we can bypass the more complicated procedure next.    -->
   <xsl:template match="p">
     <segment indentation="2">
@@ -1677,21 +1727,20 @@
   </xsl:template>
   <xsl:template match="console">
     <segment>CONSOLE</segment>
   </xsl:template>
   <xsl:template match="poem">
     <segment>POEM</segment>
   </xsl:template>
-  <!-- Next three are not structures, so as "text" -->
+  <!-- Next two are not structures, so as "text" -->
   <xsl:template match="quantity">
     <xsl:text>QUANTITY</xsl:text>
   </xsl:template>
-  <xsl:template match="kbd"/>
-  <xsl:template match="icon">
-    <xsl:text>ICON</xsl:text>
+  <xsl:template match="kbd">
+    <xsl:text>KBD</xsl:text>
   </xsl:template>
   <xsl:template name="missing-warning">
     <xsl:if test="//sage">
       <xsl:call-template name="missing-implementation">
         <xsl:with-param name="element" select="'sage'"/>
         <xsl:with-param name="ntimes" select="count(//sage)"/>
       </xsl:call-template>
@@ -1756,21 +1805,14 @@
     <xsl:if test="//kbd">
       <xsl:call-template name="missing-implementation">
         <xsl:with-param name="element" select="'kbd'"/>
         <xsl:with-param name="ntimes" select="count(//kbd)"/>
       </xsl:call-template>
     </xsl:if>
     <!--  -->
-    <xsl:if test="//icon">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'icon'"/>
-        <xsl:with-param name="ntimes" select="count(//icon)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
   </xsl:template>
   <xsl:template name="missing-implementation">
     <xsl:param name="element"/>
     <xsl:param name="ntimes"/>
     <xsl:message>
       Unimplemented:
       <xsl:value-of select="$element"/>
```

### Comparing `pretext-1.5.4.dev20230518/pretext/generate.py` & `pretext-1.5.4.dev20230519/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/project.py` & `pretext-1.5.4.dev20230519/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/__init__.py` & `pretext-1.5.4.dev20230519/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/.gitignore` & `pretext-1.5.4.dev20230519/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/article.zip` & `pretext-1.5.4.dev20230519/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160548 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/
--rw-r--r--  2.0 unx       86 b- defN 23-May-18 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-18 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-18 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-18 06:19 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-May-18 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     2059 b- defN 23-May-18 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-18 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-18 06:18 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-May-18 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-18 06:18 source/section-2.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-May-19 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-19 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-19 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-19 06:17 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-May-19 06:17 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-19 06:17 source/section-2.ptx
 15 files, 165338 bytes uncompressed, 158882 bytes compressed:  3.9%
```

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/book.zip` & `pretext-1.5.4.dev20230519/pretext/templates/resources/book.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8054 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-18 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-18 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-18 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-18 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-18 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6114 b- defN 23-May-18 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-May-18 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-19 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-19 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-19 06:17 source/main.ptx
 11 files, 16306 bytes uncompressed, 6816 bytes compressed:  58.2%
```

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/demo.zip` & `pretext-1.5.4.dev20230519/pretext/templates/resources/demo.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173747 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-18 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-18 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-18 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-18 06:19 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-18 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-18 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2059 b- defN 23-May-18 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6092 b- defN 23-May-18 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/images/
--rw-r--r--  2.0 unx      847 b- defN 23-May-18 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-18 06:18 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-18 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-18 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-18 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-18 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-18 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-18 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-May-18 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-18 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-18 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-18 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-18 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-18 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-18 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-18 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-May-18 06:18 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-May-18 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-18 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-18 06:18 source/images/sageplot3d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-19 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-19 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-19 06:17 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-19 06:17 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/images/
+-rw-r--r--  2.0 unx      847 b- defN 23-May-19 06:17 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-19 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-19 06:17 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-19 06:17 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-19 06:17 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-19 06:17 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-19 06:17 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-19 06:17 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-May-19 06:17 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-19 06:17 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-19 06:17 source/sec-features.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-19 06:17 source/backmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-19 06:17 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-19 06:17 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-19 06:17 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-19 06:17 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-May-19 06:17 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-May-19 06:17 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-19 06:17 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-19 06:17 source/images/sageplot3d.sage
 35 files, 190601 bytes uncompressed, 169647 bytes compressed:  11.0%
```

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/devcontainer.json` & `pretext-1.5.4.dev20230519/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/hello.zip` & `pretext-1.5.4.dev20230519/pretext/templates/resources/hello.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 5095 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/
--rw-r--r--  2.0 unx       69 b- defN 23-May-18 06:18 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-18 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-18 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-18 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-18 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-18 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-May-18 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-May-19 06:17 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-19 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-19 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-May-19 06:17 source/main.ptx
 11 files, 8317 bytes uncompressed, 3857 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.4.dev20230519/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/project.ptx` & `pretext-1.5.4.dev20230519/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pretext/templates/resources/slideshow.zip` & `pretext-1.5.4.dev20230519/pretext/templates/resources/slideshow.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8830 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-18 06:18 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-May-18 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-18 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-18 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-18 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-18 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      190 b- defN 23-May-18 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-18 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-May-18 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-May-19 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      190 b- defN 23-May-19 06:17 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-19 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-19 06:17 source/main.ptx
 12 files, 20904 bytes uncompressed, 7498 bytes compressed:  64.1%
```

### Comparing `pretext-1.5.4.dev20230518/pretext/utils.py` & `pretext-1.5.4.dev20230519/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230518/pyproject.toml` & `pretext-1.5.4.dev20230519/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.4.dev20230518"
+version = "1.5.4.dev20230519"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.4.dev20230518/PKG-INFO` & `pretext-1.5.4.dev20230519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.4.dev20230518
+Version: 1.5.4.dev20230519
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

