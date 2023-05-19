# Comparing `tmp/idcode-0.1.4.tar.gz` & `tmp/idcode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idcode-0.1.4.tar", max compression
+gzip compressed data, was "idcode-0.2.0.tar", max compression
```

## Comparing `idcode-0.1.4.tar` & `idcode-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.1.4/idcode/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-03 15:18:46.916433 idcode-0.1.4/idcode/cli.py
--rw-r--r--   0        0        0     2123 2023-05-03 15:18:50.169379 idcode-0.1.4/idcode/core_values.py
--rw-r--r--   0        0        0    11443 2023-05-10 12:12:58.897782 idcode-0.1.4/idcode/custom_encoding.py
--rw-r--r--   0        0        0     5713 2023-05-03 15:17:18.838725 idcode-0.1.4/idcode/interactive_decoder.py
--rw-r--r--   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.1.4/idcode/preprocessing.py
--rw-r--r--   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.1.4/LICENSE
--rw-r--r--   0        0        0      503 2023-05-12 08:16:29.106670 idcode-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1554 2023-05-10 12:13:27.926198 idcode-0.1.4/README.md
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 idcode-0.1.4/setup.py
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 idcode-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.2.0/idcode/__init__.py
+-rw-r--r--   0        0        0     1444 2023-05-19 18:12:55.109837 idcode-0.2.0/idcode/cli.py
+-rw-r--r--   0        0        0     2123 2023-05-03 15:18:50.169379 idcode-0.2.0/idcode/core_values.py
+-rw-r--r--   0        0        0    11443 2023-05-10 12:12:58.897782 idcode-0.2.0/idcode/custom_encoding.py
+-rw-r--r--   0        0        0     3281 2023-05-19 18:23:29.855090 idcode-0.2.0/idcode/interactive_decoder.py
+-rw-r--r--   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.2.0/idcode/preprocessing.py
+-rw-r--r--   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.2.0/LICENSE
+-rw-r--r--   0        0        0      503 2023-05-19 17:57:37.788653 idcode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1554 2023-05-10 12:13:27.926198 idcode-0.2.0/README.md
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 idcode-0.2.0/setup.py
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 idcode-0.2.0/PKG-INFO
```

### Comparing `idcode-0.1.4/idcode/cli.py` & `idcode-0.2.0/idcode/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,17 +40,12 @@
 def main():
     args = parse_arguments()
 
     encoded_text = get_encoded_text(args)
 
     decoder = InteractiveDecoder(all_encodings, encoded_text)
 
-    decoded_text, steps = decoder.run()
-
-    print("\n最终解码结果：")
-    print(decoded_text)
-    print("\n经过的解码方式：")
-    print(" -> ".join(steps))
+    decoder.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `idcode-0.1.4/idcode/core_values.py` & `idcode-0.2.0/idcode/core_values.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.4/idcode/custom_encoding.py` & `idcode-0.2.0/idcode/custom_encoding.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.4/LICENSE` & `idcode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idcode-0.1.4/README.md` & `idcode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `idcode-0.1.4/setup.py` & `idcode-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['idcode = idcode.cli:main']}
 
 setup_kwargs = {
     'name': 'idcode',
-    'version': '0.1.4',
+    'version': '0.2.0',
     'description': '交互式检测并解码编码文本。',
     'long_description': '# idcode\n\nidcode 是一个使用 Python 编写的命令行工具，用于交互式检测并解码编码文本。它支持命令行输入和文件输入，可以自动检测编码类型和尝试解码，并提供了一个交互式界面来逐步解码编码文本。\n\n## 支持的编码格式\n\nidcode 支持多种编码格式，包括：\n\n- Base85/Base64/Base32\n- Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8\n- Binary 编码\n- ASCII 编码\n- Hex 编码\n- URL 编码\n- HTML 实体编码\n- Quoted-printable 编码\n- 核心价值观编码\n\n## 安装\n\n从 PyPi 安装：\n\n```sh\npip install idcode\n```\n\n## 用法\n\nidcode 支持交互式输入、命令行输入和文件输入来获取编码文本。\n\n### 交互式输入\n\n当不给出任何命令行参数时，程序会在运行后提示你给出目标文本：\n\n```sh\nidcode\n```\n\n### 命令行输入\n\n要使用命令行输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -t "编码文本"\n```\n\n其中，`-t` 参数用于指定要解码的文本。\n\n### 文件输入\n\n要使用文件输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -f "文件路径"\n```\n\n其中，`-f` 参数用于指定包含编码文本的文件路径。\n\n## 贡献\n\n如果你发现了 bug，或者有改进建议，请随时创建 issue 或者 pull request。我们欢迎任何形式的贡献。\n\n## 许可证\n\nidcode 使用 MIT 许可证。请参阅 LICENSE 文件了解更多详情。',
     'author': 'p0ise',
     'author_email': 'changelf@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/p0ise/idcode',
```

### Comparing `idcode-0.1.4/PKG-INFO` & `idcode-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idcode
-Version: 0.1.4
+Version: 0.2.0
 Summary: 交互式检测并解码编码文本。
 Home-page: https://github.com/p0ise/idcode
 License: MIT
 Author: p0ise
 Author-email: changelf@163.com
 Requires-Python: >=3,<4
 Classifier: License :: OSI Approved :: MIT License
```

