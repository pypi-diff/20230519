# Comparing `tmp/jupytercards-2.5.1.tar.gz` & `tmp/jupytercards-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.5.1.tar", last modified: Wed May 17 20:46:10 2023, max compression
+gzip compressed data, was "jupytercards-2.5.3.tar", last modified: Fri May 19 14:03:02 2023, max compression
```

## Comparing `jupytercards-2.5.1.tar` & `jupytercards-2.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.1/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.1/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.1/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.1/README.md
--rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.1/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.1/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.1/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.1/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-17 20:45:36.593859 jupytercards-2.5.1/jupytercards/__init__.py
--rw-r--r--   0        0        0     9589 2023-05-12 13:11:52.978482 jupytercards-2.5.1/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.1/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.5.1/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.1/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.3/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.3/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.3/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.3/README.md
+-rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.3/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.3/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.3/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.3/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-19 14:01:51.403060 jupytercards-2.5.3/jupytercards/__init__.py
+-rw-r--r--   0        0        0     9737 2023-05-19 14:00:07.262578 jupytercards-2.5.3/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.3/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.5.3/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.3/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.3/PKG-INFO
```

### Comparing `jupytercards-2.5.1/.gitignore` & `jupytercards-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/LICENSE` & `jupytercards-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/Markdown-flashcards.ipynb` & `jupytercards-2.5.3/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/README.md` & `jupytercards-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/example.ipynb` & `jupytercards-2.5.3/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/extractdefinitions.py` & `jupytercards-2.5.3/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/flashcards.gif` & `jupytercards-2.5.3/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/jupytercards/__init__.py` & `jupytercards-2.5.3/jupytercards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.5.1'
+__version__ = '2.5.3'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.5.1/jupytercards/dynamic.py` & `jupytercards-2.5.3/jupytercards/dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,39 +37,43 @@
     text_colors = None or list of strings specfiying alternate colors.
                   front_colors, back_colors also support 'jupytercon' to use JupyterCon (2023) color theme
 
     John  M. Shea
     2021-2023
     '''
 
+    # Specify default front colors
     front_color_dict=[
         'var(--asparagus)',
         'var(--terra-cotta)',
         'var(--cyan-process)'
     ]
 
+    # Specify default back color
     back_color_dict = [
         'var(--dark-blue-gray)'
         ]
 
+    # Define color schemes for JupyterCon (2023)
     jupytercon_front = [
         'hsla(17.65,100%,50%,1)',
         'rgb(234,196,53)',
         'hsla(200,76.74%,83.14%, 1)'
     ]
 
     jupytercon_back = [
         'hsla(208.78,66.49%,36.27%,1)'
     ]
 
+    # Specify default text color
     text_color_dict = [
         'var(--snow)'
     ]
 
-
+    # Allow user to specify alternate color schemes
     if front_colors:
         if type(front_colors) == list:
             front_color_dict = front_colors
         elif front_colors == 'jupytercon':
             front_color_dict = jupytercon_front
 
     if back_colors:
@@ -79,77 +83,68 @@
             back_color_dict = jupytercon_back
 
     if text_colors:
         if type(text_colors) == list:
             text_color_dict = text_colors
 
 
-
+    # Load external style and JavaScript files
     resource_package = __name__
     package = resource_package.split('.')[0]
 
+    # Loading CSS Styles
     styles = "<style>\n"
     f = importlib.resources.files(package).joinpath('styles.css')
     css = f.read_bytes()
     styles += css.decode("utf-8")
     styles += "\n</style>"
 
-    #script ='<script src="swiped-events.min.js"></script>'
-
+    # Load JavaScript files
     script = ''
     f = importlib.resources.files(package).joinpath('swiped-events.min.js')
     js = f.read_bytes()
     script += js.decode("utf-8")
     f = importlib.resources.files(package).joinpath('flashcards.js')
     js = f.read_bytes()
     script += js.decode("utf-8")
 
-
+    # Generate a unique ID for each card set
     letters = string.ascii_letters
     div_id = ''.join(random.choice(letters) for i in range(12))
     # print(div_id)
 
-    #print(script)
-    script += f'''/* This is to handle asynchrony issues in loading Jupyter notebooks
-           where JupyterCards has been previously run. The Javascript was generally
-           being run before the div was added to the DOM. I tried to do this
-           more elegantly using Mutation Observer, but I didn't get it to work.
-
-           Someone more knowledgeable could make this better ;-) */
 
+    # Define a function to be run periodically until the div is present in the DOM.
+    # Someone more knowledgeable might be able to provide a more elegant solution
+    # using Mutation Observer
+    script += f'''
         function try_create() {{
           if(document.getElementById("{div_id}")) {{
             createCards("{div_id}", "{keyControl}", "{grabFocus}");
           }} else {{
              setTimeout(try_create, 200);
           }}
         }};
     '''
 
 
 
-
-    #print(card["front"], card["back"])
-    # Container
-    #mydiv =  '<div class="flip-container" id="'+ div_id + '"></div>'
+    # This will be the container for the cards
     mydiv =  f'<div class="flip-container" id="{div_id}" tabindex="0" style="outline:none;"></div>'
 
 
 
-    #Spacer
+    #Spacer and Next button elements
     spacer='<div style="height:40px"></div>'
-
-    # Next button will go here
     nextbutton=f"""<div class="next" id="{div_id}-next" onclick="window.checkFlip('{div_id}')"> </div> """
-    
-    #print(nextbutton)
     loadData = '\n'
 
     loadData += f"var cards{div_id}="
 
+    # Handling data based on the type of `ref` (string, URL, or Python list)
     if type(ref) == list:
         #print("List detected. Assuming JSON")
         loadData += json.dumps(ref)
         static = True
         url = ""
     elif type(ref) == str:
         if ref[0] == "[":
@@ -199,15 +194,16 @@
 
     loadData += f"var textColors{div_id}= ["
     for color in text_color_dict[:-1]:
         loadData += f'"{color}", '
     loadData += f'"{text_color_dict[-1]}" ];\n'
 
 
-
+    # Depending on whether the data is static or not, try to create the cards immediately
+    # or after fetching data from URL
     if static:
         loadData += f'''try_create(); '''
 
         print()
     else:
         loadData += f'''
 
@@ -218,26 +214,26 @@
         setTimeout(() => jmscontroller.abort(), 5000);
 
         fetch("{url}", {{signal}})
         .then(response => response.json())
         .then(json => createCards("{div_id}", "{keyControl}", "{grabFocus}"))
         .catch(err => {{
         console.log("Fetch error or timeout");
-        createCards("{div_id}", "{keyControl}", "{grabFocus}");
+        try_create(); 
         }});
         }}
         '''
         #loadData+=url+script_end
 
 
-    #print(loadData)
+    # Display the content in the notebook
     display(HTML(styles))
     display(HTML(spacer+mydiv+spacer+nextbutton+spacer))
     display(Javascript(script+loadData))
-    
+
 
 # Functions to help make flashcard JSON files
 
 def makecard (name, front, back):
   """ Convert captured data for a flashcard into a dictionary
 
   Helper for md2json() function, which converts flashcard entries from
```

### Comparing `jupytercards-2.5.1/jupytercards/flashcards.js` & `jupytercards-2.5.3/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/jupytercards/styles.css` & `jupytercards-2.5.3/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/jupytercards/swiped-events.min.js` & `jupytercards-2.5.3/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.1/PKG-INFO` & `jupytercards-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.5.1
+Version: 2.5.3
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

