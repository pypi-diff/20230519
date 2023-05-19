# Comparing `tmp/webslides-0.6.0.tar.gz` & `tmp/webslides-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webslides-0.6.0.tar", last modified: Wed Apr 19 08:26:13 2023, max compression
+gzip compressed data, was "webslides-0.6.3.tar", last modified: Fri May 19 07:47:03 2023, max compression
```

## Comparing `webslides-0.6.0.tar` & `webslides-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.089781 webslides-0.6.0/
--rw-rw-rw-   0        0        0       49 2023-04-17 08:03:59.000000 webslides-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6806 2023-04-19 08:26:13.088779 webslides-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     6464 2023-04-19 08:10:18.000000 webslides-0.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 08:26:13.089781 webslides-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-04-19 08:12:08.000000 webslides-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:26:12.845775 webslides-0.6.0/webslides/
--rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.6.0/webslides/__init__.py
--rw-rw-rw-   0        0        0     5025 2023-04-17 08:28:07.000000 webslides-0.6.0/webslides/main.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.014781 webslides-0.6.0/webslides/modules/
-drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.080778 webslides-0.6.0/webslides/modules/__pycache__/
--rw-rw-rw-   0        0        0     4741 2023-04-19 08:25:34.000000 webslides-0.6.0/webslides/modules/__pycache__/demo.cpython-310.pyc
--rw-rw-rw-   0        0        0     2562 2023-04-16 15:26:29.000000 webslides-0.6.0/webslides/modules/__pycache__/generate.cpython-310.pyc
--rw-rw-rw-   0        0        0     2445 2023-04-16 18:33:07.000000 webslides-0.6.0/webslides/modules/__pycache__/input_validations.cpython-310.pyc
--rw-rw-rw-   0        0        0     1792 2023-04-16 17:27:37.000000 webslides-0.6.0/webslides/modules/__pycache__/other.cpython-310.pyc
--rw-rw-rw-   0        0        0     1928 2023-04-19 08:10:22.000000 webslides-0.6.0/webslides/modules/__pycache__/pagination.cpython-310.pyc
--rw-rw-rw-   0        0        0     6342 2023-04-17 05:45:38.000000 webslides-0.6.0/webslides/modules/__pycache__/tohtml.cpython-310.pyc
--rw-rw-rw-   0        0        0     5950 2023-04-19 08:26:09.000000 webslides-0.6.0/webslides/modules/demo.py
--rw-rw-rw-   0        0        0    11267 2023-04-17 08:19:41.000000 webslides-0.6.0/webslides/modules/df_demo.html
--rw-rw-rw-   0        0        0    14255 2023-04-17 07:31:42.000000 webslides-0.6.0/webslides/modules/folium_demo.html
--rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.6.0/webslides/modules/generate.py
--rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.6.0/webslides/modules/hello_world.py
--rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.6.0/webslides/modules/input_validations.py
--rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.6.0/webslides/modules/other.py
--rw-rw-rw-   0        0        0     2999 2023-04-19 08:10:18.000000 webslides-0.6.0/webslides/modules/pagination.py
--rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.6.0/webslides/modules/tohtml.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:26:12.897776 webslides-0.6.0/webslides.egg-info/
--rw-rw-rw-   0        0        0     6806 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 07:47:03.238621 webslides-0.6.3/
+-rw-rw-rw-   0        0        0       49 2023-04-17 08:03:59.000000 webslides-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7086 2023-05-19 07:47:03.236619 webslides-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6744 2023-05-19 07:47:01.000000 webslides-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 07:47:03.238621 webslides-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      537 2023-05-19 07:47:01.000000 webslides-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:47:02.899613 webslides-0.6.3/webslides/
+-rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.6.3/webslides/__init__.py
+-rw-rw-rw-   0        0        0     5816 2023-05-19 06:33:40.000000 webslides-0.6.3/webslides/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:47:03.195618 webslides-0.6.3/webslides/modules/
+drwxrwxrwx   0        0        0        0 2023-05-19 07:47:03.232617 webslides-0.6.3/webslides/modules/__pycache__/
+-rw-rw-rw-   0        0        0     5355 2023-05-19 06:35:38.000000 webslides-0.6.3/webslides/modules/__pycache__/demo.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2974 2023-05-19 06:35:38.000000 webslides-0.6.3/webslides/modules/__pycache__/generate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2464 2023-05-09 11:54:12.000000 webslides-0.6.3/webslides/modules/__pycache__/input_validations.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1940 2023-05-19 06:49:25.000000 webslides-0.6.3/webslides/modules/__pycache__/other.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1958 2023-05-09 12:10:03.000000 webslides-0.6.3/webslides/modules/__pycache__/pagination.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6711 2023-05-09 12:20:41.000000 webslides-0.6.3/webslides/modules/__pycache__/tohtml.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12847 2023-05-19 06:59:20.000000 webslides-0.6.3/webslides/modules/demo.py
+-rw-rw-rw-   0        0        0    11267 2023-04-17 08:19:41.000000 webslides-0.6.3/webslides/modules/df_demo.html
+-rw-rw-rw-   0        0        0    14255 2023-04-17 07:31:42.000000 webslides-0.6.3/webslides/modules/folium_demo.html
+-rw-rw-rw-   0        0        0     4674 2023-05-19 06:33:40.000000 webslides-0.6.3/webslides/modules/generate.py
+-rw-rw-rw-   0        0        0     2919 2023-05-19 06:49:59.000000 webslides-0.6.3/webslides/modules/hello_world.py
+-rw-rw-rw-   0        0        0     2853 2023-05-09 11:54:10.000000 webslides-0.6.3/webslides/modules/input_validations.py
+-rw-rw-rw-   0        0        0     1933 2023-05-19 06:40:15.000000 webslides-0.6.3/webslides/modules/other.py
+-rw-rw-rw-   0        0        0     3049 2023-05-09 12:10:01.000000 webslides-0.6.3/webslides/modules/pagination.py
+-rw-rw-rw-   0        0        0     8489 2023-05-09 12:20:40.000000 webslides-0.6.3/webslides/modules/tohtml.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:47:02.977612 webslides-0.6.3/webslides.egg-info/
+-rw-rw-rw-   0        0        0     7086 2023-05-19 07:47:02.000000 webslides-0.6.3/webslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-19 07:47:02.000000 webslides-0.6.3/webslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 07:47:02.000000 webslides-0.6.3/webslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 07:47:02.000000 webslides-0.6.3/webslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 07:47:02.000000 webslides-0.6.3/webslides.egg-info/top_level.txt
```

### Comparing `webslides-0.6.0/PKG-INFO` & `webslides-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.6.0
+Version: 0.6.3
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## [live demo](https://datadept.nl/webslides/demo.html)
+## [Live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
@@ -32,15 +32,16 @@
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
 - No WYSIWYG editing in a graphical user interface
-- No easy conversion to PDF
+- No easy conversion to PDF / printable
+- No custom styling (ie. company style)
 
 ## Main Features
 
 Here are some of the things that Webslides does well:
 
 - Generate an index page based on your content
 - Generate a highlights page, based on your content
@@ -51,15 +52,15 @@
 
 Webslides has two dependencies:
 
 - Pandas: a Python package that provides fast, flexible, and expressive data structures for data analysis
 - Plotly: an interactive data visualization library that allows you to create a wide range of charts, graphs, and other visualizations
 
 Webslides uses Pandas to process the content that is included in your presentation.
-The Plotly package is used to convert Plotly figure opjects to HTML.
+The Plotly package is used to convert Plotly figure objects to HTML.
 
 ## Installation
 
 To install Webslides, simply run the following command:
 
 `pip install webslides`
 
@@ -133,23 +134,23 @@
 - **content** (dict, _optional_, default=None): A dictionary containing the content pages organized by top categories and subcategories.
 
 
   Example input:
 ```
 content = {
     'Topcat A': {
-        'Subcat X': [
-            {
+        'Subcat X': {
+            'page1': {
                 'title': 'Page Title 1 - HTML body',
                 'highlights': ['- highlight 1', '- highlight 2'],
                 'body': 'Content 1: this is a <b>HTML string</b>',
                 'footer': ['- footer 1a', '- <i>italic footer 1b</i>'],
                 'show': True},
                 ...
-            ],
+            },
         ...
         },
     ...
 }
 ```
 - **fname** (str, _optional_, default='output.html'): The output filename for the generated HTML file.
 
@@ -161,14 +162,16 @@
 
 - **show_topcat** (bool, _optional_, default=True): If set to True, the top category will be displayed in the index and highlights pages.
 
 - **show_subcat** (bool, _optional_, default=True): If set to True, the subcategory will be displayed in the index and highlights pages.
 
 - **show_highlights_only** (bool, _optional_, default=False): If set to True, only content pages with highlights will be shown in the index and highlights pages.
 
+- **tooltips** (dict, _optional_, default=None): Dictionary with keys 'topcats' and 'subcats' and with topcat/subcat as keys, with each a dict wit keys and values with the respective topcat names and tooltip texts.
+
 ## Page Dictionary Parameters
 
 Each content page dictionary within the content parameter can include the following keys:
 
 - **title** (str, _mandatory_): The title of the content page.
 
 - **body** (str or object, _mandatory_): The body of the content page. It can be a string containing HTML or an object (e.g., a Plotly figure).
```

### Comparing `webslides-0.6.0/README.md` & `webslides-0.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## [live demo](https://datadept.nl/webslides/demo.html)
+## [Live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
@@ -21,15 +21,16 @@
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
 - No WYSIWYG editing in a graphical user interface
-- No easy conversion to PDF
+- No easy conversion to PDF / printable
+- No custom styling (ie. company style)
 
 ## Main Features
 
 Here are some of the things that Webslides does well:
 
 - Generate an index page based on your content
 - Generate a highlights page, based on your content
@@ -40,15 +41,15 @@
 
 Webslides has two dependencies:
 
 - Pandas: a Python package that provides fast, flexible, and expressive data structures for data analysis
 - Plotly: an interactive data visualization library that allows you to create a wide range of charts, graphs, and other visualizations
 
 Webslides uses Pandas to process the content that is included in your presentation.
-The Plotly package is used to convert Plotly figure opjects to HTML.
+The Plotly package is used to convert Plotly figure objects to HTML.
 
 ## Installation
 
 To install Webslides, simply run the following command:
 
 `pip install webslides`
 
@@ -122,23 +123,23 @@
 - **content** (dict, _optional_, default=None): A dictionary containing the content pages organized by top categories and subcategories.
 
 
   Example input:
 ```
 content = {
     'Topcat A': {
-        'Subcat X': [
-            {
+        'Subcat X': {
+            'page1': {
                 'title': 'Page Title 1 - HTML body',
                 'highlights': ['- highlight 1', '- highlight 2'],
                 'body': 'Content 1: this is a <b>HTML string</b>',
                 'footer': ['- footer 1a', '- <i>italic footer 1b</i>'],
                 'show': True},
                 ...
-            ],
+            },
         ...
         },
     ...
 }
 ```
 - **fname** (str, _optional_, default='output.html'): The output filename for the generated HTML file.
 
@@ -150,14 +151,16 @@
 
 - **show_topcat** (bool, _optional_, default=True): If set to True, the top category will be displayed in the index and highlights pages.
 
 - **show_subcat** (bool, _optional_, default=True): If set to True, the subcategory will be displayed in the index and highlights pages.
 
 - **show_highlights_only** (bool, _optional_, default=False): If set to True, only content pages with highlights will be shown in the index and highlights pages.
 
+- **tooltips** (dict, _optional_, default=None): Dictionary with keys 'topcats' and 'subcats' and with topcat/subcat as keys, with each a dict wit keys and values with the respective topcat names and tooltip texts.
+
 ## Page Dictionary Parameters
 
 Each content page dictionary within the content parameter can include the following keys:
 
 - **title** (str, _mandatory_): The title of the content page.
 
 - **body** (str or object, _mandatory_): The body of the content page. It can be a string containing HTML or an object (e.g., a Plotly figure).
```

### Comparing `webslides-0.6.0/setup.py` & `webslides-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="webslides",
-    version="0.6.0",
+    version="0.6.3",
     author="Derk-Jan Woltjer",
     author_email="derkjan.woltjer@gmail.com",
     description="Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     licence="MIT License",
     packages=find_packages(),
```

### Comparing `webslides-0.6.0/webslides/main.py` & `webslides-0.6.3/webslides/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from webslides.modules.tohtml import *
 from webslides.modules.generate import *
 from webslides.modules.pagination import *
 from webslides.modules.input_validations import *
 
 def create(content=None
            , title_page=None
-           , fname='output.html'
+           , fname=None
            , open_in_browser=True
+           , show_title_page=True
            , show_index_page=False
            , show_highlights_page=False
            , show_topcat=True
            , show_subcat=True
-           , show_highlights_only=False):
+           , show_highlights_only=False
+           , tooltips=dict()):
     """
     param pd (pagedata): list of lists with html strings or plotly fig objects ie.
         [[titlepage],[hl_page_title,hl_page_content],
         [index_page_title,index_page_content],
         [content_page1_title,content_page1_comments,content_page1_fig],
         [content_page2_title,content_page2_comments,content_page2_fig]]
     param fname: str filename for output file. If not provided defaults to 'output.html')
@@ -54,24 +56,24 @@
     html = """
     <html>
     <head><meta charset="utf-8" />
     <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
     <style>
     .page {padding:50px; margin:100px; box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;}
     body {font-family: "Arial";} a {text-decoration: none;}
