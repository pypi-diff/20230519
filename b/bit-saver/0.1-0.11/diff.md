# Comparing `tmp/bit-saver-0.1.tar.gz` & `tmp/bit-saver-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bit-saver-0.1.tar", last modified: Fri May 19 13:41:13 2023, max compression
+gzip compressed data, was "bit-saver-0.11.tar", last modified: Fri May 19 14:23:54 2023, max compression
```

## Comparing `bit-saver-0.1.tar` & `bit-saver-0.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:41:13.813253 bit-saver-0.1/
--rw-rw-rw-   0        0        0     1293 2023-05-19 13:41:13.813253 bit-saver-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-19 13:04:14.000000 bit-saver-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 13:41:13.796249 bit-saver-0.1/bit_saver/
--rw-rw-rw-   0        0        0       59 2023-05-19 13:16:27.000000 bit-saver-0.1/bit_saver/__init__.py
--rw-rw-rw-   0        0        0     2594 2023-05-19 13:11:15.000000 bit-saver-0.1/bit_saver/bit_saver.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:41:13.812252 bit-saver-0.1/bit_saver.egg-info/
--rw-rw-rw-   0        0        0     1293 2023-05-19 13:41:13.000000 bit-saver-0.1/bit_saver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-19 13:41:13.000000 bit-saver-0.1/bit_saver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:41:13.000000 bit-saver-0.1/bit_saver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-19 13:41:13.000000 bit-saver-0.1/bit_saver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 13:41:13.000000 bit-saver-0.1/bit_saver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 13:41:13.814253 bit-saver-0.1/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-05-19 12:49:00.000000 bit-saver-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:23:54.033817 bit-saver-0.11/
+-rw-rw-rw-   0        0        0     1296 2023-05-19 14:23:54.032816 bit-saver-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-19 13:04:14.000000 bit-saver-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 14:23:54.012810 bit-saver-0.11/bit_saver/
+-rw-rw-rw-   0        0        0       59 2023-05-19 13:16:27.000000 bit-saver-0.11/bit_saver/__init__.py
+-rw-rw-rw-   0        0        0     2900 2023-05-19 14:21:33.000000 bit-saver-0.11/bit_saver/bit_saver.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:23:54.031815 bit-saver-0.11/bit_saver.egg-info/
+-rw-rw-rw-   0        0        0     1296 2023-05-19 14:23:53.000000 bit-saver-0.11/bit_saver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-19 14:23:53.000000 bit-saver-0.11/bit_saver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 14:23:53.000000 bit-saver-0.11/bit_saver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 14:23:53.000000 bit-saver-0.11/bit_saver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 14:23:53.000000 bit-saver-0.11/bit_saver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 14:23:54.033817 bit-saver-0.11/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-19 14:23:07.000000 bit-saver-0.11/setup.py
```

### Comparing `bit-saver-0.1/PKG-INFO` & `bit-saver-0.11/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bit-saver
-Version: 0.1
+Version: 0.11
 Summary: A package to save OHLCV data from Upbit exchange to local storage.
 Home-page: https://github.com/choisun0924/bit-saver
 Author: Choi Sun
-Author-email: choisun@hafen.co.kr
+Author-email: choisun@tritech.co.kr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Bit-Saver
```

### Comparing `bit-saver-0.1/README.md` & `bit-saver-0.11/README.md`

 * *Files identical despite different names*

### Comparing `bit-saver-0.1/bit_saver/bit_saver.py` & `bit-saver-0.11/bit_saver/bit_saver.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,41 +31,48 @@
             next_day = initial_start_date + timedelta(days=1)
             df = pyupbit.get_ohlcv(ticker, interval="day", to=next_day)
             if df is None or df.empty:
                 initial_start_date += timedelta(days=1)
             else:
                 return initial_start_date
 
-    def save_ticker_data(self, ticker, start_date):
+    def save_ticker_data(self, ticker, start_date, save_dir):
         """Save OHLCV data for a specific ticker from a specified start date.
 
         Args:
             ticker (str): The ticker symbol to save data.
             start_date (datetime): The start date from which to begin saving data.
+            save_dir (str): The directory in which to save the data.
         """
         dfs = []
         end_date = datetime.now()
         while end_date > start_date:
             df = pyupbit.get_ohlcv(ticker, interval="day", to=end_date)
             if df is None or df.empty:
                 break
             dfs.insert(0, df)
             end_date = df.index[0]
             end_date = datetime.strptime(str(end_date), '%Y-%m-%d %H:%M:%S')
         df = pd.concat(dfs)
         df.drop(columns='value', errors='ignore', inplace=True)
-        df.to_csv(os.path.join(self.save_path, f"{ticker}_ohlcv.csv"))
+        df.to_csv(os.path.join(save_dir, f"{ticker}_ohlcv.csv"))
         print(df)
 
-    def save_all_data(self):
+    def save_all_data(self, save_dir=None):
         """Save OHLCV data for all KRW tickers from Upbit exchange.
+
+        Args:
+            save_dir (str): The directory in which to save the data. If None, use the save_path from the constructor.
         """
+        if save_dir is None:
+            save_dir = self.save_path
+
         tickers = pyupbit.get_tickers(fiat="KRW")
         initial_start_date = datetime(2017, 9, 24, 9, 0, 0)
         for ticker in tickers:
             print('===========================================')
             print(ticker)
             start_date = self.get_start_date(ticker, initial_start_date)
             print(start_date)
             time.sleep(1)
-            self.save_ticker_data(ticker, start_date)
+            self.save_ticker_data(ticker, start_date, save_dir)
             time.sleep(1)
```

### Comparing `bit-saver-0.1/bit_saver.egg-info/PKG-INFO` & `bit-saver-0.11/bit_saver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bit-saver
-Version: 0.1
+Version: 0.11
 Summary: A package to save OHLCV data from Upbit exchange to local storage.
 Home-page: https://github.com/choisun0924/bit-saver
 Author: Choi Sun
-Author-email: choisun@hafen.co.kr
+Author-email: choisun@tritech.co.kr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Bit-Saver
```

### Comparing `bit-saver-0.1/setup.py` & `bit-saver-0.11/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bit-saver",
-    version="0.1",
+    version="0.11",
     description="A package to save OHLCV data from Upbit exchange to local storage.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Choi Sun",
-    author_email="choisun@hafen.co.kr",
+    author_email="choisun@tritech.co.kr",
     url="https://github.com/choisun0924/bit-saver",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
```

