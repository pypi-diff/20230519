# Comparing `tmp/p2pd-2.4.0.tar.gz` & `tmp/p2pd-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pd-2.4.0.tar", last modified: Mon May  1 10:41:31 2023, max compression
+gzip compressed data, was "p2pd-2.4.1.tar", last modified: Fri May 19 04:39:19 2023, max compression
```

## Comparing `p2pd-2.4.0.tar` & `p2pd-2.4.1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.788418 p2pd-2.4.0/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.4.0/CREDITS.md
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.4.0/LICENSE
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-04-29 16:38:16.000000 p2pd-2.4.0/MANIFEST.in
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-01 10:41:31.788418 p2pd-2.4.0/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-04-30 09:46:56.000000 p2pd-2.4.0/README.md
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.780418 p2pd-2.4.0/p2pd/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/__init__.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/ack_udp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-30 16:44:28.000000 p2pd-2.4.0/p2pd/base_stream.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/cmd_tools.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/echo_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/errors.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2465 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/http_client_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/http_server_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    19527 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    27256 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22921 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/netiface_extra.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-04-30 16:20:59.000000 p2pd-2.4.0/p2pd/ntp_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-04-30 18:20:16.000000 p2pd-2.4.0/p2pd/p2p_node.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.4.0/p2pd/p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.4.0/p2pd/p2p_protocol.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-04-30 18:51:57.000000 p2pd-2.4.0/p2pd/p2p_utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/rest_api.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7128 2023-05-01 10:13:00.000000 p2pd-2.4.0/p2pd/settings.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    40903 2023-04-30 18:50:50.000000 p2pd-2.4.0/p2pd/tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4366 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/test_init.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-04-30 16:09:18.000000 p2pd-2.4.0/p2pd/turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/turn_defs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/turn_process.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/upnp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16306 2023-04-30 18:46:00.000000 p2pd-2.4.0/p2pd/utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/var_names.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/win_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/win_netifaces.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.780418 p2pd-2.4.0/p2pd.egg-info/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1508 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/SOURCES.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/dependency_links.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      103 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/requires.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/top_level.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      305 2023-04-28 06:42:33.000000 p2pd-2.4.0/requirements.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-01 10:41:31.788418 p2pd-2.4.0/setup.cfg
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-04-30 08:33:33.000000 p2pd-2.4.0/setup.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.788418 p2pd-2.4.0/tests/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_bind.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_cmd.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:08:47.000000 p2pd-2.4.0/tests/test_net_afs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8499 2023-05-01 10:27:39.000000 p2pd-2.4.0/tests/test_p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_p2pd_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1214 2023-04-30 19:03:31.000000 p2pd-2.4.0/tests/test_py_examples.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_rudp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:23:09.000000 p2pd-2.4.0/tests/test_signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1544 2023-04-30 19:07:17.000000 p2pd-2.4.0/tests/test_sock.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_sorted_search.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-04-30 19:14:54.000000 p2pd-2.4.0/tests/test_tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3559 2023-05-01 10:20:05.000000 p2pd-2.4.0/tests/test_turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.516197 p2pd-2.4.1/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.4.1/CREDITS.md
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.4.1/LICENSE
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.4.1/MANIFEST.in
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-19 04:39:19.516197 p2pd-2.4.1/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.4.1/README.md
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.508197 p2pd-2.4.1/p2pd/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/__init__.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/ack_udp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-05-14 07:05:48.000000 p2pd-2.4.1/p2pd/address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-30 16:44:28.000000 p2pd-2.4.1/p2pd/base_stream.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/cmd_tools.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/echo_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/errors.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/http_client_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/http_server_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    21525 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5784 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/name_store.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28663 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/netiface_extra.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/ntp_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/p2p_node.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.4.1/p2pd/p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.4.1/p2pd/p2p_protocol.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/p2p_utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/rest_api.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7678 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/settings.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4766 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/test_init.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/turn_defs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/turn_process.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/upnp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16346 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/var_names.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/win_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.512197 p2pd-2.4.1/p2pd.egg-info/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1529 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/requires.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.4.1/requirements.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-19 04:39:19.516197 p2pd-2.4.1/setup.cfg
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-05-19 04:37:59.000000 p2pd-2.4.1/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.516197 p2pd-2.4.1/tests/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_bind.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_cmd.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_net_afs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9769 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_p2pd_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1258 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_py_examples.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_rudp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2197 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_sock.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_sorted_search.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6770 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_win_netifaces.py
```

### Comparing `p2pd-2.4.0/CREDITS.md` & `p2pd-2.4.1/CREDITS.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/LICENSE` & `p2pd-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/PKG-INFO` & `p2pd-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.4.0
+Version: 2.4.1
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.4.0/README.md` & `p2pd-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/__init__.py` & `p2pd-2.4.1/p2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/ack_udp.py` & `p2pd-2.4.1/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/address.py` & `p2pd-2.4.1/p2pd/address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/base_stream.py` & `p2pd-2.4.1/p2pd/base_stream.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/clock_skew.py` & `p2pd-2.4.1/p2pd/clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/cmd_tools.py` & `p2pd-2.4.1/p2pd/cmd_tools.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/daemon.py` & `p2pd-2.4.1/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/http_server_lib.py` & `p2pd-2.4.1/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/interface.py` & `p2pd-2.4.1/p2pd/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,83 @@
 import sys
 import re
 import platform
 import multiprocessing
