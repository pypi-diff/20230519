# Comparing `tmp/autil-0.2.2.tar.gz` & `tmp/autil-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autil-0.2.2.tar", last modified: Mon Aug  1 16:48:17 2022, max compression
+gzip compressed data, was "autil-0.2.3.tar", last modified: Fri May 19 17:33:58 2023, max compression
```

## Comparing `autil-0.2.2.tar` & `autil-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      510 2022-04-25 12:36:00.308470 autil-0.2.2/autil/__init__.py
--rw-r--r--   0        0        0     1055 2022-04-25 12:23:28.875685 autil-0.2.2/autil/alt_plot.py
--rwxr-xr-x   0        0        0      937 2020-10-09 14:28:44.901723 autil-0.2.2/autil/country2continent.py
--rw-r--r--   0        0        0      452 2021-11-30 08:10:07.103352 autil-0.2.2/autil/io.py
--rw-r--r--   0        0        0     1124 2020-12-09 14:28:02.713989 autil-0.2.2/autil/io_download.py
--rw-r--r--   0        0        0      437 2022-07-07 18:34:54.917037 autil-0.2.2/autil/io_parquet.py
--rw-r--r--   0        0        0      336 2021-06-28 21:09:47.281261 autil-0.2.2/autil/ipy_addpath.py
--rwxr-xr-x   0        0        0     3798 2021-09-15 11:20:18.932676 autil-0.2.2/autil/ipy_displays.py
--rw-r--r--   0        0        0     1588 2020-11-28 09:51:40.919240 autil-0.2.2/autil/ipy_print.py
--rw-r--r--   0        0        0     1398 2022-01-21 13:51:44.810518 autil-0.2.2/autil/lm_lighten.py
--rw-r--r--   0        0        0     1925 2022-04-25 12:27:21.786888 autil-0.2.2/autil/mpl_plot.py
--rw-r--r--   0        0        0     6277 2022-07-03 21:43:07.837620 autil-0.2.2/autil/mpl_set.py
--rwxr-xr-x   0        0        0      971 2022-04-25 12:19:09.214814 autil-0.2.2/autil/owari.py
--rwxr-xr-x   0        0        0      393 2020-10-09 14:28:56.506532 autil-0.2.2/autil/pd_clean.py
--rw-r--r--   0        0        0      362 2022-04-25 12:05:21.123984 autil-0.2.2/autil/pd_perform.py
--rw-r--r--   0        0        0      988 2022-04-25 12:05:26.060654 autil-0.2.2/autil/pd_table.py
--rw-r--r--   0        0        0      203 2021-10-06 16:58:32.312882 autil-0.2.2/autil/print.py
--rw-r--r--   0        0        0     3372 2022-08-01 16:03:49.044363 autil-0.2.2/autil/scrape.py
--rw-r--r--   0        0        0     4742 2022-08-01 16:42:26.170655 autil-0.2.2/autil/scrape_proxy.py
--rw-r--r--   0        0        0     1102 2022-04-25 12:30:51.577437 autil-0.2.2/autil/sendmail.py
--rw-r--r--   0        0        0     4527 2022-04-25 12:10:11.910350 autil-0.2.2/autil/sk_metrics.py
--rw-r--r--   0        0        0     1791 2021-08-19 08:33:57.016179 autil-0.2.2/autil/sqlite.py
--rw-r--r--   0        0        0     3391 2019-11-17 12:31:48.420195 autil-0.2.2/autil/stat_summary.py
--rw-r--r--   0        0        0     2828 2022-04-21 08:31:41.024812 autil-0.2.2/autil/tex_table.py
--rw-r--r--   0        0        0      659 2022-04-25 12:31:44.528913 autil-0.2.2/autil/tr.py
--rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 autil-0.2.2/autil/z2h.py
--rw-r--r--   0        0        0      745 2022-08-01 16:46:45.412514 autil-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1132 2022-08-01 16:48:17.225470 autil-0.2.2/setup.py
--rw-r--r--   0        0        0     1098 2022-08-01 16:48:17.225736 autil-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      510 2022-04-25 12:36:00.308470 autil-0.2.3/autil/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-19 17:17:27.828887 autil-0.2.3/autil/alt_plot.py
+-rwxr-xr-x   0        0        0      937 2020-10-09 14:28:44.901723 autil-0.2.3/autil/country2continent.py
+-rw-r--r--   0        0        0      782 2023-05-19 17:02:24.835613 autil-0.2.3/autil/io.py
+-rw-r--r--   0        0        0     1124 2020-12-09 14:28:02.713989 autil-0.2.3/autil/io_download.py
+-rw-r--r--   0        0        0      437 2022-07-07 18:34:54.917037 autil-0.2.3/autil/io_parquet.py
+-rw-r--r--   0        0        0      336 2021-06-28 21:09:47.281261 autil-0.2.3/autil/ipy_addpath.py
+-rwxr-xr-x   0        0        0     3798 2021-09-15 11:20:18.932676 autil-0.2.3/autil/ipy_displays.py
+-rw-r--r--   0        0        0     1588 2020-11-28 09:51:40.919240 autil-0.2.3/autil/ipy_print.py
+-rw-r--r--   0        0        0     1398 2022-01-21 13:51:44.810518 autil-0.2.3/autil/lm_lighten.py
+-rw-r--r--   0        0        0     2164 2023-03-27 06:11:48.922951 autil-0.2.3/autil/mpl_plot.py
+-rw-r--r--   0        0        0     6277 2022-07-03 21:43:07.837620 autil-0.2.3/autil/mpl_set.py
+-rwxr-xr-x   0        0        0      971 2022-04-25 12:19:09.214814 autil-0.2.3/autil/owari.py
+-rwxr-xr-x   0        0        0      393 2020-10-09 14:28:56.506532 autil-0.2.3/autil/pd_clean.py
+-rw-r--r--   0        0        0      448 2022-12-12 06:25:01.443831 autil-0.2.3/autil/pd_perform.py
+-rw-r--r--   0        0        0      988 2022-04-25 12:05:26.060654 autil-0.2.3/autil/pd_table.py
+-rw-r--r--   0        0        0      203 2021-10-06 16:58:32.312882 autil-0.2.3/autil/print.py
+-rw-r--r--   0        0        0     3372 2022-08-01 16:03:49.044363 autil-0.2.3/autil/scrape.py
+-rw-r--r--   0        0        0     5194 2022-08-06 18:39:17.423544 autil-0.2.3/autil/scrape_proxy.py
+-rw-r--r--   0        0        0     1102 2022-04-25 12:30:51.577437 autil-0.2.3/autil/sendmail.py
+-rw-r--r--   0        0        0     4527 2022-04-25 12:10:11.910350 autil-0.2.3/autil/sk_metrics.py
+-rw-r--r--   0        0        0     1791 2021-08-19 08:33:57.016179 autil-0.2.3/autil/sqlite.py
+-rw-r--r--   0        0        0     3391 2019-11-17 12:31:48.420195 autil-0.2.3/autil/stat_summary.py
+-rw-r--r--   0        0        0     3118 2022-12-09 08:05:51.189792 autil-0.2.3/autil/tex_table.py
+-rw-r--r--   0        0        0      659 2022-04-25 12:31:44.528913 autil-0.2.3/autil/tr.py
+-rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 autil-0.2.3/autil/z2h.py
+-rw-r--r--   0        0        0      745 2023-05-19 17:18:45.482262 autil-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1132 2023-05-19 17:33:58.695172 autil-0.2.3/setup.py
+-rw-r--r--   0        0        0     1098 2023-05-19 17:33:58.695445 autil-0.2.3/PKG-INFO
```

### Comparing `autil-0.2.2/autil/country2continent.py` & `autil-0.2.3/autil/country2continent.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/io_download.py` & `autil-0.2.3/autil/io_download.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/ipy_displays.py` & `autil-0.2.3/autil/ipy_displays.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/ipy_print.py` & `autil-0.2.3/autil/ipy_print.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/lm_lighten.py` & `autil-0.2.3/autil/lm_lighten.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/mpl_plot.py` & `autil-0.2.3/autil/mpl_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """
 Useful plots in data anlysis
 """
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
+from labellines import labelLine, labelLines
 
 if __name__ != "__main__":
     __version__ = 0.1
 
 
