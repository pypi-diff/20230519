# Comparing `tmp/jupyterlab-skip-traceback-4.0.4.tar.gz` & `tmp/jupyterlab_skip_traceback-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-skip-traceback-4.0.4.tar", last modified: Wed Jun 22 00:05:53 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab-skip-traceback-4.0.4.tar` & `jupyterlab_skip_traceback-5.0.0.tar`

### file list

```diff
@@ -1,47 +1,39 @@
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.692557 jupyterlab-skip-traceback-4.0.4/
--rw-r--r--   0 udoff      (501) staff       (20)     1504 2020-07-28 19:18:25.000000 jupyterlab-skip-traceback-4.0.4/LICENSE.txt
--rw-r--r--   0 udoff      (501) staff       (20)      469 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/MANIFEST.in
--rw-r--r--   0 udoff      (501) staff       (20)     5313 2022-06-22 00:05:53.692401 jupyterlab-skip-traceback-4.0.4/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     4483 2022-06-13 23:05:02.000000 jupyterlab-skip-traceback-4.0.4/README.md
--rw-r--r--   0 udoff      (501) staff       (20)      211 2021-03-17 18:17:59.000000 jupyterlab-skip-traceback-4.0.4/install.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.624306 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/
--rw-r--r--   0 udoff      (501) staff       (20)      296 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/__init__.py
--rw-r--r--   0 udoff      (501) staff       (20)      441 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/_version.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.625711 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/
--rw-r--r--   0 udoff      (501) staff       (20)    21105 2022-06-22 00:04:58.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/build_log.json
--rw-r--r--   0 udoff      (501) staff       (20)     3386 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/package.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.588688 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/schemas/
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.632510 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/schemas/jupyterlab-skip-traceback/
--rw-r--r--   0 udoff      (501) staff       (20)     3235 2022-06-22 00:04:58.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/schemas/jupyterlab-skip-traceback/package.json.orig
--rw-r--r--   0 udoff      (501) staff       (20)      430 2022-06-22 00:04:58.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/schemas/jupyterlab-skip-traceback/settings.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.675729 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/
--rw-r--r--   0 udoff      (501) staff       (20)    21336 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/lib_index_js.52dc7b1350d51c8c507c.js
--rw-r--r--   0 udoff      (501) staff       (20)    16341 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/lib_index_js.52dc7b1350d51c8c507c.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    28745 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/remoteEntry.a56bbc31679d779bf566.js
--rw-r--r--   0 udoff      (501) staff       (20)    27676 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/remoteEntry.a56bbc31679d779bf566.js.map
--rw-r--r--   0 udoff      (501) staff       (20)      168 2022-06-22 00:04:58.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/style.js
--rw-r--r--   0 udoff      (501) staff       (20)     6396 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/style_index_js.52a925870528c63c1b68.js
--rw-r--r--   0 udoff      (501) staff       (20)     4312 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/style_index_js.52a925870528c63c1b68.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    12080 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.150ab0f7f411e12ef10d.js
--rw-r--r--   0 udoff      (501) staff       (20)    13823 2022-06-22 00:05:01.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab-skip-traceback/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.150ab0f7f411e12ef10d.js.map
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.683541 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/
--rw-r--r--   0 udoff      (501) staff       (20)     5313 2022-06-22 00:05:53.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     1770 2022-06-22 00:05:53.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/SOURCES.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2022-06-22 00:05:53.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/dependency_links.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2022-05-26 22:23:50.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/not-zip-safe
--rw-r--r--   0 udoff      (501) staff       (20)       42 2022-06-22 00:05:53.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/requires.txt
--rw-r--r--   0 udoff      (501) staff       (20)       26 2022-06-22 00:05:53.000000 jupyterlab-skip-traceback-4.0.4/jupyterlab_skip_traceback.egg-info/top_level.txt
--rw-r--r--   0 udoff      (501) staff       (20)     3235 2022-06-22 00:03:40.000000 jupyterlab-skip-traceback-4.0.4/package.json
--rw-r--r--   0 udoff      (501) staff       (20)      274 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/pyproject.toml
--rw-r--r--   0 udoff      (501) staff       (20)       38 2022-06-22 00:05:53.692600 jupyterlab-skip-traceback-4.0.4/setup.cfg
--rw-r--r--   0 udoff      (501) staff       (20)     2164 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/setup.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.684117 jupyterlab-skip-traceback-4.0.4/src/
--rw-r--r--   0 udoff      (501) staff       (20)     4418 2022-06-22 00:03:40.000000 jupyterlab-skip-traceback-4.0.4/src/SkipTracebackWidget.ts
--rw-r--r--   0 udoff      (501) staff       (20)     2343 2022-05-26 20:29:31.000000 jupyterlab-skip-traceback-4.0.4/src/index.ts
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2022-06-22 00:05:53.692164 jupyterlab-skip-traceback-4.0.4/style/
--rw-r--r--   0 udoff      (501) staff       (20)      832 2022-05-26 22:23:00.000000 jupyterlab-skip-traceback-4.0.4/style/base.css
--rw-r--r--   0 udoff      (501) staff       (20)       25 2021-03-17 18:17:59.000000 jupyterlab-skip-traceback-4.0.4/style/index.css
--rw-r--r--   0 udoff      (501) staff       (20)       21 2021-03-17 18:17:59.000000 jupyterlab-skip-traceback-4.0.4/style/index.js
--rw-r--r--   0 udoff      (501) staff       (20)      555 2021-03-17 18:17:59.000000 jupyterlab-skip-traceback-4.0.4/tsconfig.json
--rw-r--r--   0 udoff      (501) staff       (20)     3177 2020-07-28 19:18:25.000000 jupyterlab-skip-traceback-4.0.4/tslint.json
--rw-r--r--   0 udoff      (501) staff       (20)   278452 2022-05-26 22:23:00.000000 jupyterlab-skip-traceback-4.0.4/yarn.lock
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.gitattributes
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.prettierignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.travis.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/install.json
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/tsconfig.json
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/tslint.json
+-rw-r--r--   0        0        0   187298 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/yarn.lock
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.husky/pre-commit
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.husky/_/.gitignore
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.husky/_/husky.sh
+-rw-r--r--   0        0        0   107125 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/docs/skip-traceback-older.gif
+-rw-r--r--   0        0        0   103538 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/docs/skip-traceback.gif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/_version.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/package.json
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/schemas/jupyterlab-skip-traceback/package.json.orig
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/schemas/jupyterlab-skip-traceback/settings.json
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/static/197.0596bfdf60c6ce658c25.js
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/static/747.4f80ed8d9fca742cc8a5.js
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/static/remoteEntry.b4861d8944599b59ea1c.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/static/style.js
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/jupyterlab-skip-traceback/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/notebooks/index.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/schema/settings.json
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/src/SkipTracebackWidget.ts
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/src/index.ts
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/style/index.js
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/.gitignore
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/README.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 jupyterlab_skip_traceback-5.0.0/PKG-INFO
```

