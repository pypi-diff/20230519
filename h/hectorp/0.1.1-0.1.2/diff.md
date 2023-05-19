# Comparing `tmp/hectorp-0.1.1.tar.gz` & `tmp/hectorp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hectorp-0.1.1.tar", last modified: Sun Oct 30 10:23:14 2022, max compression
+gzip compressed data, was "hectorp-0.1.2.tar", last modified: Fri May 19 14:37:27 2023, max compression
```

## Comparing `hectorp-0.1.1.tar` & `hectorp-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2022-10-30 10:23:14.439473 hectorp-0.1.1/
--rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.1/LICENSE
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2022-10-30 10:23:14.438843 hectorp-0.1.1/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     7108 2022-08-19 15:58:12.000000 hectorp-0.1.1/README.md
--rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.1/pyproject.toml
--rw-r--r--   0 msbos      (501) staff       (20)       38 2022-10-30 10:23:14.439669 hectorp-0.1.1/setup.cfg
--rw-r--r--   0 msbos      (501) staff       (20)     1752 2022-10-30 10:22:36.000000 hectorp-0.1.1/setup.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2022-10-30 10:23:14.419974 hectorp-0.1.1/src/
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2022-10-30 10:23:14.435169 hectorp-0.1.1/src/hectorp/
--rw-r--r--   0 msbos      (501) staff       (20)        0 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/__init__.py
--rw-r--r--   0 msbos      (501) staff       (20)     6765 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/ammargrag.py
--rw-r--r--   0 msbos      (501) staff       (20)    10305 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/apply_WF.py
--rw-r--r--   0 msbos      (501) staff       (20)     4453 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/ar1.py
--rw-r--r--   0 msbos      (501) staff       (20)     3316 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/calendar.py
--rw-r--r--   0 msbos      (501) staff       (20)     3888 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/control.py
--rw-r--r--   0 msbos      (501) staff       (20)     2217 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/convert_rlrdata2mom.py
--rw-r--r--   0 msbos      (501) staff       (20)     7568 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/covariance.py
--rw-r--r--   0 msbos      (501) staff       (20)     3395 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/datasnooping.py
--rw-r--r--   0 msbos      (501) staff       (20)     1817 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/date2mjd.py
--rw-r--r--   0 msbos      (501) staff       (20)    14416 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/designmatrix.py
--rw-r--r--   0 msbos      (501) staff       (20)     8101 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/estimate_all_trends.py
--rw-r--r--   0 msbos      (501) staff       (20)    12518 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/estimatespectrum.py
--rw-r--r--   0 msbos      (501) staff       (20)     5688 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/estimatetrend.py
--rw-r--r--   0 msbos      (501) staff       (20)     8135 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/findoffsets.py
--rw-r--r--   0 msbos      (501) staff       (20)     3082 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/fullcov.py
--rw-r--r--   0 msbos      (501) staff       (20)     9744 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/ggm.py
--rw-r--r--   0 msbos      (501) staff       (20)     7625 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/matern.py
--rw-r--r--   0 msbos      (501) staff       (20)     1617 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/mjd2date.py
--rw-r--r--   0 msbos      (501) staff       (20)     9677 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/mle.py
--rw-r--r--   0 msbos      (501) staff       (20)    23836 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/observations.py
--rw-r--r--   0 msbos      (501) staff       (20)     2574 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/ols.py
--rw-r--r--   0 msbos      (501) staff       (20)     4682 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/powerlaw.py
--rw-r--r--   0 msbos      (501) staff       (20)     8520 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/predicttrenderror.py
--rw-r--r--   0 msbos      (501) staff       (20)     4866 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/removeoutliers.py
--rw-r--r--   0 msbos      (501) staff       (20)    11672 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/simulatenoise.py
--rw-r--r--   0 msbos      (501) staff       (20)     2280 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/test_Schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     5265 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/varyingannual.py
--rw-r--r--   0 msbos      (501) staff       (20)     3067 2022-10-30 10:22:16.000000 hectorp-0.1.1/src/hectorp/white.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2022-10-30 10:23:14.438152 hectorp-0.1.1/src/hectorp.egg-info/
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     1002 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/SOURCES.txt
--rw-r--r--   0 msbos      (501) staff       (20)        1 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/dependency_links.txt
--rw-r--r--   0 msbos      (501) staff       (20)      536 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/entry_points.txt
--rw-r--r--   0 msbos      (501) staff       (20)       37 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/requires.txt
--rw-r--r--   0 msbos      (501) staff       (20)        8 2022-10-30 10:23:14.000000 hectorp-0.1.1/src/hectorp.egg-info/top_level.txt
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.106983 hectorp-0.1.2/
+-rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.2/LICENSE
+-rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-05-19 14:37:27.106540 hectorp-0.1.2/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     7108 2022-08-19 15:58:12.000000 hectorp-0.1.2/README.md
+-rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.2/pyproject.toml
+-rw-r--r--   0 msbos      (501) staff       (20)       38 2023-05-19 14:37:27.107083 hectorp-0.1.2/setup.cfg
+-rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-05-19 14:08:48.000000 hectorp-0.1.2/setup.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.081387 hectorp-0.1.2/src/
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.103229 hectorp-0.1.2/src/hectorp/
+-rw-r--r--   0 msbos      (501) staff       (20)        0 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/__init__.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ammargrag.py
+-rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/apply_WF.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ar1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/control.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/convert_rlrdata2mom.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/covariance.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/datasnooping.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/date2mjd.py
+-rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/designmatrix.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimate_all_trends.py
+-rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimatespectrum.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5688 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimatetrend.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8135 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/findoffsets.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/fullcov.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ggm.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/levinson.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/matern.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mjd2date.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mle.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4118 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/msf.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3459 2023-05-19 14:35:34.000000 hectorp-0.1.2/src/hectorp/msfdump.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3533 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/msfgen.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mycalendar.py
+-rw-r--r--   0 msbos      (501) staff       (20)    16575 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/observations.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ols.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/powerlaw.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/predicttrenderror.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/pyfftw_ex1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/removeoutliers.py
+-rw-r--r--   0 msbos      (501) staff       (20)       55 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/run_schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)    11672 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/simulatenoise.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_Schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_opencl.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_reikna.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/varyingannual.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/white.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.106031 hectorp-0.1.2/src/hectorp.egg-info/
+-rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/SOURCES.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        1 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/dependency_links.txt
+-rw-r--r--   0 msbos      (501) staff       (20)      596 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/entry_points.txt
+-rw-r--r--   0 msbos      (501) staff       (20)       37 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/requires.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        8 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/top_level.txt
```

### Comparing `hectorp-0.1.1/LICENSE` & `hectorp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/PKG-INFO` & `hectorp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hectorp-0.1.1/README.md` & `hectorp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/setup.py` & `hectorp-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hectorp",
-    version="0.1.1",
+    version="0.1.2",
     author="Machiel Bos",
     author_email="machielbos@protonmail.com",
     description="A collection of programs to analyse geodetic time series",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/machielsimonbos/hectorp",
     project_urls={
@@ -24,15 +24,15 @@
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
         'pandas',
         'numpy',
         'matplotlib',
         'scipy',
-        'mpmath'
+        'mpmath',
     ],
     entry_points ={ 
         'console_scripts': [ 
             'estimatespectrum = hectorp.estimatespectrum:main',
             'modelspectrum = hectorp.modelspectrum:main',
             'estimatetrend = hectorp.estimatetrend:main',
             'estimate_all_trends = hectorp.estimate_all_trends:main',
@@ -40,10 +40,12 @@
             'findoffsets = hectorp.findoffsets:main',
             'simulatenoise = hectorp.simulatenoise:main',
             'mjd2date = hectorp.mjd2date:main',
             'date2mjd = hectorp.date2mjd:main',
             'convert_rlrdata2mom = hectorp.convert_rlrdata2mom:main',
             'predict_error = hectorp.predict_error:main',
             'test_Schur = hectorp.test_Schur:main',
+            'msfgen= hectorp.msfgen:main',
+            'msfdump= hectorp.msfdump:main',
         ],
     }
 )
