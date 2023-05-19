# Comparing `tmp/ebmeta-1.0.4-py3-none-any.whl.zip` & `tmp/ebmeta-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17432 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 06:36 ebmeta/__init__.py
--rw-r--r--  2.0 unx     4205 b- defN 23-May-05 06:36 ebmeta/cli.py
--rw-r--r--  2.0 unx     3748 b- defN 22-Oct-28 03:41 ebmeta/isfdb.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3769 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      689 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/RECORD
-9 files, 47701 bytes uncompressed, 16248 bytes compressed:  65.9%
+Zip file size: 17276 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      355 b- defN 23-May-19 01:14 ebmeta/__init__.py
+-rw-rw-r--  2.0 unx     3270 b- defN 23-May-19 01:14 ebmeta/cli.py
+-rw-rw-r--  2.0 unx     3542 b- defN 23-May-19 01:14 ebmeta/model.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3822 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      691 b- defN 23-May-19 01:15 ebmeta-1.0.5.dist-info/RECORD
+9 files, 46978 bytes uncompressed, 16092 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ebmeta/__init__.py
 Comment: 
 
 Filename: ebmeta/cli.py
 Comment: 
 
-Filename: ebmeta/isfdb.py
+Filename: ebmeta/model.py
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/LICENSE
+Filename: ebmeta-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/METADATA
+Filename: ebmeta-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/WHEEL
+Filename: ebmeta-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/entry_points.txt
+Filename: ebmeta-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/top_level.txt
+Filename: ebmeta-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ebmeta-1.0.4.dist-info/RECORD
+Filename: ebmeta-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ebmeta/__init__.py

```diff
@@ -0,0 +1,23 @@
+00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
+00000010: 7420 6c6f 6767 696e 670a 0a0a 6465 6620  t logging...def 
+00000020: 7374 6465 7272 5f68 616e 646c 6572 2829  stderr_handler()
+00000030: 3a0a 2020 2020 6861 6e64 6c65 7220 3d20  :.    handler = 
+00000040: 6c6f 6767 696e 672e 5374 7265 616d 4861  logging.StreamHa
+00000050: 6e64 6c65 7228 7374 7265 616d 3d73 7973  ndler(stream=sys
+00000060: 2e73 7464 6572 7229 0a20 2020 2066 6f72  .stderr).    for
+00000070: 6d61 7474 6572 203d 206c 6f67 6769 6e67  matter = logging
+00000080: 2e46 6f72 6d61 7474 6572 2866 6d74 3d27  .Formatter(fmt='
+00000090: 2528 6173 6374 696d 6529 7320 2528 6e61  %(asctime)s %(na
+000000a0: 6d65 2973 2025 286c 6576 656c 6e61 6d65  me)s %(levelname
+000000b0: 292d 3873 2025 286d 6573 7361 6765 2973  )-8s %(message)s
+000000c0: 272c 2064 6174 6566 6d74 3d27 2559 2d25  ', datefmt='%Y-%
+000000d0: 6d2d 2564 2025 483a 254d 3a25 5327 290a  m-%d %H:%M:%S').
+000000e0: 2020 2020 6861 6e64 6c65 722e 7365 7446      handler.setF
+000000f0: 6f72 6d61 7474 6572 2866 6f72 6d61 7474  ormatter(formatt
+00000100: 6572 290a 2020 2020 7265 7475 726e 2068  er).    return h
+00000110: 616e 646c 6572 0a0a 0a6c 6f67 6765 7220  andler...logger 
+00000120: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
+00000130: 6765 7228 5f5f 6e61 6d65 5f5f 290a 6c6f  ger(__name__).lo
+00000140: 6767 6572 2e61 6464 4861 6e64 6c65 7228  gger.addHandler(
+00000150: 7374 6465 7272 5f68 616e 646c 6572 2829  stderr_handler()
+00000160: 290a 0a                                  )..
```

## ebmeta/cli.py

