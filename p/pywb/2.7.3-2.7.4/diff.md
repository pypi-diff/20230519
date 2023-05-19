# Comparing `tmp/pywb-2.7.3.tar.gz` & `tmp/pywb-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywb-2.7.3.tar", last modified: Fri Feb  3 01:40:46 2023, max compression
+gzip compressed data, was "pywb-2.7.4.tar", last modified: Fri May 19 18:25:16 2023, max compression
```

## Comparing `pywb-2.7.3.tar` & `pywb-2.7.4.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.692568 pywb-2.7.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-02-03 01:40:34.000000 pywb-2.7.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-03 01:40:34.000000 pywb-2.7.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-03 01:40:34.000000 pywb-2.7.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)    81373 2023-02-03 01:40:34.000000 pywb-2.7.3/CHANGES.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-02-03 01:40:34.000000 pywb-2.7.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-02-03 01:40:34.000000 pywb-2.7.3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-02-03 01:40:34.000000 pywb-2.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-03 01:40:34.000000 pywb-2.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-03 01:40:34.000000 pywb-2.7.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-03 01:40:46.692568 pywb-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-03 01:40:34.000000 pywb-2.7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-02-03 01:40:34.000000 pywb-2.7.3/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-03 01:40:34.000000 pywb-2.7.3/appveyor.disabled.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-02-03 01:40:34.000000 pywb-2.7.3/build-vue-ui.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-02-03 01:40:34.000000 pywb-2.7.3/build-wombat.sh
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-03 01:40:34.000000 pywb-2.7.3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-03 01:40:34.000000 pywb-2.7.3/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-02-03 01:40:34.000000 pywb-2.7.3/docker-entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.608566 pywb-2.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.608566 pywb-2.7.3/docs/code/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.apps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.indexer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.recorder.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.rewrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.warcserver.index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.warcserver.resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/code/pywb.warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.612566 pywb-2.7.3/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/access-control.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/apis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/apps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/cdxserver_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/localization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/memento.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/migrating-cdx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/outbackcdx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/owb-pywb-terms.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/owb-to-pywb-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/owb-to-pywb-deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/owb-to-pywb-exclusions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/owb-transition.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/recorder.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/rewriter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/template-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/ui-customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/ui-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/vue-ui.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-02-03 01:40:34.000000 pywb-2.7.3/docs/manual/warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-03 01:40:34.000000 pywb-2.7.3/extra_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    35411 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/frontendapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/live.py
--rw-r--r--   0 runner    (1001) docker     (123)    36151 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/rewriterapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/static_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb/apps/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/test/test_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/test/test_wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/warcserverapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/apps/wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb/git_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb/indexer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/indexer/archiveindexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/indexer/cdxindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb/indexer/test/
--rw-r--r--   0 runner    (1001) docker     (123)    26788 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/indexer/test/test_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.620566 pywb-2.7.3/pywb/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/aclmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/autoindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/locmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/manager/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.620566 pywb-2.7.3/pywb/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/multifilewarcwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/recorderapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/redisindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.620566 pywb-2.7.3/pywb/recorder/test/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/test/rec.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/test/simplerec.py
--rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/recorder/test/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.624566 pywb-2.7.3/pywb/rewrite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/default_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22051 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/rewrite_amf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/rewrite_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/rewrite_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/rewrite_js_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/rewriteinputreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/templateview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.624566 pywb-2.7.3/pywb/rewrite/test/
--rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/test/test_wburl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rewrite/wburl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.628567 pywb-2.7.3/pywb/static/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/autoFetchWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/calendar-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/calendar.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.628567 pywb-2.7.3/pywb/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)   153136 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    54636 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/css/query.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.632567 pywb-2.7.3/pywb/static/flowplayer/
--rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/flowplayer/flowplayer-3.2.18.swf
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/flowplayer/toolbox.flashembed.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.632567 pywb-2.7.3/pywb/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.636567 pywb-2.7.3/pywb/static/fonts/font-awesome/
--rw-r--r--   0 runner    (1001) docker     (123)   125320 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   660056 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   125016 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    84568 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    72148 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144523 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   186512 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   816218 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   186228 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96248 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74320 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.636567 pywb-2.7.3/pywb/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    76308 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/js/jquery-latest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/js/url-polyfill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.640567 pywb-2.7.3/pywb/static/loading-spinner/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/loading-spinner/loading-spinner.js
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/loading-spinner/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/pywb-logo-sm.png
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/pywb-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/query.js
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/queryWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/scroll-webkit.css
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/timeline-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/transclusions.js
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/vidrw.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.640567 pywb-2.7.3/pywb/static/vue/
--rw-r--r--   0 runner    (1001) docker     (123)  1574967 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/vue/vueui.js
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/vue_banner.css
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/wb_frame.js
--rw-r--r--   0 runner    (1001) docker     (123)   126935 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/wombat.js
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/wombatProxyMode.js
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/wombatWorkers.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/static/zoom-out-icon-333316.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.644567 pywb-2.7.3/pywb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/bootstrap_jquery.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/collinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/custom_banner.html
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/frame_insert.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/head_insert.html
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/not_found.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/proxy_cert_download.html
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/proxy_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/query.html
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/templates/vue_loc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.648567 pywb-2.7.3/pywb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/binsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/geventserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/memento.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.648567 pywb-2.7.3/pywb/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/test/test_binsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/utils/wbexception.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.600566 pywb-2.7.3/pywb/vueui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.600566 pywb-2.7.3/pywb/vueui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.648567 pywb-2.7.3/pywb/vueui/src/cdx-simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/vueui/src/cdx-simulator/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.652567 pywb-2.7.3/pywb/warcserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/access_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/amf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/basewarcserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.652567 pywb-2.7.3/pywb/warcserver/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/cdxops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.656567 pywb-2.7.3/pywb/warcserver/index/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_cdxops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_dir_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_lazy_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_memento_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_redis_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_xmlquery_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/test/test_zipnum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/index/zipnum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/inputrequest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.656567 pywb-2.7.3/pywb/warcserver/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/blockrecordloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/pathresolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/resolvingloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/responseloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.656567 pywb-2.7.3/pywb/warcserver/resource/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/test/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/resource/test/test_pathresolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.660567 pywb-2.7.3/pywb/warcserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/live.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_amf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22680 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_inputreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_warcserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/test_warcserver_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/upstreamindexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-02-03 01:40:34.000000 pywb-2.7.3/pywb/warcserver/warcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.616566 pywb-2.7.3/pywb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-03 01:40:46.000000 pywb-2.7.3/pywb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-03 01:40:34.000000 pywb-2.7.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-02-03 01:40:34.000000 pywb-2.7.3/run-gunicorn.sh
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-03 01:40:34.000000 pywb-2.7.3/run-tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-02-03 01:40:34.000000 pywb-2.7.3/run-uwsgi.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.604566 pywb-2.7.3/sample_archive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.660567 pywb-2.7.3/sample_archive/access/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/allows.aclj
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/blocks.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/list1.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/list2.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/pywb.aclj
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/access/single-line.aclj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.664568 pywb-2.7.3/sample_archive/cdx/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/bad.cdx
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/dupes.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/example-arc-test.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/example-extra.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/example.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/httpbin-resource.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)    30399 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/iana.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/missing-status-text.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/post-test.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdx/url-agnost-example.cdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.664568 pywb-2.7.3/sample_archive/cdxj/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/dupes.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/example-no-digest.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/example.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/example2.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)    43062 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/iana.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/post-test.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/cdxj/url-agnost-example.cdxj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.664568 pywb-2.7.3/sample_archive/non-surt-cdx/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/non-surt-cdx/example-non-surt.cdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.668568 pywb-2.7.3/sample_archive/text_content/
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/link_headers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/pathindex.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/quickfox_repeated.compressed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample_dash.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample_hls.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample_no_head.html
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample_no_head_2.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/sample_unclosed_script.html
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/text_content/toptest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.672568 pywb-2.7.3/sample_archive/warcs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/bad.arc
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/dupes.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-bad.warc.gz.bad
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-extra.warc
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-url-agnostic-orig.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-wget-1-14.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example-wpull.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example.arc
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example.arc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example.warc
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/example2.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/httpbin-resource.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)   786828 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/iana.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/missing-status-text.warc
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/warcs/post-test.warc.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.676568 pywb-2.7.3/sample_archive/zipcdx/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/zipcdx/zipnum-bad.idx
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/zipcdx/zipnum-bad.loc
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/zipcdx/zipnum-sample.cdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/zipcdx/zipnum-sample.idx
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-03 01:40:34.000000 pywb-2.7.3/sample_archive/zipcdx/zipnum-sample.loc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 01:40:46.692568 pywb-2.7.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4886 2023-02-03 01:40:34.000000 pywb-2.7.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-03 01:40:34.000000 pywb-2.7.3/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.684568 pywb-2.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_access.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_cert_req.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_loc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_record.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_record_dedup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_redirect_classic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/config_test_root_coll.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.604566 pywb-2.7.3/tests/i18n-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.604566 pywb-2.7.3/tests/i18n-data/l337/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.684568 pywb-2.7.3/tests/i18n-data/l337/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/i18n-data/l337/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/memento_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_acl_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_auto_colls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_cdx_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_cert_req.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_embargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_force_https.py
--rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_live_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_prefer_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_prefixed_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_record_dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_record_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_redirect_classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_redirect_revisits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_root_coll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-03 01:40:34.000000 pywb-2.7.3/tests/test_zipnum_auto_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 01:40:46.692568 pywb-2.7.3/tests_disabled/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/perms_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/server_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/server_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_cdxserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_frames.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_memento.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_proxy_http_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_proxy_https_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_proxy_ip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_proxy_ip_redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_proxy_no_banner.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_config_root_coll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_live_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_perms_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_http_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_http_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_http_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_http_ip_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_http_no_banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_proxy_https_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-03 01:40:34.000000 pywb-2.7.3/tests_disabled/test_rewrite_content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-02-03 01:40:34.000000 pywb-2.7.3/update-tag.sh
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-03 01:40:34.000000 pywb-2.7.3/uwsgi.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.290699 pywb-2.7.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-05-19 18:25:04.000000 pywb-2.7.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 18:25:04.000000 pywb-2.7.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-19 18:25:04.000000 pywb-2.7.4/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    81373 2023-05-19 18:25:04.000000 pywb-2.7.4/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-05-19 18:25:04.000000 pywb-2.7.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-19 18:25:04.000000 pywb-2.7.4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-19 18:25:04.000000 pywb-2.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-19 18:25:04.000000 pywb-2.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-19 18:25:04.000000 pywb-2.7.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 18:25:16.290699 pywb-2.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-19 18:25:04.000000 pywb-2.7.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-19 18:25:04.000000 pywb-2.7.4/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 18:25:04.000000 pywb-2.7.4/appveyor.disabled.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-05-19 18:25:04.000000 pywb-2.7.4/build-vue-ui.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-05-19 18:25:04.000000 pywb-2.7.4/build-wombat.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-19 18:25:04.000000 pywb-2.7.4/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-19 18:25:04.000000 pywb-2.7.4/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-05-19 18:25:04.000000 pywb-2.7.4/docker-entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.238695 pywb-2.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.apps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.indexer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.rewrite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/access-control.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/apis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/apps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/cdxserver_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/localization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/memento.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/migrating-cdx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/outbackcdx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-pywb-terms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-exclusions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-transition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/rewriter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/template-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/ui-customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/ui-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/vue-ui.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 18:25:04.000000 pywb-2.7.4/extra_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/pywb/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35411 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/frontendapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36153 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/rewriterapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/static_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/apps/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/test/test_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/test/test_wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/warcserverapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:25:15.000000 pywb-2.7.4/pywb/git_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/indexer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/archiveindexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/cdxindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/indexer/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    26788 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/test/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/aclmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/autoindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/locmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/multifilewarcwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/recorderapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/redisindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/recorder/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/rec.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/simplerec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/rewrite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/default_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22051 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_amf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_js_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewriteinputreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/templateview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/rewrite/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_wburl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/wburl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/autoFetchWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/calendar-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/calendar.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)   153136 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54636 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/query.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/flowplayer/
+-rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer-3.2.18.swf
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/toolbox.flashembed.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.258696 pywb-2.7.4/pywb/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/fonts/font-awesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   125320 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   660056 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   125016 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    84568 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    72148 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144523 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   186512 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   816218 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   186228 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96248 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74320 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    76308 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/jquery-latest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/url-polyfill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/loading-spinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/loading-spinner/loading-spinner.js
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/loading-spinner/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/pywb-logo-sm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/pywb-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/query.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/queryWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/scroll-webkit.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/timeline-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/transclusions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vidrw.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/vue/
+-rw-r--r--   0 runner    (1001) docker     (123)  1574967 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vue/vueui.js
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vue_banner.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wb_frame.js
+-rw-r--r--   0 runner    (1001) docker     (123)   128535 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombat.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombatProxyMode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombatWorkers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/zoom-out-icon-333316.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.266697 pywb-2.7.4/pywb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/bootstrap_jquery.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/collinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/custom_banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/frame_insert.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/head_insert.html
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/not_found.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/proxy_cert_download.html
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/proxy_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/vue_loc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.266697 pywb-2.7.4/pywb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/geventserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/memento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/test/test_binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/wbexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/pywb/vueui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/pywb/vueui/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/vueui/src/cdx-simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/vueui/src/cdx-simulator/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/access_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/amf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/basewarcserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/index/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_dir_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_lazy_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_memento_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_redis_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_xmlquery_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/inputrequest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/blockrecordloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/pathresolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/resolvingloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/responseloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/resource/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/test_pathresolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/live.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_amf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_inputreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_warcserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_warcserver_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/upstreamindexsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/warcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-19 18:25:04.000000 pywb-2.7.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-05-19 18:25:04.000000 pywb-2.7.4/run-gunicorn.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 18:25:04.000000 pywb-2.7.4/run-tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-19 18:25:04.000000 pywb-2.7.4/run-uwsgi.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/sample_archive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/sample_archive/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/allows.aclj
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/blocks.aclj
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/list1.aclj
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/list2.aclj
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/pywb.aclj
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/single-line.aclj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/sample_archive/cdx/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/bad.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/dupes.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example-arc-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example-extra.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/httpbin-resource.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)    30399 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/iana.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/missing-status-text.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/post-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/url-agnost-example.cdx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/cdxj/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/dupes.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example-no-digest.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example2.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)    43062 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/iana.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/post-test.cdxj
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/url-agnost-example.cdxj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/non-surt-cdx/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/non-surt-cdx/example-non-surt.cdx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/text_content/
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/link_headers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/pathindex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/quickfox_repeated.compressed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_dash.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_hls.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_no_head.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_no_head_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_unclosed_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/toptest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.282698 pywb-2.7.4/sample_archive/warcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/bad.arc
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/dupes.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-bad.warc.gz.bad
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-extra.warc
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-url-agnostic-orig.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-wget-1-14.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-wpull.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.arc
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.arc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.warc
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example2.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/httpbin-resource.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   786828 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/iana.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/missing-status-text.warc
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/post-test.warc.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.282698 pywb-2.7.4/sample_archive/zipcdx/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-bad.idx
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-bad.loc
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.cdx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.idx
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.loc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:25:16.290699 pywb-2.7.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4886 2023-05-19 18:25:05.000000 pywb-2.7.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 18:25:05.000000 pywb-2.7.4/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.286698 pywb-2.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_access.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_cert_req.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_loc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_record.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_record_dedup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_redirect_classic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_root_coll.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/tests/i18n-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/tests/i18n-data/l337/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.286698 pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/memento_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_acl_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_auto_colls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cdx_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cert_req.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_embargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_force_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_live_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_prefer_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_prefixed_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_record_dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_record_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirect_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirect_revisits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_root_coll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_zipnum_auto_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.290699 pywb-2.7.4/tests_disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/perms_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/server_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/server_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_cdxserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_frames.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_memento.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_http_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_https_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_ip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_ip_redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_no_banner.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_root_coll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_live_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_perms_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_ip_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_no_banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_https_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_rewrite_content.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-05-19 18:25:05.000000 pywb-2.7.4/update-tag.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-19 18:25:05.000000 pywb-2.7.4/uwsgi.ini
```

### Comparing `pywb-2.7.3/.travis.yml` & `pywb-2.7.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/CHANGES.rst` & `pywb-2.7.4/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/Dockerfile` & `pywb-2.7.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/INSTALL.rst` & `pywb-2.7.4/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/LICENSE` & `pywb-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/MANIFEST.in` & `pywb-2.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/PKG-INFO` & `pywb-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.7.3
+Version: 2.7.4
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pywb-2.7.3/README.rst` & `pywb-2.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/Vagrantfile` & `pywb-2.7.4/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/appveyor.disabled.yml` & `pywb-2.7.4/appveyor.disabled.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/config.yaml` & `pywb-2.7.4/config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docker-entrypoint.sh` & `pywb-2.7.4/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/Makefile` & `pywb-2.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.apps.rst` & `pywb-2.7.4/docs/code/pywb.apps.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.manager.rst` & `pywb-2.7.4/docs/code/pywb.manager.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.recorder.rst` & `pywb-2.7.4/docs/code/pywb.recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.rewrite.rst` & `pywb-2.7.4/docs/code/pywb.rewrite.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.utils.rst` & `pywb-2.7.4/docs/code/pywb.utils.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.warcserver.index.rst` & `pywb-2.7.4/docs/code/pywb.warcserver.index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.warcserver.resource.rst` & `pywb-2.7.4/docs/code/pywb.warcserver.resource.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/code/pywb.warcserver.rst` & `pywb-2.7.4/docs/code/pywb.warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/conf.py` & `pywb-2.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/index.rst` & `pywb-2.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/make.bat` & `pywb-2.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/access-control.rst` & `pywb-2.7.4/docs/manual/access-control.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/apps.rst` & `pywb-2.7.4/docs/manual/apps.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/cdxserver_api.rst` & `pywb-2.7.4/docs/manual/cdxserver_api.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/configuring.rst` & `pywb-2.7.4/docs/manual/configuring.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/indexing.rst` & `pywb-2.7.4/docs/manual/indexing.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/localization.rst` & `pywb-2.7.4/docs/manual/localization.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/memento.rst` & `pywb-2.7.4/docs/manual/memento.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/migrating-cdx.rst` & `pywb-2.7.4/docs/manual/migrating-cdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/outbackcdx.rst` & `pywb-2.7.4/docs/manual/outbackcdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/owb-pywb-terms.rst` & `pywb-2.7.4/docs/manual/owb-pywb-terms.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/owb-to-pywb-config.rst` & `pywb-2.7.4/docs/manual/owb-to-pywb-config.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/owb-to-pywb-deploy.rst` & `pywb-2.7.4/docs/manual/owb-to-pywb-deploy.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/owb-to-pywb-exclusions.rst` & `pywb-2.7.4/docs/manual/owb-to-pywb-exclusions.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/recorder.rst` & `pywb-2.7.4/docs/manual/recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/rewriter.rst` & `pywb-2.7.4/docs/manual/rewriter.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/template-guide.rst` & `pywb-2.7.4/docs/manual/template-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/ui-guide.rst` & `pywb-2.7.4/docs/manual/ui-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/usage.rst` & `pywb-2.7.4/docs/manual/usage.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/vue-ui.rst` & `pywb-2.7.4/docs/manual/vue-ui.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/docs/manual/warcserver.rst` & `pywb-2.7.4/docs/manual/warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/cli.py` & `pywb-2.7.4/pywb/apps/cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/frontendapp.py` & `pywb-2.7.4/pywb/apps/frontendapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/rewriterapp.py` & `pywb-2.7.4/pywb/apps/rewriterapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,16 +244,16 @@
 
         wb_url.url = mod_url
         inputreq.url = mod_url
 
         range_start = start
         range_end = end
 