```

### Comparing `hectorp-0.1.1/src/hectorp/ammargrag.py` & `hectorp-0.1.2/src/hectorp/ammargrag.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # for Toeplitz Systems", By Michael K. Ng  (page 28-29)
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY 
@@ -71,14 +71,17 @@
         Returns:
             theta (n*1 matrix)    : estimated parameters
             C_theta  (n*n matrix) : covariance matrix of estimated parameters
             ln_det_C (float)      : log(det(C))
             sigma_eta (float)     : driving noise
         """
 
+        #--- Start the clock!
+        start0 = time.time()
+
         if samenoise==False:
             #--- Get size of matrix H
             (m,n) = H.shape
 
             #--- Get size of matrix F which number of columns=count missing data
             (m,k) = F.shape
 
@@ -105,14 +108,16 @@
             l1[1:m] = r[m-2::-1]
             l2[1:m] = r[0:m-1]
 
             #-- Scale l1 & l2
             l1 *= 1.0/math.sqrt(delta)
             l2 *= 1.0/math.sqrt(delta)
 
+            start1 = time.time()
+            print("step 1: {0:8.3f} s\n".format(float(time.time() - start0)))
             #--- Perform FFT on l1 and l2
             self.Fl1 = np.fft.rfft(l1)
             self.Fl2 = np.fft.rfft(l2) 
 
             #--- Currently there might be NaN's in H and x. Make those zero
             xm = np.zeros(m)
             for i in range(0,m):
@@ -190,8 +195,12 @@
             theta = C_theta @ (A1 @ self.y1.T - A2 @ self.y2.T) 
 
             #--- Compute sigma_eta
             t1 = self.y1 - A1.T @ theta
             t2 = self.y2 - A2.T @ theta
             sigma_eta = math.sqrt((np.dot(t1,t1) - np.dot(t2,t2))/m)
 
+        #--- Total time in AmmarGrag
+        print("step 2: {0:8.3f} s\n".format(float(time.time() - start1)))
+        print("--- {0:8.3f} s ---\n".format(float(time.time() - start0)))
+
         return [theta,C_theta,self.ln_det_C,sigma_eta]
```

### Comparing `hectorp-0.1.1/src/hectorp/apply_WF.py` & `hectorp-0.1.2/src/hectorp/apply_WF.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/src/hectorp/ar1.py` & `hectorp-0.1.2/src/hectorp/ar1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/src/hectorp/calendar.py` & `hectorp-0.1.2/src/hectorp/mycalendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of HectorP 0.1.1
+# This file is part of HectorP 0.1.2
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/control.py` & `hectorp-0.1.2/src/hectorp/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # control.py
 #
-# This file is part of HectorP 0.1.1
+# This file is part of HectorP 0.1.2
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/convert_rlrdata2mom.py` & `hectorp-0.1.2/src/hectorp/convert_rlrdata2mom.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/src/hectorp/covariance.py` & `hectorp-0.1.2/src/hectorp/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  1) power-law noise using Eq. (7) of Bos et al. (2008).
 #  2) white noise
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/datasnooping.py` & `hectorp-0.1.2/src/hectorp/datasnooping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # datasnooping.py
 #
 # Class which computes residuals and removes outliers
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/date2mjd.py` & `hectorp-0.1.2/src/hectorp/date2mjd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This small program computes the Modified Julian Date (MJD).
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.1/src/hectorp/designmatrix.py` & `hectorp-0.1.2/src/hectorp/designmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # designmatrix.py
 #
 # Create design matrix
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/estimate_all_trends.py` & `hectorp-0.1.2/src/hectorp/estimate_all_trends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program find all files in ./obs_files and estimate all trends.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -153,15 +153,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n*******************************************")
-    print("    estimate_all_trends, version 0.1.1")
+    print("    estimate_all_trends, version 0.1.2")
     print("*******************************************\n")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Estimate all trends')
 
     #--- List arguments that can be given 
     parser.add_argument('-n', dest='noisemodels', action='store',default='PLWN',
```

### Comparing `hectorp-0.1.1/src/hectorp/estimatespectrum.py` & `hectorp-0.1.2/src/hectorp/estimatespectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the Welch method of scipy to compute the power spectral 
 # density (one-sided).
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -185,15 +185,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatespectrum, version 0.1.1")
+        print("    estimatespectrum, version 0.1.2")
         print("***************************************")
 
     #--- Get Classes
     observations = Observations()
 
     #--- Sampling frequency (change daily period into number of seconds)
     DeltaT = observations.sampling_period
```

### Comparing `hectorp-0.1.1/src/hectorp/estimatetrend.py` & `hectorp-0.1.2/src/hectorp/estimatetrend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program estimates a trend from the observations.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -67,15 +67,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatetrend, version 0.1.1")
+        print("    estimatetrend, version 0.1.2")
         print("***************************************")
 
    
     #--- Get basename of filename
     datafile = control.params['DataFile']
     unit = control.params['PhysicalUnit']
     try:
```

### Comparing `hectorp-0.1.1/src/hectorp/findoffsets.py` & `hectorp-0.1.2/src/hectorp/findoffsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Perform cycles of offset detection for a single station [optionally 3D]
 #  1) Compute noise and SLT model parameters
 #  2) Compute for each epoch the new log-likelihood when an offset is added
 #     but maintaining the noise parameters constant.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -86,15 +86,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    findoffsets, version 0.1.1")
+    print("    findoffsets, version 0.1.2")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Find offsets in time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-s', dest='station', action='store', required=True,
```

### Comparing `hectorp-0.1.1/src/hectorp/fullcov.py` & `hectorp-0.1.2/src/hectorp/fullcov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fullcov.py
 # 
 # Python3 implemenation of FullCov.cpp. 
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/ggm.py` & `hectorp-0.1.2/src/hectorp/ggm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ggm.py
 #
 # Create the first row of the covariance matrix for Generalised Gauss Markov
 # noise.
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/matern.py` & `hectorp-0.1.2/src/hectorp/matern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # This class implements the Matérn noise model. Eqs. are taken from
 # Lilly et al. (2017) "Fractional Brownian motion, the Matérn process, and 
 # stochastic modeling of turbulent dispersion", Nonlinear Processes in 
 # Geophysics, 24: 481-514 
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/mjd2date.py` & `hectorp-0.1.2/src/hectorp/mjd2date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # Simple MJD to date converter.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.1/src/hectorp/mle.py` & `hectorp-0.1.2/src/hectorp/mle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mle.py
 #
 # Class which computes the log-likelihood and searches for the maximum value.
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/observations.py` & `hectorp-0.1.2/src/hectorp/observations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # observations.py
 #
 # A simple interface that reads and writes mom-files and stores
 # them into a Python class 'observations'.
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY 
@@ -28,14 +28,15 @@
 import numpy as np
 import os
 import sys
 import math
 import re
 from hectorp.control import Control
 from hectorp.control import SingletonMeta
+from hectorp.msf import MSF
 from pathlib import Path
 
 #==============================================================================
 # Class definition
 #==============================================================================
 
 class Observations(metaclass=SingletonMeta):
@@ -84,14 +85,17 @@
         self.ssetanh = []
         self.sampling_period = 0.0
         self.F = None
         self.percentage_gaps = None
         self.m = 0
         self.column_name=''
 
+        self.ZIPJSON_KEY = 'base64(zip(o))'
+
+
         #--- Read filename with observations and the directory
         try:
             self.datafile = control.params['DataFile']
             directory = Path(control.params['DataDirectory'])
             fname = str(directory / self.datafile)
         except Exception as e:
             fname = self.datafile = 'None'
@@ -109,15 +113,15 @@
             #--- Are there columns with estimated trajectory models
             try:
                 self.use_residuals = control.params['UseResiduals']
             except:
                 self.use_residuals = False
             #--- Which column
             try:
-                self.observation_column = control.params['ObservationColumn']
+                self.column_name = control.params['ColumnName']
             except Exception as e:
                 print(e)
                 sys.exit()
             if not fname=='None':
                 self.msfread(fname)
         else:
             print('Unknown format: {0:s}'.format(self.ts_format))
@@ -126,22 +130,22 @@
         #--- Inform the user
         if self.verbose==True:
             print("\nFilename                   : {0:s}".format(fname))
             print("TS_format                  : {0:s}".format(self.ts_format))
             print("ScaleFactor                : {0:f}".\
                                                     format(self.scale_factor))
             if self.ts_format == 'msf':   
-                print("Observation Column         : {0:d}".\
-                                             format(self.observation_column))
+                print("Column Name                : {0:s}".\
+                                             format(self.column_name))
                 print("Use Residuals              : {0:}".\
                                                     format(self.use_residuals))
             if not fname=='None':
                 print("Number of observations+gaps: {0:d}".format(self.m))
                 print("Percentage of gaps         : {0:5.1f}".\
-					                           format(self.percentage_gaps))
+			                           format(self.percentage_gaps))
 
 
 
     def create_dataframe_and_F(self,t,obs,mod,period):
         """ Convert np.arrays into Panda DataFrame and create matrix F
 
         Args:
