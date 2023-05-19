# Comparing `tmp/feedfilter-1.0.3.tar.gz` & `tmp/feedfilter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedfilter-1.0.3.tar", max compression
+gzip compressed data, was "feedfilter-1.1.0.tar", max compression
```

## Comparing `feedfilter-1.0.3.tar` & `feedfilter-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35150 2022-12-31 23:31:41.428384 feedfilter-1.0.3/LICENSE
--rw-r--r--   0        0        0     4210 2023-01-09 13:25:32.157093 feedfilter-1.0.3/README.md
--rw-r--r--   0        0        0      932 2023-05-15 11:36:15.557204 feedfilter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      359 2022-12-31 23:41:18.220255 feedfilter-1.0.3/src/feedfilter/__init__.py
--rwxr-xr-x   0        0        0    13806 2023-05-15 11:56:42.820107 feedfilter-1.0.3/src/feedfilter/feed_filter.py
--rw-r--r--   0        0        0     3254 2022-12-31 23:41:17.808252 feedfilter-1.0.3/src/feedfilter/logger.py
--rw-r--r--   0        0        0     5098 1970-01-01 00:00:00.000000 feedfilter-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35150 2022-12-31 23:31:41.428384 feedfilter-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5946 2023-05-18 19:14:52.420783 feedfilter-1.1.0/README.md
+-rw-r--r--   0        0        0      986 2023-05-18 18:49:10.286057 feedfilter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-05-18 17:04:39.960374 feedfilter-1.1.0/src/feedfilter/__init__.py
+-rwxr-xr-x   0        0        0    16121 2023-05-18 19:18:07.494345 feedfilter-1.1.0/src/feedfilter/feed_filter.py
+-rw-r--r--   0        0        0     3254 2022-12-31 23:41:17.808252 feedfilter-1.1.0/src/feedfilter/logger.py
+-rw-r--r--   0        0        0     6930 1970-01-01 00:00:00.000000 feedfilter-1.1.0/PKG-INFO
```

### Comparing `feedfilter-1.0.3/LICENSE` & `feedfilter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feedfilter-1.0.3/README.md` & `feedfilter-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 primary sort and secondary sort fields.
 
 feed-filter can also optionaly make some modification to the content
 such as converting URLs into links.
 
 ## Options
 
+### --config-file
+
+Override the default location of the config file.  Because the config file
+if optional, if the specified files does not exits, it will be silently ignored.
+
+### --name (-n)
+
+Section name in config file to use.  If not specified, only the [DEFAULT]
+section will apply.  See Configuration File.
+
 ### --title-re and --title-sub
 
 The --title-re option specifies a regular expression.  And the --title-sub option can use backrefferences to the RE in --title-re.
 
 So for example, if you have the following options
 > --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\3'
 
@@ -40,40 +50,42 @@
 Modified title:
 > Tutorials and videos • Part design Tutorials and much more ...
 
 Either of the above two examples can be helpfull for modifying a feed
 for a forum so that you can sort the entries by title (headline) so
 all posts and their responses are groups together.
 
-### --add-date-to-title
+The regular expression systax used is that of python's regular expressions.
+
+### --add-date-to-title (--no-add-date-to-title)
 
 Just grouping all related posts together is helpfull, but you probably
 want to display them in the order they were created.  If you happen to
 have a feed reader that can sort on titles with a secondary sort on
 the date, then you are all set.  But if you can only do one sort
 (title), the posts may be in the wrong order.  This is where the
 --add-date-to-title option comes in.
 
 It does pretty much what it says.  It appends the posting's date to
 the end of the title after a bunch of spaces.  All the spaces are just
 to hide the date string.  The date aids in sorting.  Now when you sort
 on the title, the entries will implicitly have a secondary sort on the
 date due to its inclusion in the titles.
 
-### --add-posts
+### --add-posts (--no-add-posts)
 
 For each entry, it attempts to download a topic-specific rss or atom
 feed and adds each entry in place of the original entry.  This is
 usefull for sites whos forum feed only shows the topics (first post)
 and not any replies.  Note that this option won't work on many sites
 due to having to parse web pages.  Raise issue for any site that
 doesn't seem to work.  Titles on additional posts fetched will all
 be taken from the original entry.
 
-### --auto-links
+### --auto-links (--no-auto-links)
 
 In the content sections, anything that looks like a URL but is not already
 an HTML link, will be made into a link.
 
 ### --output-fmt
 
 Value can be either 'atom' (default), 'rss', or 'summary'.  The
@@ -82,17 +94,51 @@
 
 ### Others
 
 Run feed-filter with the --help option to see what other options
 are available.
 
 
