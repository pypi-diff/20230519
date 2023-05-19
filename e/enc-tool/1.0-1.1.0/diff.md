# Comparing `tmp/enc_tool-1.0.tar.gz` & `tmp/enc_tool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enc_tool-1.0.tar", last modified: Fri May 19 07:25:06 2023, max compression
+gzip compressed data, was "enc_tool-1.1.0.tar", last modified: Fri May 19 09:28:26 2023, max compression
```

## Comparing `enc_tool-1.0.tar` & `enc_tool-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 07:25:06.917816 enc_tool-1.0/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1577 2023-05-19 07:25:06.917816 enc_tool-1.0/PKG-INFO
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1359 2023-05-19 07:20:06.000000 enc_tool-1.0/README.md
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 07:25:06.917816 enc_tool-1.0/enc_tool.egg-info/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1577 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/PKG-INFO
--rw-rw-r--   0 night-error  (1000) night-error  (1000)      304 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)        1 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       54 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/entry_points.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       22 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/requires.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       20 2023-05-19 07:25:06.000000 enc_tool-1.0/enc_tool.egg-info/top_level.txt
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 07:25:06.917816 enc_tool-1.0/encrypter_decrypter/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)        0 2023-05-19 07:20:06.000000 enc_tool-1.0/encrypter_decrypter/__init__.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1887 2023-05-19 07:20:06.000000 enc_tool-1.0/encrypter_decrypter/enc_tool.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     3444 2023-05-19 07:20:06.000000 enc_tool-1.0/encrypter_decrypter/main.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       38 2023-05-19 07:25:06.917816 enc_tool-1.0/setup.cfg
--rw-rw-r--   0 night-error  (1000) night-error  (1000)      771 2023-05-19 07:20:06.000000 enc_tool-1.0/setup.py
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.035150 enc_tool-1.1.0/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1623 2023-05-19 09:28:26.035150 enc_tool-1.1.0/PKG-INFO
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1419 2023-05-19 09:17:51.000000 enc_tool-1.1.0/README.md
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.027150 enc_tool-1.1.0/enc_tool.egg-info/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1623 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      332 2023-05-19 09:28:26.000000 enc_tool-1.1.0/enc_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)        1 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       54 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       22 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/requires.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       20 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/top_level.txt
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.031150 enc_tool-1.1.0/encrypter_decrypter/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)        0 2023-05-19 08:07:57.000000 enc_tool-1.1.0/encrypter_decrypter/__init__.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     2292 2023-05-19 08:49:47.000000 enc_tool-1.1.0/encrypter_decrypter/enc_tool.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     3565 2023-05-19 09:18:22.000000 enc_tool-1.1.0/encrypter_decrypter/main.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      101 2023-05-19 09:07:41.000000 enc_tool-1.1.0/encrypter_decrypter/test.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       38 2023-05-19 09:28:26.035150 enc_tool-1.1.0/setup.cfg
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      860 2023-05-19 09:12:43.000000 enc_tool-1.1.0/setup.py
```

### Comparing `enc_tool-1.0/PKG-INFO` & `enc_tool-1.1.0/enc_tool.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
-Name: enc_tool
-Version: 1.0
-Summary: A tool to encrypt and decrypt your data!                 
+Name: enc-tool
+Version: 1.1.0
+Summary: A tool to encrypt and decrypt your data! 
 Author: Night Error
 Author-email: night.error.go@gmail.com
 Description-Content-Type: text/markdown
 
 # ENC Tool
 A Python command-line too encrypt and decrypt your data securely.
 <br><br>
 
-## Installation
+# Installation
+## Easy way
+```shell
+pip install enc-tool
+```
+
+## Hard way
 - Clone the project
 ``` shell
 git clone https://github.com/errornight/enc-tool.git
 ```
 ``` shell
 cd enc-tool
 ```
@@ -26,37 +32,38 @@
 or
 ``` shell
 pip install .
 ```
 
 <br>
 
-## Usage
+# Usage
 - To encrypt a short message
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD
 ```
 - To save the encrypted data **in a file**
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD -s WHERE-TO-SAVE
 ```
 - To encrypt data **from a file**
 ``` shell
 enc -p PASSWORD -f FILE-TO-ENCRYPT -s WHERE-TO-SAVE
 ```
-- For decryption add **-dec** to your command
+- For decryption add **-d** to your command
 ```shell
-enc -dec -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
+enc -d -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
 ```
 
 
 <br>
 