+import socket
 from .errors import *
+from .settings import *
 from .route import *
 from .nat import *
 from .route_table import *
 if sys.platform == "win32":
     from .win_netifaces import *
 else:
     import netifaces as netifaces
 
 async def init_p2pd():
+    global ENABLE_UDP
+    global ENABLE_STUN
+
+    # Attempt to get monkey patched netifaces.
     netifaces = Interface.get_netifaces()
-    if netifaces is not None:
-        return netifaces
-    
-    multiprocessing.set_start_method("spawn")
-    if sys.platform == "win32":
-        """
-        loop = get_running_loop()
+    if netifaces is None:
+        multiprocessing.set_start_method("spawn")
+        if sys.platform == "win32":
+            """
+            loop = get_running_loop()
+
+            # This happens if the asyncio REPL is used.
+            # Nested event loops are a work around.
+            if loop is not None:
+                import nest_asyncio
+                nest_asyncio.apply()
+            """
+            netifaces = await Netifaces().start()
+        else:
+            netifaces = sys.modules["netifaces"]
+
+        Interface.get_netifaces = lambda: netifaces
 
-        # This happens if the asyncio REPL is used.
-        # Nested event loops are a work around.
-        if loop is not None:
-            import nest_asyncio
-            nest_asyncio.apply()
+    # Are UDP sockets blocked?
+    # Firewalls like iptables on freehosts can do this.
+    sock = None
+    try:
+        # Figure out what address family default interface supports.
+        _, af = get_default_iface(netifaces)
+        if af == AF_ANY: # Duel stack. Just use v4.
+            af = IP4
+
+        # Set destination based on address family.
+        if af == IP4:
+            dest = ('8.8.8.8', 60000)
+        else:
+            dest = ('2001:4860:4860::8888', 60000)
+
+        # Build new UDP socket.
+        sock = socket.socket(family=af, type=socket.SOCK_DGRAM)
+
+        # Attempt to send small msg to dest.
+        sock.sendto(b'testing UDP. disregard this sorry.', 0, dest)
+    except Exception:
         """