+## Configuration File
+
+This program can optionally use a configuration file so you don't have
+to specify lots of options on the command line.  The default location
+for the configuration files is _${XDG_CONFIG_HOME}/feed-filter.conf_.
+If _${XDG_CONFIG_HOME}_ is not set, the default value as specified in
+the [XDG Base Directory Specification will be used](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).
+
+The configuration file is an INI style file.  The section to use is
+specified via the --name option.  This can ge used to group options
+for specific feeds or groups of feed (perhaps from a common site)
+together.  If there is a [DEFAULT] section, any value in that section
+will be used as a default value for whatever named section is actually
+specified (--name).  If --name is not specified, only the [DEFAULT]
+section will be used.
+
+For supported options (see --help output) just use the long option
+name without the '--' prefix, an '=' and then the value.  For boolean
+type options, use True or False as the options value.  e.g.
+
+```
+   [DEFAULT]
+   auto-links = True
+
+   [mysection]
+   date-spaces = 220
+   auto-links = False
+```
+
+Caution, there is only limited checking for valid values.  Specifying
+an invalid option will be silently ignored.
+
+
 # Installation
 
-This [package](https://pypi.org/project/feedfilter/) is on [PyPI.org](https://pypi.org/), so just install with pip or pipx like
+This [package](https://pypi.org/project/feedfilter/) is on
+[PyPI.org](https://pypi.org/), so just install with pip or pipx like
 
 ```
 pipx install feedfilter
 ```
 
 # Development setup
```

### Comparing `feedfilter-1.0.3/pyproject.toml` & `feedfilter-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # For how poetry is configured with this file, see
 # https://python-poetry.org/docs/pyproject/
 
 
 [tool.poetry]
 name = "feedfilter"
-version = "1.0.3"
+version = "1.1.0"
 description = "Modify RSS/Atom feeds"
 authors = ["Jim Bauer"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 #homepage = "url-to-homepage"
 repository = "https://gitlab.com/jim_bauer/feed-filter"
 #documentation = "url-to-documentation"
@@ -23,21 +23,23 @@
 
 [tool.poetry.scripts]
 feed-filter = "feedfilter:main"
 
 
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.10,<4.0"
 feedparser = "^6.0.10"
 feedgen = "^0.9.0"
 pytz = ">=2022.6"
 bs4 = "^0.0.1"
 requests = "^2.28.1"
 sgmllib3k = "^1.0.0"
+configparser = "^5.3.0"
+xdg-base-dirs = "^6.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 flake8 = ">=6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `feedfilter-1.0.3/src/feedfilter/feed_filter.py` & `feedfilter-1.1.0/src/feedfilter/feed_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #
-# Copyright (c) 2022 Jim Bauer <4985656-jim_bauer@users.noreply.gitlab.com>
+# Copyright (c) 2022-2023 Jim Bauer <4985656-jim_bauer@users.noreply.gitlab.com>
 # This software is licensed according to the included LICENSE file
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import sys
 import re
 import argparse
+import configparser
 import datetime
 from pytz import timezone
 from pathlib import Path
 import traceback
 import requests
 import contextlib
 import html
@@ -21,14 +22,17 @@
 
 # https://feedgen.kiesow.be/
 from feedgen.feed import FeedGenerator
 
 # https://beautiful-soup-4.readthedocs.io/en/latest/
 from bs4 import BeautifulSoup
 
+# https://pypi.org/project/xdg-base-dirs/
+from xdg_base_dirs import xdg_config_home
+
 # Local imports
 import feedfilter.logger as logger
 from feedfilter import __version__ as __version__
 
 
 @contextlib.contextmanager
 def open_file_or_stdio(fname: str, mode: str = 'r', *args, **kwargs):
@@ -317,48 +321,80 @@
 
         fe.title(mt.mangle(title, title_date))
 
 
 def feed_filter():
     prog_name = Path(sys.argv[0]).name
 
+    conf_parser = argparse.ArgumentParser(
+        description=__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        add_help=False
+    )
+    conf_loc = f'{xdg_config_home()}/feed-filter.conf'
+    conf_parser.add_argument('--config-file',
+                             default=conf_loc,
+                             help=f'Specify config file (default={conf_loc})',
+                             metavar='FILE')
+    conf_parser.add_argument('-n', '--name',
+                             default='DEFAULT',
+                             help='Use name section in config file')
+    args, rest_argv = conf_parser.parse_known_args()
+    name = args.name
+
+    if args.config_file:
+        cfg = configparser.ConfigParser()
+        cfg.read([args.config_file])
+
     # Default regex\n
     # - <prefix> is typically a forum name\n
     # - Re: is added to responses automatically
     # - <brackets> is often something like "[solved]" added to be
     #   the title to denote that the issue have been resolved
     # - <main> Main part of the title
     reg = r'(?P<prefix>[^•]+ • )?(Re: )?(?P<brackets>\[[^]]+] ?)?(?P<main>.*)'
     sub = r'\g<prefix>\g<main>'
 
     p = argparse.ArgumentParser(description='Filter RSS/Atom feeds',
+                                parents=[conf_parser],
                                 add_help=False)
     p.add_argument('-h', '--help', action='store_true',
                    help='show this help message and exit')
     logger.add_argparse_args(p)
     p.add_argument('--forum', help='Forum URL or input filename')
     p.add_argument('--outfile', default=None,
                    help='Output file (default: stdout)')
-    p.add_argument('--output-fmt', default='atom',
+    p.add_argument('--output-fmt',
+                   default=cfg.get(name, 'output-fmt', fallback='atom'),
                    choices=['atom', 'rss', 'summary'],
                    help='format of feed output (default: atom)')
-    p.add_argument('--title-re', default=reg,
+    p.add_argument('--title-re',
+                   default=cfg.get(name, 'title-re', fallback=reg),
                    help='python regex used to match titles')
-    p.add_argument('--title-sub', default=sub,
+    p.add_argument('--title-sub',
+                   default=cfg.get(name, 'title-sub', fallback=sub),
                    help='python regex subsitution')
-    p.add_argument('--add-date-to-title', default='yes',
-                   choices=['yes', 'no'],
+    p.add_argument('--add-date-to-title',
+                   action=argparse.BooleanOptionalAction,
+                   default=cfg.getboolean(name, 'add-date-to-title',
+                                          fallback=True),
                    help='add date/time string to entry title (for sorting)')
-    p.add_argument('--date_spaces', type=int, default=200,
+    p.add_argument('--date_spaces', type=int,
+                   default=cfg.getint(name, 'date-spaces', fallback=200),
+                   metavar='NUMBER_SPACES',
                    help='number of spaces to insert before date for --add-date-to-title')
-    p.add_argument('--add-posts', action='store_true',
+    p.add_argument('--add-posts',
+                   action=argparse.BooleanOptionalAction,
+                   default=cfg.getboolean(name, 'add-posts', fallback=False),
                    help='Add posts made to this topic '
                    '(requires network access)')
-    p.add_argument('--auto-links', action='store_true',
-                   help='Automatically add links for test that looks like URLs')
+    p.add_argument('--auto-links',
+                   action=argparse.BooleanOptionalAction,
+                   default=cfg.getboolean(name, 'auto-links', fallback=False),
+                   help='Automatically add links for text that looks like URLs')
     p.add_argument('--version', action='store_true',
                    help='display version and exit')
 
     args = p.parse_args()
 
     if args.help:
         p.print_help()
@@ -379,14 +415,34 @@
   Option --title-sub:
     - Default: {sub}
     - Replaces matched title with prefix followed by main part of title
       i.e. Removes "Re: " and most things between '[' and ']'
     - To reference any of: <prefix> <brackets> or <main> in title subsitution
       specify tham as \\g<name> (i.e. \\g<prefix>)
 
+  Option --config-file
+    - If file is not found, it is silently ignored
+
+Configuration file:
+
+  An optional configuration file can be used for many options.  It is an
+  ini style file (parsed by python's configparser module).  The section
+  name to use is given by the --name option, with [DEFAULT] (all caps)
+  section being used for default values.
+
+  Supported options in config file (with their default values):
+    - output-fmt = atom
+    - title-re = (?P<prefix>[^•]+ • )?(Re: )?(?P<brackets>\[[^]]+] ?)?(?P<main>.*)
+    - title-sub = \g<prefix>\g<main>
+    - add-date-to-title = True
+    - date-spaces = 200
+    - add-posts = False
+    - auto-links = False
+
+  Commandline options will override any specified in the config file.
 ''')
         sys.exit(0)
 
     if args.version:
         print(f'{prog_name} {__version__}')
         sys.exit(0)
```

### Comparing `feedfilter-1.0.3/src/feedfilter/logger.py` & `feedfilter-1.1.0/src/feedfilter/logger.py`

 * *Files identical despite different names*

### Comparing `feedfilter-1.0.3/PKG-INFO` & `feedfilter-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: feedfilter
-Version: 1.0.3
+Version: 1.1.0
 Summary: Modify RSS/Atom feeds
 Home-page: https://gitlab.com/jim_bauer/feed-filter
 License: GPL-3.0-or-later
 Keywords: rss,atom
 Author: Jim Bauer
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: feedgen (>=0.9.0,<0.10.0)
 Requires-Dist: feedparser (>=6.0.10,<7.0.0)
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sgmllib3k (>=1.0.0,<2.0.0)
+Requires-Dist: xdg-base-dirs (>=6.0.0,<7.0.0)
 Project-URL: Repository, https://gitlab.com/jim_bauer/feed-filter
 Description-Content-Type: text/markdown
 
 # feed-filter
 
 Filter for modifying feed data.  By default, reads feed from stdin and writes a
 modified feed to stdout in either Atom (default) or RSS format.
@@ -33,14 +35,24 @@
 primary sort and secondary sort fields.
 
 feed-filter can also optionaly make some modification to the content
 such as converting URLs into links.
 
 ## Options
 
+### --config-file
+
+Override the default location of the config file.  Because the config file
+if optional, if the specified files does not exits, it will be silently ignored.
+
+### --name (-n)
+
+Section name in config file to use.  If not specified, only the [DEFAULT]
+section will apply.  See Configuration File.
+
 ### --title-re and --title-sub
 
 The --title-re option specifies a regular expression.  And the --title-sub option can use backrefferences to the RE in --title-re.
 
 So for example, if you have the following options
 > --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\3'
 
@@ -64,40 +76,42 @@
 Modified title:
 > Tutorials and videos • Part design Tutorials and much more ...
 
 Either of the above two examples can be helpfull for modifying a feed
 for a forum so that you can sort the entries by title (headline) so
 all posts and their responses are groups together.
 
-### --add-date-to-title
+The regular expression systax used is that of python's regular expressions.
+
+### --add-date-to-title (--no-add-date-to-title)
 
 Just grouping all related posts together is helpfull, but you probably
 want to display them in the order they were created.  If you happen to
 have a feed reader that can sort on titles with a secondary sort on
 the date, then you are all set.  But if you can only do one sort
 (title), the posts may be in the wrong order.  This is where the
 --add-date-to-title option comes in.
 
 It does pretty much what it says.  It appends the posting's date to
 the end of the title after a bunch of spaces.  All the spaces are just
 to hide the date string.  The date aids in sorting.  Now when you sort
 on the title, the entries will implicitly have a secondary sort on the
 date due to its inclusion in the titles.
 
-### --add-posts
+### --add-posts (--no-add-posts)
 
 For each entry, it attempts to download a topic-specific rss or atom
 feed and adds each entry in place of the original entry.  This is
 usefull for sites whos forum feed only shows the topics (first post)
 and not any replies.  Note that this option won't work on many sites
 due to having to parse web pages.  Raise issue for any site that
 doesn't seem to work.  Titles on additional posts fetched will all
 be taken from the original entry.
 
-### --auto-links
+### --auto-links (--no-auto-links)
 
 In the content sections, anything that looks like a URL but is not already
 an HTML link, will be made into a link.
 
 ### --output-fmt
 
 Value can be either 'atom' (default), 'rss', or 'summary'.  The
@@ -106,17 +120,51 @@
 
 ### Others
 
 Run feed-filter with the --help option to see what other options
 are available.
 
 
+## Configuration File
+
+This program can optionally use a configuration file so you don't have
+to specify lots of options on the command line.  The default location
+for the configuration files is _${XDG_CONFIG_HOME}/feed-filter.conf_.
+If _${XDG_CONFIG_HOME}_ is not set, the default value as specified in
+the [XDG Base Directory Specification will be used](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).
+
+The configuration file is an INI style file.  The section to use is
+specified via the --name option.  This can ge used to group options
+for specific feeds or groups of feed (perhaps from a common site)
+together.  If there is a [DEFAULT] section, any value in that section
+will be used as a default value for whatever named section is actually
+specified (--name).  If --name is not specified, only the [DEFAULT]
+section will be used.
+
+For supported options (see --help output) just use the long option
+name without the '--' prefix, an '=' and then the value.  For boolean
+type options, use True or False as the options value.  e.g.
+
+```
+   [DEFAULT]
+   auto-links = True
+
+   [mysection]
+   date-spaces = 220
+   auto-links = False
+```
+
+Caution, there is only limited checking for valid values.  Specifying
+an invalid option will be silently ignored.
+
+
 # Installation
 
-This [package](https://pypi.org/project/feedfilter/) is on [PyPI.org](https://pypi.org/), so just install with pip or pipx like
+This [package](https://pypi.org/project/feedfilter/) is on
+[PyPI.org](https://pypi.org/), so just install with pip or pipx like
 
 ```
 pipx install feedfilter
 ```
 
 # Development setup
```