-## Where is **ENC-Tool** Useful?
+# Where is **ENC-Tool** Useful?
 - **Secure Communication:** Use ENC-Tool to encrypt sensitive messages or data before sending them through insecure channels.
 - **Data Protection:** Safeguard confidential data such as passwords, credit card numbers, or personal information by encrypting it using ENC-Tool.
 - **File Encryption:** Encrypt files containing important documents, private records, or sensitive information to prevent unauthorized access.<br>
 
 *Remember that in this version you can not encrypt files like images, But you can encrypt the text data in text files.*
+<br><br>
 
-## Contributing
+# Contributing
 Open a pull request and let me know what you think :)
```

### Comparing `enc_tool-1.0/README.md` & `enc_tool-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # ENC Tool
 A Python command-line too encrypt and decrypt your data securely.
 <br><br>
 
-## Installation
+# Installation
+## Easy way
+```shell
+pip install enc-tool
+```
+
+## Hard way
 - Clone the project
 ``` shell
 git clone https://github.com/errornight/enc-tool.git
 ```
 ``` shell
 cd enc-tool
 ```
@@ -18,37 +24,38 @@
 or
 ``` shell
 pip install .
 ```
 
 <br>
 
-## Usage
+# Usage
 - To encrypt a short message
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD
 ```
 - To save the encrypted data **in a file**
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD -s WHERE-TO-SAVE
 ```
 - To encrypt data **from a file**
 ``` shell
 enc -p PASSWORD -f FILE-TO-ENCRYPT -s WHERE-TO-SAVE
 ```
-- For decryption add **-dec** to your command
+- For decryption add **-d** to your command
 ```shell
-enc -dec -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
+enc -d -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
 ```
 
 
 <br>
 
-## Where is **ENC-Tool** Useful?
+# Where is **ENC-Tool** Useful?
 - **Secure Communication:** Use ENC-Tool to encrypt sensitive messages or data before sending them through insecure channels.
 - **Data Protection:** Safeguard confidential data such as passwords, credit card numbers, or personal information by encrypting it using ENC-Tool.
 - **File Encryption:** Encrypt files containing important documents, private records, or sensitive information to prevent unauthorized access.<br>
 
 *Remember that in this version you can not encrypt files like images, But you can encrypt the text data in text files.*
+<br><br>
 
-## Contributing
+# Contributing
 Open a pull request and let me know what you think :)
```

### Comparing `enc_tool-1.0/enc_tool.egg-info/PKG-INFO` & `enc_tool-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
-Name: enc-tool
-Version: 1.0
-Summary: A tool to encrypt and decrypt your data!                 
+Name: enc_tool
+Version: 1.1.0
+Summary: A tool to encrypt and decrypt your data! 
 Author: Night Error
 Author-email: night.error.go@gmail.com
 Description-Content-Type: text/markdown
 
 # ENC Tool
 A Python command-line too encrypt and decrypt your data securely.
 <br><br>
 
-## Installation
+# Installation
+## Easy way
+```shell
+pip install enc-tool
+```
+
+## Hard way
 - Clone the project
 ``` shell
 git clone https://github.com/errornight/enc-tool.git
 ```
 ``` shell
 cd enc-tool
 ```
@@ -26,37 +32,38 @@
 or
 ``` shell
 pip install .
 ```
 
 <br>
 
-## Usage
+# Usage
 - To encrypt a short message
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD
 ```
 - To save the encrypted data **in a file**
 ``` shell
 enc "THE-MESSAGE" -p PASSWORD -s WHERE-TO-SAVE
 ```
 - To encrypt data **from a file**
 ``` shell
 enc -p PASSWORD -f FILE-TO-ENCRYPT -s WHERE-TO-SAVE
 ```
-- For decryption add **-dec** to your command
+- For decryption add **-d** to your command
 ```shell
-enc -dec -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
+enc -d -f FILE-TO-DECRYPT -p PASSWORD -S WHERE-TO-SAVE
 ```
 
 
 <br>
 
-## Where is **ENC-Tool** Useful?
+# Where is **ENC-Tool** Useful?
 - **Secure Communication:** Use ENC-Tool to encrypt sensitive messages or data before sending them through insecure channels.
 - **Data Protection:** Safeguard confidential data such as passwords, credit card numbers, or personal information by encrypting it using ENC-Tool.
 - **File Encryption:** Encrypt files containing important documents, private records, or sensitive information to prevent unauthorized access.<br>
 
 *Remember that in this version you can not encrypt files like images, But you can encrypt the text data in text files.*
+<br><br>
 
-## Contributing
+# Contributing
 Open a pull request and let me know what you think :)
```

### Comparing `enc_tool-1.0/encrypter_decrypter/enc_tool.py` & `enc_tool-1.1.0/encrypter_decrypter/enc_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
 from cryptography.fernet import Fernet, InvalidToken
 import sys
