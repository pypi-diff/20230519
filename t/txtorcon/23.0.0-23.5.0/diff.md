# Comparing `tmp/txtorcon-23.0.0.tar.gz` & `tmp/txtorcon-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txtorcon-23.0.0.tar", last modified: Thu Feb 16 05:58:55 2023, max compression
+gzip compressed data, was "txtorcon-23.5.0.tar", last modified: Fri May 19 01:21:31 2023, max compression
```

## Comparing `txtorcon-23.0.0.tar` & `txtorcon-23.5.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.503877 txtorcon-23.0.0/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1000 2023-02-16 05:50:25.000000 txtorcon-23.0.0/INSTALL
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1056 2018-05-31 18:59:02.000000 txtorcon-23.0.0/LICENSE
--rw-r--r--   0 meejah    (1000) meejah    (1000)      608 2018-05-31 18:59:02.000000 txtorcon-23.0.0/MANIFEST.in
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4254 2023-02-16 05:50:25.000000 txtorcon-23.0.0/Makefile
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5339 2023-02-16 05:58:55.503877 txtorcon-23.0.0/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4344 2023-02-16 05:50:25.000000 txtorcon-23.0.0/README.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5524 2018-05-31 18:59:02.000000 txtorcon-23.0.0/TODO
--rw-r--r--   0 meejah    (1000) meejah    (1000)      178 2020-04-20 02:58:02.000000 txtorcon-23.0.0/dev-requirements.txt
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.479877 txtorcon-23.0.0/docs/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4589 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/Makefile
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.479877 txtorcon-23.0.0/docs/_static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19950 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_static/avatar.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)     6605 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_static/haiku.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)    17398 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_static/logo.png
--rw-r--r--   0 meejah    (1000) meejah    (1000)    28177 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_static/logo.svg
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.479877 txtorcon-23.0.0/docs/_themes/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      142 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/README
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.483878 txtorcon-23.0.0/docs/_themes/alabaster/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      470 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)       80 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/_version.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1844 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/about.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)      314 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/donate.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2668 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/layout.html
--rw-r--r--   0 meejah    (1000) meejah    (1000)      279 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/navigation.html
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.483878 txtorcon-23.0.0/docs/_themes/alabaster/static/
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11069 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/static/alabaster.css_t
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3215 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/static/pygments.css
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4916 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/support.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      927 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/_themes/alabaster/theme.conf
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1630 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/apilinks_sphinxext.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     8715 2022-06-17 19:32:04.000000 txtorcon-23.0.0/docs/conf.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4793 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/examples.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    33022 2020-04-20 02:58:02.000000 txtorcon-23.0.0/docs/guide.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2527 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/hacking.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3021 2022-06-17 19:32:04.000000 txtorcon-23.0.0/docs/index.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7625 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/installing.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1045 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/interop_asyncio.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5919 2022-04-11 22:21:37.000000 txtorcon-23.0.0/docs/introduction.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5144 2023-02-16 05:56:31.000000 txtorcon-23.0.0/docs/release-checklist.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)    38745 2023-02-16 05:57:17.000000 txtorcon-23.0.0/docs/releases.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      210 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-config.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      307 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-controller.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      578 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-endpoints.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      792 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-interface.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1735 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-onion.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      520 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-protocol.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1375 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-socks.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      337 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-state.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      337 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon-util.rst
--rw-r--r--   0 meejah    (1000) meejah    (1000)      487 2018-05-31 18:59:02.000000 txtorcon-23.0.0/docs/txtorcon.rst
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.491877 txtorcon-23.0.0/examples/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      919 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/close_all_circuits.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      726 2019-05-19 12:35:02.000000 txtorcon-23.0.0/examples/connect.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2034 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/disallow_streams_by_port.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      701 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/dns_lookups.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1049 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/hidden_echo.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1985 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/launch_tor.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1339 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/launch_tor2web.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     3524 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/launch_tor_endpoint.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1426 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/launch_tor_endpoint2.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2004 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/launch_tor_unix_sockets.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     4581 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/launch_tor_with_simplehttpd.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      335 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/minimal_endpoint.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)      919 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/monitor.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1294 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/readme.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1249 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/readme2.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1922 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/stem_relay_descriptor.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2589 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/stream_circuit_logger.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2609 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/tor_info.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1636 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/txtorcon.tac
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1562 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_client.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1844 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_client_authenticated.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3068 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/web_client_custom_circuit.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1085 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_client_treq.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3847 2023-02-16 04:46:25.000000 txtorcon-23.0.0/examples/web_onion_service_aiohttp.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3410 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_onion_service_endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2052 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/web_onion_service_ephemeral_auth.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1699 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/web_onion_service_ephemeral_nonanon.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1839 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/web_onion_service_ephemeral_unix.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2296 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_onion_service_filesystem.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1624 2020-06-09 22:27:42.000000 txtorcon-23.0.0/examples/web_onion_service_prop224.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1737 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/web_onion_service_prop224_endpoints_file.py
--rwxr-xr-x   0 meejah    (1000) meejah    (1000)     3598 2018-05-31 18:59:02.000000 txtorcon-23.0.0/examples/webui_server.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1688 2018-05-31 18:59:02.000000 txtorcon-23.0.0/meejah.asc
--rw-r--r--   0 meejah    (1000) meejah    (1000)      242 2020-04-20 02:58:02.000000 txtorcon-23.0.0/requirements.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-02-16 05:58:55.503877 txtorcon-23.0.0/setup.cfg
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3305 2023-02-16 05:50:25.000000 txtorcon-23.0.0/setup.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.495877 txtorcon-23.0.0/test/
--rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1012 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/py3_test_controller.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3083 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/py3_torstate.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     7246 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_addrmap.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1114 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_attacher.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    21276 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_circuit.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53939 2020-04-20 02:58:02.000000 txtorcon-23.0.0/test/test_controller.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    69362 2023-02-16 05:25:43.000000 txtorcon-23.0.0/test/test_endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3568 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_fsm.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      156 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_log.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3586 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_microdesc.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    36953 2019-05-19 12:35:02.000000 txtorcon-23.0.0/test/test_onion.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11110 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_router.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    29691 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_socks.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15183 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_stream.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    61698 2019-05-19 12:35:02.000000 txtorcon-23.0.0/test/test_torconfig.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    42897 2019-05-19 12:35:02.000000 txtorcon-23.0.0/test/test_torcontrolprotocol.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9504 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_torinfo.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    62166 2023-02-16 05:25:43.000000 txtorcon-23.0.0/test/test_torstate.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15482 2021-08-16 20:24:40.000000 txtorcon-23.0.0/test/test_util.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     1429 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/test_util_imports.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3482 2021-08-16 20:24:40.000000 txtorcon-23.0.0/test/test_web.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      435 2018-05-31 18:59:02.000000 txtorcon-23.0.0/test/util.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.475877 txtorcon-23.0.0/twisted/
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.495877 txtorcon-23.0.0/twisted/plugins/
--rw-r--r--   0 meejah    (1000) meejah    (1000)      161 2018-05-31 18:59:02.000000 txtorcon-23.0.0/twisted/plugins/txtorcon_endpoint_parser.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.499877 txtorcon-23.0.0/txtorcon/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4449 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/__init__.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      183 2023-02-16 05:50:25.000000 txtorcon-23.0.0/txtorcon/_metadata.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4485 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/_microdesc_parser.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4045 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/addrmap.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     2956 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/attacher.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    19467 2019-06-17 23:29:41.000000 txtorcon-23.0.0/txtorcon/circuit.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    54935 2023-02-16 05:25:43.000000 txtorcon-23.0.0/txtorcon/controller.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      608 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/controller_py3.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    47724 2021-08-16 20:24:37.000000 txtorcon-23.0.0/txtorcon/endpoints.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    14943 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/interface.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)      569 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/log.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    53398 2019-05-19 12:35:02.000000 txtorcon-23.0.0/txtorcon/onion.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9739 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/router.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    23368 2020-06-09 22:27:42.000000 txtorcon-23.0.0/txtorcon/socks.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     4406 2018-05-31 18:59:02.000000 txtorcon-23.0.0/txtorcon/spaghetti.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    11795 2023-02-16 05:25:43.000000 txtorcon-23.0.0/txtorcon/stream.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3760 2018-09-01 15:43:17.000000 txtorcon-23.0.0/txtorcon/testutil.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    45321 2021-08-16 20:15:09.000000 txtorcon-23.0.0/txtorcon/torconfig.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    37603 2019-05-19 12:35:02.000000 txtorcon-23.0.0/txtorcon/torcontrolprotocol.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     9645 2021-08-06 19:20:26.000000 txtorcon-23.0.0/txtorcon/torinfo.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    38804 2020-04-20 02:58:02.000000 txtorcon-23.0.0/txtorcon/torstate.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)    15709 2019-05-19 12:35:02.000000 txtorcon-23.0.0/txtorcon/util.py
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5766 2018-09-22 09:49:26.000000 txtorcon-23.0.0/txtorcon/web.py
-drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-02-16 05:58:55.503877 txtorcon-23.0.0/txtorcon.egg-info/
--rw-r--r--   0 meejah    (1000) meejah    (1000)     5339 2023-02-16 05:58:55.000000 txtorcon-23.0.0/txtorcon.egg-info/PKG-INFO
--rw-r--r--   0 meejah    (1000) meejah    (1000)     3272 2023-02-16 05:58:55.000000 txtorcon-23.0.0/txtorcon.egg-info/SOURCES.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-02-16 05:58:55.000000 txtorcon-23.0.0/txtorcon.egg-info/dependency_links.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)      304 2023-02-16 05:58:55.000000 txtorcon-23.0.0/txtorcon.egg-info/requires.txt
--rw-r--r--   0 meejah    (1000) meejah    (1000)       17 2023-02-16 05:58:55.000000 txtorcon-23.0.0/txtorcon.egg-info/top_level.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.507377 txtorcon-23.5.0/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1000 2023-02-16 05:50:25.000000 txtorcon-23.5.0/INSTALL
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1056 2018-05-31 18:59:02.000000 txtorcon-23.5.0/LICENSE
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      608 2018-05-31 18:59:02.000000 txtorcon-23.5.0/MANIFEST.in
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4254 2023-05-19 01:13:45.000000 txtorcon-23.5.0/Makefile
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5362 2023-05-19 01:21:31.507377 txtorcon-23.5.0/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4344 2023-05-19 01:11:14.000000 txtorcon-23.5.0/README.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5524 2018-05-31 18:59:02.000000 txtorcon-23.5.0/TODO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      178 2020-04-20 02:58:02.000000 txtorcon-23.5.0/dev-requirements.txt
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.483377 txtorcon-23.5.0/docs/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4589 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/Makefile
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.483377 txtorcon-23.5.0/docs/_static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19950 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_static/avatar.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6605 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_static/haiku.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    17398 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_static/logo.png
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    28177 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.483377 txtorcon-23.5.0/docs/_themes/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      142 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/README
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.487377 txtorcon-23.5.0/docs/_themes/alabaster/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      470 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       80 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/_version.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1844 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/about.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      314 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/donate.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2668 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/layout.html
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      279 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/navigation.html
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.487377 txtorcon-23.5.0/docs/_themes/alabaster/static/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11069 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/static/alabaster.css_t
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3215 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/static/pygments.css
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4916 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/support.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      927 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/_themes/alabaster/theme.conf
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1630 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/apilinks_sphinxext.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     8715 2022-06-17 19:32:04.000000 txtorcon-23.5.0/docs/conf.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4793 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/examples.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    33022 2020-04-20 02:58:02.000000 txtorcon-23.5.0/docs/guide.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2527 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/hacking.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3021 2022-06-17 19:32:04.000000 txtorcon-23.5.0/docs/index.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7625 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/installing.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1045 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/interop_asyncio.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5919 2022-04-11 22:21:37.000000 txtorcon-23.5.0/docs/introduction.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5163 2023-05-19 01:20:48.000000 txtorcon-23.5.0/docs/release-checklist.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    39522 2023-05-19 01:18:27.000000 txtorcon-23.5.0/docs/releases.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      210 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-config.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      307 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-controller.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      578 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-endpoints.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      792 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-interface.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1735 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-onion.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      520 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-protocol.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1375 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-socks.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      337 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-state.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      337 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon-util.rst
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      487 2018-05-31 18:59:02.000000 txtorcon-23.5.0/docs/txtorcon.rst
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.495377 txtorcon-23.5.0/examples/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      919 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/close_all_circuits.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      726 2019-05-19 12:35:02.000000 txtorcon-23.5.0/examples/connect.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2034 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/disallow_streams_by_port.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      701 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/dns_lookups.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1049 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/hidden_echo.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1985 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/launch_tor.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1339 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/launch_tor2web.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     3524 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/launch_tor_endpoint.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1426 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/launch_tor_endpoint2.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2004 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/launch_tor_unix_sockets.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     4581 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/launch_tor_with_simplehttpd.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      335 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/minimal_endpoint.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)      919 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/monitor.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1294 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/readme.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1249 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/readme2.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     1922 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/stem_relay_descriptor.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2589 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/stream_circuit_logger.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     2609 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/tor_info.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1636 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/txtorcon.tac
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1562 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_client.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1844 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_client_authenticated.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3068 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/web_client_custom_circuit.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1085 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_client_treq.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3847 2023-02-16 04:46:25.000000 txtorcon-23.5.0/examples/web_onion_service_aiohttp.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3410 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_onion_service_endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2052 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/web_onion_service_ephemeral_auth.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1699 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/web_onion_service_ephemeral_nonanon.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1839 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/web_onion_service_ephemeral_unix.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2296 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_onion_service_filesystem.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1624 2020-06-09 22:27:42.000000 txtorcon-23.5.0/examples/web_onion_service_prop224.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1737 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/web_onion_service_prop224_endpoints_file.py
+-rwxr-xr-x   0 meejah    (1000) meejah    (1000)     3598 2018-05-31 18:59:02.000000 txtorcon-23.5.0/examples/webui_server.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1688 2018-05-31 18:59:02.000000 txtorcon-23.5.0/meejah.asc
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      203 2023-05-19 01:11:14.000000 txtorcon-23.5.0/requirements.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       38 2023-05-19 01:21:31.507377 txtorcon-23.5.0/setup.cfg
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3334 2023-05-19 01:11:14.000000 txtorcon-23.5.0/setup.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.499377 txtorcon-23.5.0/test/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        0 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1012 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/py3_test_controller.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3083 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/py3_torstate.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     7246 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_addrmap.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1114 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_attacher.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    21276 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_circuit.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53939 2020-04-20 02:58:02.000000 txtorcon-23.5.0/test/test_controller.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    69362 2023-02-16 05:25:43.000000 txtorcon-23.5.0/test/test_endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3568 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_fsm.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      156 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_log.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3586 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_microdesc.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    36953 2019-05-19 12:35:02.000000 txtorcon-23.5.0/test/test_onion.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11110 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_router.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    29691 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_socks.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15183 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_stream.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    61698 2019-05-19 12:35:02.000000 txtorcon-23.5.0/test/test_torconfig.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    42897 2019-05-19 12:35:02.000000 txtorcon-23.5.0/test/test_torcontrolprotocol.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9504 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_torinfo.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    62166 2023-02-16 05:25:43.000000 txtorcon-23.5.0/test/test_torstate.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15482 2021-08-16 20:24:40.000000 txtorcon-23.5.0/test/test_util.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     1429 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/test_util_imports.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6433 2023-05-19 01:11:14.000000 txtorcon-23.5.0/test/test_web.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      435 2018-05-31 18:59:02.000000 txtorcon-23.5.0/test/util.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.479377 txtorcon-23.5.0/twisted/
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.499377 txtorcon-23.5.0/twisted/plugins/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      161 2018-05-31 18:59:02.000000 txtorcon-23.5.0/twisted/plugins/txtorcon_endpoint_parser.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.503377 txtorcon-23.5.0/txtorcon/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4449 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/__init__.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      183 2023-05-19 01:13:53.000000 txtorcon-23.5.0/txtorcon/_metadata.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4485 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/_microdesc_parser.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4045 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/addrmap.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     2956 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/attacher.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    19675 2023-05-19 01:11:14.000000 txtorcon-23.5.0/txtorcon/circuit.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    55142 2023-05-19 01:11:14.000000 txtorcon-23.5.0/txtorcon/controller.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      608 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/controller_py3.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    47724 2021-08-16 20:24:37.000000 txtorcon-23.5.0/txtorcon/endpoints.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15096 2023-05-19 01:11:14.000000 txtorcon-23.5.0/txtorcon/interface.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      569 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/log.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    53398 2019-05-19 12:35:02.000000 txtorcon-23.5.0/txtorcon/onion.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9739 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/router.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    23368 2020-06-09 22:27:42.000000 txtorcon-23.5.0/txtorcon/socks.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     4406 2018-05-31 18:59:02.000000 txtorcon-23.5.0/txtorcon/spaghetti.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    11795 2023-02-16 05:25:43.000000 txtorcon-23.5.0/txtorcon/stream.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3760 2018-09-01 15:43:17.000000 txtorcon-23.5.0/txtorcon/testutil.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    45321 2021-08-16 20:15:09.000000 txtorcon-23.5.0/txtorcon/torconfig.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    37603 2019-05-19 12:35:02.000000 txtorcon-23.5.0/txtorcon/torcontrolprotocol.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     9645 2021-08-06 19:20:26.000000 txtorcon-23.5.0/txtorcon/torinfo.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    38804 2020-04-20 02:58:02.000000 txtorcon-23.5.0/txtorcon/torstate.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)    15709 2019-05-19 12:35:02.000000 txtorcon-23.5.0/txtorcon/util.py
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     6531 2023-05-19 01:11:14.000000 txtorcon-23.5.0/txtorcon/web.py
+drwxr-xr-x   0 meejah    (1000) meejah    (1000)        0 2023-05-19 01:21:31.503377 txtorcon-23.5.0/txtorcon.egg-info/
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     5362 2023-05-19 01:21:31.000000 txtorcon-23.5.0/txtorcon.egg-info/PKG-INFO
+-rw-r--r--   0 meejah    (1000) meejah    (1000)     3272 2023-05-19 01:21:31.000000 txtorcon-23.5.0/txtorcon.egg-info/SOURCES.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)        1 2023-05-19 01:21:31.000000 txtorcon-23.5.0/txtorcon.egg-info/dependency_links.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)      261 2023-05-19 01:21:31.000000 txtorcon-23.5.0/txtorcon.egg-info/requires.txt
+-rw-r--r--   0 meejah    (1000) meejah    (1000)       17 2023-05-19 01:21:31.000000 txtorcon-23.5.0/txtorcon.egg-info/top_level.txt
```

### Comparing `txtorcon-23.0.0/INSTALL` & `txtorcon-23.5.0/INSTALL`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/LICENSE` & `txtorcon-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/MANIFEST.in` & `txtorcon-23.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/Makefile` & `txtorcon-23.5.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .PHONY: test html counts coverage sdist clean install doc integration diagrams
 default: test
-VERSION = 23.0.0
+VERSION = 23.5.0
 
 test:
 	PYTHONPATH=. trial --reporter=text test
 
 tox:
 	tox -i http://localhost:3141/root/pypi
```

