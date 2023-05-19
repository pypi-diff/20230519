# Comparing `tmp/hspylib-hqt-0.9.2.tar.gz` & `tmp/hspylib-hqt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-hqt-0.9.2.tar", last modified: Wed Apr 19 19:05:04 2023, max compression
+gzip compressed data, was "hspylib-hqt-0.9.3.tar", last modified: Fri May 19 18:16:19 2023, max compression
```

## Comparing `hspylib-hqt-0.9.2.tar` & `hspylib-hqt-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.432510 hspylib-hqt-0.9.2/
--rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.2/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)    11519 2023-04-19 19:05:04.431751 hspylib-hqt-0.9.2/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)    10507 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.396460 hspylib-hqt-0.9.2/hqt/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.413448 hspylib-hqt-0.9.2/hqt/promotions/
--rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/promotions/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      834 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hcombobox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7677 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hconsole.py
--rw-r--r--   0 hjunior    (504) staff       (20)      663 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hframe.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2567 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hlabel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6559 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/promotions/hlistwidget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4392 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hstacked_widget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6224 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/promotions/htablemodel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5444 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/promotions/htableview.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6280 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/htoolbox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2588 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/qt_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3851 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/stream_capturer.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.421809 hspylib-hqt-0.9.2/hqt/views/
--rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/views/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      860 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/views/main_view.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2309 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/views/qt_view.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.430888 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)    11519 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:05:04.432645 hspylib-hqt-0.9.2/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2072 2023-04-18 22:30:29.000000 hspylib-hqt-0.9.2/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.906880 hspylib-hqt-0.9.3/
+-rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.3/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)    11723 2023-05-19 18:16:19.905577 hspylib-hqt-0.9.3/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)    10711 2023-05-19 18:16:18.000000 hspylib-hqt-0.9.3/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.872965 hspylib-hqt-0.9.3/hqt/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-19 18:16:18.000000 hspylib-hqt-0.9.3/hqt/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.887851 hspylib-hqt-0.9.3/hqt/promotions/
+-rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/promotions/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hcombobox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hconsole.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hframe.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hlabel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hlistwidget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hstacked_widget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htablemodel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htableview.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htoolbox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/qt_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/stream_capturer.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.894111 hspylib-hqt-0.9.3/hqt/views/
+-rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/views/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/views/main_view.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/views/qt_view.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.903988 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)    11723 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-19 18:16:19.907110 hspylib-hqt-0.9.3/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.3/setup.py
```

### Comparing `hspylib-hqt-0.9.2/PKG-INFO` & `hspylib-hqt-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.2
-Summary: HSPyLib - QT framework extensions
+Version: 0.9.3
+Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
 Keywords: qt,ui,extensions,application,pyqt
@@ -21,20 +21,20 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# HomeSetup Python Library - HsPyLib
+# <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
-## Your mature python application
+## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -65,15 +65,15 @@
 
 Create an easy to use and code multiple select or choose input method:
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
 from clitt.core.icons.font_awesome.nav_icons import NavIcons
-from clitt.core.tui.mselect import mselect
+from clitt.core.tui.mselect.mselect import mselect
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class SelectableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -100,15 +100,15 @@
 ```
 
 ![MenuSelect](https://iili.io/HYBFh74.png "MenuSelect")
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
-from clitt.core.tui.mchoose import mchoose
+from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class ChooseableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -314,33 +314,33 @@
 
 To clone HsPyLib into your local machine type the command:
 
 `# git clone https://github.com/yorevs/hspylib.git`
 
 ## Documentation
 
