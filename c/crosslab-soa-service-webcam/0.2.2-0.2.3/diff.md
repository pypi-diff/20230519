# Comparing `tmp/crosslab_soa_service_webcam-0.2.2.tar.gz` & `tmp/crosslab_soa_service_webcam-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_webcam-0.2.2.tar", last modified: Wed Apr 19 18:32:35 2023, max compression
+gzip compressed data, was "crosslab_soa_service_webcam-0.2.3.tar", last modified: Fri May 19 08:19:53 2023, max compression
```

## Comparing `crosslab_soa_service_webcam-0.2.2.tar` & `crosslab_soa_service_webcam-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.487181 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/
--rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     1066 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/media.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      151 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/webcam_service.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      555 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:32:35.000000 crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:32:35.490515 crosslab_soa_service_webcam-0.2.2/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      628 2023-04-19 13:37:16.000000 crosslab_soa_service_webcam-0.2.2/tests/test_standard.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      578 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      153 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1165 2023-05-19 07:55:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/media.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      151 2023-04-26 09:19:14.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-03 16:08:17.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)     1051 2023-04-26 09:19:14.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/webcam_service.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      348 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      555 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:19:53.000000 crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:19:53.467347 crosslab_soa_service_webcam-0.2.3/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      641 2023-05-19 07:55:53.000000 crosslab_soa_service_webcam-0.2.3/tests/test_standard.py
```

### Comparing `crosslab_soa_service_webcam-0.2.2/setup.cfg` & `crosslab_soa_service_webcam-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_webcam
-version = 0.2.2
+version = 0.2.3
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Webcam Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/media.py` & `crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 from aiortc import MediaStreamTrack  # type: ignore
 
 
 class UDPTrack(MediaStreamTrack):
     def __init__(self, port: int, kind="video") -> None:
         super().__init__()
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)  # Internet  # UDP
-        self.sock.bind(("", port))
+        self.sock.bind(("0.0.0.0", port))
         self.sock.setblocking(False)
         self.kind = kind
         self.loop = asyncio.get_event_loop()
 
     async def raw_recv(self):
         return await self.loop.sock_recv(self.sock, 2048)
 
     def recv(self):
         return
 
     def stop(self):
-        self.sock.close()
+        pass
+        # self.sock.close() // When we close the socket, the next user would not be able to use it: ERR 9
 
 
 class GstTrack(UDPTrack):
     def __init__(self, pipeline, port: Optional[int] = None, kind="video") -> None:
         if port is None:
             port = random.randint(10000, 65535)
         super().__init__(port, kind)
         subprocess.Popen(
-            f"gst-launch-1.0 {pipeline} ! rtph264pay config-interval=10 mtu=1300 ! udpsink host=127.0.0.1 port={port}",
+            f"gst-launch-1.0 {pipeline} ! rtph264pay config-interval=1 mtu=1300 ! udpsink host=127.0.0.1 port={port}",
             shell=True,
         )
```

### Comparing `crosslab_soa_service_webcam-0.2.2/src/crosslab/soa_services/webcam/webcam_service.py` & `crosslab_soa_service_webcam-0.2.3/src/crosslab/soa_services/webcam/webcam_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.2/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt` & `crosslab_soa_service_webcam-0.2.3/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.2/tests/test_standard.py` & `crosslab_soa_service_webcam-0.2.3/tests/test_standard.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from crosslab.soa_services.webcam.media import UDPTrack
 
 
 @pytest.mark.parametrize("tiebreaker", [True, False])
 def test_teardown_reference_leaks(tiebreaker):
     con = ConnectionStub(tiebreaker)
 
-    stream = UDPTrack(4789)
+    stream = UDPTrack(4789 + tiebreaker)
 
     ws = WebcamService__Producer(stream, "test")
 
     with NoReferenceLeaks("crosslab"):
         ws.setupConnection(con, serviceConfig)
         ws.teardownConnection(con)
         con.close()
```

