# Comparing `tmp/zood-0.7.3.tar.gz` & `tmp/zood-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.7.3.tar", max compression
+gzip compressed data, was "zood-0.7.4.tar", max compression
```

## Comparing `zood-0.7.3.tar` & `zood-0.7.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      550 2023-05-02 07:49:37.104309 zood-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.3/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.3/zood/__init__.py
--rw-r--r--   0        0        0     6257 2023-04-29 06:11:53.294334 zood-0.7.3/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.3/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.3/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.3/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.3/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.3/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.3/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.3/zood/config/img/sun.png
--rw-r--r--   0        0        0    18347 2023-05-02 07:49:02.542223 zood-0.7.3/zood/config/index.css
--rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.3/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     1040 2023-04-29 02:59:13.107114 zood-0.7.3/zood/config/js/check_box.js
--rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.3/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     1951 2023-05-01 15:04:11.534885 zood-0.7.3/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.3/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.3/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.3/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.3/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.3/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.3/zood/config/js/search.js
--rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.3/zood/config/template.html
--rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.3/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.3/zood/md_parser.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.3/zood/util.py
--rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.3/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.3/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-05-19 00:23:55.203739 zood-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.4/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.4/zood/__init__.py
+-rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.4/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.4/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.4/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.4/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.4/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.4/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.4/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.4/zood/config/img/sun.png
+-rw-r--r--   0        0        0    18737 2023-05-19 00:22:38.369521 zood-0.7.4/zood/config/index.css
+-rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.4/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.4/zood/config/js/check_box.js
+-rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.4/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.4/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.4/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.4/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.4/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.4/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.4/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.4/zood/config/js/search.js
+-rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.4/zood/config/template.html
+-rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.4/zood/main.py
+-rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.4/zood/md_parser.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.4/zood/util.py
+-rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.4/zood/zood.py
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.4/setup.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.4/PKG-INFO
```

### Comparing `zood-0.7.3/pyproject.toml` & `zood-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.7.3"
+version = "0.7.4"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.7.3/zood/config/_config.yml` & `zood-0.7.4/zood/config/_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 
   # 导航栏距离左侧距离 -> 左对齐
   navigator_left: 83%
 
   # 导航栏顶部距离
   navigator_top: 10%
 
+  # 导航栏宽度
+  navigator_max_width: 15%
+
   # 一级条目上下间距
   dir_item_margin: "25px"
 
   # 一级条目左间距
   dir_item_margin_left: "-10px"
 
   # 二级条目上下间距
```

### Comparing `zood-0.7.3/zood/config/img/enter.png` & `zood-0.7.4/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/index.css` & `zood-0.7.4/zood/config/index.css`

 * *Files 3% similar despite different names*

```diff
@@ -339,14 +339,18 @@
 
 .markdown-body pre #code_copy:hover {
   background-color: #ffffff;
   box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
   border-radius: 5px;
 }
 
+.markdown-body ul li blockquote {
+  margin-top: 10px;
+}
+
 .changeMode {
   position: absolute;
   right: 50px;
   top: 50px;
   padding: 5px;
   border-radius: 50%;
   background-color: #e3e3e3;
@@ -585,14 +589,22 @@
   margin-bottom: "<%dir_item_margin%>";
   margin-left: "<%dir_item_margin_left%>";
   list-style: none;
   position: relative;
   /* box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px; */
 }
 
+.dir-tree ul li a {
+  display: inline-block;
+  max-width: 100%;
+  overflow: hidden;
+  text-overflow: ellipsis;
+  white-space: nowrap;
+}
+
 .search-bar::-webkit-scrollbar {
   display: none; /* Chrome Safari */
 }
 
 .search-bar {
   cursor: pointer;
   display: flex;
@@ -835,14 +847,15 @@
   /* transition: all 0.5s; */
   /* border-radius: 5px; */
 }
 
 .header-navigator {
   display: none;
   position: fixed;
+  width: "<%navigator_max_width%>";
   left: "<%navigator_left%>";
   top: "<%navigator_top%>";
   font-family: "<%font_family%>";
   font-size: "<%dir_item_font_size%>";
   letter-spacing: "<%letter_spacing%>";
   scrollbar-width: none; /* Firefox */
   -ms-overflow-style: none; /* IE 10+ */
@@ -873,7 +886,15 @@
   list-style: none;
   position: relative;
 }
 
 .header-navigator ul ul {
   margin-left: -20px;
 }
