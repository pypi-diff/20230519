# Comparing `tmp/aio_dt_protocol-0.9.4.tar.gz` & `tmp/aio_dt_protocol-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-0.9.4.tar", last modified: Tue May 16 08:57:38 2023, max compression
+gzip compressed data, was "aio_dt_protocol-0.9.5.tar", last modified: Fri May 19 17:25:15 2023, max compression
```

## Comparing `aio_dt_protocol-0.9.4.tar` & `aio_dt_protocol-0.9.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.187239 aio_dt_protocol-0.9.4/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-0.9.4/LICENSE
--rw-rw-rw-   0        0        0     6559 2023-05-16 08:57:38.187239 aio_dt_protocol-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     5815 2023-04-06 13:39:16.000000 aio_dt_protocol-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.019294 aio_dt_protocol-0.9.4/aio_dt_protocol/
--rw-rw-rw-   0        0        0    34959 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Actions.py
--rw-rw-rw-   0        0        0    53858 2023-05-16 08:36:51.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Browser.py
--rw-rw-rw-   0        0        0     9971 2023-04-04 10:33:45.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/BrowserEx.py
--rw-rw-rw-   0        0        0    35317 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/DOMElement.py
--rw-rw-rw-   0        0        0    32529 2023-04-05 17:29:55.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Data.py
--rw-rw-rw-   0        0        0    22749 2023-04-06 07:01:02.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Page.py
--rw-rw-rw-   0        0        0    16198 2023-04-06 13:11:03.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/PageEx.py
--rw-rw-rw-   0        0        0      453 2023-05-16 08:36:51.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.186238 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0     3631 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/BackgroundService.py
--rw-rw-rw-   0        0        0    13809 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Browser.py
--rw-rw-rw-   0        0        0     7070 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/CSS.py
--rw-rw-rw-   0        0        0     2045 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Console.py
--rw-rw-rw-   0        0        0    16735 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DOM.py
--rw-rw-rw-   0        0        0     1846 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DeviceOrientation.py
--rw-rw-rw-   0        0        0    24645 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Emulation.py
--rw-rw-rw-   0        0        0    23128 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Fetch.py
--rw-rw-rw-   0        0        0     2066 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Log.py
--rw-rw-rw-   0        0        0    22099 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Network.py
--rw-rw-rw-   0        0        0     2124 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Overlay.py
--rw-rw-rw-   0        0        0    35374 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Page.py
--rw-rw-rw-   0        0        0    32897 2023-04-05 17:56:11.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Runtime.py
--rw-rw-rw-   0        0        0     1712 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/SystemInfo.py
--rw-rw-rw-   0        0        0    17569 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Target.py
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/__init__.py
--rw-rw-rw-   0        0        0     3148 2023-04-05 17:16:11.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     1645 2023-04-06 13:08:53.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.041289 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     6559 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1083 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-0.9.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 08:57:38.189237 aio_dt_protocol-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:25:15.055277 aio_dt_protocol-0.9.5/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0     6559 2023-05-19 17:25:15.056277 aio_dt_protocol-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5815 2023-04-06 13:39:16.000000 aio_dt_protocol-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 17:25:14.839353 aio_dt_protocol-0.9.5/aio_dt_protocol/
+-rw-rw-rw-   0        0        0    34959 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Actions.py
+-rw-rw-rw-   0        0        0    50180 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Browser.py
+-rw-rw-rw-   0        0        0     9971 2023-04-04 10:33:45.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/BrowserEx.py
+-rw-rw-rw-   0        0        0    35317 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/DOMElement.py
+-rw-rw-rw-   0        0        0    32529 2023-04-05 17:29:55.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Data.py
+-rw-rw-rw-   0        0        0    22749 2023-04-06 07:01:02.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Page.py
+-rw-rw-rw-   0        0        0    10249 2023-05-19 09:09:36.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/PageEx.py
+-rw-rw-rw-   0        0        0      363 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:25:15.055277 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0     3631 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/BackgroundService.py
+-rw-rw-rw-   0        0        0    13809 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Browser.py
+-rw-rw-rw-   0        0        0     7070 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/CSS.py
+-rw-rw-rw-   0        0        0     2045 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Console.py
+-rw-rw-rw-   0        0        0    16735 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DOM.py
+-rw-rw-rw-   0        0        0     1846 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DeviceOrientation.py
+-rw-rw-rw-   0        0        0    24645 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Emulation.py
+-rw-rw-rw-   0        0        0    23665 2023-05-19 15:17:07.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Fetch.py
+-rw-rw-rw-   0        0        0     2066 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Log.py
+-rw-rw-rw-   0        0        0    22099 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Network.py
+-rw-rw-rw-   0        0        0     2124 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Overlay.py
+-rw-rw-rw-   0        0        0    35374 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Page.py
+-rw-rw-rw-   0        0        0    32897 2023-04-05 17:56:11.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Runtime.py
+-rw-rw-rw-   0        0        0     1712 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/SystemInfo.py
+-rw-rw-rw-   0        0        0    17569 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Target.py
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-05-19 09:15:55.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     5156 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:25:14.844352 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     6559 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1083 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 17:25:15.057276 aio_dt_protocol-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-0.9.5/setup.py
```

### Comparing `aio_dt_protocol-0.9.4/LICENSE` & `aio_dt_protocol-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/PKG-INFO` & `aio_dt_protocol-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 0.9.4
+Version: 0.9.5
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-0.9.4/README.md` & `aio_dt_protocol-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/Actions.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/Actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/Browser.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/Browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,69 +16,14 @@
 from .Data import TargetConnectionInfo, TargetConnectionType, CommonCallback
 from .exceptions import FlagArgumentContainError
 from .utils import get_request, registry_read_key, log, async_util_call
 
 
 class Browser:
 