-        # if start with 0, load from upstream, but add range after
-        if start == 0:
+        # if start with 0 and no end, load from upstream
+        if start == 0 and not end:
             del inputreq.env['HTTP_RANGE']
         else:
             skip_record = True
 
         return range_start, range_end, skip_record
 
     def _add_range(self, record, wb_url, range_start, range_end):
```

### Comparing `pywb-2.7.3/pywb/apps/static_handler.py` & `pywb-2.7.4/pywb/apps/static_handler.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/test/test_rewriter.py` & `pywb-2.7.4/pywb/apps/test/test_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/test/test_wbrequestresponse.py` & `pywb-2.7.4/pywb/apps/test/test_wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/apps/wbrequestresponse.py` & `pywb-2.7.4/pywb/apps/wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/default_config.yaml` & `pywb-2.7.4/pywb/default_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/indexer/archiveindexer.py` & `pywb-2.7.4/pywb/indexer/archiveindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/indexer/cdxindexer.py` & `pywb-2.7.4/pywb/indexer/cdxindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/indexer/test/test_indexing.py` & `pywb-2.7.4/pywb/indexer/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/manager/aclmanager.py` & `pywb-2.7.4/pywb/manager/aclmanager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/manager/autoindex.py` & `pywb-2.7.4/pywb/manager/autoindex.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/manager/locmanager.py` & `pywb-2.7.4/pywb/manager/locmanager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/manager/manager.py` & `pywb-2.7.4/pywb/manager/manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/manager/migrate.py` & `pywb-2.7.4/pywb/manager/migrate.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/filters.py` & `pywb-2.7.4/pywb/recorder/filters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/multifilewarcwriter.py` & `pywb-2.7.4/pywb/recorder/multifilewarcwriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/recorderapp.py` & `pywb-2.7.4/pywb/recorder/recorderapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/redisindexer.py` & `pywb-2.7.4/pywb/recorder/redisindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/test/simplerec.py` & `pywb-2.7.4/pywb/recorder/test/simplerec.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/recorder/test/test_recorder.py` & `pywb-2.7.4/pywb/recorder/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/content_rewriter.py` & `pywb-2.7.4/pywb/rewrite/content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/cookie_rewriter.py` & `pywb-2.7.4/pywb/rewrite/cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/cookies.py` & `pywb-2.7.4/pywb/rewrite/cookies.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/default_rewriter.py` & `pywb-2.7.4/pywb/rewrite/default_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/header_rewriter.py` & `pywb-2.7.4/pywb/rewrite/header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/html_insert_rewriter.py` & `pywb-2.7.4/pywb/rewrite/html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/html_rewriter.py` & `pywb-2.7.4/pywb/rewrite/html_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/jsonp_rewriter.py` & `pywb-2.7.4/pywb/rewrite/jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/regex_rewriters.py` & `pywb-2.7.4/pywb/rewrite/regex_rewriters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/rewrite_amf.py` & `pywb-2.7.4/pywb/rewrite/rewrite_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/rewrite_dash.py` & `pywb-2.7.4/pywb/rewrite/rewrite_dash.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/rewrite_hls.py` & `pywb-2.7.4/pywb/rewrite/rewrite_hls.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/rewrite_js_workers.py` & `pywb-2.7.4/pywb/rewrite/rewrite_js_workers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/rewriteinputreq.py` & `pywb-2.7.4/pywb/rewrite/rewriteinputreq.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/templateview.py` & `pywb-2.7.4/pywb/rewrite/templateview.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_content_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_cookie_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_header_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_html_insert_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_html_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_html_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_jsonp_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_regex_rewriters.py` & `pywb-2.7.4/pywb/rewrite/test/test_regex_rewriters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_url_rewriter.py` & `pywb-2.7.4/pywb/rewrite/test/test_url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/test/test_wburl.py` & `pywb-2.7.4/pywb/rewrite/test/test_wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/url_rewriter.py` & `pywb-2.7.4/pywb/rewrite/url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rewrite/wburl.py` & `pywb-2.7.4/pywb/rewrite/wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/rules.yaml` & `pywb-2.7.4/pywb/rules.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/autoFetchWorker.js` & `pywb-2.7.4/pywb/static/autoFetchWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/calendar-icon.png` & `pywb-2.7.4/pywb/static/calendar-icon.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/css/base.css` & `pywb-2.7.4/pywb/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/css/bootstrap.min.css` & `pywb-2.7.4/pywb/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/css/font-awesome.min.css` & `pywb-2.7.4/pywb/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/flowplayer/flowplayer-3.2.18.swf` & `pywb-2.7.4/pywb/static/flowplayer/flowplayer-3.2.18.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf` & `pywb-2.7.4/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf` & `pywb-2.7.4/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf` & `pywb-2.7.4/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/flowplayer/toolbox.flashembed.js` & `pywb-2.7.4/pywb/static/flowplayer/toolbox.flashembed.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.eot` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.svg` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.ttf` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.woff` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-brands-400.woff2` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.eot` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.svg` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.ttf` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.woff` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-regular-400.woff2` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.eot` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.svg` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.ttf` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.woff` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/font-awesome/fa-solid-900.woff2` & `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.eot` & `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.svg` & `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.ttf` & `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.woff` & `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/fonts/glyphicons-halflings-regular.woff2` & `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/js/bootstrap.min.js` & `pywb-2.7.4/pywb/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/js/jquery-latest.min.js` & `pywb-2.7.4/pywb/static/js/jquery-latest.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/js/url-polyfill.min.js` & `pywb-2.7.4/pywb/static/js/url-polyfill.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/loading-spinner/loading-spinner.js` & `pywb-2.7.4/pywb/static/loading-spinner/loading-spinner.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/pywb-logo-sm.png` & `pywb-2.7.4/pywb/static/pywb-logo-sm.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/pywb-logo.png` & `pywb-2.7.4/pywb/static/pywb-logo.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/query.js` & `pywb-2.7.4/pywb/static/query.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/queryWorker.js` & `pywb-2.7.4/pywb/static/queryWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/scroll-webkit.css` & `pywb-2.7.4/pywb/static/scroll-webkit.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/search.js` & `pywb-2.7.4/pywb/static/search.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/timeline-icon.png` & `pywb-2.7.4/pywb/static/timeline-icon.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/transclusions.js` & `pywb-2.7.4/pywb/static/transclusions.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/vidrw.js` & `pywb-2.7.4/pywb/static/vidrw.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/vue/vueui.js` & `pywb-2.7.4/pywb/static/vue/vueui.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/wb_frame.js` & `pywb-2.7.4/pywb/static/wb_frame.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/wombat.js` & `pywb-2.7.4/pywb/static/wombat.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -328,15 +328,15 @@
                 src: "oe_",
                 poster: "im_"
             },
             image: {
                 href: "im_",
                 "xlink:href": "im_"
             }