+
+.header-navigator a {
+  display: inline-block;
+  max-width: 100%;
+  overflow: hidden;
+  text-overflow: ellipsis;
+  white-space: nowrap;
+}
```

### Comparing `zood-0.7.3/zood/config/js/change_mode.js` & `zood-0.7.4/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/check_box.js` & `zood-0.7.4/zood/config/js/check_box.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 7% similar despite different names*

```diff
@@ -40,26 +40,26 @@
 00000270: 6b73 2e66 6f72 4561 6368 2866 756e 6374  ks.forEach(funct
 00000280: 696f 6e28 6c69 6e6b 2920 7b0d 0a20 2069  ion(link) {..  i
 00000290: 6620 286c 696e 6b2e 6872 6566 203d 3d3d  f (link.href ===
 000002a0: 2063 7572 7265 6e74 5572 6c29 207b 0d0a   currentUrl) {..
 000002b0: 2020 2020 6c69 6e6b 2e73 6372 6f6c 6c49      link.scrollI
 000002c0: 6e74 6f56 6965 7728 7b62 6c6f 636b 3a20  ntoView({block: 
 000002d0: 2763 656e 7465 7227 2c20 696e 6c69 6e65  'center', inline
-000002e0: 3a20 276e 6561 7265 7374 272c 2063 6f6e  : 'nearest', con
-000002f0: 7461 696e 6572 3a20 6469 7254 7265 6520  tainer: dirTree 
-00000300: 7d29 3b0d 0a20 2020 2069 6620 2873 6176  });..    if (sav
-00000310: 6564 5468 656d 6529 207b 0d0a 2020 2020  edTheme) {..    
-00000320: 2020 2020 6966 2028 7361 7665 6454 6865      if (savedThe
-00000330: 6d65 203d 3d20 2764 6172 6b27 2920 7b0d  me == 'dark') {.
-00000340: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
-00000350: 6b2e 636c 6173 734c 6973 742e 6164 6428  k.classList.add(
-00000360: 226c 696e 6b2d 6163 7469 7665 2d64 6172  "link-active-dar
-00000370: 6b22 293b 0d0a 2020 2020 2020 2020 7d20  k");..        } 
-00000380: 656c 7365 207b 0d0a 2020 2020 2020 2020  else {..        
-00000390: 2020 2020 6c69 6e6b 2e63 6c61 7373 4c69      link.classLi
-000003a0: 7374 2e61 6464 2822 6c69 6e6b 2d61 6374  st.add("link-act
-000003b0: 6976 6522 293b 0d0a 2020 2020 2020 2020  ive");..        
-000003c0: 7d0d 0a20 2020 207d 2065 6c73 6520 7b0d  }..    } else {.
-000003d0: 0a20 2020 2020 2020 206c 696e 6b2e 636c  .        link.cl
-000003e0: 6173 734c 6973 742e 6164 6428 226c 696e  assList.add("lin
-000003f0: 6b2d 6163 7469 7665 2229 3b0d 0a20 2020  k-active");..   
-00000400: 207d 0d0a 2020 7d0d 0a7d 293b 0d0a 0d0a   }..  }..});....
+000002e0: 3a27 6e65 6172 6573 7427 2c20 636f 6e74  :'nearest', cont
+000002f0: 6169 6e65 723a 2064 6972 5472 6565 207d  ainer: dirTree }
+00000300: 293b 0d0a 2020 2020 6966 2028 7361 7665  );..    if (save
+00000310: 6454 6865 6d65 2920 7b0d 0a20 2020 2020  dTheme) {..     
+00000320: 2020 2069 6620 2873 6176 6564 5468 656d     if (savedThem
+00000330: 6520 3d3d 2027 6461 726b 2729 207b 0d0a  e == 'dark') {..
+00000340: 2020 2020 2020 2020 2020 2020 6c69 6e6b              link
+00000350: 2e63 6c61 7373 4c69 7374 2e61 6464 2822  .classList.add("
+00000360: 6c69 6e6b 2d61 6374 6976 652d 6461 726b  link-active-dark
+00000370: 2229 3b0d 0a20 2020 2020 2020 207d 2065  ");..        } e
+00000380: 6c73 6520 7b0d 0a20 2020 2020 2020 2020  lse {..         
+00000390: 2020 206c 696e 6b2e 636c 6173 734c 6973     link.classLis
+000003a0: 742e 6164 6428 226c 696e 6b2d 6163 7469  t.add("link-acti
+000003b0: 7665 2229 3b0d 0a20 2020 2020 2020 207d  ve");..        }
+000003c0: 0d0a 2020 2020 7d20 656c 7365 207b 0d0a  ..    } else {..
+000003d0: 2020 2020 2020 2020 6c69 6e6b 2e63 6c61          link.cla
+000003e0: 7373 4c69 7374 2e61 6464 2822 6c69 6e6b  ssList.add("link
+000003f0: 2d61 6374 6976 6522 293b 0d0a 2020 2020  -active");..    
+00000400: 7d0d 0a20 207d 0d0a 7d29 3b0d 0a0d 0a    }..  }..});....
```