@@ -246,106 +250,57 @@
 
     def msfread(self,fname):
         """Read msf-file fname and store the data into the Observation class
         
         Args:
             fname (string) : name of file that will be read
         """
-        #--- Constants
-        TINY = 1.0e-6
 
-        #--- Check if file exists
-        if os.path.isfile(fname)==False:
-            print('File {0:s} does not exist'.format(fname))
+        TINY = 1.0e-7
+        msf  = MSF()
+
+        #--- Read header and data
+        [header,data] = msf.read(fname)
+
+        #--- Extract required info from header
+        self.sampling_period = header['sampling_period']
+        column_names = header['column_names']
+        if not self.column_name in column_names:
+            print('Could not find column {0:s}'.format(self.column_name))
             sys.exit()
-        
-        #--- Read the file (header + time series)
-        t = []
-        obs = []
-        mjd0 = 0.0
-        tt_old = 0.0
-        inside_observations = False
-        inside_models = False
-        inside_offsets = False
-        self.model_column = 0
-        self.fname_in = fname
-        offset_lines = []
-        with open(fname,'r') as fp:
-            for line in fp:
-                cols = line.split()
-                if line.startswith('#')==True:
-                    if len(cols)>2:
-                        if cols[1]=='sampling' and cols[2]=='period':
-                            self.sampling_period = float(cols[3])
-                    if len(cols)>1:
-                        if cols[1]=='Observations':
-                            inside_observations = True
-                        elif cols[1]=='Models':
-                            inside_observations = False
-                            inside_models = True
-                        elif cols[1]=='Offsets':
-                            inside_models = False
-                            inside_offset = True
-
-                        #-- Does the line contain column definition?
-                        m = re.match('#\s+(\d+)\.\s+(.+)',line)
-                        if m:
-                            column = int(m.group(1))
-                            if inside_observations==True and \
-                                              column==self.observation_column:
-                                self.column_name = m.group(2)
-                            elif inside_models==True and \
-                                              m.group(2)==self.column_name:
-                                self.model_column = column
-                            elif inside_offsets==True and \
-                                              column==self.observation_column:
-                                offset_lines.append(m.group(2))
- 
-                else:
-                    #--- sanity check
-                    if self.use_residuals==True:
-                        if self.model_column==0:
-                            print('Could not find requested model column')
-                            sys.exit()
-                    if len(cols)<3:
-                        print('Found illegal row: {0:s}'.format(line))
-                        sys.exit()
-                   
-                    mjd = float(cols[0])
-                    if mjd0==0.0:
-                        mjd0 = mjd
-                    sod = float(cols[1])
-                    tt = 86400.0*(mjd-mjd0) + sod
-                    #--- Fill gaps with NaN's
-                    if tt_old>0.0:
-                        while abs(tt-tt_old-self.sampling_period)>TINY:
-                            tt_old += self.sampling_period
-                            t.append(tt_old)
-                            obs.append(np.NAN)
-                            if tt_old>tt-TINY:
-                                print('Someting is very wrong here....')
-                                print('mjd={0:f}, sod={1:f}'.format(mjd,sod))
-                                sys.exit()
-                    t.append(tt)
-                    tt_old = tt
-                    if cols[self.observation_column-1]=='NaN':
-                        obs.append(np.NAN)
-                    else:
-                        if self.use_residuals==True:
-                            y = float(cols[self.observation_column-1])-\
-                                       float(cols[self.model_column-1])
-                        else:
-                            y = float(cols[self.observation_column-1])
-                        obs.append(self.scale_factor * y)
-
-        #--- Now that we know MJD0, store offset times
-        for line in offset_lines:
-            cols = line.split()
-            tt = 86400.0*(float(cols[0]) - mjd0) + float(cols[1])
-            self.offsets.append(tt)
+        if self.use_residuals==True:
+            mod_column_name = 'mod_' + self.column_name
+            if not mod_column_name in column_names:
+                print('Could not find column {0:s}'.format(mod_column_name))
+                sys.exit()
+        all_offsets = header[offsets]
+        self.offsets = all_offsets[column_name]
+             
+        #--- Select specified column data
+        sod = data['sod']
+        if self.use_residuals==True:
+            y = data[self.column_name] - data[mod_column_name]
+        else:
+            y = data[self.column_name]
+   
+        sod_old = sod[0]
+        t = [sod[0]]
+        obs = [y[0]]
+        for i in range(1,len(sod))
+            while abs(sod[i]-sold_old-self.sampling_period)>TINY:
+                sod_old += self.sampling_period
+                t.append(sod_old)
+                obs.append(np.NAN)
+                if sod_old>tt-TINY:
+                     print('Someting is very wrong here....')
+                     print('mjd={0:f}, sod={1:f}'.format(mjd,sod))
+                     sys.exit()
+                t.append(sod[i])
+                sod_old = sod[i]
+                obs.append(self.scale_factor * y[i])
 
         #---- Create pandas DataFrame
         self.create_dataframe_and_F(t,obs,[],self.sampling_period)
         
         
         
     def momwrite(self,fname):
