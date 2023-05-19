# Comparing `tmp/codal_tsetmc-1.3.0.tar.gz` & `tmp/codal_tsetmc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codal_tsetmc-1.3.0.tar", max compression
+gzip compressed data, was "codal_tsetmc-1.3.1.tar", max compression
```

## Comparing `codal_tsetmc-1.3.0.tar` & `codal_tsetmc-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-1.3.0/LICENSE
--rwxr-xr-x   0        0        0     1200 2023-05-19 10:06:29.055913 codal_tsetmc-1.3.0/README.md
--rwxr-xr-x   0        0        0      872 2023-05-19 10:06:47.285281 codal_tsetmc-1.3.0/pyproject.toml
--rwxr-xr-x   0        0        0      403 2023-05-04 20:58:19.507320 codal_tsetmc-1.3.0/src/codal_tsetmc/__init__.py
--rwxr-xr-x   0        0        0       22 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.0/src/codal_tsetmc/config/__init__.py
--rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.0/src/codal_tsetmc/config/config.default.yml
--rwxr-xr-x   0        0        0     2326 2022-08-31 10:11:07.442885 codal_tsetmc-1.3.0/src/codal_tsetmc/config/engine.py
--rwxr-xr-x   0        0        0       63 2023-05-09 11:02:46.190475 codal_tsetmc-1.3.0/src/codal_tsetmc/download/__init__.py
--rwxr-xr-x   0        0        0       89 2023-05-09 11:26:45.292434 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/__init__.py
--rw-r--r--   0        0        0     3726 2023-05-09 11:25:04.912760 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/category.py
--rwxr-xr-x   0        0        0      436 2023-05-09 12:24:55.307909 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/company.py
--rw-r--r--   0        0        0     4422 2023-05-10 15:50:00.836027 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/letters.py
--rwxr-xr-x   0        0        0     9914 2023-05-11 08:58:24.216036 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/query.py
--rw-r--r--   0        0        0     6387 2023-05-09 11:19:42.789846 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/report.py
--rwxr-xr-x   0        0        0       24 2023-05-09 11:03:06.526343 codal_tsetmc-1.3.0/src/codal_tsetmc/download/other/__init__.py
--rwxr-xr-x   0        0        0     4776 2023-05-12 09:02:29.559760 codal_tsetmc-1.3.0/src/codal_tsetmc/download/other/commodity.py
--rwxr-xr-x   0        0        0       64 2023-05-09 11:04:22.117876 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/__init__.py
--rw-r--r--   0        0        0     4409 2023-05-12 09:39:45.987692 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/capital.py
--rwxr-xr-x   0        0        0     6105 2023-05-12 08:50:46.339974 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/price.py
--rwxr-xr-x   0        0        0     3965 2023-05-05 19:11:47.649936 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/stock.py
--rwxr-xr-x   0        0        0      974 2023-05-09 11:26:24.284501 codal_tsetmc-1.3.0/src/codal_tsetmc/initializer.py
--rwxr-xr-x   0        0        0       74 2023-05-04 23:26:55.093507 codal_tsetmc-1.3.0/src/codal_tsetmc/models/__init__.py
--rwxr-xr-x   0        0        0     3404 2023-05-10 15:14:27.583197 codal_tsetmc-1.3.0/src/codal_tsetmc/models/companies.py
--rwxr-xr-x   0        0        0      631 2023-05-04 23:19:18.522855 codal_tsetmc-1.3.0/src/codal_tsetmc/models/create.py
--rwxr-xr-x   0        0        0     5668 2023-05-17 04:41:12.722129 codal_tsetmc-1.3.0/src/codal_tsetmc/models/stocks.py
--rwxr-xr-x   0        0        0      110 2023-05-09 11:19:42.789846 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/__init__.py
--rwxr-xr-x   0        0        0     1181 2023-05-12 09:31:02.527274 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/api.py
--rwxr-xr-x   0        0        0      483 2023-05-05 00:04:47.292213 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/database.py
--rwxr-xr-x   0        0        0      891 2022-07-11 11:37:09.587064 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/exception.py
--rwxr-xr-x   0        0        0     9238 2023-05-09 11:19:07.641970 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/string.py
--rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 codal_tsetmc-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-1.3.1/LICENSE
+-rwxr-xr-x   0        0        0     1193 2023-05-19 10:09:12.331470 codal_tsetmc-1.3.1/README.md
+-rwxr-xr-x   0        0        0      872 2023-05-19 10:19:02.772789 codal_tsetmc-1.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0      403 2023-05-04 20:58:19.507320 codal_tsetmc-1.3.1/src/codal_tsetmc/__init__.py
+-rwxr-xr-x   0        0        0       22 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.1/src/codal_tsetmc/config/__init__.py
+-rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.1/src/codal_tsetmc/config/config.default.yml
+-rwxr-xr-x   0        0        0     2326 2022-08-31 10:11:07.442885 codal_tsetmc-1.3.1/src/codal_tsetmc/config/engine.py
+-rwxr-xr-x   0        0        0       63 2023-05-09 11:02:46.190475 codal_tsetmc-1.3.1/src/codal_tsetmc/download/__init__.py
+-rwxr-xr-x   0        0        0       89 2023-05-09 11:26:45.292434 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/__init__.py
+-rw-r--r--   0        0        0     3726 2023-05-09 11:25:04.912760 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/category.py
+-rwxr-xr-x   0        0        0      436 2023-05-09 12:24:55.307909 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/company.py
+-rw-r--r--   0        0        0     4422 2023-05-10 15:50:00.836027 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/letters.py
+-rwxr-xr-x   0        0        0     9914 2023-05-11 08:58:24.216036 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/query.py
+-rw-r--r--   0        0        0     6387 2023-05-09 11:19:42.789846 codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/report.py
+-rwxr-xr-x   0        0        0       24 2023-05-09 11:03:06.526343 codal_tsetmc-1.3.1/src/codal_tsetmc/download/other/__init__.py
+-rwxr-xr-x   0        0        0     4776 2023-05-12 09:02:29.559760 codal_tsetmc-1.3.1/src/codal_tsetmc/download/other/commodity.py
+-rwxr-xr-x   0        0        0       64 2023-05-09 11:04:22.117876 codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/__init__.py
+-rw-r--r--   0        0        0     4409 2023-05-12 09:39:45.987692 codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/capital.py
+-rwxr-xr-x   0        0        0     6105 2023-05-12 08:50:46.339974 codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/price.py
+-rwxr-xr-x   0        0        0     3965 2023-05-05 19:11:47.649936 codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/stock.py
+-rwxr-xr-x   0        0        0      974 2023-05-09 11:26:24.284501 codal_tsetmc-1.3.1/src/codal_tsetmc/initializer.py
+-rwxr-xr-x   0        0        0       74 2023-05-04 23:26:55.093507 codal_tsetmc-1.3.1/src/codal_tsetmc/models/__init__.py
+-rwxr-xr-x   0        0        0     3404 2023-05-10 15:14:27.583197 codal_tsetmc-1.3.1/src/codal_tsetmc/models/companies.py
+-rwxr-xr-x   0        0        0      631 2023-05-04 23:19:18.522855 codal_tsetmc-1.3.1/src/codal_tsetmc/models/create.py
+-rwxr-xr-x   0        0        0     5668 2023-05-17 04:41:12.722129 codal_tsetmc-1.3.1/src/codal_tsetmc/models/stocks.py
+-rwxr-xr-x   0        0        0       90 2023-05-19 10:12:05.106303 codal_tsetmc-1.3.1/src/codal_tsetmc/tools/__init__.py
+-rwxr-xr-x   0        0        0     1181 2023-05-12 09:31:02.527274 codal_tsetmc-1.3.1/src/codal_tsetmc/tools/api.py
+-rwxr-xr-x   0        0        0      483 2023-05-05 00:04:47.292213 codal_tsetmc-1.3.1/src/codal_tsetmc/tools/database.py
+-rwxr-xr-x   0        0        0      891 2022-07-11 11:37:09.587064 codal_tsetmc-1.3.1/src/codal_tsetmc/tools/exception.py
+-rwxr-xr-x   0        0        0     9238 2023-05-09 11:19:07.641970 codal_tsetmc-1.3.1/src/codal_tsetmc/tools/string.py
+-rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 codal_tsetmc-1.3.1/PKG-INFO
```

### Comparing `codal_tsetmc-1.3.0/LICENSE` & `codal_tsetmc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/README.md` & `codal_tsetmc-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 این پکیچ برای ذخیره داده‌های سایت کدال و بازار سرمایه برای اهداف تحلیل بنیادی تهیه شده است.
 
 ## پایگاه داده
 
 ### TSETMC
 
 - [X] `tehran_stocks`: ویرایش بعضی از کدهای بسته