### Comparing `zood-0.7.3/zood/config/js/copy_code.js` & `zood-0.7.4/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/navigator.js` & `zood-0.7.4/zood/config/js/navigator.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -7,14 +7,18 @@
         event.preventDefault();
         let target = document.querySelector(this.getAttribute('href'));
         target.scrollIntoView({
             behavior: 'smooth',
             block: 'start',
             inline: 'nearest'
         });
+        // 修改网页 URL
+        let url = window.location.href.split('#')[0]; // 获取当前 URL 并去除 # 及后面的内容
+        let newUrl = url + this.getAttribute('href'); // 将当前 URL 与链接的 href 属性拼接
+        history.pushState(null, null, newUrl); // 修改网页 URL
     });
 });
 
 function isScrolledIntoView(elem) {
     var docViewTop = window.pageYOffset;
     var docViewBottom = docViewTop + window.innerHeight;
     var elemTop = elem.offsetTop;
```

### Comparing `zood-0.7.3/zood/config/js/next_front.js` & `zood-0.7.4/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/picture_preview.js` & `zood-0.7.4/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/prismjs/prism.css` & `zood-0.7.4/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/prismjs/prism.js` & `zood-0.7.4/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/js/search.js` & `zood-0.7.4/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/config/template.html` & `zood-0.7.4/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/main.py` & `zood-0.7.4/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/md_parser.py` & `zood-0.7.4/zood/md_parser.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/util.py` & `zood-0.7.4/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/zood/zood.py` & `zood-0.7.4/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.3/setup.py` & `zood-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkdownParser', 'PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['zood = zood.main:main']}
 
 setup_kwargs = {
     'name': 'zood',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': 'web page documentation & comment generation documentation',
     'long_description': '# zood\n\nzood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客\n\n## 主题预览\n\n[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)\n\n## 安装与使用\n\n```bash\npip install zood\n```\n\n参见 [用户使用文档](https://luzhixing12345.github.io/zood/)\n\n## 参考\n\n- [UI](https://remixicon.com/)',
     'author': 'kamilu',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/zood',
```

### Comparing `zood-0.7.3/PKG-INFO` & `zood-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.7.3
+Version: 0.7.4
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