-        netifaces = await Netifaces().start()
-    else:
-        netifaces = sys.modules["netifaces"]
+        Maybe in the future I write code as a fail-safe but for
+        now I don't have time. It's better to show a clear reason
+        why the library won't work then to silently fail.
+        """
+        raise Exception("Error this library needs UDP support to work.")
+    
+
+        ENABLE_UDP = False
+        ENABLE_STUN = False
+        log("UDP sockets blocked! Disabling STUN.")
+        log_exception()
+    finally:
+        if sock is not None:
+            sock.close()
 
-    Interface.get_netifaces = lambda: netifaces
     return netifaces
 
 def get_default_iface(netifaces, preference=AF_ANY, exp=1, duel_stack_test=True):
     gws = netiface_gateways(netifaces, get_interface_type, preference=preference)
     gateway = None
     iface = None
                     
@@ -297,18 +339,26 @@
                             skip_resolve
                         )
                     except NoGatewayForAF:
                         # Empty route pool.
                         self.rp[af] = RoutePool()
                         log(f"No route for gw {af}")
                 
-                tasks.append(helper(af))
+                tasks.append(
+                    asyncio.wait_for(
+                        helper(af),
+                        15
+                    )
+                )
 
             # Get all the routes concurrently.
-            await asyncio.gather(*tasks)
+            try:
+                await asyncio.gather(*tasks)
+            except asyncio.TimeoutError:
+                raise Exception("Could not start iface in 15s.")
         else:
             self.rp = rp
 
         # Update stack type based on routable.
         self.stack = get_interface_stack(self.rp)
         assert(self.stack in VALID_STACKS)
         self.resolved = True
@@ -476,15 +526,30 @@
             continue
 
         route_s = str(interface.rp[af].routes)
         log(f"> AF {af} = {route_s}")
         log(f"> nic() = {interface.route(af).nic()}")
         log(f"> ext() = {interface.route(af).ext()}")
 
-async def load_interfaces(netifaces=None):
+def get_ifs_by_af_intersect(if_list):
+    largest = []
+    af_used = None
+    for af in VALID_AFS:
+        hay = []
+        for iface in if_list:
+            if af in iface.supported():
+                hay.append(iface)
+
+        if len(hay) > len(largest):
+            largest = hay
+            af_used = af
+
+    return [largest, af_used]
+
+async def load_interfaces(netifaces=None, load_nat=True):
     # Get list of good interfaces with ::/0 or 0.0.0.0 routes.
     netifaces = netifaces or Interface.get_netifaces()
     ifs = await filter_trash_interfaces(netifaces)
     ifs = to_unique(ifs)
     if ifs == []:
         # Something must have gone wrong so just use regular netifaces.
         ifs = netifaces.interfaces()
@@ -495,15 +560,16 @@
     for if_name in ifs:
         if_info = str(netifaces.ifaddresses(if_name))
         log(f"Attempt to start if name {if_name}")
         log(f"Net iface results for that if = {if_info}")
         async def worker(if_name):
             try:
                 interface = await Interface(if_name, netifaces=netifaces).start()
-                await interface.load_nat()
+                if load_nat:
+                    await interface.load_nat()
                 if_list.append(interface)
             except Exception:
                 log_exception()
                 return
 
         tasks.append(worker(if_name))
```

### Comparing `p2pd-2.4.0/p2pd/ip_range.py` & `p2pd-2.4.1/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/nat.py` & `p2pd-2.4.1/p2pd/nat.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,14 +448,20 @@
         if range_no >= test_no:
             use_range = r
         else:
             use_range = our_nat["range"]
     else:
         use_range = our_nat["range"]
 
+    # Ensure bind ports don't end up in low port ranges.
+    if use_range[0] < 1024:
+        use_range[0] = 1024
+        if use_range[0] >= use_range[1]:
+            raise Exception("Can't find intersecting port range.")
+        
     return use_range
 
 ###############################################################
 # [ [ local, remote, reply, sock ] ... ]
 async def get_single_mapping(mode, rmap, last_mapped, use_range, our_nat, stun_client):
     # Allow last mapped to be modified from inside func.
     last_local, last_remote = last_mapped
@@ -468,15 +474,15 @@
     Normally the code tries to use the same port as
     the recipient to simplify the code and make things
     more resilient. But if you're trying to punch yourself
     using the same local port will be impossible. Choose
     a non-conflicting port.
     """
     if mode == TCP_PUNCH_SELF:
-        while 1:
+        for _ in range(0, 1000):
             bind_port = random.randrange(2000, MAX_PORT)
             if bind_port != remote_port:
                 break
 
     # If we're port restricted specify we're happy to use their mapping.
     # This may not be possible if our delta is random though.
     our_reply = bind_port if our_nat["type"] == RESTRICT_PORT_NAT else 0
@@ -679,19 +685,40 @@
                 break
             else:
                 their_maps.append([from_range(use_range), 0, 0])
 
     # Set initial mapping needed for delta type NATs.
     last_mapped = [None, None]
     if our_nat["delta"]["type"] in DELTA_N:
