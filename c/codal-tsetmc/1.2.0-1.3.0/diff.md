# Comparing `tmp/codal_tsetmc-1.2.0.tar.gz` & `tmp/codal_tsetmc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codal_tsetmc-1.2.0.tar", max compression
+gzip compressed data, was "codal_tsetmc-1.3.0.tar", max compression
```

## Comparing `codal_tsetmc-1.2.0.tar` & `codal_tsetmc-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-1.2.0/LICENSE
--rwxr-xr-x   0        0        0      724 2022-09-02 21:25:33.047939 codal_tsetmc-1.2.0/README.md
--rwxr-xr-x   0        0        0      897 2023-04-05 22:50:30.124603 codal_tsetmc-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1144 2023-02-01 22:48:46.892019 codal_tsetmc-1.2.0/src/codal_tsetmc/__init__.py
--rwxr-xr-x   0        0        0       22 2022-07-29 09:25:17.071258 codal_tsetmc-1.2.0/src/codal_tsetmc/config/__init__.py
--rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-1.2.0/src/codal_tsetmc/config/config.default.yml
--rwxr-xr-x   0        0        0     2326 2022-08-31 10:11:07.442885 codal_tsetmc-1.2.0/src/codal_tsetmc/config/engine.py
--rwxr-xr-x   0        0        0      820 2023-02-01 22:49:09.128097 codal_tsetmc-1.2.0/src/codal_tsetmc/download/__init__.py
--rwxr-xr-x   0        0        0     4436 2023-02-01 23:20:29.103539 codal_tsetmc-1.2.0/src/codal_tsetmc/download/adjusted.py
--rwxr-xr-x   0        0        0     5125 2023-02-01 23:20:02.589779 codal_tsetmc-1.2.0/src/codal_tsetmc/download/capital.py
--rwxr-xr-x   0        0        0     5183 2023-02-01 23:19:50.108923 codal_tsetmc-1.2.0/src/codal_tsetmc/download/client.py
--rwxr-xr-x   0        0        0     1412 2023-02-01 23:16:43.433283 codal_tsetmc-1.2.0/src/codal_tsetmc/download/commodity.py
--rwxr-xr-x   0        0        0      674 2023-02-01 22:51:17.312521 codal_tsetmc-1.2.0/src/codal_tsetmc/download/company.py
--rwxr-xr-x   0        0        0     5139 2023-02-01 23:19:32.967717 codal_tsetmc-1.2.0/src/codal_tsetmc/download/dividend.py
--rwxr-xr-x   0        0        0     5853 2023-04-05 22:12:53.893891 codal_tsetmc-1.2.0/src/codal_tsetmc/download/price.py
--rwxr-xr-x   0        0        0    12795 2023-02-01 22:55:08.341197 codal_tsetmc-1.2.0/src/codal_tsetmc/download/query.py
--rwxr-xr-x   0        0        0     4269 2023-02-01 22:52:35.192760 codal_tsetmc-1.2.0/src/codal_tsetmc/download/stock.py
--rwxr-xr-x   0        0        0      927 2022-09-01 23:10:17.302106 codal_tsetmc-1.2.0/src/codal_tsetmc/initializer.py
--rwxr-xr-x   0        0        0      345 2023-02-01 22:24:29.724260 codal_tsetmc-1.2.0/src/codal_tsetmc/models/__init__.py
--rwxr-xr-x   0        0        0      491 2023-02-01 22:21:19.189725 codal_tsetmc-1.2.0/src/codal_tsetmc/models/commodities.py
--rwxr-xr-x   0        0        0     1975 2023-02-01 20:52:06.515938 codal_tsetmc-1.2.0/src/codal_tsetmc/models/companies.py
--rwxr-xr-x   0        0        0      656 2022-09-02 22:17:37.592486 codal_tsetmc-1.2.0/src/codal_tsetmc/models/create.py
--rwxr-xr-x   0        0        0    15833 2023-02-02 09:53:33.426918 codal_tsetmc-1.2.0/src/codal_tsetmc/models/stocks.py
--rwxr-xr-x   0        0        0      205 2023-02-01 22:54:07.905029 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/__init__.py
--rwxr-xr-x   0        0        0      400 2023-02-01 22:14:20.353610 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/api.py
--rwxr-xr-x   0        0        0      504 2023-02-01 23:15:18.079542 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/database.py
--rwxr-xr-x   0        0        0      891 2022-07-11 11:37:09.587064 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/exception.py
--rwxr-xr-x   0        0        0      548 2023-02-02 08:54:40.600928 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/plot.py
--rwxr-xr-x   0        0        0      849 2023-02-01 22:53:49.836978 codal_tsetmc-1.2.0/src/codal_tsetmc/tools/string_edit.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 codal_tsetmc-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2022-08-31 09:49:59.670121 codal_tsetmc-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0     1200 2023-05-19 10:06:29.055913 codal_tsetmc-1.3.0/README.md
+-rwxr-xr-x   0        0        0      872 2023-05-19 10:06:47.285281 codal_tsetmc-1.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0      403 2023-05-04 20:58:19.507320 codal_tsetmc-1.3.0/src/codal_tsetmc/__init__.py
+-rwxr-xr-x   0        0        0       22 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.0/src/codal_tsetmc/config/__init__.py
+-rwxr-xr-x   0        0        0      100 2022-07-29 09:25:17.071258 codal_tsetmc-1.3.0/src/codal_tsetmc/config/config.default.yml
+-rwxr-xr-x   0        0        0     2326 2022-08-31 10:11:07.442885 codal_tsetmc-1.3.0/src/codal_tsetmc/config/engine.py
+-rwxr-xr-x   0        0        0       63 2023-05-09 11:02:46.190475 codal_tsetmc-1.3.0/src/codal_tsetmc/download/__init__.py
+-rwxr-xr-x   0        0        0       89 2023-05-09 11:26:45.292434 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/__init__.py
+-rw-r--r--   0        0        0     3726 2023-05-09 11:25:04.912760 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/category.py
+-rwxr-xr-x   0        0        0      436 2023-05-09 12:24:55.307909 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/company.py
+-rw-r--r--   0        0        0     4422 2023-05-10 15:50:00.836027 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/letters.py
+-rwxr-xr-x   0        0        0     9914 2023-05-11 08:58:24.216036 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/query.py
+-rw-r--r--   0        0        0     6387 2023-05-09 11:19:42.789846 codal_tsetmc-1.3.0/src/codal_tsetmc/download/codal/report.py
+-rwxr-xr-x   0        0        0       24 2023-05-09 11:03:06.526343 codal_tsetmc-1.3.0/src/codal_tsetmc/download/other/__init__.py
+-rwxr-xr-x   0        0        0     4776 2023-05-12 09:02:29.559760 codal_tsetmc-1.3.0/src/codal_tsetmc/download/other/commodity.py
+-rwxr-xr-x   0        0        0       64 2023-05-09 11:04:22.117876 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/__init__.py
+-rw-r--r--   0        0        0     4409 2023-05-12 09:39:45.987692 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/capital.py
+-rwxr-xr-x   0        0        0     6105 2023-05-12 08:50:46.339974 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/price.py
+-rwxr-xr-x   0        0        0     3965 2023-05-05 19:11:47.649936 codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/stock.py
+-rwxr-xr-x   0        0        0      974 2023-05-09 11:26:24.284501 codal_tsetmc-1.3.0/src/codal_tsetmc/initializer.py
+-rwxr-xr-x   0        0        0       74 2023-05-04 23:26:55.093507 codal_tsetmc-1.3.0/src/codal_tsetmc/models/__init__.py
+-rwxr-xr-x   0        0        0     3404 2023-05-10 15:14:27.583197 codal_tsetmc-1.3.0/src/codal_tsetmc/models/companies.py
+-rwxr-xr-x   0        0        0      631 2023-05-04 23:19:18.522855 codal_tsetmc-1.3.0/src/codal_tsetmc/models/create.py
+-rwxr-xr-x   0        0        0     5668 2023-05-17 04:41:12.722129 codal_tsetmc-1.3.0/src/codal_tsetmc/models/stocks.py
+-rwxr-xr-x   0        0        0      110 2023-05-09 11:19:42.789846 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/__init__.py
+-rwxr-xr-x   0        0        0     1181 2023-05-12 09:31:02.527274 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/api.py
+-rwxr-xr-x   0        0        0      483 2023-05-05 00:04:47.292213 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/database.py
+-rwxr-xr-x   0        0        0      891 2022-07-11 11:37:09.587064 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/exception.py
+-rwxr-xr-x   0        0        0     9238 2023-05-09 11:19:07.641970 codal_tsetmc-1.3.0/src/codal_tsetmc/tools/string.py
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 codal_tsetmc-1.3.0/PKG-INFO
```

### Comparing `codal_tsetmc-1.2.0/LICENSE` & `codal_tsetmc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.2.0/pyproject.toml` & `codal_tsetmc-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codal-tsetmc"
-version = "1.2.0"
+version = "1.3.0"
 description = "Data Downloader for Codal and Tehran stock market"
 authors = ["Mohsen Ebrahimi <mohsenebrahimy.ir@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mohsenebrahimyir.github.io/codal-tsetmc/"
 repository = "https://github.com/mohsenebrahimyir/codal-tsetmc.git"
 packages = [
@@ -19,15 +19,14 @@
 jalali-pandas = "^0.2.0"
 pandas = "^1.3.5"
 lxml = "^4.8.0"
 aiohttp = "^3.8.1"
 cchardet = "^2.1.7"
 aiodns = "^3.0.0"
 PyYAML = "^6.0"
-tehran_stocks = "^1.0.9"
 finplot = "^1.9.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.16.0"
 pylint = "^2.12.2"
 pytest = "^6.2.5"
 ipython = "^7.31.0"
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/config/engine.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/config/engine.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/download/capital.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/capital.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,140 @@
+from jdatetime import datetime as jdt
 from datetime import datetime
 import asyncio
 import aiohttp
 import pandas as pd
 import requests
 import io
 
 import codal_tsetmc.config as db
 from codal_tsetmc.models import Stocks
+from codal_tsetmc.tools import *
+from codal_tsetmc.download.tsetmc.stock import is_stock_in_bourse_or_fara_or_paye
 
 
-def value_to_float(x):
-    x = x.replace(",", "")
-    if type(x) == float or type(x) == int:
-        return x
-    if 'K' in x:
-        if len(x) > 1:
-            return float(x.replace(' K', '')) * 1000
-        return 1000.0
-    if 'M' in x:
-        if len(x) > 1:
-            return float(x.replace(' M', '')) * 1000000
-        return 1000000.0
-    if 'B' in x:
-        return float(x.replace(' B', '')) * 1000000000
-    return 0.0
-
-
-def get_stock_capital_history(stock_id: str) -> pd.DataFrame:
-    """Get stock capital from the web.
-
-    params:
-    ----------------
-    code: int
-        http://tsetmc.com/Loader.aspx?ParTree=15131H&i=46348559193224090#
-        interger after i=
-
-    return:
-    ----------------
-    pd.DataFrame
-        dtyyyymmdd: str
-        old_capital = int
-        new_capital = int
-
-    example
-    ----------------
-    df = get_stock_capital_history("46348559193224090")
-    """
-    url = f"http://tsetmc.com/Loader.aspx?ParTree=15131H&i={stock_id}"
-    r = requests.get(url)
-    df = pd.read_html(r.text)[0]
-    df.columns = ["date", "new_capital", "old_capital"]
-    df["new_capital"] = df["new_capital"].apply(value_to_float)
-    df["old_capital"] = df["old_capital"].apply(value_to_float)
-    df["date"] = df.date.jalali.parse_jalali("%Y/%m/%d")
-    df["dtyyyymmdd"] = (
-        df.date.jalali
-        .to_gregorian()
-        .apply(lambda x: x.strftime("%Y%m%d"))
-        .astype(int)
-    )
+def get_stock_capital_daily(code: str, date = None):
+    if date is None:
+        date = datetime.now().strftime("%Y%m%d")
+    
+    data = "Instrument/GetInstrumentHistory"
+    dict_data = get_data_from_cdn_tsetmec_api(data, code, date)
+    return dict_data["instrumentHistory"]["zTitad"]
+
+
+def cleanup_stock_capitals_records(response):
+    df = pd.read_html(io.StringIO(response))[0]
+    df.columns = ["date", "new", "old"]
+    df["date"] = df["date"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
+    df = df.sort_index(ascending=False)
+    df["old"] = df["old"].apply(value_to_float)
+    df["new"] = df["new"].apply(value_to_float)
+    df = df[
+        (df.new > df.new.shift(fill_value=0)) &
+        (df.old > df.old.shift(fill_value=0))
+    ]
+    df = df[
+        (df.old == df.new.shift(fill_value=0)) |
+        (df.old == min(df.old)) |
+        (df.new == max(df.new))
+    ]
 
-    return df
+    df = df.sort_values("date")
 
+    return df
 
-async def update_stock_capital(code: str):
-    """
-    Update (or download for the first time) Stock capital
+def get_stock_capitals_history(code: str) -> pd.DataFrame:
+    url = f"http://tsetmc.com/Loader.aspx?ParTree=15131H&i={code}"
+    response = requests.get(url).text
+    df = cleanup_stock_capitals_records(response)
+    df["code"] = code
 
+    return df
 
-    params:
-    ----------------
-    code: str or intege
-
-    example
-    ----------------
-    `update_stock_capital('44891482026867833') #Done`
-    """
+async def update_stock_capitals(code: str):
+    
     try:
-        now = datetime.now().strftime("%Y%m%d")
+        if not is_stock_in_bourse_or_fara_or_paye(code):
+            return
+        
+        jnow = jdt.now().strftime("%Y%m%d000000")
         try:
             max_date_query = (
-                f"select max(dtyyyymmdd) as date from stock_capital where code = '{code}'"
+                f"select max(up_date) as up_date from stock_capital where code = '{code}'"
             )
             max_date = pd.read_sql(max_date_query, db.engine)
-            last_date = max_date.date.iat[0]
+            last_up_date = max_date.up_date.iat[0]
+
         except Exception as e:
-            last_date = None
+            last_up_date = None
         try:
             # need to updata new capital data
-            if last_date is None or str(last_date) < now:
+            if last_up_date is None or last_up_date < jnow:
                 url = f"http://tsetmc.com/Loader.aspx?ParTree=15131H&i={code}"
             else:  # The capital data for this code is updateed
                 return
         except Exception as e:
             print(f"Error on formating capital:{str(e)}")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
-                data = await resp.text()
-
-        df = pd.read_html(data)[0]
+                response = await resp.text()
+        
+        df = cleanup_stock_capitals_records(response)
 
-        df.columns = ["dtyyyymmdd", "new_capital", "old_capital"]
-        df["new_capital"] = df["new_capital"].apply(value_to_float)
-        df["old_capital"] = df["old_capital"].apply(value_to_float)
-        df["dtyyyymmdd"] = (
-            df.dtyyyymmdd
-            .jalali.parse_jalali("%Y/%m/%d")
-            .jalali.to_gregorian()
-            .apply(lambda x: x.strftime("%Y%m%d"))
-            .astype(int)
-        )
         df["code"] = code
+        df["up_date"]= jnow
 
-        try:
-            q = f"select dtyyyymmdd from stock_capital where code = '{code}'"
-            temp = pd.read_sql(q, db.engine)
-            df = df[~df.dtyyyymmdd.isin(temp.dtyyyymmdd)]
-        except:
-            pass
-
-        df.to_sql(
-            "stock_capital",
-            db.engine,
-            if_exists="append",
-            index=False
+        fill_table_of_db_with_df(
+            df,
+            columns="date",
+            table="stock_capital",
+            conditions=f"where code = '{code}'",
+            text=f"stock: {code}"
         )
+
         return True, code
 
     except Exception as e:
         return e, code
 
 
-def update_group_capital(code):
-    """
-    Update and download data of all stocks in a group.
-
-    `Warning: Stock table should be updated`
-    """
-    stocks = db.session.query(Stocks.code).filter_by(group_code=code).all()
-    print("updating group", code, end="\r")
+def update_stocks_capitals(codes, msg=""):
     loop = asyncio.get_event_loop()
-    tasks = [update_stock_capital(stock[0]) for stock in stocks]
+    tasks = [update_stock_capitals(code) for code in codes]
     try:
         results = loop.run_until_complete(asyncio.gather(*tasks))
     except RuntimeError:
         WARNING_COLOR = "\033[93m"
         ENDING_COLOR = "\033[0m"
         print(WARNING_COLOR, "Please update stock table", ENDING_COLOR)
         print(
             f"{WARNING_COLOR}If you are using jupyter notebook, please run following command:{ENDING_COLOR}"
         )
         print("```")
         print("%pip install nest_asyncio")
         print("import nest_asyncio; nest_asyncio.apply()")
-        print("from codal_tsetmc.download import get_all_capital")
-        print("get_all_capital()")
         print("```")
         raise RuntimeError
+    print(msg, end="\r")
+    return results
+
 
-    print("group", code, "updated", end="\r")
+def update_stocks_group_capitals(group_code):
+    stocks = db.session.query(Stocks.code).filter_by(group_code=group_code).all()
+    print(f"{' '*25} group: {group_code}", end="\r")
+    codes = [stock[0] for stock in stocks]
+    msg = "group "+group_code+" updated"
+    results = update_stocks_capitals(codes, msg)
     return results
 
 
-def get_all_capital():
+def fill_stocks_capitals_table():
     codes = db.session.query(db.distinct(Stocks.group_code)).all()
     for i, code in enumerate(codes):
         print(
-            f"{' '*18} total progress: {100*(i+1)/len(codes):.2f}%",
+            f"{' '*35} total progress: {100*(i+1)/len(codes):.2f}%",
             end="\r",
         )
-        update_group_capital(code[0])
+        update_stocks_group_capitals(code[0])
 
-    print("Capital Download Finished.", " "*20)
+    print("Capital Download Finished.", " "*50)
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/download/dividend.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/download/tsetmc/price.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,166 +1,169 @@
+from jdatetime import date as jdate
+from jdatetime import datetime as jdt
 from datetime import datetime
 import asyncio
 import aiohttp
 import pandas as pd
-import numpy as np
-import requests
 import io
+import requests
 
 import codal_tsetmc.config as db
-from codal_tsetmc.models import Stocks
+from codal_tsetmc.models.stocks import Stocks
+from codal_tsetmc.tools import *
+from codal_tsetmc.download.tsetmc.stock import is_stock_in_bourse_or_fara_or_paye
 
 
-def get_stock_dividend_history(code: str) -> pd.DataFrame:
-    """Get stock dividend from the web.
 
-    params:
-    ----------------
-    code: str
-        code -> symbol
-        http://www.tsetmc.com/tsev2/data/DPSData.aspx?s=فولاد
-        string after s=
-
-    return:
-    ----------------
-    pd.DataFrame
-        dtyyyymmdd: str
-        dividend: float
-
-    example
-    ----------------
-    df = get_stock_dividend_history('44891482026867833')
-    """
-    symbol = Stocks.query.filter_by(code=code).first().name
-    url = f"http://www.tsetmc.com/tsev2/data/DPSData.aspx?s={symbol}"
-    r = requests.get(url).content.decode("utf-8").replace(";", "\n").replace("@", ",")
-    df = (
-        pd.read_csv(io.StringIO(r), header=None)[[1, 2, 6]]
-        .replace(r'^\s*$', np.nan, regex=True)
-        .dropna().drop_duplicates()
-    )
-    df.columns = ["jdate", "fiscal_year", "dividend"]
-    df = df[~df["dividend"].isin(["0", "0.00", 0])]
-    df["jdate"] = df.jdate.jalali.parse_jalali("%Y/%m/%d")
-    df["fiscal_year"] = df.fiscal_year.jalali.parse_jalali("%Y/%m/%d")
-    df["dtyyyymmdd"] = (
-        df.jdate.jalali.to_gregorian()
-        .apply(lambda x: x.strftime("%Y%m%d"))
+def get_index_prices_history():
+    code = "32097828799138957"
+    url = f'http://www.tsetmc.com/tsev2/chart/data/Index.aspx?i={code}&t=value'
+    s = requests.get(url, verify=False).content
+    df = pd.read_csv(io.StringIO(s.decode("utf-8").replace(";", "\n")), header=None)
+    df.columns = ["date", "price"]
+    df["date"] = df["date"].jalali.parse_jalali("%Y/%m/%d").apply(lambda x: x.strftime('%Y%m%d000000'))
+    df["code"] = code
+    df["ticker"] = "INDEX"
+    df = df.sort_values("date")
+
+    return df
+
+def update_index_prices():
+    index = "32097828799138957"
+    df = get_index_prices_history()
+    df["up_date"] = jdt.now().strftime("%Y%m%d000000")
+    fill_table_of_db_with_df(
+        df, 
+        columns="date",
+        table="stock_price",
+        conditions=f"where code = '{index}'",
+        text=f"stock: {index}"
     )
 
+
+def get_stock_price_daily(code: str, date: str):
+    data = "ClosingPrice/GetClosingPriceDaily"
+    dict_data = get_data_from_cdn_tsetmec_api(data, code, date)
+    
+    return dict_data["closingPriceDaily"]["pClosing"]
+
+def cleanup_stock_prices_records(response):
+    df = pd.read_csv(io.StringIO(response))
+    df.columns = [i[1:-1].lower() for i in df.columns]
+    df["date"] = df["dtyyyymmdd"].apply(lambda x: datetime.strptime(str(x), "%Y%m%d"))
+    df["date"] = df["date"].jalali.to_jalali().apply(lambda x: x.strftime('%Y%m%d000000'))
+    df["price"] = df["close"]
+    df = df.sort_values("date")
+
+    return df[["date", "ticker", "price"]]
+
+def get_stock_prices_history(code: str, from_date="20000101", to_date=datetime.now().strftime("%Y%m%d")) -> pd.DataFrame:
+    url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom={from_date}&DateTo={to_date}&b=0"
+    response = requests.get(url).text
+    df = cleanup_stock_prices_records(response)
+    df["code"] = code
+
     return df
 
 
-async def update_stock_dividend(code: str):
-    """
-    Update (or download for the first time) Stock dividend
 
 
-    params:
-    ----------------
-    code: str or intege
-
-    example
-    ----------------
-    `update_stock_dividend('44891482026867833') #Done`
-    """
+async def update_stock_prices(code: str):
     try:
+        if not is_stock_in_bourse_or_fara_or_paye(code):
+            return
+        
         now = datetime.now().strftime("%Y%m%d")
         try:
-            max_date_query = (
-                f"select max(dtyyyymmdd) as date from stock_dividend where code = '{code}'"
-            )
-            max_date = pd.read_sql(max_date_query, db.engine)
-            last_date = max_date.date.iat[0]
+            query_index = f"select max(date) as date from stock_price where ticker = INDEX"
+            max_date_index = pd.read_sql(query_index, db.engine)
+            last_date_index = max_date_index.date.iat[0]
+
+            if last_date_index is None:
+                update_index_prices()
+                max_date_index = pd.read_sql(query_index, db.engine)
+                last_date_index = max_date_index.date.iat[0]
+
+            query_stock = f"select max(date) as date from stock_price where code = {code}"
+            max_date_stock = pd.read_sql(query_stock, db.engine)
+            last_date_stock = max_date_stock.date.iat[0]
+
+            if last_date_index < last_date_stock:
+                update_index_prices()
+                max_date_index = pd.read_sql(query_index, db.engine)
+                last_date_index = max_date_index.date.iat[0]
+
         except Exception as e:
-            last_date = None
+            last_date_stock = None
         try:
-            # need to updata new dividend data
-            if last_date is None or str(last_date) < now:
-                symbol = Stocks.query.filter_by(code=code).first().name
-                url = f"http://www.tsetmc.com/tsev2/data/DPSData.aspx?s={symbol}"
-            else:  # The dividend data for this code is updateed
+            if last_date_stock is None:  # no any record added in database
+                url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom=20000101&DateTo={now}&b=0"
+            elif last_date_stock < last_date_index:  # need to updata new price data
+                last_date = jdt.strptime(str(int(last_date_stock)), "%Y%m%d%H%M%S").togregorian().strftime("%Y%m%d")
+                url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom={str(last_date)}&DateTo={now}&b=0"
+            else:  # The price data for this code is updateed
                 return
         except Exception as e:
-            print(f"Error on formating dividend:{str(e)}")
+            print(f"Error on formating price:{str(e)}")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
-                data = await resp.text()
+                response = await resp.text()
 
-        data = data.replace(";", "\n").replace("@", ",")
-        df = (
-            pd.read_csv(io.StringIO(data), header=None)[[1, 6]]
-            .replace(r'^\s*$', np.nan, regex=True)
-            .dropna().drop_duplicates()
-        )
-        df.columns = ["dtyyyymmdd", "dividend"]
-        df["dividend"] = df["dividend"].astype(float)
-        df = df[~(df["dividend"] == 0)]
-        df["dtyyyymmdd"] = (
-            df.dtyyyymmdd
-            .jalali.parse_jalali("%Y/%m/%d")
-            .jalali.to_gregorian()
-            .apply(lambda x: x.strftime("%Y%m%d"))
-            .astype(int)
-        )
+        df = cleanup_stock_prices_records(response)
         df["code"] = code
-        try:
-            q = f"select dtyyyymmdd from stock_dividend where code = '{code}'"
-            temp = pd.read_sql(q, db.engine)
-            df = df[~df.dtyyyymmdd.isin(temp.dtyyyymmdd)]
-        except:
-            pass
-
-        df.to_sql(
-            "stock_dividend",
-            db.engine,
-            if_exists="append",
-            index=False
+        df["up_date"] = jdt.now().strftime("%Y%m%d000000")
+
+        fill_table_of_db_with_df(
+            df, 
+            columns="date",
+            table="stock_price",
+            conditions=f"where code = '{code}'",
+            text=f"stock: {code}"
         )
+
         return True, code
 
     except Exception as e:
         return e, code
 
-
-def update_group_dividend(code):
-    """
-    Update and download data of all stocks in a group.
-
-    `Warning: Stock table should be updated`
-    """
-    stocks = db.session.query(Stocks.code).filter_by(group_code=code).all()
-    print("updating group", code, end="\r")
+def update_stocks_prices(codes, msg=""):
     loop = asyncio.get_event_loop()
-    tasks = [update_stock_dividend(stock[0]) for stock in stocks]
+    tasks = [update_stock_prices(code) for code in codes]
     try:
         results = loop.run_until_complete(asyncio.gather(*tasks))
     except RuntimeError:
         WARNING_COLOR = "\033[93m"
         ENDING_COLOR = "\033[0m"
         print(WARNING_COLOR, "Please update stock table", ENDING_COLOR)
         print(
             f"{WARNING_COLOR}If you are using jupyter notebook, please run following command:{ENDING_COLOR}"
         )
         print("```")
         print("%pip install nest_asyncio")
         print("import nest_asyncio; nest_asyncio.apply()")
-        print("from tehran_stocks.download import get_all_dividend")
-        print("get_all_dividend()")
         print("```")
         raise RuntimeError
+    print(msg, end="\r")
+    return results
+
 
-    print("group", code, "updated", end="\r")
+def update_stocks_group_prices(group_code):
+    stocks = db.session.query(Stocks.code).filter_by(group_code=group_code).all()
+    print(f"{' '*25} group: {group_code}", end="\r")
+    codes = [stock[0] for stock in stocks]
+    msg = "group " + group_code + " updated"
+    results = update_stocks_prices(codes, msg)
     return results
 
 
-def get_all_dividend():
+def fill_stocks_prices_table():
+    update_index_prices()
     codes = db.session.query(db.distinct(Stocks.group_code)).all()
     for i, code in enumerate(codes):
         print(
-            f"{' '*18} total progress: {100*(i+1)/len(codes):.2f}%",
+            f"{' '*35} total progress: {100*(i+1)/len(codes):.2f}%",
             end="\r",
         )
-        update_group_dividend(code[0])
+        update_stocks_group_prices(code[0])
+    print("Price Download Finished.", " "*50)
 
-    print("Dividend Download Finished.", " "*20)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/initializer.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/initializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import os
 
 from codal_tsetmc import db, models
-from codal_tsetmc.download import (
-    Categories,
-    fill_stock_table,
-    fill_companies_table
-)
+from codal_tsetmc.download import *
 
 
 def init_db():
     print("creating database")
     path = os.path.join(db.HOME_PATH, db.CDL_TSE_FOLDER)
     try:
         os.mkdir(path)
@@ -21,13 +17,19 @@
     models.create()
     print(f"DataBase created in: {path}")
 
 
 def fill_db():
     print("downloading company and stock details from CODAL and TSETMC")
     print("may take few minutes")
-    fill_stock_table()
+    fill_stocks_table()
     fill_companies_table()
-    cat = Categories()
-    cat.fill_categories_table()
+    fill_categories_table()
+    fill_stocks_prices_table()
+    fill_stocks_capitals_table()
+    fill_commodities_prices_table()
     print("For more info go to:")
     print("https://github.com/mohsenebrahimyir/codal-tsetmc")
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/models/companies.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/models/companies.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,116 @@
 from codal_tsetmc.config import *
 from sqlalchemy.orm import relationship
 
 
-class CompanyTypes(Base):
-    __tablename__ = "company_types"
-    
-    id = Column(Integer, primary_key=True)
-    code = Column(String, unique=True)
-    name = Column(String)
-    companies = relationship('Companies', backref='type')
-
-    def __repr__(self):
-        return f"({self.code}, {self.name})"
-
-class CompanyStatuses(Base):
-    __tablename__ = "company_statuses"
-    
-    id = Column(Integer, primary_key=True)
-    code = Column(String, unique=True)
-    name = Column(String)
-    companies = relationship('Companies', backref='status')
-
-    def __repr__(self):
-        return f"({self.code}, {self.name})"
-
 class Companies(Base):
     __tablename__ = "companies"
 
     id = Column(Integer, primary_key=True)
     symbol = Column(String, ForeignKey("stocks.name"), index=True)
     name = Column(String)
     isic = Column(String)
     type_code = Column(String, ForeignKey("company_types.code"), index=True)
     status_code = Column(String, ForeignKey("company_statuses.code"), index=True)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def __repr__(self):
-        return f"({self.symbol}, {self.name}, {self.type.name}, {self.status.name})"
+        return f"({self.symbol}, {self.name}, {self.type.title}, {self.status.title})"
 
 
+class CompanyTypes(Base):
+    __tablename__ = "company_types"
+    
+    id = Column(Integer, primary_key=True)
+    code = Column(Integer, unique=True)
+    title = Column(String)
+    companies = relationship('Companies', backref='type')
+
+    def __repr__(self):
+        return f"({self.code}, {self.title})"
+
+class CompanyStatuses(Base):
+    __tablename__ = "company_statuses"
+    
+    id = Column(Integer, primary_key=True)
+    code = Column(Integer, unique=True)
+    title = Column(String)
+    companies = relationship('Companies', backref='status')
+
+    def __repr__(self):
+        return f"({self.code}, {self.title})"
+
 class ReportTypes(Base):
     __tablename__ = "report_types"
     
     id = Column(Integer, primary_key=True)
-    code = Column(String, unique=True)
-    name = Column(String)
+    code = Column(Integer, unique=True)
+    title = Column(String)
 
     def __repr__(self):
-        return f"({self.code}, {self.name})"
+        return f"({self.code}, {self.title})"
 
 class LetterTypes(Base):
     __tablename__ = "letter_types"
     
     id = Column(Integer, primary_key=True)
-    code = Column(String, unique=True)
-    name = Column(String)
+    code = Column(Integer, unique=True)
+    title = Column(String)
 
     def __repr__(self):
-        return f"({self.code}, {self.name})"
+        return f"({self.code}, {self.title})"
 
 
 class Auditors(Base):
     __tablename__ = "auditors"
     
     id = Column(Integer, primary_key=True)
-    code = Column(String, unique=True)
+    code = Column(Integer, unique=True)
     name = Column(String)
 
     def __repr__(self):
-        return f"({self.code}, {self.name})"
+        return f"({self.code}, {self.name})"
+
+class Letters(Base):
+    __tablename__ = "letters"
+    
+    id = Column(Integer, primary_key=True)
+    publish_date_time = Column(Integer)
+    sent_date_time = Column(Integer)
+    tracing_no = Column(Integer, unique=True)
+    letter_serial = Column(String, unique=True)
+    letter_title = Column(String)
+    letter_code = Column(String)
+    letter_types = Column(String, ForeignKey("letter_types.title"), index=True)
+    company_symbol = Column(String, ForeignKey("companies.symbol"), index=True)
+    company_name = Column(String)
+
+    def __repr__(self):
+        return f"(گزارشات کدال)"
+
+
+# class FinancialStatement(Base):
+#     __tablename__ = "financial_statement"
+    
+#     id = Column(Integer, primary_key=True)
+#     tracing_no = Column(Integer)
+#     symbol = Column(String, ForeignKey("stocks.name"), index=True)
+#     period = Column(Integer)
+#     sent_date_time = Column(Integer)
+#     publish_date_time = Column(Integer)
+#     period_end_to_date = Column(Integer)
+#     year_end_to_date = Column(Integer)
+#     table_fa = Column(String)
+#     table_en = Column(String)
+#     alias_name = Column(String) 
+#     version_no = Column(Integer)
+#     item_fa = Column(String)
+#     item_en = Column(String)
+#     value = Column(Integer)
+#     is_audited = Column(Boolean)
+#     is_consolidated = Column(Boolean)
+
+#     def __repr__(self):
+#         return f"(صورت مالی, {self.name})"
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/models/create.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/models/create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import codal_tsetmc.config as db
 from .stocks import (
     Stocks,
     StockPrice,
-    StockClient,
     StockCapital,
-    StockDividend,
-    StockAdjusted,
+    CommodityPrice
 )
 from .companies import (
     Companies,
     CompanyTypes,
     CompanyStatuses,
     ReportTypes,
     LetterTypes,
     Auditors,
+    Letters
 )
 
 def create_table(Model):
     try:
         Model.__table__.create(db.engine)
     except:
         pass
 
 def create():
     models = [
-        Stocks, StockPrice, StockClient, StockCapital,
-        StockDividend, StockAdjusted, Companies, CompanyTypes,
-        CompanyStatuses, ReportTypes, LetterTypes, Auditors
+        Stocks, StockPrice, StockCapital,
+        Companies, CompanyTypes, CompanyStatuses,
+        ReportTypes, LetterTypes, Auditors, 
+        Letters,
+        CommodityPrice
     ]
     for model in models:
         create_table(model)
```

### Comparing `codal_tsetmc-1.2.0/src/codal_tsetmc/tools/exception.py` & `codal_tsetmc-1.3.0/src/codal_tsetmc/tools/exception.py`

 * *Files identical despite different names*

### Comparing `codal_tsetmc-1.2.0/PKG-INFO` & `codal_tsetmc-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codal-tsetmc
-Version: 1.2.0
+Version: 1.3.0
 Summary: Data Downloader for Codal and Tehran stock market
 Home-page: https://mohsenebrahimyir.github.io/codal-tsetmc/
 License: MIT
 Author: Mohsen Ebrahimi
 Author-email: mohsenebrahimy.ir@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,32 +19,51 @@
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: finplot (>=1.9.0,<2.0.0)
 Requires-Dist: jalali-pandas (>=0.2.0,<0.3.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: tehran_stocks (>=1.0.9,<2.0.0)
 Project-URL: Repository, https://github.com/mohsenebrahimyir/codal-tsetmc.git
 Description-Content-Type: text/markdown
 
 # کدال و بورس در پایتون
 
+این پکیچ برای ذخیره داده‌های سایت کدال و بازار سرمایه برای اهداف تحلیل بنیادی تهیه شده است.
+
 ## پایگاه داده
 
 ### TSETMC
 
 - [X] `tehran_stocks`: ویرایش بعضی از کدهای بسته
-- [X] `stock_client`: پایگاه داده خرید و فروش حقیقی و حقوقی
-- [X] `stock_dividend`: پایگاه داده تقسیم سود.
+    - 
+
 - [X] `stock_capital`: پایگاه داده افزایش سرمایه
-- [X] `stock_adjsuted`: پایگاه داده تعدیل قیمت
 
 ### CODAL
 
 - [X] `companies`: لیست تمام شرکت‌ها
 - [X] `company_statuses`: وضعیت شرکت‌ها
 - [X] `company_types`: نوع شرکت‌ها
 - [X] `report_types`: گروه اطلاعیه‌ها
-- [X] `financial_years`: 
-- [X] `letter_types`:
-- [X] `auditors`:
+- [X] `financial_years`: سال مالی‌ها
+- [X] `letter_types`: نوع گزارش
+- [X] `auditors`: حسابرس‌ها
+
+#### OTHER
+
+- [X] `commodities`: افزون قیمت‌های کامودیتی
+    - [X] <api.tgju.org>
+
+### Update package
+
+اگر این متن را میبینید یعنی این پکیج درحال توسعه است و قابلیت استفاده در پروژه‌های مهم را ندارد.
+
+```
+# python3 -m pip install --upgrade build
+python3 -m build
+
+# python3 -m pip install --upgrade twine
+python3 -m twine upload --repository pypi dist/*
+
+```
+
```