-    - 
 
 - [X] `stock_capital`: پایگاه داده افزایش سرمایه
 
 ### CODAL
 
 - [X] `companies`: لیست تمام شرکت‌ها
 - [X] `company_statuses`: وضعیت شرکت‌ها
```

### Comparing `codal_tsetmc-1.3.0/pyproject.toml` & `codal_tsetmc-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codal-tsetmc"
-version = "1.3.0"
+version = "1.3.1"
 description = "Data Downloader for Codal and Tehran stock market"
 authors = ["Mohsen Ebrahimi <mohsenebrahimy.ir@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mohsenebrahimyir.github.io/codal-tsetmc/"
 repository = "https://github.com/mohsenebrahimyir/codal-tsetmc.git"
 packages = [
```

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/config/engine.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/config/engine.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/category.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/category.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/letters.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/letters.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/query.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/query.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/report.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/codal/report.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/other/commodity.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/other/commodity.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/capital.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/capital.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/price.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/price.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/stock.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/download/tsetmc/stock.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/initializer.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/initializer.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/models/companies.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/models/companies.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/models/create.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/models/create.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/models/stocks.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/models/stocks.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/tools/api.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/tools/api.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/tools/exception.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/tools/exception.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/src/codal_tsetmc/tools/string.py` & `codal_tsetmc-1.3.1/src/codal_tsetmc/tools/string.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.3.0/PKG-INFO` & `codal_tsetmc-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codal-tsetmc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Data Downloader for Codal and Tehran stock market
 Home-page: https://mohsenebrahimyir.github.io/codal-tsetmc/
 License: MIT
 Author: Mohsen Ebrahimi
 Author-email: mohsenebrahimy.ir@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,14 @@
 این پکیچ برای ذخیره داده‌های سایت کدال و بازار سرمایه برای اهداف تحلیل بنیادی تهیه شده است.
 
 ## پایگاه داده
 
 ### TSETMC
 
 - [X] `tehran_stocks`: ویرایش بعضی از کدهای بسته
-    - 
 
 - [X] `stock_capital`: پایگاه داده افزایش سرمایه
 
 ### CODAL
 
 - [X] `companies`: لیست تمام شرکت‌ها
 - [X] `company_statuses`: وضعیت شرکت‌ها
```

