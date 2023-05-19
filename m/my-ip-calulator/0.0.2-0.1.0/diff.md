# Comparing `tmp/my_ip_calulator-0.0.2.tar.gz` & `tmp/my_ip_calulator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_ip_calulator-0.0.2.tar", max compression
+gzip compressed data, was "my_ip_calulator-0.1.0.tar", max compression
```

## Comparing `my_ip_calulator-0.0.2.tar` & `my_ip_calulator-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       72 2023-05-09 22:34:27.326791 my_ip_calulator-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     7324 2023-05-19 14:53:27.147549 my_ip_calulator-0.0.2/README.md
--rw-r--r--   0        0        0     7758 2023-05-19 16:44:49.186464 my_ip_calulator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       38 2023-05-09 22:34:27.340161 my_ip_calulator-0.0.2/src/app/__init__.py
--rw-r--r--   0        0        0    18495 2023-05-19 14:22:59.798550 my_ip_calulator-0.0.2/src/app/calc.py
--rw-r--r--   0        0        0    10979 2023-05-19 16:40:33.275466 my_ip_calulator-0.0.2/src/app/cmd.py
--rw-r--r--   0        0        0     8230 1970-01-01 00:00:00.000000 my_ip_calulator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-19 20:33:56.000000 my_ip_calulator-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0    31615 2023-05-19 20:40:02.338894 my_ip_calulator-0.1.0/README.md
+-rw-r--r--   0        0        0     7763 2023-05-19 20:43:23.451739 my_ip_calulator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-05-19 20:33:56.000000 my_ip_calulator-0.1.0/src/app/__init__.py
+-rw-r--r--   0        0        0    18576 2023-05-19 20:36:52.004295 my_ip_calulator-0.1.0/src/app/calc.py
+-rw-r--r--   0        0        0    11103 2023-05-19 20:43:38.870454 my_ip_calulator-0.1.0/src/app/cmd.py
+-rw-r--r--   0        0        0    32521 1970-01-01 00:00:00.000000 my_ip_calulator-0.1.0/PKG-INFO
```

### Comparing `my_ip_calulator-0.0.2/pyproject.toml` & `my_ip_calulator-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "my-ip-calulator"
-version = "0.0.2"
+version = "0.1.0"
 license = "MIT"
 description = "This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations."
 authors = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 maintainers = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 readme = "README.md"
 packages = [{include = "app", from = "src"}]
 repository = "https://github.com/brunobotelhobr/My-IP-Calculator"
@@ -107,15 +107,15 @@
   "src"
 ]
 
 [tool.taskipy.variables]
 src_dir = "src"
 docs_branch = "documentation"
 package_dir = { var = "src/app", recursive = true }
-package_name = "my-ip-calc"
+package_name = "my-ip-calulator"
 package_version = "0.0.1"
 docker_context = "brunobotelhobr"
 
 [tool.taskipy.tasks]
 pre-commit = { cmd = "task format && task lint && task tests", help = "Run all pre-commit tasks" }
 pre-release = { cmd = "task pre-commit && task bom && task req &&  task sec", help = "Run all pre-release tasks" }
 ----------- = "----------------------------------------"
```

### Comparing `my_ip_calulator-0.0.2/src/app/calc.py` & `my_ip_calulator-0.1.0/src/app/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,18 +133,21 @@
         if self.address.count("::") > 0 or self.address.count(":") < 7:
             return False
         parts: list[str] = self.address.split(":")
         # Check if the address has 8 parts
         if len(parts) != 8:
             return False
         # Check if each part is between 0 and FFFF
-        for part in parts:
-            if not 0 <= int(part, 16) <= int("FFFF", 16):
-                int(part, 16)
-                return False
+        try:
+            for part in parts:
+                if not 0 <= int(part, 16) <= int("FFFF", 16):
+                    int(part, 16)
+                    return False
+        except ValueError:
+            return False
         # Return True if all checks passed
         return True
 
     def expand_v6(self) -> str:
         """Expand v6 address with ::."""
         # If not expandable, return as received.
         # self.addres string container :::
```

### Comparing `my_ip_calulator-0.0.2/src/app/cmd.py` & `my_ip_calulator-0.1.0/src/app/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 cmd = typer.Typer(no_args_is_help=True)
 
 
 @cmd.command()
 def version() -> str:
     """Show version."""
-    app_version: str = "0.0.2"
+    app_version: str = "0.1.0"
     typer.echo(app_version)
     return app_version
 
 
 @cmd.command()
 def val(
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6")],
@@ -86,15 +86,15 @@
             "--output",
             help="Output format for the network address details of an IP address, it supports bin, hex, dec.",
             case_sensitive=False,
             show_choices=True,
         ),
     ] = None,
     mask: Annotated[
-        Optional[str], typer.Argument(help="IP address mask, if not provided an auto generated one will be assigned.")
+        str | None, typer.Argument(help="IP address mask, if not provided an auto generated one will be assigned.")
     ] = None,
 ) -> bool:
     """Calculate the network address from an IP address and a subnet mask, output the address in the desired format."""
     # Identify the address type
     address_version: int = discover_version(address=address)
     # Return False if the address is invalid
     if address_version not in [4, 6]:
@@ -167,15 +167,15 @@
 
 @cmd.command()
 def subnet(  # type: ignore
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6.")],
     mask: Annotated[str, typer.Argument(help="IP address mask.")],
     parts: Annotated[int, typer.Argument(help="Split the netork into this parts.")],
     output: Annotated[
-        Optional[str],
+        str | None,
         typer.Option(
             "-o",
             "--output",
             help="Output format for the network address details of an IP address, it supports bin, hex, dec.",
             case_sensitive=False,
             show_choices=True,
         ),
@@ -228,15 +228,19 @@
     # Validate if the parts are base 2
     if parts < 0:
         Printer().error(name="parts", value=str(parts), message="The parts must be greater than 1")
         return False
     if not log2(parts).is_integer():
         Printer().error(name="parts", value=str(parts), message="The parts must be base 2")
         return False
-    mask = str(MaskCompress(mask=mask, version=address_version).compress())
+    try:
+        mask = str(MaskCompress(mask=mask, version=address_version).compress())
+    except ValueError:
+        Printer().error(name="mask", value=mask, message="Invalid mask")
+        return False
     if address_version == 4:
         if int(mask) + parts > 32:
             Printer().error(name="parts", value=str(parts), message="The parts are too big for the mask")
             return False
     if address_version == 6:
         if int(mask) + parts > 128:
             Printer().error(name="parts", value=str(parts), message="The parts are too big for the mask")
```