-    </style>
+    </style>    
     </head>
     <body>
     <span></span>
     </body>
     </html>
     """
 
     # 1. title page
-    if title_page:
+    if title_page and show_title_page:
         page = {'title': title_page.get('title', ''),
                 'img_url': title_page.get('img_url', ''),
                 'summary': title_page.get('summary', ''),
                 'footer': title_page.get('footer', list())}
 
         # start new page
         html = html.replace('<span></span>', '<div class="page"><span></span></div>')
@@ -83,26 +85,26 @@
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     # 2. index page
     if show_index_page:
         # start new page
         html = html.replace('<span></span>', '<div class="page"><span></span></div>')
 
-        indexpage_html = generate_index_page(df, show_topcat=show_topcat, show_subcat=show_subcat)
+        indexpage_html = generate_index_page(df, show_topcat=show_topcat, show_subcat=show_subcat, tooltips=tooltips)
         html = html.replace('<span></span>', indexpage_html + '<span></span>')
 
         # close page
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     # 3. highlights page
     if show_highlights_page:
         # start new page
         html = html.replace('<span></span>', '<div class="page"><span></span></div>')
 
-        hlpage_html = generate_highlights_page(df, show_topcat=show_topcat, show_subcat=show_subcat)
+        hlpage_html = generate_highlights_page(df, show_topcat=show_topcat, show_subcat=show_subcat, tooltips=tooltips)
         html = html.replace('<span></span>', hlpage_html + '<span></span>')
 
         # close page
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     # 4. content pages
     for idx, page in df.iterrows():
@@ -111,36 +113,55 @@
 
         # insert content html
         html = content_to_html(html, page,
                                show_topcat=show_topcat,
                                show_subcat=show_subcat,
                                show_index_page=show_index_page,
                                show_highlights_page=show_highlights_page,
-                               show_navi=True)
+                               show_navi=True,
+                               tooltips=tooltips)
 
         # close page
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     ###################
     ## HANDLE OUTPUT ##
     ###################
 
-    # create output directory 'wsout' if not present
+    # default output = wsout/output.html
+    if not fname or fname == '':
+        fname = 'output.html'
     current_working_dir = os.getcwd()
-    fpath = os.path.join(current_working_dir, 'wsout')
+    fpath = os.path.join(current_working_dir, 'wsout', fname)
+    wsoutpath = os.path.join(current_working_dir, 'wsout')
+
+    # test if fname contains filename (with extension) or just base
+    base, ext = os.path.splitext(fname)
+
+    # fname contains a filename
+    if ext:
+        if os.path.exists(fname) or os.path.exists(base):
+            fpath = fname
 
-    if not os.path.exists(fpath):
-        os.makedirs(fpath)
+    # fname only contains directory name
+    else:
+        if os.path.isdir(fname):
+            fpath = os.path.join(fname, 'output.html')
+        else:
+            fpath = os.path.join(current_working_dir, 'wsout', 'output.html')
+
+    # create output directory 'wsout' if not present
+    if 'wsout' in fpath and not os.path.exists(wsoutpath):
+        os.makedirs(wsoutpath)
 
-    with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8') as f:
+    with codecs.open(f"{fpath}", "w", encoding='utf-8') as f:
         f.write(html)
-        print(f'output saved as wsout/{fname}')
+        print(f'output saved as {fpath}')
 
 
+    # open in browser to check result
     if open_in_browser:
-        # open in browser to check result
-        htmlfile = f"{fpath}/{fname}"
-        webbrowser.open(htmlfile)
-        print(f'opened in browser wsout/{fname}')
+        webbrowser.open(fpath)
+        print(f'opened in browser {fpath}')
 
     return None
```

#### html2text {}

```diff
@@ -1,55 +1,62 @@
 import os import sys import codecs import webbrowser from
 webslides.modules.tohtml import * from webslides.modules.generate import * from
 webslides.modules.pagination import * from webslides.modules.input_validations
-import * def create(content=None , title_page=None , fname='output.html' ,
-open_in_browser=True , show_index_page=False , show_highlights_page=False ,
-show_topcat=True , show_subcat=True , show_highlights_only=False): """ param pd
-(pagedata): list of lists with html strings or plotly fig objects ie. [
-[titlepage],[hl_page_title,hl_page_content],
-[index_page_title,index_page_content],
+import * def create(content=None , title_page=None , fname=None ,
+open_in_browser=True , show_title_page=True , show_index_page=False ,
+show_highlights_page=False , show_topcat=True , show_subcat=True ,
+show_highlights_only=False , tooltips=dict()): """ param pd (pagedata): list of
+lists with html strings or plotly fig objects ie. [[titlepage],
+[hl_page_title,hl_page_content], [index_page_title,index_page_content],
 [content_page1_title,content_page1_comments,content_page1_fig],
 [content_page2_title,content_page2_comments,content_page2_fig]] param fname:
 str filename for output file. If not provided defaults to 'output.html') param
 write: bool, False will only output to screen, True will write file AND output
 to screen return: str html code """ # INPUT VALIDATIONS if title_page:
 title_error = validate_title_page(title_page) if title_error: print
 (title_error) return if content: content_error = validate_content(content) if
 content_error: print(content_error) return else: print('content variable is
 mandatory') # create dataframe from pagedata list and enrich with pagination
 data df = pagination_data(content=content,
 show_highlights_only=show_highlights_only) ################# ## CREATE HTML ##
 ################# # page shadow css options: https://getcssscan.com/css-box-
 shadow-examples html = """
-""" # 1. title page if title_page: page = {'title': title_page.get('title',
-''), 'img_url': title_page.get('img_url', ''), 'summary': title_page.get
-('summary', ''), 'footer': title_page.get('footer', list())} # start new page
-html = html.replace('', '
+""" # 1. title page if title_page and show_title_page: page = {'title':
+title_page.get('title', ''), 'img_url': title_page.get('img_url', ''),
+'summary': title_page.get('summary', ''), 'footer': title_page.get('footer',
+list())} # start new page html = html.replace('', '
 ') # reuse contenpage_to_html function (normally used for contenslides) html =
 titlepage_to_html(html, page) # close page html = html.replace('
 ', '
 ') # 2. index page if show_index_page: # start new page html = html.replace('',
 '
 ') indexpage_html = generate_index_page(df, show_topcat=show_topcat,
-show_subcat=show_subcat) html = html.replace('', indexpage_html + '') # close
-page html = html.replace('
+show_subcat=show_subcat, tooltips=tooltips) html = html.replace('',
+indexpage_html + '') # close page html = html.replace('
 ', '
 ') # 3. highlights page if show_highlights_page: # start new page html =
 html.replace('', '
 ') hlpage_html = generate_highlights_page(df, show_topcat=show_topcat,
-show_subcat=show_subcat) html = html.replace('', hlpage_html + '') # close page
-html = html.replace('
+show_subcat=show_subcat, tooltips=tooltips) html = html.replace('', hlpage_html
++ '') # close page html = html.replace('
 ', '
 ') # 4. content pages for idx, page in df.iterrows(): # start new page html =
 html.replace('', '
 ') # insert content html html = content_to_html(html, page,
 show_topcat=show_topcat, show_subcat=show_subcat,
 show_index_page=show_index_page, show_highlights_page=show_highlights_page,
-show_navi=True) # close page html = html.replace('
+show_navi=True, tooltips=tooltips) # close page html = html.replace('
 ', '
-') ################### ## HANDLE OUTPUT ## ################### # create output
-directory 'wsout' if not present current_working_dir = os.getcwd() fpath =
-os.path.join(current_working_dir, 'wsout') if not os.path.exists(fpath):
-os.makedirs(fpath) with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8')
-as f: f.write(html) print(f'output saved as wsout/{fname}') if open_in_browser:
-# open in browser to check result htmlfile = f"{fpath}/{fname}" webbrowser.open
-(htmlfile) print(f'opened in browser wsout/{fname}') return None
+') ################### ## HANDLE OUTPUT ## ################### # default output
+= wsout/output.html if not fname or fname == '': fname = 'output.html'
+current_working_dir = os.getcwd() fpath = os.path.join(current_working_dir,
+'wsout', fname) wsoutpath = os.path.join(current_working_dir, 'wsout') # test
+if fname contains filename (with extension) or just base base, ext =
+os.path.splitext(fname) # fname contains a filename if ext: if os.path.exists
+(fname) or os.path.exists(base): fpath = fname # fname only contains directory
+name else: if os.path.isdir(fname): fpath = os.path.join(fname, 'output.html')
+else: fpath = os.path.join(current_working_dir, 'wsout', 'output.html') #
+create output directory 'wsout' if not present if 'wsout' in fpath and not
+os.path.exists(wsoutpath): os.makedirs(wsoutpath) with codecs.open(f"{fpath}",
+"w", encoding='utf-8') as f: f.write(html) print(f'output saved as {fpath}') #
+open in browser to check result if open_in_browser: webbrowser.open(fpath)
+print(f'opened in browser {fpath}') return None
```

### Comparing `webslides-0.6.0/webslides/modules/__pycache__/demo.cpython-310.pyc` & `webslides-0.6.3/webslides/modules/__pycache__/demo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 19 08:25:32 2023 UTC, .py size: 5948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7ca5 3f64 3c17 0000  o.......|.?d<...
+00000000: 6f0d 0d0a 0000 0000 b818 6764 2d32 0000  o.........gd-2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6401 6c05 6d06 5a07  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6405  d.l.m.Z.m.Z...d.
 00000070: 6406 8400 5a0d 6407 6408 8400 5a0e 6409  d...Z.d.d...Z.d.
@@ -64,234 +64,272 @@
 000003f0: 0029 034e 7a0c 6466 5f64 656d 6f2e 6874  .).Nz.df_demo.ht
 00000400: 6d6c 721d 0000 0072 1e00 0000 2905 7227  mlr....r....).r'
 00000410: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
 00000420: 0000 da07 6466 5f68 746d 6c72 1900 0000  ....df_htmlr....
 00000430: 7219 0000 0072 1a00 0000 da0c 6465 6d6f  r....r......demo
 00000440: 5f64 665f 6874 6d6c 1d00 0000 722d 0000  _df_html....r-..
 00000450: 0072 2f00 0000 6300 0000 0000 0000 0000  .r/...c.........
-00000460: 0000 0002 0000 000b 0000 0043 0000 0073  ...........C...s
-00000470: d800 0000 6401 6402 6403 6404 6405 6406  ....d.d.d.d.d.d.
+00000460: 0000 0003 0000 000d 0000 0043 0000 0073  ...........C...s
+00000470: 9c01 0000 6401 6402 6403 6404 6405 6406  ....d.d.d.d.d.d.
 00000480: 9c03 6407 9c03 7d00 6408 6409 640a 6701  ..d...}.d.d.d.g.
 00000490: 640b 6700 640c a201 640d 9c04 640e 640f  d.g.d...d...d.d.
 000004a0: 6410 6702 7400 8300 6411 6701 640d 9c04  d.g.t...d.g.d...
 000004b0: 6412 6413 6701 7401 8300 6414 6701 640d  d.d.g.t...d.g.d.
 000004c0: 9c04 6415 6416 6417 6702 7402 8300 6418  ..d.d.d.g.t...d.
 000004d0: 6419 6702 640d 9c04 641a 641b 6701 641c  d.g.d...d.d.g.d.
 000004e0: 641d 6701 640d 9c04 6705 6901 641e 641f  d.g.d...g.i.d.d.
 000004f0: 6420 6701 7403 6421 8301 6422 9c03 6423  d g.t.d!..d"..d#
 00000500: 6424 6701 7403 6425 8301 6426 6701 640d  d$g.t.d%..d&g.d.
 00000510: 9c04 6427 6428 6701 7404 8300 6429 6701  ..d'd(g.t...d)g.
-00000520: 640d 9c04 6703 6901 642a 9c02 7d01 7405  d...g.i.d*..}.t.
-00000530: 7c01 7c00 642b 642c 642c 642c 642c 642c  |.|.d+d,d,d,d,d,
-00000540: 642d 642e 8d09 0100 642f 5300 2930 7a40  d-d.....d/S.)0z@
-00000550: 4372 6561 7465 7320 646f 6375 6d65 6e74  Creates document
-00000560: 6174 696f 6e20 6578 706c 6169 6e69 6e67  ation explaining
-00000570: 2077 6879 2061 6e64 2068 6f77 2074 6f20   why and how to 
-00000580: 7573 6520 7468 6973 2070 6163 6b61 6765  use this package
-00000590: da00 7a17 5765 6273 6c69 6465 7320 446f  ..z.Webslides Do
-000005a0: 6375 6d65 6e74 6174 696f 6e7a b157 6562  cumentationz.Web
-000005b0: 736c 6964 6573 2069 7320 6120 5079 7468  slides is a Pyth
-000005c0: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
-000005d0: 6372 6561 7465 7320 4854 4d4c 2070 7265  creates HTML pre
-000005e0: 7365 6e74 6174 696f 6e73 203c 623e 6c69  sentations <b>li
-000005f0: 6b65 2074 6869 7320 6f6e 653c 2f62 3e2e  ke this one</b>.
-00000600: 3c62 723e 4974 2065 6e61 626c 6573 2065  <br>It enables e
-00000610: 6173 7920 7368 6172 696e 6720 6f66 2050  asy sharing of P
-00000620: 7974 686f 6e2d 6765 6e65 7261 7465 6420  ython-generated 
-00000630: 636f 6e74 656e 7420 7375 6368 2061 7320  content such as 
-00000640: 6368 6172 7473 2c20 6f74 6865 7220 7669  charts, other vi
-00000650: 7375 616c 7320 616e 6420 6461 7461 7a5a  suals and datazZ
-00000660: 5468 6973 2070 7265 7365 6e74 6174 696f  This presentatio
-00000670: 6e20 6465 6d6f 6e73 7472 6174 6573 2066  n demonstrates f
-00000680: 6561 7475 7265 7320 6f66 2074 6865 2048  eatures of the H
-00000690: 544d 4c20 666f 726d 6174 2061 6e64 2073  TML format and s
-000006a0: 686f 756c 6420 6865 6c70 2079 6f75 2067  hould help you g
-000006b0: 6574 2073 7461 7274 6564 7a55 3c61 2068  et startedzU<a h
-000006c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
-000006d0: 692e 6f72 672f 7072 6f6a 6563 742f 7765  i.org/project/we
-000006e0: 6273 6c69 6465 732f 223e 6874 7470 733a  bslides/">https:
-000006f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000700: 6374 2f77 6562 736c 6964 6573 2f3c 2f61  ct/webslides/</a
-00000710: 3e29 03da 0541 626f 7574 da08 436f 6e74  >)...About..Cont
-00000720: 656e 7473 da04 5079 5069 2903 da07 696d  ents..PyPi)...im
-00000730: 675f 7572 6c72 1000 0000 da07 7375 6d6d  g_urlr......summ
-00000740: 6172 797a 1a41 6476 616e 7461 6765 7320  aryz.Advantages 
-00000750: 6f76 6572 2050 6f77 6572 706f 696e 747a  over Powerpointz
-00000760: 1244 796e 616d 6963 2070 6167 656c 656e  .Dynamic pagelen
-00000770: 6774 687a 3b2d 2050 6167 6573 2063 616e  gthz;- Pages can
-00000780: 2062 6520 6173 206c 6f6e 6720 286f 7220   be as long (or 
-00000790: 7368 6f72 7429 2061 7320 6e65 6564 6564  short) as needed
-000007a0: 2c20 6c69 6b65 2074 6869 7320 6f6e 6521  , like this one!
-000007b0: 753e 0000 004e 6f74 6869 6e67 206d 7563  u>...Nothing muc
-000007c0: 6820 6f6e 2074 6869 7320 7061 6765 2072  h on this page r
-000007d0: 6561 6c6c 792c 2074 6861 7427 7320 7768  eally, that's wh
-000007e0: 7920 6974 7320 736f 2073 686f 7274 20f0  y its so short .
-000007f0: 9f98 8929 037a 2a2d 2061 6e64 2061 6464  ...).z*- and add
-00000800: 696e 6720 6120 666f 6f74 6572 2063 616e  ing a footer can
-00000810: 2062 6520 7573 6566 756c 6c20 746f 6f2e   be usefull too.
-00000820: 2e7a 462d 2070 732e 2048 6176 6520 796f  .zF- ps. Have yo
-00000830: 7520 6e6f 7465 6420 7468 6520 7061 6765  u noted the page
-00000840: 206e 6176 6967 6174 696f 6e20 6f6e 2074   navigation on t
-00000850: 6865 2074 6f70 2072 6967 6874 206f 6620  he top right of 
-00000860: 7468 6520 7061 6765 3f7a b42d 2026 2378  the page?z.- &#x
-00000870: 3146 3441 313b 3a20 7468 6973 206d 6172  1F4A1;: this mar
-00000880: 6b73 2070 6167 6573 2077 6974 6820 6120  ks pages with a 
-00000890: 6869 6768 6c69 6768 742e 2049 6620 6120  highlight. If a 
-000008a0: 7061 6765 2068 6173 206e 6f20 6869 6768  page has no high
-000008b0: 6c69 6768 7473 2028 7265 6d61 726b 7320  lights (remarks 
-000008c0: 696e 2067 7265 7920 6172 6561 2920 6974  in grey area) it
-000008d0: 2069 7320 6e6f 7420 7368 6f77 6e20 696e   is not shown in
-000008e0: 2074 6865 2068 6967 686c 6967 6874 2073   the highlight s
-000008f0: 756d 6d61 7279 2070 6167 6520 6e6f 7220  ummary page nor 
-00000900: 6d61 726b 6564 2069 6e20 7468 6520 7461  marked in the ta
-00000910: 626c 6520 6f66 2063 6f6e 7465 6e74 7329  ble of contents)
-00000920: 0472 1000 0000 da0a 6869 6768 6c69 6768  .r......highligh
-00000930: 7473 da04 626f 6479 da06 666f 6f74 6572  ts..body..footer
-00000940: 7a13 496e 7465 7261 6374 6976 6520 636f  z.Interactive co
-00000950: 6e74 656e 747a 602d 204e 6174 6976 6520  ntentz`- Native 
-00000960: 506c 6f74 6c79 2067 7261 7068 206f 6a65  Plotly graph oje
-00000970: 6374 7320 6361 6e20 6265 2069 6e73 6572  cts can be inser
-00000980: 7465 6420 6173 2063 6f6e 7465 6e74 2c20  ted as content, 
-00000990: 616e 6420 7468 6579 2068 6176 6520 6d61  and they have ma
-000009a0: 6e79 2069 6e74 6572 6163 7469 7665 2066  ny interactive f
-000009b0: 6561 7475 7265 737a 702d 2054 7279 207a  eatureszp- Try z
-000009c0: 6f6f 6d69 6e67 2069 6e20 7468 6520 6279  ooming in the by
-000009d0: 2064 7261 6767 696e 6720 6120 7769 6e64   dragging a wind
-000009e0: 6f77 2069 6e20 7468 6520 706c 6f74 2e20  ow in the plot. 
-000009f0: 4f72 2074 6f67 676c 6520 7669 7369 6269  Or toggle visibi
-00000a00: 6c69 7479 206f 6620 6120 6461 7461 2073  lity of a data s
-00000a10: 6572 6965 7320 7669 6120 7468 6520 6c65  eries via the le
-00000a20: 6765 6e64 206b 6579 737a 462d 204c 696e  gend keyszF- Lin
-00000a30: 6b20 746f 2050 6c6f 746c 7920 6761 6c6c  k to Plotly gall
-00000a40: 6572 7920 3c61 2068 7265 663d 2268 7474  ery <a href="htt
-00000a50: 7073 3a2f 2f70 6c6f 746c 792e 636f 6d2f  ps://plotly.com/
-00000a60: 7079 7468 6f6e 2f22 3e68 6572 653c 2f61  python/">here</a
-00000a70: 3e7a 1c41 6e79 2048 544d 4c20 636f 6e74  >z.Any HTML cont
-00000a80: 656e 7420 7769 6c6c 2072 656e 6465 727a  ent will renderz
-00000a90: 162d 2046 6f72 2065 7861 6d70 6c65 2074  .- For example t
-00000aa0: 6869 7320 6d61 707a 662d 2074 6869 7320  his mapzf- this 
-00000ab0: 6d61 7020 7761 7320 6372 6561 7465 6420  map was created 
-00000ac0: 7769 7468 2046 6f6c 6975 6d20 283c 6120  with Folium (<a 
-00000ad0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000ae0: 7468 6f6e 2d76 6973 7561 6c69 7a61 7469  thon-visualizati
-00000af0: 6f6e 2e67 6974 6875 622e 696f 2f66 6f6c  on.github.io/fol
-00000b00: 6975 6d2f 223e 646f 6373 3c2f 613e 297a  ium/">docs</a>)z
-00000b10: 1853 7479 6c65 6420 5061 6e64 6173 2044  .Styled Pandas D
-00000b20: 6174 6166 7261 6d65 737a 272d 2057 6f77  ataframesz'- Wow
-00000b30: 2c20 6e6f 7469 6365 2074 6861 7420 6d61  , notice that ma
-00000b40: 7820 7661 6c75 6520 6d61 726b 6564 2072  x value marked r
-00000b50: 6564 7a2f 2d20 4e6f 7420 746f 206d 656e  edz/- Not to men
-00000b60: 7469 6f6e 2074 6865 206c 6f77 6573 7420  tion the lowest 
-00000b70: 7661 6c75 652c 206d 6172 6b65 6420 6772  value, marked gr
-00000b80: 6565 6e7a 602d 2073 7479 6c69 6e67 206f  eenz`- styling o
-00000b90: 6620 6120 7061 6e64 6173 2064 6174 6166  f a pandas dataf
-00000ba0: 7261 6d65 2063 616e 2062 6520 646f 6e65  rame can be done
-00000bb0: 2062 7920 6372 6561 7469 6e67 2061 2073   by creating a s
-00000bc0: 7479 6c65 7220 6f62 6a65 6374 2061 6e64  tyler object and
-00000bd0: 2063 6f6e 7665 7274 2074 6861 7420 746f   convert that to
-00000be0: 2068 746d 6c7a 5b2d 2069 652e 2073 7479   htmlz[- ie. sty
-00000bf0: 6c65 645f 6466 203d 2064 662e 7374 796c  led_df = df.styl
-00000c00: 652e 6261 636b 6772 6f75 6e64 5f67 7261  e.background_gra
-00000c10: 6469 656e 7428 636d 6170 3d27 426c 7565  dient(cmap='Blue
-00000c20: 7327 2920 616e 6420 6874 6d6c 203d 2073  s') and html = s
-00000c30: 7479 6c65 645f 6466 2e74 6f5f 6874 6d6c  tyled_df.to_html
-00000c40: 2829 7a14 5375 7065 7220 7370 6565 6420  ()z.Super speed 
-00000c50: 7570 6461 7465 7321 7a69 2d20 4120 6b65  updates!zi- A ke
-00000c60: 7920 6164 7661 6e74 6167 6520 6f66 2074  y advantage of t
-00000c70: 6869 7320 7072 6573 656e 7461 7469 6f6e  his presentation
-00000c80: 2066 6f72 6d20 6d61 7920 6265 2074 6861   form may be tha
-00000c90: 7420 7570 6461 7465 7320 6f6e 6c79 2072  t updates only r
-00000ca0: 6571 7569 7265 2074 6865 203c 693e 7072  equire the <i>pr
-00000cb0: 6573 7320 6f66 2061 2062 7574 746f 6e3c  ess of a button<
-00000cc0: 2f69 3e75 dc00 0000 5665 7279 206f 6674  /i>u....Very oft
-00000cd0: 656e 2064 6174 612c 2061 6e61 6c79 7369  en data, analysi
-00000ce0: 7320 636f 6e6c 7573 696f 6e73 2061 6e64  s conlusions and
-00000cf0: 206f 7468 6572 2063 6f6e 7465 6e74 2069   other content i
-00000d00: 7320 7265 7669 7365 6420 696e 2067 6574  s revised in get
-00000d10: 7469 6e67 2074 6f20 6120 6669 6e61 6c20  ting to a final 
-00000d20: 7665 7273 696f 6e20 6f66 2061 2070 7265  version of a pre
-00000d30: 7365 6e74 6174 696f 6e2e 2053 696e 6365  sentation. Since
-00000d40: 2061 6c6c 2069 7320 696e 2070 7974 686f   all is in pytho
-00000d50: 6e20 7363 7269 7074 2c20 7570 6461 7465  n script, update
-00000d60: 7320 6f66 2074 6865 2070 7265 7365 6e74  s of the present
-00000d70: 6174 696f 6e20 6f6e 6c79 2072 6571 7569  ation only requi
-00000d80: 7265 7320 7468 6520 7072 6573 7320 6f66  res the press of
-00000d90: 2074 6865 20e2 96b6 2052 756e 2062 7574   the ... Run but
-00000da0: 746f 6e2e 7a45 2d20 616e 6420 7061 6769  ton.zE- and pagi
-00000db0: 6e61 7469 6f6e 2077 696c 6c20 6175 746f  nation will auto
-00000dc0: 6d61 7469 6361 6c6c 7920 6164 6a75 7374  matically adjust
-00000dd0: 2069 6620 6e65 7720 636f 6e74 656e 7420   if new content 
-00000de0: 6973 2069 6e73 6572 7465 647a 0f47 6574  is insertedz.Get
-00000df0: 7469 6e67 2053 7461 7274 6564 7a12 496e  ting Startedz.In
-00000e00: 7374 616c 6c20 616e 6420 496d 706f 7274  stall and Import
-00000e10: 7a2a 2d20 4e6f 7468 696e 6720 6e65 7720  z*- Nothing new 
-00000e20: 6865 7265 2c20 676f 6f64 206f 6c64 2070  here, good old p
-00000e30: 6970 2069 6e73 7461 6c6c 2e2e 7a5a 2369  ip install..zZ#i
-00000e40: 6e73 7461 6c6c 2070 6163 6b61 6765 3c62  nstall package<b
-00000e50: 723e 7069 7020 696e 7374 616c 6c20 7765  r>pip install we
-00000e60: 6273 6c69 6465 733c 6272 3e3c 6272 3e23  bslides<br><br>#
-00000e70: 696d 706f 7274 2070 6163 6b61 6765 3c62  import package<b
-00000e80: 723e 696d 706f 7274 2077 6562 736c 6964  r>import webslid
-00000e90: 6573 2061 7320 7773 2903 7210 0000 0072  es as ws).r....r
-00000ea0: 3600 0000 7237 0000 007a 0852 756e 2044  6...r7...z.Run D
-00000eb0: 656d 6f7a 362d 2077 732e 6465 6d6f 2829  emoz6- ws.demo()
-00000ec0: 2077 696c 6c20 6765 6e65 7261 7465 2074   will generate t
-00000ed0: 6865 2068 746d 6c20 796f 7520 6172 6520  he html you are 
-00000ee0: 7265 6164 696e 6720 6e6f 777a 6023 696d  reading nowz`#im
-00000ef0: 706f 7274 3c62 723e 696d 706f 7274 2077  port<br>import w
-00000f00: 6562 736c 6964 6573 2061 7320 7773 3c62  ebslides as ws<b
-00000f10: 723e 3c62 723e 2363 7265 6174 6520 616e  r><br>#create an
-00000f20: 6420 6f70 656e 2074 6869 7320 6465 6d6f  d open this demo
-00000f30: 2e68 746d 6c20 696e 2062 726f 7773 6572  .html in browser
-00000f40: 3c62 723e 7773 2e64 656d 6f28 297a 542d  <br>ws.demo()zT-
-00000f50: 2068 746d 6c20 6f75 7470 7574 2066 696c   html output fil
-00000f60: 652c 2069 6e20 7468 6973 2063 6173 6520  e, in this case 
-00000f70: 2764 656d 6f2e 6874 6d6c 272c 2069 7320  'demo.html', is 
-00000f80: 616c 7761 7973 2073 6176 6564 2074 6f20  always saved to 
-00000f90: 6120 6469 7265 6374 6f72 7920 2777 736f  a directory 'wso
-00000fa0: 7574 277a 0b48 656c 6c6f 2057 6f72 6c64  ut'z.Hello World
-00000fb0: 7a37 2d20 6261 7369 6320 6578 616d 706c  z7- basic exampl
-00000fc0: 652c 2064 656d 6f6e 7374 7261 7469 6e67  e, demonstrating
-00000fd0: 2061 6c6c 2061 7661 696c 6162 6c65 2070   all available p
-00000fe0: 6172 616d 6574 6572 737a 602d 2048 544d  arametersz`- HTM
-00000ff0: 4c20 616c 6c6f 7773 2074 6f20 6164 6420  L allows to add 
-00001000: 6a61 7661 7363 7269 7074 2074 6f6f 2c20  javascript too, 
-00001010: 6c69 6b65 2074 6865 2063 6f70 7920 6275  like the copy bu
-00001020: 7474 6f6e 2e20 5468 6174 2773 2061 6374  tton. That's act
-00001030: 7561 6c6c 7920 6f6e 6c79 206f 6e65 206c  ually only one l
-00001040: 696e 6520 6f66 2063 6f64 6529 02da 0357  ine of code)...W
-00001050: 4859 da03 484f 577a 0964 656d 6f2e 6874  HY..HOWz.demo.ht
-00001060: 6d6c 5446 2909 da07 636f 6e74 656e 74da  mlTF)...content.
-00001070: 0a74 6974 6c65 5f70 6167 6572 2700 0000  .title_pager'...
-00001080: da0b 7368 6f77 5f74 6f70 6361 74da 0b73  ..show_topcat..s
-00001090: 686f 775f 7375 6263 6174 da0f 6f70 656e  how_subcat..open
-000010a0: 5f69 6e5f 6272 6f77 7365 72da 0f73 686f  _in_browser..sho
-000010b0: 775f 696e 6465 785f 7061 6765 da14 7368  w_index_page..sh
-000010c0: 6f77 5f68 6967 686c 6967 6874 735f 7061  ow_highlights_pa
-000010d0: 6765 da14 7368 6f77 5f68 6967 686c 6967  ge..show_highlig
-000010e0: 6874 735f 6f6e 6c79 4e29 0672 1b00 0000  hts_onlyN).r....
-000010f0: 722c 0000 0072 2f00 0000 7205 0000 0072  r,...r/...r....r
-00001100: 0400 0000 7202 0000 0029 0272 3c00 0000  ....r....).r<...
-00001110: 723b 0000 0072 1900 0000 7219 0000 0072  r;...r....r....r
-00001120: 1a00 0000 da04 6465 6d6f 2600 0000 739a  ......demo&...s.
-00001130: 0000 0002 0402 0102 0202 0102 0104 fd06  ................
-00001140: fd02 0a02 0104 0102 0106 0104 fd02 0602  ................
-00001150: 0202 0102 fe04 0304 0104 fb02 0604 0104  ................
-00001160: 0102 0202 ff04 fd02 0502 0102 0102 ff04  ................
-00001170: 0202 0202 0102 fe04 fc02 0702 0202 ff02  ................
-00001180: 0204 0104 fc02 e802 ff02 2102 0104 0102  ..........!.....
-00001190: 0102 0102 ff04 fd02 0504 0102 0102 0102  ................
-000011a0: ff02 0302 ff04 fc02 0604 0104 0102 0202  ................
-000011b0: ff04 fd04 f506 de04 3502 0102 0102 0102  ........5.......
-000011c0: 0102 0102 0102 0102 0106 f804 0a72 4300  .............rC.
-000011d0: 0000 2911 721f 0000 00da 056e 756d 7079  ..).r......numpy
-000011e0: da02 6e70 da06 7061 6e64 6173 da02 7064  ..np..pandas..pd
-000011f0: da0e 706c 6f74 6c79 2e65 7870 7265 7373  ..plotly.express
-00001200: da07 6578 7072 6573 7372 1200 0000 da0e  ..expressr......
-00001210: 7765 6273 6c69 6465 732e 6d61 696e 7202  webslides.mainr.
-00001220: 0000 00da 056f 7468 6572 7204 0000 0072  .....otherr....r
-00001230: 0500 0000 721b 0000 0072 2c00 0000 722f  ....r....r,...r/
-00001240: 0000 0072 4300 0000 7219 0000 0072 1900  ...rC...r....r..
-00001250: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-00001260: 6f64 756c 653e 0100 0000 7316 0000 0008  odule>....s.....
-00001270: 0008 0108 010c 010c 0210 0108 0308 0a08  ................
-00001280: 0908 090a 4d                             ....M
+00000520: 640d 9c04 6703 6901 642a 9c02 7d01 6408  d...g.i.d*..}.d.
+00000530: 6409 640a 6701 640b 6700 640c a201 640d  d.d.g.d.g.d...d.
+00000540: 9c04 640e 640f 6410 6702 7400 8300 6411  ..d.d.d.g.t...d.
+00000550: 6701 640d 9c04 6412 6413 6701 7401 8300  g.d...d.d.g.t...
+00000560: 6414 6701 640d 9c04 6415 6416 6417 6702  d.g.d...d.d.d.g.
+00000570: 7402 8300 6418 6419 6702 640d 9c04 641a  t...d.d.g.d...d.
+00000580: 641b 6701 641c 641d 6701 640d 9c04 642b  d.g.d.d.g.d...d+
+00000590: 9c05 6901 641e 641f 6420 6701 7403 6421  ..i.d.d.d g.t.d!
+000005a0: 8301 6422 9c03 6423 6424 6701 7403 6425  ..d"..d#d$g.t.d%
+000005b0: 8301 6426 6701 640d 9c04 6427 6428 6701  ..d&g.d...d'd(g.
+000005c0: 7404 8300 6429 6701 640d 9c04 642c 9c03  t...d)g.d...d,..
+000005d0: 6901 642a 9c02 7d01 642d 642e 642a 9c02  i.d*..}.d-d.d*..
+000005e0: 642f 6430 6431 9c02 6432 9c02 7d02 7405  d/d0d1..d2..}.t.
+000005f0: 7c01 7c00 6433 6434 6434 6434 6434 6434  |.|.d3d4d4d4d4d4
+00000600: 6434 6435 7c02 6436 8d0b 0100 6437 5300  d4d5|.d6....d7S.
+00000610: 2938 7a40 4372 6561 7465 7320 646f 6375  )8z@Creates docu
+00000620: 6d65 6e74 6174 696f 6e20 6578 706c 6169  mentation explai
+00000630: 6e69 6e67 2077 6879 2061 6e64 2068 6f77  ning why and how
+00000640: 2074 6f20 7573 6520 7468 6973 2070 6163   to use this pac
+00000650: 6b61 6765 da00 7a17 5765 6273 6c69 6465  kage..z.Webslide
+00000660: 7320 446f 6375 6d65 6e74 6174 696f 6e7a  s Documentationz
+00000670: b157 6562 736c 6964 6573 2069 7320 6120  .Webslides is a 
+00000680: 5079 7468 6f6e 2070 6163 6b61 6765 2074  Python package t
+00000690: 6861 7420 6372 6561 7465 7320 4854 4d4c  hat creates HTML
+000006a0: 2070 7265 7365 6e74 6174 696f 6e73 203c   presentations <
+000006b0: 623e 6c69 6b65 2074 6869 7320 6f6e 653c  b>like this one<
+000006c0: 2f62 3e2e 3c62 723e 4974 2065 6e61 626c  /b>.<br>It enabl
+000006d0: 6573 2065 6173 7920 7368 6172 696e 6720  es easy sharing 
+000006e0: 6f66 2050 7974 686f 6e2d 6765 6e65 7261  of Python-genera
+000006f0: 7465 6420 636f 6e74 656e 7420 7375 6368  ted content such
+00000700: 2061 7320 6368 6172 7473 2c20 6f74 6865   as charts, othe
+00000710: 7220 7669 7375 616c 7320 616e 6420 6461  r visuals and da
+00000720: 7461 7a5a 5468 6973 2070 7265 7365 6e74  tazZThis present
+00000730: 6174 696f 6e20 6465 6d6f 6e73 7472 6174  ation demonstrat
+00000740: 6573 2066 6561 7475 7265 7320 6f66 2074  es features of t
+00000750: 6865 2048 544d 4c20 666f 726d 6174 2061  he HTML format a
+00000760: 6e64 2073 686f 756c 6420 6865 6c70 2079  nd should help y
+00000770: 6f75 2067 6574 2073 7461 7274 6564 7a55  ou get startedzU
+00000780: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000790: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000007a0: 742f 7765 6273 6c69 6465 732f 223e 6874  t/webslides/">ht
+000007b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000007c0: 726f 6a65 6374 2f77 6562 736c 6964 6573  roject/webslides
+000007d0: 2f3c 2f61 3e29 03da 0541 626f 7574 da08  /</a>)...About..
+000007e0: 436f 6e74 656e 7473 da04 5079 5069 2903  Contents..PyPi).
+000007f0: da07 696d 675f 7572 6c72 1000 0000 da07  ..img_urlr......
+00000800: 7375 6d6d 6172 79fa 1a41 6476 616e 7461  summary..Advanta
+00000810: 6765 7320 6f76 6572 2050 6f77 6572 706f  ges over Powerpo
+00000820: 696e 747a 1244 796e 616d 6963 2070 6167  intz.Dynamic pag
+00000830: 656c 656e 6774 687a 3b2d 2050 6167 6573  elengthz;- Pages
+00000840: 2063 616e 2062 6520 6173 206c 6f6e 6720   can be as long 
+00000850: 286f 7220 7368 6f72 7429 2061 7320 6e65  (or short) as ne
+00000860: 6564 6564 2c20 6c69 6b65 2074 6869 7320  eded, like this 
+00000870: 6f6e 6521 753e 0000 004e 6f74 6869 6e67  one!u>...Nothing
+00000880: 206d 7563 6820 6f6e 2074 6869 7320 7061   much on this pa
+00000890: 6765 2072 6561 6c6c 792c 2074 6861 7427  ge really, that'
+000008a0: 7320 7768 7920 6974 7320 736f 2073 686f  s why its so sho
+000008b0: 7274 20f0 9f98 8929 037a 2a2d 2061 6e64  rt ....).z*- and
+000008c0: 2061 6464 696e 6720 6120 666f 6f74 6572   adding a footer
+000008d0: 2063 616e 2062 6520 7573 6566 756c 6c20   can be usefull 
+000008e0: 746f 6f2e 2e7a 462d 2070 732e 2048 6176  too..zF- ps. Hav
+000008f0: 6520 796f 7520 6e6f 7465 6420 7468 6520  e you noted the 
+00000900: 7061 6765 206e 6176 6967 6174 696f 6e20  page navigation 
+00000910: 6f6e 2074 6865 2074 6f70 2072 6967 6874  on the top right
+00000920: 206f 6620 7468 6520 7061 6765 3f7a b42d   of the page?z.-
+00000930: 2026 2378 3146 3441 313b 3a20 7468 6973   &#x1F4A1;: this
+00000940: 206d 6172 6b73 2070 6167 6573 2077 6974   marks pages wit
+00000950: 6820 6120 6869 6768 6c69 6768 742e 2049  h a highlight. I
+00000960: 6620 6120 7061 6765 2068 6173 206e 6f20  f a page has no 
+00000970: 6869 6768 6c69 6768 7473 2028 7265 6d61  highlights (rema
+00000980: 726b 7320 696e 2067 7265 7920 6172 6561  rks in grey area
+00000990: 2920 6974 2069 7320 6e6f 7420 7368 6f77  ) it is not show
+000009a0: 6e20 696e 2074 6865 2068 6967 686c 6967  n in the highlig
+000009b0: 6874 2073 756d 6d61 7279 2070 6167 6520  ht summary page 
+000009c0: 6e6f 7220 6d61 726b 6564 2069 6e20 7468  nor marked in th
+000009d0: 6520 7461 626c 6520 6f66 2063 6f6e 7465  e table of conte
+000009e0: 6e74 7329 0472 1000 0000 da0a 6869 6768  nts).r......high
+000009f0: 6c69 6768 7473 da04 626f 6479 da06 666f  lights..body..fo
+00000a00: 6f74 6572 7a13 496e 7465 7261 6374 6976  oterz.Interactiv
+00000a10: 6520 636f 6e74 656e 747a 602d 204e 6174  e contentz`- Nat
+00000a20: 6976 6520 506c 6f74 6c79 2067 7261 7068  ive Plotly graph
+00000a30: 206f 6a65 6374 7320 6361 6e20 6265 2069   ojects can be i
+00000a40: 6e73 6572 7465 6420 6173 2063 6f6e 7465  nserted as conte
+00000a50: 6e74 2c20 616e 6420 7468 6579 2068 6176  nt, and they hav
+00000a60: 6520 6d61 6e79 2069 6e74 6572 6163 7469  e many interacti
+00000a70: 7665 2066 6561 7475 7265 737a 702d 2054  ve featureszp- T
+00000a80: 7279 207a 6f6f 6d69 6e67 2069 6e20 7468  ry zooming in th
+00000a90: 6520 6279 2064 7261 6767 696e 6720 6120  e by dragging a 
+00000aa0: 7769 6e64 6f77 2069 6e20 7468 6520 706c  window in the pl
+00000ab0: 6f74 2e20 4f72 2074 6f67 676c 6520 7669  ot. Or toggle vi
+00000ac0: 7369 6269 6c69 7479 206f 6620 6120 6461  sibility of a da
+00000ad0: 7461 2073 6572 6965 7320 7669 6120 7468  ta series via th
+00000ae0: 6520 6c65 6765 6e64 206b 6579 737a 462d  e legend keyszF-
+00000af0: 204c 696e 6b20 746f 2050 6c6f 746c 7920   Link to Plotly 
+00000b00: 6761 6c6c 6572 7920 3c61 2068 7265 663d  gallery <a href=
+00000b10: 2268 7474 7073 3a2f 2f70 6c6f 746c 792e  "https://plotly.
+00000b20: 636f 6d2f 7079 7468 6f6e 2f22 3e68 6572  com/python/">her
+00000b30: 653c 2f61 3e7a 1c41 6e79 2048 544d 4c20  e</a>z.Any HTML 
+00000b40: 636f 6e74 656e 7420 7769 6c6c 2072 656e  content will ren
+00000b50: 6465 727a 162d 2046 6f72 2065 7861 6d70  derz.- For examp
+00000b60: 6c65 2074 6869 7320 6d61 707a 662d 2074  le this mapzf- t
+00000b70: 6869 7320 6d61 7020 7761 7320 6372 6561  his map was crea
+00000b80: 7465 6420 7769 7468 2046 6f6c 6975 6d20  ted with Folium 
+00000b90: 283c 6120 6872 6566 3d22 6874 7470 733a  (<a href="https:
+00000ba0: 2f2f 7079 7468 6f6e 2d76 6973 7561 6c69  //python-visuali
+00000bb0: 7a61 7469 6f6e 2e67 6974 6875 622e 696f  zation.github.io
+00000bc0: 2f66 6f6c 6975 6d2f 223e 646f 6373 3c2f  /folium/">docs</
+00000bd0: 613e 297a 1853 7479 6c65 6420 5061 6e64  a>)z.Styled Pand
+00000be0: 6173 2044 6174 6166 7261 6d65 737a 272d  as Dataframesz'-
+00000bf0: 2057 6f77 2c20 6e6f 7469 6365 2074 6861   Wow, notice tha
+00000c00: 7420 6d61 7820 7661 6c75 6520 6d61 726b  t max value mark
+00000c10: 6564 2072 6564 7a2f 2d20 4e6f 7420 746f  ed redz/- Not to
+00000c20: 206d 656e 7469 6f6e 2074 6865 206c 6f77   mention the low
+00000c30: 6573 7420 7661 6c75 652c 206d 6172 6b65  est value, marke
+00000c40: 6420 6772 6565 6e7a 602d 2073 7479 6c69  d greenz`- styli
+00000c50: 6e67 206f 6620 6120 7061 6e64 6173 2064  ng of a pandas d
+00000c60: 6174 6166 7261 6d65 2063 616e 2062 6520  ataframe can be 
+00000c70: 646f 6e65 2062 7920 6372 6561 7469 6e67  done by creating
+00000c80: 2061 2073 7479 6c65 7220 6f62 6a65 6374   a styler object
+00000c90: 2061 6e64 2063 6f6e 7665 7274 2074 6861   and convert tha
+00000ca0: 7420 746f 2068 746d 6c7a 5b2d 2069 652e  t to htmlz[- ie.
+00000cb0: 2073 7479 6c65 645f 6466 203d 2064 662e   styled_df = df.
+00000cc0: 7374 796c 652e 6261 636b 6772 6f75 6e64  style.background
+00000cd0: 5f67 7261 6469 656e 7428 636d 6170 3d27  _gradient(cmap='
+00000ce0: 426c 7565 7327 2920 616e 6420 6874 6d6c  Blues') and html
+00000cf0: 203d 2073 7479 6c65 645f 6466 2e74 6f5f   = styled_df.to_
+00000d00: 6874 6d6c 2829 7a14 5375 7065 7220 7370  html()z.Super sp
+00000d10: 6565 6420 7570 6461 7465 7321 7a69 2d20  eed updates!zi- 
+00000d20: 4120 6b65 7920 6164 7661 6e74 6167 6520  A key advantage 
+00000d30: 6f66 2074 6869 7320 7072 6573 656e 7461  of this presenta
+00000d40: 7469 6f6e 2066 6f72 6d20 6d61 7920 6265  tion form may be
+00000d50: 2074 6861 7420 7570 6461 7465 7320 6f6e   that updates on
+00000d60: 6c79 2072 6571 7569 7265 2074 6865 203c  ly require the <
+00000d70: 693e 7072 6573 7320 6f66 2061 2062 7574  i>press of a but
+00000d80: 746f 6e3c 2f69 3e75 dc00 0000 5665 7279  ton</i>u....Very
+00000d90: 206f 6674 656e 2064 6174 612c 2061 6e61   often data, ana
+00000da0: 6c79 7369 7320 636f 6e6c 7573 696f 6e73  lysis conlusions
+00000db0: 2061 6e64 206f 7468 6572 2063 6f6e 7465   and other conte
+00000dc0: 6e74 2069 7320 7265 7669 7365 6420 696e  nt is revised in
+00000dd0: 2067 6574 7469 6e67 2074 6f20 6120 6669   getting to a fi
+00000de0: 6e61 6c20 7665 7273 696f 6e20 6f66 2061  nal version of a
+00000df0: 2070 7265 7365 6e74 6174 696f 6e2e 2053   presentation. S
+00000e00: 696e 6365 2061 6c6c 2069 7320 696e 2070  ince all is in p
+00000e10: 7974 686f 6e20 7363 7269 7074 2c20 7570  ython script, up
+00000e20: 6461 7465 7320 6f66 2074 6865 2070 7265  dates of the pre
+00000e30: 7365 6e74 6174 696f 6e20 6f6e 6c79 2072  sentation only r
+00000e40: 6571 7569 7265 7320 7468 6520 7072 6573  equires the pres
+00000e50: 7320 6f66 2074 6865 20e2 96b6 2052 756e  s of the ... Run
+00000e60: 2062 7574 746f 6e2e 7a45 2d20 616e 6420   button.zE- and 
+00000e70: 7061 6769 6e61 7469 6f6e 2077 696c 6c20  pagination will 
+00000e80: 6175 746f 6d61 7469 6361 6c6c 7920 6164  automatically ad
+00000e90: 6a75 7374 2069 6620 6e65 7720 636f 6e74  just if new cont
+00000ea0: 656e 7420 6973 2069 6e73 6572 7465 64fa  ent is inserted.
+00000eb0: 0f47 6574 7469 6e67 2053 7461 7274 6564  .Getting Started
+00000ec0: 7a12 496e 7374 616c 6c20 616e 6420 496d  z.Install and Im
+00000ed0: 706f 7274 7a2a 2d20 4e6f 7468 696e 6720  portz*- Nothing 
+00000ee0: 6e65 7720 6865 7265 2c20 676f 6f64 206f  new here, good o
+00000ef0: 6c64 2070 6970 2069 6e73 7461 6c6c 2e2e  ld pip install..
+00000f00: 7a5a 2369 6e73 7461 6c6c 2070 6163 6b61  zZ#install packa
+00000f10: 6765 3c62 723e 7069 7020 696e 7374 616c  ge<br>pip instal
+00000f20: 6c20 7765 6273 6c69 6465 733c 6272 3e3c  l webslides<br><
+00000f30: 6272 3e23 696d 706f 7274 2070 6163 6b61  br>#import packa
+00000f40: 6765 3c62 723e 696d 706f 7274 2077 6562  ge<br>import web
+00000f50: 736c 6964 6573 2061 7320 7773 2903 7210  slides as ws).r.
+00000f60: 0000 0072 3700 0000 7238 0000 007a 0852  ...r7...r8...z.R
+00000f70: 756e 2044 656d 6f7a 362d 2077 732e 6465  un Demoz6- ws.de
+00000f80: 6d6f 2829 2077 696c 6c20 6765 6e65 7261  mo() will genera
+00000f90: 7465 2074 6865 2068 746d 6c20 796f 7520  te the html you 
+00000fa0: 6172 6520 7265 6164 696e 6720 6e6f 777a  are reading nowz
+00000fb0: 6023 696d 706f 7274 3c62 723e 696d 706f  `#import<br>impo
+00000fc0: 7274 2077 6562 736c 6964 6573 2061 7320  rt webslides as 
+00000fd0: 7773 3c62 723e 3c62 723e 2363 7265 6174  ws<br><br>#creat
+00000fe0: 6520 616e 6420 6f70 656e 2074 6869 7320  e and open this 
+00000ff0: 6465 6d6f 2e68 746d 6c20 696e 2062 726f  demo.html in bro
+00001000: 7773 6572 3c62 723e 7773 2e64 656d 6f28  wser<br>ws.demo(
+00001010: 297a 542d 2068 746d 6c20 6f75 7470 7574  )zT- html output
+00001020: 2066 696c 652c 2069 6e20 7468 6973 2063   file, in this c
+00001030: 6173 6520 2764 656d 6f2e 6874 6d6c 272c  ase 'demo.html',
+00001040: 2069 7320 616c 7761 7973 2073 6176 6564   is always saved
+00001050: 2074 6f20 6120 6469 7265 6374 6f72 7920   to a directory 
+00001060: 2777 736f 7574 277a 0b48 656c 6c6f 2057  'wsout'z.Hello W
+00001070: 6f72 6c64 7a37 2d20 6261 7369 6320 6578  orldz7- basic ex
+00001080: 616d 706c 652c 2064 656d 6f6e 7374 7261  ample, demonstra
+00001090: 7469 6e67 2061 6c6c 2061 7661 696c 6162  ting all availab
+000010a0: 6c65 2070 6172 616d 6574 6572 737a 602d  le parametersz`-
+000010b0: 2048 544d 4c20 616c 6c6f 7773 2074 6f20   HTML allows to 
+000010c0: 6164 6420 6a61 7661 7363 7269 7074 2074  add javascript t
+000010d0: 6f6f 2c20 6c69 6b65 2074 6865 2063 6f70  oo, like the cop
+000010e0: 7920 6275 7474 6f6e 2e20 5468 6174 2773  y button. That's
+000010f0: 2061 6374 7561 6c6c 7920 6f6e 6c79 206f   actually only o
+00001100: 6e65 206c 696e 6520 6f66 2063 6f64 6529  ne line of code)
+00001110: 02da 0357 4859 da03 484f 5729 05da 0e64  ...WHY..HOW)...d
+00001120: 796e 616d 6963 5f6c 656e 6768 74da 1369  ynamic_lenght..i
+00001130: 6e74 6572 6163 7469 7665 5f63 6f6e 7465  nteractive_conte
+00001140: 6e74 da0b 6874 6d6c 5f66 6f72 6d61 74da  nt..html_format.
+00001150: 0a73 7479 6c69 6e67 5f64 66da 0775 7064  .styling_df..upd
+00001160: 6174 6573 2903 da07 696e 7374 616c 6cda  ates)...install.
+00001170: 0872 756e 5f64 656d 6fda 0b68 656c 6c6f  .run_demo..hello
+00001180: 5f77 6f72 6c64 7a14 5768 7920 746f 2075  _worldz.Why to u
+00001190: 7365 2057 6562 736c 6964 6573 7a14 486f  se Webslidesz.Ho
+000011a0: 7720 746f 2075 7365 2057 6562 736c 6964  w to use Webslid
+000011b0: 6573 7a27 4665 6174 7572 6573 2074 6861  esz'Features tha
+000011c0: 7420 6265 6174 204d 6963 726f 736f 6674  t beat Microsoft
+000011d0: 2050 6f77 6572 706f 696e 747a 164b 6963   Powerpointz.Kic
+000011e0: 6b73 7461 7274 2079 6f75 7220 7072 6f6a  kstart your proj
+000011f0: 6563 7429 0272 3600 0000 723a 0000 0029  ect).r6...r:...)
+00001200: 02da 0774 6f70 6361 7473 da07 7375 6263  ...topcats..subc
+00001210: 6174 737a 0964 656d 6f2e 6874 6d6c 5446  atsz.demo.htmlTF
+00001220: 290b da07 636f 6e74 656e 74da 0a74 6974  )...content..tit
+00001230: 6c65 5f70 6167 6572 2700 0000 da0b 7368  le_pager'.....sh
+00001240: 6f77 5f74 6f70 6361 74da 0b73 686f 775f  ow_topcat..show_
+00001250: 7375 6263 6174 da0f 6f70 656e 5f69 6e5f  subcat..open_in_
+00001260: 6272 6f77 7365 72da 0f73 686f 775f 7469  browser..show_ti
+00001270: 746c 655f 7061 6765 da0f 7368 6f77 5f69  tle_page..show_i
+00001280: 6e64 6578 5f70 6167 65da 1473 686f 775f  ndex_page..show_
+00001290: 6869 6768 6c69 6768 7473 5f70 6167 65da  highlights_page.
+000012a0: 1473 686f 775f 6869 6768 6c69 6768 7473  .show_highlights
+000012b0: 5f6f 6e6c 79da 0874 6f6f 6c74 6970 734e  _only..tooltipsN
+000012c0: 2906 721b 0000 0072 2c00 0000 722f 0000  ).r....r,...r/..
+000012d0: 0072 0500 0000 7204 0000 0072 0200 0000  .r....r....r....
+000012e0: 2903 7248 0000 0072 4700 0000 7250 0000  ).rH...rG...rP..
+000012f0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00001300: da04 6465 6d6f 2600 0000 7322 0100 0002  ..demo&...s"....
+00001310: 0402 0102 0202 0102 0104 fd06 fd02 0a02  ................
+00001320: 0104 0102 0106 0104 fd02 0602 0202 0102  ................
+00001330: fe04 0304 0104 fb02 0604 0104 0102 0202  ................
+00001340: ff04 fd02 0502 0102 0102 ff04 0202 0202  ................
+00001350: 0102 fe04 fc02 0702 0202 ff02 0204 0104  ................
+00001360: fc02 e802 ff02 2102 0104 0102 0102 0102  ......!.........
+00001370: ff04 fd02 0504 0102 0102 0102 ff02 0302  ................
+00001380: ff04 fc02 0604 0104 0102 0202 ff04 fd04  ................
+00001390: f506 de04 3502 0202 ff02 0206 0104 fc02  ....5...........
+000013a0: 0802 0202 0102 fe04 0302 0202 ff04 fb02  ................
+000013b0: 0704 0104 0102 0202 ff04 fd02 0502 0202  ................
+000013c0: 0102 fe04 0302 0202 0102 fe04 fb02 0802  ................
+000013d0: 0202 ff02 0202 0202 ff04 fc06 e404 2504  ..............%.
+000013e0: 0102 0102 0102 ff04 fe02 0402 0202 ff02  ................
+000013f0: 0202 0102 ff02 0302 ff04 fb02 0702 0202  ................
+00001400: ff04 0202 0202 ff04 fc06 f506 db08 3a02  ..............:.
+00001410: 0102 0104 ff06 ff04 0402 0102 0102 0102  ................
+00001420: 0102 0102 0102 0102 0102 0102 0106 f604  ................
+00001430: 0c72 5100 0000 2911 721f 0000 00da 056e  .rQ...).r......n
+00001440: 756d 7079 da02 6e70 da06 7061 6e64 6173  umpy..np..pandas
+00001450: da02 7064 da0e 706c 6f74 6c79 2e65 7870  ..pd..plotly.exp
+00001460: 7265 7373 da07 6578 7072 6573 7372 1200  ress..expressr..
+00001470: 0000 da0e 7765 6273 6c69 6465 732e 6d61  ....webslides.ma
+00001480: 696e 7202 0000 00da 056f 7468 6572 7204  inr......otherr.
+00001490: 0000 0072 0500 0000 721b 0000 0072 2c00  ...r....r....r,.
+000014a0: 0000 722f 0000 0072 5100 0000 7219 0000  ..r/...rQ...r...
+000014b0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+000014c0: da08 3c6d 6f64 756c 653e 0100 0000 7318  ..<module>....s.
+000014d0: 0000 0008 0008 0108 010c 010c 0210 0108  ................
+000014e0: 0308 0a08 0908 0900 7f0a 0f              ...........
```

### Comparing `webslides-0.6.0/webslides/modules/__pycache__/input_validations.cpython-310.pyc` & `webslides-0.6.3/webslides/modules/__pycache__/input_validations.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 17:57:26 2023 UTC, .py size: 2824 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0637 3c64 080b 0000  o........7<d....
+00000000: 6f0d 0d0a 0000 0000 6234 5a64 250b 0000  o.......b4Zd%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a02 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a03 6404 6405 8400 5a04 6401 5300 2906  Z.d.d...Z.d.S.).
 00000050: e900 0000 004e 6301 0000 0000 0000 0000  .....Nc.........
 00000060: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
 00000070: 9800 0000 7400 7c00 7401 8302 7307 6401  ....t.|.t...s.d.
@@ -44,110 +44,111 @@
 000002b0: 6c69 6465 735c 6d6f 6475 6c65 735c 696e  lides\modules\in
 000002c0: 7075 745f 7661 6c69 6461 7469 6f6e 732e  put_validations.
 000002d0: 7079 da13 7661 6c69 6461 7465 5f74 6974  py..validate_tit
 000002e0: 6c65 5f70 6167 6504 0000 0073 1e00 0000  le_page....s....
 000002f0: 0a01 0401 1601 0401 1601 0401 1601 0401  ................
 00000300: 1601 0c01 0a01 0601 02ff 04ff 0404 720d  ..............r.
 00000310: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000320: 0800 0000 0c00 0000 4300 0000 7362 0200  ........C...sb..
+00000320: 0900 0000 0c00 0000 4300 0000 736e 0200  ........C...sn..
 00000330: 0074 007c 0074 0183 0273 0764 0153 0074  .t.|.t...s.d.S.t
 00000340: 027c 0083 0164 026b 0072 0f64 0353 007c  .|...d.k.r.d.S.|
-00000350: 00a0 03a1 0044 0090 015d 1a5c 027d 017d  .....D...].\.}.}
+00000350: 00a0 03a1 0044 0090 015d 205c 027d 017d  .....D...] \.}.}
 00000360: 0274 007c 0274 0183 0273 3664 047c 019b  .t.|.t...s6d.|..
 00000370: 0064 0574 047c 0283 0164 0064 0685 0219  .d.t.|...d.d....
 00000380: 009b 0064 0774 047c 0283 0164 0864 0085  ...d.t.|...d.d..
 00000390: 0219 009b 009d 0602 0001 0053 0074 027c  ...........S.t.|
 000003a0: 0283 0164 026b 0072 4464 047c 019b 0064  ...d.k.rDd.|...d
 000003b0: 099d 0302 0001 0053 007c 02a0 03a1 0044  .......S.|.....D
-000003c0: 005d e55c 027d 037d 0474 007c 0474 0583  .].\.}.}.t.|.t..
+000003c0: 005d eb5c 027d 037d 0474 007c 0474 0183  .].\.}.}.t.|.t..
 000003d0: 0273 6c64 047c 039b 0064 0a74 047c 0483  .sld.|...d.t.|..
 000003e0: 0164 0064 0685 0219 009b 0064 0774 047c  .d.d.......d.t.|
 000003f0: 0483 0164 0864 0085 0219 009b 009d 0602  ...d.d..........
 00000400: 0001 0002 0001 0053 0074 027c 0483 0164  .......S.t.|...d
-00000410: 026b 0072 7c64 047c 039b 0064 0b9d 0302  .k.r|d.|...d....
-00000420: 0001 0002 0001 0053 007c 0444 005d ae7d  .......S.|.D.].}
-00000430: 0574 007c 0574 0183 0273 9f64 0c74 047c  .t.|.t...s.d.t.|
-00000440: 0583 0164 0064 0685 0219 009b 0064 0774  ...d.d.......d.t
-00000450: 047c 0583 0164 0864 0085 0219 009b 009d  .|...d.d........
-00000460: 0402 0001 0002 0001 0002 0001 0053 007c  .............S.|
-00000470: 05a0 03a1 0044 005d 885c 027d 067d 077c  .....D.].\.}.}.|
-00000480: 0664 0d6b 0272 cc74 007c 0774 0483 0273  .d.k.r.t.|.t...s
-00000490: cc64 0e74 047c 0783 0164 0064 0685 0219  .d.t.|...d.d....
-000004a0: 009b 0064 0774 047c 0783 0164 0864 0085  ...d.t.|...d.d..
-000004b0: 0219 009b 009d 0402 0001 0002 0001 0002  ................
-000004c0: 0001 0002 0001 0053 007c 0664 0f76 0072  .......S.|.d.v.r
-000004d0: fd74 007c 0774 0583 0272 de74 0664 1064  .t.|.t...r.t.d.d
-000004e0: 1184 007c 0744 0083 0183 0173 fd64 047c  ...|.D.....s.d.|
-000004f0: 069b 0064 1274 047c 0783 0164 0064 0685  ...d.t.|...d.d..
-00000500: 0219 009b 0064 0774 047c 0783 0164 0864  .....d.t.|...d.d
-00000510: 0085 0219 009b 009d 0602 0001 0002 0001  ................
-00000520: 0002 0001 0002 0001 0053 007c 0664 136b  .........S.|.d.k
-00000530: 0290 0172 2b74 007c 0774 0483 0290 0173  ...r+t.|.t.....s
-00000540: 2b74 007c 0774 076a 0883 0290 0173 2b64  +t.|.t.j.....s+d
-00000550: 1474 047c 0783 0164 0064 0685 0219 009b  .t.|...d.d......
-00000560: 0064 0774 047c 0783 0164 0864 0085 0219  .d.t.|...d.d....
-00000570: 009b 009d 0402 0001 0002 0001 0002 0001  ................
-00000580: 0002 0001 0053 0071 a371 7e71 4871 1364  .....S.q.q~qHq.d
-00000590: 0053 0029 154e 7a21 4572 726f 723a 2049  .S.).Nz!Error: I
-000005a0: 6e70 7574 2069 7320 6e6f 7420 6120 6469  nput is not a di
-000005b0: 6374 696f 6e61 7279 2ee9 0100 0000 7a36  ctionary......z6
-000005c0: 4572 726f 723a 2044 6963 7469 6f6e 6172  Error: Dictionar
-000005d0: 7920 6d75 7374 2068 6176 6520 6174 206c  y must have at l
-000005e0: 6561 7374 2031 206b 6579 2d76 616c 7565  east 1 key-value
-000005f0: 2070 6169 722e 7a08 4572 726f 723a 2027   pair.z.Error: '
-00000600: 7a26 2720 7661 6c75 6520 6973 206e 6f74  z&' value is not
-00000610: 2061 2064 6963 7469 6f6e 6172 792e 2043   a dictionary. C
-00000620: 6f6e 7465 6e74 3a20 e90d 0000 007a 032e  ontent: .....z..
-00000630: 2e2e 69f2 ffff ff7a 3427 2073 7562 6469  ..i....z4' subdi
-00000640: 6374 696f 6e61 7279 206d 7573 7420 6861  ctionary must ha
-00000650: 7665 2061 7420 6c65 6173 7420 3120 6b65  ve at least 1 ke
-00000660: 792d 7661 6c75 6520 7061 6972 2e7a 2027  y-value pair.z '
-00000670: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
-00000680: 6c69 7374 2e20 436f 6e74 656e 743a 207a  list. Content: z
-00000690: 2427 206c 6973 7420 6d75 7374 2068 6176  $' list must hav
-000006a0: 6520 6174 206c 6561 7374 2031 2065 6c65  e at least 1 ele
-000006b0: 6d65 6e74 2e7a 3245 7272 6f72 3a20 4c69  ment.z2Error: Li
-000006c0: 7374 2065 6c65 6d65 6e74 2069 7320 6e6f  st element is no
-000006d0: 7420 6120 6469 6374 696f 6e61 7279 2e20  t a dictionary. 
-000006e0: 436f 6e74 656e 743a 2072 0200 0000 7a2f  Content: r....z/
-000006f0: 4572 726f 723a 2027 7469 746c 6527 2076  Error: 'title' v
-00000700: 616c 7565 2069 7320 6e6f 7420 6120 7374  alue is not a st
-00000710: 7269 6e67 2e20 436f 6e74 656e 743a 2029  ring. Content: )
-00000720: 02da 0a68 6967 686c 6967 6874 7372 0500  ...highlightsr..
-00000730: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00000740: 0000 0004 0000 0073 0000 0073 1a00 0000  .......s...s....
-00000750: 8100 7c00 5d08 7d01 7400 7c01 7401 8302  ..|.].}.t.|.t...
-00000760: 5600 0100 7102 6400 5300 2901 4e29 0272  V...q.d.S.).N).r
-00000770: 0600 0000 7208 0000 0029 02da 022e 30da  ....r....)....0.
-00000780: 0176 720b 0000 0072 0b00 0000 720c 0000  .vr....r....r...
-00000790: 00da 093c 6765 6e65 7870 723e 3200 0000  ...<genexpr>2...
-000007a0: 7304 0000 0002 8018 007a 2376 616c 6964  s........z#valid
-000007b0: 6174 655f 636f 6e74 656e 742e 3c6c 6f63  ate_content.<loc
-000007c0: 616c 733e 2e3c 6765 6e65 7870 723e 7a2b  als>.<genexpr>z+
-000007d0: 2720 7661 6c75 6520 6973 206e 6f74 2061  ' value is not a
-000007e0: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-000007f0: 2e20 436f 6e74 656e 743a 20da 0462 6f64  . Content: ..bod
-00000800: 797a 4845 7272 6f72 3a20 2762 6f64 7927  yzHError: 'body'
-00000810: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
-00000820: 7374 7269 6e67 206f 7220 6120 506c 6f74  string or a Plot
-00000830: 6c79 2046 6967 7572 6520 6f62 6a65 6374  ly Figure object
-00000840: 2e20 436f 6e74 656e 743a 2029 0972 0600  . Content: ).r..
-00000850: 0000 7207 0000 00da 036c 656e da05 6974  ..r......len..it
-00000860: 656d 7372 0800 0000 7209 0000 00da 0361  emsr....r......a
-00000870: 6c6c da02 676f da06 4669 6775 7265 2908  ll..go..Figure).
-00000880: da07 636f 6e74 656e 74da 0674 6f70 6361  ..content..topca
-00000890: 74da 0773 7562 6361 7473 da06 7375 6263  t..subcats..subc
-000008a0: 6174 7216 0000 00da 0469 7465 6dda 036b  atr......item..k
-000008b0: 6579 da05 7661 6c75 6572 0b00 0000 720b  ey..valuer....r.
-000008c0: 0000 0072 0c00 0000 da10 7661 6c69 6461  ...r......valida
-000008d0: 7465 5f63 6f6e 7465 6e74 1500 0000 7342  te_content....sB
-000008e0: 0000 000a 0104 010c 0204 0112 020a 0132  ...............2
-000008f0: 010c 0210 0110 020a 0136 010c 0214 0108  .........6......
-00000900: 020a 0134 0110 0212 0138 0108 0108 0102  ...4.....8......
-00000910: ff10 0102 ff3e 0224 0138 0102 8002 f902  .....>.$.8......
-00000920: fc02 f904 1372 2100 0000 2905 da14 706c  .....r!...)...pl
-00000930: 6f74 6c79 2e67 7261 7068 5f6f 626a 6563  otly.graph_objec
-00000940: 7473 da0d 6772 6170 685f 6f62 6a65 6374  ts..graph_object
-00000950: 7372 1800 0000 720d 0000 0072 2100 0000  sr....r....r!...
-00000960: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000970: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000980: 0000 7306 0000 000c 0008 030c 11         ..s..........
+00000410: 0b6b 0272 7c64 047c 039b 0064 0c9d 0302  .k.r|d.|...d....
+00000420: 0001 0002 0001 0053 007c 04a0 03a1 0044  .......S.|.....D
+00000430: 005d b25c 027d 057d 0674 007c 0674 0183  .].\.}.}.t.|.t..
+00000440: 0273 a364 0d74 047c 0683 0164 0064 0685  .s.d.t.|...d.d..
+00000450: 0219 009b 0064 0774 047c 0683 0164 0864  .....d.t.|...d.d
+00000460: 0085 0219 009b 009d 0402 0001 0002 0001  ................
+00000470: 0002 0001 0053 007c 06a0 03a1 0044 005d  .....S.|.....D.]
+00000480: 8a5c 027d 077d 087c 0764 0e6b 0272 d074  .\.}.}.|.d.k.r.t
+00000490: 007c 0874 0483 0273 d064 0f74 047c 0883  .|.t...s.d.t.|..
+000004a0: 0164 0064 0685 0219 009b 0064 0774 047c  .d.d.......d.t.|
+000004b0: 0883 0164 0864 0085 0219 009b 009d 0402  ...d.d..........
+000004c0: 0001 0002 0001 0002 0001 0002 0001 0053  ...............S
+000004d0: 007c 0764 1076 0090 0172 0374 007c 0874  .|.d.v...r.t.|.t
+000004e0: 0583 0272 e474 0664 1164 1284 007c 0844  ...r.t.d.d...|.D
+000004f0: 0083 0183 0190 0173 0364 047c 079b 0064  .......s.d.|...d
+00000500: 1374 047c 0883 0164 0064 0685 0219 009b  .t.|...d.d......
+00000510: 0064 0774 047c 0883 0164 0864 0085 0219  .d.t.|...d.d....
+00000520: 009b 009d 0602 0001 0002 0001 0002 0001  ................
+00000530: 0002 0001 0053 007c 0764 146b 0290 0172  .....S.|.d.k...r
+00000540: 3174 007c 0874 0483 0290 0173 3174 007c  1t.|.t.....s1t.|
+00000550: 0874 076a 0883 0290 0173 3164 1574 047c  .t.j.....s1d.t.|
+00000560: 0883 0164 0064 0685 0219 009b 0064 0774  ...d.d.......d.t
+00000570: 047c 0883 0164 0864 0085 0219 009b 009d  .|...d.d........
+00000580: 0402 0001 0002 0001 0002 0001 0002 0001  ................
+00000590: 0053 0071 a771 8071 4871 1364 0053 0029  .S.q.q.qHq.d.S.)
+000005a0: 164e 7a21 4572 726f 723a 2049 6e70 7574  .Nz!Error: Input
+000005b0: 2069 7320 6e6f 7420 6120 6469 6374 696f   is not a dictio
+000005c0: 6e61 7279 2ee9 0100 0000 7a36 4572 726f  nary......z6Erro
+000005d0: 723a 2044 6963 7469 6f6e 6172 7920 6d75  r: Dictionary mu
+000005e0: 7374 2068 6176 6520 6174 206c 6561 7374  st have at least
+000005f0: 2031 206b 6579 2d76 616c 7565 2070 6169   1 key-value pai
+00000600: 722e 7a08 4572 726f 723a 2027 7a26 2720  r.z.Error: 'z&' 
+00000610: 7661 6c75 6520 6973 206e 6f74 2061 2064  value is not a d
+00000620: 6963 7469 6f6e 6172 792e 2043 6f6e 7465  ictionary. Conte
+00000630: 6e74 3a20 e90d 0000 007a 032e 2e2e 69f2  nt: .....z....i.
+00000640: ffff ff7a 3427 2073 7562 6469 6374 696f  ...z4' subdictio
+00000650: 6e61 7279 206d 7573 7420 6861 7665 2061  nary must have a
+00000660: 7420 6c65 6173 7420 3120 6b65 792d 7661  t least 1 key-va
+00000670: 6c75 6520 7061 6972 2e7a 2027 2076 616c  lue pair.z ' val
+00000680: 7565 2069 7320 6e6f 7420 6120 6469 6374  ue is not a dict
+00000690: 2e20 436f 6e74 656e 743a 2072 0100 0000  . Content: r....
+000006a0: 7a24 2720 6469 6374 206d 7573 7420 6861  z$' dict must ha
+000006b0: 7665 2061 7420 6c65 6173 7420 3120 656c  ve at least 1 el
+000006c0: 656d 656e 742e 7a32 4572 726f 723a 2050  ement.z2Error: P
+000006d0: 6167 6520 636f 6e74 656e 7420 6973 206e  age content is n
+000006e0: 6f74 2061 2064 6963 7469 6f6e 6172 792e  ot a dictionary.
+000006f0: 2043 6f6e 7465 6e74 3a20 7202 0000 007a   Content: r....z
+00000700: 2f45 7272 6f72 3a20 2774 6974 6c65 2720  /Error: 'title' 
+00000710: 7661 6c75 6520 6973 206e 6f74 2061 2073  value is not a s
+00000720: 7472 696e 672e 2043 6f6e 7465 6e74 3a20  tring. Content: 
+00000730: 2902 da0a 6869 6768 6c69 6768 7473 7205  )...highlightsr.
+00000740: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000750: 0200 0000 0400 0000 7300 0000 731a 0000  ........s...s...
+00000760: 0081 007c 005d 087d 0174 007c 0174 0183  ...|.].}.t.|.t..
+00000770: 0256 0001 0071 0264 0053 0029 014e 2902  .V...q.d.S.).N).
+00000780: 7206 0000 0072 0800 0000 2902 da02 2e30  r....r....)....0
+00000790: da01 7672 0b00 0000 720b 0000 0072 0c00  ..vr....r....r..
+000007a0: 0000 da09 3c67 656e 6578 7072 3e35 0000  ....<genexpr>5..
+000007b0: 0073 0400 0000 0280 1800 7a23 7661 6c69  .s........z#vali
+000007c0: 6461 7465 5f63 6f6e 7465 6e74 2e3c 6c6f  date_content.<lo
+000007d0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
+000007e0: 2b27 2076 616c 7565 2069 7320 6e6f 7420  +' value is not 
+000007f0: 6120 6c69 7374 206f 6620 7374 7269 6e67  a list of string
+00000800: 732e 2043 6f6e 7465 6e74 3a20 da04 626f  s. Content: ..bo
+00000810: 6479 7a48 4572 726f 723a 2027 626f 6479  dyzHError: 'body
+00000820: 2720 7661 6c75 6520 6973 206e 6f74 2061  ' value is not a
+00000830: 2073 7472 696e 6720 6f72 2061 2050 6c6f   string or a Plo
+00000840: 746c 7920 4669 6775 7265 206f 626a 6563  tly Figure objec
+00000850: 742e 2043 6f6e 7465 6e74 3a20 2909 7206  t. Content: ).r.
+00000860: 0000 0072 0700 0000 da03 6c65 6eda 0569  ...r......len..i
+00000870: 7465 6d73 7208 0000 0072 0900 0000 da03  temsr....r......
+00000880: 616c 6cda 0267 6fda 0646 6967 7572 6529  all..go..Figure)
+00000890: 09da 0763 6f6e 7465 6e74 da06 746f 7063  ...content..topc
+000008a0: 6174 da07 7375 6263 6174 73da 0673 7562  at..subcats..sub
+000008b0: 6361 7472 1600 0000 5a02 696b da02 6976  catr....Z.ik..iv
+000008c0: da03 6b65 79da 0576 616c 7565 720b 0000  ..key..valuer...
+000008d0: 0072 0b00 0000 720c 0000 00da 1076 616c  .r....r......val
+000008e0: 6964 6174 655f 636f 6e74 656e 7415 0000  idate_content...
+000008f0: 0073 4200 0000 0a01 0401 0c02 0401 1202  .sB.............
+00000900: 0a01 3201 0c02 1001 1002 0a02 3601 0c02  ..2.........6...
+00000910: 1401 1002 0a02 3401 1002 1202 3801 0a01  ......4.....8...
+00000920: 0801 02ff 1001 04ff 3e02 2401 3801 0280  ........>.$.8...
+00000930: 02f8 02fb 02f8 0416 7221 0000 0029 05da  ........r!...)..
+00000940: 1470 6c6f 746c 792e 6772 6170 685f 6f62  .plotly.graph_ob
+00000950: 6a65 6374 73da 0d67 7261 7068 5f6f 626a  jects..graph_obj
+00000960: 6563 7473 7218 0000 0072 0d00 0000 7221  ectsr....r....r!
+00000970: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00000980: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000990: 3e01 0000 0073 0600 0000 0c00 0803 0c11  >....s..........
```

### Comparing `webslides-0.6.0/webslides/modules/__pycache__/other.cpython-310.pyc` & `webslides-0.6.3/webslides/modules/__pycache__/other.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 16:39:50 2023 UTC, .py size: 1724 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d624 3c64 bc06 0000  o........$<d....
+00000000: 6f0d 0d0a 0000 0000 cf19 6764 8d07 0000  o.........gd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6502 6403 6502 6604 6404 6405 8404 5a03  e.d.e.f.d.d...Z.
 00000050: 6406 6407 8400 5a04 6408 6409 8400 5a05  d.d...Z.d.d...Z.
 00000060: 6401 5300 290a e900 0000 004e da09 6669  d.S.)......N..fi
 00000070: 6c65 5f6e 616d 65da 0672 6574 7572 6e63  le_name..returnc
@@ -29,84 +29,94 @@
 000001c0: 6273 6c69 6465 735c 7765 6273 6c69 6465  bslides\webslide
 000001d0: 735c 6d6f 6475 6c65 735c 6f74 6865 722e  s\modules\other.
 000001e0: 7079 da0f 6578 7472 6163 745f 7665 7273  py..extract_vers
 000001f0: 696f 6e05 0000 0073 1c00 0000 0401 0401  ion....s........
 00000200: 0c02 0801 0c01 0401 0c01 0afc 0406 02fd  ................
 00000210: 0afd 0406 10fa 0406 7211 0000 0063 0000  ........r....c..
 00000220: 0000 0000 0000 0000 0000 0800 0000 0800  ................
-00000230: 0000 4300 0000 73d2 0000 0064 017d 0074  ..C...s....d.}.t
+00000230: 0000 4300 0000 73f6 0000 0064 017d 0074  ..C...s....d.}.t
 00000240: 006a 01a0 0274 006a 01a0 0374 04a1 01a1  .j...t.j...t....
 00000250: 017d 0174 006a 01a0 057c 01a1 017d 0274  .}.t.j...|...}.t
 00000260: 067c 029b 0064 027c 009b 009d 0364 0383  .|...d.|.....d..
 00000270: 028f 0c7d 037c 03a0 07a1 007d 0457 0064  ...}.|.....}.W.d
 00000280: 0004 0004 0083 0301 006e 0831 0073 2b77  .........n.1.s+w
 00000290: 0101 0001 0001 0059 0001 0064 0467 017d  .......Y...d.g.}
-000002a0: 057c 0444 005d 197d 067c 06a0 0864 0564  .|.D.].}.|...d.d
-000002b0: 06a1 027d 067c 06a0 09a1 00a0 0864 0764  ...}.|.......d.d
-000002c0: 08a1 02a0 0864 0964 0aa1 027d 077c 05a0  .....d.d...}.|..
-000002d0: 0a7c 07a1 0101 0071 357c 05a0 0a64 0ba1  .|.....q5|...d..
-000002e0: 0101 007c 05a0 0a64 0c64 0da0 057c 0564  ...|...d.d...|.d
-000002f0: 0e64 0f85 0219 00a1 0117 0064 1017 00a1  .d.........d....
-00000300: 0101 0064 0da0 057c 05a1 0153 0029 114e  ...d...|...S.).N
-00000310: 7a0e 6865 6c6c 6f5f 776f 726c 642e 7079  z.hello_world.py
-00000320: fa01 2f72 0400 0000 7a66 3c64 6976 2073  ../r....zf<div s
-00000330: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00000340: 312e 3165 6d3b 7061 6464 696e 673a 3135  1.1em;padding:15
-00000350: 7078 3b62 6163 6b67 726f 756e 642d 636f  px;background-co
-00000360: 6c6f 723a 2366 6466 6663 373b 2064 6973  lor:#fdffc7; dis
-00000370: 706c 6179 3a20 696e 6c69 6e65 2d62 6c6f  play: inline-blo
-00000380: 636b 3b22 3e3c 7072 653e 3c63 6f64 653e  ck;"><pre><code>
-00000390: 7a11 696d 706f 7274 206d 6169 6e20 6173  z.import main as
-000003a0: 2077 737a 1669 6d70 6f72 7420 7765 6273   wsz.import webs
-000003b0: 6c69 6465 7320 6173 2077 73da 013c 7a04  lides as ws..<z.
-000003c0: 266c 743b da01 3e7a 0426 6774 3bfa 133c  &lt;..>z.&gt;..<
-000003d0: 2f63 6f64 653e 3c2f 7072 653e 3c2f 6469  /code></pre></di
-000003e0: 763e 7aaf 3c62 723e 3c62 723e 3c62 7574  v>z.<br><br><but
-000003f0: 746f 6e20 7374 796c 653d 2266 6f6e 742d  ton style="font-
-00000400: 7369 7a65 3a20 312e 3365 6d3b 2062 6163  size: 1.3em; bac
-00000410: 6b67 726f 756e 642d 636f 6c6f 723a 2023  kground-color: #
-00000420: 3030 6262 3030 3b63 6f6c 6f72 3a20 7768  00bb00;color: wh
-00000430: 6974 653b 626f 7264 6572 2d63 6f6c 6f72  ite;border-color
-00000440: 3a20 2363 3763 3763 3720 2169 6d70 6f72  : #c7c7c7 !impor
-00000450: 7461 6e74 3b20 626f 7264 6572 2d72 6164  tant; border-rad
-00000460: 6975 733a 2036 7078 3b22 206f 6e63 6c69  ius: 6px;" oncli
-00000470: 636b 3d22 6e61 7669 6761 746f 722e 636c  ck="navigator.cl
-00000480: 6970 626f 6172 642e 7772 6974 6554 6578  ipboard.writeTex
-00000490: 7428 60da 010a 7205 0000 00e9 ffff ffff  t(`...r.........
-000004a0: 7a40 6029 3b61 6c65 7274 2827 436f 6465  z@`);alert('Code
-000004b0: 2063 6f70 6965 6420 746f 2063 6c69 7062   copied to clipb
-000004c0: 6f61 7264 2729 3b22 3e3c 623e 434f 5059  oard');"><b>COPY
-000004d0: 2043 4f44 453c 2f62 3e3c 2f62 7574 746f   CODE</b></butto
-000004e0: 6e3e 290b da02 6f73 da04 7061 7468 da07  n>)...os..path..
-000004f0: 6469 726e 616d 65da 0761 6273 7061 7468  dirname..abspath
-00000500: da08 5f5f 6669 6c65 5f5f da04 6a6f 696e  ..__file__..join
-00000510: 7206 0000 00da 0972 6561 646c 696e 6573  r......readlines
-00000520: da07 7265 706c 6163 65da 0672 7374 7269  ..replace..rstri
-00000530: 70da 0661 7070 656e 6429 08da 0566 6e61  p..append)...fna
-00000540: 6d65 da0b 6375 7272 656e 745f 6469 72da  me..current_dir.
-00000550: 0566 7061 7468 da01 665a 0a63 6f64 655f  .fpath..fZ.code_
-00000560: 6c69 6e65 735a 0a68 746d 6c5f 6c69 6e65  linesZ.html_line
-00000570: 73da 046c 696e 655a 0968 746d 6c5f 6c69  s..lineZ.html_li
-00000580: 6e65 720f 0000 0072 0f00 0000 7210 0000  ner....r....r...
-00000590: 00da 1068 656c 6c6f 5f77 6f72 6c64 5f68  ...hello_world_h
-000005a0: 746d 6c12 0000 0073 2a00 0000 0401 1401  tml....s*.......
-000005b0: 0c01 1601 0a01 1cff 0204 04ff 0802 0c01  ................
-000005c0: 1801 0c01 0a01 0403 0601 0a01 04ff 0201  ................
-000005d0: 02ff 04ff 0a04 7227 0000 0063 0100 0000  ......r'...c....
-000005e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000005f0: 4300 0000 730c 0000 0064 017c 009b 0064  C...s....d.|...d
-00000600: 029d 0353 0029 034e 7a66 3c64 6976 2073  ...S.).Nzf<div s
-00000610: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
-00000620: 2d63 6f6c 6f72 3a23 6664 6666 6337 3b20  -color:#fdffc7; 
-00000630: 6469 7370 6c61 793a 2069 6e6c 696e 652d  display: inline-
-00000640: 626c 6f63 6b3b 666f 6e74 2d73 697a 653a  block;font-size:
-00000650: 312e 3165 6d3b 7061 6464 696e 673a 3135  1.1em;padding:15
-00000660: 7078 3b22 3e3c 7072 653e 3c63 6f64 653e  px;"><pre><code>
-00000670: 7215 0000 0072 0f00 0000 2901 da04 636f  r....r....)...co
-00000680: 6465 720f 0000 0072 0f00 0000 7210 0000  der....r....r...
-00000690: 00da 0c63 6f64 655f 746f 5f68 746d 6c29  ...code_to_html)
-000006a0: 0000 0073 0200 0000 0c02 7229 0000 0029  ...s......r)...)
-000006b0: 0672 1800 0000 7208 0000 00da 0373 7472  .r....r......str
-000006c0: 7211 0000 0072 2700 0000 7229 0000 0072  r....r'...r)...r
-000006d0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000006e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000006f0: 0073 0a00 0000 0800 0801 1203 080d 0c17  .s..............
+000002a0: 057c 0444 005d 2b7d 067c 06a0 0864 0564  .|.D.]+}.|...d.d
+000002b0: 06a1 027d 067c 06a0 0864 0764 06a1 027d  ...}.|...d.d...}
+000002c0: 067c 06a0 0864 0864 06a1 027d 067c 06a0  .|...d.d...}.|..
+000002d0: 0864 0964 0aa1 027d 067c 06a0 09a1 00a0  .d.d...}.|......
+000002e0: 0864 0b64 0ca1 02a0 0864 0d64 0ea1 027d  .d.d.....d.d...}
+000002f0: 077c 05a0 0a7c 07a1 0101 0071 357c 05a0  .|...|.....q5|..
+00000300: 0a64 0fa1 0101 007c 05a0 0a64 1064 11a0  .d.....|...d.d..
+00000310: 057c 0564 1264 1385 0219 00a1 0117 0064  .|.d.d.........d
+00000320: 1417 00a1 0101 0064 11a0 057c 05a1 0153  .......d...|...S
+00000330: 0029 154e 7a0e 6865 6c6c 6f5f 776f 726c  .).Nz.hello_worl
+00000340: 642e 7079 fa01 2f72 0400 0000 7a66 3c64  d.py../r....zf<d
+00000350: 6976 2073 7479 6c65 3d22 666f 6e74 2d73  iv style="font-s
+00000360: 697a 653a 312e 3165 6d3b 7061 6464 696e  ize:1.1em;paddin
+00000370: 673a 3135 7078 3b62 6163 6b67 726f 756e  g:15px;backgroun
+00000380: 642d 636f 6c6f 723a 2366 6466 6663 373b  d-color:#fdffc7;
+00000390: 2064 6973 706c 6179 3a20 696e 6c69 6e65   display: inline
+000003a0: 2d62 6c6f 636b 3b22 3e3c 7072 653e 3c63  -block;"><pre><c
+000003b0: 6f64 653e 7a0a 696d 706f 7274 2073 7973  ode>z.import sys
+000003c0: da00 7a09 696d 706f 7274 206f 737a 4f73  ..z.import oszOs
+000003d0: 7973 2e70 6174 682e 6170 7065 6e64 286f  ys.path.append(o
+000003e0: 732e 7061 7468 2e61 6273 7061 7468 286f  s.path.abspath(o
+000003f0: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
+00000400: 6174 682e 6469 726e 616d 6528 5f5f 6669  ath.dirname(__fi
+00000410: 6c65 5f5f 292c 2027 2e2e 2729 2929 7a11  le__), '..')))z.
+00000420: 696d 706f 7274 206d 6169 6e20 6173 2077  import main as w
+00000430: 737a 1669 6d70 6f72 7420 7765 6273 6c69  sz.import websli
+00000440: 6465 7320 6173 2077 73fa 013c 7a04 266c  des as ws..<z.&l
+00000450: 743b fa01 3e7a 0426 6774 3bfa 133c 2f63  t;..>z.&gt;..</c
+00000460: 6f64 653e 3c2f 7072 653e 3c2f 6469 763e  ode></pre></div>
+00000470: 7aaf 3c62 723e 3c62 723e 3c62 7574 746f  z.<br><br><butto
+00000480: 6e20 7374 796c 653d 2266 6f6e 742d 7369  n style="font-si
+00000490: 7a65 3a20 312e 3365 6d3b 2062 6163 6b67  ze: 1.3em; backg
+000004a0: 726f 756e 642d 636f 6c6f 723a 2023 3030  round-color: #00
+000004b0: 6262 3030 3b63 6f6c 6f72 3a20 7768 6974  bb00;color: whit
+000004c0: 653b 626f 7264 6572 2d63 6f6c 6f72 3a20  e;border-color: 
+000004d0: 2363 3763 3763 3720 2169 6d70 6f72 7461  #c7c7c7 !importa
+000004e0: 6e74 3b20 626f 7264 6572 2d72 6164 6975  nt; border-radiu
+000004f0: 733a 2036 7078 3b22 206f 6e63 6c69 636b  s: 6px;" onclick
+00000500: 3d22 6e61 7669 6761 746f 722e 636c 6970  ="navigator.clip
+00000510: 626f 6172 642e 7772 6974 6554 6578 7428  board.writeText(
+00000520: 60da 010a 7205 0000 00e9 ffff ffff 7a40  `...r.........z@
+00000530: 6029 3b61 6c65 7274 2827 436f 6465 2063  `);alert('Code c
+00000540: 6f70 6965 6420 746f 2063 6c69 7062 6f61  opied to clipboa
+00000550: 7264 2729 3b22 3e3c 623e 434f 5059 2043  rd');"><b>COPY C
+00000560: 4f44 453c 2f62 3e3c 2f62 7574 746f 6e3e  ODE</b></button>
+00000570: 290b da02 6f73 da04 7061 7468 da07 6469  )...os..path..di
+00000580: 726e 616d 65da 0761 6273 7061 7468 da08  rname..abspath..
+00000590: 5f5f 6669 6c65 5f5f da04 6a6f 696e 7206  __file__..joinr.
+000005a0: 0000 00da 0972 6561 646c 696e 6573 da07  .....readlines..
+000005b0: 7265 706c 6163 65da 0672 7374 7269 70da  replace..rstrip.
+000005c0: 0661 7070 656e 6429 08da 0566 6e61 6d65  .append)...fname
+000005d0: da0b 6375 7272 656e 745f 6469 72da 0566  ..current_dir..f
+000005e0: 7061 7468 da01 665a 0a63 6f64 655f 6c69  path..fZ.code_li
+000005f0: 6e65 735a 0a68 746d 6c5f 6c69 6e65 73da  nesZ.html_lines.
+00000600: 046c 696e 655a 0968 746d 6c5f 6c69 6e65  .lineZ.html_line
+00000610: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000620: 1068 656c 6c6f 5f77 6f72 6c64 5f68 746d  .hello_world_htm
+00000630: 6c12 0000 0073 3000 0000 0401 1401 0c01  l....s0.........
+00000640: 1601 0a01 1cff 0204 04ff 0802 0c01 0c01  ................
+00000650: 0c01 0c01 1801 0c01 0a01 0403 0601 0a01  ................
+00000660: 04ff 0201 02ff 04ff 0a04 7228 0000 0063  ..........r(...c
+00000670: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000680: 0300 0000 4300 0000 730c 0000 0064 017c  ....C...s....d.|
+00000690: 009b 0064 029d 0353 0029 034e 7a66 3c64  ...d...S.).Nzf<d
+000006a0: 6976 2073 7479 6c65 3d22 6261 636b 6772  iv style="backgr
+000006b0: 6f75 6e64 2d63 6f6c 6f72 3a23 6664 6666  ound-color:#fdff
+000006c0: 6337 3b20 6469 7370 6c61 793a 2069 6e6c  c7; display: inl
+000006d0: 696e 652d 626c 6f63 6b3b 666f 6e74 2d73  ine-block;font-s
+000006e0: 697a 653a 312e 3165 6d3b 7061 6464 696e  ize:1.1em;paddin
+000006f0: 673a 3135 7078 3b22 3e3c 7072 653e 3c63  g:15px;"><pre><c
+00000700: 6f64 653e 7216 0000 0072 0f00 0000 2901  ode>r....r....).
+00000710: da04 636f 6465 720f 0000 0072 0f00 0000  ..coder....r....
+00000720: 7210 0000 00da 0c63 6f64 655f 746f 5f68  r......code_to_h
+00000730: 746d 6c2c 0000 0073 0200 0000 0c02 722a  tml,...s......r*
+00000740: 0000 0029 0672 1900 0000 7208 0000 00da  ...).r....r.....
+00000750: 0373 7472 7211 0000 0072 2800 0000 722a  .strr....r(...r*
+00000760: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000770: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000780: 3e01 0000 0073 0a00 0000 0800 0801 1203  >....s..........
+00000790: 080d 0c1a                                ....
```

### Comparing `webslides-0.6.0/webslides/modules/__pycache__/tohtml.cpython-310.pyc` & `webslides-0.6.3/webslides/modules/__pycache__/tohtml.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 18:40:55 2023 UTC, .py size: 7774 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,397 +1,420 @@
-00000000: 6f0d 0d0a 0000 0000 3741 3c64 5e1e 0000  o.......7A<d^...
+00000000: 6f0d 0d0a 0000 0000 983a 5a64 2921 0000  o........:Zd)!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000020: 0007 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6402 6403 8400 5a05 0904 0904 6415  ..d.d...Z.....d.
-00000050: 6405 6406 8401 5a06 6407 6408 8400 5a07  d.d...Z.d.d...Z.
-00000060: 6416 640b 640c 8401 5a08 640d 640e 8400  d.d.d...Z.d.d...
-00000070: 5a09 640f 6410 8400 5a0a 6411 6412 8400  Z.d.d...Z.d.d...
-00000080: 5a0b 6413 6414 8400 5a0c 6401 5300 2917  Z.d.d...Z.d.S.).
-00000090: e900 0000 004e 6302 0000 0000 0000 0000  .....Nc.........
-000000a0: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
-000000b0: ec00 0000 6401 7c01 7600 7215 7400 7c01  ....d.|.v.r.t.|.
-000000c0: 6401 1900 8301 6402 6b04 7215 6403 7c01  d.....d.k.r.d.|.
-000000d0: 6401 1900 1700 6404 1700 7d02 6e03 7401  d.....d...}.n.t.
-000000e0: 8300 7d02 6405 7d03 7c03 a002 6406 7c02  ..}.d.}.|...d.|.
-000000f0: a102 7d03 7c03 a002 6407 7c01 6408 1900  ..}.|...d.|.d...
-00000100: a102 7d03 6409 7d04 7c01 640a 1900 a003  ..}.d.}.|.d.....
-00000110: a100 4400 5d0f 5c02 7d05 7d06 7c04 640b  ..D.].\.}.}.|.d.
-00000120: 7c05 9b00 640c 7c06 9b00 640d 9d05 3700  |...d.|...d...7.
-00000130: 7d04 7130 7c04 640e 3700 7d04 7c03 a002  }.q0|.d.7.}.|...
-00000140: 640f 7c04 a102 7d03 7c00 a002 6410 7c03  d.|...}.|...d.|.
-00000150: 6410 1700 a102 7d00 6411 7c01 7600 7274  d.....}.d.|.v.rt
-00000160: 7c01 6411 1900 7d07 7c07 a004 7405 6a06  |.d...}.|...t.j.
-00000170: a007 a100 a008 6412 a101 9b00 a101 0100  ......d.........
-00000180: 7409 7c01 6411 1900 8301 7d08 7c00 a002  t.|.d.....}.|...
-00000190: 6410 7c08 6410 1700 a102 7d00 7c00 5300  d.|.d.....}.|.S.
-000001a0: 2913 4eda 0769 6d67 5f75 726c 7201 0000  ).N..img_urlr...
-000001b0: 007a 0a3c 696d 6720 7372 633d 277a 2327  .z.<img src='z#'
-000001c0: 2073 7479 6c65 3d27 7769 6474 683a 3230   style='width:20
-000001d0: 3070 783b 6d61 7267 696e 3a31 3070 783b  0px;margin:10px;
-000001e0: 273e 61dc 0100 003c 7374 796c 653e 0a20  '>a....<style>. 
-000001f0: 2020 202e 636f 6e74 6169 6e65 7220 7b70     .container {p
-00000200: 6f73 6974 696f 6e3a 2072 656c 6174 6976  osition: relativ
-00000210: 653b 2068 6569 6768 743a 2036 3030 7078  e; height: 600px
-00000220: 3b7d 0a20 2020 202e 6365 6e74 6572 6564  ;}.    .centered
-00000230: 2d65 6c65 6d65 6e74 207b 7465 7874 2d61  -element {text-a
-00000240: 6c69 676e 3a20 6365 6e74 6572 3b20 6d61  lign: center; ma
-00000250: 7267 696e 3a20 303b 2077 6964 7468 3a38  rgin: 0; width:8
-00000260: 3025 3b20 706f 7369 7469 6f6e 3a20 6162  0%; position: ab
-00000270: 736f 6c75 7465 3b20 746f 703a 2035 3025  solute; top: 50%
-00000280: 3b20 6c65 6674 3a20 3530 253b 202d 6d73  ; left: 50%; -ms
-00000290: 2d74 7261 6e73 666f 726d 3a20 7472 616e  -transform: tran
-000002a0: 736c 6174 6528 2d35 3025 2c20 2d35 3025  slate(-50%, -50%
-000002b0: 293b 2074 7261 6e73 666f 726d 3a20 7472  ); transform: tr
-000002c0: 616e 736c 6174 6528 2d35 3025 2c20 2d35  anslate(-50%, -5
-000002d0: 3025 293b 7d0a 2020 2020 3c2f 7374 796c  0%);}.    </styl
-000002e0: 653e 0a20 2020 203c 6469 7620 636c 6173  e>.    <div clas
-000002f0: 733d 2763 6f6e 7461 696e 6572 273e 0a20  s='container'>. 
-00000300: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000310: 733d 2763 656e 7465 7265 642d 656c 656d  s='centered-elem
-00000320: 656e 7427 3e0a 2020 2020 2020 2020 2020  ent'>.          
-00000330: 2020 5641 525f 494d 4147 455f 4854 4d4c    VAR_IMAGE_HTML
-00000340: 0a20 2020 2020 2020 2020 2020 203c 6831  .            <h1
-00000350: 3e56 4152 5f54 4954 4c45 3c2f 6831 3e3c  >VAR_TITLE</h1><
-00000360: 6272 3e0a 2020 2020 2020 2020 2020 2020  br>.            
-00000370: 3c70 2073 7479 6c65 3d27 6c69 6e65 2d68  <p style='line-h
-00000380: 6569 6768 743a 2031 2e35 3b27 3e0a 2020  eight: 1.5;'>.  
-00000390: 2020 2020 2020 2020 2020 5641 525f 5355            VAR_SU
-000003a0: 4d4d 4152 593c 2f70 3e0a 2020 2020 2020  MMARY</p>.      
-000003b0: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-000003c0: 6976 3eda 0e56 4152 5f49 4d41 4745 5f48  iv>..VAR_IMAGE_H
-000003d0: 544d 4c5a 0956 4152 5f54 4954 4c45 da05  TMLZ.VAR_TITLE..
-000003e0: 7469 746c 6561 0401 0000 0a20 2020 2020  titlea.....     
-000003f0: 2020 203c 7461 626c 6520 7374 796c 653d     <table style=
-00000400: 2277 6964 7468 3a20 3130 3025 3b20 7465  "width: 100%; te
-00000410: 7874 2d61 6c69 676e 3a20 6c65 6674 3b20  xt-align: left; 
-00000420: 666f 6e74 2d73 697a 653a 2031 656d 3b20  font-size: 1em; 
-00000430: 626f 7264 6572 2d63 6f6c 6c61 7073 653a  border-collapse:
-00000440: 2063 6f6c 6c61 7073 653b 2062 6f72 6465   collapse; borde
-00000450: 723a 2030 3b22 3e0a 2020 2020 2020 2020  r: 0;">.        
-00000460: 2020 2020 3c63 6f6c 6772 6f75 703e 0a20      <colgroup>. 
-00000470: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000480: 636f 6c20 7374 796c 653d 2277 6964 7468  col style="width
-00000490: 3a20 3230 253b 223e 0a20 2020 2020 2020  : 20%;">.       
-000004a0: 2020 2020 2020 2020 203c 636f 6c20 7374           <col st
-000004b0: 796c 653d 2277 6964 7468 3a20 3830 253b  yle="width: 80%;
-000004c0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-000004d0: 2f63 6f6c 6772 6f75 703e 0a20 2020 2020  /colgroup>.     
-000004e0: 2020 2020 2020 203c 7462 6f64 793e da07         <tbody>..
-000004f0: 7375 6d6d 6172 797a a70a 2020 2020 2020  summaryz..      
-00000500: 2020 2020 2020 2020 2020 3c74 7220 7374            <tr st
-00000510: 796c 653d 2262 6f72 6465 723a 2030 3b22  yle="border: 0;"
-00000520: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000530: 2020 2020 2020 3c74 6420 7374 796c 653d        <td style=
-00000540: 2262 6f72 6465 723a 2030 3b20 7061 6464  "border: 0; padd
-00000550: 696e 673a 2031 3070 783b 2074 6578 742d  ing: 10px; text-
-00000560: 6465 636f 7261 7469 6f6e 3a20 756e 6465  decoration: unde
-00000570: 726c 696e 653b 2076 6572 7469 6361 6c2d  rline; vertical-
-00000580: 616c 6967 6e3a 2074 6f70 3b20 7465 7874  align: top; text
-00000590: 2d61 6c69 676e 3a20 7269 6768 743b 223e  -align: right;">
-000005a0: 7a40 3c2f 7464 3e0a 2020 2020 2020 2020  z@</td>.        
-000005b0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-000005c0: 7374 796c 653d 2262 6f72 6465 723a 2030  style="border: 0
-000005d0: 3b20 7061 6464 696e 673a 2031 3070 783b  ; padding: 10px;
-000005e0: 223e 7a2c 3c2f 7464 3e0a 2020 2020 2020  ">z,</td>.      
-000005f0: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 7a4e 0a20 2020 2020 2020 2020 2020 2020  zN.             
-00000620: 2020 203c 212d 2d20 6d6f 7265 2072 6f77     <!-- more row
-00000630: 7320 6865 7265 202d 2d3e 0a20 2020 2020  s here -->.     
-00000640: 2020 2020 2020 203c 2f74 626f 6479 3e0a         </tbody>.
-00000650: 2020 2020 2020 2020 3c2f 7461 626c 653e          </table>
-00000660: 5a0b 5641 525f 5355 4d4d 4152 59fa 0d3c  Z.VAR_SUMMARY..<
-00000670: 7370 616e 3e3c 2f73 7061 6e3e da06 666f  span></span>..fo
-00000680: 6f74 6572 7a09 2565 2025 622e 2025 5929  oterz.%e %b. %Y)
-00000690: 0ada 036c 656e da0c 7773 5f6c 6f67 6f5f  ...len..ws_logo_
-000006a0: 6874 6d6c da07 7265 706c 6163 65da 0569  html..replace..i
-000006b0: 7465 6d73 da06 6170 7065 6e64 da02 6474  tems..append..dt
-000006c0: da08 6461 7465 7469 6d65 da03 6e6f 77da  ..datetime..now.
-000006d0: 0873 7472 6674 696d 65da 0e66 6f6f 7465  .strftime..foote
-000006e0: 725f 746f 5f68 746d 6c29 09da 0468 746d  r_to_html)...htm
-000006f0: 6cda 0470 6167 6572 0300 0000 5a09 7469  l..pager....Z.ti
-00000700: 746c 6570 6167 655a 0c73 756d 6d61 7279  tlepageZ.summary
-00000710: 5f68 746d 6cda 016b da01 7672 0700 0000  _html..k..vr....
-00000720: da0b 666f 6f74 6572 5f68 746d 6ca9 0072  ..footer_html..r
-00000730: 1700 0000 fa4f 433a 5c55 7365 7273 5c64  .....OC:\Users\d
-00000740: 6572 6b2d 6a61 6e2e 776f 6c74 6a65 725c  erk-jan.woltjer\
-00000750: 5079 6368 6172 6d50 726f 6a65 6374 735c  PycharmProjects\
-00000760: 7765 6273 6c69 6465 735c 7765 6273 6c69  webslides\websli
-00000770: 6465 735c 6d6f 6475 6c65 735c 746f 6874  des\modules\toht
-00000780: 6d6c 2e70 79da 1174 6974 6c65 7061 6765  ml.py..titlepage
-00000790: 5f74 6f5f 6874 6d6c 0500 0000 732c 0000  _to_html....s,..
-000007a0: 0018 0212 0306 0504 030c 0d10 0104 0314  ................
-000007b0: 0804 0102 0204 fe02 030c fd08 060c 0510  ................
-000007c0: 0208 0308 0118 010c 0110 0104 0272 1900  .............r..
-000007d0: 0000 4663 0700 0000 0000 0000 0000 0000  ..Fc............
-000007e0: 0c00 0000 0a00 0000 4300 0000 7308 0100  ........C...s...
-000007f0: 007c 0672 2074 007c 0164 0119 007c 0164  .|.r t.|.d...|.d
-00000800: 0219 007c 047c 057c 01a0 0164 0364 00a1  ...|.|.|...d.d..
-00000810: 027c 01a0 0164 0464 00a1 0264 058d 067d  .|...d.d...d...}
-00000820: 077c 00a0 0264 067c 0764 0617 00a1 027d  .|...d.|.d.....}
-00000830: 0064 077c 0176 0072 407c 0164 0719 0064  .d.|.v.r@|.d...d
-00000840: 086b 0372 4074 037c 0164 0919 007c 0164  .k.r@t.|.d...|.d
-00000850: 0a19 007c 0164 0719 007c 027c 0383 057d  ...|.d...|.|...}
-00000860: 087c 00a0 0264 067c 0864 0617 00a1 027d  .|...d.|.d.....}
-00000870: 0064 0b7c 0176 0072 587c 0164 0b19 0064  .d.|.v.rX|.d...d
-00000880: 086b 0372 5874 047c 0164 0b19 0083 017d  .k.rXt.|.d.....}
-00000890: 097c 00a0 0264 067c 0964 0617 00a1 027d  .|...d.|.d.....}
-000008a0: 0064 0c7c 0176 0072 6a74 057c 0164 0c19  .d.|.v.rjt.|.d..
-000008b0: 0083 017d 0a7c 00a0 0264 067c 0a64 0617  ...}.|...d.|.d..
-000008c0: 00a1 027d 0064 0d7c 0176 0072 827c 0164  ...}.d.|.v.r.|.d
-000008d0: 0d19 0064 086b 0372 8274 067c 0164 0d19  ...d.k.r.t.|.d..
-000008e0: 0083 017d 0b7c 00a0 0264 067c 0b64 0617  ...}.|...d.|.d..
-000008f0: 00a1 027d 007c 0053 0029 0e4e da06 7061  ...}.|.S.).N..pa
-00000900: 6765 6e6f da07 7061 6765 6b65 795a 0b68  geno..pagekeyZ.h
-00000910: 6c5f 7072 6576 5f6b 6579 5a0b 686c 5f6e  l_prev_keyZ.hl_n
-00000920: 6578 745f 6b65 7929 0672 1a00 0000 721b  ext_key).r....r.
-00000930: 0000 00da 0f73 686f 775f 696e 6465 785f  .....show_index_
-00000940: 7061 6765 da14 7368 6f77 5f68 6967 686c  page..show_highl
-00000950: 6967 6874 735f 7061 6765 da12 7072 6576  ights_page..prev
-00000960: 5f68 6967 686c 6967 6874 5f6b 6579 da12  _highlight_key..
-00000970: 6e65 7874 5f68 6967 686c 6967 6874 5f6b  next_highlight_k
-00000980: 6579 7206 0000 0072 0400 0000 da00 da06  eyr....r........
-00000990: 746f 7063 6174 da06 7375 6263 6174 da0a  topcat..subcat..
-000009a0: 6869 6768 6c69 6768 7473 da04 626f 6479  highlights..body
-000009b0: 7207 0000 0029 07da 1070 6167 656e 6176  r....)...pagenav
-000009c0: 695f 746f 5f68 746d 6cda 0367 6574 720a  i_to_html..getr.
-000009d0: 0000 00da 0d74 6974 6c65 5f74 6f5f 6874  .....title_to_ht
-000009e0: 6d6c da12 6869 6768 6c69 6768 7473 5f74  ml..highlights_t
-000009f0: 6f5f 6874 6d6c da0c 626f 6479 5f74 6f5f  o_html..body_to_
-00000a00: 6874 6d6c 7211 0000 0029 0c72 1200 0000  htmlr....).r....
-00000a10: 7213 0000 00da 0b73 686f 775f 746f 7063  r......show_topc
-00000a20: 6174 da0b 7368 6f77 5f73 7562 6361 7472  at..show_subcatr
-00000a30: 1c00 0000 721d 0000 00da 0973 686f 775f  ....r......show_
-00000a40: 6e61 7669 5a08 7061 6765 6e61 7669 7204  naviZ.pagenavir.
-00000a50: 0000 005a 0f68 6967 686c 6967 6874 735f  ...Z.highlights_
-00000a60: 6874 6d6c 5a09 626f 6479 5f68 746d 6c72  htmlZ.body_htmlr
-00000a70: 1600 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000a80: 0000 00da 0f63 6f6e 7465 6e74 5f74 6f5f  .....content_to_
-00000a90: 6874 6d6c 4500 0000 732c 0000 0004 0308  htmlE...s,......
-00000aa0: 0106 0102 0102 010a 010a 0106 fb10 0614  ................
-00000ab0: 031c 0110 0114 030c 0110 0108 030c 0110  ................
-00000ac0: 0114 030c 0110 0104 0272 2d00 0000 6306  .........r-...c.
-00000ad0: 0000 0000 0000 0000 0000 000b 0000 0006  ................
-00000ae0: 0000 0043 0000 0073 6e00 0000 7c04 6401  ...C...sn...|.d.
-00000af0: 6b02 7206 6401 6e05 6402 7c04 9b00 6403  k.r.d.n.d.|...d.
-00000b00: 9d03 7d06 7c05 6401 6b02 7212 6401 6e05  ..}.|.d.k.r.d.n.
-00000b10: 6404 7c05 9b00 6405 9d03 7d07 6406 7c03  d.|...d...}.d.|.
-00000b20: 9b00 6407 9d03 7c01 1400 7d08 7c06 9b00  ..d...|...}.|...
-00000b30: 6408 7c07 9b00 6409 9d04 7c02 1400 7d09  d.|...d...|...}.
-00000b40: 640a 7c09 9b00 7c08 9b00 640b 7c00 9b00  d.|...|...d.|...
-00000b50: 640c 9d06 7d0a 7c0a 5300 290d 61d2 0200  d...}.|.S.).a...
-00000b60: 000a 2020 2020 3a70 6172 616d 2070 6167  ..    :param pag
-00000b70: 656e 6f3a 2069 6e74 2070 6167 656e 756d  eno: int pagenum
-00000b80: 6265 720a 2020 2020 3a70 6172 616d 206e  ber.    :param n
-00000b90: 616d 653a 2073 7472 206e 616d 6520 6f66  ame: str name of
-00000ba0: 2074 6865 2068 746d 6c20 7061 6765 2028   the html page (
-00000bb0: 6964 2075 7365 6420 746f 206e 6176 6967  id used to navig
-00000bc0: 6174 6520 746f 2074 6869 7320 7061 6765  ate to this page
-00000bd0: 2c20 6965 2e20 6672 6f6d 2069 6e64 6578  , ie. from index
-00000be0: 2070 6167 6529 0a20 2020 203a 7061 7261   page).    :para
-00000bf0: 6d20 7368 6f77 5f69 6e64 6578 5f70 6167  m show_index_pag
-00000c00: 653a 2062 6f6f 6c20 6966 2046 616c 7365  e: bool if False
-00000c10: 2c20 7265 6665 7265 6e63 6573 2074 6f20  , references to 
-00000c20: 696e 6465 7820 7061 6765 2061 7265 206f  index page are o
-00000c30: 6d69 7474 6564 0a20 2020 203a 7061 7261  mitted.    :para
-00000c40: 6d20 7368 6f77 5f68 6967 686c 6967 6874  m show_highlight
-00000c50: 735f 7061 6765 3a20 626f 6f6c 2069 6620  s_page: bool if 
-00000c60: 4661 6c73 652c 2072 6566 6572 656e 6365  False, reference
-00000c70: 7320 746f 2068 6967 686c 6967 6874 7320  s to highlights 
-00000c80: 7061 6765 2061 7265 206f 6d69 7474 6564  page are omitted
-00000c90: 0a20 2020 203a 7061 7261 6d20 7072 6576  .    :param prev
-00000ca0: 5f68 6967 686c 6967 6874 5f6b 6579 3a20  _highlight_key: 
-00000cb0: 7374 7220 6874 6d6c 2069 6420 6f66 2070  str html id of p
-00000cc0: 7265 7669 6f75 7320 6869 6768 6c69 6768  revious highligh
-00000cd0: 7420 7061 6765 0a20 2020 203a 7061 7261  t page.    :para
-00000ce0: 6d20 6e65 7874 5f68 6967 686c 6967 6874  m next_highlight
-00000cf0: 5f6b 6579 3a20 7374 7220 6874 6d6c 2069  _key: str html i
-00000d00: 6420 6f66 206e 6578 7420 6869 6768 6c69  d of next highli
-00000d10: 6768 7420 7061 6765 0a20 2020 203a 7265  ght page.    :re
-00000d20: 7475 726e 3a20 7374 7269 6e67 2068 746d  turn: string htm
-00000d30: 6c20 636f 6465 2074 6f20 706c 6163 6520  l code to place 
-00000d40: 6f6e 2074 6f70 206f 6620 6561 6368 2070  on top of each p
-00000d50: 6167 652c 2075 7365 6420 666f 720a 2020  age, used for.  
-00000d60: 2020 2020 2020 2d20 6e61 7669 6761 7469        - navigati
-00000d70: 6f6e 2074 6f20 6e65 7874 2f70 7265 7669  on to next/previ
-00000d80: 6f75 7320 6869 6768 6c69 6768 7420 7061  ous highlight pa
-00000d90: 6765 0a20 2020 2020 2020 202d 206e 6176  ge.        - nav
-00000da0: 6967 6174 696f 6e20 746f 2069 6e64 6578  igation to index
-00000db0: 2070 6167 650a 2020 2020 2020 2020 2d20   page.        - 
-00000dc0: 6e61 7669 6761 7469 6f6e 2074 6f20 6869  navigation to hi
-00000dd0: 6768 6c69 6768 7473 2070 6167 650a 2020  ghlights page.  
-00000de0: 2020 2020 2020 2d20 6469 7370 6c61 7920        - display 
-00000df0: 7061 6765 6e75 6d62 6572 0a20 2020 2020  pagenumber.     
-00000e00: 2020 202d 2070 6167 6520 6964 2074 6167     - page id tag
-00000e10: 2075 7365 6420 746f 206e 6176 6967 6174   used to navigat
-00000e20: 6520 746f 2074 6861 7420 7061 6765 0a20  e to that page. 
-00000e30: 2020 2072 2000 0000 7a25 3c61 2074 6974     r ...z%<a tit
-00000e40: 6c65 3d22 5072 6576 696f 7573 2068 6967  le="Previous hig
-00000e50: 686c 6967 6874 2220 6872 6566 3d22 237a  hlight" href="#z
-00000e60: 0d22 3e26 2339 3636 343b 3c2f 613e 7a21  .">&#9664;</a>z!
-00000e70: 3c61 2074 6974 6c65 3d22 4e65 7874 2068  <a title="Next h
-00000e80: 6967 686c 6967 6874 2220 6872 6566 3d22  ighlight" href="
-00000e90: 237a 0d22 3e26 2339 3635 383b 3c2f 613e  #z.">&#9658;</a>
-00000ea0: 7a07 3c61 2069 643d 227a 3e22 2074 6974  z.<a id="z>" tit
-00000eb0: 6c65 3d22 5461 626c 6520 6f66 2063 6f6e  le="Table of con
-00000ec0: 7465 6e74 7322 2068 7265 663d 2223 6964  tents" href="#id
-00000ed0: 5f63 6f6e 7465 6e74 7322 3e26 2331 3238  _contents">&#128
-00000ee0: 3139 363b 3c2f 613e 207a 4020 3c61 2074  196;</a> z@ <a t
-00000ef0: 6974 6c65 3d22 4869 6768 6c69 6768 7473  itle="Highlights
-00000f00: 2073 756d 6d61 7279 2220 6872 6566 3d22   summary" href="
-00000f10: 2368 6967 686c 6967 6874 7322 3e26 2331  #highlights">&#1
-00000f20: 3238 3136 313b 3c2f 613e 20da 0120 7a4b  28161;</a> .. zK
-00000f30: 3c64 6976 2063 6c61 7373 3d22 666f 6f74  <div class="foot
-00000f40: 6572 2220 7374 796c 653d 2277 6964 7468  er" style="width
-00000f50: 3a20 3130 3025 3b20 6d61 7267 696e 3a20  : 100%; margin: 
-00000f60: 3020 6175 746f 3b20 7465 7874 2d61 6c69  0 auto; text-ali
-00000f70: 676e 3a72 6967 6874 3b22 3eda 0170 fa06  gn:right;">..p..
-00000f80: 3c2f 6469 763e 7217 0000 0029 0b72 1a00  </div>r....).r..
-00000f90: 0000 721c 0000 0072 1d00 0000 721b 0000  ..r....r....r...
-00000fa0: 0072 1e00 0000 721f 0000 005a 096c 696e  .r....r....Z.lin
-00000fb0: 6b5f 7072 6576 5a09 6c69 6e6b 5f6e 6578  k_prevZ.link_nex
-00000fc0: 745a 1370 6167 656e 6176 695f 696e 6465  tZ.pagenavi_inde
-00000fd0: 785f 7061 6765 5a18 7061 6765 6e61 7669  x_pageZ.pagenavi
-00000fe0: 5f68 6967 686c 6967 6874 735f 7061 6765  _highlights_page
-00000ff0: 5a0d 7061 6765 6e61 7669 5f68 746d 6c72  Z.pagenavi_htmlr
-00001000: 1700 0000 7217 0000 0072 1800 0000 7225  ....r....r....r%
-00001010: 0000 0068 0000 0073 0c00 0000 1810 1801  ...h...s........
-00001020: 1002 1401 1602 0402 7225 0000 0072 2000  ........r%...r .
-00001030: 0000 5463 0500 0000 0000 0000 0000 0000  ..Tc............
-00001040: 0500 0000 0500 0000 4300 0000 7358 0000  ........C...sX..
-00001050: 0074 007c 0083 0164 016b 0472 0e64 027c  .t.|...d.k.r.d.|
-00001060: 00a0 01a1 009b 0064 039d 036e 0164 047d  .......d...n.d.}
-00001070: 0074 007c 0183 0164 016b 0472 1c64 057c  .t.|...d.k.r.d.|
-00001080: 019b 0064 069d 036e 0164 047d 0164 077c  ...d...n.d.}.d.|
-00001090: 037c 0014 009b 007c 047c 0114 009b 007c  .|.....|.|.....|
-000010a0: 029b 0064 089d 0553 0029 097a 570a 2020  ...d...S.).zW.  
-000010b0: 2020 3a70 6172 616d 2074 6974 6c65 3a20    :param title: 
-000010c0: 7374 7220 7469 746c 6520 6f66 2068 746d  str title of htm
-000010d0: 6c20 7061 6765 0a20 2020 203a 7265 7475  l page.    :retu
-000010e0: 726e 3a20 7374 7269 6e67 2068 746d 6c20  rn: string html 
-000010f0: 666f 726d 6174 7465 6420 7469 746c 650a  formatted title.
-00001100: 2020 2020 7201 0000 007a 443c 7370 616e      r....zD<span
-00001110: 2073 7479 6c65 3d27 636f 6c6f 723a 2077   style='color: w
-00001120: 6869 7465 3b20 6261 636b 6772 6f75 6e64  hite; background
-00001130: 2d63 6f6c 6f72 3a20 2330 3038 4143 393b  -color: #008AC9;
-00001140: 2070 6164 6469 6e67 3a35 7078 3b27 3e7a   padding:5px;'>z
-00001150: 083c 2f73 7061 6e3e 2072 2000 0000 7a23  .</span> r ...z#
-00001160: 3c73 7061 6e20 7374 796c 653d 2766 6f6e  <span style='fon
-00001170: 742d 7765 6967 6874 3a20 6e6f 726d 616c  t-weight: normal
-00001180: 3b27 3e7a 093c 2f73 7061 6e3e 3a20 7a1c  ;'>z.</span>: z.
-00001190: 3c68 3320 7374 796c 653d 276c 696e 652d  <h3 style='line-
-000011a0: 6865 6967 6874 3a20 323b 273e 7a05 3c2f  height: 2;'>z.</
-000011b0: 6833 3e29 0272 0800 0000 da05 7570 7065  h3>).r......uppe
-000011c0: 7229 0572 2100 0000 7222 0000 0072 0400  r).r!...r"...r..
-000011d0: 0000 722a 0000 0072 2b00 0000 7217 0000  ..r*...r+...r...
-000011e0: 0072 1700 0000 7218 0000 0072 2700 0000  .r....r....r'...
-000011f0: 8300 0000 7312 0000 0002 0502 0102 ff02  ....s...........
-00001200: 0114 ff02 0102 ff1c 021c 0172 2700 0000  ...........r'...
-00001210: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00001220: 0004 0000 0043 0000 00f3 2800 0000 6401  .....C....(...d.
-00001230: 7d01 7c00 4400 5d09 7d02 7c01 7c02 9b00  }.|.D.].}.|.|...
-00001240: 6402 9d02 3700 7d01 7104 7c01 6403 3700  d...7.}.q.|.d.7.
-00001250: 7d01 7c01 5300 2904 7a65 0a20 2020 203a  }.|.S.).ze.    :
-00001260: 7061 7261 6d20 636f 6d6d 656e 7473 3a20  param comments: 
-00001270: 6c69 7374 2077 6974 6820 7465 7874 2074  list with text t
-00001280: 6f20 7368 6f77 2069 6e20 6865 6164 6572  o show in header
-00001290: 0a20 2020 203a 7265 7475 726e 3a20 7374  .    :return: st
-000012a0: 7269 6e67 2068 746d 6c20 666f 726d 6174  ring html format
-000012b0: 7465 6420 6865 6164 6572 0a20 2020 207a  ted header.    z
-000012c0: 483c 6469 7620 7374 796c 653d 2262 6163  H<div style="bac
-000012d0: 6b67 726f 756e 642d 636f 6c6f 723a 2023  kground-color: #
-000012e0: 4542 4542 4542 3b20 6c69 6e65 2d68 6569  EBEBEB; line-hei
-000012f0: 6768 743a 2031 2e36 3b20 7061 6464 696e  ght: 1.6; paddin
-00001300: 673a 3130 7078 3b22 3efa 043c 6272 3e72  g:10px;">..<br>r
-00001310: 3000 0000 7217 0000 0029 0372 2300 0000  0...r....).r#...
-00001320: 7212 0000 00da 016f 7217 0000 0072 1700  r......or....r..
-00001330: 0000 7218 0000 0072 2800 0000 8e00 0000  ..r....r(.......
-00001340: f308 0000 0004 0518 0108 0104 0172 2800  .............r(.
-00001350: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001360: 0000 0006 0000 0043 0000 0073 2e00 0000  .......C...s....
-00001370: 7400 7c00 7401 8302 720b 6401 7c00 9b00  t.|.t...r.d.|...
-00001380: 6402 9d03 5300 6401 7402 6a03 7c00 6403  d...S.d.t.j.|.d.
-00001390: 6404 6405 8d03 9b00 6402 9d03 5300 2906  d.d.....d...S.).
-000013a0: 4e7a 183c 6469 7620 7374 796c 653d 2770  Nz.<div style='p
-000013b0: 6164 6469 6e67 3a33 2527 3e72 3000 0000  adding:3%'>r0...
-000013c0: 46da 0364 6976 2902 da10 696e 636c 7564  F..div)...includ
-000013d0: 655f 706c 6f74 6c79 6a73 da0b 6f75 7470  e_plotlyjs..outp
-000013e0: 7574 5f74 7970 6529 04da 0a69 7369 6e73  ut_type)...isins
-000013f0: 7461 6e63 65da 0373 7472 da02 706f da04  tance..str..po..
-00001400: 706c 6f74 2901 7224 0000 0072 1700 0000  plot).r$...r....
-00001410: 7217 0000 0072 1800 0000 7229 0000 0099  r....r....r)....
-00001420: 0000 0073 0600 0000 0a02 0c02 1804 7229  ...s..........r)
-00001430: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001440: 0300 0000 0400 0000 4300 0000 7232 0000  ........C...r2..
-00001450: 0029 047a 630a 2020 2020 3a70 6172 616d  .).zc.    :param
-00001460: 2066 6f6f 7465 723a 206c 6973 7420 7769   footer: list wi
-00001470: 7468 2074 6578 7420 746f 2073 686f 7720  th text to show 
-00001480: 696e 2066 6f6f 7465 720a 2020 2020 3a72  in footer.    :r
-00001490: 6574 7572 6e3a 2073 7472 696e 6720 6874  eturn: string ht
-000014a0: 6d6c 2066 6f72 6d61 7474 6564 2066 6f6f  ml formatted foo
-000014b0: 7465 720a 2020 2020 7a6e 3c64 6976 2073  ter.    zn<div s
-000014c0: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
-000014d0: 2d63 6f6c 6f72 3a20 2346 4646 4646 463b  -color: #FFFFFF;
-000014e0: 206c 696e 652d 6865 6967 6874 3a20 312e   line-height: 1.
-000014f0: 363b 2070 6164 6469 6e67 3a31 3070 783b  6; padding:10px;
-00001500: 223e 3c48 5220 7374 796c 653d 2277 6964  "><HR style="wid
-00001510: 7468 3a32 3025 3b20 6d61 7267 696e 2d6c  th:20%; margin-l
-00001520: 6566 743a 303b 223e 7233 0000 0072 3000  eft:0;">r3...r0.
-00001530: 0000 7217 0000 0029 0372 0700 0000 7212  ..r....).r....r.
-00001540: 0000 0072 3400 0000 7217 0000 0072 1700  ...r4...r....r..
-00001550: 0000 7218 0000 0072 1100 0000 a400 0000  ..r....r........
-00001560: 7235 0000 0072 1100 0000 6300 0000 0000  r5...r....c.....
-00001570: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
-00001580: 0000 0073 0400 0000 6401 5300 2902 4e61  ...s....d.S.).Na
-00001590: 5b02 0000 0a20 2020 2020 2020 203c 7374  [....        <st
-000015a0: 796c 653e 0a20 2020 2020 2020 202e 6261  yle>.        .ba
-000015b0: 6467 6520 7b0a 2020 2020 2020 2020 2020  dge {.          
-000015c0: 2020 7769 6474 683a 2032 3130 7078 3b0a    width: 210px;.
-000015d0: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-000015e0: 6874 3a20 3133 3070 783b 0a20 2020 2020  ht: 130px;.     
-000015f0: 2020 2020 2020 206d 6172 6769 6e3a 2034         margin: 4
-00001600: 3270 7820 6175 746f 3b0a 2020 2020 2020  2px auto;.      
-00001610: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-00001620: 3a20 6c69 6e65 6172 2d67 7261 6469 656e  : linear-gradien
-00001630: 7428 746f 2062 6f74 746f 6d20 7269 6768  t(to bottom righ
-00001640: 742c 2077 6869 7465 2c20 2330 3036 6666  t, white, #006ff
-00001650: 6629 3b0a 2020 2020 2020 2020 2020 2020  f);.            
-00001660: 626f 7264 6572 3a20 3370 7820 736f 6c69  border: 3px soli
-00001670: 6420 2338 6361 3566 663b 0a20 2020 2020  d #8ca5ff;.     
-00001680: 2020 2020 2020 2062 6f72 6465 722d 7261         border-ra
-00001690: 6469 7573 3a20 3130 7078 3b0a 2020 2020  dius: 10px;.    
-000016a0: 2020 2020 2020 2020 626f 782d 7368 6164          box-shad
-000016b0: 6f77 3a20 3270 7820 3270 7820 3570 7820  ow: 2px 2px 5px 
-000016c0: 7267 6228 3020 3020 3020 2f20 3330 2529  rgb(0 0 0 / 30%)
-000016d0: 3b0a 2020 2020 2020 2020 2020 2020 6469  ;.            di
-000016e0: 7370 6c61 793a 2066 6c65 783b 0a20 2020  splay: flex;.   
-000016f0: 2020 2020 2020 2020 206a 7573 7469 6679           justify
-00001700: 2d63 6f6e 7465 6e74 3a20 6365 6e74 6572  -content: center
-00001710: 3b0a 2020 2020 2020 2020 2020 2020 616c  ;.            al
-00001720: 6967 6e2d 6974 656d 733a 2063 656e 7465  ign-items: cente
-00001730: 723b 0a20 2020 2020 2020 2020 2020 2066  r;.            f
-00001740: 6f6e 742d 7765 6967 6874 3a20 626f 6c64  ont-weight: bold
-00001750: 3b0a 2020 2020 2020 2020 2020 2020 666f  ;.            fo
-00001760: 6e74 2d73 697a 653a 2036 303b 0a20 2020  nt-size: 60;.   
-00001770: 2020 2020 2020 2020 2063 6f6c 6f72 3a20           color: 
-00001780: 2365 6465 6465 643b 0a20 2020 2020 2020  #ededed;.       
-00001790: 207d 0a20 2020 2020 2020 203c 2f73 7479   }.        </sty
-000017a0: 6c65 3e0a 2020 2020 2020 2020 3c64 6976  le>.        <div
-000017b0: 2063 6c61 7373 3d22 6261 6467 6522 3e0a   class="badge">.
-000017c0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-000017d0: 6e3e 5753 3c2f 7370 616e 3e0a 2020 2020  n>WS</span>.    
-000017e0: 2020 2020 3c2f 6469 763e 0a20 2020 2072      </div>.    r
-000017f0: 1700 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-00001800: 0000 0072 1800 0000 7209 0000 00af 0000  ...r....r.......
-00001810: 0073 0200 0000 0401 7209 0000 0029 0346  .s......r....).F
-00001820: 4646 2905 7220 0000 0072 2000 0000 7220  FF).r ...r ...r 
-00001830: 0000 0054 5429 0d72 0e00 0000 720d 0000  ...TT).r....r...
-00001840: 005a 0e70 6c6f 746c 792e 6f66 666c 696e  .Z.plotly.offlin
-00001850: 655a 076f 6666 6c69 6e65 723b 0000 0072  eZ.offliner;...r
-00001860: 1900 0000 722d 0000 0072 2500 0000 7227  ....r-...r%...r'
-00001870: 0000 0072 2800 0000 7229 0000 0072 1100  ...r(...r)...r..
-00001880: 0000 7209 0000 0072 1700 0000 7217 0000  ..r....r....r...
-00001890: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
-000018a0: 6475 6c65 3e01 0000 0073 1800 0000 0800  dule>....s......
-000018b0: 0c01 0803 0240 0201 0aff 0823 0a1b 080b  .....@.....#....
-000018c0: 080b 080b 0c0b                           ......
+00000040: 0100 6402 6403 8400 5a05 0904 0904 0904  ..d.d...Z.......
+00000050: 0901 6415 6405 6406 8401 5a06 6407 6408  ..d.d.d...Z.d.d.
+00000060: 8400 5a07 6409 6409 6409 6409 640a 640a  ..Z.d.d.d.d.d.d.
+00000070: 6508 8300 6607 640b 640c 8401 5a09 640d  e...f.d.d...Z.d.
+00000080: 640e 8400 5a0a 640f 6410 8400 5a0b 6411  d...Z.d.d...Z.d.
+00000090: 6412 8400 5a0c 6413 6414 8400 5a0d 6401  d...Z.d.d...Z.d.
+000000a0: 5300 2916 e900 0000 004e 6302 0000 0000  S.)......Nc.....
+000000b0: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
+000000c0: 0000 0073 ec00 0000 6401 7c01 7600 7215  ...s....d.|.v.r.
+000000d0: 7400 7c01 6401 1900 8301 6402 6b04 7215  t.|.d.....d.k.r.
+000000e0: 6403 7c01 6401 1900 1700 6404 1700 7d02  d.|.d.....d...}.
+000000f0: 6e03 7401 8300 7d02 6405 7d03 7c03 a002  n.t...}.d.}.|...
+00000100: 6406 7c02 a102 7d03 7c03 a002 6407 7c01  d.|...}.|...d.|.
+00000110: 6408 1900 a102 7d03 6409 7d04 7c01 640a  d.....}.d.}.|.d.
+00000120: 1900 a003 a100 4400 5d0f 5c02 7d05 7d06  ......D.].\.}.}.
+00000130: 7c04 640b 7c05 9b00 640c 7c06 9b00 640d  |.d.|...d.|...d.
+00000140: 9d05 3700 7d04 7130 7c04 640e 3700 7d04  ..7.}.q0|.d.7.}.
+00000150: 7c03 a002 640f 7c04 a102 7d03 7c00 a002  |...d.|...}.|...
+00000160: 6410 7c03 6410 1700 a102 7d00 6411 7c01  d.|.d.....}.d.|.
+00000170: 7600 7274 7c01 6411 1900 7d07 7c07 a004  v.rt|.d...}.|...
+00000180: 7405 6a06 a007 a100 a008 6412 a101 9b00  t.j.......d.....
+00000190: a101 0100 7409 7c01 6411 1900 8301 7d08  ....t.|.d.....}.
+000001a0: 7c00 a002 6410 7c08 6410 1700 a102 7d00  |...d.|.d.....}.
+000001b0: 7c00 5300 2913 4eda 0769 6d67 5f75 726c  |.S.).N..img_url
+000001c0: 7201 0000 007a 0a3c 696d 6720 7372 633d  r....z.<img src=
+000001d0: 277a 2327 2073 7479 6c65 3d27 7769 6474  'z#' style='widt
+000001e0: 683a 3230 3070 783b 6d61 7267 696e 3a31  h:200px;margin:1
+000001f0: 3070 783b 273e 61dc 0100 003c 7374 796c  0px;'>a....<styl
+00000200: 653e 0a20 2020 202e 636f 6e74 6169 6e65  e>.    .containe
+00000210: 7220 7b70 6f73 6974 696f 6e3a 2072 656c  r {position: rel
+00000220: 6174 6976 653b 2068 6569 6768 743a 2036  ative; height: 6
+00000230: 3030 7078 3b7d 0a20 2020 202e 6365 6e74  00px;}.    .cent
+00000240: 6572 6564 2d65 6c65 6d65 6e74 207b 7465  ered-element {te
+00000250: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
+00000260: 3b20 6d61 7267 696e 3a20 303b 2077 6964  ; margin: 0; wid
+00000270: 7468 3a38 3025 3b20 706f 7369 7469 6f6e  th:80%; position
+00000280: 3a20 6162 736f 6c75 7465 3b20 746f 703a  : absolute; top:
+00000290: 2035 3025 3b20 6c65 6674 3a20 3530 253b   50%; left: 50%;
+000002a0: 202d 6d73 2d74 7261 6e73 666f 726d 3a20   -ms-transform: 
+000002b0: 7472 616e 736c 6174 6528 2d35 3025 2c20  translate(-50%, 
+000002c0: 2d35 3025 293b 2074 7261 6e73 666f 726d  -50%); transform
+000002d0: 3a20 7472 616e 736c 6174 6528 2d35 3025  : translate(-50%
+000002e0: 2c20 2d35 3025 293b 7d0a 2020 2020 3c2f  , -50%);}.    </
+000002f0: 7374 796c 653e 0a20 2020 203c 6469 7620  style>.    <div 
+00000300: 636c 6173 733d 2763 6f6e 7461 696e 6572  class='container
+00000310: 273e 0a20 2020 2020 2020 203c 6469 7620  '>.        <div 
+00000320: 636c 6173 733d 2763 656e 7465 7265 642d  class='centered-
+00000330: 656c 656d 656e 7427 3e0a 2020 2020 2020  element'>.      
+00000340: 2020 2020 2020 5641 525f 494d 4147 455f        VAR_IMAGE_
+00000350: 4854 4d4c 0a20 2020 2020 2020 2020 2020  HTML.           
+00000360: 203c 6831 3e56 4152 5f54 4954 4c45 3c2f   <h1>VAR_TITLE</
+00000370: 6831 3e3c 6272 3e0a 2020 2020 2020 2020  h1><br>.        
+00000380: 2020 2020 3c70 2073 7479 6c65 3d27 6c69      <p style='li
+00000390: 6e65 2d68 6569 6768 743a 2031 2e35 3b27  ne-height: 1.5;'
+000003a0: 3e0a 2020 2020 2020 2020 2020 2020 5641  >.            VA
+000003b0: 525f 5355 4d4d 4152 593c 2f70 3e0a 2020  R_SUMMARY</p>.  
+000003c0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000003d0: 203c 2f64 6976 3eda 0e56 4152 5f49 4d41   </div>..VAR_IMA
+000003e0: 4745 5f48 544d 4c5a 0956 4152 5f54 4954  GE_HTMLZ.VAR_TIT
+000003f0: 4c45 da05 7469 746c 6561 0401 0000 0a20  LE..titlea..... 
+00000400: 2020 2020 2020 203c 7461 626c 6520 7374         <table st
+00000410: 796c 653d 2277 6964 7468 3a20 3130 3025  yle="width: 100%
+00000420: 3b20 7465 7874 2d61 6c69 676e 3a20 6c65  ; text-align: le
+00000430: 6674 3b20 666f 6e74 2d73 697a 653a 2031  ft; font-size: 1
+00000440: 656d 3b20 626f 7264 6572 2d63 6f6c 6c61  em; border-colla
+00000450: 7073 653a 2063 6f6c 6c61 7073 653b 2062  pse: collapse; b
+00000460: 6f72 6465 723a 2030 3b22 3e0a 2020 2020  order: 0;">.    
+00000470: 2020 2020 2020 2020 3c63 6f6c 6772 6f75          <colgrou
+00000480: 703e 0a20 2020 2020 2020 2020 2020 2020  p>.             
+00000490: 2020 203c 636f 6c20 7374 796c 653d 2277     <col style="w
+000004a0: 6964 7468 3a20 3230 253b 223e 0a20 2020  idth: 20%;">.   
+000004b0: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+000004c0: 6c20 7374 796c 653d 2277 6964 7468 3a20  l style="width: 
+000004d0: 3830 253b 223e 0a20 2020 2020 2020 2020  80%;">.         
+000004e0: 2020 203c 2f63 6f6c 6772 6f75 703e 0a20     </colgroup>. 
+000004f0: 2020 2020 2020 2020 2020 203c 7462 6f64             <tbod
+00000500: 793e da07 7375 6d6d 6172 797a a70a 2020  y>..summaryz..  
+00000510: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00000520: 7220 7374 796c 653d 2262 6f72 6465 723a  r style="border:
+00000530: 2030 3b22 3e0a 2020 2020 2020 2020 2020   0;">.          
+00000540: 2020 2020 2020 2020 2020 3c74 6420 7374            <td st
+00000550: 796c 653d 2262 6f72 6465 723a 2030 3b20  yle="border: 0; 
+00000560: 7061 6464 696e 673a 2031 3070 783b 2074  padding: 10px; t
+00000570: 6578 742d 6465 636f 7261 7469 6f6e 3a20  ext-decoration: 
+00000580: 756e 6465 726c 696e 653b 2076 6572 7469  underline; verti
+00000590: 6361 6c2d 616c 6967 6e3a 2074 6f70 3b20  cal-align: top; 
+000005a0: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+000005b0: 743b 223e 7a40 3c2f 7464 3e0a 2020 2020  t;">z@</td>.    
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
+000005e0: 723a 2030 3b20 7061 6464 696e 673a 2031  r: 0; padding: 1
+000005f0: 3070 783b 223e 7a2c 3c2f 7464 3e0a 2020  0px;">z,</td>.  
+00000600: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000610: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
+00000620: 2020 2020 7a4e 0a20 2020 2020 2020 2020      zN.         
+00000630: 2020 2020 2020 203c 212d 2d20 6d6f 7265         <!-- more
+00000640: 2072 6f77 7320 6865 7265 202d 2d3e 0a20   rows here -->. 
+00000650: 2020 2020 2020 2020 2020 203c 2f74 626f             </tbo
+00000660: 6479 3e0a 2020 2020 2020 2020 3c2f 7461  dy>.        </ta
+00000670: 626c 653e 5a0b 5641 525f 5355 4d4d 4152  ble>Z.VAR_SUMMAR
+00000680: 59fa 0d3c 7370 616e 3e3c 2f73 7061 6e3e  Y..<span></span>
+00000690: da06 666f 6f74 6572 7a09 2565 2025 622e  ..footerz.%e %b.
+000006a0: 2025 5929 0ada 036c 656e da0c 7773 5f6c   %Y)...len..ws_l
+000006b0: 6f67 6f5f 6874 6d6c da07 7265 706c 6163  ogo_html..replac
+000006c0: 65da 0569 7465 6d73 da06 6170 7065 6e64  e..items..append
+000006d0: da02 6474 da08 6461 7465 7469 6d65 da03  ..dt..datetime..
+000006e0: 6e6f 77da 0873 7472 6674 696d 65da 0e66  now..strftime..f
+000006f0: 6f6f 7465 725f 746f 5f68 746d 6c29 09da  ooter_to_html)..
+00000700: 0468 746d 6cda 0470 6167 6572 0300 0000  .html..pager....
+00000710: 5a09 7469 746c 6570 6167 655a 0c73 756d  Z.titlepageZ.sum
+00000720: 6d61 7279 5f68 746d 6cda 016b da01 7672  mary_html..k..vr
+00000730: 0700 0000 da0b 666f 6f74 6572 5f68 746d  ......footer_htm
+00000740: 6ca9 0072 1700 0000 fa4f 433a 5c55 7365  l..r.....OC:\Use
+00000750: 7273 5c64 6572 6b2d 6a61 6e2e 776f 6c74  rs\derk-jan.wolt
+00000760: 6a65 725c 5079 6368 6172 6d50 726f 6a65  jer\PycharmProje
+00000770: 6374 735c 7765 6273 6c69 6465 735c 7765  cts\webslides\we
+00000780: 6273 6c69 6465 735c 6d6f 6475 6c65 735c  bslides\modules\
+00000790: 746f 6874 6d6c 2e70 79da 1174 6974 6c65  tohtml.py..title
+000007a0: 7061 6765 5f74 6f5f 6874 6d6c 0500 0000  page_to_html....
+000007b0: 732c 0000 0018 0212 0306 0504 030c 0d10  s,..............
+000007c0: 0104 0314 0804 0102 0204 fe02 030c fd08  ................
+000007d0: 060c 0510 0208 0308 0118 010c 0110 0104  ................
+000007e0: 0272 1900 0000 4663 0800 0000 0000 0000  .r....Fc........
+000007f0: 0000 0000 0d00 0000 0a00 0000 4300 0000  ............C...
+00000800: 732a 0100 007c 0672 2074 007c 0164 0119  s*...|.r t.|.d..
+00000810: 007c 0164 0219 007c 047c 057c 01a0 0164  .|.d...|.|.|...d
+00000820: 0364 00a1 027c 01a0 0164 0464 00a1 0264  .d...|...d.d...d
+00000830: 058d 067d 087c 00a0 0264 067c 0864 0617  ...}.|...d.|.d..
+00000840: 00a1 027d 0064 077c 0176 0072 457c 0164  ...}.d.|.v.rE|.d
+00000850: 0719 0064 086b 0372 4574 037c 0164 0919  ...d.k.rEt.|.d..
+00000860: 007c 0164 0a19 007c 0164 0b19 007c 0164  .|.d...|.d...|.d
+00000870: 0719 007c 027c 037c 0764 0c8d 077d 097c  ...|.|.|.d...}.|
+00000880: 00a0 0264 067c 0964 0617 00a1 027d 0064  ...d.|.d.....}.d
+00000890: 0d7c 0176 0072 637c 0164 0d19 0064 086b  .|.v.rc|.d...d.k
+000008a0: 0372 637c 0164 0d19 0067 006b 0372 6374  .rc|.d...g.k.rct
+000008b0: 047c 0164 0d19 0083 017d 0a7c 00a0 0264  .|.d.....}.|...d
+000008c0: 067c 0a64 0617 00a1 027d 0064 0e7c 0176  .|.d.....}.d.|.v
+000008d0: 0072 7574 057c 0164 0e19 0083 017d 0b7c  .rut.|.d.....}.|
+000008e0: 00a0 0264 067c 0b64 0617 00a1 027d 0064  ...d.|.d.....}.d
+000008f0: 0f7c 0176 0072 937c 0164 0f19 0064 086b  .|.v.r.|.d...d.k
+00000900: 0372 937c 0164 0f19 0067 006b 0372 9374  .r.|.d...g.k.r.t
+00000910: 067c 0164 0f19 0083 017d 0c7c 00a0 0264  .|.d.....}.|...d
+00000920: 067c 0c64 0617 00a1 027d 007c 0053 0029  .|.d.....}.|.S.)
+00000930: 104e da06 7061 6765 6e6f da07 7061 6765  .N..pageno..page
+00000940: 6b65 795a 0b68 6c5f 7072 6576 5f6b 6579  keyZ.hl_prev_key
+00000950: 5a0b 686c 5f6e 6578 745f 6b65 7929 0672  Z.hl_next_key).r
+00000960: 1a00 0000 721b 0000 00da 0f73 686f 775f  ....r......show_
+00000970: 696e 6465 785f 7061 6765 da14 7368 6f77  index_page..show
+00000980: 5f68 6967 686c 6967 6874 735f 7061 6765  _highlights_page
+00000990: da12 7072 6576 5f68 6967 686c 6967 6874  ..prev_highlight
+000009a0: 5f6b 6579 da12 6e65 7874 5f68 6967 686c  _key..next_highl
+000009b0: 6967 6874 5f6b 6579 7206 0000 0072 0400  ight_keyr....r..
+000009c0: 0000 da00 da06 7061 6765 6964 da06 746f  ......pageid..to
+000009d0: 7063 6174 da06 7375 6263 6174 2907 7221  pcat..subcat).r!
+000009e0: 0000 0072 2200 0000 7223 0000 0072 0400  ...r"...r#...r..
+000009f0: 0000 da0b 7368 6f77 5f74 6f70 6361 74da  ....show_topcat.
+00000a00: 0b73 686f 775f 7375 6263 6174 da08 746f  .show_subcat..to
+00000a10: 6f6c 7469 7073 da0a 6869 6768 6c69 6768  oltips..highligh
+00000a20: 7473 da04 626f 6479 7207 0000 0029 07da  ts..bodyr....)..
+00000a30: 1070 6167 656e 6176 695f 746f 5f68 746d  .pagenavi_to_htm
+00000a40: 6cda 0367 6574 720a 0000 00da 0d74 6974  l..getr......tit
+00000a50: 6c65 5f74 6f5f 6874 6d6c da12 6869 6768  le_to_html..high
+00000a60: 6c69 6768 7473 5f74 6f5f 6874 6d6c da0c  lights_to_html..
+00000a70: 626f 6479 5f74 6f5f 6874 6d6c 7211 0000  body_to_htmlr...
+00000a80: 0029 0d72 1200 0000 7213 0000 0072 2400  .).r....r....r$.
+00000a90: 0000 7225 0000 0072 1c00 0000 721d 0000  ..r%...r....r...
+00000aa0: 00da 0973 686f 775f 6e61 7669 7226 0000  ...show_navir&..
+00000ab0: 005a 0870 6167 656e 6176 6972 0400 0000  .Z.pagenavir....
+00000ac0: 5a0f 6869 6768 6c69 6768 7473 5f68 746d  Z.highlights_htm
+00000ad0: 6c5a 0962 6f64 795f 6874 6d6c 7216 0000  lZ.body_htmlr...
+00000ae0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000af0: da0f 636f 6e74 656e 745f 746f 5f68 746d  ..content_to_htm
+00000b00: 6c45 0000 0073 3400 0000 0406 0801 0601  lE...s4.........
+00000b10: 0201 0201 0a01 0a01 06fb 1006 1403 0801  ................
+00000b20: 0c01 0801 0401 06fd 1004 2003 0c01 1001  .......... .....
+00000b30: 0803 0c01 1001 2003 0c01 1001 0402 722f  ...... .......r/
+00000b40: 0000 0063 0600 0000 0000 0000 0000 0000  ...c............
+00000b50: 0b00 0000 0600 0000 4300 0000 736e 0000  ........C...sn..
+00000b60: 007c 0464 016b 0272 0664 016e 0564 027c  .|.d.k.r.d.n.d.|
+00000b70: 049b 0064 039d 037d 067c 0564 016b 0272  ...d...}.|.d.k.r
+00000b80: 1264 016e 0564 047c 059b 0064 059d 037d  .d.n.d.|...d...}
+00000b90: 0764 067c 039b 0064 079d 037c 0114 007d  .d.|...d...|...}
+00000ba0: 087c 069b 0064 087c 079b 0064 099d 047c  .|...d.|...d...|
+00000bb0: 0214 007d 0964 0a7c 099b 007c 089b 0064  ...}.d.|...|...d
+00000bc0: 0b7c 009b 0064 0c9d 067d 0a7c 0a53 0029  .|...d...}.|.S.)
+00000bd0: 0d61 d202 0000 0a20 2020 203a 7061 7261  .a.....    :para
+00000be0: 6d20 7061 6765 6e6f 3a20 696e 7420 7061  m pageno: int pa
+00000bf0: 6765 6e75 6d62 6572 0a20 2020 203a 7061  genumber.    :pa
+00000c00: 7261 6d20 6e61 6d65 3a20 7374 7220 6e61  ram name: str na
+00000c10: 6d65 206f 6620 7468 6520 6874 6d6c 2070  me of the html p
+00000c20: 6167 6520 2869 6420 7573 6564 2074 6f20  age (id used to 
+00000c30: 6e61 7669 6761 7465 2074 6f20 7468 6973  navigate to this
+00000c40: 2070 6167 652c 2069 652e 2066 726f 6d20   page, ie. from 
+00000c50: 696e 6465 7820 7061 6765 290a 2020 2020  index page).    
+00000c60: 3a70 6172 616d 2073 686f 775f 696e 6465  :param show_inde
+00000c70: 785f 7061 6765 3a20 626f 6f6c 2069 6620  x_page: bool if 
+00000c80: 4661 6c73 652c 2072 6566 6572 656e 6365  False, reference
+00000c90: 7320 746f 2069 6e64 6578 2070 6167 6520  s to index page 
+00000ca0: 6172 6520 6f6d 6974 7465 640a 2020 2020  are omitted.    
+00000cb0: 3a70 6172 616d 2073 686f 775f 6869 6768  :param show_high
+00000cc0: 6c69 6768 7473 5f70 6167 653a 2062 6f6f  lights_page: boo
+00000cd0: 6c20 6966 2046 616c 7365 2c20 7265 6665  l if False, refe
+00000ce0: 7265 6e63 6573 2074 6f20 6869 6768 6c69  rences to highli
+00000cf0: 6768 7473 2070 6167 6520 6172 6520 6f6d  ghts page are om
+00000d00: 6974 7465 640a 2020 2020 3a70 6172 616d  itted.    :param
+00000d10: 2070 7265 765f 6869 6768 6c69 6768 745f   prev_highlight_
+00000d20: 6b65 793a 2073 7472 2068 746d 6c20 6964  key: str html id
+00000d30: 206f 6620 7072 6576 696f 7573 2068 6967   of previous hig
+00000d40: 686c 6967 6874 2070 6167 650a 2020 2020  hlight page.    
+00000d50: 3a70 6172 616d 206e 6578 745f 6869 6768  :param next_high
+00000d60: 6c69 6768 745f 6b65 793a 2073 7472 2068  light_key: str h
+00000d70: 746d 6c20 6964 206f 6620 6e65 7874 2068  tml id of next h
+00000d80: 6967 686c 6967 6874 2070 6167 650a 2020  ighlight page.  
+00000d90: 2020 3a72 6574 7572 6e3a 2073 7472 696e    :return: strin
+00000da0: 6720 6874 6d6c 2063 6f64 6520 746f 2070  g html code to p
+00000db0: 6c61 6365 206f 6e20 746f 7020 6f66 2065  lace on top of e
+00000dc0: 6163 6820 7061 6765 2c20 7573 6564 2066  ach page, used f
+00000dd0: 6f72 0a20 2020 2020 2020 202d 206e 6176  or.        - nav
+00000de0: 6967 6174 696f 6e20 746f 206e 6578 742f  igation to next/
+00000df0: 7072 6576 696f 7573 2068 6967 686c 6967  previous highlig
+00000e00: 6874 2070 6167 650a 2020 2020 2020 2020  ht page.        
+00000e10: 2d20 6e61 7669 6761 7469 6f6e 2074 6f20  - navigation to 
+00000e20: 696e 6465 7820 7061 6765 0a20 2020 2020  index page.     
+00000e30: 2020 202d 206e 6176 6967 6174 696f 6e20     - navigation 
+00000e40: 746f 2068 6967 686c 6967 6874 7320 7061  to highlights pa
+00000e50: 6765 0a20 2020 2020 2020 202d 2064 6973  ge.        - dis
+00000e60: 706c 6179 2070 6167 656e 756d 6265 720a  play pagenumber.
+00000e70: 2020 2020 2020 2020 2d20 7061 6765 2069          - page i
+00000e80: 6420 7461 6720 7573 6564 2074 6f20 6e61  d tag used to na
+00000e90: 7669 6761 7465 2074 6f20 7468 6174 2070  vigate to that p
+00000ea0: 6167 650a 2020 2020 7220 0000 007a 253c  age.    r ...z%<
+00000eb0: 6120 7469 746c 653d 2250 7265 7669 6f75  a title="Previou
+00000ec0: 7320 6869 6768 6c69 6768 7422 2068 7265  s highlight" hre
+00000ed0: 663d 2223 7a0d 223e 2623 3936 3634 3b3c  f="#z.">&#9664;<
+00000ee0: 2f61 3e7a 213c 6120 7469 746c 653d 224e  /a>z!<a title="N
+00000ef0: 6578 7420 6869 6768 6c69 6768 7422 2068  ext highlight" h
+00000f00: 7265 663d 2223 7a0d 223e 2623 3936 3538  ref="#z.">&#9658
+00000f10: 3b3c 2f61 3e7a 073c 6120 6964 3d22 7a3e  ;</a>z.<a id="z>
+00000f20: 2220 7469 746c 653d 2254 6162 6c65 206f  " title="Table o
+00000f30: 6620 636f 6e74 656e 7473 2220 6872 6566  f contents" href
+00000f40: 3d22 2369 645f 636f 6e74 656e 7473 223e  ="#id_contents">
+00000f50: 2623 3132 3831 3936 3b3c 2f61 3e20 7a40  &#128196;</a> z@
+00000f60: 203c 6120 7469 746c 653d 2248 6967 686c   <a title="Highl
+00000f70: 6967 6874 7320 7375 6d6d 6172 7922 2068  ights summary" h
+00000f80: 7265 663d 2223 6869 6768 6c69 6768 7473  ref="#highlights
+00000f90: 223e 2623 3132 3831 3631 3b3c 2f61 3e20  ">&#128161;</a> 
+00000fa0: fa01 207a 4b3c 6469 7620 636c 6173 733d  .. zK<div class=
+00000fb0: 2266 6f6f 7465 7222 2073 7479 6c65 3d22  "footer" style="
+00000fc0: 7769 6474 683a 2031 3030 253b 206d 6172  width: 100%; mar
+00000fd0: 6769 6e3a 2030 2061 7574 6f3b 2074 6578  gin: 0 auto; tex
+00000fe0: 742d 616c 6967 6e3a 7269 6768 743b 223e  t-align:right;">
+00000ff0: da01 70fa 063c 2f64 6976 3e72 1700 0000  ..p..</div>r....
+00001000: 290b 721a 0000 0072 1c00 0000 721d 0000  ).r....r....r...
+00001010: 0072 1b00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001020: 5a09 6c69 6e6b 5f70 7265 765a 096c 696e  Z.link_prevZ.lin
+00001030: 6b5f 6e65 7874 5a13 7061 6765 6e61 7669  k_nextZ.pagenavi
+00001040: 5f69 6e64 6578 5f70 6167 655a 1870 6167  _index_pageZ.pag
+00001050: 656e 6176 695f 6869 6768 6c69 6768 7473  enavi_highlights
+00001060: 5f70 6167 655a 0d70 6167 656e 6176 695f  _pageZ.pagenavi_
+00001070: 6874 6d6c 7217 0000 0072 1700 0000 7218  htmlr....r....r.
+00001080: 0000 0072 2900 0000 6e00 0000 730c 0000  ...r)...n...s...
+00001090: 0018 1018 0110 0214 0116 0204 0272 2900  .............r).
+000010a0: 0000 7220 0000 0054 6307 0000 0000 0000  ..r ...Tc.......
+000010b0: 0000 0000 000b 0000 0008 0000 0043 0000  .............C..
+000010c0: 0073 b000 0000 7c00 6401 6b02 7206 7c03  .s....|.d.k.r.|.
+000010d0: 6e01 7c00 7d00 7c06 a000 6402 7401 8300  n.|.}.|...d.t...
+000010e0: a102 7d07 7c06 a000 6403 7401 8300 a102  ..}.|...d.t.....
+000010f0: 7d08 7c07 a000 7c01 7c01 a102 7d09 7c08  }.|...|.|...}.|.
+00001100: a000 7c02 7c02 a102 7d0a 7402 7c01 8301  ..|.|...}.t.|...
+00001110: 6404 6b04 7233 6405 7c09 9b00 6406 7c01  d.k.r3d.|...d.|.
+00001120: a003 a100 9b00 6407 9d05 6e01 6401 7d01  ......d...n.d.}.
+00001130: 7402 7c02 8301 6404 6b04 7244 6408 7c0a  t.|...d.k.rDd.|.
+00001140: 9b00 6406 7c02 9b00 6409 9d05 6e01 6401  ..d.|...d...n.d.
+00001150: 7d02 640a 7c04 7c01 1400 9b00 7c05 7c02  }.d.|.|.....|.|.
+00001160: 1400 9b00 640b 7c00 9b00 6406 7c03 9b00  ....d.|...d.|...
+00001170: 640c 9d08 5300 290d 7a57 0a20 2020 203a  d...S.).zW.    :
+00001180: 7061 7261 6d20 7469 746c 653a 2073 7472  param title: str
+00001190: 2074 6974 6c65 206f 6620 6874 6d6c 2070   title of html p
+000011a0: 6167 650a 2020 2020 3a72 6574 7572 6e3a  age.    :return:
+000011b0: 2073 7472 696e 6720 6874 6d6c 2066 6f72   string html for
+000011c0: 6d61 7474 6564 2074 6974 6c65 0a20 2020  matted title.   
+000011d0: 2072 2000 0000 da07 746f 7063 6174 73da   r .....topcats.
+000011e0: 0773 7562 6361 7473 7201 0000 007a 4b3c  .subcatsr....zK<
+000011f0: 7370 616e 2073 7479 6c65 3d27 636f 6c6f  span style='colo
+00001200: 723a 2077 6869 7465 3b20 6261 636b 6772  r: white; backgr
+00001210: 6f75 6e64 2d63 6f6c 6f72 3a20 2330 3038  ound-color: #008
+00001220: 4143 393b 2070 6164 6469 6e67 3a35 7078  AC9; padding:5px
+00001230: 3b27 2074 6974 6c65 3d27 7a02 273e 7a08  ;' title='z.'>z.
+00001240: 3c2f 7370 616e 3e20 7a2a 3c73 7061 6e20  </span> z*<span 
+00001250: 7374 796c 653d 2766 6f6e 742d 7765 6967  style='font-weig
+00001260: 6874 3a20 6e6f 726d 616c 3b27 2074 6974  ht: normal;' tit
+00001270: 6c65 3d27 7a09 3c2f 7370 616e 3e3a 207a  le='z.</span>: z
+00001280: 2e3c 6833 2063 6c61 7373 3d27 7061 6765  .<h3 class='page
+00001290: 7469 746c 6527 2073 7479 6c65 3d27 6c69  title' style='li
+000012a0: 6e65 2d68 6569 6768 743a 2032 3b27 3e7a  ne-height: 2;'>z
+000012b0: 0d3c 7370 616e 2074 6974 6c65 3d27 7a0c  .<span title='z.
+000012c0: 3c2f 7370 616e 3e3c 2f68 333e 2904 722a  </span></h3>).r*
+000012d0: 0000 00da 0464 6963 7472 0800 0000 da05  .....dictr......
+000012e0: 7570 7065 7229 0b72 2100 0000 7222 0000  upper).r!...r"..
+000012f0: 0072 2300 0000 7204 0000 0072 2400 0000  .r#...r....r$...
+00001300: 7225 0000 0072 2600 0000 5a0f 746f 6f6c  r%...r&...Z.tool
+00001310: 7469 7073 5f74 6f70 6361 745a 0f74 6f6f  tips_topcatZ.too
+00001320: 6c74 6970 735f 7375 6263 6174 5a0e 746f  ltips_subcatZ.to
+00001330: 6f6c 7469 705f 746f 7063 6174 5a0e 746f  oltip_topcatZ.to
+00001340: 6f6c 7469 705f 7375 6263 6174 7217 0000  oltip_subcatr...
+00001350: 0072 1700 0000 7218 0000 0072 2b00 0000  .r....r....r+...
+00001360: 8900 0000 731c 0000 0010 060e 010e 010c  ....s...........
+00001370: 010c 0102 0202 0102 ff02 011a ff02 0102  ................
+00001380: ff22 0224 0172 2b00 0000 6301 0000 0000  .".$.r+...c.....
+00001390: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+000013a0: 0000 00f3 2800 0000 6401 7d01 7c00 4400  ....(...d.}.|.D.
+000013b0: 5d09 7d02 7c01 7c02 9b00 6402 9d02 3700  ].}.|.|...d...7.
+000013c0: 7d01 7104 7c01 6403 3700 7d01 7c01 5300  }.q.|.d.7.}.|.S.
+000013d0: 2904 7a65 0a20 2020 203a 7061 7261 6d20  ).ze.    :param 
+000013e0: 636f 6d6d 656e 7473 3a20 6c69 7374 2077  comments: list w
+000013f0: 6974 6820 7465 7874 2074 6f20 7368 6f77  ith text to show
+00001400: 2069 6e20 6865 6164 6572 0a20 2020 203a   in header.    :
+00001410: 7265 7475 726e 3a20 7374 7269 6e67 2068  return: string h
+00001420: 746d 6c20 666f 726d 6174 7465 6420 6865  tml formatted he
+00001430: 6164 6572 0a20 2020 207a 483c 6469 7620  ader.    zH<div 
+00001440: 7374 796c 653d 2262 6163 6b67 726f 756e  style="backgroun
+00001450: 642d 636f 6c6f 723a 2023 4542 4542 4542  d-color: #EBEBEB
+00001460: 3b20 6c69 6e65 2d68 6569 6768 743a 2031  ; line-height: 1
+00001470: 2e36 3b20 7061 6464 696e 673a 3130 7078  .6; padding:10px
+00001480: 3b22 3efa 043c 6272 3e72 3200 0000 7217  ;">..<br>r2...r.
+00001490: 0000 0029 0372 2700 0000 7212 0000 00da  ...).r'...r.....
+000014a0: 016f 7217 0000 0072 1700 0000 7218 0000  .or....r....r...
+000014b0: 0072 2c00 0000 9b00 0000 f308 0000 0004  .r,.............
+000014c0: 0518 0108 0104 0172 2c00 0000 6301 0000  .......r,...c...
+000014d0: 0000 0000 0000 0000 0001 0000 0006 0000  ................
+000014e0: 0043 0000 0073 2e00 0000 7400 7c00 7401  .C...s....t.|.t.
+000014f0: 8302 720b 6401 7c00 9b00 6402 9d03 5300  ..r.d.|...d...S.
+00001500: 6401 7402 6a03 7c00 6403 6404 6405 8d03  d.t.j.|.d.d.d...
+00001510: 9b00 6402 9d03 5300 2906 4e7a 183c 6469  ..d...S.).Nz.<di
+00001520: 7620 7374 796c 653d 2770 6164 6469 6e67  v style='padding
+00001530: 3a33 2527 3e72 3200 0000 46da 0364 6976  :3%'>r2...F..div
+00001540: 2902 da10 696e 636c 7564 655f 706c 6f74  )...include_plot
+00001550: 6c79 6a73 da0b 6f75 7470 7574 5f74 7970  lyjs..output_typ
+00001560: 6529 04da 0a69 7369 6e73 7461 6e63 65da  e)...isinstance.
+00001570: 0373 7472 da02 706f da04 706c 6f74 2901  .str..po..plot).
+00001580: 7228 0000 0072 1700 0000 7217 0000 0072  r(...r....r....r
+00001590: 1800 0000 722d 0000 00a6 0000 0073 0600  ....r-.......s..
+000015a0: 0000 0a02 0c02 1804 722d 0000 0063 0100  ........r-...c..
+000015b0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+000015c0: 0000 4300 0000 7237 0000 0029 047a 630a  ..C...r7...).zc.
+000015d0: 2020 2020 3a70 6172 616d 2066 6f6f 7465      :param foote
+000015e0: 723a 206c 6973 7420 7769 7468 2074 6578  r: list with tex
+000015f0: 7420 746f 2073 686f 7720 696e 2066 6f6f  t to show in foo
+00001600: 7465 720a 2020 2020 3a72 6574 7572 6e3a  ter.    :return:
+00001610: 2073 7472 696e 6720 6874 6d6c 2066 6f72   string html for
+00001620: 6d61 7474 6564 2066 6f6f 7465 720a 2020  matted footer.  
+00001630: 2020 7a6e 3c64 6976 2073 7479 6c65 3d22    zn<div style="
+00001640: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00001650: 3a20 2346 4646 4646 463b 206c 696e 652d  : #FFFFFF; line-
+00001660: 6865 6967 6874 3a20 312e 363b 2070 6164  height: 1.6; pad
+00001670: 6469 6e67 3a31 3070 783b 223e 3c48 5220  ding:10px;"><HR 
+00001680: 7374 796c 653d 2277 6964 7468 3a32 3025  style="width:20%
+00001690: 3b20 6d61 7267 696e 2d6c 6566 743a 303b  ; margin-left:0;
+000016a0: 223e 7238 0000 0072 3200 0000 7217 0000  ">r8...r2...r...
+000016b0: 0029 0372 0700 0000 7212 0000 0072 3900  .).r....r....r9.
+000016c0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000016d0: 0072 1100 0000 b100 0000 723a 0000 0072  .r........r:...r
+000016e0: 1100 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000016f0: 0000 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00001700: 0000 6401 5300 2902 4e61 5b02 0000 0a20  ..d.S.).Na[.... 
+00001710: 2020 2020 2020 203c 7374 796c 653e 0a20         <style>. 
+00001720: 2020 2020 2020 202e 6261 6467 6520 7b0a         .badge {.
+00001730: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+00001740: 683a 2032 3130 7078 3b0a 2020 2020 2020  h: 210px;.      
+00001750: 2020 2020 2020 6865 6967 6874 3a20 3133        height: 13
+00001760: 3070 783b 0a20 2020 2020 2020 2020 2020  0px;.           
+00001770: 206d 6172 6769 6e3a 2034 3270 7820 6175   margin: 42px au
+00001780: 746f 3b0a 2020 2020 2020 2020 2020 2020  to;.            
+00001790: 6261 636b 6772 6f75 6e64 3a20 6c69 6e65  background: line
+000017a0: 6172 2d67 7261 6469 656e 7428 746f 2062  ar-gradient(to b
+000017b0: 6f74 746f 6d20 7269 6768 742c 2077 6869  ottom right, whi
+000017c0: 7465 2c20 2330 3036 6666 6629 3b0a 2020  te, #006fff);.  
+000017d0: 2020 2020 2020 2020 2020 626f 7264 6572            border
+000017e0: 3a20 3370 7820 736f 6c69 6420 2338 6361  : 3px solid #8ca
+000017f0: 3566 663b 0a20 2020 2020 2020 2020 2020  5ff;.           
+00001800: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+00001810: 3130 7078 3b0a 2020 2020 2020 2020 2020  10px;.          
+00001820: 2020 626f 782d 7368 6164 6f77 3a20 3270    box-shadow: 2p
+00001830: 7820 3270 7820 3570 7820 7267 6228 3020  x 2px 5px rgb(0 
+00001840: 3020 3020 2f20 3330 2529 3b0a 2020 2020  0 0 / 30%);.    
+00001850: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
+00001860: 2066 6c65 783b 0a20 2020 2020 2020 2020   flex;.         
+00001870: 2020 206a 7573 7469 6679 2d63 6f6e 7465     justify-conte
+00001880: 6e74 3a20 6365 6e74 6572 3b0a 2020 2020  nt: center;.    
+00001890: 2020 2020 2020 2020 616c 6967 6e2d 6974          align-it
+000018a0: 656d 733a 2063 656e 7465 723b 0a20 2020  ems: center;.   
+000018b0: 2020 2020 2020 2020 2066 6f6e 742d 7765           font-we
+000018c0: 6967 6874 3a20 626f 6c64 3b0a 2020 2020  ight: bold;.    
+000018d0: 2020 2020 2020 2020 666f 6e74 2d73 697a          font-siz
+000018e0: 653a 2036 303b 0a20 2020 2020 2020 2020  e: 60;.         
+000018f0: 2020 2063 6f6c 6f72 3a20 2365 6465 6465     color: #edede
+00001900: 643b 0a20 2020 2020 2020 207d 0a20 2020  d;.        }.   
+00001910: 2020 2020 203c 2f73 7479 6c65 3e0a 2020       </style>.  
+00001920: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001930: 3d22 6261 6467 6522 3e0a 2020 2020 2020  ="badge">.      
+00001940: 2020 2020 2020 3c73 7061 6e3e 5753 3c2f        <span>WS</
+00001950: 7370 616e 3e0a 2020 2020 2020 2020 3c2f  span>.        </
+00001960: 6469 763e 0a20 2020 2072 1700 0000 7217  div>.    r....r.
+00001970: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00001980: 0000 7209 0000 00bc 0000 0073 0200 0000  ..r........s....
+00001990: 0401 7209 0000 0029 0446 4646 4e29 0e72  ..r....).FFFN).r
+000019a0: 0e00 0000 720d 0000 005a 0e70 6c6f 746c  ....r....Z.plotl
+000019b0: 792e 6f66 666c 696e 655a 076f 6666 6c69  y.offlineZ.offli
+000019c0: 6e65 7240 0000 0072 1900 0000 722f 0000  ner@...r....r/..
+000019d0: 0072 2900 0000 7235 0000 0072 2b00 0000  .r)...r5...r+...
+000019e0: 722c 0000 0072 2d00 0000 7211 0000 0072  r,...r-...r....r
+000019f0: 0900 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
+00001a00: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
+00001a10: 653e 0100 0000 731c 0000 0008 000c 0108  e>....s.........
+00001a20: 0302 4102 0102 0102 010a fc08 291a 1b08  ..A.........)...
+00001a30: 1208 0b08 0b0c 0b                        .......
```

### Comparing `webslides-0.6.0/webslides/modules/df_demo.html` & `webslides-0.6.3/webslides/modules/df_demo.html`

 * *Files identical despite different names*

### Comparing `webslides-0.6.0/webslides/modules/folium_demo.html` & `webslides-0.6.3/webslides/modules/folium_demo.html`

 * *Files identical despite different names*

### Comparing `webslides-0.6.0/webslides/modules/hello_world.py` & `webslides-0.6.3/webslides/modules/hello_world.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 # imports
+import sys
+import os
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 import main as ws
 import plotly.graph_objects as go
 
 # title page
 title_page = {
     'img_url': '',
     'title': 'Title of Title Page',
     'summary': {'Summary item 1': 'item text 1', 'Summary item 2': 'item text 2'},
     'footer': ['- use custom title image via the img_url parameter', '- footer2']
 }
 
+# tooltips (optional!)
+tooltips = {'topcats': {'Topcat A': 'Put your own tooltip text here',
+                        'Topcat B': 'Put your own tooltip text here'},
+            'subcats': {'Subcat X': 'Tooltip text for subcat x here',
+                        'Subcat Y': 'Tooltip text for subcat y yere'}}
 
 # simple plotly fig
 def simple_fig():
     x = list(range(1, 11))
     y1 = [2 * i for i in x]
     y2 = [3 * i for i in x]
     trace1 = go.Scatter(x=x, y=y1, mode='markers+lines', name='Line 1')
@@ -24,50 +32,53 @@
     fig.update_layout(title='Simple Plotly Line Figure with Two Lines')
     return fig
 
 
 # content pages
 content = {
     'Topcat A': {
-        'Subcat X': [
-            {
+        'Subcat X': {
+            'page1': {
                 'title': 'Page Title 1 - HTML body',
                 'highlights': ['- highlight 1', '- highlight 2'],
                 'body': 'Content 1: this is a <b>HTML string</b>',
                 'footer': ['- footer 1a', '- <i>italic footer 1b</i>'],
                 'show': True},
-            {
+            'page2': {
                 'title': 'Page Title 2 - No highlights',
                 'body': 'Content 2: this is a <b>HTML string</b>',
                 'footer': ['- Note: No highlights, so no lightbulb in the index page', '- <i>italic footer 2b</i>'],
                 'show': True}
-        ],
-        'Subcat Y': [
-            {
+        },
+        'Subcat Y': {
+            'page3': {
                 'title': 'Page Title 3 - Plotly fig !',
                 'highlights': ['- highlight 3', '- note: no footer on this page'],
                 'body': simple_fig(),
                 'show': True}
-        ]
+        }
     },
     'Topcat B': {
-        'Subcat Z': [
-            {
-                'title': 'Page Title 4 - Different topcat',
-                'highlights': ['- highlight 5', '- highlight 6'],
-                'body': 'Content 3',
-                'footer': ['- footer 4a', '- footer 4b'],
-                'show': True}
-        ]
+        'Subcat Z': {
+            'page4':
+                {
+                    'title': 'Page Title 4 - Different topcat',
+                    'highlights': ['- highlight 5', '- highlight 6'],
+                    'body': 'Content 3',
+                    'footer': ['- footer 4a', '- footer 4b'],
+                    'show': True
+                }
+        }
     }
 }
 
 # MAIN
 ws.create(content=content
           , title_page=title_page
           , fname='webslides_hello_world.html'
           , open_in_browser=True
           , show_index_page=True
           , show_topcat=True
           , show_subcat=True
           , show_highlights_page=True
-          , show_highlights_only=False)
+          , show_highlights_only=False
+          , tooltips=tooltips)
```

### Comparing `webslides-0.6.0/webslides/modules/input_validations.py` & `webslides-0.6.3/webslides/modules/input_validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,28 @@
         if not isinstance(subcats, dict):
             return f"Error: '{topcat}' value is not a dictionary. Content: {str(subcats)[:13]}...{str(subcats)[-14:]}"
 
         if len(subcats) < 1:
             return f"Error: '{topcat}' subdictionary must have at least 1 key-value pair."
 
         for subcat, items in subcats.items():
-            if not isinstance(items, list):
-                return f"Error: '{subcat}' value is not a list. Content: {str(items)[:13]}...{str(items)[-14:]}"
 
-            if len(items) < 1:
-                return f"Error: '{subcat}' list must have at least 1 element."
+            if not isinstance(items, dict):
+                return f"Error: '{subcat}' value is not a dict. Content: {str(items)[:13]}...{str(items)[-14:]}"
 
-            for item in items:
-                if not isinstance(item, dict):
-                    return f"Error: List element is not a dictionary. Content: {str(item)[:13]}...{str(item)[-14:]}"
+            if len(items) == 0:
+                return f"Error: '{subcat}' dict must have at least 1 element."
 
-                for key, value in item.items():
+            for ik, iv in items.items():
+
+                if not isinstance(iv, dict):
+                    return f"Error: Page content is not a dictionary. Content: {str(iv)[:13]}...{str(iv)[-14:]}"
+
+                for key, value in iv.items():
+                    
                     if key == 'title' and not isinstance(value, str):
                         return f"Error: 'title' value is not a string. Content: {str(value)[:13]}...{str(value)[-14:]}"
                     elif key in ['highlights', 'footer'] and not (
                             isinstance(value, list) and all(isinstance(v, str) for v in value)):
                         return f"Error: '{key}' value is not a list of strings. Content: {str(value)[:13]}...{str(value)[-14:]}"
                     elif key == 'body' and not (isinstance(value, str) or isinstance(value, go.Figure)):
                         return f"Error: 'body' value is not a string or a Plotly Figure object. Content: {str(value)[:13]}...{str(value)[-14:]}"
```

### Comparing `webslides-0.6.0/webslides/modules/other.py` & `webslides-0.6.3/webslides/modules/other.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     fpath = os.path.join(current_dir)
     with open(f"{fpath}/{fname}", 'r') as f:
         code_lines = f.readlines()
 
     html_lines = [
         '<div style="font-size:1.1em;padding:15px;background-color:#fdffc7; display: inline-block;"><pre><code>']
     for line in code_lines:
+        line = line.replace('import sys', '')
+        line = line.replace('import os', '')
+        line = line.replace("sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))", "")
         line = line.replace('import main as ws', 'import webslides as ws')
         html_line = line.rstrip().replace('<', '&lt;').replace('>', '&gt;')
         html_lines.append(html_line)
     html_lines.append('</code></pre></div>')
 
     # add copy button
     html_lines.append(
```

### Comparing `webslides-0.6.0/webslides/modules/pagination.py` & `webslides-0.6.3/webslides/modules/pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
     """
     :param pagedata: list of dicts with config and contents per page
     :return: df with pagination data, like pagenumber, category, page order
     """
 
     data = list()
     for topcat, subcats in content.items():
-        for subcat, items in subcats.items():
-            for item in items:
-                item_copy = item.copy()
+        for subcat, pages in subcats.items():
+            for kp, vp in pages.items():
+                item_copy = vp.copy()
                 item_copy['topcat'] = topcat
                 item_copy['subcat'] = subcat
+                item_copy['pageid'] = kp
 
                 # Check for the presence of 'footer' and 'highlights' keys
                 if 'footer' not in item_copy:
                     item_copy['footer'] = None
                 if 'highlights' not in item_copy:
                     item_copy['highlights'] = None
```

### Comparing `webslides-0.6.0/webslides/modules/tohtml.py` & `webslides-0.6.3/webslides/modules/tohtml.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,43 +62,49 @@
         footer.append(f"{dt.datetime.now().strftime('%e %b. %Y')}")
         footer_html = footer_to_html(page['footer'])
         html = html.replace('<span></span>', footer_html + '<span></span>')
 
     return html
 
 
-def content_to_html(html, page, show_topcat, show_subcat, show_index_page=False, show_highlights_page=False,
-                    show_navi=False):
+def content_to_html(html, page, show_topcat, show_subcat,
+                    show_index_page=False,
+                    show_highlights_page=False,
+                    show_navi=False,
+                    tooltips=None):
     # A. page navigation
     if show_navi:  # dont show for title page
         pagenavi = pagenavi_to_html(pageno=page['pageno'],
                                     pagekey=page['pagekey'],
                                     show_index_page=show_index_page,
                                     show_highlights_page=show_highlights_page,
                                     prev_highlight_key=page.get('hl_prev_key', None),
                                     next_highlight_key=page.get('hl_next_key', None))
         html = html.replace('<span></span>', pagenavi + '<span></span>')
 
     # B. page title
     if 'title' in page and page['title'] != '':
-        title = title_to_html(page['topcat'], page['subcat'], page['title'], show_topcat, show_subcat)
+        title = title_to_html(pageid=page['pageid'],
+                              topcat=page['topcat'], subcat=page['subcat'],
+                              title=page['title'], show_topcat=show_topcat,
+                              show_subcat=show_subcat, tooltips=tooltips)
         html = html.replace('<span></span>', title + '<span></span>')
 
     # C. highlights
-    if 'highlights' in page and page['highlights'] != '':
+    if 'highlights' in page and page['highlights'] != '' and page['highlights'] != []:
         highlights_html = highlights_to_html(page['highlights'])
         html = html.replace('<span></span>', highlights_html + '<span></span>')
 
     # D. body
     if 'body' in page:
         body_html = body_to_html(page['body'])
         html = html.replace('<span></span>', body_html + '<span></span>')
 
     # E. footer
-    if 'footer' in page and page['footer'] != '':
+    if 'footer' in page and page['footer'] != '' and page['footer'] != []:
         footer_html = footer_to_html(page['footer'])
         html = html.replace('<span></span>', footer_html + '<span></span>')
 
     return html
 
 
 def pagenavi_to_html(pageno, show_index_page, show_highlights_page, pagekey, prev_highlight_key, next_highlight_key):
@@ -124,23 +130,30 @@
     pagenavi_highlights_page = f'{link_prev} <a title="Highlights summary" href="#highlights">&#128161;</a> {link_next} ' * show_highlights_page
 
     pagenavi_html = f'<div class="footer" style="width: 100%; margin: 0 auto; text-align:right;">{pagenavi_highlights_page}{pagenavi_index_page}p{pageno}</div>'
 
     return pagenavi_html
 
 
-def title_to_html(topcat='', subcat='', title='', show_topcat=True, show_subcat=True):
+def title_to_html(pageid='', topcat='', subcat='', title='', show_topcat=True, show_subcat=True, tooltips=dict()):
     """
     :param title: str title of html page
     :return: string html formatted title
     """
-    topcat = f"<span style='color: white; background-color: #008AC9; padding:5px;'>{topcat.upper()}</span> " if len(
+
+    pageid = title if pageid == '' else pageid
+    tooltips_topcat = tooltips.get('topcats', dict())
+    tooltips_subcat = tooltips.get('subcats', dict())
+    tooltip_topcat = tooltips_topcat.get(topcat, topcat)
+    tooltip_subcat = tooltips_subcat.get(subcat, subcat)
+
+    topcat = f"<span style='color: white; background-color: #008AC9; padding:5px;' title='{tooltip_topcat}'>{topcat.upper()}</span> " if len(
         topcat) > 0 else ''
-    subcat = f"<span style='font-weight: normal;'>{subcat}</span>: " if len(subcat) > 0 else ''
-    return f"<h3 style='line-height: 2;'>{show_topcat * topcat}{show_subcat * subcat}{title}</h3>"
+    subcat = f"<span style='font-weight: normal;' title='{tooltip_subcat}'>{subcat}</span>: " if len(subcat) > 0 else ''
+    return f"<h3 class='pagetitle' style='line-height: 2;'>{show_topcat * topcat}{show_subcat * subcat}<span title='{pageid}'>{title}</span></h3>"
 
 
 def highlights_to_html(highlights):
     """
     :param comments: list with text to show in header
     :return: string html formatted header
     """
```

#### html2text {}

```diff
@@ -14,47 +14,53 @@
 {k} {v}
 """ titlepage = titlepage.replace('VAR_SUMMARY', summary_html) html =
 html.replace('', titlepage + '') # footer if 'footer' in page: footer = page
 ['footer'] footer.append(f"{dt.datetime.now().strftime('%e %b. %Y')}")
 footer_html = footer_to_html(page['footer']) html = html.replace('',
 footer_html + '') return html def content_to_html(html, page, show_topcat,
 show_subcat, show_index_page=False, show_highlights_page=False,
-show_navi=False): # A. page navigation if show_navi: # dont show for title page
-pagenavi = pagenavi_to_html(pageno=page['pageno'], pagekey=page['pagekey'],
-show_index_page=show_index_page, show_highlights_page=show_highlights_page,
-prev_highlight_key=page.get('hl_prev_key', None), next_highlight_key=page.get
-('hl_next_key', None)) html = html.replace('', pagenavi + '') # B. page title
-if 'title' in page and page['title'] != '': title = title_to_html(page
-['topcat'], page['subcat'], page['title'], show_topcat, show_subcat) html =
+show_navi=False, tooltips=None): # A. page navigation if show_navi: # dont show
+for title page pagenavi = pagenavi_to_html(pageno=page['pageno'], pagekey=page
+['pagekey'], show_index_page=show_index_page,
+show_highlights_page=show_highlights_page, prev_highlight_key=page.get
+('hl_prev_key', None), next_highlight_key=page.get('hl_next_key', None)) html =
+html.replace('', pagenavi + '') # B. page title if 'title' in page and page
+['title'] != '': title = title_to_html(pageid=page['pageid'], topcat=page
+['topcat'], subcat=page['subcat'], title=page['title'],
+show_topcat=show_topcat, show_subcat=show_subcat, tooltips=tooltips) html =
 html.replace('', title + '') # C. highlights if 'highlights' in page and page
