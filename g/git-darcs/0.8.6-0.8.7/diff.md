# Comparing `tmp/git_darcs-0.8.6.tar.gz` & `tmp/git_darcs-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_darcs-0.8.6.tar", max compression
+gzip compressed data, was "git_darcs-0.8.7.tar", max compression
```

## Comparing `git_darcs-0.8.6.tar` & `git_darcs-0.8.7.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    34523 2022-12-15 04:56:03.339252 git_darcs-0.8.6/LICENSE
--rw-r--r--   0        0        0    13060 2022-12-20 15:01:39.100504 git_darcs-0.8.6/README.md
--rw-r--r--   0        0        0    26531 2022-12-20 14:32:31.222792 git_darcs-0.8.6/git_darcs.py
--rw-r--r--   0        0        0     1255 2022-12-20 15:03:29.923736 git_darcs-0.8.6/pyproject.toml
--rw-r--r--   0        0        0    14364 1970-01-01 00:00:00.000000 git_darcs-0.8.6/setup.py
--rw-r--r--   0        0        0    14223 1970-01-01 00:00:00.000000 git_darcs-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-12-15 04:56:03.339252 git_darcs-0.8.7/LICENSE
+-rw-r--r--   0        0        0    13062 2022-12-20 15:11:00.476877 git_darcs-0.8.7/README.md
+-rw-r--r--   0        0        0    26970 2023-05-19 18:26:24.758132 git_darcs-0.8.7/git_darcs.py
+-rw-r--r--   0        0        0     1255 2023-05-19 18:28:44.065711 git_darcs-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0    14225 1970-01-01 00:00:00.000000 git_darcs-0.8.7/PKG-INFO
```

### Comparing `git_darcs-0.8.6/LICENSE` & `git_darcs-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `git_darcs-0.8.6/README.md` & `git_darcs-0.8.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 [git-darcs on pypi](https://pypi.org/project/git-darcs/)
 
 - [Warning](#-warning)
 - [Install](#Install)
 - [Use-cases](#use-cases)
   * [Main use-case](#main-use-case)
   * [Other use-case](#other-use-case)
+  * [But why?](#but-why)
 - [Tutorial](#Tutorial)
-- [But why?](#but-why)
 - [For darcs beginners](#for-darcs-beginners)
 - [Caveats](#caveats)
   * [Performance](#performance)
   * [chmod and symbolic-links](#chmod-and-symbolic-links)
   * [Linearized History](#linearized-history)
 - [Usage](#usage)
 
@@ -56,14 +56,24 @@
 Other use-cases
 ---------------
 
 * Convert a git repository to darcs using the [linearized history](#linearized-history)
   proposed by git-darcs
 * Visualize a git-repository using `darcs show dependencies`
 
+But why?
+--------
+
+I prefer to group changes by topic, so I am constantly amending commits/patches.
+This is very easy in darcs and more complicated in git. Yes, I know about
+`--fixup` and `--autosquash` in git. Also I can find independent low-risk
+patches easily with `darcs show dependencies`, so I can constantly make MRs.
+Making the final _breaking_ change/MR much smaller. This is less tedious for the
+reviewers.
+
 Tutorial
 ========
 
 The tutorial covers the main use-case:
 
 1. Check-out a git-repo, because at work you have to use git
 2. Snapshot the latest commit into darcs
@@ -256,24 +266,14 @@
 ```
 
 ```bash
 $> cd ..
 $> rm -r dms-stage
 ```
 
