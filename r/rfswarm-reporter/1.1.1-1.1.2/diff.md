# Comparing `tmp/rfswarm-reporter-1.1.1.tar.gz` & `tmp/rfswarm-reporter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-reporter-1.1.1.tar", last modified: Fri Apr 28 08:51:31 2023, max compression
+gzip compressed data, was "rfswarm-reporter-1.1.2.tar", last modified: Fri May 19 05:26:26 2023, max compression
```

## Comparing `rfswarm-reporter-1.1.1.tar` & `rfswarm-reporter-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-04-28 08:33:44.000000 rfswarm-reporter-1.1.1/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/rfswarm_reporter/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   310811 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter/rfswarm_reporter.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-04-28 08:51:30.000000 rfswarm-reporter-1.1.1/setup-reporter.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-04-28 08:51:31.009142 rfswarm-reporter-1.1.1/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.2/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-05-19 05:23:33.000000 rfswarm-reporter-1.1.2/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.526295 rfswarm-reporter-1.1.2/rfswarm_reporter/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/rfswarm_reporter/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   311404 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/rfswarm_reporter/rfswarm_reporter.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/setup-reporter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/setup.cfg
```

### Comparing `rfswarm-reporter-1.1.1/LICENSE` & `rfswarm-reporter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-reporter-1.1.1/PKG-INFO` & `rfswarm-reporter-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.1
+Version: 1.1.2
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.1/README.md` & `rfswarm-reporter-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.1&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.1&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.2&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.2&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-reporter-1.1.1/rfswarm_reporter/rfswarm_reporter.py` & `rfswarm-reporter-1.1.2/rfswarm_reporter/rfswarm_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Reporter
-#    Version 1.1.1
+#    Version 1.1.2
 #
 
 import argparse
 import base64  # used for embedding images  # used for xhtml export
 import configparser
 import inspect
 import math
@@ -114,15 +114,15 @@
 			base.debugmsg(8, "res:", res)
 			return res
 		except Exception as e:
 			base.debugmsg(5, "Exception:", e)
 
 
 class ReporterBase():
-	version = "1.1.1"
+	version = "1.1.2"
 	debuglvl = 0
 
 	save_ini = True
 	running = True
 	displaygui = True
 	gui = None
 	darkmode = False
@@ -527,32 +527,40 @@
 		if value is None:
 			return "#0000FF"  # Blue
 		else:
 			return value
 
 	def rs_setting_get_font(self):
 		value = self.rs_setting_get('font')
-		if not self.gui:
+		base.debugmsg(6, "value", value)
+		if not base.displaygui:
+			base.debugmsg(6, "value", value)
 			return value
 		else:
 			fontlst = list(tkFont.families())
 			base.debugmsg(9, "fontlst", fontlst)
 			if value not in fontlst:
 				value = None
+				base.debugmsg(6, "value", value)
 			if value is None:
 				# Verdana, Tahoma, Arial, Helvetica, sans-serif
 				fontorder = ['Helvetica', 'Verdana', 'Tahoma', 'Arial', 'FreeSans']
+				base.debugmsg(6, "fontorder", fontorder)
 				for fnt in fontorder:
 					if fnt in fontlst:
+						base.debugmsg(6, "fnt", fnt)
 						return fnt
 				for fnt in fontlst:
 					if 'Sans' in fnt or 'sans' in fnt:
+						base.debugmsg(6, "fnt", fnt)
 						return fnt
+				base.debugmsg(6, "sans-serif")
 				return 'sans-serif'
 			else:
+				base.debugmsg(6, "value", value)
 				return value
 
 	def rs_setting_get_fontsize(self):
 		value = self.rs_setting_get_int('fontsize')
 		if value < 1:
 			return 12
 		else:
@@ -3380,15 +3388,19 @@
 		number = base.report_sect_number(id)
 		base.debugmsg(5, "number:", number)
 		name = base.report_item_get_name(id)
 		base.debugmsg(5, "name:", name)
 
 		heading_text = "{} {}".format(number, name)
 
