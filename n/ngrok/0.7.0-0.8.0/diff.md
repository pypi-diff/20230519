# Comparing `tmp/ngrok-0.7.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ngrok-0.8.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2321440 bytes, number of entries: 10
--rw-r--r--  4.6 unx     9828 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       53 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11558 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/license_files/LICENSE-APACHE
--rw-r--r--  4.6 unx     1056 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/license_files/LICENSE-MIT
--rw-r--r--  4.6 unx     5139 b- defN 23-May-09 21:34 ngrok/ngrok_parser.py
--rw-r--r--  4.6 unx      109 b- defN 23-May-09 21:34 ngrok/__init__.py
--rw-r--r--  4.6 unx     6527 b- defN 23-May-09 21:34 ngrok/__main__.py
--rwxr-xr-x  4.6 unx  6248960 b- defN 23-May-09 21:34 ngrok/ngrok.pyd
--rw-r--r--  4.6 unx      805 b- defN 23-May-09 21:34 ngrok-0.7.0.dist-info/RECORD
-10 files, 6284131 bytes uncompressed, 2320078 bytes compressed:  63.1%
+Zip file size: 2392214 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     9950 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx       53 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11558 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE
+-rw-r--r--  4.6 unx     1056 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/license_files/LICENSE-MIT
+-rw-r--r--  4.6 unx     5139 b- defN 23-May-19 21:52 ngrok/ngrok_parser.py
+-rw-r--r--  4.6 unx      109 b- defN 23-May-19 21:52 ngrok/__init__.py
+-rw-r--r--  4.6 unx     6527 b- defN 23-May-19 21:52 ngrok/__main__.py
+-rwxr-xr-x  4.6 unx  6440960 b- defN 23-May-19 21:52 ngrok/ngrok.pyd
+-rw-r--r--  4.6 unx      805 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/RECORD
+10 files, 6476253 bytes uncompressed, 2390852 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: ngrok-0.7.0.dist-info/METADATA
+Filename: ngrok-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: ngrok-0.7.0.dist-info/WHEEL
+Filename: ngrok-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: ngrok-0.7.0.dist-info/entry_points.txt
+Filename: ngrok-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ngrok-0.7.0.dist-info/license_files/LICENSE-APACHE
+Filename: ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE
 Comment: 
 
-Filename: ngrok-0.7.0.dist-info/license_files/LICENSE-MIT
+Filename: ngrok-0.8.0.dist-info/license_files/LICENSE-MIT
 Comment: 
 
 Filename: ngrok/ngrok_parser.py
 Comment: 
 
 Filename: ngrok/__init__.py
 Comment: 
 
 Filename: ngrok/__main__.py
 Comment: 
 
 Filename: ngrok/ngrok.pyd
 Comment: 
 