-But why?
-========
-
-I prefer to group changes by topic, so I am constantly amending commits/patches.
-This is very easy in darcs and more complicated in git. Yes, I know about
-`--fixup` and `--autosquash` in git. Also I can find independent low-risk
-patches easily with `darcs show dependencies`, so I can constantly make MRs.
-Making the final _breaking_ change/MR much smaller. This is less tedious for the
-reviewers.
-
 For darcs beginners
 ===================
 
 * There is a great [video](https://hikari.acmelabs.space/videos/hikari-darcs.mp4) by
   [raichoo](https://hub.darcs.net/raichoo) the maintainer of
   [hikari](https://hikari.acmelabs.space/)
 * You have to read the [darcs book](https://darcsbook.acmelabs.space/), you just
```

### Comparing `git_darcs-0.8.6/git_darcs.py` & `git_darcs-0.8.7/git_darcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,28 @@
             "--no-merges",
             f"{base}..{head}",
         ],
         stdout=PIPE,
     ) as res:
         while line := res.stdout.readline():
             yield line.decode("UTF-8").strip()
-
+        else:
+            with Popen(
+                [
+                    "git",
+                    "rev-list",
+                    "--reverse",
+                    "--topo-order",
+                    "--ancestry-path",
+                    f"{base}..{head}",
+                ],
+                stdout=PIPE,
+            ) as res:
+                while line := res.stdout.readline():
+                    yield line.decode("UTF-8").strip()
 
 def get_base():
     """Get the root/base commit from git."""
     base = (
         run(
             ["git", "rev-list", "--max-parents=0", "HEAD"],
             check=True,
```

### Comparing `git_darcs-0.8.6/pyproject.toml` & `git_darcs-0.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-darcs"
-version = "0.8.6"
+version = "0.8.7"
 description = " Incremental import of git into darcs and back again"
 authors = ["Jean-Louis Fuchs <jean-louis.fuchs@adfinis.com>"]
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/ganwell/git-darcs"
 repository = "https://github.com/ganwell/git-darcs"
 keywords = ["git", "darcs", "import", "incremental"]
 readme = "README.md"
```

### Comparing `git_darcs-0.8.6/setup.py` & `git_darcs-0.8.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,461 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: git-darcs
+Version: 0.8.7
+Summary:  Incremental import of git into darcs and back again
+Home-page: https://github.com/ganwell/git-darcs
+License: AGPL-3.0-or-later
+Keywords: git,darcs,import,incremental
+Author: Jean-Louis Fuchs
+Author-email: jean-louis.fuchs@adfinis.com
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Version Control
+Requires-Dist: Flake8-pyproject (>=1.1.0.post0,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: colorama (>=0.4.5,<0.5.0)
+Requires-Dist: readchar (>=4.0.3,<5.0.0)
+Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Project-URL: Repository, https://github.com/ganwell/git-darcs
+Description-Content-Type: text/markdown
 
-modules = \
-['git_darcs']
-install_requires = \
-['Flake8-pyproject>=1.1.0.post0,<2.0.0',
- 'click>=8.1.3,<9.0.0',
- 'colorama>=0.4.5,<0.5.0',
- 'readchar>=4.0.3,<5.0.0',
- 'tqdm>=4.64.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['git-darcs = git_darcs:main']}
-
-setup_kwargs = {
-    'name': 'git-darcs',
-    'version': '0.8.6',
-    'description': ' Incremental import of git into darcs and back again',
-    'long_description': 'Incremental import of git into darcs and back again\n====================================================\n\n[![Test](https://github.com/ganwell/git-darcs/actions/workflows/test.yml/badge.svg)](https://github.com/ganwell/git-darcs/actions/workflows/test.yml) [![CodeQL](https://github.com/ganwell/git-darcs/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ganwell/git-darcs/actions/workflows/codeql-analysis.yml)\n\n[git-darcs on pypi](https://pypi.org/project/git-darcs/)\n\n- [Warning](#-warning)\n- [Install](#Install)\n- [Use-cases](#use-cases)\n  * [Main use-case](#main-use-case)\n  * [Other use-case](#other-use-case)\n- [Tutorial](#Tutorial)\n- [But why?](#but-why)\n- [For darcs beginners](#for-darcs-beginners)\n- [Caveats](#caveats)\n  * [Performance](#performance)\n  * [chmod and symbolic-links](#chmod-and-symbolic-links)\n  * [Linearized History](#linearized-history)\n- [Usage](#usage)\n\n⚠ Warning\n=========\n\ngit-darcs needs a repository only for tracking. Don\'t use your working\ngit-repository. git-darcs will clear all your work that is not commited. It also\nneeds to temporarily change `.gitignore` and `_darcs/pref/boring`. By default it\nwill warn about this. You can add `-nw` to avoid the warning. The tutorial never\ncontains a `-nw`, so people don\'t copy-paste from the tutorial and lose their\nwork.\n\nThe tool is made for developers, while error-handling is okayish, there is\nalmost no error-reporting, you\'ll have to read the traceback.\n\n![demo](https://github.com/ganwell/git-darcs/blob/main/demo.gif?raw=true)\n\nInstall\n=======\n\nIntegration tests run on python 3.7 - 3.11.\n\n```bash\npip install git-darcs\n```\n\nUse-cases\n=========\n\nMain use-case\n-------------\n\nUse the excellent capabilities of darcs to craft consistent, clear and concise\npatches while the remote repository still remains git. Thats the situation most\nof us in are because at work we have to use git.\n\nOther use-cases\n---------------\n\n* Convert a git repository to darcs using the [linearized history](#linearized-history)\n  proposed by git-darcs\n* Visualize a git-repository using `darcs show dependencies`\n\nTutorial\n========\n\nThe tutorial covers the main use-case:\n\n1. Check-out a git-repo, because at work you have to use git\n2. Snapshot the latest commit into darcs\n3. Craft patches: Use the excellent capabilities of darcs to move code between\n   patches to create very consistent and clean patches\n4. Use `git darcs pull` to bring the darcs-patches back into git and\n   create pull-request\n\nClone your tracking-repository.\n\n```bash\n$> git clone https://github.com/adfinis-sygroup/document-merge-service.git dms-track\nCloning into \'document-merge-service\'...\n\n.....\n\nResolving deltas: 100% (1267/1267), done.\n```\n\nLazily import the git-repository to darcs.\n\n```bash\n$> git darcs update\nUse CTRL-D for a graceful shutdown.\n```\n\ngit-darcs will import the latest commit and tag it, so it can update from there,\nwhen you pull commits from upstream.\n\n```bash\n$> (cd dms-track; darcs log)\npatch 7997a3365da1022db4b669ea63a37dc3f370a225\nAuthor: Jean-Louis Fuchs <email>\nDate:   Fri Oct  7 17:40:10 CEST 2022\n  tagged git-checkpoint 2022-10-07T17:40:10.963827\nd3ce714f2d77897e773e89ee3344602fceb1b625\n\npatch 4e917fcc769b7a69858e0b11e7ee5aaffc76fbda\nAuthor: Jean-Louis Fuchs <email>\nDate:   Fri Oct  7 17:40:10 CEST 2022\n  * d3ce714 chore(release): v5.0.0\n```\n\nCreate the work-repository. Note that git and darcs make sure that no historical\ndata is duplicated on disk (using hardlinks).\n\n```bash\n$> git darcs clone dms-track/ dms-work\nclone: 100%|████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.75it/s]\n```\n\nNow you can implement a new feature.\n\n```bash\n$> cd dms-work\n$> touch document_merge_service/feature.py\n$> darcs add document_merge_service/feature.py\nAdding \'./document_merge_service/feature.py\'\nFinished adding:\n./document_merge_service/feature.py\n\n$> darcs record -m "a new feature"\naddfile ./document_merge_service/feature.py\nShall I record this change? (1/1)  [ynW...], or ? for more options: y\nDo you want to Record these changes? [Yglqk...], or ? for more options: y\nFinished recording patch \'a new feature\'\n```\n\n```bash\ndarcs show dependencies | dot -Tpdf -Grankdir=TB -o $ftmp\n```\n\n![first record](https://github.com/ganwell/git-darcs/blob/main/_static/first.png?raw=true)\n\nThere are new changes on upstream, let\'s pull them in.\n\n```bash\n$> cd ../dms-track/\n$> git pull\nUpdating d3ce714..a6a8e35\nFast-forward\n .github/workflows/tests.yml                         |  6 ++++-\n \n.....\n \n 18 files changed, 262 insertions(+), 67 deletions(-)\n```\n\nFrom now on git-darcs will import every commit, but with a linearized\nhistory. That means the history might look different than in git, but no change will be\nforgotten. (See [Linearized History](#linearized-history))\n\n```bash\n$> git darcs update\nUse CTRL-D for a graceful shutdown.\ncommits:\n100%|███████████████████████████████████████████████████████| 18/18 [00:00<00:00, 19.14it/s]\n```\n\nWe pull the new patches into `dms-work`.\n\n```bash\n$> cd ../dms-track/\n$> darcs pull ../dms-track/\nPulling from "/home/jeanlf/Temp/dms-track"...\npatch 309682700e7142e37945c45cc3375674012e8050\nAuthor: GitHub <noreply@github.com>\nDate:   Fri Oct  7 18:07:08 CEST 2022\n  * 85892f6 fix(docker): fix docker uwsgi command\nShall I pull this patch? (1/19)  [ynW...], or ? for more options: a\nFinished pulling.\n```\n\nThe 18 patches we pulled are now in `dms-work` along with a new snapshot-tag.\n\n```bash\n$> darcs log --from-tag=.\npatch 430136524b02be562fdf0f0459594ffa981d386b\nAuthor: Jean-Louis Fuchs <email>\nDate:   Fri Oct  7 18:07:09 CEST 2022\n  tagged git-checkpoint 2022-10-07T18:07:09.041126 a6a8e35ae3c3b42b04837a75ff59aa092130f326\n\npatch ef1f2894abd21d0deef19090d4b873bf62af890a\nAuthor: Jean-Louis Fuchs <email>\nDate:   Fri Oct  7 17:55:22 CEST 2022\n  * a new feature\n```\n\nWe can now either pull the `a new feature`-patch into `dms-track` or we can\ncreate a temporary `dms-stage` so it is easier to clean up after the\nmerge-request has been accepted. Note `git-darcs clone` will copy git-remotes\nfrom the source, so you can push into your fork if it is set up.\n\nIf you pull into `dms-track` instead, you have to remove patches or commits on\nboth darcs and git, keeping darcs and git manually in sync.\n\n\n```bash\n$> cd ..\n$> git darcs clone dms-track/ dms-stage\nclone: 100%|████████████████████████████████████████████████| 5/5 [00:00<00:00, 48.32it/s]\n$> cd dms-stage\n```\n\n`git-darcs pull` tries to emulate `darcs pull`.\n\n```bash\n$> git darcs pull ../dms-work/\npatch ef1f2894abd21d0deef19090d4b873bf62af890a\nAuthor: Jean-Louis Fuchs <email>\nDate: 2022-10-07 15:55:22\nSubject: a new feature\nShall I pull this patch? 1/1  [ynwasc], or ? for more options: ?\n\ny: pull this patch\nn: don\'t pull it\nw: decide later\n\na: pull all remaining patches\ni: don\'t pull remaining patches\n\nl: show full log message\nf: show full patch\n\n?: help\nh: help\n\nc: cancel without pulling\nq: cancel without pulling\n\nShall I pull this patch? 1/1  [ynwasc], or ? for more options: y\nresolve: 0it [00:00, ?it/s]\nShall I pull 1 patches?   [yn], or ? for more options: y\npull: 100%|█████████████████████████████████████████████████| 1/1 [00:00<00:00,  2.58it/s]\n```\n\nThe patch `a new feature` is now a git-commit.\n\n```bash\n$> git show\ncommit c2541c6c3527d99a7fe69dc43b5863992d919a45 (HEAD -> main)\nAuthor: Jean-Louis Fuchs <email>\nDate:   Fri Oct 7 20:01:22 2022 +0200\n\n    a new feature\n\ndiff --git a/document_merge_service/feature.py b/document_merge_service/feature.py\nnew file mode 100644\nindex 0000000..e69de29\n```\n\n```bash\n$> cd ..\n$> rm -r dms-stage\n```\n\nBut why?\n========\n\nI prefer to group changes by topic, so I am constantly amending commits/patches.\nThis is very easy in darcs and more complicated in git. Yes, I know about\n`--fixup` and `--autosquash` in git. Also I can find independent low-risk\npatches easily with `darcs show dependencies`, so I can constantly make MRs.\nMaking the final _breaking_ change/MR much smaller. This is less tedious for the\nreviewers.\n\nFor darcs beginners\n===================\n\n* There is a great [video](https://hikari.acmelabs.space/videos/hikari-darcs.mp4) by\n  [raichoo](https://hub.darcs.net/raichoo) the maintainer of\n  [hikari](https://hikari.acmelabs.space/)\n* You have to read the [darcs book](https://darcsbook.acmelabs.space/), you just\n  have to\n* `_darcs/pref/boring` is the equivalent of `.gitignore`, but has quite a wide\n  definition of boring by default\n\nCaveats\n=======\n\nPerformance\n-----------\n\ngit-darcs will playback the history of the git-repository. Every commit that is\nrecorded will first be checked out in git and then recorded in darcs. For that reason\ngit-darcs lazily imports the latest commit by default. This is how it is meant\nto be used: Using darcs to complement git. You can use it to convert\nrepositories, if you like the way non-linear history is handled, it will be\nsloooow. See also `darcs convert import`.\n\nchmod and symbolic links\n------------------------\n\nDarcs does not handle `chmod` or symbolic links. The easiest way to work around\nthis is by  letting `git` do the work. Since I always make git-commits from the\ndarcs-patches `git` will track `chmod` and symbolic links for me.\n\nLinearized History\n------------------\n\ngit-darcs will traverse the git-history in topological order. For every commit\nit encounters, it will test if the previous commit was an ancestor, if not it\nwill ignore that commit for now. That way git-darcs can only "enter" one branch\nof parallel history. Once it reaches a commit that is an ancestor it will import\nthat commit and log the complete history between it and the last successful\ncommit. So git-darcs creates patches that combine the complete history of a\nparallel branch.\n\nThis git-log\n\n```\n$> git log --oneline --graph\n* eef24d8 (HEAD -> master) end > end0\n* 841c900 end\n*   969ad57 Merge branch \'b\'\n|\\\n| * 76ca538 (b) bb2 > bb3\n| * 0040cee bb1 > bb2\n* | 663168a antiforward > antiforward0\n* |   0d94733 Merge branch \'a\'\n|\\ \\\n| * | d26d325 (a) aa2 > aa3\n| * | 8090696 aa1 > aa2\n| |/\n* / fa7accb antiforward\n|/\n* 7bc2b76 aa0 > aa1, bb0 > bb1\n* 665937d aa > aa0, bb bb0\n* 1fd0236 aa, bb\n```\n\nbecomes this darcs-log\n\n```\n* eef24d8 end > end0\n    move ./end ./end0\n* 841c900 end\n    addfile ./end\n* 969ad57 Merge branch \'b\'\n  76ca538 bb2 > bb3\n  0040cee bb1 > bb2\n    move ./bb1 ./bb3\n* 663168a antiforward > antiforward0\n    move ./antiforward ./antiforward0\n* 0d94733 Merge branch \'a\'\n  d26d325 aa2 > aa3\n  8090696 aa1 > aa2\n    move ./aa1 ./aa3\n* fa7accb antiforward\n    addfile ./antiforward\n* 7bc2b76 aa0 > aa1, bb0 > bb1\n    move ./aa0 ./aa1\n    move ./bb0 ./bb1\n* 665937d aa > aa0, bb bb0\n    move ./aa ./aa0\n    move ./bb ./bb0\n* 1fd0236 aa, bb\n    addfile ./aa\n```\n\nSee how `0d94733 Merge branch \'a\'` also contains `d26d325` and `0d94733`.\n\nUsage\n=====\n\n```\n$> git-darcs --help\nUsage: git-darcs [OPTIONS] COMMAND [ARGS]...\n\n  Click entrypoint.\n\nOptions:\n  --help  Sow this message and exit.\n\nCommands:\n  clone   Locally clone a tracking-repository to get a working-repository.\n  pull    Pull from source darcs-repository into a tracking-repository.\n  update  Incremental import of git into darcs.\n```\n\n```\n$> git-darcs update --help\nUsage: git-darcs update [OPTIONS]\n\n  Incremental import of git into darcs.\n\n  By default it imports a shallow copy (the current commit). Use `--no-\n  shallow` to import the complete history.\n\nOptions:\n  -v, --verbose / -nv, --no-verbose\n  -w, --warn / -nw, --no-warn     Warn that repository will be cleared\n  -b, --base TEXT                 On first update import from (commit-ish)\n  -s, --shallow / -ns, --no-shallow\n                                  On first update only import current commit\n  --help                          Show this message and exit.\n```\n\n```\n$> git-darcs clone --help\nUsage: git-darcs clone [OPTIONS] SOURCE DESTINATION\n\n  Locally clone a tracking-repository to get a working-repository.\n\nOptions:\n  -v, --verbose / -nv, --no-verbose\n  --help                          Show this message and exit.\n```\n\n```\n$> git-darcs pull --help\nUsage: git-darcs pull [OPTIONS] SOURCE [DARCS]...\n\n  Pull from source darcs-repository into a tracking-repository.\n\n  A tracking-repository is created by `git darcs update` and contains a git-\n  and a darcs-repository. Arguments after `--` are passed to `darcs pull`.\n\nOptions:\n  -v, --verbose / -nv, --no-verbose\n  -w, --warn / -nw, --no-warn     Warn that repository will be cleared\n  -a, --all / -na, --no-all       Pull all patches\n  -i, --ignore-temp / -ni, --no-ignore-temp\n                                  Ignore temporary patches (with \'temp: \')\n  --help                          Show this message and exit.\n```\n',
-    'author': 'Jean-Louis Fuchs',
-    'author_email': 'jean-louis.fuchs@adfinis.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ganwell/git-darcs',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Incremental import of git into darcs and back again
+====================================================
 
+[![Test](https://github.com/ganwell/git-darcs/actions/workflows/test.yml/badge.svg)](https://github.com/ganwell/git-darcs/actions/workflows/test.yml) [![CodeQL](https://github.com/ganwell/git-darcs/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ganwell/git-darcs/actions/workflows/codeql-analysis.yml)
+
+[git-darcs on pypi](https://pypi.org/project/git-darcs/)
+
+- [Warning](#-warning)
+- [Install](#Install)
+- [Use-cases](#use-cases)
+  * [Main use-case](#main-use-case)
+  * [Other use-case](#other-use-case)
+  * [But why?](#but-why)
+- [Tutorial](#Tutorial)
+- [For darcs beginners](#for-darcs-beginners)
+- [Caveats](#caveats)
+  * [Performance](#performance)
+  * [chmod and symbolic-links](#chmod-and-symbolic-links)
+  * [Linearized History](#linearized-history)
+- [Usage](#usage)
+
+⚠ Warning
+=========
+
+git-darcs needs a repository only for tracking. Don't use your working
+git-repository. git-darcs will clear all your work that is not commited. It also
+needs to temporarily change `.gitignore` and `_darcs/pref/boring`. By default it
+will warn about this. You can add `-nw` to avoid the warning. The tutorial never
+contains a `-nw`, so people don't copy-paste from the tutorial and lose their
+work.
+
+The tool is made for developers, while error-handling is okayish, there is
+almost no error-reporting, you'll have to read the traceback.
+
+![demo](https://github.com/ganwell/git-darcs/blob/main/demo.gif?raw=true)
+
+Install
+=======
+
+Integration tests run on python 3.7 - 3.11.
+
+```bash
+pip install git-darcs
+```
+
+Use-cases
+=========
+
+Main use-case
+-------------
+
+Use the excellent capabilities of darcs to craft consistent, clear and concise
+patches while the remote repository still remains git. Thats the situation most
+of us in are because at work we have to use git.
+
+Other use-cases
+---------------
+
+* Convert a git repository to darcs using the [linearized history](#linearized-history)
+  proposed by git-darcs
+* Visualize a git-repository using `darcs show dependencies`
+
+But why?
+--------
+
+I prefer to group changes by topic, so I am constantly amending commits/patches.
+This is very easy in darcs and more complicated in git. Yes, I know about
+`--fixup` and `--autosquash` in git. Also I can find independent low-risk
+patches easily with `darcs show dependencies`, so I can constantly make MRs.
+Making the final _breaking_ change/MR much smaller. This is less tedious for the
+reviewers.
+
+Tutorial
+========
+
+The tutorial covers the main use-case:
+
+1. Check-out a git-repo, because at work you have to use git
+2. Snapshot the latest commit into darcs
+3. Craft patches: Use the excellent capabilities of darcs to move code between
+   patches to create very consistent and clean patches
+4. Use `git darcs pull` to bring the darcs-patches back into git and
+   create pull-request
+
+Clone your tracking-repository.
+
+```bash
+$> git clone https://github.com/adfinis-sygroup/document-merge-service.git dms-track
+Cloning into 'document-merge-service'...
+
+.....
+
+Resolving deltas: 100% (1267/1267), done.
+```
+
+Lazily import the git-repository to darcs.
+
+```bash
+$> git darcs update
+Use CTRL-D for a graceful shutdown.
+```
+
+git-darcs will import the latest commit and tag it, so it can update from there,
+when you pull commits from upstream.
+
+```bash
+$> (cd dms-track; darcs log)
+patch 7997a3365da1022db4b669ea63a37dc3f370a225
+Author: Jean-Louis Fuchs <email>
+Date:   Fri Oct  7 17:40:10 CEST 2022
+  tagged git-checkpoint 2022-10-07T17:40:10.963827
+d3ce714f2d77897e773e89ee3344602fceb1b625
+
+patch 4e917fcc769b7a69858e0b11e7ee5aaffc76fbda
+Author: Jean-Louis Fuchs <email>
+Date:   Fri Oct  7 17:40:10 CEST 2022
+  * d3ce714 chore(release): v5.0.0
+```
+
+Create the work-repository. Note that git and darcs make sure that no historical
+data is duplicated on disk (using hardlinks).
+
+```bash
+$> git darcs clone dms-track/ dms-work
+clone: 100%|████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.75it/s]
+```
+
+Now you can implement a new feature.
+
+```bash
+$> cd dms-work
+$> touch document_merge_service/feature.py
+$> darcs add document_merge_service/feature.py
+Adding './document_merge_service/feature.py'
+Finished adding:
+./document_merge_service/feature.py
+
+$> darcs record -m "a new feature"
+addfile ./document_merge_service/feature.py
+Shall I record this change? (1/1)  [ynW...], or ? for more options: y
+Do you want to Record these changes? [Yglqk...], or ? for more options: y
+Finished recording patch 'a new feature'
+```
+
+```bash
+darcs show dependencies | dot -Tpdf -Grankdir=TB -o $ftmp
+```
+
+![first record](https://github.com/ganwell/git-darcs/blob/main/_static/first.png?raw=true)
+
+There are new changes on upstream, let's pull them in.
+
+```bash
+$> cd ../dms-track/
+$> git pull
+Updating d3ce714..a6a8e35
+Fast-forward
+ .github/workflows/tests.yml                         |  6 ++++-
+ 
+.....
+ 
+ 18 files changed, 262 insertions(+), 67 deletions(-)
+```
+
+From now on git-darcs will import every commit, but with a linearized
+history. That means the history might look different than in git, but no change will be
+forgotten. (See [Linearized History](#linearized-history))
+
+```bash
+$> git darcs update
+Use CTRL-D for a graceful shutdown.
+commits:
+100%|███████████████████████████████████████████████████████| 18/18 [00:00<00:00, 19.14it/s]
+```
+
+We pull the new patches into `dms-work`.
+
+```bash
+$> cd ../dms-track/
+$> darcs pull ../dms-track/
+Pulling from "/home/jeanlf/Temp/dms-track"...
+patch 309682700e7142e37945c45cc3375674012e8050
+Author: GitHub <noreply@github.com>
+Date:   Fri Oct  7 18:07:08 CEST 2022
+  * 85892f6 fix(docker): fix docker uwsgi command
+Shall I pull this patch? (1/19)  [ynW...], or ? for more options: a
+Finished pulling.
+```
+
+The 18 patches we pulled are now in `dms-work` along with a new snapshot-tag.
+
+```bash
+$> darcs log --from-tag=.
+patch 430136524b02be562fdf0f0459594ffa981d386b
+Author: Jean-Louis Fuchs <email>
+Date:   Fri Oct  7 18:07:09 CEST 2022
+  tagged git-checkpoint 2022-10-07T18:07:09.041126 a6a8e35ae3c3b42b04837a75ff59aa092130f326
+
+patch ef1f2894abd21d0deef19090d4b873bf62af890a
+Author: Jean-Louis Fuchs <email>
+Date:   Fri Oct  7 17:55:22 CEST 2022
+  * a new feature
+```
+
+We can now either pull the `a new feature`-patch into `dms-track` or we can
+create a temporary `dms-stage` so it is easier to clean up after the
+merge-request has been accepted. Note `git-darcs clone` will copy git-remotes
+from the source, so you can push into your fork if it is set up.
+
+If you pull into `dms-track` instead, you have to remove patches or commits on
+both darcs and git, keeping darcs and git manually in sync.
+
+
+```bash
+$> cd ..
+$> git darcs clone dms-track/ dms-stage
+clone: 100%|████████████████████████████████████████████████| 5/5 [00:00<00:00, 48.32it/s]
+$> cd dms-stage
+```
+
+`git-darcs pull` tries to emulate `darcs pull`.
+
+```bash
+$> git darcs pull ../dms-work/
+patch ef1f2894abd21d0deef19090d4b873bf62af890a
+Author: Jean-Louis Fuchs <email>
+Date: 2022-10-07 15:55:22
+Subject: a new feature
+Shall I pull this patch? 1/1  [ynwasc], or ? for more options: ?
+
+y: pull this patch
+n: don't pull it
+w: decide later
+
+a: pull all remaining patches
+i: don't pull remaining patches
+
+l: show full log message
+f: show full patch
+
+?: help
+h: help
+
+c: cancel without pulling
+q: cancel without pulling
+
+Shall I pull this patch? 1/1  [ynwasc], or ? for more options: y
+resolve: 0it [00:00, ?it/s]
+Shall I pull 1 patches?   [yn], or ? for more options: y
+pull: 100%|█████████████████████████████████████████████████| 1/1 [00:00<00:00,  2.58it/s]
+```
+
+The patch `a new feature` is now a git-commit.
+
+```bash
+$> git show
+commit c2541c6c3527d99a7fe69dc43b5863992d919a45 (HEAD -> main)
+Author: Jean-Louis Fuchs <email>
+Date:   Fri Oct 7 20:01:22 2022 +0200
+
+    a new feature
+
+diff --git a/document_merge_service/feature.py b/document_merge_service/feature.py
+new file mode 100644
+index 0000000..e69de29
+```
+
+```bash
+$> cd ..
+$> rm -r dms-stage
+```
+
+For darcs beginners
+===================
+
+* There is a great [video](https://hikari.acmelabs.space/videos/hikari-darcs.mp4) by
+  [raichoo](https://hub.darcs.net/raichoo) the maintainer of
+  [hikari](https://hikari.acmelabs.space/)
+* You have to read the [darcs book](https://darcsbook.acmelabs.space/), you just
+  have to
+* `_darcs/pref/boring` is the equivalent of `.gitignore`, but has quite a wide
+  definition of boring by default
+
+Caveats
+=======
+
+Performance
+-----------
+
+git-darcs will playback the history of the git-repository. Every commit that is
+recorded will first be checked out in git and then recorded in darcs. For that reason
+git-darcs lazily imports the latest commit by default. This is how it is meant
+to be used: Using darcs to complement git. You can use it to convert
+repositories, if you like the way non-linear history is handled, it will be
+sloooow. See also `darcs convert import`.
+
+chmod and symbolic links
+------------------------
+
+Darcs does not handle `chmod` or symbolic links. The easiest way to work around
+this is by  letting `git` do the work. Since I always make git-commits from the
+darcs-patches `git` will track `chmod` and symbolic links for me.
+
+Linearized History
+------------------
+
+git-darcs will traverse the git-history in topological order. For every commit
+it encounters, it will test if the previous commit was an ancestor, if not it
+will ignore that commit for now. That way git-darcs can only "enter" one branch
+of parallel history. Once it reaches a commit that is an ancestor it will import
+that commit and log the complete history between it and the last successful
+commit. So git-darcs creates patches that combine the complete history of a
+parallel branch.
+
+This git-log
+
+```
+$> git log --oneline --graph
+* eef24d8 (HEAD -> master) end > end0
+* 841c900 end
+*   969ad57 Merge branch 'b'
+|\
+| * 76ca538 (b) bb2 > bb3
+| * 0040cee bb1 > bb2
+* | 663168a antiforward > antiforward0
+* |   0d94733 Merge branch 'a'
+|\ \
+| * | d26d325 (a) aa2 > aa3
+| * | 8090696 aa1 > aa2
+| |/
+* / fa7accb antiforward
+|/
+* 7bc2b76 aa0 > aa1, bb0 > bb1
+* 665937d aa > aa0, bb bb0
+* 1fd0236 aa, bb
+```
+
+becomes this darcs-log
+
+```
+* eef24d8 end > end0
+    move ./end ./end0
+* 841c900 end
+    addfile ./end
+* 969ad57 Merge branch 'b'
+  76ca538 bb2 > bb3
+  0040cee bb1 > bb2
+    move ./bb1 ./bb3
+* 663168a antiforward > antiforward0
+    move ./antiforward ./antiforward0
+* 0d94733 Merge branch 'a'
+  d26d325 aa2 > aa3
+  8090696 aa1 > aa2
+    move ./aa1 ./aa3
+* fa7accb antiforward
+    addfile ./antiforward
+* 7bc2b76 aa0 > aa1, bb0 > bb1
+    move ./aa0 ./aa1
+    move ./bb0 ./bb1
+* 665937d aa > aa0, bb bb0
+    move ./aa ./aa0
+    move ./bb ./bb0
+* 1fd0236 aa, bb
+    addfile ./aa
+```
+
+See how `0d94733 Merge branch 'a'` also contains `d26d325` and `0d94733`.
+
+Usage
+=====
+
+```
+$> git-darcs --help
+Usage: git-darcs [OPTIONS] COMMAND [ARGS]...
+
+  Click entrypoint.
+
+Options:
+  --help  Sow this message and exit.
+
+Commands:
+  clone   Locally clone a tracking-repository to get a working-repository.
+  pull    Pull from source darcs-repository into a tracking-repository.
+  update  Incremental import of git into darcs.
+```
+
+```
+$> git-darcs update --help
+Usage: git-darcs update [OPTIONS]
+
+  Incremental import of git into darcs.
+
+  By default it imports a shallow copy (the current commit). Use `--no-
+  shallow` to import the complete history.
+
+Options:
+  -v, --verbose / -nv, --no-verbose
+  -w, --warn / -nw, --no-warn     Warn that repository will be cleared
+  -b, --base TEXT                 On first update import from (commit-ish)
+  -s, --shallow / -ns, --no-shallow
+                                  On first update only import current commit
+  --help                          Show this message and exit.
+```
+
+```
+$> git-darcs clone --help
+Usage: git-darcs clone [OPTIONS] SOURCE DESTINATION
+
+  Locally clone a tracking-repository to get a working-repository.
+
+Options:
+  -v, --verbose / -nv, --no-verbose
+  --help                          Show this message and exit.
+```
+
+```
+$> git-darcs pull --help
+Usage: git-darcs pull [OPTIONS] SOURCE [DARCS]...
+
+  Pull from source darcs-repository into a tracking-repository.
+
+  A tracking-repository is created by `git darcs update` and contains a git-
+  and a darcs-repository. Arguments after `--` are passed to `darcs pull`.
+
+Options:
+  -v, --verbose / -nv, --no-verbose
+  -w, --warn / -nw, --no-warn     Warn that repository will be cleared
+  -a, --all / -na, --no-all       Pull all patches
+  -i, --ignore-temp / -ni, --no-ignore-temp
+                                  Ignore temporary patches (with 'temp: ')
+  --help                          Show this message and exit.
+```
 
-setup(**setup_kwargs)
```