-        _, s, local_port, remote_port, _, _ = await stun_client.get_mapping(
-            proto=STREAM
-        )
+        # NOTE: if local < 1024 it may not be possible to reuse.
+        r = stun_client.interface.route(stun_client.af)
+        s = None
+        for i in range(0, 5):
+            try:
+                # Reserve a sock for use.
+                # Close it so it can be used.
+                reserved_sock, high_port = await get_high_port_socket(r, sock_type=TCP)
+                #reserved_sock.close()
+
+                
+                _, s, local_port, remote_port, _, _ = await stun_client.get_mapping(
+                    proto=STREAM,
+                    source_port=high_port
+                )
+
+                #socket.setsockopt(s, socket.SO_REUSEPORT)
+                last_mapped = [local_port, remote_port]
+                break
+            except:
+                log_exception()
+                s = None
+                continue
 
-        last_mapped = [local_port, remote_port]
+        if s is None:
+            raise Exception("high port sock fail in init map punch.")
         stun_socks.append(s)
 
     # Make a list of tasks to build port predictions.
     # Use default ports for client if unknown or try use their ports.
     tasks = []
     results = []
     for i in range(0, test_no):
@@ -786,8 +813,23 @@
         "af": stun_client.af,
         "local": local_ports,
         "remote": remote_ports,
         "reply": reply_ports,
         "stun_socks": stun_socks,
         "default_maps": their_maps,
         "last_mapped": last_mapped
-    }
+    }
+
+"""
+It's extremely important that all predicts are above a certain
+value otherwise admin or root will be needed to bind to the port
+"""
+def nat_check_for_low_ports(map_info):
+    for k in ["local"]:
+        for p in map_info[k]:
+            if p <= 1024:
+                error = f"invalid low port found for mapping {p}"
+                log(error)
+                raise Exception(error)
+
+
+
```

### Comparing `p2pd-2.4.0/p2pd/net.py` & `p2pd-2.4.1/p2pd/net.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     # Non-none = linger value.
     "linger": None,
 
     # Ref to an event loop.
     "loop": None
 }
 
+af_to_v = lambda af: 4 if af == IP4 else 6
 v_to_af = lambda v: IP4 if v == 4 else IP6
 max_cidr = lambda af: 32 if af == IP4 else 128
 
 class FakeSocket():
     def __init__(self, response_bytes):
         self._file = BytesIO(response_bytes)
 
@@ -742,7 +743,33 @@
     except Exception:
         log(f"Could not bind to interface af = {route.af}")
         log(f"sock = {sock}")
         log(bind_tup or route.bind_tup(flag=bind_flag))
         log_exception()
         if sock is not None:
             sock.close()
+
+async def get_high_port_socket(route, sock_type=TCP):
+    # Minimal config to pass socket factory.
+    conf = {
+        "broadcast": False,
+        "linger": None,
+        "sock_proto": 0,
+        "reuse_addr": True
+    }
+
+    # Get a new socket bound to a high order port.
+    for i in range(0, 20):
+        n = rand_rang(2000, MAX_PORT - 1000)
+        await route.bind(n)
+        try:
+            s = await socket_factory(
+                route,
+                sock_type=sock_type,
+                conf=conf
+            )
+        except:
+            continue
+
+        return s, n
+    
+    raise Exception("Could not bind high range port.")
```

### Comparing `p2pd-2.4.0/p2pd/netiface_extra.py` & `p2pd-2.4.1/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/ntp_client.py` & `p2pd-2.4.1/p2pd/ntp_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/p2p_addr.py` & `p2pd-2.4.1/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/p2p_node.py` & `p2pd-2.4.1/p2pd/p2p_node.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/p2p_pipe.py` & `p2pd-2.4.1/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/p2p_protocol.py` & `p2pd-2.4.1/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/p2p_utils.py` & `p2pd-2.4.1/p2pd/p2p_utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/rest_api.py` & `p2pd-2.4.1/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/route.py` & `p2pd-2.4.1/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/route_table.py` & `p2pd-2.4.1/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/settings.py` & `p2pd-2.4.1/p2pd/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from .net import IP4, IP6
+import socket
+IP4 = socket.AF_INET
+IP6 = socket.AF_INET6
 
+ENABLE_STUN = True
+ENABLE_UDP = True
 P2PD_TEST_INFRASTRUCTURE = False
 
 """
 To keep things simple P2PD uses a number of services to
 help facilitate peer-to-peer connections. At the moment
 there is no massive list of servers to use because
 (as I've learned) -- you need to also have a way to
@@ -14,49 +18,67 @@
 Note to any engineers:
 
 If you wanted to run P2PD privately you could simply
 point all of these servers to your private infrastructure.
 """
 
 