-from colorama import Fore, Style
+from colorama import Fore, Style, init
+init(autoreset=True)
+import os
 
 def fernet_encrypt(data, password):
     # generate encryption KEY base on the password provided!
     hash_obj = hashes.Hash(hashes.SHA256(), backend=default_backend())
     hash_obj.update(password.encode())
     key = base64.urlsafe_b64encode(hash_obj.finalize())
 
@@ -53,8 +55,19 @@
         print(Fore.RED + "Error: Path you've givent does not exist!")
         sys.exit()
     except FileNotFoundError:
         print(Fore.RED + "Error: Path you've givent is not available!!")
         sys.exit()
     except UnicodeDecodeError:
         print(Fore.RED + Style.BRIGHT + "ENC still can not encrypt this kind of file!\nThis feature will be added soon...")
-        sys.exit()
+        sys.exit()
+
+def path_manager(path):
+    # check if the given path is a file and exists
+    if not os.path.isfile(path) or not os.path.exists(path):
+        print(Fore.RED + f"Your given path: {path}, Does not exists or is not a file!")
+        sys.exit()
+    
+    file_path = os.path.abspath(path)
+
+    return [os.path.dirname(file_path) + "/", os.path.basename(file_path)]
+
```

### Comparing `enc_tool-1.0/encrypter_decrypter/main.py` & `enc_tool-1.1.0/encrypter_decrypter/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from encrypter_decrypter import enc_tool as enc
 import argparse
+import json
 # Just styles
 from colorama import Fore, Style, init
 init(autoreset=True)
 
+# read data from config file
+with open("encrypter_decrypter/config/config.json", "r") as file:
+    config = json.load(file)
+
 
 def main():
-    parser = argparse.ArgumentParser(description="A tool to encrypt and decrypt your data! \
-                                     \n Use it to make safe your messages and files...", 
-                                     prog='ENC encrypter / decrypter')
+    parser = argparse.ArgumentParser(prog= config['name'], 
+                                    description= config['description'])
     parser.add_argument('data', nargs='?', help="The message you want to encrypt.")
     parser.add_argument('-p', '--password', help="Password to encrypt or decrypt your data.", required=True)
-    parser.add_argument('-dec', '--decrypt', help="Add this for decryption", action="store_true")
+    parser.add_argument('-d', '--decrypt', help="Add this for decryption", action="store_true")
     parser.add_argument('-s', '--save', help="Path to file that encrypted / decrypted data will be saved in.")
     parser.add_argument('-f', '--file', help="Path to file that you want encrypt / decrypt data in it.")
     args = parser.parse_args()
 
     if not args.decrypt:
         if args.file:
             data = enc.read_data(args.file)
             enc_data = enc.fernet_encrypt(data, args.password)
 
-            file_path = args.save or f'encrypted_{args.file}'
+            path = enc.path_manager(args.file)
+            file_path = args.save or f'{path[0]}encrypted_{path[1]}'
             enc.save_data(enc_data, file_path)
             print(Fore.BLUE + "Your data was encrypted succesfully.", 
               Style.BRIGHT + Fore.WHITE + f"Encrypted data saved in '{file_path}'",
               Style.DIM + f"Your password key: {args.password}",
               sep="\n")
         else:
             if not args.data:
@@ -47,15 +52,16 @@
 
 
     elif args.decrypt:
         if args.file:
             data = enc.read_data(args.file)
             dec_data = enc.fernet_decrypt(data, args.password)
 
-            file_path = args.save or f'decrypted_{args.file}'
+            path = enc.path_manager(args.file)
+            file_path = args.save or f'{path[0]}decrypted_{path[1]}'
             enc.save_data(dec_data, file_path)
             print(Fore.GREEN + "Your data was decrypted succesfully.", 
               Style.BRIGHT + Fore.WHITE + f"Decrypted data saved in '{file_path}'",
               sep="\n")
         
         else:
             if not args.data:
```

### Comparing `enc_tool-1.0/setup.py` & `enc_tool-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup, find_packages
 import os
-
+import json
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+# read data from config file
+with open(os.path.join(directory, "encrypter_decrypter/config/config.json"), "r") as file:
+    config = json.load(file)
+
 setup(
-    name='enc_tool',
-    version='1.0',
+    name=config['name'],
+    version= config['version'],
     packages=find_packages(),
-    description="A tool to encrypt and decrypt your data! \
-                \n Use it to make  your messages and files safe...",
+    description= config['description'],
     long_description= long_description,
     long_description_content_type="text/markdown",
-    author= "Night Error",
-    author_email="night.error.go@gmail.com",
+    author= config['author'],
+    author_email= config['author_email'],
 
     entry_points={
         'console_scripts': [
             'enc = encrypter_decrypter.main:main',
         ],
     },
     install_requires=[
```