### Comparing `txtorcon-23.0.0/PKG-INFO` & `txtorcon-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtorcon
-Version: 23.0.0
+Version: 23.5.0
 Summary:      Twisted-based Tor controller client, with state-tracking and     configuration abstractions.     https://txtorcon.readthedocs.org     https://github.com/meejah/txtorcon 
 Home-page: https://github.com/meejah/txtorcon
 Author: meejah
 Author-email: meejah@meejah.ca
 License: MIT
 Keywords: python,twisted,tor,tor controller
 Classifier: Framework :: Twisted
@@ -16,14 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
 
 
@@ -60,15 +61,15 @@
 txtorcon
 ========
 
 - **docs**: https://txtorcon.readthedocs.org or http://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/
 - **code**: https://github.com/meejah/txtorcon
 - ``torsocks git clone git://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/txtorcon.git``
 - MIT-licensed;
-- Python 3.5+, PyPy 5.0.0+;
+- Python 3.8+, PyPy 7.3.7+;
 - depends on
   `Twisted`_,
   `Automat <https://github.com/glyph/automat>`_
 
 
 Ten Thousand Feet
 -----------------
```

### Comparing `txtorcon-23.0.0/README.rst` & `txtorcon-23.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 txtorcon
 ========
 
 - **docs**: https://txtorcon.readthedocs.org or http://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/
 - **code**: https://github.com/meejah/txtorcon
 - ``torsocks git clone git://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/txtorcon.git``
 - MIT-licensed;
