# Comparing `tmp/hagworm-5.5.2.tar.gz` & `tmp/hagworm-5.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.2.tar", last modified: Thu May 18 11:19:47 2023, max compression
+gzip compressed data, was "hagworm-5.5.3.tar", last modified: Fri May 19 06:03:20 2023, max compression
```

## Comparing `hagworm-5.5.2.tar` & `hagworm-5.5.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.457363 hagworm-5.5.2/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.2/LICENSE
--rw-rw-rw-   0        0        0     7515 2023-05-18 11:19:47.456362 hagworm-5.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.351362 hagworm-5.5.2/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.2/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.353362 hagworm-5.5.2/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.359362 hagworm-5.5.2/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.362362 hagworm-5.5.2/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.2/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.2/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.363362 hagworm-5.5.2/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.364362 hagworm-5.5.2/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.2/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.2/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.366362 hagworm-5.5.2/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-18 08:48:52.000000 hagworm-5.5.2/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.402362 hagworm-5.5.2/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.430362 hagworm-5.5.2/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.2/hagworm/extend/asyncio/etcd.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1570 2023-05-18 08:40:46.000000 hagworm-5.5.2/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.2/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.2/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.2/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.434363 hagworm-5.5.2/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.442362 hagworm-5.5.2/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.2/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.445362 hagworm-5.5.2/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.446362 hagworm-5.5.2/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.449362 hagworm-5.5.2/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.455362 hagworm-5.5.2/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.2/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.5.2/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.5.2/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:19:47.373362 hagworm-5.5.2/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7515 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      678 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 11:19:47.000000 hagworm-5.5.2/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 11:19:47.457363 hagworm-5.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-05-18 08:48:32.000000 hagworm-5.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.990197 hagworm-5.5.3/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.3/LICENSE
+-rw-rw-rw-   0        0        0     7515 2023-05-19 06:03:20.990197 hagworm-5.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.874195 hagworm-5.5.3/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.3/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.878196 hagworm-5.5.3/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.884197 hagworm-5.5.3/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.887196 hagworm-5.5.3/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.3/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.3/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.889198 hagworm-5.5.3/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.890196 hagworm-5.5.3/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.3/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.3/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.892196 hagworm-5.5.3/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-19 06:01:12.000000 hagworm-5.5.3/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.931195 hagworm-5.5.3/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.962195 hagworm-5.5.3/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     2432 2023-05-18 10:57:40.000000 hagworm-5.5.3/hagworm/extend/asyncio/etcd.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1570 2023-05-18 08:40:46.000000 hagworm-5.5.3/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12506 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.3/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.3/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.3/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.967194 hagworm-5.5.3/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.974198 hagworm-5.5.3/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     8148 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.3/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.977196 hagworm-5.5.3/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.979195 hagworm-5.5.3/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.982235 hagworm-5.5.3/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.988195 hagworm-5.5.3/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.3/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.5.3/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.5.3/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:03:20.899196 hagworm-5.5.3/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7515 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      701 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-19 06:03:20.000000 hagworm-5.5.3/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:03:20.991196 hagworm-5.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     2372 2023-05-19 05:58:06.000000 hagworm-5.5.3/setup.py
```

### Comparing `hagworm-5.5.2/LICENSE` & `hagworm-5.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/PKG-INFO` & `hagworm-5.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.2
+Version: 5.5.3
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.2/README.md` & `hagworm-5.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/c_extend/math.c` & `hagworm-5.5.3/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.5.3/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/example/fastapi_demo/main.py` & `hagworm-5.5.3/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.3/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/example/fastapi_demo/setting.py` & `hagworm-5.5.3/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/example/main_test.py` & `hagworm-5.5.3/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/base.py` & `hagworm-5.5.3/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.3/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/command.py` & `hagworm-5.5.3/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/etcd.py` & `hagworm-5.5.3/hagworm/extend/asyncio/etcd.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/event.py` & `hagworm-5.5.3/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/file.py` & `hagworm-5.5.3/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/future.py` & `hagworm-5.5.3/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.3/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.3/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.3/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/net.py` & `hagworm-5.5.3/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.3/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/pool.py` & `hagworm-5.5.3/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.3/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.3/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/task.py` & `hagworm-5.5.3/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.3/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/asyncio/zmq.py` & `hagworm-5.5.3/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/base.py` & `hagworm-5.5.3/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/cache.py` & `hagworm-5.5.3/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/compile.py` & `hagworm-5.5.3/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/config.py` & `hagworm-5.5.3/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/crypto.py` & `hagworm-5.5.3/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/error.py` & `hagworm-5.5.3/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/event.py` & `hagworm-5.5.3/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/igraph.py` & `hagworm-5.5.3/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/interface.py` & `hagworm-5.5.3/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/logging.py` & `hagworm-5.5.3/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/media.py` & `hagworm-5.5.3/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/metaclass.py` & `hagworm-5.5.3/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/process.py` & `hagworm-5.5.3/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/qrcode.py` & `hagworm-5.5.3/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/struct.py` & `hagworm-5.5.3/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/text.py` & `hagworm-5.5.3/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/trace.py` & `hagworm-5.5.3/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/transaction.py` & `hagworm-5.5.3/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/extend/validator.py` & `hagworm-5.5.3/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/fastapi/base.py` & `hagworm-5.5.3/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/fastapi/field.py` & `hagworm-5.5.3/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/fastapi/model.py` & `hagworm-5.5.3/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/fastapi/response.py` & `hagworm-5.5.3/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/gunicorn.py` & `hagworm-5.5.3/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/frame/stress_tests.py` & `hagworm-5.5.3/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/static/cacert.pem` & `hagworm-5.5.3/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/third/consul/config.py` & `hagworm-5.5.3/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.3/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.3/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.3/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.3/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.2
+Version: 5.5.3
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.5.2/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.3/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.2/hagworm.egg-info/requires.txt` & `hagworm-5.5.3/hagworm.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 motor==3.0.0
 msgpack==1.0.3
 ntplib==0.4.0
 numpy==1.22.3
 psutil==5.9.0
 pyahocorasick==1.4.4
 pytest-asyncio==0.18.3
+python-dateutil==2.8.2
 python-stdnum==1.17
 python-consul2==0.1.5
 python-multipart==0.0.5
 pyzmq==22.3.0
 qrcode==7.3.1
 texttable==1.6.4
 ujson==5.2.0
```

### Comparing `hagworm-5.5.2/setup.py` & `hagworm-5.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         r'motor==3.0.0',
         r'msgpack==1.0.3',
         r'ntplib==0.4.0',
         r'numpy==1.22.3',
         r'psutil==5.9.0',
         r'pyahocorasick==1.4.4',
         r'pytest-asyncio==0.18.3',
+        r'python-dateutil==2.8.2',
         r'python-stdnum==1.17',
         r'python-consul2==0.1.5',
         r'python-multipart==0.0.5',
         r'pyzmq==22.3.0',
         r'qrcode==7.3.1',
         r'texttable==1.6.4',
         r'ujson==5.2.0',
```