+NET_DEBUG_PROVIDERS = {
+    IP4: [
+        "http://net-debug.000webhostapp.com/net_debug.php"
+    ],
+    IP6: [
+        "http://net-debug.000webhostapp.com/net_debug.php"
+    ]
+}
+
+NAME_STORE_PROVIDERS = [
+    {
+        "afs": [IP4, IP6],
+        "url": "http://net-debug.000webhostapp.com/name_store.php"
+    }
+]
+
 """
 Used to lookup what a nodes IP is and do NAT enumeration.
 Supports IPv6 / IPv4 / TCP / UDP -- change IP and port requests.
 
 STUNT servers support TCP.
 STUND servers support UDP.
 """
 STUNT_SERVERS = {
     # Try to use the oldest servers around.
     # Presumably these are the most reliable.
     IP4: [
         # ['p2pd.net', 34780],
-        ['stun.stunprotocol.org', 3478], # 19 Sept 2005
+        ['stunserver.stunprotocol.org', 3478], # 19 Sept 2005
         ['stun.sipnet.ru', 3478], # 19 Sept 2005
         ['stun.1cbit.ru', 3478], # 30 Aug 2017
         ['stun.acronis.com', 3478], # 30 Aug 2017
         ['stun.bitburger.de', 3478], # 30 Aug 2017
         ['stun.innovaphone.com', 3478], # 30 Aug 2017
         ['stun.onthenet.com.au', 3478], # 30 Aug 2017
         ['stun.zepter.ru', 3478], # 30 Aug 2017
         ['stun.siedle.com', 3478], # 12 Apr 2018
     ],
 
     # There's basically none unfortunately.
     IP6: [
         # ['p2pd.net', 34780],
-        ['stun.stunprotocol.org', 3478],
+        ['stunserver.stunprotocol.org', 3478],
     ]
 }
 
+
+
 STUND_SERVERS = {
     # A few aged, OG stun servers/
     IP4: [
         # ['p2pd.net', 34780],
-        ['stun.stunprotocol.org', 3478],
+        ['stunserver.stunprotocol.org', 3478],
         ['stun.voipcheap.co.uk', 3478], # 19 Sept 2005
         ['stun.usfamily.net', 3478], # 19 Sept 2005
         ['stun.ozekiphone.com', 3478], # 19 Sept 2005
         ['stun.voipwise.com', 3478], # 19 Sept 2005
         ['stun.mit.de', 3478], # 19 Sept 2005
         ['stun.hot-chilli.net', 3478], # 14 Aug 2012
         ['stun.counterpath.com', 3478], # 19 Sept 2005
@@ -76,22 +98,28 @@
         ['stun.nexxtmobile.de', 3478], # 13 June 2018
         ['stun.siptrunk.com', 3478], # 1 May 2014 
     ],
 
     # Still not many support IP6 with multiple IPs..
     IP6: [
         # ['p2pd.net', 34780],
-        ['stun.stunprotocol.org', 3478], # 19 Sept 2005
+        ['stunserver.stunprotocol.org', 3478], # 19 Sept 2005
         ['stun.einfachcallback.de', 3478], # 21 Apr 2021
         ['stun.hot-chilli.net', 3478], # 14 Aug 2012
         ['stun.palava.tv', 3478], # 21 Apr 2021
         ['stun.simlar.org', 3478], # 21 Apr 2021
     ]
 }
 