-- Python 3.5+, PyPy 5.0.0+;
+- Python 3.8+, PyPy 7.3.7+;
 - depends on
   `Twisted`_,
   `Automat <https://github.com/glyph/automat>`_
 
 
 Ten Thousand Feet
 -----------------
```

### Comparing `txtorcon-23.0.0/TODO` & `txtorcon-23.5.0/TODO`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/Makefile` & `txtorcon-23.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_static/avatar.png` & `txtorcon-23.5.0/docs/_static/avatar.png`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_static/haiku.css` & `txtorcon-23.5.0/docs/_static/haiku.css`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_static/logo.png` & `txtorcon-23.5.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_static/logo.svg` & `txtorcon-23.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/about.html` & `txtorcon-23.5.0/docs/_themes/alabaster/about.html`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/layout.html` & `txtorcon-23.5.0/docs/_themes/alabaster/layout.html`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/static/alabaster.css_t` & `txtorcon-23.5.0/docs/_themes/alabaster/static/alabaster.css_t`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/static/pygments.css` & `txtorcon-23.5.0/docs/_themes/alabaster/static/pygments.css`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/support.py` & `txtorcon-23.5.0/docs/_themes/alabaster/support.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/_themes/alabaster/theme.conf` & `txtorcon-23.5.0/docs/_themes/alabaster/theme.conf`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/apilinks_sphinxext.py` & `txtorcon-23.5.0/docs/apilinks_sphinxext.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/conf.py` & `txtorcon-23.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/examples.rst` & `txtorcon-23.5.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/guide.rst` & `txtorcon-23.5.0/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/hacking.rst` & `txtorcon-23.5.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/index.rst` & `txtorcon-23.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/installing.rst` & `txtorcon-23.5.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/interop_asyncio.rst` & `txtorcon-23.5.0/docs/interop_asyncio.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/introduction.rst` & `txtorcon-23.5.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/release-checklist.rst` & `txtorcon-23.5.0/docs/release-checklist.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
    * tox -e readme_render
 
 * "make pep8" should run cleanly (ideally)
 
 * update docs/releases.rst to reflect upcoming reality
    * blindly make links to the signatures
    * update heading, date