@@ -391,180 +346,66 @@
                 if len(self.data.columns)==2:
                     fp.write(' {0:13.6f}\n'.format(self.data.iloc[i,1]))
                 else:
                     fp.write('\n')
             
         fp.close()
         
-       
 
-    def msfwrite(self,fname):
+
+    def msfwrite(self,fname,header=={}):
         """Write the msf data to a file called fname
         
         Args:
             fname (string) : name of file that will be written
 
-        self.observation_column, self.column_name are assumed to be known
-        after msfread call. If not, then self.fname_in is also '' and a new
-        header will be created, setting these two variables
-
         """
 
-        #--- Constant
-        TINY = 1.0e-8
-
-        #--- Initial value, to be changed later
-        mjd0 = 0.0
-
-        #--- Create header from scratch
-        if self.datafile=="None":
-            self.column_name='unknown'
-            self.observation_columnn = 3
-
-            lines = []
-            lines.append('# sampling period {0:f}\n#\n'.\
-                                                format(self.sampling_period))
-            lines.append('# Observations\n# ------------\n')
-            lines.append('# 1. MJD - Modified Julian Date\n')
-            lines.append('# 2. sod - seconds of day\n')
-            lines.append('# 3. {0:s}\n#\n'.format(self.column_name))
-
-            lines.append('# Models\n# ------------\n#\n')
-
-            #--- Write offsets in header
-            mjd0 = 58849.0
-            lines.append('# Offsets\n# ------------\n')
-            for i in range(0,len(self.offsets)):
-                sod = self.offsets[i]
-                mjd = mjd0
-                while sod>86400.0:
-                    mjd += 1
-                    sod -= 86400.0
-                lines.append('# 3. {0:6.0f} {1:10.4f}\n'.format(mjd,sod))
- 
-            lines.append('#\n#=====================================' + \
-                                '==========================================\n')
-
-            #--- Add MJD, sod & observation lines
-            for i in range(0,self.m):
-                mjd = mjd0
-                sod = self.data.index[i]
-                while sod>86400.0:
-                    mjd += 1
-                    sod -= 86400.0
-                lines.append('{0:6.0f} {1:10.4f} {2:12.6f}\n'.\
-                                          format(mjd,sod,self.data.iloc[i,0]))
-
-        else:
-            with open(self.fname_in,'r') as fp:
-                lines = fp.readlines()
-
-        #--- Try to open the file for writing
-        try:
-            fp = open(fname,'w')
-        except IOError:
-           print('Error: File {0:s} cannot be opened for written.'. \
-                                                         format(fname))
-           sys.exit()
+        #--- Create instance of msf
+        msf = MSF()
 
