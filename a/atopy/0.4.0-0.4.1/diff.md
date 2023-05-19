# Comparing `tmp/atopy-0.4.0.tar.gz` & `tmp/atopy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atopy-0.4.0.tar", last modified: Fri Mar 10 14:30:54 2023, max compression
+gzip compressed data, was "atopy-0.4.1.tar", last modified: Sat Mar 18 09:47:36 2023, max compression
```

## Comparing `atopy-0.4.0.tar` & `atopy-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1799 2023-03-08 23:58:59.597810 atopy-0.4.0/.gitignore
--rw-r--r--   0        0        0     1060 2023-03-08 23:58:59.597810 atopy-0.4.0/LICENSE
--rw-r--r--   0        0        0      228 2023-03-08 23:58:59.597810 atopy-0.4.0/README.md
--rw-r--r--   0        0        0       51 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/__init__.py
--rw-r--r--   0        0        0     1654 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/datetime.py
--rw-r--r--   0        0        0     2081 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/decimal.py
--rw-r--r--   0        0        0      521 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/io.py
--rw-r--r--   0        0        0      328 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/main.py
--rw-r--r--   0        0        0        0 2023-03-08 23:58:59.597810 atopy-0.4.0/atopy/py.typed
--rw-r--r--   0        0        0      228 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/pydantic.py
--rw-r--r--   0        0        0       85 2023-03-10 14:30:20.515317 atopy-0.4.0/atopy/typer.py
--rwxr-xr-x   0        0        0      138 2023-03-08 23:58:59.597810 atopy-0.4.0/lint.sh
--rw-r--r--   0        0        0     1383 2023-03-10 14:30:20.515317 atopy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 atopy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-03-18 00:53:41.335528 atopy-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1060 2023-03-18 00:53:41.335528 atopy-0.4.1/LICENSE
+-rw-r--r--   0        0        0      228 2023-03-18 00:53:41.335528 atopy-0.4.1/README.md
+-rw-r--r--   0        0        0       51 2023-03-18 09:47:22.039899 atopy-0.4.1/atopy/__init__.py
+-rw-r--r--   0        0        0     1654 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/datetime.py
+-rw-r--r--   0        0        0     1834 2023-03-18 09:47:22.039899 atopy-0.4.1/atopy/decimal.py
+-rw-r--r--   0        0        0      521 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/io.py
+-rw-r--r--   0        0        0      328 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/main.py
+-rw-r--r--   0        0        0        0 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/py.typed
+-rw-r--r--   0        0        0      228 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/pydantic.py
+-rw-r--r--   0        0        0       85 2023-03-18 00:53:41.335528 atopy-0.4.1/atopy/typer.py
+-rwxr-xr-x   0        0        0      138 2023-03-18 00:53:41.335528 atopy-0.4.1/lint.sh
+-rw-r--r--   0        0        0     1383 2023-03-18 00:53:41.335528 atopy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 atopy-0.4.1/PKG-INFO
```

### Comparing `atopy-0.4.0/.gitignore` & `atopy-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atopy-0.4.0/LICENSE` & `atopy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atopy-0.4.0/atopy/datetime.py` & `atopy-0.4.1/atopy/datetime.py`

 * *Files identical despite different names*

### Comparing `atopy-0.4.0/atopy/decimal.py` & `atopy-0.4.1/atopy/decimal.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,31 +55,18 @@
     return ticksize * div_di_ceil(price, ticksize)
 
 
 def qty_unit(qty: Decimal, qtyunit: Decimal) -> Decimal:
     return qtyunit * div_di_down(qty, qtyunit)
 
 
-def cash_qty(
-    cash: Decimal,
-    price: Decimal,
-    cash_leverage: Decimal,
-    contract_unit: Decimal,
-    qtyunit: Decimal,
-) -> Decimal:
-    return qty_unit(
-        div(cash * cash_leverage, price * contract_unit),
-        qtyunit,
-    )
-
-
 def cash_risk_qty(
     cash: Decimal,
+    bet_fraction: Decimal,
+    risk_point: Decimal,
     contract_unit: Decimal,
     qtyunit: Decimal,
-    risk_point: Decimal,
-    risk_target: Decimal,
 ) -> Decimal:
     return qty_unit(
-        div(cash * risk_target, risk_point * contract_unit),
+        div(cash * bet_fraction, risk_point * contract_unit),
         qtyunit,
     )
```

### Comparing `atopy-0.4.0/atopy/io.py` & `atopy-0.4.1/atopy/io.py`

 * *Files identical despite different names*

### Comparing `atopy-0.4.0/pyproject.toml` & `atopy-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atopy-0.4.0/PKG-INFO` & `atopy-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atopy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Common Library
 Author-email: Tom <nanticj@users.noreply.github.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: loguru >=0.6,<0.7
 Requires-Dist: pydantic >=1.10,<1.11
```