-['highlights'] != '': highlights_html = highlights_to_html(page['highlights'])
-html = html.replace('', highlights_html + '') # D. body if 'body' in page:
-body_html = body_to_html(page['body']) html = html.replace('', body_html + '')
-# E. footer if 'footer' in page and page['footer'] != '': footer_html =
-footer_to_html(page['footer']) html = html.replace('', footer_html + '') return
-html def pagenavi_to_html(pageno, show_index_page, show_highlights_page,
-pagekey, prev_highlight_key, next_highlight_key): """ :param pageno: int
-pagenumber :param name: str name of the html page (id used to navigate to this
-page, ie. from index page) :param show_index_page: bool if False, references to
-index page are omitted :param show_highlights_page: bool if False, references
-to highlights page are omitted :param prev_highlight_key: str html id of
-previous highlight page :param next_highlight_key: str html id of next
-highlight page :return: string html code to place on top of each page, used for
-- navigation to next/previous highlight page - navigation to index page -
-navigation to highlights page - display pagenumber - page id tag used to
-navigate to that page """ link_prev = '' if prev_highlight_key == '' else f'◀'
-link_next = '' if next_highlight_key == '' else f'►' pagenavi_index_page = f'
-' * show_index_page pagenavi_highlights_page = f'{link_prev}  {link_next} ' *
+['highlights'] != '' and page['highlights'] != []: highlights_html =
+highlights_to_html(page['highlights']) html = html.replace('', highlights_html
++ '') # D. body if 'body' in page: body_html = body_to_html(page['body']) html
+= html.replace('', body_html + '') # E. footer if 'footer' in page and page
+['footer'] != '' and page['footer'] != []: footer_html = footer_to_html(page
+['footer']) html = html.replace('', footer_html + '') return html def
+pagenavi_to_html(pageno, show_index_page, show_highlights_page, pagekey,
+prev_highlight_key, next_highlight_key): """ :param pageno: int pagenumber :
+param name: str name of the html page (id used to navigate to this page, ie.
+from index page) :param show_index_page: bool if False, references to index
+page are omitted :param show_highlights_page: bool if False, references to
+highlights page are omitted :param prev_highlight_key: str html id of previous
+highlight page :param next_highlight_key: str html id of next highlight page :
+return: string html code to place on top of each page, used for - navigation to
+next/previous highlight page - navigation to index page - navigation to
+highlights page - display pagenumber - page id tag used to navigate to that
+page """ link_prev = '' if prev_highlight_key == '' else f'◀' link_next = '' if
+next_highlight_key == '' else f'►' pagenavi_index_page = f' ' *
+show_index_page pagenavi_highlights_page = f'{link_prev}  {link_next} ' *
 show_highlights_page pagenavi_html = f'
 {pagenavi_highlights_page}{pagenavi_index_page}p{pageno}