-		document.add_heading(heading_text, level)
+		base.debugmsg(5, "heading_text:", heading_text, "	level:", level)
+		hdpg = document.add_heading(heading_text, level)
+		stylename = "Heading {}".format(level)
+		base.debugmsg(5, "stylename:", stylename)
+		hdpg.style = stylename
 		# document.add_paragraph("", style='Normal')
 
 	def docx_sections_contents(self, id):
 		base.debugmsg(5, "id:", id)
 
 		mode = base.rt_contents_get_mode(id)
 		level = base.rt_contents_get_level(id)
@@ -3401,15 +3413,15 @@
 		# 	fmode = "graph"
 		# if mode == "Table Of Tables":
 		# 	fmode = "table"
 
 		document = self.cg_data["docx"]["document"]
 		# document.add_paragraph("", style='Normal')
 
-		paragraph = document.add_paragraph()
+		paragraph = document.add_paragraph(style='Normal')
 		run = paragraph.add_run()
 		fldChar = OxmlElement('w:fldChar')  # creates a new element
 		fldChar.set(qn('w:fldCharType'), 'begin')  # sets attribute on element
 		instrText = OxmlElement('w:instrText')
 		instrText.set(qn('xml:space'), 'preserve')  # sets attribute on element
 		if mode == "Table Of Contents":
 			instrText.text = 'TOC \\o "1-' + str(level) + '" \\h \\z \\u'   # change 1-3 depending on heading levels you need
@@ -4072,14 +4084,15 @@
 			# =HYPERLINK(CONCAT("#'10 agents'!A",MATCH("10.8 selenium versions",'10 agents' A:A,0)),'10.8 selenium versions')
 			match = "MATCH(\"" + heading_text + "\",'" + parent_text + "'!A:A,0)"
 			base.debugmsg(9, "match:", match)
 			concat = "CONCATENATE(\"#'" + parent_text + "'!A\"," + match + ")"
 			base.debugmsg(9, "concat:", concat)
 			hyper = "=HYPERLINK(" + concat + ",\"" + heading_text + "\")"
 			base.debugmsg(8, "hyper:", hyper)
+			c.style = "Default"
 			c.value = hyper
 
 		if level < maxlevel:
 			if len(sections) > 0:
 				for sect in sections:
 					self.xlsx_sections_contents_row(sect, maxlevel, mode)
 
@@ -7168,28 +7181,28 @@
 			numarr = titlenum.split(".")
 			base.debugmsg(5, "numarr:", numarr)
 			pagenum = int(numarr[0]) + 1
 			base.debugmsg(5, "pagenum:", pagenum)
 
 			colnum = 1
 			cellname = "{}_{}".format(id, colnum)
-			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(titlenum))
+			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(titlenum), style='Report.TLabel')
 			self.contentdata[fid][cellname].grid(column=colnum, row=rownum, sticky="nsew")
 
 			colnum += 1
 			cellname = "{}_{}".format(id, colnum)
-			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(titlename))
+			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(titlename), style='Report.TLabel')
 			self.contentdata[fid][cellname].grid(column=colnum, row=rownum, sticky="nsew")
 
 			colnum += 1
 			self.contentdata[fid]["fmeTOC"].columnconfigure(colnum, weight=1)
 
 			colnum += 1
 			cellname = "{}_{}".format(id, colnum)
-			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(pagenum))
+			self.contentdata[fid][cellname] = ttk.Label(self.contentdata[fid]["fmeTOC"], text=str(pagenum), style='Report.TLabel')
 			self.contentdata[fid][cellname].grid(column=colnum, row=rownum, sticky="nsew")
 
 			nextrow = rownum + 1
 
 		base.debugmsg(9, "nextrow:", nextrow)
 		if level < flevel:
 			children = base.report_get_order(id)
```

### Comparing `rfswarm-reporter-1.1.1/rfswarm_reporter.egg-info/PKG-INFO` & `rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.1
+Version: 1.1.2
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.1/setup-reporter.py` & `rfswarm-reporter-1.1.2/setup-reporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-reporter",
-	version="1.1.1",
+	version="1.1.2",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm reporter",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_manag*", "*fswarm_agen*", "build/*"]),
```

