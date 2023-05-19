# Comparing `tmp/arxiv-astro-summarizer-1.0.tar.gz` & `tmp/arxiv-astro-summarizer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-astro-summarizer-1.0.tar", last modified: Thu May 18 23:01:54 2023, max compression
+gzip compressed data, was "arxiv-astro-summarizer-1.1.tar", last modified: Fri May 19 19:05:38 2023, max compression
```

## Comparing `arxiv-astro-summarizer-1.0.tar` & `arxiv-astro-summarizer-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.789044 arxiv-astro-summarizer-1.0/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 23:01:54.788773 arxiv-astro-summarizer-1.0/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.786685 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    19473 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/astroph_summarizer.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 23:01:54.788283 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      110 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-18 23:01:54.000000 arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      320 2023-05-18 22:35:31.000000 arxiv-astro-summarizer-1.0/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-18 23:01:54.789130 arxiv-astro-summarizer-1.0/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1087 2023-05-18 22:59:09.000000 arxiv-astro-summarizer-1.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.108250 arxiv-astro-summarizer-1.1/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-19 19:05:38.107942 arxiv-astro-summarizer-1.1/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.103844 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    20092 2023-05-19 18:47:06.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/astroph_summarizer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.107542 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      119 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      337 2023-05-19 17:17:05.000000 arxiv-astro-summarizer-1.1/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-19 19:05:38.108344 arxiv-astro-summarizer-1.1/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1100 2023-05-19 17:17:26.000000 arxiv-astro-summarizer-1.1/setup.py
```

### Comparing `arxiv-astro-summarizer-1.0/LICENSE.txt` & `arxiv-astro-summarizer-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-1.0/PKG-INFO` & `arxiv-astro-summarizer-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 1.0
+Version: 1.1
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-1.0/README.md` & `arxiv-astro-summarizer-1.1/README.md`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-1.0/arxiv_astro_summarizer/astroph_summarizer.py` & `arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/astroph_summarizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,44 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon May 15 20:10:00 2023
 
 @author: daniel
 """
 import re
+import logging
 import requests
+import unicodedata
+import textract
+import datefinder
+from progress import bar
+
 import arxivscraper
 import numpy as np 
 import pandas as pd
 from pathlib import Path
 from PyPDF2 import PdfReader
 from datetime import datetime
-from transformers import pipeline
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
+from transformers import pipeline
+logging.getLogger("transformers").setLevel(logging.ERROR)
 import os; os.environ['TOKENIZERS_PARALLELISM'] = 'false'
+from textract.exceptions import MissingFileError
 
 import nltk
 try:
     nltk.data.find('tokenizers/punkt')
 except LookupError:
     nltk.download('punkt') 
 nltk.download('stopwords'); nltk.download('stopwords'); nltk.download('wordnet')
 from nltk.tokenize import sent_tokenize, word_tokenize
 from nltk.corpus import stopwords
 from nltk.stem import WordNetLemmatizer
 
-import unicodedata
-import textract
-import datefinder
-
 class Scraper:
     """
     Class object to scrape, read, and analyze arXiv papers published on a given date.
 
     Args:
         date (str): The initial date to consider for scraping, in the following format: YYYY-MM-DD, e.g. '2022-05-12'.
         user_input (str, optional): A short excerpt describing the kind of papers the user is interested in. Defaults to None.
@@ -236,18 +240,22 @@
             filename = '-'.join(filename_parts)
             filename = filename.title()
             filename += '.pdf'
 
             return filename
 
         if self.df is None:
-            raise ValueError('Meta-data has not been scraped! Run the scrape_arxiv() class method first. ')
+            raise ValueError('Meta-data has not been scraped, run the scrape_arxiv() class method first!')
            
         if index == 'all':
+
+            progess_bar = bar.FillingSquaresBar('Saving files......', max=len(self.df))
+            
             for i in range(len(self.df)):
+
                 filename = format_filename(self.df.iloc[i].authors[0].split()[-1] + '_' + self.df.iloc[i].created[:4]) # Filename, author_YYYY
 
                 try:
                     response = requests.get(self.return_arxiv_url(self.df.id.iloc[i]))
 
                     with open(self.path + filename, 'wb') as f:
                         f.write(response.content)
@@ -256,34 +264,38 @@
                         #print('File saved in: {}'.format(self.path + filename))
                         self.filenames.append(filename)
                     else:
                         os.remove(self.path + filename)
                         #print(f"{filename[:-4]} outside date range, removing...")
                 except Exception as e:
                     print('An error occurred while downloading the PDF: {}'.format(str(e)))
+
+                progess_bar.next()
+
+            progess_bar.finish()
+
         else:
+
             filename = format_filename(self.df.iloc[index].authors[0].split()[-1] + '_' + self.df.iloc[index].created[:4])  # Filename, author_YYYY
 
             try:
                 response = requests.get(self.return_arxiv_url(self.df.id.iloc[index]))
 
                 with open(self.path + filename, 'wb') as f:
                     f.write(response.content)
 
                 if self.check_pdf_contains_text(self.path + filename, self.format_date()):
                     #print('File saved in: {}'.format(self.path + filename))
                     self.filenames.append(filename)
                 else:
                     os.remove(self.path + filename)
-                    #print('File outside date range, removing...')
+                    #print(f"{filename[:-4]} outside date range, removing...")
             except Exception as e:
                 print('An error occurred while downloading the PDF: {}'.format(str(e)))
 
-        print('Complete!')
-
         return
 
     def extract_abstract_from_pdf(self, filename):
         """
         Extracts the abstract from a PDF file.
 
         Args:
@@ -368,28 +380,34 @@
         """
 
         if len(self.filenames) == 0:
             raise ValueError('The filenames attribute is empty, run the save_paper() class method first!')
         
         summaries, authors, similarity_score = [], [], []
 
+        progess_bar = bar.FillingSquaresBar('Summarizing.......', max=len(self.filenames))
+
         for fname in self.filenames:
-            self.extract_abstract_from_pdf(filename=self.path+fname) #Creates the ``raw_text`` attribute
+            try:
+                self.extract_abstract_from_pdf(filename=self.path+fname) #Creates the ``raw_text`` attribute
+            except MissingFileError: 
+                print(); print(f"WARNING: Could not find file: {self.path+fname}")
+
             if self.raw_text == '':
                 print(f"Could not extract abstract for: {fname}")
                 summaries.append('!!!Could not extract abstract!!!'); authors.append(fname)
                 if self.user_input is not None:
                     similarity_score.append(self.is_related(generated_summary))
                 continue
                 
             self.process_abstract() #Creates the ``text`` attribute
          
             # Generate summary
             summarizer = pipeline('summarization', model='sshleifer/distilbart-cnn-12-6', revision='a4f8f3e')
-
+        
             try:
                 # Tokenize self.text
                 tokenized_text = word_tokenize(self.text)
 
                 # Truncate if necessary
                 if len(tokenized_text) > max_length:
                     tokenized_text = tokenized_text[:max_length]
@@ -408,20 +426,26 @@
                 print(f"Error occurred while summarizing {fname}: {str(e)}")
 
                 if self.user_input is not None:
                     similarity_score.append(self.is_related(generated_summary))
             except Exception as e:
                 print(f"Error occurred while summarizing {fname}: {str(e)}")
 
+            progess_bar.next()
+
+        progess_bar.finish()
+
         if self.user_input is None:
             self.df = pd.DataFrame({'Author': authors, 'Summary': summaries}, columns=['Author', 'Summary'])
         else:
             self.df = pd.DataFrame({'Author': authors, 'Summary': summaries, 'Similarity': similarity_score}, columns=['Author', 'Summary', 'Similarity'])
             self.df = self.df.sort_values(by='Similarity', ascending=False)
 
+        self.df = self.df.reset_index(drop=True)
+
         return 
 
     def is_related(self, summary):
         """
         This function is_related calculates the cosine similarity between a user input and a summary text. 
         It uses the TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer to create TF-IDF matrices for the input and summary. 
         The cosine similarity is then calculated based on these matrices and returned.
@@ -430,15 +454,15 @@
             summary: The summary text.
 
         Returns:
             The cosine similarity score.
         """
 
         if self.user_input is None:
-            raise ValueError('The user_input attribute has not been configured!')
+            raise ValueError('The user_input attribute has not been input!')
 
         # Initialize the TF-IDF vectorizer
         vectorizer = TfidfVectorizer(stop_words='english')
 
         # Create TF-IDF matrices for the user input and summary text
         tfidf_matrix = vectorizer.fit_transform([self.user_input, summary])
 
@@ -452,21 +476,24 @@
         Removes the papers that have similarity scores less than or equal to the specified similarity_threshold.
 
         Args:
             similarity_threshold
         """
 
         if self.df is None:
-            raise ValueError('The df attribute does not yet exist! Run the summarize() class method first!')
+            raise ValueError('The df attribute does not yet exist, run the summarize() class method first!')
 
         indices = np.where(self.df.Similarity <= similarity_threshold)[0]
 
         for index in indices:
-            os.remove(self.path+self.df.Author.iloc[index])
-
+            try:
+                os.remove(self.path+self.df.Author.iloc[index])
+            except FileNotFoundError:
+                pass 
+                
         print(f"Complete! The following directory now contains only relevant papers: {self.path}")
 
         return 
 
 def replace_astronomical_terms(text):
     """
     Replaces astronomical terms and abbreviations with their expanded forms or corresponding concepts.
@@ -500,16 +527,8 @@
     }
 
     for term, replacement in replacements.items():
         text = text.replace(term, replacement)
         text = text.replace(term.upper(), replacement)
         text = text.replace(term.capitalize(), replacement)
 
-    return text
-
-
-#scraper = Scraper('2023-05-12', path='/Users/daniel/Desktop/testst')
-#scraper.scrape_arxiv()
-#scraper.save_paper(index='all')
-
-
-
+    return text
```

### Comparing `arxiv-astro-summarizer-1.0/arxiv_astro_summarizer.egg-info/PKG-INFO` & `arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 1.0
+Version: 1.1
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-1.0/setup.py` & `arxiv-astro-summarizer-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="arxiv-astro-summarizer",
-    version="1.0",
+    version="1.01",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/arxiv-astro-summarizer",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Intended Audience :: Developers',
 		'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 		'Programming Language :: Python :: 3',	   
 ],
     packages=find_packages('.'),
-    install_requires = ['numpy', 'requests', 'arxivscraper', 'pandas', 'PyPDF2', 'transformers', 'scikit-learn', 'nltk', 'textract', 'datefinder', 'tensorflow', 'torch'],
+    install_requires = ['numpy', 'requests', 'arxivscraper', 'pandas', 'PyPDF2', 'transformers', 'scikit-learn', 'nltk', 'textract', 'datefinder', 'tensorflow', 'torch', 'progress'],
     python_requires='>=3.7,<4',
     include_package_data=True,
     test_suite="nose.collector",
 )
```