-        if self.verbose==True:
-            print('--> {0:s}'.format(fname))
-
-        #--- Case of adding anther column 
-        inside_observations = False
-        inside_models = False
-        inside_offsets = False
-        i = 0
-
-        for line in lines:
-
-            #--- header stuff
-            if line.startswith('#'):
-                #--- If new trajectory model is estimated, add name in header
-                if len(self.data.columns)==2:
-                    if inside_observations==True:
-                        #-- Does the line contain column definition?
-                        m = re.match('# (\d+)\.\s+(.+)',line)
-                        if m:
-                            column = int(m.group(1))
-                    elif inside_models==True:
-                        #-- Does the line contain column definition?
-                        m = re.match('# (\d+)\.\s+(.+)',line)
-                        if m:
-                            column = int(m.group(1))
-                            if m.group(2)==self.column_name:
-                                self.model_column = column
-                        else:
-                            if not line.startswith('# ------------') and \
-                                                        self.model_column==0:
-                                self.model_column = column+1
-                                fp.write('# {0:d}. {1:s}\n'.format(column+1,
-                                                            self.column_name))
-                                inside_models=False
-
-                    #--- Which block are we processing?
-                    cols = line.split()
-                    if len(cols)>1:
-                        if cols[1]=='Observations':
-                            inside_observations = True
-                        if cols[1]=='Models':
-                            inside_observations = False
-                            inside_models = True
-                        elif cols[1]=='Offsets':
-                            inside_models = False
- 
-                #--- Just copy header line to new file
-                fp.write(line)
-            else:
-                #--- Get time to see if this is equal to data.index[i]
-                cols = line.split()
-                mjd = float(cols[0])
-                sod = float(cols[1])
-                if mjd0==0.0:
-                    mjd0 = mjd
-
-                tt = 86400.0*(mjd - mjd0) + sod
-                while self.data.index[i]<tt:
-                    i += 1
-                if abs(tt - self.data.index[i])>TINY:
-                    print('Expected regularly spaced data!')
-                    print('file time = {0:f}, array time = {1:f}'.\
-                                            format(tt,self.data.index[i]))
-                    sys.exit()
+        #--- Do some checking
+        mod_column_name = ''
+        if self.DataFile=='None' and header=={}:
+            print('Both DataFile in ctl-file and header are not specified!')
+            sys.exit()
+        elif not self.DataFile=='None' and not header=={}:
+            print('Both DataFile in ctl-file and header are specified!')
+            sys.exit()
+        elif not self.DataFile=='None'
+            [header,data] = msf.read(fname)
 