+"""
+stun_test = [["stunserver.stunprotocol.org", 3478]]
+STUNT_SERVERS = { IP4: stun_test, IP6: stun_test }
+STUND_SERVERS = STUNT_SERVERS
+"""
+
 # The main server used to exchange 'signaling' messages.
 # These are messages that help nodes create connections.
 MQTT_SERVERS = [
     # [b"p2pd.net", 1883],
     [b"mqtt.eclipseprojects.io", 1883],
     [b"broker.mqttdashboard.com", 1883],
     [b"test.mosquitto.org", 1883],
```

### Comparing `p2pd-2.4.0/p2pd/signaling.py` & `p2pd-2.4.1/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/stun_client.py` & `p2pd-2.4.1/p2pd/stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/tcp_punch.py` & `p2pd-2.4.1/p2pd/tcp_punch.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,17 @@
         map_info = await get_nat_predictions(
             mode,
             stun_client,
             self.interface.nat,
             dest_nat
         )
 
+        # Sanity check.
+        nat_check_for_low_ports(map_info)
+
         """
         The NAT prediction code tries to choose ports in a way
         where both parties trying to connect can use the same
         remote port. The reason for this is if host A knows that
         host B will also try use the same ports -- then it may
         be able to connect to host B even if host B can't get
         back a message to host A with its remote mappings.
@@ -466,14 +469,17 @@
             mode,
             stun_client,
             self.interface.nat,
             recv_nat,
             their_maps
         )
 
+        # Sanity check.
+        nat_check_for_low_ports(map_info)
+
         # Expect them to use our reply port if set.
         """
         It's possible that the Initiator has already chosen a remote
         port that matches what our reply port will be. In which case
         this code will have no effect. The code intelligently
         selects ports to use based on its partners NAT type.
```

### Comparing `p2pd-2.4.0/p2pd/test_init.py` & `p2pd-2.4.1/p2pd/test_init.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,28 @@
     async def get_mapping(self, proto, af=None, source_port=0, group="map", alt_port=0, do_close=0, fast_fail=0, servers=None, conf=STUN_CONF):
         run_time = time.time()
         local, mapped = self.mappings[self.p]
         out = [self.interface, self.sock, local, mapped, self.rip, run_time]
         self.p = (self.p + 1) % len(self.mappings)
 
         return out
+    
+async def duel_if_setup(netifaces, load_nat=False):
+    # Load interface list.
+    ifs = await load_interfaces(netifaces, load_nat=load_nat)
+    ifs, af = get_ifs_by_af_intersect(ifs)
+    if len(ifs) <= 1:
+        return [], None
+    
+    # Only need at most 2.
+    ifs = ifs[:2]
+    if(ifs[0].route(af).ext() != ifs[1].route(af).ext()):
+        return ifs, af
+    else:
+        return [], None
 
 class FakeNetifaces():
     def __init__(self):
         self.addr_info = None
 
     def set_addr_info(self, addr_info):
         self.addr_info = addr_info
```

### Comparing `p2pd-2.4.0/p2pd/turn_client.py` & `p2pd-2.4.1/p2pd/turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/turn_defs.py` & `p2pd-2.4.1/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/turn_process.py` & `p2pd-2.4.1/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/upnp.py` & `p2pd-2.4.1/p2pd/upnp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/utils.py` & `p2pd-2.4.1/p2pd/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,25 +542,23 @@
 
 # Will be used in sample code to avoid boilerplate.
 def async_test(f, args=[], loop=None):
     #uvloop.install()
     loop = get_loop(loop)
     #if IS_DEBUG:
     #    loop.set_debug(True)
-    loop.set_debug(False)
+    loop.set_debug(True)
 
     # Can have cleanup errors.
-    try:
-        if len(args):
-            loop.run_until_complete(async_wrap_errors(f(*args)))
-        else:
-            loop.run_until_complete(async_wrap_errors(f()))
-        loop.close()
-    except:
-        log_exception()
+    if len(args):
+        loop.run_until_complete(f(*args))
+    else:
+        loop.run_until_complete(f())
+    loop.close()
+ 
 
 async def return_true(result=None):
     return True
             
 # If there's an error that its already in a loop
 # Run nest_asyncio.apply()
 def async_to_sync(f, params=None, loop=None):
@@ -582,14 +580,19 @@
         if version >= 7:
             return asyncio.get_running_loop()
         else:
             return asyncio.get_event_loop()
     except RuntimeError:
         return None
 
+def sqlite_dict_factory(cursor, row):
+    d = {}
+    for idx, col in enumerate(cursor.description):
+        d[col[0]] = row[idx]
+    return d
 
 if __name__ == "__main__": # pragma: no cover
     x = [1, 1]
     y = [2, 2]
     assert(range_intersects(x, y) == False)
 
     x = [1, 2]
```

### Comparing `p2pd-2.4.0/p2pd/var_names.py` & `p2pd-2.4.1/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/win_net.py` & `p2pd-2.4.1/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd/win_netifaces.py` & `p2pd-2.4.1/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/p2pd.egg-info/PKG-INFO` & `p2pd-2.4.1/p2pd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.4.0
+Version: 2.4.1
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.4.0/p2pd.egg-info/SOURCES.txt` & `p2pd-2.4.1/p2pd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ./p2pd/daemon.py
 ./p2pd/echo_server.py
 ./p2pd/errors.py
 ./p2pd/http_client_lib.py
 ./p2pd/http_server_lib.py
 ./p2pd/interface.py
 ./p2pd/ip_range.py
+./p2pd/name_store.py
 ./p2pd/nat.py
 ./p2pd/net.py
 ./p2pd/netiface_extra.py
 ./p2pd/ntp_client.py
 ./p2pd/p2p_addr.py
 ./p2pd/p2p_node.py
 ./p2pd/p2p_pipe.py
```

### Comparing `p2pd-2.4.0/setup.py` & `p2pd-2.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.4.0',
+    version='2.4.1',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

### Comparing `p2pd-2.4.0/tests/test_address.py` & `p2pd-2.4.1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_bind.py` & `p2pd-2.4.1/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_clock_skew.py` & `p2pd-2.4.1/tests/test_clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_cmd.py` & `p2pd-2.4.1/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_daemon.py` & `p2pd-2.4.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_interface.py` & `p2pd-2.4.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_ip_range.py` & `p2pd-2.4.1/tests/test_ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_nat.py` & `p2pd-2.4.1/tests/test_nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_net.py` & `p2pd-2.4.1/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_net_afs.py` & `p2pd-2.4.1/tests/test_net_afs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_p2p_pipe.py` & `p2pd-2.4.1/tests/test_p2p_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 from p2pd.p2p_addr import is_p2p_addr_us
 from p2pd.p2p_node import *
 from p2pd.p2p_utils import *
 from p2pd.p2p_pipe import *
 from p2pd.interface import *
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
-async def test_setup():
+async def test_setup(netifaces=None, ifs=None):
     # Suppress socket unclosed warnings.
     if not hasattr(test_setup, "netifaces"):
-        test_setup.netifaces = await init_p2pd()
+        if netifaces is None:
+            test_setup.netifaces = await init_p2pd()
+        else:
+            test_setup.netifaces = netifaces
         warnings.filterwarnings('ignore', message="unclosed", category=ResourceWarning)
 
     # Static setup because it's fast.
     if not hasattr(test_setup, "ifs"):
         if socket.gethostname() == "p2pd.net":
             test_setup.ifs = P2PD_IFS
         else:
@@ -30,35 +33,39 @@
     if not hasattr(test_setup, "clock_skew"):
         test_setup.clock_skew = (await SysClock(test_setup.ifs[0]).start()).clock_skew
 
     # Load process pool executors.
     pp_executors = await get_pp_executors(workers=2)
 
     # Main node used for testing p2p functionality.
+    node_a_ifs = [ifs[0]] if ifs is not None else test_setup.ifs
     node_a = await start_p2p_node(
         node_id=node_name(b"node_a"),
 
         # Get brand new unassigned listen port.
         # Avoid TIME_WAIT buggy sockets from port reuse.
         port=0,
-        ifs=test_setup.ifs,
+        ifs=node_a_ifs,
         clock_skew=test_setup.clock_skew,
-        pp_executors=pp_executors
+        pp_executors=pp_executors,
+        enable_upnp=False
     )
 
     # Test local punching algorithm.
+    node_b_ifs = [ifs[1  % len(ifs)]] if ifs is not None else test_setup.ifs
     node_b = await start_p2p_node(
         node_id=node_name(b"node_b"),
 
         # Get brand new unassigned listen port.
         # Avoid TIME_WAIT buggy sockets from port reuse.
         port=0,
-        ifs=test_setup.ifs,
+        ifs=node_b_ifs,
         clock_skew=test_setup.clock_skew,
-        pp_executors=pp_executors
+        pp_executors=pp_executors,
+        enable_upnp=False
     )
 
     print(f"Node a = {node_a.p2p_addr}")
     print(f"Node b = {node_b.p2p_addr}")
     return node_a, node_b
 
 async def test_cleanup(node_a, node_b):
@@ -209,32 +216,59 @@
 
         if not found_open:
             print("> Skipping reverse connect test")
             print("> NAT type is not open.\r\n")
 
         await test_cleanup(node_a, node_b)
 
-    async def test_remote_punch(self):
-        if not P2PD_TEST_INFRASTRUCTURE:
+    async def test_remote_punch_duel_ifs(self):
+        # Load interface list.
+        netifaces = await init_p2pd()
+        ifs, af = await duel_if_setup(netifaces, load_nat=True)
+        if af is None:
+            return
+        
+        # Start nodes on different interfaces.
+        node_a, node_b = await test_setup(netifaces, ifs)
+        pipe, _ = await node_a.connect(
+            node_b.address(),
+            strategies=[P2P_PUNCH]
+        )
+
+        # Check if a connection was spawned.
+        self.assertTrue(pipe is not None)
+        pipe_okay = await check_pipe(pipe)
+        self.assertTrue(pipe_okay is not None)
+
+        # Cleanup        
+        if pipe is not None:
+            await pipe.close()
+        await test_cleanup(node_a, node_b)
+
+    async def test_remote_punch(self, netifaces=None, ifs=None, is_optional=False):
+        if not P2PD_TEST_INFRASTRUCTURE and ifs is None:
             return
 
         # If P2PD_NET_ADDR_BYTES is not us then test punching to it.
         log(">>> test_remote_punch")
-        node_a, node_b = await test_setup()
+        node_a, node_b = await test_setup(netifaces, ifs)
         if not is_p2p_addr_us(P2PD_NET_ADDR_BYTES, node_a.if_list):
             # Connect to p2pd.net test server.
             pipe, _ = await node_a.connect(
                 P2PD_NET_ADDR_BYTES,
                 strategies=[P2P_PUNCH]
             )
             self.assertTrue(pipe is not None)
 
             # Test pipe is valid.
             pipe_okay = await check_pipe(pipe)
-            self.assertTrue(pipe_okay)
+            if not pipe_okay and is_optional:
+                log("remote punch failed but was optional.")
+            else:
+                self.assertTrue(pipe_okay)
             await pipe.close()
         else:
             print("> p2pd net addr is us. Skipping remote punch test.")
 
         await test_cleanup(node_a, node_b)
 
     async def test_remote_turn_connect(self):
```

### Comparing `p2pd-2.4.0/tests/test_p2pd_server.py` & `p2pd-2.4.1/tests/test_p2pd_server.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_py_examples.py` & `p2pd-2.4.1/tests/test_py_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,11 +31,13 @@
                     what_exception()
                     assert(0)
 
                 # Run the async callback.
                 coro = globals().get("example")
                 await coro()
 
+            log(f"py example {no} passed")
+
         await asyncio.sleep(.25)
 
 if __name__ == '__main__':
     main()
```

### Comparing `p2pd-2.4.0/tests/test_route.py` & `p2pd-2.4.1/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_route_table.py` & `p2pd-2.4.1/tests/test_route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_rudp.py` & `p2pd-2.4.1/tests/test_rudp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_signaling.py` & `p2pd-2.4.1/tests/test_signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_sock.py` & `p2pd-2.4.1/tests/test_sock.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,14 +40,35 @@
             s, 
             d.tup
         )
 
         if s is not None:
             s.close()
 
+    async def test_high_port_reuse(self):
+        # Config for reuse.
+        conf = copy.deepcopy(NET_CONF)
+        conf["reuse_addr"] = True
+
+        # Load default interface.
+        n = await init_p2pd()
+        i = await Interface(netifaces=n).start_local()
+        r = i.route()
+
+        # Make a new socket bound to a high order port.
+        high_sock, high_port = await get_high_port_socket(r)
+
+        # Make a new socket that shares the same port.
+        r = await i.route().bind(high_port)
+        reuse_sock = await socket_factory(r, conf=conf)
+
+        # Cleanup both socket handles.
+        high_sock.close()
+        reuse_sock.close()
+
 
 
 if __name__ == '__main__':
     main()
 
 """
 one of the nic ips is not working. why would this break the
```

### Comparing `p2pd-2.4.0/tests/test_sorted_search.py` & `p2pd-2.4.1/tests/test_sorted_search.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_stun_client.py` & `p2pd-2.4.1/tests/test_stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_tcp_punch.py` & `p2pd-2.4.1/tests/test_tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.0/tests/test_win_netifaces.py` & `p2pd-2.4.1/tests/test_win_netifaces.py`

 * *Files identical despite different names*

