# Comparing `tmp/BTKSorgu-1.1.4.tar.gz` & `tmp/BTKSorgu-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.1.4.tar", last modified: Thu May 18 19:45:04 2023, max compression
+gzip compressed data, was "BTKSorgu-1.1.5.tar", last modified: Fri May 19 09:18:41 2023, max compression
```

## Comparing `BTKSorgu-1.1.4.tar` & `BTKSorgu-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.639430 BTKSorgu-1.1.4/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 09:18:41.000000 BTKSorgu-1.1.5/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:18:41.245724 BTKSorgu-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-19 09:18:21.000000 BTKSorgu-1.1.5/setup.py
```

### Comparing `BTKSorgu-1.1.4/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.1.5/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.1.5/BTKSorgu/KekikGUI.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         # ? Pencere Kapanmadan Önce Fonksiyon Tetiklemek
         self.protocol("WM_DELETE_WINDOW", self.pencereyi_kapat)
 
         # ? Pencere Özellikleri
         self.bind("<Escape>",    lambda event: self.pencereyi_kapat()) # * ESC ile çıkış
         self.bind("<F11>",       lambda event: self.tam_ekran())       # * Tam Ekran
         self.bind("<Control-a>", lambda event: self.ctrl_a(event))
+        self.bind("<Control-A>", lambda event: self.ctrl_a(event))
 
         # ? Pencere İkonu
         logo_b64 = encodebytes(open(logo_yolu, "rb").read())
         favicon  = tk.PhotoImage(data=logo_b64)
         self.iconphoto(False, favicon)
 
         # ? Pencere için bir minimum boyut ayarlayın ve ortasına yerleştirin
```

### Comparing `BTKSorgu-1.1.4/BTKSorgu/arayuz.py` & `BTKSorgu-1.1.5/BTKSorgu/arayuz.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
     # Ayırıcı
     kekik.pencere.ayrac = ttk.Separator(kekik.pencere.inputlar_frame)
     kekik.pencere.ayrac.grid(row=2, column=0, padx=(10, 10), pady=10, sticky="ew")
 
 def ara_buton_tiklaninca():
     arama_sorgusu = kekik.pencere.arama_metni.get()
+    if not arama_sorgusu:
+        return False
+
     kekik.pencere.arama_metni.state(["!invalid"])
 
     kekik.pencere.cikti_frame = ttk.Frame(kekik.pencere, padding=(0, 0, 0, 10))
     kekik.pencere.cikti_frame.grid(row=1, column=0, sticky="n")
     kekik.pencere.cikti_frame.columnconfigure(index=0, weight=1)
     kekik.pencere.cikti_frame.rowconfigure(index=0, weight=1)
```

### Comparing `BTKSorgu-1.1.4/BTKSorgu/konsol.py` & `BTKSorgu-1.1.5/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/BTKSorgu/logo.png` & `BTKSorgu-1.1.5/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.1.5/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.4
+Version: 1.1.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.4/LICENSE` & `BTKSorgu-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/PKG-INFO` & `BTKSorgu-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.4
+Version: 1.1.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.4/README.md` & `BTKSorgu-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 14% similar despite different names*

#### Comparing `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -4,18 +4,21 @@
   <metadata_license>CC0-1.0</metadata_license>
   <project_license>GPL-3.0</project_license>
   <id type="desktop">org.KekikAkademi.BTKSorgu.desktop</id>
   <launchable type="desktop-id">org.KekikAkademi.BTKSorgu.desktop</launchable>
   <name>BTKSorgu</name>
   <summary>Is the target website accessible in Turkey? (BTK)</summary>
   <summary xml:lang="tr_TR">Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..</summary>
-  <url type="homepage">https://github.com/keyiflerolsun/BTKSorgu</url>
-  <url type="bugtracker">https://github.com/keyiflerolsun/BTKSorgu/issues</url>
-  <url type="donation">https://keyiflerolsun.me/Kahve</url>
   <developer_name>keyiflerolsun</developer_name>
+  <url type="homepage">https://kekikakademi.org</url>
+  <url type="donation">https://keyiflerolsun.me/Kahve</url>
+  <url type="help">https://t.me/KekikKahve</url>
+  <url type="vcs-browser">https://github.com/keyiflerolsun/BTKSorgu</url>
+  <url type="bugtracker">https://github.com/keyiflerolsun/BTKSorgu/issues</url>
+  <url type="faq">https://blog.keyiflerolsun.dev</url>
   <description>
     <p>Is the target website accessible in Turkey? (BTK)</p>
     <p>An example application prepared with Python language and Tkinter Library.</p>
   </description>
   <description xml:lang="tr_TR">
     <p>Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..</p>
     <p>https://t.me/KekikAkademi için hazırlanmıştır..</p>
@@ -25,14 +28,19 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.1.5" date="2023-5-19">
+      <description>
+        <p>Çeşitli hatalar giderildi..</p>
+      </description>
+    </release>
     <release version="1.1.4" date="2023-5-18">
       <description>
         <p>Github aksiyonlarıyla otomatik paketlenme ve yayınlama eklendi..</p>
       </description>
     </release>
     <release version="1.1.2" date="2023-5-18">
       <description>
```

### Comparing `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.1.5/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.4/setup.py` & `BTKSorgu-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.1.4",
+    version      = "1.1.5",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