-        }, this.URL_PROPS = ["href", "hash", "pathname", "host", "hostname", "protocol", "origin", "search", "port"], this.wb_info = wbinfo, this.wb_opts = wbinfo.wombat_opts, this.wb_replay_prefix = wbinfo.prefix, this.wb_is_proxy = this.wb_info.proxy_magic || !this.wb_replay_prefix, this.wb_info.top_host = this.wb_info.top_host || "*", this.wb_curr_host = $wbwindow.location.protocol + "//" + $wbwindow.location.host, this.wb_info.wombat_opts = this.wb_info.wombat_opts || {}, this.wb_orig_scheme = this.wb_info.wombat_scheme + "://", this.wb_orig_origin = this.wb_orig_scheme + this.wb_info.wombat_host, this.wb_abs_prefix = this.wb_replay_prefix, this.wb_capture_date_part = "", !this.wb_info.is_live && this.wb_info.wombat_ts && (this.wb_capture_date_part = "/" + this.wb_info.wombat_ts + "/"), this.BAD_PREFIXES = ["http:" + this.wb_replay_prefix, "https:" + this.wb_replay_prefix, "http:/" + this.wb_replay_prefix, "https:/" + this.wb_replay_prefix], this.hostnamePortRe = /^[\w-]+(\.[\w-_]+)+(:\d+)(\/|$)/, this.ipPortRe = /^\d+\.\d+\.\d+\.\d+(:\d+)?(\/|$)/, this.workerBlobRe = /__WB_pmw\(.*?\)\.(?=postMessage\()/g, this.rmCheckThisInjectRe = /_____WB\$wombat\$check\$this\$function_____\(.*?\)/g, this.STYLE_REGEX = /(url\s*\(\s*[\\"']*)([^)'"]+)([\\"']*\s*\))/gi, this.IMPORT_REGEX = /(@import\s*[\\"']*)([^)'";]+)([\\"']*\s*;?)/gi, this.IMPORT_JS_REGEX = /^(import\s*\(['"]+)([^'"]+)(["'])/i, this.no_wombatRe = /WB_wombat_/g, this.srcsetRe = /\s*(\S*\s+[\d.]+[wx]),|(?:\s*,(?:\s+|(?=https?:)))/, this.cookie_path_regex = /\bPath='?"?([^;'"\s]+)/i, this.cookie_domain_regex = /\bDomain=([^;'"\s]+)/i, this.cookie_expires_regex = /\bExpires=([^;'"]+)/gi, this.SetCookieRe = /,(?![|])/, this.IP_RX = /^(\d)+\.(\d)+\.(\d)+\.(\d)+$/, this.FullHTMLRegex = /^\s*<(?:html|head|body|!doctype html)/i, this.IsTagRegex = /^\s*</, this.DotPostMessageRe = /(\.postMessage\s*\()/, this.extractPageUnderModiferRE = /\/(?:[0-9]{14})?([a-z]{2, 3}_)\//, this.write_buff = "";
+        }, this.URL_PROPS = ["href", "hash", "pathname", "host", "hostname", "protocol", "origin", "search", "port"], this.wb_info = wbinfo, this.wb_opts = wbinfo.wombat_opts, this.wb_replay_prefix = wbinfo.prefix, this.wb_is_proxy = this.wb_info.proxy_magic || !this.wb_replay_prefix, this.wb_info.top_host = this.wb_info.top_host || "*", this.wb_curr_host = $wbwindow.location.protocol + "//" + $wbwindow.location.host, this.wb_info.wombat_opts = this.wb_info.wombat_opts || {}, this.wb_orig_scheme = this.wb_info.wombat_scheme + "://", this.wb_orig_origin = this.wb_orig_scheme + this.wb_info.wombat_host, this.wb_abs_prefix = this.wb_replay_prefix, this.wb_capture_date_part = "", !this.wb_info.is_live && this.wb_info.wombat_ts && (this.wb_capture_date_part = "/" + this.wb_info.wombat_ts + "/"), this.BAD_PREFIXES = ["http:" + this.wb_replay_prefix, "https:" + this.wb_replay_prefix, "http:/" + this.wb_replay_prefix, "https:/" + this.wb_replay_prefix], this.hostnamePortRe = /^[\w-]+(\.[\w-_]+)+(:\d+)(\/|$)/, this.ipPortRe = /^\d+\.\d+\.\d+\.\d+(:\d+)?(\/|$)/, this.workerBlobRe = /__WB_pmw\(.*?\)\.(?=postMessage\()/g, this.rmCheckThisInjectRe = /_____WB\$wombat\$check\$this\$function_____\(.*?\)/g, this.STYLE_REGEX = /(url\s*\(\s*[\\"']*)([^)'"]+)([\\"']*\s*\))/gi, this.IMPORT_REGEX = /(@import\s*[\\"']*)([^)'";]+)([\\"']*\s*;?)/gi, this.IMPORT_JS_REGEX = /^(import\s*\(['"]+)([^'"]+)(["'])/i, this.no_wombatRe = /WB_wombat_/g, this.srcsetRe = /\s*(\S*\s+[\d.]+[wx]),|(?:\s*,(?:\s+|(?=https?:)))/, this.cookie_path_regex = /\bPath='?"?([^;'"\s]+)/i, this.cookie_domain_regex = /\bDomain=([^;'"\s]+)/i, this.cookie_expires_regex = /\bExpires=([^;'"]+)/gi, this.SetCookieRe = /,(?![|])/, this.IP_RX = /^(\d)+\.(\d)+\.(\d)+\.(\d)+$/, this.FullHTMLRegex = /^\s*<(?:html|head|body|!doctype html)/i, this.IsTagRegex = /^\s*</, this.DotPostMessageRe = /(\.postMessage\s*\()/, this.extractPageUnderModifierRE = /\/(?:[0-9]{14})?([a-z]{2, 3}_)\//, this.write_buff = "";
         var eTargetProto = ($wbwindow.EventTarget || {}).prototype;
         this.utilFns = {
             cspViolationListener: function(e) {
                 if (console.group("CSP Violation"), console.log("Replayed Page URL", window.WB_wombat_location.href), console.log("The documentURI", e.documentURI), console.log("The blocked URL", e.blockedURI), console.log("The directive violated", e.violatedDirective), console.log("Our policy", e.originalPolicy), e.sourceFile) {
                     var fileInfo = "File: " + e.sourceFile;
                     e.lineNumber && e.columnNumber ? fileInfo += " @ " + e.lineNumber + ":" + e.columnNumber : e.lineNumber && (fileInfo += " @ " + e.lineNumber), console.log(fileInfo)
                 }
@@ -583,27 +583,39 @@
         this.showCSPViolations.yesNo = yesNo, this.showCSPViolations.yesNo && !this.showCSPViolations.added ? (this.showCSPViolations.added = true, this._addEventListener(document, "securitypolicyviolation", this.utilFns.cspViolationListener)) : (this.showCSPViolations.added = false, this._removeEventListener(document, "securitypolicyviolation", this.utilFns.cspViolationListener))
     }, Wombat.prototype._addEventListener = function(obj, event, fun) {
         return this.utilFns.addEventListener ? this.utilFns.addEventListener.call(obj, event, fun) : void obj.addEventListener(event, fun)
     }, Wombat.prototype._removeEventListener = function(obj, event, fun) {
         return this.utilFns.removeEventListener ? this.utilFns.removeEventListener.call(obj, event, fun) : void obj.removeEventListener(event, fun)
     }, Wombat.prototype.getPageUnderModifier = function() {
         try {
-            var pageUnderModifier = this.extractPageUnderModiferRE.exec(location.pathname);
+            var pageUnderModifier = this.extractPageUnderModifierRE.exec(location.pathname);
             if (pageUnderModifier && pageUnderModifier[1]) {
                 var mod = pageUnderModifier[1].trim();
                 return mod || "mp_"
             }
         } catch (e) {}
         return "mp_"
     }, Wombat.prototype.isNativeFunction = function(funToTest) {
         if (!funToTest || typeof funToTest !== "function") return false;
         var str = this.wb_funToString.call(funToTest);
         return str.indexOf("[native code]") != -1 && (!(funToTest.__WB_is_native_func__ !== undefined) || !!funToTest.__WB_is_native_func__)
     }, Wombat.prototype.isString = function(arg) {
         return arg != null && Object.getPrototypeOf(arg) === String.prototype
+    }, Wombat.prototype.blobUrlForIframe = function(iframe, string) {
+        var blob = new Blob([string], {
+                type: "text/html"
+            }),
+            url = URL.createObjectURL(blob);
+        iframe.__wb_blobSrc = url, iframe.addEventListener("load", function() {
+            iframe.__wb_blobSrc && (URL.revokeObjectURL(iframe.__wb_blobSrc), iframe.__wb_blobSrc = null)
+        }, {
+            once: true
+        }), iframe.__wb_origSrc = iframe.src;
+        var blobIdUrl = url.slice(url.lastIndexOf("/") + 1) + "/" + this.wb_info.url;
+        iframe.src = this.wb_info.prefix + this.wb_info.request_ts + "mp_/blob:" + blobIdUrl
     }, Wombat.prototype.isSavedSrcSrcset = function(elem) {
         switch (elem.tagName) {
             case "IMG":
             case "VIDEO":
             case "AUDIO":
                 return true;
             case "SOURCE":
@@ -1064,15 +1076,15 @@
                 break;
             case "FORM":
                 changed = this.rewriteAttr(elem, "poster"), changed = this.rewriteAttr(elem, "action") || changed, changed = this.rewriteAttr(elem, "style") || changed;
                 break;
             case "IFRAME":
                 if (changed = this.rewriteFrameSrc(elem, "src"), this.wb_info.isSW && !changed) {
                     var srcdoc = elem.getAttribute("srcdoc");
-                    if (elem.hasAttribute("srcdoc") && elem.removeAttribute("srcdoc"), srcdoc) elem.src = this.wb_info.prefix + this.wb_info.request_ts + "id_/srcdoc:" + btoa(encodeURIComponent(srcdoc));
+                    if (elem.hasAttribute("srcdoc") && elem.removeAttribute("srcdoc"), srcdoc) this.blobUrlForIframe(elem, srcdoc);
                     else {
                         var src = elem.getAttribute("src");
                         src && src !== "about:blank" || (!src && (elem.__WB_blank = true), elem.src = this.wb_info.prefix + this.wb_info.request_ts + "mp_/about:blank")
                     }
                 }
                 changed = this.rewriteAttr(elem, "style") || changed;
                 break;
@@ -1204,22 +1216,14 @@
         var args, deproxiedThis = this.proxyToObj(fnThis);
         if (argsObj.length > 0 && deproxiedThis.parentElement && deproxiedThis.parentElement.tagName === "STYLE") {
             args = new Array(argsObj.length);
             var dataIndex = argsObj.length - 1;
             dataIndex === 2 ? (args[0] = argsObj[0], args[1] = argsObj[1]) : dataIndex === 1 && (args[0] = argsObj[0]), args[dataIndex] = this.rewriteStyle(argsObj[dataIndex])
         } else args = argsObj;
         return originalFn.__WB_orig_apply ? originalFn.__WB_orig_apply(deproxiedThis, args) : originalFn.apply(deproxiedThis, args)
-    }, Wombat.prototype.rewriteDocWriteWriteln = function(fnThis, originalFn, argsObj) {
-        var string, thisObj = this.proxyToObj(fnThis),
-            argLen = argsObj.length;
-        if (argLen === 0) return originalFn.call(thisObj);
-        string = argLen === 1 ? argsObj[0] : Array.prototype.join.call(argsObj, "");
-        var new_buff = this.rewriteHtml(string, true),
-            res = originalFn.call(thisObj, new_buff);
-        return this.initNewWindowWombat(thisObj.defaultView), res
     }, Wombat.prototype.rewriteChildNodeFn = function(fnThis, originalFn, argsObj) {
         var thisObj = this.proxyToObj(fnThis);
         if (argsObj.length === 0) return originalFn.call(thisObj);
         var newArgs = this.rewriteElementsInArguments(argsObj);
         return originalFn.__WB_orig_apply ? originalFn.__WB_orig_apply(thisObj, newArgs) : originalFn.apply(thisObj, newArgs)
     }, Wombat.prototype.rewriteInsertAdjHTMLOrElemArgs = function(fnThis, originalFn, position, textOrElem, rwHTML) {
         var fnThisObj = this.proxyToObj(fnThis);
@@ -1280,30 +1284,30 @@
                 return wombat.wb_setAttribute ? wombat.wb_setAttribute.call(this, attr, val) : void 0
             },
             getter = function newAttrPropGetter() {
                 var res;
                 return orig_getter ? res = orig_getter.call(this) : wombat.wb_getAttribute && (res = wombat.wb_getAttribute.call(this, attr)), res = wombat.extractOriginalURL(res), this.__WB_blank && res === "about:blank" ? "" : res
             };
         this.defProp(obj, attr, setter, getter)
-    }, Wombat.prototype.overridePropExtract = function(proto, prop, cond) {
+    }, Wombat.prototype.overridePropExtract = function(proto, prop) {
         var orig_getter = this.getOrigGetter(proto, prop),
             wombat = this;
         if (orig_getter) {
-            var new_getter = function overridePropExtractNewGetter() {
+            var new_getter = function() {
                 var obj = wombat.proxyToObj(this),
                     res = orig_getter.call(obj);
-                return !cond || cond(obj) ? wombat.extractOriginalURL(res) : res
+                return wombat.extractOriginalURL(res)
             };
             this.defGetterProp(proto, prop, new_getter)
         }
     }, Wombat.prototype.overrideReferrer = function($document) {
         var orig_getter = this.getOrigGetter($document, "referrer"),
             wombat = this;
         if (orig_getter) {
-            var new_getter = function overridePropExtractNewGetter() {
+            var new_getter = function() {
                 var obj = wombat.proxyToObj(this),
                     $win = this.defaultView;
                 if ($win === $win.__WB_replay_top) return "";
                 var res = orig_getter.call(obj);
                 return wombat.extractOriginalURL(res)
             };
             this.defGetterProp($document, "referrer", new_getter)
@@ -1341,17 +1345,22 @@
         var orig_getter = this.getOrigGetter(obj, attr),
             orig_setter = this.getOrigSetter(obj, attr),
             wombat = this,
             setter = function overrideStyleAttrSetter(orig) {
                 var val = wombat.rewriteStyle(orig);
                 return orig_setter ? orig_setter.call(this, val) : this.setProperty(propName, val), val
             },
-            getter = orig_getter;
+            getter = orig_getter,
+            extractUrl = function(_, p1, p2, p3, p4) {
+                return p1 + (p2 || "") + wombat.extractOriginalURL(p3) + p4
+            },
+            EXTRACT_URL_RX = /(url\()(['"])?(.*?)(\2\))/;
         orig_getter || (getter = function overrideStyleAttrGetter() {
-            return this.getPropertyValue(propName)
+            var res = this.getPropertyValue(propName);
+            return res && res.startsWith("url(") && (res = res.replace(EXTRACT_URL_RX, extractUrl)), res
         }), (orig_setter && orig_getter || propName) && this.defProp(obj, attr, setter, getter)
     }, Wombat.prototype.overrideStyleSetProp = function(style_proto) {
         var orig_setProp = style_proto.setProperty,
             wombat = this;
         style_proto.setProperty = function rwSetProperty(name, value, priority) {
             var rwvalue = wombat.rewriteStyle(value);
             return orig_setProp.call(this, name, rwvalue, priority)
@@ -1383,14 +1392,26 @@
                     getter = function overrideHTMLAssignGetter() {
                         var res = orig_getter.call(this);
                         return this._no_rewrite ? res : res.replace(wb_unrewrite_rx, "")
                     };
                 this.defProp(obj, prop, setter, rewriteGetter ? getter : orig_getter)
             }
         }
+    }, Wombat.prototype.overrideHtmlAssignSrcDoc = function(elem, prop) {
+        var obj = elem.prototype;
+        this.getOrigGetter(obj, prop);
+        var orig_setter = this.getOrigSetter(obj, prop),
+            wombat = this,
+            setter = function overrideSetter(orig) {
+                return this.__wb_srcdoc = orig, wombat.wb_info.isSW ? (wombat.blobUrlForIframe(this, orig), orig) : wombat.rewriteHTMLAssign(this, orig_setter, orig)
+            },
+            getter = function overrideGetter() {
+                return this.__wb_srcdoc
+            };
+        this.defProp(obj, prop, setter, getter)
     }, Wombat.prototype.overrideDataSet = function() {
         var obj = this.$wbwindow.HTMLElement.prototype,
             orig_getter = this.getOrigGetter(obj, "dataset"),
             wombat = this,
             getter = function wrapDataSet() {
                 var dataset = orig_getter.call(this),
                     proxy = new Proxy(dataset, {
@@ -1914,26 +1935,26 @@
                             break;
                         case "object":
                             if (newInput = input, input.url) {
                                 var new_url = wombat.rewriteUrl(input.url);
                                 new_url !== input.url && (newInput = new Request_(new_url, input))
                             } else input.href && (newInput = wombat.rewriteUrl(input.toString(), true));
                     }
-                    return newInitOpts.credentials = "include", new Request_(newInput, newInitOpts)
+                    return newInitOpts.credentials = "include", newInitOpts.referrer && (newInitOpts.referrer = wombat.rewriteUrl(newInitOpts.referrer)), new Request_(newInput, newInitOpts)
                 }
             }(this.$wbwindow.Request), this.$wbwindow.Request.prototype = orig_request.prototype, Object.defineProperty(this.$wbwindow.Request.prototype, "constructor", {
                 value: this.$wbwindow.Request
-            })
+            }), this.overridePropExtract(this.$wbwindow.Request.prototype, "url"), this.overridePropExtract(this.$wbwindow.Request.prototype, "referrer")
         }
         if (this.$wbwindow.Response && this.$wbwindow.Response.prototype) {
             var originalRedirect = this.$wbwindow.Response.prototype.redirect;
             this.$wbwindow.Response.prototype.redirect = function redirect(url, status) {
                 var rwURL = wombat.rewriteUrl(url, true, null, wombat.$wbwindow.document);
                 return originalRedirect.call(this, rwURL, status)
-            }
+            }, this.overridePropExtract(this.$wbwindow.Response.prototype, "url")
         }
         if (this.$wbwindow.EventSource && this.$wbwindow.EventSource.prototype) {
             var origEventSource = this.$wbwindow.EventSource;
             this.$wbwindow.EventSource = function(EventSource_) {
                 return function EventSource(url, configuration) {
                     wombat.domConstructorErrorChecker(this, "EventSource", arguments);
                     var rwURL = url;
@@ -2066,41 +2087,58 @@
                 },
                 domain_getter = function domain() {
                     return this.__wb_domain || this.WB_wombat_location.hostname
                 };
             this.defProp($document, "domain", domain_setter, domain_getter)
         }
     }, Wombat.prototype.initDocWriteOpenCloseOverride = function() {
+        function isSWLoad() {
+            return wombat.wb_info.isSW && wombat.$wbwindow.frameElement
+        }
+
+        function prepForWrite(args) {
+            var string;
+            return args.length === 0 ? "" : (string = args.length === 1 ? args[0] : Array.prototype.join.call(args, ""), string)
+        }
+
+        function docWrite(fnThis, originalFn, string) {
+            if (wombat.$wbwindow, isSWLoad()) return void(wombat._writeBuff += string);
+            string = wombat.rewriteHtml(string, true);
+            var thisObj = wombat.proxyToObj(fnThis),
+                res = originalFn.call(thisObj, string);
+            return wombat.initNewWindowWombat(thisObj.defaultView), res
+        }
         if (this.$wbwindow.DOMParser) {
             var DocumentProto = this.$wbwindow.Document.prototype,
-                $wbDocument = this.$wbwindow.document,
-                docWriteWritelnRWFn = this.rewriteDocWriteWriteln,
+                $wbDocument = this.$wbwindow.document;
+            this._writeBuff = "";
+            var wombat = this,
                 orig_doc_write = $wbDocument.write,
                 new_write = function write() {
-                    return docWriteWritelnRWFn(this, orig_doc_write, arguments)
+                    return docWrite(this, orig_doc_write, prepForWrite(arguments))
                 };
             $wbDocument.write = new_write, DocumentProto.write = new_write;
             var orig_doc_writeln = $wbDocument.writeln,
                 new_writeln = function writeln() {
-                    return docWriteWritelnRWFn(this, orig_doc_writeln, arguments)
+                    return docWrite(this, orig_doc_writeln, prepForWrite(arguments))
                 };
             $wbDocument.writeln = new_writeln, DocumentProto.writeln = new_writeln;
-            var wombat = this,
-                orig_doc_open = $wbDocument.open,
+            var orig_doc_open = $wbDocument.open,
                 new_open = function open() {
                     var res, thisObj = wombat.proxyToObj(this);
                     if (arguments.length === 3) {
                         var rwUrl = wombat.rewriteUrl(arguments[0], false, "mp_");
                         res = orig_doc_open.call(thisObj, rwUrl, arguments[1], arguments[2]), wombat.initNewWindowWombat(res, arguments[0])
-                    } else res = orig_doc_open.call(thisObj), wombat.initNewWindowWombat(thisObj.defaultView);
+                    } else res = orig_doc_open.call(thisObj), isSWLoad() ? wombat._writeBuff = "" : wombat.initNewWindowWombat(thisObj.defaultView);
                     return res
                 };
             $wbDocument.open = new_open, DocumentProto.open = new_open;
             var originalClose = $wbDocument.close,
                 newClose = function close() {
+                    if (wombat._writeBuff) return wombat.blobUrlForIframe(wombat.$wbwindow.frameElement, wombat._writeBuff), void(wombat._writeBuff = "");
                     var thisObj = wombat.proxyToObj(this);
                     return wombat.initNewWindowWombat(thisObj.defaultView), originalClose.__WB_orig_apply ? originalClose.__WB_orig_apply(thisObj, arguments) : originalClose.apply(thisObj, arguments)
                 };
             $wbDocument.close = newClose, DocumentProto.close = newClose;
             var oBodyGetter = this.getOrigGetter(DocumentProto, "body"),
                 oBodySetter = this.getOrigSetter(DocumentProto, "body");
             oBodyGetter && oBodySetter && this.defProp(DocumentProto, "body", function body(newBody) {
@@ -2143,50 +2181,50 @@
             var originalSetInterval = this.$wbwindow.setInterval;
             this.$wbwindow.setInterval = function setInterval() {
                 return rewriteFn(this, originalSetInterval, arguments)
             }, this.$wbwindow.setInterval.__$wbpatched$__ = true
         }
     }, Wombat.prototype.initWorkerOverrides = function() {
         var wombat = this;
-        if (this.$wbwindow.Worker && !this.$wbwindow.Worker._wb_worker_overriden) {
+        if (this.$wbwindow.Worker && !this.$wbwindow.Worker._wb_worker_overridden) {
             var orig_worker = this.$wbwindow.Worker;
             this.$wbwindow.Worker = function(Worker_) {
                 return function Worker(url, options) {
                     return wombat.domConstructorErrorChecker(this, "Worker", arguments), new Worker_(wombat.rewriteWorker(url), options)
                 }
             }(orig_worker), this.$wbwindow.Worker.prototype = orig_worker.prototype, Object.defineProperty(this.$wbwindow.Worker.prototype, "constructor", {
                 value: this.$wbwindow.Worker
-            }), this.$wbwindow.Worker._wb_worker_overriden = true
+            }), this.$wbwindow.Worker._wb_worker_overridden = true
         }
-        if (this.$wbwindow.SharedWorker && !this.$wbwindow.SharedWorker.__wb_sharedWorker_overriden) {
+        if (this.$wbwindow.SharedWorker && !this.$wbwindow.SharedWorker.__wb_sharedWorker_overridden) {
             var oSharedWorker = this.$wbwindow.SharedWorker;
             this.$wbwindow.SharedWorker = function(SharedWorker_) {
                 return function SharedWorker(url, options) {
                     return wombat.domConstructorErrorChecker(this, "SharedWorker", arguments), new SharedWorker_(wombat.rewriteWorker(url), options)
                 }
             }(oSharedWorker), this.$wbwindow.SharedWorker.prototype = oSharedWorker.prototype, Object.defineProperty(this.$wbwindow.SharedWorker.prototype, "constructor", {
                 value: this.$wbwindow.SharedWorker
-            }), this.$wbwindow.SharedWorker.__wb_sharedWorker_overriden = true
+            }), this.$wbwindow.SharedWorker.__wb_sharedWorker_overridden = true
         }
         if (this.$wbwindow.ServiceWorkerContainer && this.$wbwindow.ServiceWorkerContainer.prototype && this.$wbwindow.ServiceWorkerContainer.prototype.register) {
             var orig_register = this.$wbwindow.ServiceWorkerContainer.prototype.register;
             this.$wbwindow.ServiceWorkerContainer.prototype.register = function register(scriptURL, options) {
                 var newScriptURL = new URL(scriptURL, wombat.$wbwindow.document.baseURI).href,
                     mod = wombat.getPageUnderModifier();
                 return options && options.scope ? options.scope = wombat.rewriteUrl(options.scope, false, mod) : options = {
                     scope: wombat.rewriteUrl("/", false, mod)
                 }, orig_register.call(this, wombat.rewriteUrl(newScriptURL, false, "sw_"), options)
             }
         }
-        if (this.$wbwindow.Worklet && this.$wbwindow.Worklet.prototype && this.$wbwindow.Worklet.prototype.addModule && !this.$wbwindow.Worklet.__wb_workerlet_overriden) {
+        if (this.$wbwindow.Worklet && this.$wbwindow.Worklet.prototype && this.$wbwindow.Worklet.prototype.addModule && !this.$wbwindow.Worklet.__wb_workerlet_overridden) {
             var oAddModule = this.$wbwindow.Worklet.prototype.addModule;
             this.$wbwindow.Worklet.prototype.addModule = function addModule(moduleURL, options) {
                 var rwModuleURL = wombat.rewriteUrl(moduleURL, false, "js_");
                 return oAddModule.call(this, rwModuleURL, options)
-            }, this.$wbwindow.Worklet.__wb_workerlet_overriden = true
+            }, this.$wbwindow.Worklet.__wb_workerlet_overridden = true
         }
     }, Wombat.prototype.initLocOverride = function(loc, oSetter, oGetter) {
         if (Object.defineProperty)
             for (var prop, i = 0; i < this.URL_PROPS.length; i++) prop = this.URL_PROPS[i], this.defProp(loc, prop, this.makeSetLocProp(prop, oSetter, oGetter), this.makeGetLocProp(prop, oGetter), true)
     }, Wombat.prototype.initWombatLoc = function(win) {
         if (!(!win || win.WB_wombat_location && win.document.WB_wombat_location)) {
             var wombat_location = new WombatLocation(win.location, this),
@@ -2235,16 +2273,16 @@
                 value: function(thisObj) {
                     return thisObj && thisObj._WB_wombat_obj_proxy ? thisObj._WB_wombat_obj_proxy : thisObj
                 }
             })
         } catch (e) {}
     }, Wombat.prototype.initImportWrapperFunc = function(win) {
         var wombat = this;
-        win.____wb_rewrite_import__ = function(url) {
-            return import(wombat.rewriteUrl(url))
+        win.____wb_rewrite_import__ = function(base, url) {
+            return base && (url = new URL(url, base).href), import(wombat.rewriteUrl(url, false, "esm_"))
         }
     }, Wombat.prototype.overrideGetOwnPropertyNames = function(win) {
         var orig_getOwnPropertyNames = win.Object.getOwnPropertyNames,
             removeProps = [this.WB_CHECK_THIS_FUNC, "WB_wombat_location", "__WB_pmw", "WB_wombat_top", "WB_wombat_eval", "WB_wombat_runEval"];
         try {
             win.Object.defineProperty(win.Object, "getOwnPropertyNames", {
                 value: function(object) {
@@ -2730,15 +2768,15 @@
             };
         this.defProp(this.$wbwindow.Object.prototype, "WB_wombat_runEval", setNoop, function() {
             return runEval
         }), this.defProp(this.$wbwindow.Object.prototype, "WB_wombat_runEval2", setNoop, function() {
             return runEval2
         })
     }, Wombat.prototype.wombatInit = function() {
-        this._internalInit(), this.initCookiePreset(), this.initHistoryOverrides(), this.overrideFunctionApply(this.$wbwindow), this.overrideFunctionBind(this.$wbwindow), this.initDocTitleOverride(), this.initHashChange(), this.wb_opts.skip_postmessage || (this.initPostMessageOverride(this.$wbwindow), this.initMessageEventOverride(this.$wbwindow)), this.initCheckThisFunc(this.$wbwindow), this.initImportWrapperFunc(this.$wbwindow), this.overrideGetOwnPropertyNames(this.$wbwindow), this.initUIEventsOverrides(), this.initDocWriteOpenCloseOverride(), this.initEvalOverride(), this.initHTTPOverrides(), this.initAudioOverride(), this.initFontFaceOverride(this.$wbwindow), this.initWorkerOverrides(), this.initTextNodeOverrides(), this.initCSSOMOverrides(), this.overrideHtmlAssign(this.$wbwindow.Element, "innerHTML", true), this.overrideHtmlAssign(this.$wbwindow.Element, "outerHTML", true), this.overrideHtmlAssign(this.$wbwindow.HTMLIFrameElement, "srcdoc", true), this.overrideHtmlAssign(this.$wbwindow.HTMLStyleElement, "textContent"), this.overrideShadowDom(), this.overridePropExtract(this.$wbwindow.Document.prototype, "URL"), this.overridePropExtract(this.$wbwindow.Document.prototype, "documentURI"), this.overridePropExtract(this.$wbwindow.Node.prototype, "baseURI"), this.overrideAttrProps(), this.overrideDataSet(), this.initInsertAdjacentElementHTMLOverrides(), this.overrideIframeContentAccess("contentWindow"), this.overrideIframeContentAccess("contentDocument"), this.overrideFuncArgProxyToObj(this.$wbwindow.MutationObserver, "observe"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "compareDocumentPosition"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "contains"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "createTreeWalker"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "evaluate", 1), this.overrideFuncArgProxyToObj(this.$wbwindow.XSLTProcessor, "transformToFragment", 1), this.overrideFuncThisProxyToObj(this.$wbwindow, "getComputedStyle", this.$wbwindow), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearTimeout"), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearInterval"), this.overrideFuncThisProxyToObj(this.$wbwindow.EventTarget.prototype, "dispatchEvent"), this.initTimeoutIntervalOverrides(), this.overrideFramesAccess(this.$wbwindow), this.overrideSWAccess(this.$wbwindow), this.initElementGetSetAttributeOverride(), this.initSvgImageOverrides(), this.initAttrOverrides(), this.initCookiesOverride(), this.initCreateElementNSFix(), this.wb_opts.skip_dom || this.initDomOverride(), this.initRegisterUnRegPHOverride(), this.initPresentationRequestOverride(), this.initBeaconOverride(), this.initMiscNavigatorOverrides(), this.initSeededRandom(this.wb_info.wombat_sec), this.initCryptoRandom(), this.initFixedRatio(this.wb_info.pixel_ratio || 1), this.initDateOverride(this.wb_info.wombat_sec), this.initBlobOverride(), this.initWSOverride(), this.initOpenOverride(), this.initDisableNotificationsGeoLocation(), this.initStorageOverride(), this.initCachesOverride(), this.initIndexedDBOverride(), this.initWindowObjProxy(this.$wbwindow), this.initDocumentObjProxy(this.$wbwindow.document);
+        this._internalInit(), this.initCookiePreset(), this.initHistoryOverrides(), this.overrideFunctionApply(this.$wbwindow), this.overrideFunctionBind(this.$wbwindow), this.initDocTitleOverride(), this.initHashChange(), this.wb_opts.skip_postmessage || (this.initPostMessageOverride(this.$wbwindow), this.initMessageEventOverride(this.$wbwindow)), this.initCheckThisFunc(this.$wbwindow), this.initImportWrapperFunc(this.$wbwindow), this.overrideGetOwnPropertyNames(this.$wbwindow), this.initUIEventsOverrides(), this.initDocWriteOpenCloseOverride(), this.initEvalOverride(), this.initHTTPOverrides(), this.initAudioOverride(), this.initFontFaceOverride(this.$wbwindow), this.initWorkerOverrides(), this.initTextNodeOverrides(), this.initCSSOMOverrides(), this.overrideHtmlAssign(this.$wbwindow.Element, "innerHTML", true), this.overrideHtmlAssign(this.$wbwindow.Element, "outerHTML", true), this.overrideHtmlAssignSrcDoc(this.$wbwindow.HTMLIFrameElement, "srcdoc", true), this.overrideHtmlAssign(this.$wbwindow.HTMLStyleElement, "textContent"), this.overrideShadowDom(), this.overridePropExtract(this.$wbwindow.Document.prototype, "URL"), this.overridePropExtract(this.$wbwindow.Document.prototype, "documentURI"), this.overridePropExtract(this.$wbwindow.Node.prototype, "baseURI"), this.overrideAttrProps(), this.overrideDataSet(), this.initInsertAdjacentElementHTMLOverrides(), this.overrideIframeContentAccess("contentWindow"), this.overrideIframeContentAccess("contentDocument"), this.overrideFuncArgProxyToObj(this.$wbwindow.MutationObserver, "observe"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "compareDocumentPosition"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "contains"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "createTreeWalker"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "evaluate", 1), this.overrideFuncArgProxyToObj(this.$wbwindow.XSLTProcessor, "transformToFragment", 1), this.overrideFuncThisProxyToObj(this.$wbwindow, "getComputedStyle", this.$wbwindow), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearTimeout"), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearInterval"), this.overrideFuncThisProxyToObj(this.$wbwindow.EventTarget.prototype, "dispatchEvent"), this.initTimeoutIntervalOverrides(), this.overrideFramesAccess(this.$wbwindow), this.overrideSWAccess(this.$wbwindow), this.initElementGetSetAttributeOverride(), this.initSvgImageOverrides(), this.initAttrOverrides(), this.initCookiesOverride(), this.initCreateElementNSFix(), this.wb_opts.skip_dom || this.initDomOverride(), this.initRegisterUnRegPHOverride(), this.initPresentationRequestOverride(), this.initBeaconOverride(), this.initMiscNavigatorOverrides(), this.initSeededRandom(this.wb_info.wombat_sec), this.initCryptoRandom(), this.initFixedRatio(this.wb_info.pixel_ratio || 1), this.initDateOverride(this.wb_info.wombat_sec), this.initBlobOverride(), this.initWSOverride(), this.initOpenOverride(), this.initDisableNotificationsGeoLocation(), this.initStorageOverride(), this.initCachesOverride(), this.initIndexedDBOverride(), this.initWindowObjProxy(this.$wbwindow), this.initDocumentObjProxy(this.$wbwindow.document);
         var wombat = this;
         return {
             extract_orig: this.extractOriginalURL,
             rewrite_url: this.rewriteUrl,
             watch_elem: this.watchElem,
             init_new_window_wombat: this.initNewWindowWombat,
             init_paths: this.initPaths,
```

### Comparing `pywb-2.7.3/pywb/static/wombatProxyMode.js` & `pywb-2.7.4/pywb/static/wombatProxyMode.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/wombatWorkers.js` & `pywb-2.7.4/pywb/static/wombatWorkers.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/static/zoom-out-icon-333316.png` & `pywb-2.7.4/pywb/static/zoom-out-icon-333316.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/banner.html` & `pywb-2.7.4/pywb/templates/banner.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/base.html` & `pywb-2.7.4/pywb/templates/base.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/error.html` & `pywb-2.7.4/pywb/templates/error.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/frame_insert.html` & `pywb-2.7.4/pywb/templates/frame_insert.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/head_insert.html` & `pywb-2.7.4/pywb/templates/head_insert.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/header.html` & `pywb-2.7.4/pywb/templates/header.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/index.html` & `pywb-2.7.4/pywb/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/instructions.html` & `pywb-2.7.4/pywb/templates/instructions.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/not_found.html` & `pywb-2.7.4/pywb/templates/not_found.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/proxy_cert_download.html` & `pywb-2.7.4/pywb/templates/proxy_cert_download.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/proxy_select.html` & `pywb-2.7.4/pywb/templates/proxy_select.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/query.html` & `pywb-2.7.4/pywb/templates/query.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/search.html` & `pywb-2.7.4/pywb/templates/search.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/templates/vue_loc.html` & `pywb-2.7.4/pywb/templates/vue_loc.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/README.md` & `pywb-2.7.4/pywb/utils/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/binsearch.py` & `pywb-2.7.4/pywb/utils/binsearch.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/canonicalize.py` & `pywb-2.7.4/pywb/utils/canonicalize.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/format.py` & `pywb-2.7.4/pywb/utils/format.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/geventserver.py` & `pywb-2.7.4/pywb/utils/geventserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/io.py` & `pywb-2.7.4/pywb/utils/io.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/loaders.py` & `pywb-2.7.4/pywb/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/memento.py` & `pywb-2.7.4/pywb/utils/memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/merge.py` & `pywb-2.7.4/pywb/utils/merge.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/test/test_binsearch.py` & `pywb-2.7.4/pywb/utils/test/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/test/test_loaders.py` & `pywb-2.7.4/pywb/utils/test/test_loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/utils/wbexception.py` & `pywb-2.7.4/pywb/utils/wbexception.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/vueui/src/cdx-simulator/README.md` & `pywb-2.7.4/pywb/vueui/src/cdx-simulator/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/access_checker.py` & `pywb-2.7.4/pywb/warcserver/access_checker.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/amf.py` & `pywb-2.7.4/pywb/warcserver/amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/basewarcserver.py` & `pywb-2.7.4/pywb/warcserver/basewarcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/handlers.py` & `pywb-2.7.4/pywb/warcserver/handlers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/http.py` & `pywb-2.7.4/pywb/warcserver/http.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/aggregator.py` & `pywb-2.7.4/pywb/warcserver/index/aggregator.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/cdxobject.py` & `pywb-2.7.4/pywb/warcserver/index/cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/cdxops.py` & `pywb-2.7.4/pywb/warcserver/index/cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/fuzzymatcher.py` & `pywb-2.7.4/pywb/warcserver/index/fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/indexsource.py` & `pywb-2.7.4/pywb/warcserver/index/indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/query.py` & `pywb-2.7.4/pywb/warcserver/index/query.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_cdxobject.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_cdxops.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_dir_agg.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_dir_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_fuzzymatcher.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_indexsource.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_lazy_ops.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_lazy_ops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_memento_agg.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_memento_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_redis_agg.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_redis_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_timeouts.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_xmlquery_indexsource.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_xmlquery_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/test/test_zipnum.py` & `pywb-2.7.4/pywb/warcserver/index/test/test_zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/index/zipnum.py` & `pywb-2.7.4/pywb/warcserver/index/zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/inputrequest.py` & `pywb-2.7.4/pywb/warcserver/inputrequest.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/blockrecordloader.py` & `pywb-2.7.4/pywb/warcserver/resource/blockrecordloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/pathresolvers.py` & `pywb-2.7.4/pywb/warcserver/resource/pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/resolvingloader.py` & `pywb-2.7.4/pywb/warcserver/resource/resolvingloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/responseloader.py` & `pywb-2.7.4/pywb/warcserver/resource/responseloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/test/test_loading.py` & `pywb-2.7.4/pywb/warcserver/resource/test/test_loading.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/resource/test/test_pathresolvers.py` & `pywb-2.7.4/pywb/warcserver/resource/test/test_pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_access.py` & `pywb-2.7.4/pywb/warcserver/test/test_access.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_amf.py` & `pywb-2.7.4/pywb/warcserver/test/test_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_handlers.py` & `pywb-2.7.4/pywb/warcserver/test/test_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,15 +381,16 @@
         resp = self.testapp.get('/urlagnost/resource?url=http://example.com/&param.arg=foo')
 
         assert resp.status_int == 200
         assert resp.headers['Link'] == MementoUtils.make_link('http://test@example.com/', 'original')
         assert resp.headers['Warcserver-Source-Coll'] == 'url-agnost'
         assert resp.headers['Memento-Datetime'] == 'Mon, 29 Jul 2013 19:51:51 GMT'
 
-    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    @pytest.mark.skip("youtube-dl update needed")
     def test_live_video_loader(self):
         pytest.importorskip('youtube_dl')
         params = {'url': 'http://www.youtube.com/v/BfBgWtAIbRc',
                   'content_type': 'application/vnd.youtube-dl_formats+json'
                  }
 
         resp = self.testapp.get('/live/resource', params=params)
@@ -400,15 +401,16 @@
 
         assert resp.headers['Link'] == MementoUtils.make_link('metadata://www.youtube.com/v/BfBgWtAIbRc', 'original')
         assert resp.headers['Memento-Datetime'] != ''
 
         assert b'WARC-Type: metadata' in resp.body
         assert b'Content-Type: application/vnd.youtube-dl_formats+json' in resp.body
 
-    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    @pytest.mark.skip("youtube-dl update needed")
     def test_live_video_loader_post(self):
         pytest.importorskip('youtube_dl')
         req_data = """\
 GET /v/BfBgWtAIbRc HTTP/1.1
 accept-encoding: gzip, deflate
 accept: */*
 host: www.youtube.com\
```

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_inputreq.py` & `pywb-2.7.4/pywb/warcserver/test/test_inputreq.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_upstream.py` & `pywb-2.7.4/pywb/warcserver/test/test_upstream.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_warcserver.py` & `pywb-2.7.4/pywb/warcserver/test/test_warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/test_warcserver_config.yaml` & `pywb-2.7.4/pywb/warcserver/test/test_warcserver_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/test/testutils.py` & `pywb-2.7.4/pywb/warcserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/upstreamindexsource.py` & `pywb-2.7.4/pywb/warcserver/upstreamindexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb/warcserver/warcserver.py` & `pywb-2.7.4/pywb/warcserver/warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/pywb.egg-info/PKG-INFO` & `pywb-2.7.4/pywb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.7.3
+Version: 2.7.4
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pywb-2.7.3/pywb.egg-info/SOURCES.txt` & `pywb-2.7.4/pywb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/access/pywb.aclj` & `pywb-2.7.4/sample_archive/access/pywb.aclj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdx/bad.cdx` & `pywb-2.7.4/sample_archive/cdx/bad.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdx/dupes.cdx` & `pywb-2.7.4/sample_archive/cdx/dupes.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdx/iana.cdx` & `pywb-2.7.4/sample_archive/cdx/iana.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdx/post-test.cdx` & `pywb-2.7.4/sample_archive/cdx/post-test.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdxj/dupes.cdxj` & `pywb-2.7.4/sample_archive/cdxj/dupes.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdxj/example.cdxj` & `pywb-2.7.4/sample_archive/cdxj/example.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdxj/iana.cdxj` & `pywb-2.7.4/sample_archive/cdxj/iana.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/cdxj/post-test.cdxj` & `pywb-2.7.4/sample_archive/cdxj/post-test.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/text_content/link_headers.yaml` & `pywb-2.7.4/sample_archive/text_content/link_headers.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/text_content/sample_dash.mpd` & `pywb-2.7.4/sample_archive/text_content/sample_dash.mpd`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/text_content/sample_hls.m3u8` & `pywb-2.7.4/sample_archive/text_content/sample_hls.m3u8`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/dupes.warc.gz` & `pywb-2.7.4/sample_archive/warcs/dupes.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-bad.warc.gz.bad` & `pywb-2.7.4/sample_archive/warcs/example-bad.warc.gz.bad`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-extra.warc` & `pywb-2.7.4/sample_archive/warcs/example-extra.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-url-agnostic-orig.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example-url-agnostic-orig.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-url-agnostic-revisit.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example-url-agnostic-revisit.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-wget-1-14.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example-wget-1-14.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example-wpull.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example-wpull.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example.arc` & `pywb-2.7.4/sample_archive/warcs/example.arc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example.arc.gz` & `pywb-2.7.4/sample_archive/warcs/example.arc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example.warc` & `pywb-2.7.4/sample_archive/warcs/example.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/example2.warc.gz` & `pywb-2.7.4/sample_archive/warcs/example2.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/iana.warc.gz` & `pywb-2.7.4/sample_archive/warcs/iana.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/warcs/post-test.warc.gz` & `pywb-2.7.4/sample_archive/warcs/post-test.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/zipcdx/zipnum-sample.cdx.gz` & `pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.cdx.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/sample_archive/zipcdx/zipnum-sample.idx` & `pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.idx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/setup.py` & `pywb-2.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/base_config_test.py` & `pywb-2.7.4/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/config_test.yaml` & `pywb-2.7.4/tests/config_test.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/config_test_access.yaml` & `pywb-2.7.4/tests/config_test_access.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/i18n-data/l337/LC_MESSAGES/messages.po` & `pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/memento_fixture.py` & `pywb-2.7.4/tests/memento_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_acl.py` & `pywb-2.7.4/tests/test_acl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_acl_manager.py` & `pywb-2.7.4/tests/test_acl_manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_auto_colls.py` & `pywb-2.7.4/tests/test_auto_colls.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_cdx_server_app.py` & `pywb-2.7.4/tests/test_cdx_server_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_cert_req.py` & `pywb-2.7.4/tests/test_cert_req.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_cli.py` & `pywb-2.7.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_embargo.py` & `pywb-2.7.4/tests/test_embargo.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_force_https.py` & `pywb-2.7.4/tests/test_force_https.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_integration.py` & `pywb-2.7.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_live_rewriter.py` & `pywb-2.7.4/tests/test_live_rewriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,16 @@
         assert resp.status_int == 400
 
     def test_live_invalid_2(self, fmod_sl):
         resp = self.get('/live/{0}@#$@#$', fmod_sl, status=307)
         resp = resp.follow(status=400)
         assert resp.status_int == 400
 
-    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
+    @pytest.mark.skip("youtube-dl update needed")
     def test_live_video_info(self):
         pytest.importorskip('youtube_dl')
         resp = self.testapp.get('/live/vi_/https://www.youtube.com/watch?v=DjFZyFWSt1M')
         assert resp.status_int == 200
         assert resp.content_type == 'application/vnd.youtube-dl_formats+json', resp.content_type
 
     def test_deflate(self, fmod_sl):
```

### Comparing `pywb-2.7.3/tests/test_locales.py` & `pywb-2.7.4/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_memento.py` & `pywb-2.7.4/tests/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_prefer_header.py` & `pywb-2.7.4/tests/test_prefer_header.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_prefixed_deploy.py` & `pywb-2.7.4/tests/test_prefixed_deploy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_proxy.py` & `pywb-2.7.4/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_range.py` & `pywb-2.7.4/tests/test_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         resp = self.get('/pywb/20140127171250{0}/http://example.com/', fmod, headers=headers)
 
         assert resp.status_int == 206
         assert resp.headers['Accept-Ranges'] == 'bytes'
         assert resp.headers['Content-Range'] == 'bytes 0-200/1270', resp.headers['Content-Range']
         assert resp.content_length == 201, resp.content_length
 
-        assert self.recorder_skip == None
+        assert self.recorder_skip == '1'
 
         assert 'wombat.js' not in resp.text
 
     def test_replay_range_start_end_2(self, fmod):
         headers = [('Range', 'bytes=10-200')]
         resp = self.get('/pywb/20140127171250{0}/http://example.com/', fmod, headers=headers)
```

### Comparing `pywb-2.7.3/tests/test_record_dedup.py` & `pywb-2.7.4/tests/test_record_dedup.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_record_replay.py` & `pywb-2.7.4/tests/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_redirect_classic.py` & `pywb-2.7.4/tests/test_redirect_classic.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_redirect_revisits.py` & `pywb-2.7.4/tests/test_redirect_revisits.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_redirects.py` & `pywb-2.7.4/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_root_coll.py` & `pywb-2.7.4/tests/test_root_coll.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests/test_socks.py` & `pywb-2.7.4/tests/test_socks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .base_config_test import BaseConfigTest, fmod_sl
 
+import sys
 import os
 import pytest
 
 
 # ============================================================================
+@pytest.mark.skipif(sys.version_info >= (3, 10), reason="need to reexamine on py3.10")
 class TestSOCKSProxy(BaseConfigTest):
     @classmethod
     def setup_class(cls):
         pytest.importorskip('socks')
         os.environ['SOCKS_HOST'] = 'localhost'
         os.environ['SOCKS_PORT'] = '0'
```

### Comparing `pywb-2.7.3/tests/test_zipnum_auto_dir.py` & `pywb-2.7.4/tests/test_zipnum_auto_dir.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/fixture.py` & `pywb-2.7.4/tests_disabled/fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/live.py` & `pywb-2.7.4/tests_disabled/live.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/perms_fixture.py` & `pywb-2.7.4/tests_disabled/perms_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/server_mock.py` & `pywb-2.7.4/tests_disabled/server_mock.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/server_thread.py` & `pywb-2.7.4/tests_disabled/server_thread.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_cdxserver.py` & `pywb-2.7.4/tests_disabled/test_cdxserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_config_memento.yaml` & `pywb-2.7.4/tests_disabled/test_config_memento.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_config_proxy_https_cookie.yaml` & `pywb-2.7.4/tests_disabled/test_config_proxy_https_cookie.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_live_proxy.py` & `pywb-2.7.4/tests_disabled/test_live_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_memento.py` & `pywb-2.7.4/tests_disabled/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_perms.py` & `pywb-2.7.4/tests_disabled/test_perms.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_perms_app.py` & `pywb-2.7.4/tests_disabled/test_perms_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_http_auth.py` & `pywb-2.7.4/tests_disabled/test_proxy_http_auth.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_http_cookie.py` & `pywb-2.7.4/tests_disabled/test_proxy_http_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_http_ip.py` & `pywb-2.7.4/tests_disabled/test_proxy_http_ip.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_http_ip_redis.py` & `pywb-2.7.4/tests_disabled/test_proxy_http_ip_redis.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_http_no_banner.py` & `pywb-2.7.4/tests_disabled/test_proxy_http_no_banner.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_proxy_https_cookie.py` & `pywb-2.7.4/tests_disabled/test_proxy_https_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.3/tests_disabled/test_rewrite_content.py` & `pywb-2.7.4/tests_disabled/test_rewrite_content.py`

 * *Files identical despite different names*