-Filename: ngrok-0.7.0.dist-info/RECORD
+Filename: ngrok-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ngrok-0.7.0.dist-info/METADATA` & `ngrok-0.8.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok
-Version: 0.7.0
+Version: 0.8.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Utilities
@@ -22,35 +22,35 @@
 License-File: LICENSE-MIT
 Summary: The ngrok Agent SDK for Python
 Keywords: ngrok,python,pypi,pyo3,ingress,networking
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://ngrok.com
-Project-URL: changelog, https://github.com/ngrok/ngrok-py/blob/main/CHANGELOG.md
-Project-URL: repository, https://github.com/ngrok/ngrok-py
+Project-URL: repository, https://github.com/ngrok/ngrok-python
+Project-URL: changelog, https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md
 
 # The ngrok Agent SDK for Python
 
 [![PyPI][pypi-badge]][pypi-url]
 [![Supported Versions][ver-badge]][ver-url]
 [![MIT licensed][mit-badge]][mit-url]
 [![Apache-2.0 licensed][apache-badge]][apache-url]
 [![Continuous integration][ci-badge]][ci-url]
 
 [pypi-badge]: https://img.shields.io/pypi/v/ngrok
 [pypi-url]: https://pypi.org/project/ngrok
 [ver-badge]: https://img.shields.io/pypi/pyversions/ngrok.svg
 [ver-url]: https://pypi.org/project/ngrok
 [mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
-[mit-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-MIT
+[mit-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-MIT
 [apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
-[apache-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-APACHE
-[ci-badge]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml/badge.svg
-[ci-url]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml
+[apache-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-APACHE
+[ci-badge]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml/badge.svg
+[ci-url]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml
 
 **Note: This is beta-quality software. Interfaces may change without warning.**
 
 [ngrok](https://ngrok.com) is a globally distributed reverse proxy commonly used for quickly getting a public URL to a
 service running inside a private network, such as on your local laptop. The ngrok agent is usually
 deployed inside a private network and is used to communicate with the ngrok cloud service.
 
@@ -65,37 +65,37 @@
 The published library is available on
 [PyPI](https://pypi.org/project/ngrok).
 
 ```shell
 python -m pip install ngrok
 ```
 
-ngrok-py officially supports Python 3.7+.
+ngrok-python officially supports Python 3.7+.
 
 # Documentation
 
-A quickstart guide and a full API reference are included in the [ngrok-py Python API documentation](https://ngrok.github.io/ngrok-py/).
+A quickstart guide and a full API reference are included in the [ngrok-python Python API documentation](https://ngrok.github.io/ngrok-python/).
 
 # Quickstart
 
 After you've installed the package, you'll need an Auth Token. Retrieve one on the
 [Auth Token page of your ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken)
 
-There are multiple examples in [the /examples directory](https://github.com/ngrok/ngrok-py/tree/main/examples).
+There are multiple examples in [the /examples directory](https://github.com/ngrok/ngrok-python/tree/main/examples).
 A minimal use-case looks like the following:
 
 ```python
 async def create_tunnel():
     session = await ngrok.NgrokSessionBuilder().authtoken_from_env().connect()
     tunnel = await session.http_endpoint().listen()
     print (f"Ingress established at {tunnel.url()}")
     tunnel.forward_tcp("localhost:9000")
 ```
 
-Or with [the 'connect' convenience function](https://github.com/ngrok/ngrok-py/blob/main/examples/ngrok-connect-minimal.py):
+Or with [the 'connect' convenience function](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-connect-minimal.py):
 
 ```python
 tunnel = ngrok.connect(9000, authtoken_from_env=True)
 print (f"Ingress established at {tunnel.url()}")
 ```
 
 # ASGI Runner - Tunnels to Uvicorn, Gunicorn, Django and More, With No Code
@@ -125,59 +125,59 @@
 # Can use the module name as well, such as:
 python -m ngrok gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --response-header X-Awesome True
 ```
 
 # Examples
 
 ## Frameworks
-* [Aiohttp](https://docs.aiohttp.org) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/aiohttp-ngrok.py)
-* [Django](https://www.djangoproject.com/) - [Single File Example](https://github.com/ngrok/ngrok-py/tree/main/examples/django-single-file.py), [Modify manage.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/manage.py), [Modify asgi.py Example](https://github.com/ngrok/ngrok-py/tree/main/examples/djangosite/djangosite/ngrok-asgi.py), or use the `ngrok-asgi` ASGI Runner discussed above
-* [Flask](https://flask.palletsprojects.com) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/flask-ngrok.py)
+* [Aiohttp](https://docs.aiohttp.org) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/aiohttp-ngrok.py)
+* [Django](https://www.djangoproject.com/) - [Single File Example](https://github.com/ngrok/ngrok-python/tree/main/examples/django-single-file.py), [Modify manage.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/manage.py), [Modify asgi.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/djangosite/ngrok-asgi.py), or use the `ngrok-asgi` ASGI Runner discussed above
+* [Flask](https://flask.palletsprojects.com) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/flask-ngrok.py)
 * [Gunicorn](https://gunicorn.org/) - Use the `ngrok-asgi` ASGI Runner discussed above
-* [Streamlit](https://streamlit.io) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/streamlit/streamlit-ngrok.py)
-* [Tornado](https://www.tornadoweb.org) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/tornado-ngrok.py)
-* [Uvicorn](https://www.uvicorn.org/) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/uvicorn-ngrok.py), or use the `ngrok-asgi` ASGI Runner discussed above
+* [Streamlit](https://streamlit.io) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/streamlit/streamlit-ngrok.py)
+* [Tornado](https://www.tornadoweb.org) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/tornado-ngrok.py)
+* [Uvicorn](https://www.uvicorn.org/) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/uvicorn-ngrok.py), or use the `ngrok-asgi` ASGI Runner discussed above
 
 ## Machine Learning
-* [Gradio](https://gradio.app/) - [ngrok-asgi Example](https://github.com/ngrok/ngrok-py/tree/main/examples/gradio/gradio-asgi.py), [gradio CLI Example](https://github.com/ngrok/ngrok-py/tree/main/examples/gradio/gradio-ngrok.py) sharing machine learning apps
-* [OpenPlayground](https://github.com/nat/openplayground) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/openplayground/run.py) of an LLM playground you can run on your laptop
-* [GPT4ALL](https://github.com/nomic-ai/gpt4all) - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/gpt4all/run.py) of running the [GPT4All-L Snoozy 13B](https://gpt4all.io/index.html) model with a Gradio frontend
+* [Gradio](https://gradio.app/) - [ngrok-asgi Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-asgi.py), [gradio CLI Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-ngrok.py) sharing machine learning apps
+* [OpenPlayground](https://github.com/nat/openplayground) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/openplayground/run.py) of an LLM playground you can run on your laptop
+* [GPT4ALL](https://github.com/nomic-ai/gpt4all) - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gpt4all/run.py) of running the [GPT4All-L Snoozy 13B](https://gpt4all.io/index.html) model with a Gradio frontend
 
 ## Tunnel Types
-* HTTP - [Minimal Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-minimal.py), [Full Configuration Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-http-full.py)
-* Labeled - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-labeled.py)
-* TCP - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tcp.py)
-* TLS - [Example](https://github.com/ngrok/ngrok-py/tree/main/examples/ngrok-tls.py)
+* HTTP - [Minimal Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-minimal.py), [Full Configuration Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-full.py)
+* Labeled - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-labeled.py)
+* TCP - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tcp.py)
+* TLS - [Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tls.py)
 
 # Platform Support
 
 Pre-built binaries are provided on PyPI for the following platforms:
 
 | OS         | i686 | x64 | aarch64 | arm |
 | ---------- | -----|-----|---------|-----|
 | Windows    |   ✓  |  ✓  |    *    |     |
 | MacOS      |      |  ✓  |    ✓    |     |
 | Linux      |      |  ✓  |    ✓    |  ✓  |
 | Linux musl |      |  ✓  |    ✓    |     |
 | FreeBSD    |      |  *  |         |     |
 
-ngrok-py, and [ngrok-rs](https://github.com/ngrok/ngrok-rs/) which it depends on, are open source, so it may be possible to build them for other platforms.
+ngrok-python, and [ngrok-rust](https://github.com/ngrok/ngrok-rust/) which it depends on, are open source, so it may be possible to build them for other platforms.
 
 * Windows-aarch64 will be supported after the next release of [Ring](https://github.com/briansmith/ring/issues/1167).
 * FreeBSD-x64 is built by the release process, but PyPI won't accept BSD flavors.
 
 # Dependencies
 
 This project relies on [PyO3](https://pyo3.rs/), an excellent system to ease development and building of Rust plugins for Python.
 
 Thank you to [OpenIoTHub](https://github.com/OpenIoTHub/ngrok) for handing over the ngrok name on PyPI.
 
 # Change Log
 
-Changes are tracked in [CHANGELOG.md](https://github.com/ngrok/ngrok-py/blob/main/CHANGELOG.md).
+Changes are tracked in [CHANGELOG.md](https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md).
 
 # License
 
 This project is licensed under either of
 
  * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or
    http://www.apache.org/licenses/LICENSE-2.0)
@@ -185,10 +185,10 @@
    http://opensource.org/licenses/MIT)
 
 at your option.
 
 ### Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted
-for inclusion in tokio-core by you, as defined in the Apache-2.0 license, shall be
+for inclusion in ngrok-python by you, as defined in the Apache-2.0 license, shall be
 dual licensed as above, without any additional terms or conditions.
```

## Comparing `ngrok-0.7.0.dist-info/license_files/LICENSE-APACHE` & `ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE`

 * *Files identical despite different names*

## Comparing `ngrok-0.7.0.dist-info/license_files/LICENSE-MIT` & `ngrok-0.8.0.dist-info/license_files/LICENSE-MIT`

 * *Files identical despite different names*

## Comparing `ngrok-0.7.0.dist-info/RECORD` & `ngrok-0.8.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ngrok-0.7.0.dist-info/METADATA,sha256=N9I8hB230AbTgs8Eq3zJAS-uryf8Is3DPTnbTcFpu6Q,9828
-ngrok-0.7.0.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
-ngrok-0.7.0.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
-ngrok-0.7.0.dist-info/license_files/LICENSE-APACHE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ngrok-0.7.0.dist-info/license_files/LICENSE-MIT,sha256=k2H9oRPELrEi8YIKhwwvdIYmJTrpic5YINff621X-Fw,1056
+ngrok-0.8.0.dist-info/METADATA,sha256=NrsvPHGOus_XldonFdfMBdolW5gS3bG2k6mLcOOK-FM,9950
+ngrok-0.8.0.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
+ngrok-0.8.0.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
+ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+ngrok-0.8.0.dist-info/license_files/LICENSE-MIT,sha256=k2H9oRPELrEi8YIKhwwvdIYmJTrpic5YINff621X-Fw,1056
 ngrok/ngrok_parser.py,sha256=To2QN5nmRK_U0t4e_K3FtHwQDsIuhxfgMb3jar2FENc,5139
 ngrok/__init__.py,sha256=SVQFcbYIelbBItRJLTUbvEnhgLsOvauDlC3_hMuj-Ck,109
 ngrok/__main__.py,sha256=3W7zfMZKeAebaaLFZF9K9PQv25K1vMr7YM8lsN6TzCI,6527
-ngrok/ngrok.pyd,sha256=WjTDe7umWInLXxDOnqUJs-QffVM1ET6X6WsrNd71Xok,6248960
-ngrok-0.7.0.dist-info/RECORD,,
+ngrok/ngrok.pyd,sha256=Xa8qbS97jdjnZTPp59AjVejXvz6h2mmtwnW3mJc_teo,6440960
+ngrok-0.8.0.dist-info/RECORD,,
```