+   * commit it all
 
 * on both signing-machine and build-machine shells:
    * export VERSION=22.0.0
 
 * (if on signing machine) "make dist" and "make dist-sigs"
    * creates:
      dist/txtorcon-${VERSION}.tar.gz.asc
```

### Comparing `txtorcon-23.0.0/docs/releases.rst` & `txtorcon-23.5.0/docs/releases.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,28 @@
 major version being the 2-digit year. The second digit will be
 "non-trivial" releases and the third will be for bugfix releases. So
 the second release in 2019 would be "19.2.0" and a bug-fix release of
 that will be "19.2.1".
 
 See also :ref:`api_stability`.
 
-`git main <https://github.com/meejah/txtorcon>`_ *will likely become v23.1.0*
+`git main <https://github.com/meejah/txtorcon>`_ *will likely become v23.6.0*
+
+
+
+v23.5.0
+-------
+
+May 18, 2023
+
+ * `txtorcon-23.5.0.tar.gz <http://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/txtorcon-23.5.0.tar.gz>`_ (`PyPI <https://pypi.python.org/pypi/txtorcon/23.5.0>`_ (:download:`local-sig </../signatues/txtorcon-23.5.0.tar.gz.asc>` or `github-sig <https://github.com/meejah/txtorcon/blob/main/signatues/txtorcon-23.5.0.tar.gz.asc?raw=true>`_) (`source <https://github.com/meejah/txtorcon/archive/v23.5.0.tar.gz>`_)
+* ``twisted.web.client.Agent`` instances now use the same HTTPS policy by default as ``twisted.web.client.Agent``.
+  It is possible to override this policy with the ``tls_context_factory`` argument, the equivalent to ``Agent``'s ``contextFactory=``.
+* Added support for Python 3.11.
+* No more ipaddress dependency
 
 
 v23.0.0
 -------
 
 February 15, 2023
```

### Comparing `txtorcon-23.0.0/docs/txtorcon-endpoints.rst` & `txtorcon-23.5.0/docs/txtorcon-endpoints.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/txtorcon-interface.rst` & `txtorcon-23.5.0/docs/txtorcon-interface.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/txtorcon-onion.rst` & `txtorcon-23.5.0/docs/txtorcon-onion.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/txtorcon-protocol.rst` & `txtorcon-23.5.0/docs/txtorcon-protocol.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/docs/txtorcon-socks.rst` & `txtorcon-23.5.0/docs/txtorcon-socks.rst`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/close_all_circuits.py` & `txtorcon-23.5.0/examples/close_all_circuits.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/connect.py` & `txtorcon-23.5.0/examples/connect.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/disallow_streams_by_port.py` & `txtorcon-23.5.0/examples/disallow_streams_by_port.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/dns_lookups.py` & `txtorcon-23.5.0/examples/dns_lookups.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/hidden_echo.py` & `txtorcon-23.5.0/examples/hidden_echo.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor.py` & `txtorcon-23.5.0/examples/launch_tor.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor2web.py` & `txtorcon-23.5.0/examples/launch_tor2web.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor_endpoint.py` & `txtorcon-23.5.0/examples/launch_tor_endpoint.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor_endpoint2.py` & `txtorcon-23.5.0/examples/launch_tor_endpoint2.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor_unix_sockets.py` & `txtorcon-23.5.0/examples/launch_tor_unix_sockets.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/launch_tor_with_simplehttpd.py` & `txtorcon-23.5.0/examples/launch_tor_with_simplehttpd.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/monitor.py` & `txtorcon-23.5.0/examples/monitor.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/readme.py` & `txtorcon-23.5.0/examples/readme.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/readme2.py` & `txtorcon-23.5.0/examples/readme2.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/stem_relay_descriptor.py` & `txtorcon-23.5.0/examples/stem_relay_descriptor.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/stream_circuit_logger.py` & `txtorcon-23.5.0/examples/stream_circuit_logger.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/tor_info.py` & `txtorcon-23.5.0/examples/tor_info.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/txtorcon.tac` & `txtorcon-23.5.0/examples/txtorcon.tac`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_client.py` & `txtorcon-23.5.0/examples/web_client.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_client_authenticated.py` & `txtorcon-23.5.0/examples/web_client_authenticated.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_client_custom_circuit.py` & `txtorcon-23.5.0/examples/web_client_custom_circuit.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_client_treq.py` & `txtorcon-23.5.0/examples/web_client_treq.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_aiohttp.py` & `txtorcon-23.5.0/examples/web_onion_service_aiohttp.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_endpoints.py` & `txtorcon-23.5.0/examples/web_onion_service_endpoints.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_ephemeral_auth.py` & `txtorcon-23.5.0/examples/web_onion_service_ephemeral_auth.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_ephemeral_nonanon.py` & `txtorcon-23.5.0/examples/web_onion_service_ephemeral_nonanon.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_ephemeral_unix.py` & `txtorcon-23.5.0/examples/web_onion_service_ephemeral_unix.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_filesystem.py` & `txtorcon-23.5.0/examples/web_onion_service_filesystem.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_prop224.py` & `txtorcon-23.5.0/examples/web_onion_service_prop224.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/web_onion_service_prop224_endpoints_file.py` & `txtorcon-23.5.0/examples/web_onion_service_prop224_endpoints_file.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/examples/webui_server.py` & `txtorcon-23.5.0/examples/webui_server.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/meejah.asc` & `txtorcon-23.5.0/meejah.asc`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/setup.py` & `txtorcon-23.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 sphinx_docs += [join('docs/_static', x) for x in listdir('docs/_static')]
 examples = [x for x in listdir('examples') if x[-3:] == '.py']
 
 setup(
     name='txtorcon',
     version=__version__,
     description=description,
+    python_requires=">=3.8",
 ##    setup_requires="setuptools>=36.2",
     long_description=open('README.rst', 'r').read(),
     keywords=['python', 'twisted', 'tor', 'tor controller'],
     install_requires=open('requirements.txt').readlines(),
     # "pip install -e .[dev]" will install development requirements
     extras_require=dict(
         dev=open('dev-requirements.txt').readlines(),
```

### Comparing `txtorcon-23.0.0/test/py3_test_controller.py` & `txtorcon-23.5.0/test/py3_test_controller.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/py3_torstate.py` & `txtorcon-23.5.0/test/py3_torstate.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_addrmap.py` & `txtorcon-23.5.0/test/test_addrmap.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_attacher.py` & `txtorcon-23.5.0/test/test_attacher.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_circuit.py` & `txtorcon-23.5.0/test/test_circuit.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_controller.py` & `txtorcon-23.5.0/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_endpoints.py` & `txtorcon-23.5.0/test/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_fsm.py` & `txtorcon-23.5.0/test/test_fsm.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_microdesc.py` & `txtorcon-23.5.0/test/test_microdesc.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_onion.py` & `txtorcon-23.5.0/test/test_onion.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_router.py` & `txtorcon-23.5.0/test/test_router.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_socks.py` & `txtorcon-23.5.0/test/test_socks.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_stream.py` & `txtorcon-23.5.0/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_torconfig.py` & `txtorcon-23.5.0/test/test_torconfig.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_torcontrolprotocol.py` & `txtorcon-23.5.0/test/test_torcontrolprotocol.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_torinfo.py` & `txtorcon-23.5.0/test/test_torinfo.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_torstate.py` & `txtorcon-23.5.0/test/test_torstate.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_util.py` & `txtorcon-23.5.0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/test/test_util_imports.py` & `txtorcon-23.5.0/test/test_util_imports.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/__init__.py` & `txtorcon-23.5.0/txtorcon/__init__.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/_microdesc_parser.py` & `txtorcon-23.5.0/txtorcon/_microdesc_parser.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/addrmap.py` & `txtorcon-23.5.0/txtorcon/addrmap.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/attacher.py` & `txtorcon-23.5.0/txtorcon/attacher.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/circuit.py` & `txtorcon-23.5.0/txtorcon/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,31 +260,35 @@
         Returns a Deferred that callback()'s (with this Circuit instance)
         when this circuit hits CLOSED or FAILED.
         """
         if self.state in ['CLOSED', 'FAILED']:
             return defer.succeed(self)
         return self._when_closed.when_fired()
 
-    def web_agent(self, reactor, socks_endpoint, pool=None):
+    def web_agent(self, reactor, socks_endpoint, pool=None, tls_context_factory=None):
         """
         :param socks_endpoint: create one with
             :meth:`txtorcon.TorConfig.create_socks_endpoint`. Can be a
             Deferred.
 
         :param pool: passed on to the Agent (as ``pool=``)
+
+        :param tls_context_factory: A factory for TLS contexts. If ``None``,
+            ``BrowserLikePolicyForHTTPS`` is used.
         """
         # local import because there isn't Agent stuff on some
         # platforms we support, so this will only error if you try
         # this on the wrong platform (pypy [??] and old-twisted)
         from txtorcon import web
         return web.tor_agent(
             reactor,
             socks_endpoint,
             circuit=self,
             pool=pool,
+            tls_context_factory=tls_context_factory,
         )
 
     # XXX should make this API match above web_agent (i.e. pass a
     # socks_endpoint) or change the above...
     def stream_via(self, reactor, host, port,
                    socks_endpoint,
                    use_tls=False):
```

### Comparing `txtorcon-23.0.0/txtorcon/controller.py` & `txtorcon-23.5.0/txtorcon/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,25 +562,28 @@
             instance (even if another controller is connected). If you
             call this more than once you'll get the same TorConfig back.
         """
         if self._config is None:
             self._config = yield TorConfig.from_protocol(self._protocol)
         returnValue(self._config)
 
-    def web_agent(self, pool=None, socks_endpoint=None):
+    def web_agent(self, pool=None, socks_endpoint=None, tls_context_factory=None):
         """
         :param socks_endpoint: If ``None`` (the default), a suitable
             SOCKS port is chosen from our config (or added). If supplied,
             should be a Deferred which fires an IStreamClientEndpoint
             (e.g. the return-value from
             :meth:`txtorcon.TorConfig.socks_endpoint`) or an immediate
             IStreamClientEndpoint You probably don't need to mess with
             this.
 
         :param pool: passed on to the Agent (as ``pool=``)
+
+        :param tls_context_factory: A factory for TLS contexts. If ``None``,
+            ``BrowserLikePolicyForHTTPS`` is used.
         """
         if self._non_anonymous:
             raise Exception(
                 "Cannot use web_agent when in non_anonymous mode"
             )
         # local import since not all platforms have this
         from txtorcon import web
@@ -593,14 +596,15 @@
                     "'socks_endpoint' should be a Deferred or an IStreamClient"
                     "Endpoint (got '{}')".format(type(socks_endpoint))
                 )
         return web.tor_agent(
             self._reactor,
             socks_endpoint,
             pool=pool,
+            tls_context_factory=tls_context_factory
         )
 
     @inlineCallbacks
     def dns_resolve(self, hostname):
         """
         :param hostname: a string
```

### Comparing `txtorcon-23.0.0/txtorcon/controller_py3.py` & `txtorcon-23.5.0/txtorcon/controller_py3.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/endpoints.py` & `txtorcon-23.5.0/txtorcon/endpoints.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/interface.py` & `txtorcon-23.5.0/txtorcon/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,25 +37,28 @@
 
     def create_state(self):
         """
         returns a Deferred that fires with a ready-to-go
         :class:`txtorcon.TorState` instance.
         """
 
-    def web_agent(self, pool=None, _socks_endpoint=None):
+    def web_agent(self, pool=None, socks_endpoint=None, tls_context_factory=None):
         """
