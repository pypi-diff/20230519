# Comparing `tmp/new-component-0.3.1.tar.gz` & `tmp/new-component-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.3.1.tar", max compression
+gzip compressed data, was "new-component-0.3.2.tar", last modified: Fri May 19 04:20:38 2023, max compression
```

## Comparing `new-component-0.3.1.tar` & `new-component-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1067 2022-07-13 16:50:07.610651 new-component-0.3.1/LICENSE
--rw-r--r--   0        0        0     4857 2022-07-13 16:50:07.610651 new-component-0.3.1/README.md
--rw-r--r--   0        0        0      347 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/__init__.py
--rw-r--r--   0        0        0      142 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/__main__.py
--rw-r--r--   0        0        0     1961 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_config.py
--rw-r--r--   0        0        0      708 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_confirms.py
--rw-r--r--   0        0        0      566 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_constants.py
--rw-r--r--   0        0        0     2088 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_echos.py
--rw-r--r--   0        0        0      360 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_jinja.py
--rw-r--r--   0        0        0      249 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_utils.py
--rw-r--r--   0        0        0      206 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/_version.py
--rw-r--r--   0        0        0     4121 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/cli.py
--rw-r--r--   0        0        0        0 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/py.typed
--rw-r--r--   0        0        0      269 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/templates/component.js.j2
--rw-r--r--   0        0        0       48 2022-07-13 16:50:07.610651 new-component-0.3.1/new_component/templates/index.js.j2
--rw-r--r--   0        0        0     1195 2022-07-13 16:50:07.610651 new-component-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5968 2022-07-13 16:52:28.507619 new-component-0.3.1/setup.py
--rw-r--r--   0        0        0     5573 2022-07-13 16:52:28.508095 new-component-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 04:20:24.255170 new-component-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4857 2023-05-19 04:20:24.255170 new-component-0.3.2/README.md
+-rw-r--r--   0        0        0      347 2023-05-19 04:20:24.255170 new-component-0.3.2/new_component/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-19 04:20:24.255170 new-component-0.3.2/new_component/__main__.py
+-rw-r--r--   0        0        0     1961 2023-05-19 04:20:24.255170 new-component-0.3.2/new_component/_config.py
+-rw-r--r--   0        0        0      708 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_confirms.py
+-rw-r--r--   0        0        0      566 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_constants.py
+-rw-r--r--   0        0        0     2088 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_echos.py
+-rw-r--r--   0        0        0      360 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_jinja.py
+-rw-r--r--   0        0        0      249 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_utils.py
+-rw-r--r--   0        0        0      206 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/_version.py
+-rw-r--r--   0        0        0     4121 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/cli.py
+-rw-r--r--   0        0        0        0 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/py.typed
+-rw-r--r--   0        0        0      269 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/templates/component.js.j2
+-rw-r--r--   0        0        0       48 2023-05-19 04:20:24.259170 new-component-0.3.2/new_component/templates/index.js.j2
+-rw-r--r--   0        0        0     1595 2023-05-19 04:20:24.259170 new-component-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6187 2023-05-19 04:20:24.259170 new-component-0.3.2/tests/test_new_component.py
+-rw-r--r--   0        0        0      517 2023-05-19 04:20:24.259170 new-component-0.3.2/tests/test_version.py
+-rw-r--r--   0        0        0     5112 1970-01-01 00:00:00.000000 new-component-0.3.2/PKG-INFO
```

### Comparing `new-component-0.3.1/LICENSE` & `new-component-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/README.md` & `new-component-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/new_component/_config.py` & `new-component-0.3.2/new_component/_config.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/new_component/_confirms.py` & `new-component-0.3.2/new_component/_confirms.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/new_component/_constants.py` & `new-component-0.3.2/new_component/_constants.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/new_component/_echos.py` & `new-component-0.3.2/new_component/_echos.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/new_component/cli.py` & `new-component-0.3.2/new_component/cli.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.1/setup.py` & `new-component-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,159 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: new-component
+Version: 0.3.2
+Summary: Quickly create opinionated Styled Components for React Projects
+License: MIT
+Author-email: Ian Cleary <github@iancleary.me>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 
-packages = \
-['new_component']
+# new-component
 
