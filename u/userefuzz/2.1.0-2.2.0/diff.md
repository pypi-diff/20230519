# Comparing `tmp/userefuzz-2.1.0.tar.gz` & `tmp/userefuzz-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userefuzz-2.1.0.tar", last modified: Mon Jan 16 06:28:20 2023, max compression
+gzip compressed data, was "userefuzz-2.2.0.tar", last modified: Fri May 19 17:28:23 2023, max compression
```

## Comparing `userefuzz-2.1.0.tar` & `userefuzz-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-01-16 06:28:20.177682 userefuzz-2.1.0/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1066 2022-12-13 07:35:38.000000 userefuzz-2.1.0/LICENSE
--rw-rw-r--   0 kun       (1000) kun       (1000)     5718 2023-01-16 06:28:20.177682 userefuzz-2.1.0/PKG-INFO
--rw-rw-r--   0 kun       (1000) kun       (1000)     5393 2023-01-16 06:26:55.000000 userefuzz-2.1.0/README.md
--rw-rw-r--   0 kun       (1000) kun       (1000)       38 2023-01-16 06:28:20.177682 userefuzz-2.1.0/setup.cfg
--rw-rw-r--   0 kun       (1000) kun       (1000)      660 2023-01-16 06:24:49.000000 userefuzz-2.1.0/setup.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-01-16 06:28:20.177682 userefuzz-2.1.0/userefuzz/
--rw-rw-r--   0 kun       (1000) kun       (1000)     5126 2022-12-13 06:58:29.000000 userefuzz-2.1.0/userefuzz/__init__.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     8397 2022-12-14 04:58:13.000000 userefuzz-2.1.0/userefuzz/__main__.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-01-16 06:28:20.177682 userefuzz-2.1.0/userefuzz.egg-info/
--rw-rw-r--   0 kun       (1000) kun       (1000)     5718 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/PKG-INFO
--rw-rw-r--   0 kun       (1000) kun       (1000)      270 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/SOURCES.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)        1 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/dependency_links.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)       55 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/entry_points.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)       18 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/requires.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)       10 2023-01-16 06:28:20.000000 userefuzz-2.1.0/userefuzz.egg-info/top_level.txt
+drwxr-xr-x   0 tanishq   (1000) tanishq   (1000)        0 2023-05-19 17:28:23.281048 userefuzz-2.2.0/
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     1066 2023-05-19 17:16:07.000000 userefuzz-2.2.0/LICENSE
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     5221 2023-05-19 17:28:23.281048 userefuzz-2.2.0/PKG-INFO
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     4916 2023-05-19 17:27:47.000000 userefuzz-2.2.0/README.md
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)       38 2023-05-19 17:28:23.281048 userefuzz-2.2.0/setup.cfg
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)      660 2023-05-19 17:16:23.000000 userefuzz-2.2.0/setup.py
+drwxr-xr-x   0 tanishq   (1000) tanishq   (1000)        0 2023-05-19 17:28:23.281048 userefuzz-2.2.0/userefuzz/
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     6232 2023-05-19 17:16:56.000000 userefuzz-2.2.0/userefuzz/__init__.py
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     6929 2023-05-19 17:16:56.000000 userefuzz-2.2.0/userefuzz/__main__.py
+drwxr-xr-x   0 tanishq   (1000) tanishq   (1000)        0 2023-05-19 17:28:23.281048 userefuzz-2.2.0/userefuzz.egg-info/
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)     5221 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/PKG-INFO
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)      270 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)        1 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)       54 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/entry_points.txt
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)       18 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/requires.txt
+-rw-r--r--   0 tanishq   (1000) tanishq   (1000)       10 2023-05-19 17:28:23.000000 userefuzz-2.2.0/userefuzz.egg-info/top_level.txt
```

### Comparing `userefuzz-2.1.0/LICENSE` & `userefuzz-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userefuzz-2.1.0/PKG-INFO` & `userefuzz-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: userefuzz
-Version: 2.1.0
+Version: 2.2.0
 Summary: User-Agent and Referer Header SQLI Fuzzer
 Home-page: https://github.com/root-tanishq/userefuzz
 Author: Tanishq Rathore
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/userefuzz_icon.png">
+<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/ufz_banner_may_23.png">
 </p>
 <h1 align="center">
 
 [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://pypi.org/project/userefuzz/) 
 [![MIT](https://img.shields.io/github/license/root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/LICENSE) 
-[![Version](https://img.shields.io/badge/Latest--Version-2.1.0-brightgreen)](#)
+[![Version](https://img.shields.io/badge/Latest--Version-2.2.0-brightgreen)](#)
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)](https://twitter.com/root_tanishq) <br />
 [![Youtube](https://img.shields.io/youtube/channel/subscribers/UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/@boyfromfuture69)
 [![Github](https://img.shields.io/github/stars/root-tanishq/userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://expy.bio/tanishq)
 </h1>
 
 <h3 align="center">
 
 User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`<br/>
-**Works on `linux`, `Windows` and `MacOS` based systems**<br />
+**Works on `linux` and `unix` based systems**<br />
 </h3>
 
 <table>
 <tr>
 <td>  
 
 <h3 align="center">
@@ -50,23 +49,23 @@
 
 # Installation
 </h1>
 
 ### pip
 
 ```sh
-pip install userefuzz
+sudo pip install userefuzz
 ```
 
 ### setup
 
 ```sh
 git clone https://github.com/root-tanishq/userefuzz
 cd userefuzz
-python3 setup.py install
+sudo python3 setup.py install
 ```
 
 <h1 align="center">
 
 # Usage  
 </h1>
 <h2 align="center">
@@ -134,29 +133,28 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg.png">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg2.png">
 </p>
 
 ### Custom payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <CUSTOM SQLI PAYLOAD> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject.png">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject2.png">
-</p>
 
 ### Multi payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <SQLI PAYLOAD FILE> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject.png">
-</p>
 
 ### Custom header injection
 ```sh
 $ userefuzz <LIST/URL> -ch <CUSTOM HEADER NAME>
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject2.png">
@@ -189,26 +187,7 @@
 
 
 
 ### Output file content
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_out_md.png">
 </p>
-<table>
-<tr>
-<td>  
-<h2 align="center">
-
-## Telify Notifications
-</h2>
-
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration file for sending notification .So inorder to use this feature you need to setup telify.
-
-```sh
-$ userefuzz <LIST / URL> -t
-```
-
-</td>
-</tr>
-</table>
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: userefuzz Version: 2.1.0 Summary: User-Agent and
+Metadata-Version: 2.1 Name: userefuzz Version: 2.2.0 Summary: User-Agent and
 Referer Header SQLI Fuzzer Home-page: https://github.com/root-tanishq/userefuzz
-Author: Tanishq Rathore License: MIT Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Description-Content-Type: text/markdown License-File:
-LICENSE
+Author: Tanishq Rathore License: MIT Classifier: Programming Language :: Python
+:: 3 Description-Content-Type: text/markdown License-File: LICENSE
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              userefuzz_icon.png]
+                            ufz_banner_may_23.png]
  ****** [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://
   pypi.org/project/userefuzz/) [![MIT](https://img.shields.io/github/license/
  root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/
-   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.1.0-
+   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.2.0-
   brightgreen)](#) [![Twitter URL](https://img.shields.io/twitter/url/https/
   twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)]
                       (https://twitter.com/root_tanishq)
         [![Youtube](https://img.shields.io/youtube/channel/subscribers/
        UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/
 @boyfromfuture69) [![Github](https://img.shields.io/github/stars/root-tanishq/
 userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://
                            expy.bio/tanishq) ******
  **** User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`
-           **Works on `linux`, `Windows` and `MacOS` based systems**
+                 **Works on `linux` and `unix` based systems**
                                       ****
                         **** ### Legal Disclaimer ****
 Usage of userefuzz for attacking targets without prior mutual consent is
 illegal. It is the end user's responsibility to obey all applicable local,
 state and federal laws. Developers assume no liability and are not responsible
 for any misuse or damage caused by this program
                          ****** # Installation ******
-### pip ```sh pip install userefuzz ``` ### setup ```sh git clone https://
-github.com/root-tanishq/userefuzz cd userefuzz python3 setup.py install ```
+### pip ```sh sudo pip install userefuzz ``` ### setup ```sh git clone https://
+github.com/root-tanishq/userefuzz cd userefuzz sudo python3 setup.py install
+```
                              ****** # Usage ******
                           ***** ## Parsing URLs *****
 ### Parsing a list of URLs ```sh $ userefuzz -l  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                 u_2.1_list.png]
 ### Parsing a URL ```sh $ userefuzz -u  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
@@ -54,24 +54,19 @@
   u_2.1_proxy.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                          main/images/u_2.1_proxy2.png]
 ### Custom message in request ```sh $ userefuzz
 RL> -m  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_msg.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/
                             images/u_2.1_msg2.png]
-### Custom payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
- u_2.1_pinject.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
-                        main/images/u_2.1_pinject2.png]
-### Multi payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              u_2.1_finject.png]
-### Custom header injection ```sh $ userefuzz
+### Custom payload with custom sleep > Replace `sleep time` with `$UFZ$`
+variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Multi payload with custom sleep > Replace `sleep time` with
+`$UFZ$` variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Custom header injection ```sh $ userefuzz
 RL> -ch  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_finject2.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                           main/images/u_2.1_sch2.png]
 ### Multi header injection > For multiple headers use `|` as shown below. ```sh
 $ userefuzz
 RL> -ch
@@ -83,12 +78,7 @@
 ### Markdown output ```sh $ userefuzz
 RL> -o  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_output.png]
 ### Output file content
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_out_md.png]
-                      ***** ## Telify Notifications *****
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration
-file for sending notification .So inorder to use this feature you need to setup
-telify. ```sh $ userefuzz
-URL> -t ```
```

### Comparing `userefuzz-2.1.0/README.md` & `userefuzz-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/userefuzz_icon.png">
+<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/ufz_banner_may_23.png">
 </p>
 <h1 align="center">
 
 [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://pypi.org/project/userefuzz/) 
 [![MIT](https://img.shields.io/github/license/root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/LICENSE) 
-[![Version](https://img.shields.io/badge/Latest--Version-2.1.0-brightgreen)](#)
+[![Version](https://img.shields.io/badge/Latest--Version-2.2.0-brightgreen)](#)
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)](https://twitter.com/root_tanishq) <br />
 [![Youtube](https://img.shields.io/youtube/channel/subscribers/UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/@boyfromfuture69)
 [![Github](https://img.shields.io/github/stars/root-tanishq/userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://expy.bio/tanishq)
 </h1>
 
 <h3 align="center">
 
 User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`<br/>
-**Works on `linux`, `Windows` and `MacOS` based systems**<br />
+**Works on `linux` and `unix` based systems**<br />
 </h3>
 
 <table>
 <tr>
 <td>  
 
 <h3 align="center">
@@ -38,23 +38,23 @@
 
 # Installation
 </h1>
 
 ### pip
 
 ```sh
-pip install userefuzz
+sudo pip install userefuzz
 ```
 
 ### setup
 
 ```sh
 git clone https://github.com/root-tanishq/userefuzz
 cd userefuzz
-python3 setup.py install
+sudo python3 setup.py install
 ```
 
 <h1 align="center">
 
 # Usage  
 </h1>
 <h2 align="center">
@@ -122,29 +122,28 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg.png">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg2.png">
 </p>
 
 ### Custom payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <CUSTOM SQLI PAYLOAD> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject.png">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject2.png">
-</p>
 
 ### Multi payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <SQLI PAYLOAD FILE> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject.png">
-</p>
 
 ### Custom header injection
 ```sh
 $ userefuzz <LIST/URL> -ch <CUSTOM HEADER NAME>
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject2.png">
@@ -177,24 +176,7 @@
 
 
 
 ### Output file content
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_out_md.png">
 </p>
-<table>
-<tr>
-<td>  
-<h2 align="center">
-
-## Telify Notifications
-</h2>
-
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration file for sending notification .So inorder to use this feature you need to setup telify.
-
-```sh
-$ userefuzz <LIST / URL> -t
-```
-
-</td>
-</tr>
-</table>
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              userefuzz_icon.png]
+                            ufz_banner_may_23.png]
  ****** [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://
   pypi.org/project/userefuzz/) [![MIT](https://img.shields.io/github/license/
  root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/
-   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.1.0-
+   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.2.0-
   brightgreen)](#) [![Twitter URL](https://img.shields.io/twitter/url/https/
   twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)]
                       (https://twitter.com/root_tanishq)
         [![Youtube](https://img.shields.io/youtube/channel/subscribers/
        UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/
 @boyfromfuture69) [![Github](https://img.shields.io/github/stars/root-tanishq/
 userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://
                            expy.bio/tanishq) ******
  **** User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`
-           **Works on `linux`, `Windows` and `MacOS` based systems**
+                 **Works on `linux` and `unix` based systems**
                                       ****
                         **** ### Legal Disclaimer ****
 Usage of userefuzz for attacking targets without prior mutual consent is
 illegal. It is the end user's responsibility to obey all applicable local,
 state and federal laws. Developers assume no liability and are not responsible
 for any misuse or damage caused by this program
                          ****** # Installation ******
-### pip ```sh pip install userefuzz ``` ### setup ```sh git clone https://
-github.com/root-tanishq/userefuzz cd userefuzz python3 setup.py install ```
+### pip ```sh sudo pip install userefuzz ``` ### setup ```sh git clone https://
+github.com/root-tanishq/userefuzz cd userefuzz sudo python3 setup.py install
+```
                              ****** # Usage ******
                           ***** ## Parsing URLs *****
 ### Parsing a list of URLs ```sh $ userefuzz -l  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                 u_2.1_list.png]
 ### Parsing a URL ```sh $ userefuzz -u  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
@@ -49,24 +50,19 @@
   u_2.1_proxy.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                          main/images/u_2.1_proxy2.png]
 ### Custom message in request ```sh $ userefuzz
 RL> -m  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_msg.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/
                             images/u_2.1_msg2.png]
-### Custom payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
- u_2.1_pinject.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
-                        main/images/u_2.1_pinject2.png]
-### Multi payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              u_2.1_finject.png]
-### Custom header injection ```sh $ userefuzz
+### Custom payload with custom sleep > Replace `sleep time` with `$UFZ$`
+variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Multi payload with custom sleep > Replace `sleep time` with
+`$UFZ$` variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Custom header injection ```sh $ userefuzz
 RL> -ch  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_finject2.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                           main/images/u_2.1_sch2.png]
 ### Multi header injection > For multiple headers use `|` as shown below. ```sh
 $ userefuzz
 RL> -ch
@@ -78,12 +74,7 @@
 ### Markdown output ```sh $ userefuzz
 RL> -o  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_output.png]
 ### Output file content
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_out_md.png]
-                      ***** ## Telify Notifications *****
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration
-file for sending notification .So inorder to use this feature you need to setup
-telify. ```sh $ userefuzz
-URL> -t ```
```

### Comparing `userefuzz-2.1.0/setup.py` & `userefuzz-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name='userefuzz',
-    version='2.1.0',
+    version='2.2.0',
     long_description=readme(),
     long_description_content_type="text/markdown",
     description='User-Agent and Referer Header SQLI Fuzzer',
     url='https://github.com/root-tanishq/userefuzz',
     author='Tanishq Rathore',
     license='MIT',
     packages=['userefuzz'],
```

### Comparing `userefuzz-2.1.0/userefuzz/__init__.py` & `userefuzz-2.2.0/userefuzz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,137 @@
 # UseReFuzz Modules for Python
-# No Documentations will be provided as the modules are only created for UseReFuzz tool only
 # Author = Tanishq Rathore
-# Version = 2.1.0
 import colorama
 import requests
 import urllib3
 import os
+import re
 
 
-def header_injector(url,custom_header,injection_payload,userefuzz_message,http_proxy,output,telify_APITOKEN,telify_CHATID,is_telify,verbose,sleep_time):
-    # For Colouring in Windows and other OS
+def headerInjector(url,customHeader,injectionPayload,ufzMessage,httpProxy,output,verbose,sleepTime,alreadyVuln):
+    # Disable SSL Warnings
+    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+    # For coloring in other OS also
     colorama.init()
-    # Use the following name if you dont want to run the following part of the function
-    # custom_header  = 'NO_CUSTOM_HEADER'
-    # http_proxy = 'NO_PROXY'
+    
+    # customHeader  = 'NO_CUSTOM_HEADER'
+    # httpProxy = 'NO_PROXY'
     # output = 'NO_OUTPUT'
-    # Colour Codes
+
+    # Color codes
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
     SLANT = '\x1B[3m'
 
-    # Disable SSL Warnings
-    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+    # Already Vulnerable URL check
+    if url in alreadyVuln:
+        return None
+
+    # Injection payload configuration
+    if len(re.findall(r'\$UFZ\$' , injectionPayload)) >= 1:
+        iPayload = injectionPayload.replace("$UFZ$" , str(sleepTime))
+        iPayload2 = injectionPayload.replace("$UFZ$" , str(21)) # 21 sleep to verify properly 
+    else:
+        print(f"😺{WARNING}_SQLI Payload not in correct format {bcolors.ENDC}{bcolors.BOLD}# userefuzz --help {ENDC}")
+        exit(0)
 
-    #  X-Auth|Bearer|X-Forward-For
-    if custom_header != 'NO_CUSTOM_HEADER':
-        headlist = custom_header.split('|')
+    # Custom header verification 
+    # X-Auth|Authorization|X-Forwarded-For
+    if customHeader != 'NO_CUSTOM_HEADER': 
+        headList = customHeader.split('|')
         header = {}
-        for head in headlist:
-            header[head] = injection_payload
-        
-        header['UseReFuzz'] = userefuzz_message
+        header2 = {}
+        for head in headList:
+            header[head] = iPayload
+            header2[head] = iPayload2
     else:
-        header = {'User-Agent':injection_payload , 'Referer': injection_payload , 'X-Forwarded-For': injection_payload , 'UseReFuzz': userefuzz_message}
+        header = {'User-Agent':iPayload , 'Referer': iPayload , 'X-Forwarded-For': iPayload , 'UseReFuzz': ufzMessage}
+        header2 = {'User-Agent':iPayload2 , 'Referer': iPayload2 , 'X-Forwarded-For': iPayload2 , 'UseReFuzz': ufzMessage}
+
+
+    # Proxy configuration for sending request
+    proxy = {'http' : httpProxy , 'https': httpProxy}
     
-    proxy = {'http' : http_proxy , 'https': http_proxy}
+    # First checking request
     sess = requests.Session()
-    resp = sess.get(url, headers=header , verify=False)
-    resp_time = resp.elapsed.total_seconds()
-    try:
-        if resp_time >= sleep_time-1:
-            if http_proxy != 'NO_PROXY':
-                try:
-                    sess.get(url , headers=header , verify=False , proxies=proxy , timeout=0.000000000001)
-                except:
-                    pass
-                print(f'{OKGREEN}{BOLD}[💉P{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{OKGREEN} ] URL => {ENDC}', url)
-                print(f'{OKGREEN}{BOLD}[💉P{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{OKGREEN} ] (↑) PAYLOAD => {ENDC}', injection_payload)
-            else:
-                print(f'{OKGREEN}{BOLD}[💉💉{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{OKGREEN} ] URL => {ENDC}', url)
-                print(f'{OKGREEN}{BOLD}[💉💉{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{OKGREEN} ] (↑) PAYLOAD => {ENDC}', injection_payload)
+    resp1 = sess.get(url, headers=header , verify=False)
+    resp1Time = resp1.elapsed.total_seconds()
 
-            if output != 'NO_OUTPUT':
-                fileappend = open(output + ".md" , "a")
-                fileappend.write(f'| {resp_time} | "{url}" | 💉True | "{injection_payload}"\n')
-                fileappend.flush()
-                fileappend.close()
+    # Main Verification
+    try:
+        if resp1Time >= sleepTime and resp1Time <= sleepTime+4: # the 4 is for verification purpose
+            # Secondary verification
+            resp2 = sess.get(url, headers=header2 , verify=False)
+            resp2Time = resp2.elapsed.total_seconds()
+            if resp2Time >= 21 and resp2Time <= 21+4: # the 4 is for verification purpose
+                alreadyVuln.append(url)
+                if httpProxy != 'NO_PROXY': # proxy for sending request to burp or ZAP
+                    try:
+                        sess.get(url , headers=header , verify=False , proxies=proxy , timeout=0.000000000001)
+                    except:
+                        pass
+                    print(f'{OKGREEN}{BOLD}[💉P{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{OKGREEN} ] URL => {ENDC}', url)
+                    print(f'{OKGREEN}{BOLD}[💉P{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{OKGREEN} ] (↑) Payload => {ENDC}', iPayload)
+                    print()
+                else:
+                    print(f'{OKGREEN}{BOLD}[💉💉{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{OKGREEN} ] URL => {ENDC}', url)
+                    print(f'{OKGREEN}{BOLD}[💉💉{ENDC}{OKGREEN}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{OKGREEN} ] (↑) Payload => {ENDC}', iPayload)
+                    print()
 
-            if is_telify == 'TELIFY_UP':
-                telifyurl = f'https://api.telegram.org/bot{telify_APITOKEN}/sendMessage'
-                requests.post(telifyurl, json={'chat_id': telify_CHATID, 'text': f'[💎] (USEREFUZZ)⛓️URL(💻)⛓️ {url} ⛓️RESPONSE TIME(⏲️)⛓️ {resp_time} ⛓️PAYLOAD(🔫)⛓️ {injection_payload}'})
+                if output != 'NO_OUTPUT':
+                    fileappend = open(output + ".md" , "a")
+                    fileappend.write(f'| {resp1Time} | "{url}" | 💉true | "{iPayload}"\n')
+                    fileappend.flush()
+                    fileappend.close()
+            else:
+                if verbose:
+                    print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] URL => {ENDC}', url)
+                    print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] (↑) Payload => {ENDC}', iPayload)
+                    print()
+
+                    if output != 'NO_OUTPUT':
+                        fileappend = open(output + ".md" , "a")
+                        fileappend.write(f'| {resp1Time} | "{url}" | false | "{iPayload}"\n')
+                        fileappend.flush()
+                        fileappend.close()
 
         else:
             if verbose:
-                print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{FAIL} ] URL => {ENDC}', url)
-                print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{FAIL} ] (↑) PAYLOAD => {ENDC}', injection_payload)
+                print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] URL => {ENDC}', url)
+                print(f'{FAIL}{BOLD}[{ENDC}NV{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] (↑) Payload => {ENDC}', iPayload)
+                print()
 
                 if output != 'NO_OUTPUT':
                     fileappend = open(output + ".md" , "a")
-                    fileappend.write(f'| {resp_time} | "{url}" | False | "{injection_payload}"\n')
+                    fileappend.write(f'| {resp1Time} | "{url}" | false | "{iPayload}"\n')
                     fileappend.flush()
                     fileappend.close()
     except:
         if verbose:
-            print(f'{FAIL}{BOLD}[{ENDC}ER{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{FAIL} ] URL => {ENDC}', url)
-            print(f'{FAIL}{BOLD}[{ENDC}ER{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp_time)[:4]}{BOLD}{FAIL} ] (↑) PAYLOAD => {ENDC}', injection_payload)
+            print(f'{FAIL}{BOLD}[{ENDC}ER{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] URL => {ENDC}', url)
+            print(f'{FAIL}{BOLD}[{ENDC}ER{ENDC}{FAIL}{BOLD}] \t[ {ENDC}{str(resp1Time)[:4]}{BOLD}{FAIL} ] (↑) Payload => {ENDC}', iPayload)
+            print()
 
             if output != 'NO_OUTPUT':
                 fileappend = open(output + ".md" , "a")
-                fileappend.write(f'| {resp_time} | "{url}" | ERROR | "{injection_payload}"\n')
+                fileappend.write(f'| {resp1Time} | "{url}" | error | "{iPayload}"\n')
                 fileappend.flush()
                 fileappend.close()
 
-def multi_payload(url_mp,custom_header_mp,injection_payload_mp,userefuzz_message_mp,http_proxy_mp,output_mp,telify_APITOKEN_mp,telify_CHATID_mp,is_telify_mp,verbose_mp,sleep_time_mp):
-    if os.path.exists(injection_payload_mp):
-        payload_file_mp = open(injection_payload_mp, 'r')
-        for payload_file_mp_lines in payload_file_mp.readlines():
-            inject_end = payload_file_mp_lines.replace('\n','')
-            header_injector(url_mp,custom_header_mp,inject_end,userefuzz_message_mp,http_proxy_mp,output_mp,telify_APITOKEN_mp,telify_CHATID_mp,is_telify_mp,verbose_mp,sleep_time_mp)
+
+def multiPayload(urlMp,customHeaderMp,injectionPayloadMp,userefuzzMessageMp,httpProxyMp,outputMp,verboseMp,sleepTimeMp,alreadyVulnMp):
+    if os.path.exists(injectionPayloadMp):
+        payloadFileMp = open(injectionPayloadMp, 'r')
+        for payloadFileMpLines in payloadFileMp.readlines():
+            injectEnd = payloadFileMpLines.replace('\n','')
+            headerInjector(urlMp,customHeaderMp,injectEnd,userefuzzMessageMp,httpProxyMp,outputMp,verboseMp,sleepTimeMp,alreadyVulnMp)
     else:
-        inject_end = injection_payload_mp
-        header_injector(url_mp,custom_header_mp,inject_end,userefuzz_message_mp,http_proxy_mp,output_mp,telify_APITOKEN_mp,telify_CHATID_mp,is_telify_mp,verbose_mp,sleep_time_mp)
+        injectEnd = injectionPayloadMp
+        headerInjector(urlMp,customHeaderMp,injectEnd,userefuzzMessageMp,httpProxyMp,outputMp,verboseMp,sleepTimeMp,alreadyVulnMp)
```

### Comparing `userefuzz-2.1.0/userefuzz/__main__.py` & `userefuzz-2.2.0/userefuzz/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 try:
-    from __init__ import header_injector , multi_payload
+    from __init__ import headerInjector , multiPayload
 except:
-    from userefuzz import header_injector , multi_payload
+    from userefuzz import headerInjector , multiPayload
 
 import colorama
 import argparse
 import os
 import datetime
 import configparser
 import multiprocessing as mp
 import sys
 from functools import partial
 
 # For Colouring on Windows based OS
 colorama.init()
 
-VERSION = '2.1.0'
+VERSION = '2.2.0'
+
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
@@ -47,39 +48,23 @@
 print(banner)
 
 # Arguments
 parser = argparse.ArgumentParser()
 parser.add_argument('-l','--list', type=str,help=f'📄_List of URL to check for Header SQL Injection \t \t {bcolors.BOLD} {bcolors.OKBLUE}-l urllist.txt{bcolors.ENDC}',default="NO_LIST")
 parser.add_argument('-p','--proxy', type=str,help=f'✈️ _Burp proxy or any other proxy to send the request \t \t{bcolors.BOLD} {bcolors.OKBLUE} -p http://127.1:8080{bcolors.ENDC}',default="NO_PROXY")
 parser.add_argument('-m','--message', type=str,help=f'✉️ _Send a message in header for ease of search in Burp history \t \t{bcolors.BOLD} {bcolors.OKBLUE} -m "Just Testing SQLI"{bcolors.ENDC}',default="Testing for SQLI in User-Agent and Referer Header")
-parser.add_argument('-s','--sleep', type=int,help=f'😴_How much sleep is used in your custom payload \t \t{bcolors.BOLD} {bcolors.OKBLUE} -s 12 {bcolors.ENDC} Default Sleep = 10' , default=10)
+parser.add_argument('-s','--sleep', type=int,help=f'😴_How much sleep you want to use with custom payload \t \t{bcolors.BOLD} {bcolors.OKBLUE} -s 12 {bcolors.ENDC} Default Sleep = 10' , default=10)
 parser.add_argument('-v','--verbose', help=f'💣_Display All URLs and output \t \t{bcolors.BOLD} {bcolors.OKBLUE} -v {bcolors.ENDC}', action='store_true' , default=False)
-parser.add_argument('-t','--telify', help=f'💬_Notify on telegram (https://github.com/root-tanishq/telify configuration file required) \t \t{bcolors.BOLD} {bcolors.OKBLUE} -t {bcolors.ENDC}', action='store_true' , default=False)
 parser.add_argument('-o','--output', type=str,help=f'📁_Save the vulnerable URLs to an output file \t \t{bcolors.BOLD} {bcolors.OKBLUE} -o savefile {bcolors.ENDC}', default="NO_OUTPUT")
 parser.add_argument('-u','--url', type=str,help=f'🤖_Pass a URL to check for Header SQLI Injections \t \t{bcolors.BOLD} {bcolors.OKBLUE} -u http://domain.tld/index.php {bcolors.ENDC}', default='NO_URL')
 parser.add_argument('-ch','--customheader', type=str,help=f'🔒_Custom Header for SQLI Injections (For Multiple Header seperate them with | )\t \t{bcolors.BOLD} {bcolors.OKBLUE} FOR ONE HEADER: -ch X-Auth FOR MULTIPLE HEADER: -ch "X-Auth|X-Test|Bearer|Custom_HEAD" {bcolors.ENDC}', default="NO_CUSTOM_HEADER")
 parser.add_argument('-w','--workers', type=int,help=f'👷_No. of workers (Processes) at a time \t \t{bcolors.BOLD} {bcolors.OKBLUE}-w 10 {bcolors.ENDC}\t \t Default Workers = 5',default=5)
-parser.add_argument('-i','--inject', type=str,help=f"""💉_Send your custom payload Or a file of payloads for SQL Injection \t \t{bcolors.BOLD} {bcolors.OKBLUE} -i "'+sleep(10)+'" -i sqli_payloads.txt{bcolors.ENDC} """ , default='"XOR(if(now()=sysdate(),sleep(10),0))XOR"')
+parser.add_argument('-i','--inject', type=str,help=f"""💉_Send your custom payload Or a file of payloads for SQL Injection => `replace sleep with $UFZ$` \t \t{bcolors.BOLD} {bcolors.OKBLUE} -i "'+sleep($UFZ$)+'" -i sqli_payloads.txt{bcolors.ENDC} """ , default='"XOR(if(now()=sysdate(),sleep($UFZ$),0))XOR"')
 args = parser.parse_args()
 
-# Telify
-CHAT_ID = ''
-API_TOKEN = ''
-is_telify_main = 'TELIFY_DOWN'
-if args.telify:    
-    try:
-        config = configparser.ConfigParser()
-        config.read(os.path.join(os.path.expanduser( '~' ),'telify.ini'))
-        CHAT_ID = config['TELIFY']['CHATID']
-        API_TOKEN = config['TELIFY']['APITOKEN']
-        telifyurl = f'https://api.telegram.org/bot{API_TOKEN}/sendMessage'
-        requests.post(telifyurl, json={'chat_id': CHAT_ID, 'text': f'[💡] (USEREFUZZ) Runned on (⏲️) {datetime.datetime.now()} ⏬'})
-        is_telify_main = 'TELIFY_UP'
-    except:
-        print(f"😺{bcolors.WARNING}_No Configuration found , setup telify  now => {bcolors.ENDC}{bcolors.BOLD} https://github.com/root-tanishq/telify {bcolors.ENDC}")
 
 if args.customheader != 'NO_CUSTOM_HEADER':
     print(f'{bcolors.BOLD}{bcolors.OKGREEN}[{bcolors.ENDC}##{bcolors.BOLD}{bcolors.OKGREEN}]{bcolors.ENDC}',' Headers which UseReFuzz using for injection',bcolors.BOLD,bcolors.OKBLUE, args.customheader.replace('|',', '),bcolors.ENDC)
     print()
 else:
     print(f'{bcolors.BOLD}{bcolors.OKGREEN}[{bcolors.ENDC}##{bcolors.BOLD}{bcolors.OKGREEN}]{bcolors.ENDC}',' Headers which UseReFuzz using for injection',bcolors.BOLD,bcolors.OKBLUE,'User-Agent, X-Forwarded-For, Referer',bcolors.ENDC)
     print()
@@ -91,65 +76,59 @@
     if args.customheader != 'NO_CUSTOM_HEADER':
         output_ch = args.customheader.replace('|',', ')
     else:
         output_ch = 'User-Agent, X-Forwarded-For, Referer'
     file.write(f"""
 # UseReFuzz HEADER SQLI INJECTION REPORT
 
-## Author - Tanishq Rathore (Kun)
-## Github - https://github.com/root-tanishq/userefuzz
-## Twitter - https://twitter.com/root_tanishq
-
 > UseReFuzz runned on `{datetime.datetime.now()}`
 
-## Legality
-
-```
-Usage of userefuzz for attacking targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program
-```
-
 - Headers `{output_ch}`
 
 - Sleep used for checking `{args.sleep}`
 
 # Report Results
 | TIME TAKEN | URL | IS VULNERABLE | PAYLOAD |
 | --- | --- | --- | --- |
 """)
     file.close()
 
 def main():
+    # Already vuln check 
+    alreadyVuln = []
+
+    # Parsing 
     if args.url != "NO_URL":
-        multi_payload(args.url,args.customheader,args.inject,args.message,args.proxy,args.output,API_TOKEN,CHAT_ID,is_telify_main,args.verbose,args.sleep)
+        multiPayload(args.url,args.customheader,args.inject,args.message,args.proxy,args.output,args.verbose,args.sleep,alreadyVuln)
     elif args.list != "NO_LIST":
         try:
-            urllist = filter(None , open(args.list,'r').read().split("\n"))
+            urlList = filter(None , open(args.list,'r').read().split("\n"))
             with mp.Pool(args.workers) as worker:
-                multi_fuzz = partial(multi_payload, custom_header_mp=args.customheader,injection_payload_mp=args.inject,userefuzz_message_mp=args.message,http_proxy_mp=args.proxy,output_mp=args.output,telify_APITOKEN_mp=API_TOKEN,telify_CHATID_mp=CHAT_ID,is_telify_mp=is_telify_main,verbose_mp=args.verbose,sleep_time_mp=args.sleep)
-                worker.map(multi_fuzz , urllist)
+                multiFuzz = partial(multiPayload, customHeaderMp=args.customheader,injectionPayloadMp=args.inject,userefuzzMessageMp=args.message,httpProxyMp=args.proxy,outputMp=args.output,verboseMp=args.verbose,sleepTimeMp=args.sleep,alreadyVulnMp=alreadyVuln)
+                worker.map(multiFuzz , urlList)
         except KeyboardInterrupt:
             exit(0)
         except:
             if os.path.isfile(args.list):
                 exit(0)
             else:
                 print(f'😥{bcolors.BOLD}{bcolors.FAIL}_We are unable to read the file or the file does not exist{bcolors.ENDC}')
     elif not sys.stdin.isatty():
         try:
-            urlfile = []
+            urlFile = []
             for line in sys.stdin:
                 try:
-                    urlfile.append(line.split()[0])
+                    urlFile.append(line.split()[0])
                 except:
                     pass
             with mp.Pool(args.workers) as worker:
-                multi_fuzz = partial(multi_payload, custom_header_mp=args.customheader,injection_payload_mp=args.inject,userefuzz_message_mp=args.message,http_proxy_mp=args.proxy,output_mp=args.output,telify_APITOKEN_mp=API_TOKEN,telify_CHATID_mp=CHAT_ID,is_telify_mp=is_telify_main,verbose_mp=args.verbose,sleep_time_mp=args.sleep)
-                worker.map(multi_fuzz , urlfile)
+                multiFuzz = partial(multiPayload, customHeaderMp=args.customheader,injectionPayloadMp=args.inject,userefuzzMessageMp=args.message,httpProxyMp=args.proxy,outputMp=args.output,verboseMp=args.verbose,sleepTimeMp=args.sleep,alreadyVulnMp=alreadyVuln)
+                worker.map(multiFuzz , urlFile)
         except KeyboardInterrupt:
             exit(0)
         except:
             exit(0)
     else:
         print(f"😺{bcolors.WARNING}_No Option Provided please check {bcolors.ENDC}{bcolors.BOLD}# userefuzz --help {bcolors.ENDC}")
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `userefuzz-2.1.0/userefuzz.egg-info/PKG-INFO` & `userefuzz-2.2.0/userefuzz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: userefuzz
-Version: 2.1.0
+Version: 2.2.0
 Summary: User-Agent and Referer Header SQLI Fuzzer
 Home-page: https://github.com/root-tanishq/userefuzz
 Author: Tanishq Rathore
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/userefuzz_icon.png">
+<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/ufz_banner_may_23.png">
 </p>
 <h1 align="center">
 
 [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://pypi.org/project/userefuzz/) 
 [![MIT](https://img.shields.io/github/license/root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/LICENSE) 
-[![Version](https://img.shields.io/badge/Latest--Version-2.1.0-brightgreen)](#)
+[![Version](https://img.shields.io/badge/Latest--Version-2.2.0-brightgreen)](#)
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)](https://twitter.com/root_tanishq) <br />
 [![Youtube](https://img.shields.io/youtube/channel/subscribers/UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/@boyfromfuture69)
 [![Github](https://img.shields.io/github/stars/root-tanishq/userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://expy.bio/tanishq)
 </h1>
 
 <h3 align="center">
 
 User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`<br/>
-**Works on `linux`, `Windows` and `MacOS` based systems**<br />
+**Works on `linux` and `unix` based systems**<br />
 </h3>
 
 <table>
 <tr>
 <td>  
 
 <h3 align="center">
@@ -50,23 +49,23 @@
 
 # Installation
 </h1>
 
 ### pip
 
 ```sh
-pip install userefuzz
+sudo pip install userefuzz
 ```
 
 ### setup
 
 ```sh
 git clone https://github.com/root-tanishq/userefuzz
 cd userefuzz
-python3 setup.py install
+sudo python3 setup.py install
 ```
 
 <h1 align="center">
 
 # Usage  
 </h1>
 <h2 align="center">
@@ -134,29 +133,28 @@
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg.png">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_msg2.png">
 </p>
 
 ### Custom payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <CUSTOM SQLI PAYLOAD> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject.png">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_pinject2.png">
-</p>
 
 ### Multi payload with custom sleep
+
+> Replace `sleep time` with `$UFZ$` variable for double verification of userefuzz
+
 ```sh
 $ userefuzz <LIST/URL> -i <SQLI PAYLOAD FILE> -s <SLEEP COUNT IN THE PAYLOAD>
 ```
-<p align="center">
-<img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject.png">
-</p>
 
 ### Custom header injection
 ```sh
 $ userefuzz <LIST/URL> -ch <CUSTOM HEADER NAME>
 ```
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_finject2.png">
@@ -189,26 +187,7 @@
 
 
 
 ### Output file content
 <p align="center">
 <img src="https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/u_2.1_out_md.png">
 </p>
-<table>
-<tr>
-<td>  
-<h2 align="center">
-
-## Telify Notifications
-</h2>
-
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration file for sending notification .So inorder to use this feature you need to setup telify.
-
-```sh
-$ userefuzz <LIST / URL> -t
-```
-
-</td>
-</tr>
-</table>
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: userefuzz Version: 2.1.0 Summary: User-Agent and
+Metadata-Version: 2.1 Name: userefuzz Version: 2.2.0 Summary: User-Agent and
 Referer Header SQLI Fuzzer Home-page: https://github.com/root-tanishq/userefuzz
-Author: Tanishq Rathore License: MIT Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Description-Content-Type: text/markdown License-File:
-LICENSE
+Author: Tanishq Rathore License: MIT Classifier: Programming Language :: Python
+:: 3 Description-Content-Type: text/markdown License-File: LICENSE
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              userefuzz_icon.png]
+                            ufz_banner_may_23.png]
  ****** [![PYPI](https://img.shields.io/badge/PYPI-UseReFuzz-orange)](https://
   pypi.org/project/userefuzz/) [![MIT](https://img.shields.io/github/license/
  root-tanishq/userefuzz)](https://github.com/root-tanishq/userefuzz/blob/main/
-   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.1.0-
+   LICENSE) [![Version](https://img.shields.io/badge/Latest--Version-2.2.0-
   brightgreen)](#) [![Twitter URL](https://img.shields.io/twitter/url/https/
   twitter.com/root_tanishq.svg?style=social&label=Follow%20%40root_tanishq)]
                       (https://twitter.com/root_tanishq)
         [![Youtube](https://img.shields.io/youtube/channel/subscribers/
        UC0HLRnmOx3x_hsAGAdG9VaQ?style=social)](https://www.youtube.com/
 @boyfromfuture69) [![Github](https://img.shields.io/github/stars/root-tanishq/
 userefuzz?style=social)](https://github.com/root-tanishq/userefuzz/stargazers)
 [![Expy](https://img.shields.io/badge/Author-Tanishq%20Rathore-blue)](https://
                            expy.bio/tanishq) ******
  **** User-Agent , X-Forwarded-For and Referer SQLI Fuzzer made with `python`
-           **Works on `linux`, `Windows` and `MacOS` based systems**
+                 **Works on `linux` and `unix` based systems**
                                       ****
                         **** ### Legal Disclaimer ****
 Usage of userefuzz for attacking targets without prior mutual consent is
 illegal. It is the end user's responsibility to obey all applicable local,
 state and federal laws. Developers assume no liability and are not responsible
 for any misuse or damage caused by this program
                          ****** # Installation ******
-### pip ```sh pip install userefuzz ``` ### setup ```sh git clone https://
-github.com/root-tanishq/userefuzz cd userefuzz python3 setup.py install ```
+### pip ```sh sudo pip install userefuzz ``` ### setup ```sh git clone https://
+github.com/root-tanishq/userefuzz cd userefuzz sudo python3 setup.py install
+```
                              ****** # Usage ******
                           ***** ## Parsing URLs *****
 ### Parsing a list of URLs ```sh $ userefuzz -l  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                 u_2.1_list.png]
 ### Parsing a URL ```sh $ userefuzz -u  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
@@ -54,24 +54,19 @@
   u_2.1_proxy.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                          main/images/u_2.1_proxy2.png]
 ### Custom message in request ```sh $ userefuzz
 RL> -m  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_msg.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/
                             images/u_2.1_msg2.png]
-### Custom payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
- u_2.1_pinject.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
-                        main/images/u_2.1_pinject2.png]
-### Multi payload with custom sleep ```sh $ userefuzz
-RL> -i  -s  ```
-    [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
-                              u_2.1_finject.png]
-### Custom header injection ```sh $ userefuzz
+### Custom payload with custom sleep > Replace `sleep time` with `$UFZ$`
+variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Multi payload with custom sleep > Replace `sleep time` with
+`$UFZ$` variable for double verification of userefuzz ```sh $ userefuzz
+RL> -i  -s  ``` ### Custom header injection ```sh $ userefuzz
 RL> -ch  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
 u_2.1_finject2.png] [https://raw.githubusercontent.com/root-tanishq/userefuzz/
                           main/images/u_2.1_sch2.png]
 ### Multi header injection > For multiple headers use `|` as shown below. ```sh
 $ userefuzz
 RL> -ch
@@ -83,12 +78,7 @@
 ### Markdown output ```sh $ userefuzz
 RL> -o  ```
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_output.png]
 ### Output file content
     [https://raw.githubusercontent.com/root-tanishq/userefuzz/main/images/
                                u_2.1_out_md.png]
-                      ***** ## Telify Notifications *****
-> The Tool uses [Telify](https://github.com/root-tanishq/telify) configuration
-file for sending notification .So inorder to use this feature you need to setup
-telify. ```sh $ userefuzz
-URL> -t ```
```