-                #--- Replace observation values
-                cols = line.split()
-                fp.write('{0:>6s} {1:>10s}'.format(cols[0],cols[1]))
-                for j in range(2,self.observation_column-1):
-                    fp.write('{0:>12s} '.format(cols[j]))
-                if math.isnan(self.data.iloc[i,0])==True:
-                    fp.write('{0:>12s}'.format('NaN'))
-                else:
-                    fp.write('{0:12.6f}'.format(self.data.iloc[i,0]))
+        #--- Start with new data dictionary
+        data_new = {}
+        for column_name in header['column_names']:
+            data_new[column_name] = []
+
+        #--- Do we need to add another column?
+        if len(self.data.columns)==2:
+            mod_column_name = 'mod_' + self.column_name
+            if not mod_column_name in header['column_names']:
+                header['column_names'].append(mod_column_name)
+                data_new[mod_column_name] = []                
+        
 
-                if len(self.data.columns)==2:
-                    #--- Replace Model values
-                    for j in range(self.observation_column,\
-                                                         self.model_column-1):
-                        fp.write(' {0:>12s}'.format(cols[j]))
-                    if math.isnan(self.data.iloc[i,0])==True:
-                        fp.write('{0:>12s}'.format('NaN'))
+        #--- Add sod & observations
+        for i in range(0,self.m):
+            y = self.data.iloc[i,0]
+            if not np.isnan(y):
+                for j in range(0,len(header['column_names'])):
+                    cname = header['column_names'][j]
+                    if cname == self.column_name:
+                        data_new[cname].append(y)
+                    elif cname == mod_column_name:
+                        data_new[cname].append(self.data.iloc[i,1])
                     else:
-                        fp.write('{0:12.6f}'.format(self.data.iloc[i,1]))
-                    for j in range(self.model_column,len(cols)):
-                        fp.write(' {0:>12s}'.format(cols[j]))
-                else:
-                    for j in range(self.observation_column,len(cols)):
-                        fp.write(' {0:>12s}'.format(cols[j]))
-                fp.write('\n')
-                
-                #--- Go to next item in array
-                i += 1
+                        data_new[cname].append(data[cname])
 
-        fp.close()
+        #--- Finally, write header + data_new to file
+        msf.write(fname,header,data_new)
 
 
 
     def show_results(self,output):
         """ add info to json-ouput dict
         """
```

### Comparing `hectorp-0.1.1/src/hectorp/ols.py` & `hectorp-0.1.2/src/hectorp/ols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ols.py
 # 
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/powerlaw.py` & `hectorp-0.1.2/src/hectorp/powerlaw.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Create the first row of the covariance matrix for power-law noise models
 # using Eq. (7) of Bos et al. (2008).
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
-# This file is part of HectorP 0.1.1.
+# This file is part of HectorP 0.1.2.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.1/src/hectorp/predicttrenderror.py` & `hectorp-0.1.2/src/hectorp/predicttrenderror.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the estimated noise models parameters to predict the 
 # trend error for given number of observations.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -113,15 +113,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    predict error, version 0.1.1")