-package_data = \
-{'': ['*'], 'new_component': ['templates/*']}
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![ci](https://github.com/iancleary/new-component/workflows/ci/badge.svg)](https://github.com/iancleary/new-component/actions/workflows/ci.yml)
 
-install_requires = \
-['Jinja2>=3.0.3,<4.0.0',
- 'colorama>=0.4.3,<0.5.0',
- 'rich>=10.11.0,<13.0.0',
- 'shellingham>=1.3.0,<2.0.0',
- 'typer==0.6.1']
-
-entry_points = \
-{'console_scripts': ['new-component = new_component.__main__:main']}
-
-setup_kwargs = {
-    'name': 'new-component',
-    'version': '0.3.1',
-    'description': 'Quickly create opinionated Styled Components for React Projects',
-    'long_description': '# new-component\n\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![ci](https://github.com/iancleary/new-component/workflows/ci/badge.svg)](https://github.com/iancleary/new-component/actions/workflows/ci.yml)\n\nIan Cleary ([iancleary](https://github.com/iancleary))\n\n## Description\n\n**Welcome!** This is a CLI for creating [styled-components](https://styled-components.com) for React projects quickly.\n\n> Note: I\'ve rewrote Josh W Comeau\'s [new-component](https://www.npmjs.com/package/new-component) NPM package in Python 🐍 and adapted it to my preferences. It is an excellent project and you should check it out!\n\nI didn\'t understand styled components at first. At the time of this writing, I\'m looking to develop my understanding of CSS, upon the advice of Josh W Comeau\'s blog post "[The styled-components Happy Path](https://www.joshwcomeau.com/css/styled-components/)".\n\nAfter you read that article, you\'ll gather that this CLI aims to combine the wisdom of Josh\'s templates with my personal preferences.\n\n- Adding the `import styled from "styled-components"` in the new `component.js` file.\n- Adding a `styled.Wrapper` component definition (and making it .the parent html element in the React Component\'s `render` function)\n\n## Quickstart\n\n```sh\n❯ pipx install new-component\n❯ new-component --help\n```\n\nThat will output the following:\n\n```\nUsage: new_component [OPTIONS] NAME\n\n  Creates an new component directory in a React project, with opinionated\n  defaults for styled-components.\n\n  See https://styled-components.com/ for more information.\n\nArguments:\n  NAME  Name of component to create.  [required]\n\nOptions:\n  -d, --directory TEXT  The directory in which to create the component.\n                        [default: src/components/]\n  -e, --extension TEXT  The file extension for the created component files.\n                        [default: js]\n  -v, --version         Show the application\'s version and exit.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n```\n\n## Example Usage\n\nThe first and only argument is the name of the component to create.\n\n```bash\n❯ new-component Backdrop\nCreated a new Backdrop Component 💅 🚀!\n/Users/iancleary/Personal/new-component/src/components/Test4\n```\n\nThe path printed is the absolute path to new component folder.\n\n> It will very based upon your setup!\n\nThis command created two files:\n\n`src/components/Backdrop/index.js`\n`src/components/Backdrop/Backdrop.js`\n\nThe contents of the files will be as follows:\n\n```js\n// `src/components/Backdrop/index.js`\nexport { default } from "./Backdrop"\n```\n\n```js\n// `src/components/Backdrop/Backdrop.js`\nimport React from "react"\nimport styled from "styled-components"\n\nconst Backdrop = ({children}) => {\n  return (\n    <Wrapper>\n      {children}\n    </Wrapper>\n  )\n};\n\nconst Wrapper = styled.div`\n  /* CSS Goes Here */\n`\n\nexport default Backdrop\n```\n\n## Configuration\n\nConfiguration can be done through 3 different ways:\n\n* Creating a global `settings.json` in your home directory (`~/.config/new-component/settings.json`).\n* Creating a local `.new-component-config.json` in your project\'s root directory.\n* Command-line arguments.\n\nThe resulting values are merged, with command-line values overwriting local values, and local values overwriting global ones.\n\n## API Reference\n\n### Directory\n\nControls the desired directory for the created component. Defaults to src/components\n\nUsage:\n\nCommand line: `--directory <value>` or `-d <value>`\n\nJSON config: `{ "directory": <value> }`\n\n### File Extension\n\nControls the file extension for the created components. Can be either js (default) or jsx.\n\nUsage:\n\nCommand line: `--extension <value> or -e <value>`\n\nJSON config: `{ "extension": <value> }`\n\n## Further information\n\n> I will likely evolve this CLI as I learn more; I\'m on my way 😊\n\n- Add different component types\n- Promote better patterns to ensure CSS (single source of styles, Isolated CSS)\n\nThanks to Josh W Comeau\'s blog post "[The styled-components Happy Path\n](https://www.joshwcomeau.com/css/styled-components/) for starting my education! Again, it puts this README in perspective.\n\n**Enjoy quickly creating styled components 💅 🚀!**\n\n## Contributing\n\nI created this CLI for my opinionated uses and may not accept changes.\n\nSee [CONTRIBUTING.md](.github/CONTRIBUTING.md).\n',
-    'author': 'Ian Cleary',
-    'author_email': 'contact@iancleary.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/iancleary/new-component',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+Ian Cleary ([iancleary](https://github.com/iancleary))
 
+## Description
+
+**Welcome!** This is a CLI for creating [styled-components](https://styled-components.com) for React projects quickly.
+
+> Note: I've rewrote Josh W Comeau's [new-component](https://www.npmjs.com/package/new-component) NPM package in Python 🐍 and adapted it to my preferences. It is an excellent project and you should check it out!
+
+I didn't understand styled components at first. At the time of this writing, I'm looking to develop my understanding of CSS, upon the advice of Josh W Comeau's blog post "[The styled-components Happy Path](https://www.joshwcomeau.com/css/styled-components/)".
+
+After you read that article, you'll gather that this CLI aims to combine the wisdom of Josh's templates with my personal preferences.
+
+- Adding the `import styled from "styled-components"` in the new `component.js` file.
+- Adding a `styled.Wrapper` component definition (and making it .the parent html element in the React Component's `render` function)
+
+## Quickstart
+
+```sh
+❯ pipx install new-component
+❯ new-component --help
+```
+
+That will output the following:
+
+```
+Usage: new_component [OPTIONS] NAME
+
+  Creates an new component directory in a React project, with opinionated
+  defaults for styled-components.
+
+  See https://styled-components.com/ for more information.
+
+Arguments:
+  NAME  Name of component to create.  [required]
+
+Options:
+  -d, --directory TEXT  The directory in which to create the component.
+                        [default: src/components/]
+  -e, --extension TEXT  The file extension for the created component files.
+                        [default: js]
+  -v, --version         Show the application's version and exit.
+  --install-completion  Install completion for the current shell.
+  --show-completion     Show completion for the current shell, to copy it or
+                        customize the installation.
+  --help                Show this message and exit.
+```
+
+## Example Usage
+
+The first and only argument is the name of the component to create.
+
+```bash
+❯ new-component Backdrop
+Created a new Backdrop Component 💅 🚀!
+/Users/iancleary/Personal/new-component/src/components/Test4
+```
+
+The path printed is the absolute path to new component folder.
+
+> It will very based upon your setup!
+
+This command created two files:
+
+`src/components/Backdrop/index.js`
+`src/components/Backdrop/Backdrop.js`
+
+The contents of the files will be as follows:
+
+```js
+// `src/components/Backdrop/index.js`
+export { default } from "./Backdrop"
+```
+
+```js
+// `src/components/Backdrop/Backdrop.js`
+import React from "react"
+import styled from "styled-components"
+
+const Backdrop = ({children}) => {
+  return (
+    <Wrapper>
+      {children}
+    </Wrapper>
+  )
+};
+
+const Wrapper = styled.div`
+  /* CSS Goes Here */
+`
+
+export default Backdrop
+```
+
+## Configuration
+
+Configuration can be done through 3 different ways:
+
+* Creating a global `settings.json` in your home directory (`~/.config/new-component/settings.json`).
+* Creating a local `.new-component-config.json` in your project's root directory.
+* Command-line arguments.
+
+The resulting values are merged, with command-line values overwriting local values, and local values overwriting global ones.
+
+## API Reference
+
+### Directory
+
+Controls the desired directory for the created component. Defaults to src/components
+
+Usage:
+
+Command line: `--directory <value>` or `-d <value>`
+
+JSON config: `{ "directory": <value> }`
+
+### File Extension
+
+Controls the file extension for the created components. Can be either js (default) or jsx.
+
+Usage:
+
+Command line: `--extension <value> or -e <value>`
+
+JSON config: `{ "extension": <value> }`
+
+## Further information
+
+> I will likely evolve this CLI as I learn more; I'm on my way 😊
+
+- Add different component types
+- Promote better patterns to ensure CSS (single source of styles, Isolated CSS)
+
+Thanks to Josh W Comeau's blog post "[The styled-components Happy Path
+](https://www.joshwcomeau.com/css/styled-components/) for starting my education! Again, it puts this README in perspective.
+
+**Enjoy quickly creating styled components 💅 🚀!**
+
+## Contributing
+
+I created this CLI for my opinionated uses and may not accept changes.
+
+See [CONTRIBUTING.md](.github/CONTRIBUTING.md).
 
-setup(**setup_kwargs)
```

