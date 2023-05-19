# Comparing `tmp/jupyterlab_pyflyby-4.2.0.tar.gz` & `tmp/jupyterlab_pyflyby-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pyflyby-4.2.0.tar", last modified: Tue Aug  9 06:22:20 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_pyflyby-4.2.0.tar` & `jupyterlab_pyflyby-5.0.0.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.281239 jupyterlab_pyflyby-4.2.0/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1504 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/LICENSE.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      455 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/MANIFEST.in
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     5633 2022-08-09 06:22:20.280842 jupyterlab_pyflyby-4.2.0/PKG-INFO
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3943 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/README.md
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      197 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/install.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.271583 jupyterlab_pyflyby-4.2.0/jupyter-config/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       93 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/jupyter-config/jupyterlab_pyflyby.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.272419 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      788 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/__init__.py
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      441 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/_version.py
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3050 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/handlers.py
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.274367 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3115 2022-08-09 06:17:20.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/package.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.268117 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.268197 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.275122 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     2972 2022-08-09 06:17:19.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      836 2022-08-09 06:17:19.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.278069 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     7411 2022-08-09 06:17:20.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/227.1cad1bc26a111ee76cd4.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     8551 2022-08-09 06:17:20.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/316.4f44e21efbe062818edc.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3424 2022-08-09 06:17:20.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/534.2469f0c98db18f365947.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     7123 2022-08-09 06:17:20.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/remoteEntry.a3db63230ba521cc3ddb.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      169 2022-08-09 06:17:19.000000 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/style.js
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.274122 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     5633 2022-08-09 06:22:20.272820 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/PKG-INFO
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1131 2022-08-09 06:22:20.273107 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/SOURCES.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        1 2022-08-09 06:22:20.273379 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/dependency_links.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        1 2022-08-09 06:22:20.273655 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/not-zip-safe
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       71 2022-08-09 06:22:20.273964 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/requires.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       19 2022-08-09 06:22:20.274184 jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby.egg-info/top_level.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     2972 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/package.json
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      274 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/pyproject.toml
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       38 2022-08-09 06:22:20.281354 jupyterlab_pyflyby-4.2.0/setup.cfg
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     2286 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/setup.py
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.279190 jupyterlab_pyflyby-4.2.0/src/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3650 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/src/cellUtils.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      361 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/src/constants.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1094 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/src/handler.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)    16074 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/src/index.tsx
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:22:20.280230 jupyterlab_pyflyby-4.2.0/style/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        0 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/style/base.css
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       25 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/style/index.css
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       21 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/style/index.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      555 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/tsconfig.json
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)   188705 2022-08-09 06:13:52.000000 jupyterlab_pyflyby-4.2.0/yarn.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.gitattributes
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/install.json
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/tsconfig.json
+-rw-r--r--   0        0        0   209252 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/yarn.lock
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/pre-commit
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/_/.gitignore
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/_/husky.sh
+-rw-r--r--   0        0        0    47943 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/docs/pyflyby.gif
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/nb-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/server-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/_version.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/handlers.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/package.json
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/36.815b80fd2ca5b739309a.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/747.642119a933d152ff1ed4.js
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/remoteEntry.2f3f2d893fd3c5c9aea1.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/style.js
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/schema/plugin.json
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/cellUtils.ts
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/constants.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/handler.ts
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/index.tsx
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/index.js
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.gitignore
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/README.md
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/PKG-INFO
```

### Comparing `jupyterlab_pyflyby-4.2.0/LICENSE.txt` & `jupyterlab_pyflyby-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.2.0/README.md` & `jupyterlab_pyflyby-5.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ![Screenshot](https://github.com/deshaw/jupyterlab-pyflyby/blob/main/docs/pyflyby.gif 'PyFlyBy')
 
 You can decide cell where imports should be added by adding 'pyflyby-cell' cell tag to it.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0
 
 ## Install
 
 ```bash
 pip install jupyterlab_pyflyby
 ```
 
@@ -71,30 +71,29 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist
-python setup.py sdist bdist_wheel
+rm -rf dist tsconfig.tsbuildinfo lib jupyterlab_pyflyby/labextension jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl
+hatch build .
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:
 
 ```
-twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-# In a new venv
+twine upload --repository-url https://test.pypi.org/legacy/ jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl# In a new venv
 pip install --index-url https://test.pypi.org/simple/ jupyterlab_pyflyby
 ```
 
 5. Upload this to pypi:
 
 ```
-twine upload dist/*
+twine upload jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl
 ```
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_pyflyby
 ```
@@ -109,14 +108,17 @@
     </a>
 </p>
 
 ## License
 
 This project is released under a [BSD-3-Clause license](https://github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt).
 
+We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla).
+This CLA is in place to protect all users of this project.
+
 "Jupyter" is a trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
 
 [pypi-url]: https://pypi.org/project/jupyterlab-pyflyby
 [pypi-image]: https://img.shields.io/pypi/v/jupyterlab-pyflyby
 [pypi-dm-image]: https://img.shields.io/pypi/dm/jupyterlab-pyflyby
 [github-status-image]: https://github.com/deshaw/jupyterlab-pyflyby/workflows/Build/badge.svg
 [github-status-url]: https://github.com/deshaw/jupyterlab-pyflyby/actions?query=workflow%3ABuild
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 [github-status-url] A labextension to integrate pyflyby with notebooks
 [Pyflyby](https://github.com/deshaw/pyflyby) helps you get rid of the tedious
 task of recalling and adding import statements. This labextension takes it
 further by adding the import statements automatically in your notebook. For eg.
 executing `np.arange(10)` ![Screenshot](https://github.com/deshaw/jupyterlab-
 pyflyby/blob/main/docs/pyflyby.gif 'PyFlyBy') You can decide cell where imports
 should be added by adding 'pyflyby-cell' cell tag to it. ## Requirements -
-JupyterLab >= 3.0 ## Install ```bash pip install jupyterlab_pyflyby ``` ##
+JupyterLab >= 4.0 ## Install ```bash pip install jupyterlab_pyflyby ``` ##
 Contributing ### Development install Note: You will need NodeJS to build the
 extension package. The `jlpm` command is JupyterLab's pinned version of [yarn]
 (https://yarnpkg.com/) that is installed with JupyterLab. You may use `yarn` or
 `npm` in lieu of `jlpm` below. ```bash # Clone the repo to your local
 environment # Change directory to the jupyterlab_pyflyby directory # Install
 package in development mode pip install -e . # Link your development version of
 the extension with JupyterLab jupyter-labextension develop . --overwrite #
@@ -27,25 +27,30 @@
 build` command generates the source maps for this extension to make it easier
 to debug using the browser dev tools. To also generate source maps for the
 JupyterLab core extensions, you can run the following command: ```bash jupyter
 lab build --minimize=False ``` #### Publishing Before starting, you'll need to
 have run: `pip install twine jupyter_packaging` 1. Update the version in
 `package.json` and update the release date in `CHANGELOG.md` 2. Commit the
 change in step 1, tag it, then push it ``` git commit -am  git tag vX.Z.Y git
-push && git push --tags ``` 3. Create the artifacts ``` rm -rf dist python
-setup.py sdist bdist_wheel ``` 4. Test this against the test pypi. You can then
-install from here to test as well: ``` twine upload --repository-url https://
-test.pypi.org/legacy/ dist/* # In a new venv pip install --index-url https://
+push && git push --tags ``` 3. Create the artifacts ``` rm -rf dist
+tsconfig.tsbuildinfo lib jupyterlab_pyflyby/labextension jupyterlab_pyflyby-
+*.tar.gz jupyterlab_pyflyby-*.whl hatch build . ``` 4. Test this against the
+test pypi. You can then install from here to test as well: ``` twine upload --
+repository-url https://test.pypi.org/legacy/ jupyterlab_pyflyby-*.tar.gz
+jupyterlab_pyflyby-*.whl# In a new venv pip install --index-url https://
 test.pypi.org/simple/ jupyterlab_pyflyby ``` 5. Upload this to pypi: ``` twine
-upload dist/* ``` ### Uninstall ```bash pip uninstall jupyterlab_pyflyby ``` ##
-History This plugin was contributed back to the community by the [D. E. Shaw
-group](https://www.deshaw.com/).
+upload jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl ``` ### Uninstall
+```bash pip uninstall jupyterlab_pyflyby ``` ## History This plugin was
+contributed back to the community by the [D. E. Shaw group](https://
+www.deshaw.com/).
                                [D._E._Shaw_Logo]
 ## License This project is released under a [BSD-3-Clause license](https://
-github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt). "Jupyter" is a
-trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
-[pypi-url]: https://pypi.org/project/jupyterlab-pyflyby [pypi-image]: https://
-img.shields.io/pypi/v/jupyterlab-pyflyby [pypi-dm-image]: https://
-img.shields.io/pypi/dm/jupyterlab-pyflyby [github-status-image]: https://
-github.com/deshaw/jupyterlab-pyflyby/workflows/Build/badge.svg [github-status-
-url]: https://github.com/deshaw/jupyterlab-pyflyby/
-actions?query=workflow%3ABuild
+github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt). We love
+contributions! Before you can contribute, please sign and submit this
+[Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla). This CLA
+is in place to protect all users of this project. "Jupyter" is a trademark of
+the NumFOCUS foundation, of which Project Jupyter is a part. [pypi-url]: https:
+//pypi.org/project/jupyterlab-pyflyby [pypi-image]: https://img.shields.io/
+pypi/v/jupyterlab-pyflyby [pypi-dm-image]: https://img.shields.io/pypi/dm/
+jupyterlab-pyflyby [github-status-image]: https://github.com/deshaw/jupyterlab-
+pyflyby/workflows/Build/badge.svg [github-status-url]: https://github.com/
+deshaw/jupyterlab-pyflyby/actions?query=workflow%3ABuild
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/handlers.py` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from jupyter_server.base.handlers import APIHandler
-from jupyter_server.utils import url_path_join
-import tornado
 import json
-from notebook.base.handlers import IPythonHandler
 import os
 import subprocess
 
+from jupyter_server.base.handlers import APIHandler
+from jupyter_server.utils import url_path_join
+import tornado
+
+
+class Status(APIHandler):
+    """Checks if pyflyby is loaded by default in ipython session
 
-class PyflybyStatus(IPythonHandler):
-    """
-    Checks if pyflyby is loaded by default in ipython session
     Return {"status": "loaded"} if included by default, else {"status": "not-loaded"}
     """
-
+    # Users must be authenticated to make requests to the jupyter server
+    @tornado.web.authenticated
     def get(self):
         from IPython.terminal.ipapp import load_default_config
 
         extensions = load_default_config().InteractiveShellApp.extensions.to_dict()
         if any(["pyflyby" in val for val in extensions.values()]):
             self.finish({"status": "loaded"})
         else:
             self.finish({"status": "not-loaded"})
 
 
-class InstallPyflyby(IPythonHandler):
-    """
-    Adds pyflyby to ipython extensions, to be included default everytime ipython is launched
-    """
+class Install(APIHandler):
+    """Adds pyflyby to ipython extensions.
 
+    Pyflyby will be included by default everytime ipython is launched.
+    """
+    @tornado.web.authenticated
     def post(self):
         try:
             subprocess.run(["py", "pyflyby.install_in_ipython_config_file"])
             self.finish({"result": "Installed pyflyby successfully"})
         except Exception as err:
             self.send_error({"result": "Pyflyby installation failed - {}".format(err)})
 
 
-class DisablePyflybyClient(IPythonHandler):
-    """
-    Disables jupyterlab-pyflyby labextension for user
-    """
-
+class Disable(APIHandler):
+    """Disables jupyterlab-pyflyby labextension for user"""
+    @tornado.web.authenticated
     def post(self):
         try:
             settings_dir = os.environ.get(
                 "JUPYTERLAB_SETTINGS_DIR",
                 os.path.join(os.environ.get("HOME"), ".jupyter/lab/user-settings"),
             )
             pyflyby_settings_file = os.path.join(
@@ -53,15 +53,16 @@
             installDialogDisplayed = (
                 True
                 if self.get_body_argument("installDialogDisplayed") == "true"
                 else False
             )
 
             settings = {"enabled": False}
-            # To remember dialog box to install pyflyby ipython extension was displayed for current user
+            # To remember dialog box to install pyflyby ipython extension was
+            # displayed for current user
             settings["installDialogDisplayed"] = installDialogDisplayed
 
             if os.path.exists(pyflyby_settings_file):
                 with open(pyflyby_settings_file, "r") as f:
                     settings = {**json.load(f), **settings}
 
             with open(pyflyby_settings_file, "w") as f:
@@ -72,16 +73,14 @@
                 {"result": "Could not disable pyflyby extension - {}".format(err)}
             )
 
 
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
-    pyflyby_handlers = [
-        ("/pyflyby/pyflyby-status", PyflybyStatus),
-        ("/pyflyby/install-pyflyby", InstallPyflyby),
-        ("/pyflyby/disable-pyflyby", DisablePyflybyClient),
-    ]
     base_url = web_app.settings["base_url"]
-    pyflyby_handlers = [(url_path_join(base_url, v[0]), v[1]) for v in pyflyby_handlers]
-
-    web_app.add_handlers(host_pattern, pyflyby_handlers)
+    handlers = [
+        (url_path_join(base_url, "pyflyby", "pyflyby-status"), Status),
+        (url_path_join(base_url, "pyflyby", "install-pyflyby"), Install),
+        (url_path_join(base_url, "pyflyby", "disable-pyflyby"), Disable),
+    ]
+    web_app.add_handlers(host_pattern, handlers)
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/package.json` & `jupyterlab_pyflyby-5.0.0/package.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8619285806785808%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,57 +1,59 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.a3db63230ba521cc3ddb.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -65,30 +67,37 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.2.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8688730251230252%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,51 +1,58 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
@@ -60,30 +67,37 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.2.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/227.1cad1bc26a111ee76cd4.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -3,18 +3,18 @@
         227: (e, t, n) => {
             var r = n(155);
             t.formatArgs = function(t) {
                 if (t[0] = (this.useColors ? "%c" : "") + this.namespace + (this.useColors ? " %c" : " ") + t[0] + (this.useColors ? "%c " : " ") + "+" + e.exports.humanize(this.diff), !this.useColors) return;
                 const n = "color: " + this.color;
                 t.splice(1, 0, n, "color: inherit");
                 let r = 0,
-                    s = 0;
+                    o = 0;
                 t[0].replace(/%[a-zA-Z%]/g, (e => {
-                    "%%" !== e && (r++, "%c" === e && (s = r))
-                })), t.splice(s, 0, n)
+                    "%%" !== e && (r++, "%c" === e && (o = r))
+                })), t.splice(o, 0, n)
             }, t.save = function(e) {
                 try {
                     e ? t.storage.setItem("debug", e) : t.storage.removeItem("debug")
                 } catch (e) {}
             }, t.load = function() {
                 let e;
                 try {
@@ -23,130 +23,135 @@
                 return !e && void 0 !== r && "env" in r && (e = r.env.DEBUG), e
             }, t.useColors = function() {
                 return !("undefined" == typeof window || !window.process || "renderer" !== window.process.type && !window.process.__nwjs) || ("undefined" == typeof navigator || !navigator.userAgent || !navigator.userAgent.toLowerCase().match(/(edge|trident)\/(\d+)/)) && ("undefined" != typeof document && document.documentElement && document.documentElement.style && document.documentElement.style.WebkitAppearance || "undefined" != typeof window && window.console && (window.console.firebug || window.console.exception && window.console.table) || "undefined" != typeof navigator && navigator.userAgent && navigator.userAgent.toLowerCase().match(/firefox\/(\d+)/) && parseInt(RegExp.$1, 10) >= 31 || "undefined" != typeof navigator && navigator.userAgent && navigator.userAgent.toLowerCase().match(/applewebkit\/(\d+)/))
             }, t.storage = function() {
                 try {
                     return localStorage
                 } catch (e) {}
-            }(), t.colors = ["#0000CC", "#0000FF", "#0033CC", "#0033FF", "#0066CC", "#0066FF", "#0099CC", "#0099FF", "#00CC00", "#00CC33", "#00CC66", "#00CC99", "#00CCCC", "#00CCFF", "#3300CC", "#3300FF", "#3333CC", "#3333FF", "#3366CC", "#3366FF", "#3399CC", "#3399FF", "#33CC00", "#33CC33", "#33CC66", "#33CC99", "#33CCCC", "#33CCFF", "#6600CC", "#6600FF", "#6633CC", "#6633FF", "#66CC00", "#66CC33", "#9900CC", "#9900FF", "#9933CC", "#9933FF", "#99CC00", "#99CC33", "#CC0000", "#CC0033", "#CC0066", "#CC0099", "#CC00CC", "#CC00FF", "#CC3300", "#CC3333", "#CC3366", "#CC3399", "#CC33CC", "#CC33FF", "#CC6600", "#CC6633", "#CC9900", "#CC9933", "#CCCC00", "#CCCC33", "#FF0000", "#FF0033", "#FF0066", "#FF0099", "#FF00CC", "#FF00FF", "#FF3300", "#FF3333", "#FF3366", "#FF3399", "#FF33CC", "#FF33FF", "#FF6600", "#FF6633", "#FF9900", "#FF9933", "#FFCC00", "#FFCC33"], t.log = console.debug || console.log || (() => {}), e.exports = n(447)(t);
+            }(), t.destroy = (() => {
+                let e = !1;
+                return () => {
+                    e || (e = !0, console.warn("Instance method `debug.destroy()` is deprecated and no longer does anything. It will be removed in the next major version of `debug`."))
+                }
+            })(), t.colors = ["#0000CC", "#0000FF", "#0033CC", "#0033FF", "#0066CC", "#0066FF", "#0099CC", "#0099FF", "#00CC00", "#00CC33", "#00CC66", "#00CC99", "#00CCCC", "#00CCFF", "#3300CC", "#3300FF", "#3333CC", "#3333FF", "#3366CC", "#3366FF", "#3399CC", "#3399FF", "#33CC00", "#33CC33", "#33CC66", "#33CC99", "#33CCCC", "#33CCFF", "#6600CC", "#6600FF", "#6633CC", "#6633FF", "#66CC00", "#66CC33", "#9900CC", "#9900FF", "#9933CC", "#9933FF", "#99CC00", "#99CC33", "#CC0000", "#CC0033", "#CC0066", "#CC0099", "#CC00CC", "#CC00FF", "#CC3300", "#CC3333", "#CC3366", "#CC3399", "#CC33CC", "#CC33FF", "#CC6600", "#CC6633", "#CC9900", "#CC9933", "#CCCC00", "#CCCC33", "#FF0000", "#FF0033", "#FF0066", "#FF0099", "#FF00CC", "#FF00FF", "#FF3300", "#FF3333", "#FF3366", "#FF3399", "#FF33CC", "#FF33FF", "#FF6600", "#FF6633", "#FF9900", "#FF9933", "#FFCC00", "#FFCC33"], t.log = console.debug || console.log || (() => {}), e.exports = n(447)(t);
             const {
-                formatters: s
+                formatters: o
             } = e.exports;
-            s.j = function(e) {
+            o.j = function(e) {
                 try {
                     return JSON.stringify(e)
                 } catch (e) {
                     return "[UnexpectedJSONParseError]: " + e.message
                 }
             }
         },
         447: (e, t, n) => {
             e.exports = function(e) {
                 function t(e) {
-                    let n;
+                    let n, o, s, a = null;
 
-                    function o(...e) {
-                        if (!o.enabled) return;
-                        const r = o,
-                            s = Number(new Date),
-                            a = s - (n || s);
-                        r.diff = a, r.prev = n, r.curr = s, n = s, e[0] = t.coerce(e[0]), "string" != typeof e[0] && e.unshift("%O");
-                        let i = 0;
-                        e[0] = e[0].replace(/%([a-zA-Z%])/g, ((n, s) => {
-                            if ("%%" === n) return n;
-                            i++;
-                            const o = t.formatters[s];
-                            if ("function" == typeof o) {
-                                const t = e[i];
-                                n = o.call(r, t), e.splice(i, 1), i--
+                    function i(...e) {
+                        if (!i.enabled) return;
+                        const r = i,
+                            o = Number(new Date),
+                            s = o - (n || o);
+                        r.diff = s, r.prev = n, r.curr = o, n = o, e[0] = t.coerce(e[0]), "string" != typeof e[0] && e.unshift("%O");
+                        let a = 0;
+                        e[0] = e[0].replace(/%([a-zA-Z%])/g, ((n, o) => {
+                            if ("%%" === n) return "%";
+                            a++;
+                            const s = t.formatters[o];
+                            if ("function" == typeof s) {
+                                const t = e[a];
+                                n = s.call(r, t), e.splice(a, 1), a--
                             }
                             return n
                         })), t.formatArgs.call(r, e), (r.log || t.log).apply(r, e)
                     }
-                    return o.namespace = e, o.enabled = t.enabled(e), o.useColors = t.useColors(), o.color = t.selectColor(e), o.destroy = r, o.extend = s, "function" == typeof t.init && t.init(o), t.instances.push(o), o
-                }
-
-                function r() {
-                    const e = t.instances.indexOf(this);
-                    return -1 !== e && (t.instances.splice(e, 1), !0)
+                    return i.namespace = e, i.useColors = t.useColors(), i.color = t.selectColor(e), i.extend = r, i.destroy = t.destroy, Object.defineProperty(i, "enabled", {
+                        enumerable: !0,
+                        configurable: !1,
+                        get: () => null !== a ? a : (o !== t.namespaces && (o = t.namespaces, s = t.enabled(e)), s),
+                        set: e => {
+                            a = e
+                        }
+                    }), "function" == typeof t.init && t.init(i), i
                 }
 
-                function s(e, n) {
+                function r(e, n) {
                     const r = t(this.namespace + (void 0 === n ? ":" : n) + e);
                     return r.log = this.log, r
                 }
 
                 function o(e) {
                     return e.toString().substring(2, e.toString().length - 2).replace(/\.\*\?$/, "*")
                 }
                 return t.debug = t, t.default = t, t.coerce = function(e) {
                     return e instanceof Error ? e.stack || e.message : e
                 }, t.disable = function() {
                     const e = [...t.names.map(o), ...t.skips.map(o).map((e => "-" + e))].join(",");
                     return t.enable(""), e
                 }, t.enable = function(e) {
                     let n;
-                    t.save(e), t.names = [], t.skips = [];
+                    t.save(e), t.namespaces = e, t.names = [], t.skips = [];
                     const r = ("string" == typeof e ? e : "").split(/[\s,]+/),
-                        s = r.length;
-                    for (n = 0; n < s; n++) r[n] && ("-" === (e = r[n].replace(/\*/g, ".*?"))[0] ? t.skips.push(new RegExp("^" + e.substr(1) + "$")) : t.names.push(new RegExp("^" + e + "$")));
-                    for (n = 0; n < t.instances.length; n++) {
-                        const e = t.instances[n];
-                        e.enabled = t.enabled(e.namespace)
-                    }
+                        o = r.length;
+                    for (n = 0; n < o; n++) r[n] && ("-" === (e = r[n].replace(/\*/g, ".*?"))[0] ? t.skips.push(new RegExp("^" + e.slice(1) + "$")) : t.names.push(new RegExp("^" + e + "$")))
                 }, t.enabled = function(e) {
                     if ("*" === e[e.length - 1]) return !0;
                     let n, r;
                     for (n = 0, r = t.skips.length; n < r; n++)
                         if (t.skips[n].test(e)) return !1;
                     for (n = 0, r = t.names.length; n < r; n++)
                         if (t.names[n].test(e)) return !0;
                     return !1
-                }, t.humanize = n(824), Object.keys(e).forEach((n => {
+                }, t.humanize = n(824), t.destroy = function() {
+                    console.warn("Instance method `debug.destroy()` is deprecated and no longer does anything. It will be removed in the next major version of `debug`.")
+                }, Object.keys(e).forEach((n => {
                     t[n] = e[n]
-                })), t.instances = [], t.names = [], t.skips = [], t.formatters = {}, t.selectColor = function(e) {
+                })), t.names = [], t.skips = [], t.formatters = {}, t.selectColor = function(e) {
                     let n = 0;
                     for (let t = 0; t < e.length; t++) n = (n << 5) - n + e.charCodeAt(t), n |= 0;
                     return t.colors[Math.abs(n) % t.colors.length]
                 }, t.enable(t.load()), t
             }
         },
         824: e => {
             var t = 1e3,
                 n = 60 * t,
                 r = 60 * n,
-                s = 24 * r;
+                o = 24 * r;
 
-            function o(e, t, n, r) {
-                var s = t >= 1.5 * n;
-                return Math.round(e / n) + " " + r + (s ? "s" : "")
+            function s(e, t, n, r) {
+                var o = t >= 1.5 * n;
+                return Math.round(e / n) + " " + r + (o ? "s" : "")
             }
             e.exports = function(e, a) {
                 a = a || {};
                 var i, c, u = typeof e;
                 if ("string" === u && e.length > 0) return function(e) {
                     if (!((e = String(e)).length > 100)) {
-                        var o = /^(-?(?:\d+)?\.?\d+) *(milliseconds?|msecs?|ms|seconds?|secs?|s|minutes?|mins?|m|hours?|hrs?|h|days?|d|weeks?|w|years?|yrs?|y)?$/i.exec(e);
-                        if (o) {
-                            var a = parseFloat(o[1]);
-                            switch ((o[2] || "ms").toLowerCase()) {
+                        var s = /^(-?(?:\d+)?\.?\d+) *(milliseconds?|msecs?|ms|seconds?|secs?|s|minutes?|mins?|m|hours?|hrs?|h|days?|d|weeks?|w|years?|yrs?|y)?$/i.exec(e);
+                        if (s) {
+                            var a = parseFloat(s[1]);
+                            switch ((s[2] || "ms").toLowerCase()) {
                                 case "years":
                                 case "year":
                                 case "yrs":
                                 case "yr":
                                 case "y":
                                     return 315576e5 * a;
                                 case "weeks":
                                 case "week":
                                 case "w":
                                     return 6048e5 * a;
                                 case "days":
                                 case "day":
                                 case "d":
-                                    return a * s;
+                                    return a * o;
                                 case "hours":
                                 case "hour":
                                 case "hrs":
                                 case "hr":
                                 case "h":
                                     return a * r;
                                 case "minutes":
@@ -169,100 +174,100 @@
                                     return a;
                                 default:
                                     return
                             }
                         }
                     }
                 }(e);
-                if ("number" === u && isFinite(e)) return a.long ? (i = e, (c = Math.abs(i)) >= s ? o(i, c, s, "day") : c >= r ? o(i, c, r, "hour") : c >= n ? o(i, c, n, "minute") : c >= t ? o(i, c, t, "second") : i + " ms") : function(e) {
-                    var o = Math.abs(e);
-                    return o >= s ? Math.round(e / s) + "d" : o >= r ? Math.round(e / r) + "h" : o >= n ? Math.round(e / n) + "m" : o >= t ? Math.round(e / t) + "s" : e + "ms"
+                if ("number" === u && isFinite(e)) return a.long ? (i = e, (c = Math.abs(i)) >= o ? s(i, c, o, "day") : c >= r ? s(i, c, r, "hour") : c >= n ? s(i, c, n, "minute") : c >= t ? s(i, c, t, "second") : i + " ms") : function(e) {
+                    var s = Math.abs(e);
+                    return s >= o ? Math.round(e / o) + "d" : s >= r ? Math.round(e / r) + "h" : s >= n ? Math.round(e / n) + "m" : s >= t ? Math.round(e / t) + "s" : e + "ms"
                 }(e);
                 throw new Error("val is not a non-empty string or a valid number. val=" + JSON.stringify(e))
             }
         },
         155: e => {
             var t, n, r = e.exports = {};
 
-            function s() {
+            function o() {
                 throw new Error("setTimeout has not been defined")
             }
 
-            function o() {
+            function s() {
                 throw new Error("clearTimeout has not been defined")
             }
 
             function a(e) {
                 if (t === setTimeout) return setTimeout(e, 0);
-                if ((t === s || !t) && setTimeout) return t = setTimeout, setTimeout(e, 0);
+                if ((t === o || !t) && setTimeout) return t = setTimeout, setTimeout(e, 0);
                 try {
                     return t(e, 0)
                 } catch (n) {
                     try {
                         return t.call(null, e, 0)
                     } catch (n) {
                         return t.call(this, e, 0)
                     }
                 }
             }! function() {
                 try {
-                    t = "function" == typeof setTimeout ? setTimeout : s
+                    t = "function" == typeof setTimeout ? setTimeout : o
                 } catch (e) {
-                    t = s
+                    t = o
                 }
                 try {
-                    n = "function" == typeof clearTimeout ? clearTimeout : o
+                    n = "function" == typeof clearTimeout ? clearTimeout : s
                 } catch (e) {
-                    n = o
+                    n = s
                 }
             }();
             var i, c = [],
                 u = !1,
                 l = -1;
 
             function C() {
-                u && i && (u = !1, i.length ? c = i.concat(c) : l = -1, c.length && f())
+                u && i && (u = !1, i.length ? c = i.concat(c) : l = -1, c.length && d())
             }
 
-            function f() {
+            function d() {
                 if (!u) {
                     var e = a(C);
                     u = !0;
                     for (var t = c.length; t;) {
                         for (i = c, c = []; ++l < t;) i && i[l].run();
                         l = -1, t = c.length
                     }
                     i = null, u = !1,
                         function(e) {
                             if (n === clearTimeout) return clearTimeout(e);
-                            if ((n === o || !n) && clearTimeout) return n = clearTimeout, clearTimeout(e);
+                            if ((n === s || !n) && clearTimeout) return n = clearTimeout, clearTimeout(e);
                             try {
-                                n(e)
+                                return n(e)
                             } catch (t) {
                                 try {
                                     return n.call(null, e)
                                 } catch (t) {
                                     return n.call(this, e)
                                 }
                             }
                         }(e)
                 }
             }
 
-            function d(e, t) {
+            function f(e, t) {
                 this.fun = e, this.array = t
             }
 
             function h() {}
             r.nextTick = function(e) {
                 var t = new Array(arguments.length - 1);
                 if (arguments.length > 1)
                     for (var n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
-                c.push(new d(e, t)), 1 !== c.length || u || a(f)
-            }, d.prototype.run = function() {
+                c.push(new f(e, t)), 1 !== c.length || u || a(d)
+            }, f.prototype.run = function() {
                 this.fun.apply(null, this.array)
             }, r.title = "browser", r.browser = !0, r.env = {}, r.argv = [], r.version = "", r.versions = {}, r.on = h, r.addListener = h, r.once = h, r.off = h, r.removeListener = h, r.removeAllListeners = h, r.emit = h, r.prependListener = h, r.prependOnceListener = h, r.listeners = function(e) {
                 return []
             }, r.binding = function(e) {
                 throw new Error("process.binding is not supported")
             }, r.cwd = function() {
                 return "/"
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/316.4f44e21efbe062818edc.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/36.815b80fd2ca5b739309a.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,323 +1,321 @@
+"use strict";
 (self.webpackChunk_deshaw_jupyterlab_pyflyby = self.webpackChunk_deshaw_jupyterlab_pyflyby || []).push([
-    [316], {
-        316: (t, e, s) => {
-            "use strict";
-            s.r(e), s.d(e, {
-                default: () => P
+    [36], {
+        36: (e, t, s) => {
+            s.r(t), s.d(t, {
+                default: () => v
             });
-            var o = s(918),
-                n = s(433),
-                i = s(118),
-                r = s(345),
-                l = s(840),
-                a = s(305),
-                c = s(271),
+            var o = s(697),
+                n = s(778),
+                i = s(501),
+                r = s(629),
+                a = s(901),
+                l = s(305),
+                c = s(29),
                 h = s.n(c);
-            const u = "pyflyby-cell",
-                d = "# THIS CELL WAS AUTO-GENERATED BY PYFLYBY\n",
-                m = "# END AUTO-GENERATED BLOCK\n",
-                y = "pyflyby.missing_imports",
-                g = "pyflyby.format_imports",
-                _ = "pyflyby.init_comms",
-                p = t => "string" == typeof t ? t.split("\n") : t,
-                f = t => !(t.startsWith("#") || t.startsWith('"""') || "" === t.trim() || t.match(/^\s.*$/)) || t.startsWith("%"),
-                b = t => "" === t.trim() || !t.match(/^\s.*$/);
-            var C = s(398),
-                w = s(238);
-            async function x(t = "", e = {}) {
-                const s = w.ServerConnection.makeSettings(),
-                    o = C.URLExt.join(s.baseUrl, "pyflyby", t);
+            const d = "pyflyby-cell",
+                u = "# END AUTO-GENERATED BLOCK\n",
+                m = "pyflyby.missing_imports",
+                y = "pyflyby.format_imports",
+                g = "pyflyby.init_comms",
+                _ = e => "string" == typeof e ? e.split("\n") : e,
+                p = e => !(e.startsWith("#") || e.startsWith('"""') || "" === e.trim() || e.match(/^\s.*$/)) || e.startsWith("%"),
+                f = e => "" === e.trim() || !e.match(/^\s.*$/);
+            var b = s(406),
+                C = s(67);
+            async function w(e = "", t = {}) {
+                const s = C.ServerConnection.makeSettings(),
+                    o = b.URLExt.join(s.baseUrl, "pyflyby", e);
                 let n;
                 try {
-                    n = await w.ServerConnection.makeRequest(o, e, s)
-                } catch (t) {
-                    throw new w.ServerConnection.NetworkError(t)
+                    n = await C.ServerConnection.makeRequest(o, t, s)
+                } catch (e) {
+                    throw new C.ServerConnection.NetworkError(e)
                 }
                 let i = await n.text();
                 if (i.length > 0) try {
                     i = JSON.parse(i)
-                } catch (t) {
+                } catch (e) {
                     console.log("Not a JSON response body.", n)
                 }
-                if (!n.ok) throw new w.ServerConnection.ResponseError(n, i.message || i);
+                if (!n.ok) throw new C.ServerConnection.ResponseError(n, i.message || i);
                 return i
             }
-            const k = (0, a.debug)("PYFLYBY:");
-            class S {
-                constructor(t, e) {
-                    this._lockTimeout = t, this._activeTimeout = null, this.requestedLockCount = 0, this.clearedLockCount = 0, this._releaseLock = {}, this.promise = {
+            const k = (0, l.debug)("PYFLYBY:");
+            class x {
+                constructor(e, t) {
+                    this._recentKernelState = "", this._lockTimeout = e, this._activeTimeout = void 0, this.requestedLockCount = 0, this.clearedLockCount = 0, this._releaseLock = {}, this.promise = {
                         0: Promise.resolve()
-                    }, this._timeoutSignal = new l.Signal(this), this._sessionContext = e, this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this), this._timeoutSignal.connect(this.timeoutExpireHandler, this)
+                    }, this._timeoutSignal = new a.Signal(this), this._sessionContext = t, this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this), this._timeoutSignal.connect(this.timeoutExpireHandler, this)
                 }
-                kernelStateRecorder(t, e) {
-                    this._recentKernelState = e
+                kernelStateRecorder(e, t) {
+                    this._recentKernelState = t
                 }
                 _clearTimeout() {
-                    window.clearTimeout(this._activeTimeout), this._activeTimeout = null
+                    window.clearTimeout(this._activeTimeout), this._activeTimeout = void 0
                 }
-                timeoutExpireHandler(t, e) {
-                    this._clearTimeout(), "busy" === this._recentKernelState ? (console.debug("Extending Timeout For: ", e), this.createTimeout(e)) : this.release(e)
+                timeoutExpireHandler(e, t) {
+                    this._clearTimeout(), "busy" === this._recentKernelState ? (console.debug("Extending Timeout For: ", t), this.createTimeout(t)) : this.release(t)
                 }
                 async acquire() {
-                    const t = this.promise[this.requestedLockCount];
+                    const e = this.promise[this.requestedLockCount];
                     this.requestedLockCount++;
-                    const e = this.requestedLockCount;
-                    return this.promise[e] = new Promise((t => {
-                        this._releaseLock[e] = t
-                    })), await t, new Promise(((t, s) => t(e)))
-                }
-                release(t) {
-                    var e, s;
-                    this.clearedLockCount = t, null === (s = (e = this._releaseLock)[t]) || void 0 === s || s.call(e), delete this._releaseLock[t], this._clearTimeout(), this.clearedLockCount < this.requestedLockCount && this.createTimeout(t + 1)
+                    const t = this.requestedLockCount;
+                    return this.promise[t] = new Promise((e => {
+                        this._releaseLock[t] = e
+                    })), await e, new Promise(((e, s) => e(t)))
+                }
+                release(e) {
+                    var t, s;
+                    this.clearedLockCount = e, null === (s = (t = this._releaseLock)[e]) || void 0 === s || s.call(t), delete this._releaseLock[e], this._clearTimeout(), this.clearedLockCount < this.requestedLockCount && this.createTimeout(e + 1)
                 }
-                createTimeout(t) {
+                createTimeout(e) {
                     this._activeTimeout = setTimeout((() => {
-                        this._timeoutSignal.emit(t)
+                        this._timeoutSignal.emit(e)
                     }), this._lockTimeout)
                 }
             }
-            let Y = !1;
-            class E extends n.Widget {
-                constructor(t, e, s) {
-                    super(), this._context = null, this._sessionContext = null, this._settings = null, this._comms = {}, s.load("@deshaw/jupyterlab-pyflyby:plugin").then((t => {
-                        this._settings = t, (t.get("enabled").user || t.get("enabled").composite) && (this._sessionContext.kernelChanged.connect(this._handleKernelChange, this), this._sessionContext.statusChanged.connect(this._handleKernelStatusChange, this));
-                        const e = 1e3 * (t.get("lockTimeout").user || t.get("lockTimeout").composite);
-                        this._lock = new S(e, this._sessionContext)
-                    }), (t => {
+            let S = !1;
+            class Y extends n.Widget {
+                constructor(e, t, s) {
+                    super(), this._comms = {}, s.load("@deshaw/jupyterlab-pyflyby:plugin").then((e => {
+                        this._settings = e, (e.get("enabled").user || e.get("enabled").composite) && (this._sessionContext.kernelChanged.connect(this._handleKernelChange, this), this._sessionContext.statusChanged.connect(this._handleKernelStatusChange, this));
+                        const t = 1e3 * (e.get("lockTimeout").user || e.get("lockTimeout").composite);
+                        this._lock = new x(t, this._sessionContext)
+                    }), (e => {
                         k("PYFLYBY extension has been disabled")
-                    })), this._context = t, this._sessionContext = t.sessionContext
+                    })), this._context = e, this._sessionContext = e.sessionContext
                 }
-                async _launchDialog(t) {
-                    const e = new i.Dialog({
+                async _launchDialog(e) {
+                    const t = new i.Dialog({
                         title: "PYFLYBY",
                         body: "PYFLYBY will be adding imports to the first code cell in the notebook.\n            To disable the PYFLYBY extension or to disable this notification in future, go\n            to Settings -> Advanced Settings Editor and choose PYFLYBY preferences tab",
                         buttons: [i.Dialog.okButton()]
                     });
                     try {
-                        return await e.launch(), t
-                    } catch (t) {
-                        console.error(t)
+                        return await t.launch(), e
+                    } catch (e) {
+                        console.error(e)
                     }
                 }
                 _findAndSetImportCoordinates() {
                     const {
-                        model: t
+                        model: e
                     } = this._context;
-                    let e = o.ArrayExt.findFirstIndex((0, o.toArray)(t.cells), ((t, e) => {
-                        const s = t.metadata.get("tags");
-                        return !(!s || -1 === s.indexOf(u))
-                    })); - 1 === e && (e = (t => {
-                        const e = (0, o.toArray)(t);
-                        for (let t = 0; t < e.length; t++) {
-                            const s = e[t];
+                    let t = o.ArrayExt.findFirstIndex(Array.from(e.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
+                    })); - 1 === t && (t = (e => {
+                        const t = (0, o.toArray)(e);
+                        for (let e = 0; e < t.length; e++) {
+                            const s = t[e];
                             if ("code" === s.type) {
-                                const e = p(s.toJSON().source);
-                                if (e.length > 0 && !e[0].startsWith("%") && !e[0].startsWith('"""'))
-                                    for (let s = 0; s < e.length; s++)
-                                        if (f(e[s])) return t
+                                const t = _(s.toJSON().source);
+                                if (t.length > 0 && !t[0].startsWith("%") && !t[0].startsWith('"""'))
+                                    for (let s = 0; s < t.length; s++)
+                                        if (p(t[s])) return e
                             }
                         }
                         return -1
-                    })((0, o.toArray)(t.cells)));
-                    let s = t.cells.get(e),
-                        n = (t => {
-                            const e = p(t.toJSON().source);
-                            for (let t = e.length - 1; t >= 0; t--)
-                                if (e[t] === m.substr(0, m.length - 1)) {
+                    })(Array.from(e.cells)));
+                    let s = e.cells.get(t).sharedModel,
+                        n = (e => {
+                            const t = _(e.toJSON().source);
+                            for (let e = t.length - 1; e >= 0; e--)
+                                if (t[e] === u.substr(0, 26)) {
                                     let s = 0;
-                                    for (let o = 0; o < t - 1; o++) s += e[o].length + 1;
+                                    for (let o = 0; o < e - 1; o++) s += t[o].length + 1;
                                     return s
-                                } for (let t = e.length - 1; t >= 0; t--)
-                                if (s = e[t], f(s) && (s.includes("__future__") || -1 !== s.split(" ").indexOf("import") || s.includes("import_all_names")) && (t === e.length - 1 || b(e[t + 1]))) {
+                                } for (let e = t.length - 1; e >= 0; e--)
+                                if (s = t[e], p(s) && (s.includes("__future__") || -1 !== s.split(" ").indexOf("import") || s.includes("import_all_names")) && (e === t.length - 1 || f(t[e + 1]))) {
                                     let s = 0;
-                                    for (let o = 0; o <= t; o++) s += e[o].length + 1;
+                                    for (let o = 0; o <= e; o++) s += t[o].length + 1;
                                     return s
                                 } var s;
                             return -1
-                        })(t.cells.get(e));
-                    return -1 === n && (s = this._context.model.contentFactory.createCodeCell({
-                        cell: {
-                            source: `${d}\n\n${m}`,
-                            cell_type: "code",
-                            metadata: {}
-                        }
-                    }), this._context.model.cells.insert(e, s), n = d.length + 1), s.metadata.set("tags", [u]), {
-                        cellIndex: e,
+                        })(e.cells.get(t));
+                    return -1 === n && (s = this._context.model.sharedModel.insertCell(0, {
+                        source: `# THIS CELL WAS AUTO-GENERATED BY PYFLYBY\n\n\n${u}`,
+                        cell_type: "code",
+                        metadata: {}
+                    }), n = 43), s.setMetadata("tags", [d]), {
+                        cellIndex: t,
                         position: n
                     }
                 }
-                _insertImport(t) {
-                    let e = null;
-                    return Y || this._settings.get("disableNotification").user ? e = Promise.resolve(t) : (e = this._launchDialog(t), Y = !0), this._findAndSetImportCoordinates(), e
-                }
-                _sendFormatCodeMsg(t, e) {
-                    const s = o.ArrayExt.findFirstIndex((0, o.toArray)(this._context.model.cells), ((t, e) => {
-                        const s = t.metadata.get("tags");
-                        return !(!s || -1 === s.indexOf(u))
+                _insertImport(e) {
+                    let t;
+                    return S || !this._settings || this._settings.get("disableNotification").user ? t = Promise.resolve(e) : (t = this._launchDialog(e), S = !0), this._findAndSetImportCoordinates(), t
+                }
+                _sendFormatCodeMsg(e, t) {
+                    const s = o.ArrayExt.findFirstIndex(Array.from(this._context.model.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
                     }));
                     if (-1 !== s) {
                         const o = this._context.model.cells.get(s).toJSON().source,
-                            n = this._comms["pyflyby.format_imports"];
+                            n = this._comms[y];
                         n && !n.isDisposed && n.send({
-                            msg_id: e,
+                            msg_id: t,
                             input_code: o,
-                            imports: t,
-                            type: g
+                            imports: e,
+                            type: y
                         })
                     }
                 }
                 _getCommMsgHandler() {
-                    return async t => {
-                        const e = t.content.data;
-                        switch (e.type) {
-                            case y: {
-                                const t = e.missing_imports;
-                                this._insertImport(t).then((async t => {
-                                    const e = await this._lock.acquire();
-                                    this._sendFormatCodeMsg(t, e)
+                    return async e => {
+                        const t = e.content.data;
+                        switch (t.type) {
+                            case m: {
+                                const e = t.missing_imports;
+                                this._insertImport(e).then((async e => {
+                                    if (void 0 !== this._lock) {
+                                        const t = await this._lock.acquire();
+                                        this._sendFormatCodeMsg(e, t)
+                                    }
                                 }));
                                 break
                             }
-                            case g: {
-                                this._formatImports(e);
+                            case y: {
+                                this._formatImports(t);
                                 const {
-                                    msg_id: t
-                                } = e;
-                                this._lock.release(t);
+                                    msg_id: e
+                                } = t;
+                                void 0 !== this._lock && this._lock.release(e);
                                 break
                             }
-                            case _:
+                            case g:
                                 this._initializeComms().catch(console.error)
                         }
                     }
                 }
                 async _initializeComms() {
                     if (!this._sessionContext.session) return;
                     const {
-                        kernel: t
+                        kernel: e
                     } = this._sessionContext.session;
-                    if (!t) return;
-                    const e = t.createComm("pyflyby.missing_imports");
-                    e.onMsg = this._getCommMsgHandler();
+                    if (!e) return;
+                    const t = m,
+                        s = e.createComm(t);
+                    s.onMsg = this._getCommMsgHandler();
                     try {
-                        e.open()
-                    } catch (t) {
-                        console.error(`Unable to open PYFLYBY comm - ${t}`)
+                        s.open()
+                    } catch (e) {
+                        console.error(`Unable to open PYFLYBY comm - ${e}`)
                     }
-                    const s = t.createComm(g);
-                    s.onMsg = this._getCommMsgHandler(), s.onClose = t => {
-                        const e = t.content.comm_id;
-                        delete this._comms[e]
-                    }, this._comms["pyflyby.format_imports"] = s;
+                    const o = e.createComm(y);
+                    o.onMsg = this._getCommMsgHandler(), o.onClose = e => {
+                        const t = e.content.comm_id;
+                        delete this._comms[t]
+                    }, this._comms[y] = o;
                     try {
-                        s.open()
-                    } catch (t) {
-                        console.error(`Unable to open PYFLYBY comm - ${t}`)
+                        o.open()
+                    } catch (e) {
+                        console.error(`Unable to open PYFLYBY comm - ${e}`)
                     }
-                    return t.registerCommTarget(_, ((t, e) => {
-                        t.onMsg = this._getCommMsgHandler()
+                    return e.registerCommTarget(g, ((e, t) => {
+                        e.onMsg = this._getCommMsgHandler()
                     })), Promise.resolve()
                 }
-                _formatImports(t) {
+                _formatImports(e) {
                     const {
-                        formatted_code: e
-                    } = t, s = o.ArrayExt.findFirstIndex((0, o.toArray)(this._context.model.cells), ((t, e) => {
-                        const s = t.metadata.get("tags");
-                        return !(!s || -1 === s.indexOf(u))
+                        formatted_code: t
+                    } = e, s = o.ArrayExt.findFirstIndex(Array.from(this._context.model.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
                     }));
                     if (-1 !== s) {
-                        const t = this._context.model.cells.get(s);
-                        t.value.remove(0, t.value.text.length), t.value.insert(0, e)
+                        const e = this._context.model.cells.get(s).sharedModel;
+                        e.updateSource(0, e.source.length, t)
                     }
                 }
-                async _handleKernelChange(t, e) {
+                async _handleKernelChange(e, t) {
                     return await this._initializeComms()
                 }
-                _handleKernelStatusChange(t, e) {
-                    return "restarting" === e ? this._initializeComms() : null
+                _handleKernelStatusChange(e, t) {
+                    return "restarting" === t ? this._initializeComms() : null
                 }
             }
-            class T {
-                constructor(t) {
-                    this._settingRegistry = null, this._settingRegistry = t, this._loadSettings().catch(console.error)
+            class E {
+                constructor(e) {
+                    this._settingRegistry = e, this._loadSettings().catch(console.error)
                 }
                 async _loadSettings() {
                     try {
                         await this._settingRegistry.load("@deshaw/jupyterlab-pyflyby:plugin"), k("Successfully loaded PYFLYBY extension settings")
-                    } catch (t) {
+                    } catch (e) {
                         console.error("Settings could not be loaded")
                     }
                 }
-                createNew(t, e) {
-                    return new E(e, t, this._settingRegistry)
+                createNew(e, t) {
+                    return new Y(t, e, this._settingRegistry)
                 }
             }
-            async function L() {
+            async function T() {
                 try {
-                    await x("install-pyflyby", {
+                    await w("install-pyflyby", {
                         method: "POST"
                     })
-                } catch (t) {
-                    const e = await t.json();
-                    console.error(e.result)
+                } catch (e) {
+                    console.error(e)
                 }
             }
-            const v = h().createElement("div", null, h().createElement("p", null, "To use @deshaw/jupyterlab-pyflyby,", " ", h().createElement("a", {
+            const L = h().createElement("div", null, h().createElement("p", null, "To use @deshaw/jupyterlab-pyflyby,", " ", h().createElement("a", {
                     href: "https://github.com/deshaw/pyflyby/blob/master/README.rst",
                     style: {
                         color: "#0000EE"
                     },
                     target: "_blank",
                     rel: "noopener noreferrer"
                 }, "pyflyby"), " ", "ipython extension needs to be installed."), h().createElement("br", null), h().createElement("p", null, 'Clicking on "Install" will run following command'), h().createElement("div", {
                     style: {
                         font: "monospace",
                         color: "#ffffff",
                         backgroundColor: "#000000",
                         marginTop: "5px"
                     }
                 }, "$ py pyflyby.install_in_ipython_config_file"), h().createElement("br", null)),
-                P = {
+                v = {
                     id: "@deshaw/jupyterlab-pyflyby:plugin",
                     autoStart: !0,
                     requires: [r.ISettingRegistry],
-                    activate: async function(t, e) {
+                    activate: async function(e, t) {
                         console.log("JupyterLab extension @deshaw/jupyterlab-pyflyby is activated!");
-                        const s = await e.load("@deshaw/jupyterlab-pyflyby:plugin"),
+                        const s = await t.load("@deshaw/jupyterlab-pyflyby:plugin"),
                             o = s.get("enabled").user || s.get("enabled").composite,
                             n = s.get("installDialogDisplayed").user;
                         o && "loaded" !== await async function() {
-                            return (await x("pyflyby-status")).status
+                            return (await w("pyflyby-status")).status
                         }() && (n || (await (0, i.showDialog)({
                             title: "Installation required",
-                            body: v,
+                            body: L,
                             buttons: [i.Dialog.okButton({
                                 label: "Install"
                             }), i.Dialog.cancelButton({
                                 label: "Cancel",
                                 displayType: "default"
                             })],
                             defaultButton: 0
-                        })).button.accept ? await L() : await async function(t) {
+                        })).button.accept ? await T() : await async function(e) {
                             try {
-                                await x("disable-pyflyby", {
+                                await w("disable-pyflyby", {
                                     method: "POST",
                                     mode: "cors",
                                     cache: "no-cache",
                                     credentials: "include",
                                     headers: {
                                         "Content-type": "application/x-www-form-urlencoded"
                                     },
                                     body: new URLSearchParams("installDialogDisplayed=true")
                                 })
-                            } catch (t) {
-                                const e = await t.json();
-                                console.error(e.result)
+                            } catch (e) {
+                                console.error(e)
                             }
-                            await t.reload("@deshaw/jupyterlab-pyflyby:plugin")
-                        }(e)), t.docRegistry.addWidgetExtension("Notebook", new T(e))
+                            await e.reload("@deshaw/jupyterlab-pyflyby:plugin")
+                        }(t)), e.docRegistry.addWidgetExtension("Notebook", new E(t))
                     }
                 }
         }
     }
 ]);
```

### Comparing `jupyterlab_pyflyby-4.2.0/jupyterlab_pyflyby/labextension/static/remoteEntry.a3db63230ba521cc3ddb.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/remoteEntry.2f3f2d893fd3c5c9aea1.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,139 +1,136 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, d, f, p, c, h, b, v, y, g = {
-            603: (e, r, t) => {
+    var e, r, t, n, a, o, i, u, l, d, s, f, p, c, h, v, y, b, g, m = {
+            556: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(316).then((() => () => t(316))),
-                        "./extension": () => t.e(316).then((() => () => t(316))),
-                        "./style": () => t.e(534).then((() => () => t(534)))
+                        "./index": () => t.e(36).then((() => () => t(36))),
+                        "./extension": () => t.e(36).then((() => () => t(36))),
+                        "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var n = t.S.default,
-                                a = "default";
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[a] = e, t.I(a, r)
+                            var n = "default",
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => a,
                     init: () => o
                 })
             }
         },
-        m = {};
+        w = {};
 
-    function w(e) {
-        var r = m[e];
+    function j(e) {
+        var r = w[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = w[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, w), t.exports
+        return m[e](t, t.exports, j), t.exports
     }
-    w.m = g, w.c = m, w.n = e => {
+    j.m = m, j.c = w, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        227: "1cad1bc26a111ee76cd4",
-        316: "4f44e21efbe062818edc",
-        534: "2469f0c98db18f365947"
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        36: "815b80fd2ca5b739309a",
+        227: "d0383463ef62876fb46f",
+        747: "642119a933d152ff1ed4"
     } [e] + ".js?v=" + {
-        227: "1cad1bc26a111ee76cd4",
-        316: "4f44e21efbe062818edc",
-        534: "2469f0c98db18f365947"
-    } [e], w.g = function() {
+        36: "815b80fd2ca5b739309a",
+        227: "d0383463ef62876fb46f",
+        747: "642119a933d152ff1ed4"
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deshaw/jupyterlab-pyflyby:", w.l = (t, n, a, o) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deshaw/jupyterlab-pyflyby:", j.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        j.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        j.I = (t, n) => {
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var o = w.S[t],
+                j.o(j.S, t) || (j.S[t] = {});
+                var o = j.S[t],
                     i = "@deshaw/jupyterlab-pyflyby",
                     u = (e, r, t, n) => {
                         var a = o[e] = o[e] || {},
                             u = a[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                switch (t) {
-                    case "default":
-                        u("@deshaw/jupyterlab-pyflyby", "4.2.0", (() => w.e(316).then((() => () => w(316))))), u("debug", "4.2.0", (() => w.e(227).then((() => () => w(227)))))
-                }
-                return e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@deshaw/jupyterlab-pyflyby", "5.0.0", (() => j.e(36).then((() => () => j(36))))), u("debug", "4.3.4", (() => j.e(227).then((() => () => j(227)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -170,120 +167,125 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == d) {
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
+                if ("u" == s) {
                     if (!l || "u" != f) return !1
                 } else if (l)
-                    if (f == d)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (a ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != a) return !1;
+                    if (u <= n || s < f != a) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + a(t) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(t, a, n)), f(e[t][a])
-    }, d = (e, r, t) => {
+        return o(n, a) || f(l(e, t, a, n)), p(e[t][a])
+    }, s = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
-        var o = w.I(r);
-        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && d(r, t, n);
-        return o ? f(o) : a()
-    })), b = {}, v = {
-        118: () => c("default", "@jupyterlab/apputils", [1, 3, 4, 3]),
-        238: () => c("default", "@jupyterlab/services", [1, 6, 4, 3]),
-        271: () => c("default", "react", [1, 17, 0, 1]),
-        305: () => h("default", "debug", [1, 4, 1, 1], (() => w.e(227).then((() => () => w(227))))),
-        345: () => c("default", "@jupyterlab/settingregistry", [1, 3, 4, 3]),
-        398: () => c("default", "@jupyterlab/coreutils", [1, 5, 4, 3]),
-        433: () => c("default", "@lumino/widgets", [1, 1, 30, 0]),
-        840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0])
-    }, y = {
-        316: [118, 238, 271, 305, 345, 398, 433, 840, 918]
-    }, w.f.consumes = (e, r) => {
-        w.o(y, e) && y[e].forEach((e => {
-            if (w.o(b, e)) return r.push(b[e]);
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, a) {
+        var o = j.I(r);
+        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), v = c(((e, r, t, n, a) => {
+        var o = r && j.o(r, t) && s(r, t, n);
+        return o ? p(o) : a()
+    })), y = {}, b = {
+        29: () => h("default", "react", [1, 18, 2, 0]),
+        67: () => h("default", "@jupyterlab/services", [1, 7, 0, 0]),
+        305: () => v("default", "debug", [1, 4, 1, 1], (() => j.e(227).then((() => () => j(227))))),
+        406: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        501: () => h("default", "@jupyterlab/apputils", [1, 4, 0, 0]),
+        629: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
+        697: () => h("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        778: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
+        901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
+    }, g = {
+        36: [29, 67, 305, 406, 501, 629, 697, 778, 901]
+    }, j.f.consumes = (e, r) => {
+        j.o(g, e) && g[e].forEach((e => {
+            if (j.o(y, e)) return r.push(y[e]);
             var t = r => {
-                    b[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    y[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete y[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var a = b[e]();
+                a.then ? r.push(y[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             585: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var a = new Promise(((t, a) => n = e[r] = [t, a]));
                     t.push(n[2] = a);
-                    var o = w.p + w.u(r),
+                    var o = j.p + j.u(r),
                         i = new Error;
-                    w.l(o, (t => {
-                        if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    j.l(o, (t => {
+                        if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, a, [o, i, u] = t,
                     l = 0;
-                for (n in i) w.o(i, n) && (w.m[n] = i[n]);
-                for (u && u(w), r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[o[l]] = 0
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    u && u(j)
+                }
+                for (r && r(t); l < o.length; l++) a = o[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_deshaw_jupyterlab_pyflyby = self.webpackChunk_deshaw_jupyterlab_pyflyby || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var j = w(603);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deshaw/jupyterlab-pyflyby"] = j
+    })(), j.nc = void 0;
+    var S = j(556);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deshaw/jupyterlab-pyflyby"] = S
 })();
```

### Comparing `jupyterlab_pyflyby-4.2.0/package.json` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8619285806785808%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,52 +1,64 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.2f3f2d893fd3c5c9aea1.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -60,30 +72,37 @@
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.2.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.2.0/src/cellUtils.ts` & `jupyterlab_pyflyby-5.0.0/src/cellUtils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.2.0/src/handler.ts` & `jupyterlab_pyflyby-5.0.0/src/handler.ts`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
   } catch (error) {
-    throw new ServerConnection.NetworkError(error);
+    throw new ServerConnection.NetworkError(error as any);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
       data = JSON.parse(data);
```

### Comparing `jupyterlab_pyflyby-4.2.0/src/index.tsx` & `jupyterlab_pyflyby-5.0.0/src/index.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,26 @@
  * 1. If PYFLYBY_END_MSG is present, import is added above it.
  * 2. Added import after last import statement in code cell. Identifying import statement is
  *    is done by simple heuristics. This step can be shifted to pyflyby where python parser can be used to
  *    determine it accurately.
  */
 
 // Lumino imports
-import { toArray, ArrayExt } from '@lumino/algorithm';
+import { ArrayExt } from '@lumino/algorithm';
 import { JSONValue, JSONObject } from '@lumino/coreutils';
 import { Widget, Panel } from '@lumino/widgets';
 
 // Jupyterlab imports
-import { JupyterFrontEnd } from '@jupyterlab/application';
+import {
+  JupyterFrontEnd,
+  JupyterFrontEndPlugin
+} from '@jupyterlab/application';
 import { Dialog, ISessionContext, showDialog } from '@jupyterlab/apputils';
 import { ICellModel } from '@jupyterlab/cells';
+import { ISharedCell } from '@jupyter/ydoc';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { INotebookModel } from '@jupyterlab/notebook';
 import { Session, Kernel, KernelMessage } from '@jupyterlab/services';
 import { Signal } from '@lumino/signaling';
 
 import { debug } from 'debug';
@@ -48,47 +52,47 @@
 const log = debug('PYFLYBY:');
 
 class CommLock {
   _releaseLock: any;
   promise: any;
   requestedLockCount: number;
   clearedLockCount: number;
-  _activeTimeout: number;
+  _activeTimeout: number | undefined;
   _lockTimeout: number;
   _timeoutSignal: Signal<CommLock, number>;
-  _recentKernelState: string;
+  _recentKernelState = '';
   _sessionContext: ISessionContext;
 
   constructor(_lockTimeout: number, sessionContext: ISessionContext) {
     this._lockTimeout = _lockTimeout;
-    this._activeTimeout = null;
+    this._activeTimeout = undefined;
     this.requestedLockCount = 0;
     this.clearedLockCount = 0;
     this._releaseLock = {};
     this.promise = { 0: Promise.resolve() };
     this._timeoutSignal = new Signal<CommLock, number>(this);
     this._sessionContext = sessionContext;
     this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this);
     this._timeoutSignal.connect(this.timeoutExpireHandler, this);
   }
 
-  kernelStateRecorder(sender: ISessionContext, args: Kernel.Status) {
+  kernelStateRecorder(_sender: ISessionContext, args: Kernel.Status) {
     this._recentKernelState = args;
   }
 
   _clearTimeout() {
     window.clearTimeout(this._activeTimeout);
-    this._activeTimeout = null;
+    this._activeTimeout = undefined;
   }
 
   /*
-    If the kernel was busy the last time, we assume it was busy executing 
+    If the kernel was busy the last time, we assume it was busy executing
     code and we restart the timeout.
   */
-  timeoutExpireHandler(sender: CommLock, id: number) {
+  timeoutExpireHandler(_sender: CommLock, id: number) {
     this._clearTimeout();
     if (this._recentKernelState === 'busy') {
       console.debug('Extending Timeout For: ', id);
       this.createTimeout(id);
     } else {
       this.release(id);
     }
@@ -98,15 +102,15 @@
     const lastLockPromise = this.promise[this.requestedLockCount];
     this.requestedLockCount++;
     const lockId = this.requestedLockCount;
     this.promise[lockId] = new Promise(resolve => {
       this._releaseLock[lockId] = resolve;
     });
     await lastLockPromise;
-    return new Promise((res, rej) => res(lockId));
+    return new Promise((res, _rej) => res(lockId));
   }
 
   release(lockId: number): void {
     this.clearedLockCount = lockId;
     this._releaseLock[lockId]?.();
     delete this._releaseLock[lockId];
     this._clearTimeout();
@@ -125,18 +129,18 @@
 // We'd like to show the notification only once per session, not for each notebook
 let _userWasNotified = false;
 
 /**
  * An extension that adds pyflyby integration to a single notebook widget
  */
 class PyflyByWidget extends Widget {
-  _lock: CommLock;
+  _lock: CommLock | undefined;
   constructor(
     context: DocumentRegistry.IContext<INotebookModel>,
-    panel: Panel,
+    _panel: Panel,
     settingRegistry: ISettingRegistry
   ) {
     super();
     // get a reference to the settings registry
     settingRegistry.load('@deshaw/jupyterlab-pyflyby:plugin').then(
       (settings: ISettingRegistry.ISettings) => {
         this._settings = settings;
@@ -155,15 +159,15 @@
 
         const _lockTimeout =
           1000 *
           ((settings.get('lockTimeout').user ||
             settings.get('lockTimeout').composite) as number);
         this._lock = new CommLock(_lockTimeout, this._sessionContext);
       },
-      (err: any) => {
+      (_err: any) => {
         log('PYFLYBY extension has been disabled');
       }
     );
     this._context = context;
     this._sessionContext = context.sessionContext;
   }
 
@@ -182,80 +186,79 @@
       await dialog.launch();
       return imports;
     } catch (e) {
       console.error(e);
     }
   }
 
-  /**
-   * All the logic related to finding the right cell
-   */
+  // /**
+  //  * All the logic related to finding the right cell
+  //  */
   _findAndSetImportCoordinates() {
     const { model } = this._context;
     let pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
 
     /**
      * Since the cell doesn't exist, we make one or, if the first
      * code cell contains an import block, put it below that.
      */
     if (pyflybyCellIndex === -1) {
-      pyflybyCellIndex = findCell(toArray(model.cells));
+      pyflybyCellIndex = findCell(Array.from(model.cells));
     }
 
-    let cell = model.cells.get(pyflybyCellIndex);
-
+    let cell = model.cells.get(pyflybyCellIndex).sharedModel;
     let position = findLinePos(model.cells.get(pyflybyCellIndex));
 
     if (position === -1) {
-      cell = this._context.model.contentFactory.createCodeCell({
-        cell: {
-          source: `${PYFLYBY_START_MSG}\n\n${PYFLYBY_END_MSG}`,
-          cell_type: 'code',
-          metadata: {}
-        }
+      cell = this._context.model.sharedModel.insertCell(0, {
+        source: `${PYFLYBY_START_MSG}\n\n${PYFLYBY_END_MSG}`,
+        cell_type: 'code',
+        metadata: {}
       });
-
-      this._context.model.cells.insert(pyflybyCellIndex, cell);
       position = PYFLYBY_START_MSG.length + 1;
     }
-    cell.metadata.set('tags', [PYFLYBY_CELL_TAG]);
+    cell.setMetadata('tags', [PYFLYBY_CELL_TAG]);
     return { cellIndex: pyflybyCellIndex, position };
   }
 
   /**
    * Adds the import block to the appropriate cell at the appropriate
    * location.
    *
    * @param importBlock - the import statement or block of import statements
    */
   _insertImport(imports: any) {
-    let p: Promise<any> = null;
-    if (!_userWasNotified && !this._settings.get('disableNotification').user) {
+    let p: Promise<any>;
+    if (
+      !_userWasNotified &&
+      this._settings &&
+      !this._settings.get('disableNotification').user
+    ) {
       p = this._launchDialog(imports);
       _userWasNotified = true;
     } else {
       p = Promise.resolve(imports);
     }
 
     // creates the cell for imports
     this._findAndSetImportCoordinates();
     return p;
   }
 
   _sendFormatCodeMsg(imports: any, lockId: number) {
     const pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(this._context.model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(this._context.model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
     if (pyflybyCellIndex !== -1) {
       const cellSource = this._context.model.cells
         .get(pyflybyCellIndex)
         .toJSON().source;
@@ -275,23 +278,27 @@
     return async (msg: KernelMessage.ICommMsgMsg) => {
       const msgContent: JSONValue = msg.content.data;
       switch ((msgContent as JSONObject).type) {
         case PYFLYBY_COMMS.MISSING_IMPORTS: {
           const itd = msgContent['missing_imports'];
           this._insertImport(itd).then(async imports => {
             // Acquire new lock but wait for previous lock to expire
-            const currentLockId = await this._lock.acquire();
-            this._sendFormatCodeMsg(imports, currentLockId);
+            if (this._lock !== undefined) {
+              const currentLockId = await this._lock.acquire();
+              this._sendFormatCodeMsg(imports, currentLockId);
+            }
           });
           break;
         }
         case PYFLYBY_COMMS.FORMAT_IMPORTS: {
           this._formatImports(msgContent);
           const { msg_id: lockId }: any = msgContent;
-          this._lock.release(lockId);
+          if (this._lock !== undefined) {
+            this._lock.release(lockId);
+          }
           break;
         }
         case PYFLYBY_COMMS.INIT: {
           this._initializeComms().catch(console.error);
           break;
         }
         default:
@@ -329,58 +336,58 @@
       formatMsgComm.open();
     } catch (e) {
       console.error(`Unable to open PYFLYBY comm - ${e}`);
     }
 
     kernel.registerCommTarget(
       PYFLYBY_COMMS.INIT,
-      (comm, msg: KernelMessage.ICommOpenMsg) => {
+      (comm, _msg: KernelMessage.ICommOpenMsg) => {
         comm.onMsg = this._getCommMsgHandler();
       }
     );
 
     return Promise.resolve();
   }
 
   _formatImports(msgData: any) {
     const { formatted_code: formattedCode } = msgData;
     const pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(this._context.model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(this._context.model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
     if (pyflybyCellIndex !== -1) {
-      const cell: ICellModel = this._context.model.cells.get(pyflybyCellIndex);
-      cell.value.remove(0, cell.value.text.length);
-      cell.value.insert(0, formattedCode);
+      const cell: ISharedCell =
+        this._context.model.cells.get(pyflybyCellIndex).sharedModel;
+      cell.updateSource(0, cell.source.length, formattedCode);
     }
   }
 
   async _handleKernelChange(
-    sender: ISessionContext,
-    kernelChangedArgs: Session.ISessionConnection.IKernelChangedArgs
+    _sender: ISessionContext,
+    _kernelChangedArgs: Session.ISessionConnection.IKernelChangedArgs
   ): Promise<any> {
     return await this._initializeComms();
   }
 
   _handleKernelStatusChange(
-    sender: ISessionContext,
+    _sender: ISessionContext,
     args: Kernel.Status
   ): Promise<any> | null {
     if (args === 'restarting') {
       return this._initializeComms();
     }
     return null;
   }
 
-  private _context: DocumentRegistry.IContext<INotebookModel> = null;
-  private _sessionContext: ISessionContext = null;
-  private _settings: ISettingRegistry.ISettings = null;
+  private _context: DocumentRegistry.IContext<INotebookModel>;
+  private _sessionContext: ISessionContext;
+  private _settings: ISettingRegistry.ISettings | undefined;
   private _comms: any = {};
 }
 
 /**
  * An extension that adds pyflyby integration to a notebook widget
  */
 class PyflyByWidgetExtension implements DocumentRegistry.WidgetExtension {
@@ -401,44 +408,42 @@
     }
   }
 
   createNew(panel: Panel, context: DocumentRegistry.IContext<INotebookModel>) {
     return new PyflyByWidget(context, panel, this._settingRegistry);
   }
 
-  private _settingRegistry: ISettingRegistry = null;
+  private _settingRegistry: ISettingRegistry;
 }
 
 async function isPyflybyInstalled() {
   const pyflybyStatus = await requestAPI<any>('pyflyby-status');
   return pyflybyStatus.status;
 }
 
 async function installPyflyby() {
   try {
     await requestAPI<any>('install-pyflyby', { method: 'POST' });
   } catch (err) {
-    const errMsg = await err.json();
-    console.error(errMsg.result);
+    console.error(err);
   }
 }
 
 async function disableJupyterlabPyflyby(registry: ISettingRegistry) {
   try {
     await requestAPI<any>('disable-pyflyby', {
       method: 'POST',
       mode: 'cors',
       cache: 'no-cache',
       credentials: 'include',
       headers: { 'Content-type': 'application/x-www-form-urlencoded' },
       body: new URLSearchParams('installDialogDisplayed=true')
     });
   } catch (err) {
-    const errMsg = await err.json();
-    console.error(errMsg.result);
+    console.error(err);
   }
   await registry.reload('@deshaw/jupyterlab-pyflyby:plugin');
 }
 
 const installationBody = (
   <div>
     <p>
@@ -465,15 +470,15 @@
     >
       $ py pyflyby.install_in_ipython_config_file
     </div>
     <br />
   </div>
 );
 
-const extension = {
+const extension: JupyterFrontEndPlugin<void> = {
   id: '@deshaw/jupyterlab-pyflyby:plugin',
   autoStart: true,
   requires: [ISettingRegistry],
   activate: async function (
     app: JupyterFrontEnd,
     registry: ISettingRegistry
   ): Promise<void> {
```

### Comparing `jupyterlab_pyflyby-4.2.0/tsconfig.json` & `jupyterlab_pyflyby-5.0.0/tsconfig.json`

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