-        :param _socks_endpoint: If ``None`` (the default), a suitable
+        :param socks_endpoint: If ``None`` (the default), a suitable
             SOCKS port is chosen from our config (or added). If supplied,
             should be a Deferred which fires an IStreamClientEndpoint
             (e.g. the return-value from
             :meth:`txtorcon.TorConfig.socks_endpoint`) or an immediate
             IStreamClientEndpoint You probably don't need to mess with
             this.
 
         :param pool: passed on to the Agent (as ``pool=``)
+
+        :param tls_context_factory: A factory for TLS contexts. If ``None``,
+            ``BrowserLikePolicyForHTTPS`` is used.
         """
 
     def dns_resolve(self, hostname):
         """
         :param hostname: a string
 
         :returns: a Deferred that calbacks with the hostname as looked-up
```

### Comparing `txtorcon-23.0.0/txtorcon/log.py` & `txtorcon-23.5.0/txtorcon/log.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/onion.py` & `txtorcon-23.5.0/txtorcon/onion.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/router.py` & `txtorcon-23.5.0/txtorcon/router.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/socks.py` & `txtorcon-23.5.0/txtorcon/socks.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/spaghetti.py` & `txtorcon-23.5.0/txtorcon/spaghetti.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/stream.py` & `txtorcon-23.5.0/txtorcon/stream.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/testutil.py` & `txtorcon-23.5.0/txtorcon/testutil.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/torconfig.py` & `txtorcon-23.5.0/txtorcon/torconfig.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/torcontrolprotocol.py` & `txtorcon-23.5.0/txtorcon/torcontrolprotocol.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/torinfo.py` & `txtorcon-23.5.0/txtorcon/torinfo.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/torstate.py` & `txtorcon-23.5.0/txtorcon/torstate.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/util.py` & `txtorcon-23.5.0/txtorcon/util.py`

 * *Files identical despite different names*

### Comparing `txtorcon-23.0.0/txtorcon/web.py` & `txtorcon-23.5.0/txtorcon/web.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import absolute_import
 from __future__ import print_function
 from __future__ import with_statement
 
 from twisted.web.iweb import IAgentEndpointFactory