-' return pagenavi_html def title_to_html(topcat='', subcat='', title='',
-show_topcat=True, show_subcat=True): """ :param title: str title of html page :
-return: string html formatted title """ topcat = f"{topcat.upper()} " if len
-( topcat) > 0 else '' subcat = f"{subcat}: " if len(subcat) > 0 else '' return
-f"
+' return pagenavi_html def title_to_html(pageid='', topcat='', subcat='',
+title='', show_topcat=True, show_subcat=True, tooltips=dict()): """ :param
+title: str title of html page :return: string html formatted title """ pageid =
+title if pageid == '' else pageid tooltips_topcat = tooltips.get('topcats',
+dict()) tooltips_subcat = tooltips.get('subcats', dict()) tooltip_topcat =
+tooltips_topcat.get(topcat, topcat) tooltip_subcat = tooltips_subcat.get
+(subcat, subcat) topcat = f"{topcat.upper()} " if len( topcat) > 0 else ''
+subcat = f"{subcat}: " if len(subcat) > 0 else '' return f"
 **** {show_topcat * topcat}{show_subcat * subcat}{title} ****
 " def highlights_to_html(highlights): """ :param comments: list with text to
 show in header :return: string html formatted header """ html = '
 ' for o in highlights: html += f"{o}
 " html += "
 " return html def body_to_html(body): # insert html string if isinstance(body,
 str): # add some padding to the body content return f"
```

### Comparing `webslides-0.6.0/webslides.egg-info/PKG-INFO` & `webslides-0.6.3/webslides.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.6.0
+Version: 0.6.3
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## [live demo](https://datadept.nl/webslides/demo.html)
+## [Live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
@@ -32,15 +32,16 @@
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
 - No WYSIWYG editing in a graphical user interface
-- No easy conversion to PDF
+- No easy conversion to PDF / printable
+- No custom styling (ie. company style)
 
 ## Main Features
 
 Here are some of the things that Webslides does well:
 
 - Generate an index page based on your content
 - Generate a highlights page, based on your content
@@ -51,15 +52,15 @@
 
 Webslides has two dependencies:
 
 - Pandas: a Python package that provides fast, flexible, and expressive data structures for data analysis
 - Plotly: an interactive data visualization library that allows you to create a wide range of charts, graphs, and other visualizations
 
 Webslides uses Pandas to process the content that is included in your presentation.
-The Plotly package is used to convert Plotly figure opjects to HTML.
+The Plotly package is used to convert Plotly figure objects to HTML.
 
 ## Installation
 
 To install Webslides, simply run the following command:
 
 `pip install webslides`
 
@@ -133,23 +134,23 @@
 - **content** (dict, _optional_, default=None): A dictionary containing the content pages organized by top categories and subcategories.
 
 
   Example input:
 ```
 content = {
     'Topcat A': {
-        'Subcat X': [
-            {
+        'Subcat X': {
+            'page1': {
                 'title': 'Page Title 1 - HTML body',
                 'highlights': ['- highlight 1', '- highlight 2'],
                 'body': 'Content 1: this is a <b>HTML string</b>',
                 'footer': ['- footer 1a', '- <i>italic footer 1b</i>'],
                 'show': True},
                 ...
-            ],
+            },
         ...
         },
     ...
 }
 ```
 - **fname** (str, _optional_, default='output.html'): The output filename for the generated HTML file.
 
@@ -161,14 +162,16 @@
 
 - **show_topcat** (bool, _optional_, default=True): If set to True, the top category will be displayed in the index and highlights pages.
 
 - **show_subcat** (bool, _optional_, default=True): If set to True, the subcategory will be displayed in the index and highlights pages.
 
 - **show_highlights_only** (bool, _optional_, default=False): If set to True, only content pages with highlights will be shown in the index and highlights pages.
 
+- **tooltips** (dict, _optional_, default=None): Dictionary with keys 'topcats' and 'subcats' and with topcat/subcat as keys, with each a dict wit keys and values with the respective topcat names and tooltip texts.
+
 ## Page Dictionary Parameters
 
 Each content page dictionary within the content parameter can include the following keys:
 
 - **title** (str, _mandatory_): The title of the content page.
 
 - **body** (str or object, _mandatory_): The body of the content page. It can be a string containing HTML or an object (e.g., a Plotly figure).
```

### Comparing `webslides-0.6.0/webslides.egg-info/SOURCES.txt` & `webslides-0.6.3/webslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