+def add_label_for_lines(ax, lw=3, zorder=2.5):
+    """
+    Add line labels for a line plot
+    """
+    ax.get_lines()[-1].set(lw=lw)
+    labelLines(ax.get_lines(), zorder=zorder)
+    return ax
+
 def plot_scatter_with_text(
         data, x, y, z, hue=None, style=None,
         text_condition=None, text_adjust=False, adjust_precision=0.1):
     """
     Use seaborn, matplotlib and adjustText to plot scatter with text
     """
     data = data.copy().reset_index(drop=True)
```

### Comparing `autil-0.2.2/autil/mpl_set.py` & `autil-0.2.3/autil/mpl_set.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/owari.py` & `autil-0.2.3/autil/owari.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/pd_table.py` & `autil-0.2.3/autil/pd_table.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/scrape.py` & `autil-0.2.3/autil/scrape.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/scrape_proxy.py` & `autil-0.2.3/autil/scrape_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,17 +59,19 @@
         if abs(day_now - self.last_proxy_refresh_day) >= self.day_for_refresh:
             self.proxies = self.get_proxies()
             self.last_proxy_refresh_day = day_now
         print("Refresh proxies")
 
 
 class ProxyBrowser(ProxySession):
-    def __init__(self,):
+    def __init__(self, headless=False):
         super().__init__()
 
+        self.headless = headless
+
         self.proxy_options = None
         self.chrome_options = None
         self.browser = None
 
         self.set_option_proxy()
         self.set_option_chrome()
         self.set_browser()