### Comparing `jupyterlab-skip-traceback-4.0.4/LICENSE.txt` & `jupyterlab_skip_traceback-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-skip-traceback-4.0.4/PKG-INFO` & `jupyterlab_skip_traceback-5.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,21 @@
-Metadata-Version: 2.1
-Name: jupyterlab-skip-traceback
-Version: 4.0.4
-Summary: A JupyterLab extension for rendering Errors with a copy/paste button and expand/collapse
-Home-page: https://github.com/deshaw/jupyterlab-skip-traceback
-Author: Marc Udoff
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # jupyterlab-skip-traceback
 
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url] [![Binder][binder-image]][binder-url]
 
 A JupyterLab extension for rendering Errors with a copy/paste button and expand/collapse.
 
 This is inspired by the notebook version [here](https://github.com/ipython-contrib/jupyter_contrib_nbextensions/tree/master/src/jupyter_contrib_nbextensions/nbextensions/skip-traceback).
 
 ![Screenshot](https://github.com/deshaw/jupyterlab-skip-traceback/blob/master/docs/skip-traceback.gif?raw=true 'Skip Traceback Screenshot')
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0
 
 ## Install
 
 ```bash
 pip install jupyterlab-skip-traceback
 ```
 
@@ -92,31 +69,30 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist tsconfig.tsbuildinfo lib jupyterlab-skip-traceback/labextension
-jlpm build
-python setup.py sdist bdist_wheel
+rm -rf dist tsconfig.tsbuildinfo lib jupyterlab-skip-traceback/labextension jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl
+hatch build .
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:gi
 
 ```
-twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+twine upload --repository-url https://test.pypi.org/legacy/ jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl
 # In a new venv
 pip install --index-url https://test.pypi.org/simple/ jupyterlab_skip_traceback
 ```
 
 5. Upload this to pypi:
 
 ```
-twine upload dist/*
+twine upload jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl
 ```
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab-skip-traceback
 ```
@@ -131,15 +107,15 @@
     </a>
 </p>
 
 ## License
 
 This project is released under a [BSD-3-Clause license](https://github.com/deshaw/jupyterlab-skip-traceback/blob/master/LICENSE.txt).
 
-We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/forms/MzYxRTE4MEMtNDQ4OC00RjI0LTg1QTItMzEwODM1RTYzQzVF).
+We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla).
 This CLA is in place to protect all users of this project.
 
 "Jupyter" is a trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
 
 [pypi-url]: https://pypi.org/project/jupyterlab-skip-traceback
 [pypi-image]: https://img.shields.io/pypi/v/jupyterlab-skip-traceback
 [pypi-dm-image]: https://img.shields.io/pypi/dm/jupyterlab-skip-traceback
```

#### html2text {}

```diff
@@ -1,69 +1,60 @@
-Metadata-Version: 2.1 Name: jupyterlab-skip-traceback Version: 4.0.4 Summary: A
-JupyterLab extension for rendering Errors with a copy/paste button and expand/
-collapse Home-page: https://github.com/deshaw/jupyterlab-skip-traceback Author:
-Marc Udoff License: BSD-3-Clause Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux Platform: Mac OS X Platform: Windows Classifier: License :: OSI
-Approved :: BSD License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Framework :: Jupyter Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # jupyterlab-
-skip-traceback [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-
-image]][pypi-url] [![Github Actions Status][github-status-image]][github-
-status-url] [![Binder][binder-image]][binder-url] A JupyterLab extension for
-rendering Errors with a copy/paste button and expand/collapse. This is inspired
-by the notebook version [here](https://github.com/ipython-contrib/
-jupyter_contrib_nbextensions/tree/master/src/jupyter_contrib_nbextensions/
-nbextensions/skip-traceback). ![Screenshot](https://github.com/deshaw/
-jupyterlab-skip-traceback/blob/master/docs/skip-traceback.gif?raw=true 'Skip
-Traceback Screenshot') ## Requirements - JupyterLab >= 3.0 ## Install ```bash
-pip install jupyterlab-skip-traceback ``` ## Contributing ### Development
-install Note: You will need NodeJS to build the extension package. The `jlpm`
-command is JupyterLab's pinned version of [yarn](https://yarnpkg.com/) that is
-installed with JupyterLab. You may use `yarn` or `npm` in lieu of `jlpm` below.
-```bash # Clone the repo to your local environment # Change directory to the
-jupyterlab-skip-traceback directory # Install package in development mode pip
-install -e . # Link your development version of the extension with JupyterLab
-jupyter-labextension develop . --overwrite # Rebuild extension Typescript
-source after making changes jlpm run build ``` You can watch the source
-directory and run JupyterLab at the same time in different terminals to watch
-for changes in the extension's source and automatically rebuild the extension.
-```bash # Watch the source directory in one terminal, automatically rebuilding
-when needed jlpm run watch # Run JupyterLab in another terminal jupyter lab ```
-With the watch command running, every saved change will immediately be built
-locally and available in your running JupyterLab. Refresh JupyterLab to load
-the change in your browser (you may need to wait several seconds for the
-extension to be rebuilt). By default, the `jlpm run build` command generates
-the source maps for this extension to make it easier to debug using the browser
-dev tools. To also generate source maps for the JupyterLab core extensions, you
-can run the following command: ```bash jupyter lab build --minimize=False ```
-#### Publishing Before starting, you'll need to have run: `pip install twine
-jupyter_packaging` 1. Update the version in `package.json` and update the
-release date in `CHANGELOG.md` 2. Commit the change in step 1, tag it, then
-push it ``` git commit -am  git tag vX.Z.Y git push && git push --tags ``` 3.
-Create the artifacts ``` rm -rf dist tsconfig.tsbuildinfo lib jupyterlab-skip-
-traceback/labextension jlpm build python setup.py sdist bdist_wheel ``` 4. Test
-this against the test pypi. You can then install from here to test as well:gi
-``` twine upload --repository-url https://test.pypi.org/legacy/ dist/* # In a
-new venv pip install --index-url https://test.pypi.org/simple/
-jupyterlab_skip_traceback ``` 5. Upload this to pypi: ``` twine upload dist/
-* ``` ### Uninstall ```bash pip uninstall jupyterlab-skip-traceback ``` ##
-History This plugin was contributed back to the community by the [D. E. Shaw
-group](https://www.deshaw.com/).
+# jupyterlab-skip-traceback [![PyPI version][pypi-image]][pypi-url] [![PyPI DM]
+[pypi-dm-image]][pypi-url] [![Github Actions Status][github-status-image]]
+[github-status-url] [![Binder][binder-image]][binder-url] A JupyterLab
+extension for rendering Errors with a copy/paste button and expand/collapse.
+This is inspired by the notebook version [here](https://github.com/ipython-
+contrib/jupyter_contrib_nbextensions/tree/master/src/
+jupyter_contrib_nbextensions/nbextensions/skip-traceback). ![Screenshot](https:
+//github.com/deshaw/jupyterlab-skip-traceback/blob/master/docs/skip-
+traceback.gif?raw=true 'Skip Traceback Screenshot') ## Requirements -
+JupyterLab >= 4.0 ## Install ```bash pip install jupyterlab-skip-traceback ```
+## Contributing ### Development install Note: You will need NodeJS to build the
+extension package. The `jlpm` command is JupyterLab's pinned version of [yarn]
+(https://yarnpkg.com/) that is installed with JupyterLab. You may use `yarn` or
+`npm` in lieu of `jlpm` below. ```bash # Clone the repo to your local
+environment # Change directory to the jupyterlab-skip-traceback directory #
+Install package in development mode pip install -e . # Link your development
+version of the extension with JupyterLab jupyter-labextension develop . --
+overwrite # Rebuild extension Typescript source after making changes jlpm run
+build ``` You can watch the source directory and run JupyterLab at the same
+time in different terminals to watch for changes in the extension's source and
+automatically rebuild the extension. ```bash # Watch the source directory in
+one terminal, automatically rebuilding when needed jlpm run watch # Run
+JupyterLab in another terminal jupyter lab ``` With the watch command running,
+every saved change will immediately be built locally and available in your
+running JupyterLab. Refresh JupyterLab to load the change in your browser (you
+may need to wait several seconds for the extension to be rebuilt). By default,
+the `jlpm run build` command generates the source maps for this extension to
+make it easier to debug using the browser dev tools. To also generate source
+maps for the JupyterLab core extensions, you can run the following command:
+```bash jupyter lab build --minimize=False ``` #### Publishing Before starting,
+you'll need to have run: `pip install twine jupyter_packaging` 1. Update the
+version in `package.json` and update the release date in `CHANGELOG.md` 2.
+Commit the change in step 1, tag it, then push it ``` git commit -am  git tag
+vX.Z.Y git push && git push --tags ``` 3. Create the artifacts ``` rm -rf dist
+tsconfig.tsbuildinfo lib jupyterlab-skip-traceback/labextension
+jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl hatch build
+. ``` 4. Test this against the test pypi. You can then install from here to
+test as well:gi ``` twine upload --repository-url https://test.pypi.org/legacy/
+jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl # In a new
+venv pip install --index-url https://test.pypi.org/simple/
+jupyterlab_skip_traceback ``` 5. Upload this to pypi: ``` twine upload
+jupyterlab_skip_traceback-*.tar.gz jupyterlab_skip_traceback-*.whl ``` ###
+Uninstall ```bash pip uninstall jupyterlab-skip-traceback ``` ## History This
+plugin was contributed back to the community by the [D. E. Shaw group](https://
+www.deshaw.com/).
                                [D._E._Shaw_Logo]
 ## License This project is released under a [BSD-3-Clause license](https://
 github.com/deshaw/jupyterlab-skip-traceback/blob/master/LICENSE.txt). We love
 contributions! Before you can contribute, please sign and submit this
-[Contributor License Agreement (CLA)](https://www.deshaw.com/forms/
-MzYxRTE4MEMtNDQ4OC00RjI0LTg1QTItMzEwODM1RTYzQzVF). This CLA is in place to
-protect all users of this project. "Jupyter" is a trademark of the NumFOCUS
-foundation, of which Project Jupyter is a part. [pypi-url]: https://pypi.org/
-project/jupyterlab-skip-traceback [pypi-image]: https://img.shields.io/pypi/v/
-jupyterlab-skip-traceback [pypi-dm-image]: https://img.shields.io/pypi/dm/
-jupyterlab-skip-traceback [github-status-image]: https://github.com/deshaw/
-jupyterlab-skip-traceback/workflows/Build/badge.svg [github-status-url]: https:
-//github.com/deshaw/jupyterlab-skip-traceback/actions?query=workflow%3ABuild
-[binder-image]: https://mybinder.org/badge_logo.svg [binder-url]: https://
-mybinder.org/v2/gh/deshaw/jupyterlab-skip-traceback.git/
-master?urlpath=lab%2Ftree%2Fnotebooks%2Findex.ipynb
+[Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla). This CLA
+is in place to protect all users of this project. "Jupyter" is a trademark of
+the NumFOCUS foundation, of which Project Jupyter is a part. [pypi-url]: https:
+//pypi.org/project/jupyterlab-skip-traceback [pypi-image]: https://
+img.shields.io/pypi/v/jupyterlab-skip-traceback [pypi-dm-image]: https://
+img.shields.io/pypi/dm/jupyterlab-skip-traceback [github-status-image]: https:/
+/github.com/deshaw/jupyterlab-skip-traceback/workflows/Build/badge.svg [github-
+status-url]: https://github.com/deshaw/jupyterlab-skip-traceback/
+actions?query=workflow%3ABuild [binder-image]: https://mybinder.org/
+badge_logo.svg [binder-url]: https://mybinder.org/v2/gh/deshaw/jupyterlab-skip-
+traceback.git/master?urlpath=lab%2Ftree%2Fnotebooks%2Findex.ipynb
```

### Comparing `jupyterlab-skip-traceback-4.0.4/src/SkipTracebackWidget.ts` & `jupyterlab_skip_traceback-5.0.0/src/SkipTracebackWidget.ts`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   ename: string; // Exception name, as a string
   evalue: string; // Exception value, as a string
   traceback: string[]; // The traceback will contain a list of frames, represented each as a string.
 }
 
 const setMessageInCollapsedState = (
   shortError: HTMLPreElement,
-  data: IError
+  data: IError,
 ) => {
   const eName = document.createElement('span');
   eName.className = RED_BOLD_TEXT_CLASS;
   eName.textContent = data.ename;
   const eValue = document.createTextNode(`: ${data.evalue}`);
   shortError.innerHTML = '';
   shortError.appendChild(eName);
@@ -50,15 +50,15 @@
     SkipTracebackWidget._defaults = {
       ...SkipTracebackWidget._defaults,
       ...newDefaults,
     };
   }
 
   _toggleTraceback(): void {
-    if (this._toggleBtn && this._tracebackNode) {
+    if (this._toggleBtn && this._tracebackNode && this._shortError && this._data) {
       const isToggled = this._toggleBtn.className === TOGGLE_CLOSED_CLASS;
       if (isToggled) {
         this._toggleBtn.className = TOGGLE_OPENED_CLASS;
         this._shortError.innerHTML = '';
         this.node.appendChild(this._tracebackNode);
       } else {
         this._toggleBtn.className = TOGGLE_CLOSED_CLASS;
```

### Comparing `jupyterlab-skip-traceback-4.0.4/src/index.ts` & `jupyterlab_skip_traceback-5.0.0/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -35,41 +35,41 @@
 const extensionSettings: JupyterFrontEndPlugin<void> = {
   id: `${PLUGIN_NAME}:plugin`,
   autoStart: true,
   requires: [IRenderMimeRegistry, ISettingRegistry],
   activate: function (
     app: JupyterFrontEnd,
     rendermime: IRenderMimeRegistry,
-    settingRegistry: ISettingRegistry
+    settingRegistry: ISettingRegistry,
   ) {
     function updateSettings(settings: ISettingRegistry.ISettings) {
       const enabled = settings.get('enabled').composite;
       if (enabled) {
         // Safe to do multiple times as the code replaces the current one
         rendermime.addFactory(extension.rendererFactory, extension.rank);
       } else {
         // We assume we were the only mime render ever installed and nothing removed us already
-        extension.rendererFactory.mimeTypes.forEach((type) =>
-          rendermime.removeMimeType(type)
+        extension.rendererFactory.mimeTypes.forEach(type =>
+          rendermime.removeMimeType(type),
         );
       }
       const collapsed = settings.get('collapsed').composite;
       SkipTracebackWidget.setDefaults({ collapsed });
     }
 
     settingRegistry.load(`${PLUGIN_NAME}:settings`).then(
       (settings: ISettingRegistry.ISettings) => {
         updateSettings(settings);
         settings.changed.connect(updateSettings);
       },
       (err: Error) => {
         console.error(
-          `Could not load settings, so did not active ${PLUGIN_NAME}: ${err}`
+          `Could not load settings, so did not active ${PLUGIN_NAME}: ${err}`,
         );
-      }
+      },
     );
     // eslint-disable-next-line no-console
     console.log('JupyterLab extension jupyterlab-skip-traceback is activated!');
   },
 };
 
 export default extensionSettings;
```

### Comparing `jupyterlab-skip-traceback-4.0.4/style/base.css` & `jupyterlab_skip_traceback-5.0.0/style/base.css`

 * *Files 16% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 .skip-traceback > .short-error {
   display: inline;
 }
 
 .skip-traceback > .fa-copy {
   border: dotted;
   border-width: 1px;
+  min-height: unset;
+  min-width: unset;
 }
 
 .skip-traceback > .fa-caret-right,
 .skip-traceback > .fa-caret-down {
-  /*To fix shifting of text to the right when toggled*/
+  /* To fix shifting of text to the right when toggled */
   width: 17px;
   height: 17px;
 }
 
 .skip-traceback > .right-align {
   float: right;
 }
```

### Comparing `jupyterlab-skip-traceback-4.0.4/tsconfig.json` & `jupyterlab_skip_traceback-5.0.0/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, 'target': 'ES2018'}"}*

```diff
@@ -12,15 +12,15 @@
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
-        "target": "es2017",
+        "strictNullChecks": true,
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

### Comparing `jupyterlab-skip-traceback-4.0.4/tslint.json` & `jupyterlab_skip_traceback-5.0.0/tslint.json`

 * *Files identical despite different names*