+        print("    predict error, version 0.1.2")
         print("***************************************")
 
     #--- Get Classes
     white = White()
     powerlaw = Powerlaw()
     ggm = GGM()
     varyingannual = VaryingAnnual()
```

### Comparing `hectorp-0.1.1/src/hectorp/removeoutliers.py` & `hectorp-0.1.2/src/hectorp/removeoutliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program removes outliers from the observations.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -71,15 +71,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    removeoutliers, version 0.1.1")
+        print("    removeoutliers, version 0.1.2")
         print("***************************************")
 
     #--- Get Classes
     datasnooping = DataSnooping()
     observations = Observations()
 
     #--- Get data
```

### Comparing `hectorp-0.1.1/src/hectorp/simulatenoise.py` & `hectorp-0.1.2/src/hectorp/simulatenoise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program creates synthetic noise.
 #
-#  This script is part of HectorP 0.1.1
+#  This script is part of HectorP 0.1.2
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -242,15 +242,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    simulatenoise, version 0.1.1")
+    print("    simulatenoise, version 0.1.2")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Simulate noise time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-i', required=False, default='simulatenoise.ctl', \
```

### Comparing `hectorp-0.1.1/src/hectorp/varyingannual.py` & `hectorp-0.1.2/src/hectorp/varyingannual.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/src/hectorp/white.py` & `hectorp-0.1.2/src/hectorp/white.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.1/src/hectorp.egg-info/PKG-INFO` & `hectorp-0.1.2/src/hectorp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hectorp-0.1.1/src/hectorp.egg-info/SOURCES.txt` & `hectorp-0.1.2/src/hectorp.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,46 @@
 README.md
 pyproject.toml
 setup.py
 src/hectorp/__init__.py
 src/hectorp/ammargrag.py
 src/hectorp/apply_WF.py
 src/hectorp/ar1.py
-src/hectorp/calendar.py
 src/hectorp/control.py
 src/hectorp/convert_rlrdata2mom.py
 src/hectorp/covariance.py
 src/hectorp/datasnooping.py
 src/hectorp/date2mjd.py
 src/hectorp/designmatrix.py
 src/hectorp/estimate_all_trends.py
 src/hectorp/estimatespectrum.py
 src/hectorp/estimatetrend.py
 src/hectorp/findoffsets.py
 src/hectorp/fullcov.py
 src/hectorp/ggm.py
+src/hectorp/levinson.py
 src/hectorp/matern.py
 src/hectorp/mjd2date.py
 src/hectorp/mle.py
+src/hectorp/msf.py
+src/hectorp/msfdump.py
+src/hectorp/msfgen.py
+src/hectorp/mycalendar.py
 src/hectorp/observations.py
 src/hectorp/ols.py
 src/hectorp/powerlaw.py
 src/hectorp/predicttrenderror.py
+src/hectorp/pyfftw_ex1.py
 src/hectorp/removeoutliers.py
+src/hectorp/run_schur.py
+src/hectorp/schur.py
 src/hectorp/simulatenoise.py
 src/hectorp/test_Schur.py
+src/hectorp/test_opencl.py
+src/hectorp/test_reikna.py
 src/hectorp/varyingannual.py
 src/hectorp/white.py
 src/hectorp.egg-info/PKG-INFO
 src/hectorp.egg-info/SOURCES.txt
 src/hectorp.egg-info/dependency_links.txt
 src/hectorp.egg-info/entry_points.txt
 src/hectorp.egg-info/requires.txt
```

### Comparing `hectorp-0.1.1/src/hectorp.egg-info/entry_points.txt` & `hectorp-0.1.2/src/hectorp.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,11 +3,13 @@
 date2mjd = hectorp.date2mjd:main
 estimate_all_trends = hectorp.estimate_all_trends:main
 estimatespectrum = hectorp.estimatespectrum:main
 estimatetrend = hectorp.estimatetrend:main
 findoffsets = hectorp.findoffsets:main
 mjd2date = hectorp.mjd2date:main
 modelspectrum = hectorp.modelspectrum:main
+msfdump = hectorp.msfdump:main
+msfgen = hectorp.msfgen:main
 predict_error = hectorp.predict_error:main
 removeoutliers = hectorp.removeoutliers:main
 simulatenoise = hectorp.simulatenoise:main
 test_Schur = hectorp.test_Schur:main
```