-from twisted.web.client import Agent
+from twisted.web.client import Agent, BrowserLikePolicyForHTTPS
 from twisted.internet.defer import inlineCallbacks, returnValue, Deferred
 from twisted.internet.endpoints import TCP4ClientEndpoint, UNIXClientEndpoint
 
 from zope.interface import implementer
 
 from txtorcon.socks import TorSocksEndpoint
 from txtorcon.log import txtorlog
 from txtorcon.util import SingleObserver
 
 
 @implementer(IAgentEndpointFactory)
 class _AgentEndpointFactoryUsingTor(object):
-    def __init__(self, reactor, tor_socks_endpoint):
+    def __init__(self, reactor, tor_socks_endpoint, tls_context_factory):
         self._reactor = reactor
         self._proxy_ep = SingleObserver()
         # if _proxy_ep is Deferred, but we get called twice, we must
         # remember the resolved object here
         if isinstance(tor_socks_endpoint, Deferred):
             tor_socks_endpoint.addCallback(self._set_proxy)
         else:
             self._proxy_ep.fire(tor_socks_endpoint)
 
+        if tls_context_factory is None:
+            tls_context_factory = BrowserLikePolicyForHTTPS()
+        self._tls_context_factory = tls_context_factory
+
     def _set_proxy(self, p):
         self._proxy_ep.fire(p)
         return p
 
     def endpointForURI(self, uri):