```diff
@@ -1,164 +1,116 @@
-import os
 import sys
+import json
 import logging
-import tempfile
 
 import click
 from ebooklib import epub
 
-REVNAMESPACE = { url:ns for ns, url in epub.NAMESPACES.items() }
+from . import logger
+from .model import MyBook
 
-logger = logging.getLogger(__name__)
-
-def stderr_handler():
-    handler = logging.StreamHandler(stream=sys.stderr)
-    formatter = logging.Formatter(fmt='%(asctime)s %(name)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-    handler.setFormatter(formatter)
-    return handler
-
-logger.addHandler(stderr_handler())
 
 @click.group()
 @click.option('--debug', is_flag=True, default=False, help='enable debug output for ebmeta')
 @click.option('--debugall', is_flag=True, default=False, help='enable debug output for everything')
 def cli(debug, debugall):
     if debug:
         logger.setLevel(logging.DEBUG)
     if debugall:
         logging.getLogger('').setLevel(logging.DEBUG)
 
 
-
-
-
-
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 @click.argument('keys', nargs=-1)
 def get(filename, keys):
-    '''get the value of one key'''
-
-    book = epub.read_epub(filename)
-    logger.debug(f'Book {filename} {book.metadata!r}')
+    '''
+    get the value of the specified key, or all keys if unspecified
+    '''
+    book = MyBook.orExit(filename)
 
     if not keys:
-        keys = []
-        for url, kv in book.metadata.items():
-            ns = REVNAMESPACE.get(url, url)
-            for k in kv:
-                keys.append(f'{ns}:{k}')
+        keys = book.all_meta_keys()
 
     for key in keys:
-        if ':' in key:
-            ns, k = key.rsplit(':', 1)
-        else:
-            ns, k = None, key
-
-        show_one_key(filename, book, key, ns, k)
+        book.show_key(key)
 
 
-def show_one_key(filename, book, key, ns, k):
-    try:
-        value = book.get_metadata(ns, k)
-    except KeyError as e:
-        value = 'Key Not Found'
-        logger.exception(e)
-    print(f'{filename} {key} {value}')
-
-
-def show_one_book_key(filename, key, ns, k):
-    book = epub.read_epub(filename)
-    show_one_key(filename, book, key, ns, k)
-    
-
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 def ls(filename):
+    '''
+    List interior files of the specified epub
+    '''
+    book = MyBook.orExit(filename)
 
-    book = epub.read_epub(filename)
-    for item in book.get_items():
+    for item in book.book.get_items():
         print(f'{filename} {item.get_name()} {item.media_type}')
 
+@cli.command()
+@click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
+def metadata(filename):
+    '''
+    List metadata of the specified epub
+    '''
 
-def set_raw_bookmeta(book, ns, k, val):
-    book.metadata[ns] = book.metadata.get(ns, {})
-    book.metadata[ns][k] = val
-
-
-def update_book(filename, book):
-    tempfh = tempfile.NamedTemporaryFile()
-    tempname = tempfh.name
-    tempfh.close()
-
-    epub.write_epub(tempname, book)
-    try:
-        os.rename(tempname, filename)
-    except PermissionError:
-        print(f"PermissionError: can't write to {filename}")
-
-
-def update_book_metadata(filename, ns, k, val):
-    book = epub.read_epub(filename)
-    set_raw_bookmeta(book, ns, k, val)
-    update_book(filename, book)
-
-
-
+    book = MyBook.orExit(filename)
+    print(json.dumps(book.metadata, sort_keys=True, indent=4))
 
 
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 @click.argument('key')
 @click.argument('value')
-def rawset(filename, key, value):
+def set_any(filename, key, value):
     '''set the value of one key
 
        KEY is of the form NAMESPACE:FIELD
        VALUE is eval'd by python
     '''
-
-    if ':' in key:
-        ns, k = key.split(':', 1)
-    else:
-        ns, k = None, key
-
-    ns = epub.NAMESPACES.get(ns, ns)
     val = eval(value)
-    
-    update_book_metadata(filename, ns, k, val)
 
+    MyBook.set_and_save(filename, key, val)
 
 
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 def get_series(filename):
-    ns, k = 'calibre', 'series'
-    show_one_book_key(filename, k, ns, k)
+    '''show the series'''
+    MyBook.show_one_book_key(filename, 'calibre:series')
 
 
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 @click.argument('value')
 def set_series(filename, value):
-    ns, k = 'calibre', 'series'
-    val = [(None, {'name': f'{ns}:{k}', 'content': str(value)})]
-
-    update_book_metadata(filename, ns, k, val)
-
+    '''set the series'''
+    book = MyBook.orExit(filename)
+    book.book.set_unique_metadata('calibre', 'series', str(value))
+    book.save()
 
 @cli.command()
 @click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
 @click.argument('value', type=click.FLOAT)
 def set_series_index(filename, value):
-    ns, k = 'calibre', 'series_index'
-    val = [(None, {'name': f'{ns}:{k}', 'content': str(value)})]
-
-    update_book_metadata(filename, ns, k, val)
+    '''set the series index'''
+    book = MyBook.orExit(filename)
+    book.book.set_unique_metadata('calibre', 'series_index', str(value))
+    book.save()
 
 
+@cli.command()
+@click.argument('filename', type=click.Path(exists=True, dir_okay=False), required=True, nargs=1)
+def rewrite(filename):
+    '''load and save the book in order to upgrade the metadata to EPUB3'''
+    MyBook(filename).save()
 
 
+def cli_wrapper():
+    try:
+        return cli()  # pylint: disable=no-value-for-parameter
+    except Exception as e:
+        logging.debug("Crash! when called with args %r :", sys.argv, exc_info=e)
 
 
 if __name__ == '__main__':
-    cli()  # pylint: disable=no-value-for-parameter
+    cli_wrapper()
```

## Comparing `ebmeta-1.0.4.dist-info/LICENSE` & `ebmeta-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ebmeta-1.0.4.dist-info/METADATA` & `ebmeta-1.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebmeta
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ebook Metadata Munging CLI
 Home-page: http://github.com/pjz/ebmeta
 Author: Paul Jimenez
 Author-email: pj@place.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,15 @@
 Requires-Dist: importlib-metadata (==6.6.0) ; extra == 'dev'
 Requires-Dist: iniconfig (==1.1.1) ; extra == 'dev'
 Requires-Dist: isort (==5.10.1) ; extra == 'dev'
 Requires-Dist: jaraco-classes (==3.2.3) ; extra == 'dev'
 Requires-Dist: jeepney (==0.8.0) ; extra == 'dev'
 Requires-Dist: keyring (==23.13.1) ; extra == 'dev'
 Requires-Dist: lazy-object-proxy (==1.7.1) ; extra == 'dev'
+Requires-Dist: lxml-stubs (==0.4.0) ; extra == 'dev'
 Requires-Dist: markdown-it-py (==2.2.0) ; extra == 'dev'
 Requires-Dist: mccabe (==0.7.0) ; extra == 'dev'
 Requires-Dist: mdurl (==0.1.2) ; extra == 'dev'
 Requires-Dist: more-itertools (==9.1.0) ; extra == 'dev'
 Requires-Dist: mypy (==0.982) ; extra == 'dev'
 Requires-Dist: mypy-extensions (==0.4.3) ; extra == 'dev'
 Requires-Dist: packaging (==21.3) ; extra == 'dev'
```

