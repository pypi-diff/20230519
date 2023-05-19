# Comparing `tmp/timey_wimey-0.1.1.tar.gz` & `tmp/timey_wimey-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timey_wimey-0.1.1.tar", max compression
+gzip compressed data, was "timey_wimey-0.1.2.tar", max compression
```

## Comparing `timey_wimey-0.1.1.tar` & `timey_wimey-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      709 2023-05-19 02:19:16.572552 timey_wimey-0.1.1/README.md
--rw-r--r--   0        0        0      572 2023-05-19 02:19:01.584827 timey_wimey-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 21:03:17.111855 timey_wimey-0.1.1/timey_wimey/__init__.py
--rw-r--r--   0        0        0     1877 2023-05-19 02:01:59.578323 timey_wimey-0.1.1/timey_wimey/main.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 timey_wimey-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-05-19 02:19:16.572552 timey_wimey-0.1.2/README.md
+-rw-r--r--   0        0        0      572 2023-05-19 20:44:18.984948 timey_wimey-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 21:03:17.111855 timey_wimey-0.1.2/timey_wimey/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-19 20:42:24.242096 timey_wimey-0.1.2/timey_wimey/main.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 timey_wimey-0.1.2/PKG-INFO
```

### Comparing `timey_wimey-0.1.1/README.md` & `timey_wimey-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `timey_wimey-0.1.1/pyproject.toml` & `timey_wimey-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timey-wimey"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple CLI for generating times"
 authors = ["Sam Phinizy <83414895+sam-phinizy@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `timey_wimey-0.1.1/timey_wimey/main.py` & `timey_wimey-0.1.2/timey_wimey/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,28 @@
 
     if interval_type not in valid_interval_types:
         raise ValueError(f"{interval_type} not in {','.join(valid_interval_types)}")
 
     return number,interval_type
 
 
+def print_date(date_obj: pendulum.DateTime,format: Optional[str] = None):
+
+    if format:
+        typer.echo(date_obj.strftime(format))
+    else:
+        typer.echo(date_obj)
+
+
 @app.command()
 def date(
     date_string: str,
     to: Optional[str] = typer.Option(None, help="An optional end time to go to."),
     time_zone: Optional[str] = typer.Option(None,help="Optional timezone to use."),
+    format: Optional[str] = typer.Option(None,help="Stftime format to use."),
     interval: Optional[str] = typer.Option(
         "1 hours", help="Interval to use if a range. Should be like `2 days` or `37 minutes`"
     ),
 ):
 
     if time_zone is None:
         time_zone = tzlocal.get_localzone_name()
@@ -58,22 +67,22 @@
 
     start_date = pendulum.parse(str(parsed_start))
 
     if not parsed_start.tzinfo:
         local_tz = pendulum.timezone(time_zone)
         start_date = local_tz.convert(start_date)
 
-    typer.echo(start_date)
+    print_date(start_date,format)
     if to is None:
         exit(0)
 
     end_date = pendulum.parse(str(dateparser.parse(to)))
 
     period = pendulum.period(start_date,end_date)
 
     amount,unit = parse_range(interval)
 
     for dt in period.range(unit,amount):
-        typer.echo(dt)
+        print_date(dt,format)
 
 if __name__ == "__main__":
     app()
```

### Comparing `timey_wimey-0.1.1/PKG-INFO` & `timey_wimey-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timey-wimey
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI for generating times
 License: MIT
 Author: Sam Phinizy
 Author-email: 83414895+sam-phinizy@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