+        if uri.scheme == b'https':
+            tls = self._tls_context_factory.creatorForNetloc(uri.host, uri.port)
+        else:
+            tls = False
         return TorSocksEndpoint(
             self._proxy_ep.when_fired(),
             uri.host,
             uri.port,
-            tls=(uri.scheme == b'https'),
+            tls=tls,
         )
 
 
 @implementer(IAgentEndpointFactory)
 class _AgentEndpointFactoryForCircuit(object):
-    def __init__(self, reactor, tor_socks_endpoint, circ):
+    def __init__(self, reactor, tor_socks_endpoint, circ, tls_context_factory):
         self._reactor = reactor
         self._socks_ep = tor_socks_endpoint
         self._circ = circ
+        if tls_context_factory is None:
+            tls_context_factory = BrowserLikePolicyForHTTPS()
+        self._tls_context_factory = tls_context_factory
 
     def endpointForURI(self, uri):
         """IAgentEndpointFactory API"""
+        if uri.scheme == b'https':
+            tls = self._tls_context_factory.creatorForNetloc(uri.host, uri.port)
+        else:
+            tls = False
         torsocks = TorSocksEndpoint(
             self._socks_ep,
             uri.host, uri.port,
-            tls=uri.scheme == b'https',
+            tls=tls,
         )
         from txtorcon.circuit import TorCircuitEndpoint
         return TorCircuitEndpoint(
             self._reactor, self._circ._torstate, self._circ, torsocks,
         )
 
 