@@ -78,24 +80,31 @@
         proxies = self.session.proxies
         proxies["no_proxy"] = 'localhost,127.0.0.1'
         proxy_options = {'proxy': proxies}
         self.proxy_options = proxy_options
 
     def set_option_chrome(self,):
         chrome_options = webdriver.ChromeOptions()
+        chrome_options.add_argument('--no-sandbox')
+        # chrome_options.add_argument('--start-maximized')
+        # chrome_options.add_argument('--start-fullscreen')
+        chrome_options.add_argument('--single-process')
+        chrome_options.add_argument('--disable-dev-shm-usage')
+        chrome_options.add_argument("--incognito")
+        chrome_options.add_argument('--disable-blink-features=AutomationControlled')
+        chrome_options.add_argument("disable-infobars")
         chrome_options.add_experimental_option(
             "excludeSwitches", ["enable-automation"])
         chrome_options.add_experimental_option('useAutomationExtension', False)
         preferences = {
             "webrtc.ip_handling_policy": "disable_non_proxied_udp",
             "webrtc.multiple_routes_enabled": False,
             "webrtc.nonproxied_udp_enabled": False
         }
         chrome_options.add_experimental_option("prefs", preferences)
-        chrome_options.add_argument("disable-blink-features=AutomationControlled")
         self.chrome_options = chrome_options
 
     def get_timezone_geolocation(self):
         url = "http://ip-api.com/json/"
         response = self.session.get(url)
         return response.json()
 
@@ -108,21 +117,21 @@
         }
         tz = {
             "timezoneId": res_json["timezone"]
         }
         self.browser.execute_cdp_cmd("Emulation.setGeolocationOverride", geo)
         self.browser.execute_cdp_cmd("Emulation.setTimezoneOverride", tz)
 
-    def set_browser(self, headless=True, wait=14):
+    def set_browser(self, wait=14):
         # not sure seleniumwire allow for load model thus remove the load module
         chrome_options = self.chrome_options
-        chrome_options.headless = headless
+        chrome_options.headless = self.headless
         chrome_options.add_argument("window-size=1920,1080")
 
         browser = webdriver.Chrome(chrome_options=chrome_options, seleniumwire_options=self.proxy_options)
         browser.implicitly_wait(wait)
         self.browser = browser
 
-    def reset_browser(self,):
+    def reset_browser(self, headless=True):
         """After using `update_proxy` or `replace_proxy`, use this function to reset browser"""
         self.set_option_proxy()
         self.set_browser()
```

### Comparing `autil-0.2.2/autil/sendmail.py` & `autil-0.2.3/autil/sendmail.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/sk_metrics.py` & `autil-0.2.3/autil/sk_metrics.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/sqlite.py` & `autil-0.2.3/autil/sqlite.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/stat_summary.py` & `autil-0.2.3/autil/stat_summary.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/tex_table.py` & `autil-0.2.3/autil/tex_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,7 +89,18 @@
     with open(file_path, 'r', encoding='utf8') as f:
         lines = f.readlines()
 
     lines.insert(line_idx, " " + new_line + linebreak)
 
     with open(file_path, 'w', encoding='utf8') as f:
         f.writelines(lines)
+
+
+def drop_line(file_path: str, lines_idx: list):
+
+    with open(file_path, 'r', encoding='utf8') as f:
+        lines = f.readlines()
+
+    lines = [li for idx, li in enumerate(lines) if idx not in lines_idx]
+
+    with open(file_path, 'w', encoding='utf8') as f:
+        f.writelines(lines)
```

### Comparing `autil-0.2.2/autil/tr.py` & `autil-0.2.3/autil/tr.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/autil/z2h.py` & `autil-0.2.3/autil/z2h.py`

 * *Files identical despite different names*

### Comparing `autil-0.2.2/pyproject.toml` & `autil-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 authors = ["alalalalaki <harlan.zhu@gmail.com>"]
 description = "Some Python snippets for a researcher's daily use"
 name = "autil"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.dependencies]
 adjustText = "^0.7.3"
 altair = "^4.1"
 country_converter = "^0.7.3"
 cycler = "^0.10"
 deepl = "^1.6.0"
```

### Comparing `autil-0.2.2/setup.py` & `autil-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'selenium>=3.141.0,<4.0.0',
  'tenacity>=8.0.1,<9.0.0',
  'tqdm>=4.62,<5.0',
  'translators>=4.9.5,<5.0.0']
 
 setup_kwargs = {
     'name': 'autil',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': "Some Python snippets for a researcher's daily use",
     'long_description': None,
     'author': 'alalalalaki',
     'author_email': 'harlan.zhu@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `autil-0.2.2/PKG-INFO` & `autil-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autil
-Version: 0.2.2
+Version: 0.2.3
 Summary: Some Python snippets for a researcher's daily use
 Author: alalalalaki
 Author-email: harlan.zhu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: adjustText (>=0.7.3,<0.8.0)
```