-    @staticmethod
-    def FindInstances(for_port: Optional[int] = None, browser: str = "chrome") -> Dict[int, int]:
-        """
-        Используется для обнаружения уже запущенных инстансов браузера в режиме отладки.
-        Более быстрая альтернатива для win32 систем FindInstances() есть в aio_dt_utils.Utils,
-            но она требует установленный пакет pywin32 для использования COM.
-        Например:
-                if browser_instances := Browser.FindInstances():
-                    port, pid = [(k, v) for k, v in browser_instances.items()][0]
-                    browser_instance = Browser(debug_port=port, chrome_pid=pid)
-                else:
-                    browser_instance = Browser()
-
-                # Или для конкретного, известного порта:
-                if browser_instances := Browser.FindInstances(port):
-                    pid = browser_instances[port]
-                    browser_instance = Browser(debug_port=port, chrome_pid=pid)
-                else:
-                    browser_instance = Browser()
-        :param for_port:    - порт, для которого осуществляется поиск.
-        :param browser:     - браузер, для которого запрашивается поиск.
-        :return:            - словарь, ключами которого являются используемые порты запущенных
-                                браузеров, а значениями, их ProcessID, или пустой словарь,
-                                если ничего не найдено.
-                                { 9222: 16017, 9223: 2001, ... }
-        """
-        result = {}
-        if sys.platform == "win32":
-            if "chrome" in browser: browser = "chrome.exe"
-            elif "brave" in browser: browser = "brave.exe"
-            elif "edge" in browser: browser = "msedge.exe"
-            else: ValueError("Not support browser: " + browser)
-            cmd = f"WMIC PROCESS WHERE NAME='{browser}' GET Commandline,Processid"
-            for line in subprocess.Popen(cmd, stdout=subprocess.PIPE).stdout:
-                if b"--type=renderer" not in line and b"--remote-debugging-port=" in line:
-                    port, pid = re.findall(r"--remote-debugging-port=(\d+).*?(\d+)\s*$", line.decode())[0]
-                    port, pid = int(port), int(pid)
-                    if for_port == port: return {port: pid}
-                    result[port] = pid
-        elif sys.platform == "linux":
-            if "chrome" in browser: browser = "google-chrome"
-            elif "brave" in browser: browser = "brave"
-            elif "edge" in browser: browser = "edge"
-            else: ValueError("Not support browser: " + browser)
-            try: itr = map(int, subprocess.check_output(["pidof", browser]).split())
-            except subprocess.CalledProcessError: itr = []
-            for pid in itr:
-                with open("/proc/" + str(pid) + "/cmdline") as f: cmd_line =  f.read()[:-1]
-                if "--type=renderer" not in cmd_line and "--remote-debugging-port=" in cmd_line:
-                    port = int(re.findall(r"--remote-debugging-port=(\d+)", cmd_line)[0])
-                    if for_port == port: return {port: pid}
-                    result[port] = pid
-        else: raise OSError(f"Platform '{sys.platform}' — not supported")
-        return {} if for_port else result
-
     def __init__(
             self,
             profile_path: str = "testProfile",
             dev_tool_profiles:  bool = False,
             url: Optional[Union[str, bytes]] = None,
             flags:  Optional["FlagBuilder"] = None,
             browser_path: str = "",
```

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/BrowserEx.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/BrowserEx.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/DOMElement.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/DOMElement.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/Data.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/Data.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/Page.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/Page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/BackgroundService.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/BackgroundService.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Browser.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/CSS.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/CSS.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Console.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Console.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DOM.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DOM.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DeviceOrientation.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DeviceOrientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Emulation.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Fetch.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,21 @@
                 params: dict, func: Callable[["FetchType.EventRequestPaused"], Awaitable[None]]) -> None:
             await func(FetchType.EventRequestPaused(**params))
 
         async def on_auth_decorator(
                 params: dict, func: Callable[["FetchType.EventAuthRequired"], Awaitable[None]]) -> None:
             await func(FetchType.EventAuthRequired(**params))
 
-        if on_pause is not None: await self.AddListenerForEvent(FetchEvent.requestPaused, on_pause_decorator, on_pause)
-        if on_auth is not None: await self.AddListenerForEvent(FetchEvent.authRequired, on_auth_decorator, on_auth)
+        if on_pause is not None:
+            await self.AddListenerForEvent(
+                FetchEvent.requestPaused, on_pause_decorator, on_pause)
+
+        if on_auth is not None:
+            await self.AddListenerForEvent(
+                FetchEvent.authRequired, on_auth_decorator, on_auth)
 
         args = {}
         patterns = patterns if patterns is not None else []
         if patterns:
             args.update({"patterns": [p.dict() for p in patterns]})
         if handleAuthRequests: args.update({"handleAuthRequests": handleAuthRequests})
         await self.Call("Fetch.enable", args)
@@ -101,15 +106,15 @@
             responseHeaders: Optional[List[dict]] = None,
             binaryResponseHeaders:  Optional[str] = None,
             body:                   Optional[str] = None,
             responsePhrase:         Optional[str] = None,
             wait_for_response:               bool = False
     ) -> None:
         """
-        Предоставляет ответ на запрос.
+        Предоставляет браузеру ответ на запрос.
         https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-fulfillRequest
         :param requestId:               Идентификатор, полученный клиентом в событии requestPaused.
         :param responseCode:            Код ответа HTTP(например - 200).
         :param responseHeaders:         (optional) Заголовки ответа. Например:
                                             [
                                                 { "name": "User-Agent", "value": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36" },
                                                 { "name": "Content-Type", "value": "application/json; charset=UTF-8" }
@@ -136,14 +141,15 @@
 
     async def ContinueRequest(
         self, requestId: str,
         url:                Optional[str] = None,
         method:             Optional[str] = None,
         postData:           Optional[str] = None,
         headers:     Optional[List[dict]] = None,
+        interceptResponse: Optional[bool] = None,
         wait_for_response:           bool = False
     ) -> None:
         """
         Продолжает запрос, дополнительно изменяя некоторые его параметры.
         https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-continueRequest
         :param requestId:           Идентификатор, полученный клиентом в событии requestPaused.
         :param url:                 (optional) Если установлено, URL-адрес запроса будет изменен так,
@@ -151,22 +157,24 @@
         :param method:              (optional) Переопределяет метод запроса переданным значением.
         :param postData:            (optional) Переопределяет данные запроса переданными.
         :param headers:             (optional) Переопределяет заголовки запроса переданными. . Например:
                                         [
                                             { "name": "User-Agent", "value": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36" },
                                             { "name": "Content-Type", "value": "application/json; charset=UTF-8" }
                                         ]
-        :param wait_for_response:       (optional) Дожидаться ответа?
+        :param interceptResponse:   (optional) Если установлено, переопределяет поведение перехвата ответа для этого запроса.
+        :param wait_for_response:   (optional) Дожидаться ответа?
         :return:
         """
         args = {"requestId": requestId}
         if url is not None: args.update({"url": url})
         if method is not None: args.update({"method": method})
         if postData is not None: args.update({"postData": postData})
         if headers is not None: args.update({"headers": headers})
+        if interceptResponse is not None: args.update({"interceptResponse": interceptResponse})
         await self.Call("Fetch.continueRequest", args, wait_for_response=wait_for_response)
 
     async def ContinueWithAuth(self, requestId: str, authChallengeResponse: list) -> None:
         """
         Продолжает запрос, предоставляющий authChallengeResponse после события authRequired.
         https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-continueWithAuth
         :param requestId:               Идентификатор, полученный клиентом в событии requestPaused.
@@ -266,14 +274,15 @@
                                                         # !     ConnectionClosed, ConnectionReset, ConnectionRefused,
                                                         # !     ConnectionAborted, ConnectionFailed, NameNotResolved,
                                                         # !     InternetDisconnected, AddressUnreachable,
                                                         # !     BlockedByClient, BlockedByResponse
         responseStatusCode: Optional[int] = None
         responseStatusText: Optional[str] = None
         networkId: Optional[str] = None                 # ! id of request
+        redirectedRequestId: Optional[str] = None       # ! id запроса вызвавшего редирект
         _request: NetworkType.Request = field(init=False, repr=False, default=None)
         _responseHeaders: Optional[list["FetchType.HeaderEntry"]] = field(init=False, repr=False, default=None)
 
         @property
         def request(self) -> NetworkType.Request:
             return self._request
```

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Log.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Network.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Overlay.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Page.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Runtime.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/SystemInfo.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Target.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-0.9.5/aio_dt_protocol/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,26 +39,29 @@
 
 class UniqueContextIdNotFound(MyBaseException): pass
 
 class AnotherLocaleOverrideIsAlreadyInEffect(MyBaseException): pass     # ! при установке той же локали
 
 class FontFamiliesCanOnlyBeSetOnce(MyBaseException): pass               # ! при установке тех же шрифтов
 
+class GetRequestBodyBeforeRequestReceived(MyBaseException): pass        # ! получение тела до получения ответа
+
 
 exception_store = {
     "Target crashed": TargetCrashed,
     "Position out of bounds": PositionOutOfBounds,
     "Could not find node with given id": CouldNotFindNodeWithGivenID,
     "Could not compute content quads": CouldNotComputeContentQuads,
     "No dialog is showing": NoDialogIsShowing,
     "No target with given id found": NoTargetWithGivenIdFound,
     "No script with given id": NoScriptWithGivenId,
     "uniqueContextId not found": UniqueContextIdNotFound,
     "Another locale override is already in effect": AnotherLocaleOverrideIsAlreadyInEffect,
-    "Font families can only be set once": FontFamiliesCanOnlyBeSetOnce
+    "Font families can only be set once": FontFamiliesCanOnlyBeSetOnce,
+    "Can only get response body on requests captured after headers received": GetRequestBodyBeforeRequestReceived,
 }
 
 
 def get_cdtp_error(error_text: str) -> Optional[Type[MyBaseException]]:
     for title, ex in exception_store.items():
         if title in error_text:
             return ex
```

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 0.9.4
+Version: 0.9.5
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.4/setup.py` & `aio_dt_protocol-0.9.5/setup.py`

 * *Files identical despite different names*