-TBD
+The API documentation can be found [here](docs/api/index.html)
 
 ## Contact
 
 You can contact us using our [Gitter](https://gitter.im/hspylib/community) community or using our
 [Reddit](https://www.reddit.com/user/yorevs).
 
 ## Support HsPyLib
 
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
-[guidelines](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).
+[guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 ## Links
 
-- Documentation: TBD
+- Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
 - Official chat: https://gitter.im/hspylib/community
 - Contact: https://www.reddit.com/user/yorevs
-- Mailto: yorevs@hotmail.com
+- Mailto: [Yorevs](mailto:yorevs@hotmail.com)
```

### Comparing `hspylib-hqt-0.9.2/README.md` & `hspylib-hqt-0.9.3/hspylib_hqt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,40 @@
-# HomeSetup Python Library - HsPyLib
+Metadata-Version: 2.1
+Name: hspylib-hqt
+Version: 0.9.3
+Summary: HsPyLib - QT framework extensions
+Home-page: https://github.com/yorevs/hspylib
+Author: Hugo Saporetti Junior
+Author-email: yorevs@hotmail.com
+License: MIT
+Project-URL: GitHub, https://github.com/yorevs/hspylib
+Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
+Keywords: qt,ui,extensions,application,pyqt
+Platform: Darwin
+Platform: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Natural Language :: English
+Classifier: Topic :: Terminals
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 
-## Your mature python application
+# <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
+
+## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -38,15 +65,15 @@
 
 Create an easy to use and code multiple select or choose input method:
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
 from clitt.core.icons.font_awesome.nav_icons import NavIcons
-from clitt.core.tui.mselect import mselect
+from clitt.core.tui.mselect.mselect import mselect
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class SelectableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -73,15 +100,15 @@
 ```
 
 ![MenuSelect](https://iili.io/HYBFh74.png "MenuSelect")
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
-from clitt.core.tui.mchoose import mchoose
+from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class ChooseableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -287,33 +314,33 @@
 
 To clone HsPyLib into your local machine type the command:
 
 `# git clone https://github.com/yorevs/hspylib.git`
 
 ## Documentation
 
-TBD
+The API documentation can be found [here](docs/api/index.html)
 
 ## Contact
 
 You can contact us using our [Gitter](https://gitter.im/hspylib/community) community or using our
 [Reddit](https://www.reddit.com/user/yorevs).
 
 ## Support HsPyLib
 
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
-[guidelines](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).
+[guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 ## Links
 
-- Documentation: TBD
+- Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
 - Official chat: https://gitter.im/hspylib/community
 - Contact: https://www.reddit.com/user/yorevs
-- Mailto: yorevs@hotmail.com
+- Mailto: [Yorevs](mailto:yorevs@hotmail.com)
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hcombobox.py` & `hspylib-hqt-0.9.3/hqt/promotions/hcombobox.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hcombobox.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from PyQt5.QtWidgets import QComboBox
 
 
 class HComboBox(QComboBox):
     def set_item(self, item: str) -> None:
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hconsole.py` & `hspylib-hqt-0.9.3/hqt/promotions/hconsole.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hconsole.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-from typing import Optional
-
 from PyQt5.QtCore import QRect, QSize, Qt
 from PyQt5.QtGui import QColor, QCursor, QFont, QPainter, QPaintEvent, QPalette, QResizeEvent, QTextCursor, QTextFormat
 from PyQt5.QtWidgets import QPlainTextEdit, QTextEdit, QWidget
+from typing import Optional
 
 
 class HConsole(QPlainTextEdit):
     """TODO"""
 
     class _LineNumberArea(QWidget):
         """TODO"""
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hframe.py` & `hspylib-hqt-0.9.3/hqt/promotions/hframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hframe.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtGui import QKeyEvent
 from PyQt5.QtWidgets import QFrame
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hlabel.py` & `hspylib-hqt-0.9.3/hqt/promotions/hlabel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hlabel.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-from typing import Optional
-
 from PyQt5.QtCore import pyqtSignal, Qt
 from PyQt5.QtGui import QFontMetrics, QMouseEvent, QResizeEvent, QTextDocument
 from PyQt5.QtWidgets import QLabel, QSizePolicy, QWidget
+from typing import Optional
 
 
 class HLabel(QLabel):
     """TODO"""
 
     clicked = pyqtSignal()
     elisionChanged = pyqtSignal()
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hlistwidget.py` & `hspylib-hqt-0.9.3/hqt/promotions/hlistwidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hlistwidget.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-from typing import List, Optional, Union
-
 from hspylib.core.preconditions import check_argument, check_not_none, check_state
 from PyQt5.QtCore import pyqtSignal, QModelIndex, Qt
 from PyQt5.QtGui import QCursor, QKeyEvent
 from PyQt5.QtWidgets import QListWidget, QListWidgetItem, QMenu, QWidget
+from typing import List, Optional, Union
 
 
 class HListWidget(QListWidget):
     """TODO"""
 
     keyPressed = pyqtSignal(int)
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/hstacked_widget.py` & `hspylib-hqt-0.9.3/hqt/promotions/hstacked_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: hspylib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: hstacked_widget.py
    @created: Wed, 8 Jun 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-from typing import List
-
-from PyQt5.QtCore import (
-    pyqtSlot, QAbstractAnimation, QEasingCurve, QParallelAnimationGroup, QPoint, QPropertyAnimation, Qt,
-)
+from PyQt5.QtCore import (pyqtSlot, QAbstractAnimation, QEasingCurve, QParallelAnimationGroup, QPoint,
+                          QPropertyAnimation, Qt)
 from PyQt5.QtWidgets import QStackedWidget, QWidget
+from typing import List
 
 
 class HStackedWidget(QStackedWidget):
     """TODO"""
 
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/htablemodel.py` & `hspylib-hqt-0.9.3/hqt/promotions/htablemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: htablemodel.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-import collections
-from typing import List, Tuple, Type, TypeVar, Union
-
 from hspylib.core.collection_filter import CollectionFilter, FilterCondition
 from hspylib.core.tools.commons import class_attribute_names, class_attribute_values
 from PyQt5.QtCore import QAbstractTableModel, QModelIndex, Qt, QVariant
 from PyQt5.QtGui import QPalette
 from PyQt5.QtWidgets import QTableView
+from typing import List, Tuple, Type, TypeVar, Union
+
+import collections
 
 T = TypeVar("T")
 
 
 class HTableModel(QAbstractTableModel):
     """TODO"""
 
@@ -33,15 +33,14 @@
         parent: QTableView,
         clazz: Type,
         headers: List[str] = None,
         table_data: List[T] = None,
         cell_alignments: List[Qt.AlignmentFlag] = None,
         max_rows: int = 500,
     ):
-
         QAbstractTableModel.__init__(self, parent)
         self._parent = parent
         self._clazz = clazz
         self._data = collections.deque(maxlen=max_rows)
         self._filters = CollectionFilter()
         self._headers = headers or self._headers_by_entity()
         self._cell_alignments = cell_alignments
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/htableview.py` & `hspylib-hqt-0.9.3/hqt/promotions/htableview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: htableview.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import os
-from typing import Callable, Optional
-
-import pyperclip as clipboard
 from hspylib.core.collection_filter import CollectionFilter
 from hspylib.core.preconditions import check_argument, check_not_none, check_state
 from hspylib.core.tools.text_tools import strip_linebreaks
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QCursor, QPainter, QPaintEvent
 from PyQt5.QtWidgets import QAbstractScrollArea, QHeaderView, QMenu, QTableView, QWidget
+from typing import Callable, Optional
+
+import os
+import pyperclip as clipboard
 
 CB_ACTION = Callable[[], None]
 
 
 class HTableView(QTableView):
     """Promoted QTableView widget."""
```

### Comparing `hspylib-hqt-0.9.2/hqt/promotions/htoolbox.py` & `hspylib-hqt-0.9.3/hqt/promotions/htoolbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: hspylib
+   @project: HsPyLib-Hqt
    @package: hqt.promotions
       @file: htoolbox.py
    @created: Fri, 29 Jul 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from functools import cached_property
-
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtProperty, pyqtSignal, pyqtSlot, QObject, Qt, QVariantAnimation
 from PyQt5.QtWidgets import QToolBox
 
 
 class HToolBox(QToolBox):
     """Animated QToolBox
```

### Comparing `hspylib-hqt-0.9.2/hqt/qt_application.py` & `hspylib-hqt-0.9.3/hqt/qt_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt
       @file: qt_application.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import sys
-from pathlib import Path
-from typing import TypeVar
-
 from hspylib.core.preconditions import check_argument, check_state
 from hspylib.core.tools.text_tools import titlecase
 from hspylib.modules.application.application import Application
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
+from pathlib import Path
 from PyQt5.QtGui import QFont, QFontDatabase, QIcon
 from PyQt5.QtWidgets import QApplication
+from typing import TypeVar
+
+import sys
 
 V = TypeVar("V", bound="QWidget")
 
 
 class QtApplication(Application):
     def __init__(
         self,
```

### Comparing `hspylib-hqt-0.9.2/hqt/stream_capturer.py` & `hspylib-hqt-0.9.3/hqt/stream_capturer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt
       @file: stream_capturer.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-import io
-import logging as log
 from contextlib import redirect_stderr, redirect_stdout
-from time import sleep
-
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import is_debugging, syserr
 from PyQt5.QtCore import pyqtSignal, QThread
+from time import sleep
+
+import io
+import logging as log
 
 
 class StreamCapturer(QThread):
     """QThread to captures stdout and/or stderr messages and send them via PyQt Signal"""
 
     stdoutCaptured = pyqtSignal(str)
     stderrCaptured = pyqtSignal(str)
@@ -74,15 +74,14 @@
     def __init__(
         self,
         capture_stderr: bool = True,
         capture_stdout: bool = True,
         stdout_poll_interval: float = 0.5,
         stderr_poll_interval: float = 0.5,
     ):
-
         check_argument(capture_stderr or capture_stdout, "At least one capturer must be started")
         super().__init__()
         self.setObjectName("stream-capturer")
         self._capture_stdout = capture_stdout
         self._capture_stderr = capture_stderr
         self._poll_interval = stdout_poll_interval + stderr_poll_interval
```

### Comparing `hspylib-hqt-0.9.2/hqt/views/main_view.py` & `hspylib-hqt-0.9.3/hqt/views/main_view.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.views
       @file: main_view.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from abc import abstractmethod
-
-from PyQt5 import uic
-
 from hqt.views.qt_view import QtView
+from PyQt5 import uic
 
 
 class MainView(QtView):
     """TODO"""
 
     def __init__(self, ui_file_path: str):
         form, window = uic.loadUiType(ui_file_path)
```

### Comparing `hspylib-hqt-0.9.2/hqt/views/qt_view.py` & `hspylib-hqt-0.9.3/hqt/views/qt_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib
+   @project: HsPyLib-Hqt
    @package: hqt.views
       @file: qt_view.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import os
 from abc import ABC
-from typing import Optional, Tuple, Type
-
 from hspylib.core.preconditions import check_argument, check_state
 from hspylib.core.tools.commons import run_dir
 from PyQt5 import uic
 from PyQt5.QtGui import QFont
 from PyQt5.QtWidgets import QWidget
+from typing import Optional, Tuple, Type
+
+import os
 
 
 class QtView(ABC):
     """TODO"""
 
     MAIN_QT_VIEW_UI = "main_qt_view.ui"
```

### Comparing `hspylib-hqt-0.9.2/hspylib_hqt.egg-info/PKG-INFO` & `hspylib-hqt-0.9.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,13 @@
-Metadata-Version: 2.1
-Name: hspylib-hqt
-Version: 0.9.2
-Summary: HSPyLib - QT framework extensions
-Home-page: https://github.com/yorevs/hspylib
-Author: Hugo Saporetti Junior
-Author-email: yorevs@hotmail.com
-License: MIT
-Project-URL: GitHub, https://github.com/yorevs/hspylib
-Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
-Keywords: qt,ui,extensions,application,pyqt
-Platform: Darwin
-Platform: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Natural Language :: English
-Classifier: Topic :: Terminals
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+# <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
-# HomeSetup Python Library - HsPyLib
-
-## Your mature python application
+## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -65,15 +38,15 @@
 
 Create an easy to use and code multiple select or choose input method:
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
 from clitt.core.icons.font_awesome.nav_icons import NavIcons
-from clitt.core.tui.mselect import mselect
+from clitt.core.tui.mselect.mselect import mselect
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class SelectableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -100,15 +73,15 @@
 ```
 
 ![MenuSelect](https://iili.io/HYBFh74.png "MenuSelect")
 
 ```python
 from hspylib.modules.cli.vt100.vt_color import VtColor
 
-from clitt.core.tui.mchoose import mchoose
+from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.tui_preferences import TUIPreferences
 
 
 class ChooseableItem:
     def __init__(self, name: str, value: str):
         self.name = name
         self.value = value
@@ -314,33 +287,33 @@
 
 To clone HsPyLib into your local machine type the command:
 
 `# git clone https://github.com/yorevs/hspylib.git`
 
 ## Documentation
 
-TBD
+The API documentation can be found [here](docs/api/index.html)
 
 ## Contact
 
 You can contact us using our [Gitter](https://gitter.im/hspylib/community) community or using our
 [Reddit](https://www.reddit.com/user/yorevs).
 
 ## Support HsPyLib
 
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
-[guidelines](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).
+[guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 ## Links
 
-- Documentation: TBD
+- Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
 - Official chat: https://gitter.im/hspylib/community
 - Contact: https://www.reddit.com/user/yorevs
-- Mailto: yorevs@hotmail.com
+- Mailto: [Yorevs](mailto:yorevs@hotmail.com)
```

### Comparing `hspylib-hqt-0.9.2/hspylib_hqt.egg-info/SOURCES.txt` & `hspylib-hqt-0.9.3/hspylib_hqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.2/setup.py` & `hspylib-hqt-0.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Hqt
+   @project: HsPyLib-Hqt
       @file: setup.py
    @created: Tue, 18 Apr 2023
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 
    Reference: https://setuptools.pypa.io/en/latest/references/keywords.html
 """
 
 import pathlib
-
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
@@ -29,15 +28,15 @@
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name="hspylib-hqt",
     version=VERSION,
-    description="HSPyLib - QT framework extensions",
+    description="HsPyLib - QT framework extensions",
     author="Hugo Saporetti Junior",
     author_email="yorevs@hotmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
     project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-hqt/"},
     license="MIT",
```

