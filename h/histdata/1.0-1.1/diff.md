# Comparing `tmp/histdata-1.0.tar.gz` & `tmp/histdata-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/histdata-1.0.tar", last modified: Mon Sep  2 06:23:11 2019, max compression
+gzip compressed data, was "histdata-1.1.tar", last modified: Fri May 19 15:02:08 2023, max compression
```

## Comparing `histdata-1.0.tar` & `histdata-1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 premy    (901776550) staff       (20)        0 2019-09-02 06:23:11.000000 histdata-1.0/
--rw-r--r--   0 premy    (901776550) staff       (20)     4554 2019-09-02 06:23:11.000000 histdata-1.0/PKG-INFO
-drwxr-xr-x   0 premy    (901776550) staff       (20)        0 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/
--rw-r--r--   0 premy    (901776550) staff       (20)     4554 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/PKG-INFO
--rw-r--r--   0 premy    (901776550) staff       (20)      214 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/SOURCES.txt
--rw-r--r--   0 premy    (901776550) staff       (20)       24 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/requires.txt
--rw-r--r--   0 premy    (901776550) staff       (20)        9 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/top_level.txt
--rw-r--r--   0 premy    (901776550) staff       (20)        1 2019-09-02 06:23:11.000000 histdata-1.0/histdata.egg-info/dependency_links.txt
--rw-r--r--   0 premy    (901776550) staff       (20)     3302 2019-09-02 05:00:51.000000 histdata-1.0/README.md
-drwxr-xr-x   0 premy    (901776550) staff       (20)        0 2019-09-02 06:23:11.000000 histdata-1.0/histdata/
--rw-r--r--   0 premy    (901776550) staff       (20)       65 2019-09-02 06:19:34.000000 histdata-1.0/histdata/__init__.py
--rw-r--r--   0 premy    (901776550) staff       (20)     8226 2019-09-02 06:21:56.000000 histdata-1.0/histdata/api.py
--rw-r--r--   0 premy    (901776550) staff       (20)      381 2019-09-02 06:22:31.000000 histdata-1.0/setup.py
--rw-r--r--   0 premy    (901776550) staff       (20)       38 2019-09-02 06:23:11.000000 histdata-1.0/setup.cfg
+drwxr-xr-x   0 philipperemy   (501) wheel        (0)        0 2023-05-19 15:02:08.806460 histdata-1.1/
+-rw-r--r--   0 philipperemy   (501) wheel        (0)    11357 2023-05-19 15:01:34.000000 histdata-1.1/LICENSE
+-rw-r--r--   0 philipperemy   (501) wheel        (0)     4341 2023-05-19 15:02:08.806317 histdata-1.1/PKG-INFO
+-rw-r--r--   0 philipperemy   (501) wheel        (0)     4125 2023-05-19 15:01:34.000000 histdata-1.1/README.md
+drwxr-xr-x   0 philipperemy   (501) wheel        (0)        0 2023-05-19 15:02:08.805591 histdata-1.1/histdata/
+-rw-r--r--   0 philipperemy   (501) wheel        (0)       65 2023-05-19 15:01:34.000000 histdata-1.1/histdata/__init__.py
+-rw-r--r--   0 philipperemy   (501) wheel        (0)     8340 2023-05-19 15:01:34.000000 histdata-1.1/histdata/api.py
+drwxr-xr-x   0 philipperemy   (501) wheel        (0)        0 2023-05-19 15:02:08.806152 histdata-1.1/histdata.egg-info/
+-rw-r--r--   0 philipperemy   (501) wheel        (0)     4341 2023-05-19 15:02:08.000000 histdata-1.1/histdata.egg-info/PKG-INFO
+-rw-r--r--   0 philipperemy   (501) wheel        (0)      222 2023-05-19 15:02:08.000000 histdata-1.1/histdata.egg-info/SOURCES.txt
+-rw-r--r--   0 philipperemy   (501) wheel        (0)        1 2023-05-19 15:02:08.000000 histdata-1.1/histdata.egg-info/dependency_links.txt
+-rw-r--r--   0 philipperemy   (501) wheel        (0)       24 2023-05-19 15:02:08.000000 histdata-1.1/histdata.egg-info/requires.txt
+-rw-r--r--   0 philipperemy   (501) wheel        (0)        9 2023-05-19 15:02:08.000000 histdata-1.1/histdata.egg-info/top_level.txt
+-rw-r--r--   0 philipperemy   (501) wheel        (0)       38 2023-05-19 15:02:08.806503 histdata-1.1/setup.cfg
+-rw-r--r--   0 philipperemy   (501) wheel        (0)      381 2023-05-19 15:02:04.000000 histdata-1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `histdata-1.0/histdata/api.py` & `histdata-1.1/histdata/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,32 +63,33 @@
 
 
 def download_hist_data(year='2016',
                        month=None,
                        pair='eurusd',
                        time_frame=TimeFrame.ONE_MINUTE,
                        platform=Platform.GENERIC_ASCII,
-                       output_directory='.'):
+                       output_directory='.',
+                       verbose=True):
     """
     Download 1-Minute FX data per month.
     :param year: Trading year. Format is 2016.
     :param month: Trading month. Format is 7 or 12.
     :param pair: Currency pair. Example: eurgbp.
     :param time_frame: M1 (one minute) or T (tick data)
     :param platform: MT, ASCII, XLSX, NT, MS
     :param output_directory: Where to dump the data.
     :return: ZIP Filename.
     """
 
     tick_data = time_frame.startswith('T')
     if (not tick_data) and ((int(year) >= datetime.now().year and month is None) or
                             (int(year) <= datetime.now().year - 1 and month is not None)):
-        print('For the current year, please specify month=7 for example.')
-        print('For the past years, please query per year with month=None.')
-        exit(1)
+        msg = 'For the current year, please specify month=7 for example.\n'
+        msg += 'For the past years, please query per year with month=None.'
+        raise AssertionError(msg)
 
     prefix_referer = get_prefix_referer(time_frame, platform)
     referer = get_referer(prefix_referer, pair.lower(), year, month)
 
     # Referer is the most important thing here.
     headers = {'Host': 'www.histdata.com',
                'Connection': 'keep-alive',
@@ -96,15 +97,16 @@
                'Cache-Control': 'max-age=0',
                'Origin': 'https://www.histdata.com',
                'Upgrade-Insecure-Requests': '1',
                'Content-Type': 'application/x-www-form-urlencoded',
                'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                'Referer': referer}
 
-    print(referer)
+    if verbose:
+        print(referer)
     r1 = requests.get(referer, allow_redirects=True)
     assert r1.status_code == 200, 'Make sure the website www.histdata.com is up.'
 
     soup = BeautifulSoup(r1.content, 'html.parser')
     try:
         token = soup.find('input', {'id': 'tk'}).attrs['value']
         assert len(token) > 0
@@ -119,30 +121,30 @@
             'timeframe': time_frame,
             'fxpair': pair.upper()}
     r = requests.post(url='https://www.histdata.com/get.php',
                       data=data,
                       headers=headers)
 
     assert len(r.content) > 0, 'No data could be found here.'
-    print(data)
-
+    if verbose:
+        print(data)
     if not os.path.exists(output_directory):
         os.makedirs(output_directory)
-
     if month is None:
         output_filename = 'DAT_{}_{}_{}_{}.zip'.format(platform, pair.upper(), time_frame, str(year))
     else:
         output_filename = 'DAT_{}_{}_{}_{}.zip'.format(platform, pair.upper(), time_frame,
                                                        '{}{}'.format(year, str(month).zfill(2)))
     output_filename = os.path.join(output_directory, output_filename)
     with open(output_filename, 'wb') as f:
         for chunk in r.iter_content(chunk_size=1024):
             if chunk:
                 f.write(chunk)
-    print('Wrote to {}'.format(output_filename))
+    if verbose:
+        print('Wrote to {}'.format(output_filename))
     return output_filename
 
 
 if __name__ == '__main__':
     # print(download_hist_data(year='2019', month='6', platform=Platform.NINJA_TRADER, time_frame=TimeFrame.TICK_DATA_LAST))
     # print(download_hist_data(year='2019', month='6', platform=Platform.NINJA_TRADER, time_frame=TimeFrame.TICK_DATA_ASK))
     # print(download_hist_data(year='2019', month='6', platform=Platform.NINJA_TRADER, time_frame=TimeFrame.TICK_DATA_BID))
```