-def tor_agent(reactor, socks_endpoint, circuit=None, pool=None):
+def tor_agent(reactor, socks_endpoint, circuit=None, pool=None, tls_context_factory=None):
     """
     This is the low-level method used by
     :meth:`txtorcon.Tor.web_agent` and
     :meth:`txtorcon.Circuit.web_agent` -- probably you should call one
     of those instead.
 
     :returns: a Deferred that fires with an object that implements
@@ -79,29 +94,37 @@
     :param circuit: If supplied, a particular circuit to use
 
     :param socks_endpoint: Deferred that fires w/
         IStreamClientEndpoint (or IStreamClientEndpoint instance)
         which points at a SOCKS5 port of our Tor
 
     :param pool: passed on to the Agent (as ``pool=``)
-    """
 
+    :param tls_context_factory: A factory for TLS contexts. If ``None``,
+        ``BrowserLikePolicyForHTTPS`` is used.
+    """
     if socks_endpoint is None:
         raise ValueError(
             "Must provide socks_endpoint as Deferred or IStreamClientEndpoint"
         )
     if circuit is not None:
-        factory = _AgentEndpointFactoryForCircuit(reactor, socks_endpoint, circuit)
+        factory = _AgentEndpointFactoryForCircuit(
+            reactor, socks_endpoint, circuit, tls_context_factory
+        )
     else:
-        factory = _AgentEndpointFactoryUsingTor(reactor, socks_endpoint)
+        factory = _AgentEndpointFactoryUsingTor(
+            reactor, socks_endpoint, tls_context_factory
+        )
+
     return Agent.usingEndpointFactory(reactor, factory, pool=pool)
 
 
 @inlineCallbacks
-def agent_for_socks_port(reactor, torconfig, socks_config, pool=None):
+def agent_for_socks_port(reactor, torconfig, socks_config, pool=None,
+                         tls_context_factory=None):
     """
     This returns a Deferred that fires with an object that implements
     :class:`twisted.web.iweb.IAgent` and is thus suitable for passing
     to ``treq`` as the ``agent=`` kwarg. Of course can be used
     directly; see `using Twisted web cliet
     <http://twistedmatrix.com/documents/current/web/howto/client.html>`_. If
     you have a :class:`txtorcon.Tor` instance already, the preferred
@@ -112,21 +135,18 @@
     :param socks_config: anything valid for Tor's ``SocksPort``
         option. This is generally just a TCP port (e.g. ``9050``), but
         can also be a unix path like so ``unix:/path/to/socket`` (Tor
         has restrictions on the ownership/permissions of the directory
         containing ``socket``). If the given SOCKS option is not
         already available in the underlying Tor instance, it is
         re-configured to add the SOCKS option.
-    """
-    # :param tls: True (the default) will use Twisted's default options
-    #     with the hostname in the URI -- that is, TLS verification
-    #     similar to a Browser. Otherwise, you can pass whatever Twisted
-    #     returns for `optionsForClientTLS
-    #     <https://twistedmatrix.com/documents/current/api/twisted.internet.ssl.optionsForClientTLS.html>`_
 
+    :param tls_context_factory: A factory for TLS contexts. If ``None``,
+        ``BrowserLikePolicyForHTTPS`` is used.
+    """
     socks_config = str(socks_config)  # sadly, all lists are lists-of-strings to Tor :/
     if socks_config not in torconfig.SocksPort:
         txtorlog.msg("Adding SOCKS port '{}' to Tor".format(socks_config))
         torconfig.SocksPort.append(socks_config)
         try:
             yield torconfig.save()
         except Exception as e:
@@ -145,11 +165,13 @@
             host = '127.0.0.1'
             port = int(socks_config)
         socks_ep = TCP4ClientEndpoint(reactor, host, port)
 
     returnValue(
         Agent.usingEndpointFactory(
             reactor,
-            _AgentEndpointFactoryUsingTor(reactor, socks_ep),
+            _AgentEndpointFactoryUsingTor(
+                reactor, socks_ep, tls_context_factory=tls_context_factory
+            ),
             pool=pool,
         )
     )
```

### Comparing `txtorcon-23.0.0/txtorcon.egg-info/PKG-INFO` & `txtorcon-23.5.0/txtorcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtorcon
-Version: 23.0.0
+Version: 23.5.0
 Summary:      Twisted-based Tor controller client, with state-tracking and     configuration abstractions.     https://txtorcon.readthedocs.org     https://github.com/meejah/txtorcon 
 Home-page: https://github.com/meejah/txtorcon
 Author: meejah
 Author-email: meejah@meejah.ca
 License: MIT
 Keywords: python,twisted,tor,tor controller
 Classifier: Framework :: Twisted
@@ -16,14 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
 
 
@@ -60,15 +61,15 @@
 txtorcon
 ========
 
 - **docs**: https://txtorcon.readthedocs.org or http://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/
 - **code**: https://github.com/meejah/txtorcon
 - ``torsocks git clone git://fjblvrw2jrxnhtg67qpbzi45r7ofojaoo3orzykesly2j3c2m3htapid.onion/txtorcon.git``
 - MIT-licensed;
-- Python 3.5+, PyPy 5.0.0+;
+- Python 3.8+, PyPy 7.3.7+;
 - depends on
   `Twisted`_,
   `Automat <https://github.com/glyph/automat>`_
 
 
 Ten Thousand Feet
 -----------------
```

### Comparing `txtorcon-23.0.0/txtorcon.egg-info/SOURCES.txt` & `txtorcon-23.5.0/txtorcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

