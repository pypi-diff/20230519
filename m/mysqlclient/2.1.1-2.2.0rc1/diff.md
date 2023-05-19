# Comparing `tmp/mysqlclient-2.1.1.tar.gz` & `tmp/mysqlclient-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlclient-2.1.1.tar", last modified: Wed Jun 22 07:46:25 2022, max compression
+gzip compressed data, was "mysqlclient-2.2.0rc1.tar", last modified: Fri May 19 04:58:30 2023, max compression
```

## Comparing `mysqlclient-2.1.1.tar` & `mysqlclient-2.2.0rc1.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.635090 mysqlclient-2.1.1/
--rw-r--r--   0 inada-n    (502) staff       (20)    15327 2022-06-22 01:21:39.000000 mysqlclient-2.1.1/HISTORY.rst
--rw-r--r--   0 inada-n    (502) staff       (20)    18092 2010-03-23 23:34:05.000000 mysqlclient-2.1.1/LICENSE
--rw-r--r--   0 inada-n    (502) staff       (20)      261 2021-01-08 06:39:10.000000 mysqlclient-2.1.1/MANIFEST.in
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.617027 mysqlclient-2.1.1/MySQLdb/
--rw-r--r--   0 inada-n    (502) staff       (20)     3448 2021-10-19 04:21:25.000000 mysqlclient-2.1.1/MySQLdb/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2472 2022-06-21 11:30:19.000000 mysqlclient-2.1.1/MySQLdb/_exceptions.py
--rw-r--r--   0 inada-n    (502) staff       (20)    79808 2022-06-21 11:30:23.000000 mysqlclient-2.1.1/MySQLdb/_mysql.c
--rw-r--r--   0 inada-n    (502) staff       (20)    11360 2021-10-20 04:25:54.000000 mysqlclient-2.1.1/MySQLdb/connections.py
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.621179 mysqlclient-2.1.1/MySQLdb/constants/
--rw-r--r--   0 inada-n    (502) staff       (20)      666 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/MySQLdb/constants/CLIENT.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2828 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/MySQLdb/constants/CR.py
--rw-r--r--   0 inada-n    (502) staff       (20)    24888 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/MySQLdb/constants/ER.py
--rw-r--r--   0 inada-n    (502) staff       (20)      566 2018-12-13 01:23:28.000000 mysqlclient-2.1.1/MySQLdb/constants/FIELD_TYPE.py
--rw-r--r--   0 inada-n    (502) staff       (20)      363 2015-10-11 07:34:59.000000 mysqlclient-2.1.1/MySQLdb/constants/FLAG.py
--rw-r--r--   0 inada-n    (502) staff       (20)       55 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/MySQLdb/constants/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3444 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/MySQLdb/converters.py
--rw-r--r--   0 inada-n    (502) staff       (20)    15511 2022-06-21 11:30:19.000000 mysqlclient-2.1.1/MySQLdb/cursors.py
--rw-r--r--   0 inada-n    (502) staff       (20)      108 2022-06-22 07:46:24.000000 mysqlclient-2.1.1/MySQLdb/release.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3604 2020-12-04 03:22:51.000000 mysqlclient-2.1.1/MySQLdb/times.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4365 2022-06-22 07:46:25.634787 mysqlclient-2.1.1/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)     3124 2021-10-19 03:45:22.000000 mysqlclient-2.1.1/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.625609 mysqlclient-2.1.1/doc/
--rw-r--r--   0 inada-n    (502) staff       (20)     4937 2018-12-10 09:24:35.000000 mysqlclient-2.1.1/doc/FAQ.rst
--rw-r--r--   0 inada-n    (502) staff       (20)      871 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/doc/MySQLdb.constants.rst
--rw-r--r--   0 inada-n    (502) staff       (20)     1077 2019-12-01 03:04:26.000000 mysqlclient-2.1.1/doc/MySQLdb.rst
--rw-r--r--   0 inada-n    (502) staff       (20)     7882 2020-12-07 07:28:55.000000 mysqlclient-2.1.1/doc/conf.py
--rw-r--r--   0 inada-n    (502) staff       (20)      243 2015-12-13 14:19:20.000000 mysqlclient-2.1.1/doc/index.rst
--rw-r--r--   0 inada-n    (502) staff       (20)    29016 2022-06-21 11:30:19.000000 mysqlclient-2.1.1/doc/user_guide.rst
--rw-r--r--   0 inada-n    (502) staff       (20)     1418 2022-06-22 01:21:47.000000 mysqlclient-2.1.1/metadata.cfg
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.627966 mysqlclient-2.1.1/mysqlclient.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)     4365 2022-06-22 07:46:25.000000 mysqlclient-2.1.1/mysqlclient.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      934 2022-06-22 07:46:25.000000 mysqlclient-2.1.1/mysqlclient.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2022-06-22 07:46:25.000000 mysqlclient-2.1.1/mysqlclient.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        8 2022-06-22 07:46:25.000000 mysqlclient-2.1.1/mysqlclient.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2022-06-22 07:46:25.635163 mysqlclient-2.1.1/setup.cfg
--rw-r--r--   0 inada-n    (502) staff       (20)      563 2020-07-03 02:22:24.000000 mysqlclient-2.1.1/setup.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1037 2021-10-19 08:02:41.000000 mysqlclient-2.1.1/setup_common.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4817 2021-05-31 05:27:01.000000 mysqlclient-2.1.1/setup_posix.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1577 2021-10-19 03:45:22.000000 mysqlclient-2.1.1/setup_windows.py
--rw-r--r--   0 inada-n    (502) staff       (20)      450 2021-10-19 03:45:22.000000 mysqlclient-2.1.1/site.cfg
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2022-06-22 07:46:25.634243 mysqlclient-2.1.1/tests/
--rw-r--r--   0 inada-n    (502) staff       (20)    10030 2020-12-04 03:22:51.000000 mysqlclient-2.1.1/tests/capabilities.py
--rw-r--r--   0 inada-n    (502) staff       (20)      577 2020-12-04 03:22:51.000000 mysqlclient-2.1.1/tests/configdb.py
--rw-r--r--   0 inada-n    (502) staff       (20)    31524 2022-06-21 11:30:19.000000 mysqlclient-2.1.1/tests/dbapi20.py
--rw-r--r--   0 inada-n    (502) staff       (20)     6278 2021-10-19 03:45:22.000000 mysqlclient-2.1.1/tests/test_MySQLdb_capabilities.py
--rw-r--r--   0 inada-n    (502) staff       (20)     8096 2020-12-04 03:22:51.000000 mysqlclient-2.1.1/tests/test_MySQLdb_dbapi20.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3421 2020-07-02 03:56:48.000000 mysqlclient-2.1.1/tests/test_MySQLdb_nonstandard.py
--rw-r--r--   0 inada-n    (502) staff       (20)     5960 2021-01-08 07:30:30.000000 mysqlclient-2.1.1/tests/test_MySQLdb_times.py
--rw-r--r--   0 inada-n    (502) staff       (20)      132 2018-12-10 09:24:35.000000 mysqlclient-2.1.1/tests/test__mysql.py
--rw-r--r--   0 inada-n    (502) staff       (20)      605 2021-09-03 02:05:17.000000 mysqlclient-2.1.1/tests/test_connection.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4538 2020-12-08 09:36:05.000000 mysqlclient-2.1.1/tests/test_cursor.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.366335 mysqlclient-2.2.0rc1/
+-rw-r--r--   0 inada-n    (502) staff       (20)    15952 2023-05-19 04:35:28.000000 mysqlclient-2.2.0rc1/HISTORY.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)    18092 2010-03-23 23:34:05.000000 mysqlclient-2.2.0rc1/LICENSE
+-rw-r--r--   0 inada-n    (502) staff       (20)      148 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/MANIFEST.in
+-rw-r--r--   0 inada-n    (502) staff       (20)     4393 2023-05-19 04:58:30.366198 mysqlclient-2.2.0rc1/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)     3093 2023-05-18 12:51:09.000000 mysqlclient-2.2.0rc1/README.md
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.360628 mysqlclient-2.2.0rc1/doc/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4937 2018-12-10 09:24:35.000000 mysqlclient-2.2.0rc1/doc/FAQ.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)      871 2020-07-02 03:56:48.000000 mysqlclient-2.2.0rc1/doc/MySQLdb.constants.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     1051 2023-05-17 01:59:25.000000 mysqlclient-2.2.0rc1/doc/MySQLdb.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     8014 2023-05-17 01:59:25.000000 mysqlclient-2.2.0rc1/doc/conf.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      243 2015-12-13 14:19:20.000000 mysqlclient-2.2.0rc1/doc/index.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)    29657 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/doc/user_guide.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     1551 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/pyproject.toml
+-rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-05-19 04:58:30.366380 mysqlclient-2.2.0rc1/setup.cfg
+-rw-r--r--   0 inada-n    (502) staff       (20)     4456 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/setup.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      275 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/site.cfg
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.357443 mysqlclient-2.2.0rc1/src/
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.362454 mysqlclient-2.2.0rc1/src/MySQLdb/
+-rw-r--r--   0 inada-n    (502) staff       (20)     3393 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2472 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/_exceptions.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    82709 2023-05-19 03:57:37.000000 mysqlclient-2.2.0rc1/src/MySQLdb/_mysql.c
+-rw-r--r--   0 inada-n    (502) staff       (20)    11651 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/connections.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.363295 mysqlclient-2.2.0rc1/src/MySQLdb/constants/
+-rw-r--r--   0 inada-n    (502) staff       (20)      666 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/CLIENT.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2818 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/CR.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    24878 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/ER.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      566 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/FIELD_TYPE.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      363 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/FLAG.py
+-rw-r--r--   0 inada-n    (502) staff       (20)       55 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3452 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/converters.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    15838 2023-05-18 17:06:53.000000 mysqlclient-2.2.0rc1/src/MySQLdb/cursors.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      112 2023-05-19 04:35:28.000000 mysqlclient-2.2.0rc1/src/MySQLdb/release.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3604 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/times.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.363750 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4393 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)      981 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/top_level.txt
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.365881 mysqlclient-2.2.0rc1/tests/
+-rw-r--r--   0 inada-n    (502) staff       (20)    10047 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/capabilities.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      577 2020-12-04 03:22:51.000000 mysqlclient-2.2.0rc1/tests/configdb.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    31502 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/dbapi20.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     6277 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_capabilities.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     8096 2020-12-04 03:22:51.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     4272 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     5960 2021-01-08 07:30:30.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_times.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      132 2018-12-10 09:24:35.000000 mysqlclient-2.2.0rc1/tests/test__mysql.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      605 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_connection.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     7107 2023-05-18 08:59:02.000000 mysqlclient-2.2.0rc1/tests/test_cursor.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1382 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_errors.py
```

### Comparing `mysqlclient-2.1.1/HISTORY.rst` & `mysqlclient-2.2.0rc1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,27 @@
 ======================
+ What's new in 2.2.0
+======================
+
+Release: TBD
+
+* Use ``pkg-config`` instead of ``mysql_config`` (#586)
+* Raise ProgrammingError on -inf (#557)
+* Raise IntegrityError for ER_BAD_NULL. (#579)
+* Windows: Use MariaDB Connector/C 3.3.4 (#585)
+* Use pkg-config instead of mysql_config (#586)
+* Add collation option (#564)
+* Drop Python 3.7 support (#593)
+* Use pyproject.toml for build (#598)
+* Add Cursor.mogrify (#477)
+* Partial support of ssl_mode option with mariadbclient (#475)
+* Discard remaining results without creating Python objects (#601)
+* Fix executemany with binary prefix (#605)
+
+======================
  What's new in 2.1.1
 ======================
 
 Release: 2022-06-22
 
 * Fix qualname of exception classes. (#522)
 * Fix range check in ``MySQLdb._mysql.result.fetch_row()``. Invalid ``how`` argument caused SEGV. (#538)
```

### Comparing `mysqlclient-2.1.1/LICENSE` & `mysqlclient-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/MySQLdb/__init__.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 See the C API specification and the MySQL documentation for more info
 on other items.
 
 For information on how MySQLdb handles type conversion, see the
 MySQLdb.converters module.
 """
 
-try:
-    from MySQLdb.release import version_info
-    from . import _mysql
+from .release import version_info
+from . import _mysql
 
-    assert version_info == _mysql.version_info
-except Exception:
+if version_info != _mysql.version_info:
     raise ImportError(
-        "this is MySQLdb version {}, but _mysql is version {!r}\n_mysql: {!r}".format(
-            version_info, _mysql.version_info, _mysql.__file__
-        )
+        f"this is MySQLdb version {version_info}, "
+        f"but _mysql is version {_mysql.version_info!r}\n"
+        f"_mysql: {_mysql.__file__!r}"
     )
 
 
 from ._mysql import (
     NotSupportedError,
     OperationalError,
     get_client_info,
```

### Comparing `mysqlclient-2.1.1/MySQLdb/_exceptions.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/MySQLdb/_mysql.c` & `mysqlclient-2.2.0rc1/src/MySQLdb/_mysql.c`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 #endif
 #ifdef ER_CANNOT_ADD_FOREIGN
     case ER_CANNOT_ADD_FOREIGN:
 #endif
 #ifdef ER_NO_DEFAULT_FOR_FIELD
     case ER_NO_DEFAULT_FOR_FIELD:
 #endif
+    case ER_BAD_NULL_ERROR:
         e = _mysql_IntegrityError;
         break;
 #ifdef ER_WARNING_NOT_COMPLETE_ROLLBACK
     case ER_WARNING_NOT_COMPLETE_ROLLBACK:
 #endif
 #ifdef ER_NOT_SUPPORTED_YET
     case ER_NOT_SUPPORTED_YET:
@@ -375,30 +376,36 @@
 static int _mysql_ResultObject_clear(_mysql_ResultObject *self)
 {
     Py_CLEAR(self->converter);
     Py_CLEAR(self->conn);
     return 0;
 }
 
-#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
+enum {
+    SSLMODE_DISABLED = 1,
+    SSLMODE_PREFERRED = 2,
+    SSLMODE_REQUIRED = 3,
+    SSLMODE_VERIFY_CA = 4,
+    SSLMODE_VERIFY_IDENTITY = 5
+};
+
 static int
 _get_ssl_mode_num(char *ssl_mode)
 {
     static char *ssl_mode_list[] = { "DISABLED", "PREFERRED",
                   "REQUIRED", "VERIFY_CA", "VERIFY_IDENTITY" };
     unsigned int i;
     for (i=0; i < sizeof(ssl_mode_list)/sizeof(ssl_mode_list[0]); i++) {
         if (strcmp(ssl_mode, ssl_mode_list[i]) == 0) {
             // SSL_MODE one-based
             return i + 1;
         }
     }
     return -1;
 }
-#endif
 
 static int
 _mysql_ConnectionObject_Initialize(
     _mysql_ConnectionObject *self,
     PyObject *args,
     PyObject *kwargs)
 {
@@ -424,14 +431,15 @@
                   "read_timeout", "write_timeout", "charset",
                   "auth_plugin",
                   NULL } ;
     int connect_timeout = 0;
     int read_timeout = 0;
     int write_timeout = 0;
     int compress = -1, named_pipe = -1, local_infile = -1;
+    int ssl_mode_num = SSLMODE_DISABLED;
     char *init_command=NULL,
          *read_default_file=NULL,
          *read_default_group=NULL,
          *charset=NULL,
          *auth_plugin=NULL;
 
     self->converter = NULL;
@@ -464,32 +472,27 @@
         _stringsuck(ca, value, ssl);
         _stringsuck(capath, value, ssl);
         _stringsuck(cert, value, ssl);
         _stringsuck(key, value, ssl);
         _stringsuck(cipher, value, ssl);
     }
     if (ssl_mode) {
-#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
-        if (_get_ssl_mode_num(ssl_mode) <= 0) {
+        if ((ssl_mode_num = _get_ssl_mode_num(ssl_mode)) <= 0) {
             PyErr_SetString(_mysql_NotSupportedError, "Unknown ssl_mode specification");
             return -1;
         }
-#else
-        PyErr_SetString(_mysql_NotSupportedError, "MySQL client library does not support ssl_mode specification");
-        return -1;
-#endif
     }
 
     conn = mysql_init(&(self->connection));
     if (!conn) {
         PyErr_SetNone(PyExc_MemoryError);
         return -1;
     }
-    Py_BEGIN_ALLOW_THREADS ;
     self->open = 1;
+
     if (connect_timeout) {
         unsigned int timeout = connect_timeout;
         mysql_options(&(self->connection), MYSQL_OPT_CONNECT_TIMEOUT,
                 (char *)&timeout);
     }
     if (read_timeout) {
         unsigned int timeout = read_timeout;
@@ -516,31 +519,43 @@
 
     if (local_infile != -1)
         mysql_options(&(self->connection), MYSQL_OPT_LOCAL_INFILE, (char *) &local_infile);
 
     if (ssl) {
         mysql_ssl_set(&(self->connection), key, cert, ca, capath, cipher);
     }
-#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
     if (ssl_mode) {
-        int ssl_mode_num = _get_ssl_mode_num(ssl_mode);
+#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
         mysql_options(&(self->connection), MYSQL_OPT_SSL_MODE, &ssl_mode_num);
-    }
+#else
+        // MariaDB doesn't support MYSQL_OPT_SSL_MODE.
+        // See https://github.com/PyMySQL/mysqlclient/issues/474
+        // TODO: Does MariaDB supports PREFERRED and VERIFY_CA?
+        // We support only two levels for now.
+        my_bool enforce_tls = 1;
+        if (ssl_mode_num >= SSLMODE_REQUIRED) {
+            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_ENFORCE, (void *)&enforce_tls);
+        }
+        if (ssl_mode_num >= SSLMODE_VERIFY_CA) {
+            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_VERIFY_SERVER_CERT, (void *)&enforce_tls);
+        }
 #endif
+    }
+
     if (charset) {
         mysql_options(&(self->connection), MYSQL_SET_CHARSET_NAME, charset);
     }
     if (auth_plugin) {
         mysql_options(&(self->connection), MYSQL_DEFAULT_AUTH, auth_plugin);
     }
 
+    Py_BEGIN_ALLOW_THREADS
     conn = mysql_real_connect(&(self->connection), host, user, passwd, db,
                   port, unix_socket, client_flag);
-
-    Py_END_ALLOW_THREADS ;
+    Py_END_ALLOW_THREADS
 
     if (ssl) {
         int i;
         for (i=0; i<n_ssl_keepref; i++) {
             Py_DECREF(ssl_keepref[i]);
             ssl_keepref[i] = NULL;
         }
@@ -925,15 +940,15 @@
 static PyObject *
 _mysql_escape_string(
     _mysql_ConnectionObject *self,
     PyObject *args)
 {
     PyObject *str;
     char *in, *out;
-    int len;
+    unsigned long len;
     Py_ssize_t size;
     if (!PyArg_ParseTuple(args, "s#:escape_string", &in, &size)) return NULL;
     str = PyBytes_FromStringAndSize((char *) NULL, size*2+1);
     if (!str) return PyErr_NoMemory();
     out = PyBytes_AS_STRING(str);
 
     if (self && PyModule_Check((PyObject*)self))
@@ -962,56 +977,77 @@
 _mysql.string_literal(obj) cannot handle character sets.";
 
 static PyObject *
 _mysql_string_literal(
     _mysql_ConnectionObject *self,
     PyObject *o)
 {
-    PyObject *str, *s;
-    char *in, *out;
-    unsigned long len;
-    Py_ssize_t size;
+    PyObject *s; // input string or bytes. need to decref.
 
     if (self && PyModule_Check((PyObject*)self))
         self = NULL;
 
     if (PyBytes_Check(o)) {
         s = o;
         Py_INCREF(s);
-    } else {
-        s = PyObject_Str(o);
-        if (!s) return NULL;
-        {
-            PyObject *t = PyUnicode_AsASCIIString(s);
-            Py_DECREF(s);
-            if (!t) return NULL;
+    }
+    else {
+        PyObject *t = PyObject_Str(o);
+        if (!t) return NULL;
+
+        const char *encoding = (self && self->open) ?
+            _get_encoding(&self->connection) : utf8;
+        if (encoding == utf8) {
             s = t;
         }
+        else {
+            s = PyUnicode_AsEncodedString(t, encoding, "strict");
+            Py_DECREF(t);
+            if (!s) return NULL;
+        }
     }
-    in = PyBytes_AsString(s);
-    size = PyBytes_GET_SIZE(s);
-    str = PyBytes_FromStringAndSize((char *) NULL, size*2+3);
+
+    // Prepare input string (in, size)
+    const char *in;
+    Py_ssize_t size;
+    if (PyUnicode_Check(s)) {
+        in = PyUnicode_AsUTF8AndSize(s, &size);
+    } else {
+        assert(PyBytes_Check(s));
+        in = PyBytes_AsString(s);
+        size = PyBytes_GET_SIZE(s);
+    }
+
+    // Prepare output buffer (str, out)
+    PyObject *str = PyBytes_FromStringAndSize((char *) NULL, size*2+3);
     if (!str) {
         Py_DECREF(s);
         return PyErr_NoMemory();
     }
-    out = PyBytes_AS_STRING(str);
+    char *out = PyBytes_AS_STRING(str);
+
+    // escape
+    unsigned long len;
     if (self && self->open) {
 #if MYSQL_VERSION_ID >= 50707 && !defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
         len = mysql_real_escape_string_quote(&(self->connection), out+1, in, size, '\'');
 #else
         len = mysql_real_escape_string(&(self->connection), out+1, in, size);
 #endif
     } else {
         len = mysql_escape_string(out+1, in, size);
     }
-    *out = *(out+len+1) = '\'';
-    if (_PyBytes_Resize(&str, len+2) < 0) return NULL;
+
     Py_DECREF(s);
-    return (str);
+    *out = *(out+len+1) = '\'';
+    if (_PyBytes_Resize(&str, len+2) < 0) {
+        Py_DECREF(str);
+        return NULL;
+    }
+    return str;
 }
 
 static PyObject *
 _escape_item(
     PyObject *self,
     PyObject *item,
     PyObject *d)
@@ -1384,17 +1420,17 @@
 
     Py_ssize_t i;
     for (i = 0; i < maxrows; i++) {
         MYSQL_ROW row;
         if (!self->use)
             row = mysql_fetch_row(self->result);
         else {
-            Py_BEGIN_ALLOW_THREADS;
+            Py_BEGIN_ALLOW_THREADS
             row = mysql_fetch_row(self->result);
-            Py_END_ALLOW_THREADS;
+            Py_END_ALLOW_THREADS
         }
         if (!row && mysql_errno(&(((_mysql_ConnectionObject *)(self->conn))->connection))) {
             _mysql_Exception((_mysql_ConnectionObject *)self->conn);
             goto error;
         }
         if (!row) {
             break;
@@ -1465,14 +1501,37 @@
     Py_DECREF(r);
     return t;
   error:
     Py_XDECREF(r);
     return NULL;
 }
 
+static const char _mysql_ResultObject_discard__doc__[] =
+"discard() -- Discard remaining rows in the resultset.";
+
+static PyObject *
+_mysql_ResultObject_discard(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    check_result_connection(self);
+
+    MYSQL_ROW row;
+    Py_BEGIN_ALLOW_THREADS
+    while (NULL != (row = mysql_fetch_row(self->result))) {
+        // do nothing
+    }
+    Py_END_ALLOW_THREADS
+    _mysql_ConnectionObject *conn = (_mysql_ConnectionObject *)self->conn;
+    if (mysql_errno(&conn->connection)) {
+        return _mysql_Exception(conn);
+    }
+    Py_RETURN_NONE;
+}
+
 static char _mysql_ConnectionObject_change_user__doc__[] =
 "Changes the user and causes the database specified by db to\n\
 become the default (current) database on the connection\n\
 specified by mysql. In subsequent queries, this database is\n\
 the default for table references that do not include an\n\
 explicit database specifier.\n\
 \n\
@@ -1708,17 +1767,15 @@
 static PyObject *
 _mysql_ConnectionObject_insert_id(
     _mysql_ConnectionObject *self,
     PyObject *noargs)
 {
     my_ulonglong r;
     check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
     r = mysql_insert_id(&(self->connection));
-    Py_END_ALLOW_THREADS
     return PyLong_FromUnsignedLongLong(r);
 }
 
 static char _mysql_ConnectionObject_kill__doc__[] =
 "Asks the server to kill the thread specified by pid.\n\
 Non-standard.";
 
@@ -2019,17 +2076,15 @@
 static PyObject *
 _mysql_ConnectionObject_thread_id(
     _mysql_ConnectionObject *self,
     PyObject *noargs)
 {
     unsigned long pid;
     check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
     pid = mysql_thread_id(&(self->connection));
-    Py_END_ALLOW_THREADS
     return PyLong_FromLong((long)pid);
 }
 
 static char _mysql_ConnectionObject_use_result__doc__[] =
 "Returns a result object acquired by mysql_use_result\n\
 (results stored in the server). If no results are available,\n\
 None is returned. Non-standard.\n\
@@ -2062,14 +2117,51 @@
     }
   error:
     Py_DECREF(arglist);
     Py_XDECREF(kwarglist);
     return result;
 }
 
+static const char _mysql_ConnectionObject_discard_result__doc__[] =
+"Discard current result set.\n\n"
+"This function can be called instead of use_result() or store_result(). Non-standard.";
+
+static PyObject *
+_mysql_ConnectionObject_discard_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    MYSQL *conn = &(self->connection);
+
+    Py_BEGIN_ALLOW_THREADS;
+
+    MYSQL_RES *res = mysql_use_result(conn);
+    if (res == NULL) {
+        Py_BLOCK_THREADS;
+        if (mysql_errno(conn) != 0) {
+            // fprintf(stderr, "mysql_use_result failed: %s\n", mysql_error(conn));
+            return _mysql_Exception(self);
+        }
+        Py_RETURN_NONE;
+    }
+
+    MYSQL_ROW row;
+    while (NULL != (row = mysql_fetch_row(res))) {
+        // do nothing.
+    }
+    mysql_free_result(res);
+    Py_END_ALLOW_THREADS;
+    if (mysql_errno(conn)) {
+        // fprintf(stderr, "mysql_free_result failed: %s\n", mysql_error(conn));
+        return _mysql_Exception(self);
+    }
+    Py_RETURN_NONE;
+}
+
 static void
 _mysql_ConnectionObject_dealloc(
     _mysql_ConnectionObject *self)
 {
     PyObject_GC_UnTrack(self);
     if (self->open) {
         mysql_close(&(self->connection));
@@ -2357,14 +2449,20 @@
     },
     {
         "use_result",
         (PyCFunction)_mysql_ConnectionObject_use_result,
         METH_NOARGS,
         _mysql_ConnectionObject_use_result__doc__
     },
+    {
+        "discard_result",
+        (PyCFunction)_mysql_ConnectionObject_discard_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_discard_result__doc__
+    },
     {NULL,              NULL} /* sentinel */
 };
 
 static struct PyMemberDef _mysql_ConnectionObject_memberlist[] = {
     {
         "open",
         T_INT,
@@ -2419,14 +2517,20 @@
     {
         "fetch_row",
         (PyCFunction)_mysql_ResultObject_fetch_row,
         METH_VARARGS | METH_KEYWORDS,
         _mysql_ResultObject_fetch_row__doc__
     },
     {
+        "discard",
+        (PyCFunction)_mysql_ResultObject_discard,
+        METH_NOARGS,
+        _mysql_ResultObject_discard__doc__
+    },
+    {
         "field_flags",
         (PyCFunction)_mysql_ResultObject_field_flags,
         METH_NOARGS,
         _mysql_ResultObject_field_flags__doc__
     },
     {
         "num_fields",
```

### Comparing `mysqlclient-2.1.1/MySQLdb/connections.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,22 @@
             this setting.
             Default to True.
 
         :param str charset:
             If supplied, the connection character set will be changed
             to this character set.
 
+        :param str collation:
+            If ``charset`` and ``collation`` are both supplied, the
+            character set and collation for the current connection
+            will be set.
+
+            If omitted, empty string, or None, the default collation
+            for the ``charset`` is implied.
+
         :param str auth_plugin:
             If supplied, the connection default authentication plugin will be
             changed to this value. Example values:
             `mysql_native_password` or `caching_sha2_password`
 
         :param str sql_mode:
             If supplied, the session SQL mode will be changed to this
@@ -140,15 +148,14 @@
             arguments (e.g. Binary). This is disabled by default.
 
         There are a number of undocumented, non-standard methods. See the
         documentation for the MySQL C API for some hints on what they do.
         """
         from MySQLdb.constants import CLIENT, FIELD_TYPE
         from MySQLdb.converters import conversions, _bytes_or_str
-        from weakref import proxy
 
         kwargs2 = kwargs.copy()
 
         if "db" in kwargs2:
             kwargs2["database"] = kwargs2.pop("db")
         if "passwd" in kwargs2:
             kwargs2["password"] = kwargs2.pop("passwd")
@@ -164,14 +171,15 @@
                 conv2[k] = v[:]
             else:
                 conv2[k] = v
         kwargs2["conv"] = conv2
 
         cursorclass = kwargs2.pop("cursorclass", self.default_cursor)
         charset = kwargs2.get("charset", "")
+        collation = kwargs2.pop("collation", "")
         use_unicode = kwargs2.pop("use_unicode", True)
         sql_mode = kwargs2.pop("sql_mode", "")
         self._binary_prefix = kwargs2.pop("binary_prefix", False)
 
         client_flag = kwargs.get("client_flag", 0)
         client_flag |= CLIENT.MULTI_RESULTS
         multi_statements = kwargs2.pop("multi_statements", True)
@@ -190,15 +198,15 @@
             [numeric_part(n) for n in self.get_server_info().split(".")[:2]]
         )
 
         self.encoding = "ascii"  # overridden in set_character_set()
 
         if not charset:
             charset = self.character_set_name()
-        self.set_character_set(charset)
+        self.set_character_set(charset, collation)
 
         if sql_mode:
             self.set_sql_mode(sql_mode)
 
         if use_unicode:
             for t in (
                 FIELD_TYPE.STRING,
@@ -210,21 +218,14 @@
                 FIELD_TYPE.BLOB,
             ):
                 self.converter[t] = _bytes_or_str
             # Unlike other string/blob types, JSON is always text.
             # MySQL may return JSON with charset==binary.
             self.converter[FIELD_TYPE.JSON] = str
 
-        db = proxy(self)
-
-        def unicode_literal(u, dummy=None):
-            return db.string_literal(u.encode(db.encoding))
-
-        self.encoders[str] = unicode_literal
-
         self._transactional = self.server_capabilities & CLIENT.TRANSACTIONS
         if self._transactional:
             if autocommit is not None:
                 self.autocommit(autocommit)
         self.messages = []
 
     def __enter__(self):
@@ -289,18 +290,21 @@
     def begin(self):
         """Explicitly begin a connection.
 
         This method is not used when autocommit=False (default).
         """
         self.query(b"BEGIN")
 
-    def set_character_set(self, charset):
+    def set_character_set(self, charset, collation=None):
         """Set the connection character set to charset."""
         super().set_character_set(charset)
         self.encoding = _charset_to_encoding.get(charset, charset)
+        if collation:
+            self.query(f"SET NAMES {charset} COLLATE {collation}")
+            self.store_result()
 
     def set_sql_mode(self, sql_mode):
         """Set the connection sql_mode. See MySQL documentation for
         legal values."""
         if self._server_version < (4, 1):
             raise NotSupportedError("server is too old to set sql_mode")
         self.query("SET SESSION sql_mode='%s'" % sql_mode)
```

### Comparing `mysqlclient-2.1.1/MySQLdb/constants/CLIENT.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/MySQLdb/constants/CR.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/CR.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     error_last = value
                 continue
             if value not in data:
                 data[value] = set()
             data[value].add(name)
     for value, names in sorted(data.items()):
         for name in sorted(names):
-            print("{} = {}".format(name, value))
+            print(f"{name} = {value}")
     if error_last is not None:
         print("ERROR_LAST = %s" % error_last)
 
 
 ERROR_FIRST = 2000
 MIN_ERROR = 2000
 UNKNOWN_ERROR = 2000
```

### Comparing `mysqlclient-2.1.1/MySQLdb/constants/ER.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/ER.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     error_last = value
                 continue
             if value not in data:
                 data[value] = set()
             data[value].add(name)
     for value, names in sorted(data.items()):
         for name in sorted(names):
-            print("{} = {}".format(name, value))
+            print(f"{name} = {value}")
     if error_last is not None:
         print("ERROR_LAST = %s" % error_last)
 
 
 ERROR_FIRST = 1000
 NO = 1002
 YES = 1003
```

### Comparing `mysqlclient-2.1.1/MySQLdb/constants/FIELD_TYPE.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/FIELD_TYPE.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/MySQLdb/converters.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 def Thing2Str(s, d):
     """Convert something into a string via str()."""
     return str(s)
 
 
 def Float2Str(o, d):
     s = repr(o)
-    if s in ("inf", "nan"):
+    if s in ("inf", "-inf", "nan"):
         raise ProgrammingError("%s can not be used with MySQL" % s)
     if "e" not in s:
         s += "e0"
     return s
 
 
 def None2NULL(o, d):
```

### Comparing `mysqlclient-2.1.1/MySQLdb/cursors.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/cursors.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 default, MySQLdb uses the Cursor class.
 """
 import re
 
 from ._exceptions import ProgrammingError
 
 
-#: Regular expression for :meth:`Cursor.executemany`.
+#: Regular expression for ``Cursor.executemany```.
 #: executemany only supports simple bulk insert.
 #: You can use it to load large dataset.
 RE_INSERT_VALUES = re.compile(
     "".join(
         [
             r"\s*((?:INSERT|REPLACE)\b.+\bVALUES?\s*)",
             r"(\(\s*(?:%s|%\(.+\)s)\s*(?:,\s*(?:%s|%\(.+\)s)\s*)*\))",
@@ -62,69 +62,60 @@
 
     connection = None
 
     def __init__(self, connection):
         self.connection = connection
         self.description = None
         self.description_flags = None
-        self.rowcount = -1
+        self.rowcount = 0
         self.arraysize = 1
         self._executed = None
 
         self.lastrowid = None
         self._result = None
         self.rownumber = None
         self._rows = None
 
+    def _discard(self):
+        self.description = None
+        self.description_flags = None
+        # Django uses some member after __exit__.
+        # So we keep rowcount and lastrowid here. They are cleared in Cursor._query().
+        # self.rowcount = 0
+        # self.lastrowid = None
+        self._rows = None
+        self.rownumber = None
+
+        if self._result:
+            self._result.discard()
+            self._result = None
+
+        con = self.connection
+        if con is None:
+            return
+        while con.next_result() == 0:  # -1 means no more data.
+            con.discard_result()
+
     def close(self):
         """Close the cursor. No further queries will be possible."""
         try:
             if self.connection is None:
                 return
-            while self.nextset():
-                pass
+            self._discard()
         finally:
             self.connection = None
             self._result = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc_info):
         del exc_info
         self.close()
 
-    def _escape_args(self, args, conn):
-        encoding = conn.encoding
-        literal = conn.literal
-
-        def ensure_bytes(x):
-            if isinstance(x, str):
-                return x.encode(encoding)
-            elif isinstance(x, tuple):
-                return tuple(map(ensure_bytes, x))
-            elif isinstance(x, list):
-                return list(map(ensure_bytes, x))
-            return x
-
-        if isinstance(args, (tuple, list)):
-            ret = tuple(literal(ensure_bytes(arg)) for arg in args)
-        elif isinstance(args, dict):
-            ret = {
-                ensure_bytes(key): literal(ensure_bytes(val))
-                for (key, val) in args.items()
-            }
-        else:
-            # If it's not a dictionary let's try escaping it anyways.
-            # Worst case it will throw a Value error
-            ret = literal(ensure_bytes(args))
-
-        ensure_bytes = None  # break circular reference
-        return ret
-
     def _check_executed(self):
         if not self._executed:
             raise ProgrammingError("execute() first")
 
     def nextset(self):
         """Advance to the next result set.
 
@@ -176,16 +167,24 @@
 
         Note: If args is a sequence, then %s must be used as the
         parameter placeholder in the query. If a mapping is used,
         %(key)s must be used as the placeholder.
 
         Returns integer represents rows affected, if any
         """
-        while self.nextset():
-            pass
+        self._discard()
+
+        mogrified_query = self._mogrify(query, args)
+
+        assert isinstance(mogrified_query, (bytes, bytearray))
+        res = self._query(mogrified_query)
+        return res
+
+    def _mogrify(self, query, args=None):
+        """Return query after binding args."""
         db = self._get_db()
 
         if isinstance(query, str):
             query = query.encode(db.encoding)
 
         if args is not None:
             if isinstance(args, dict):
@@ -198,17 +197,29 @@
             else:
                 args = tuple(map(db.literal, args))
             try:
                 query = query % args
             except TypeError as m:
                 raise ProgrammingError(str(m))
 
-        assert isinstance(query, (bytes, bytearray))
-        res = self._query(query)
-        return res
+        return query
+
+    def mogrify(self, query, args=None):
+        """Return query after binding args.
+
+        query -- string, query to mogrify
+        args -- optional sequence or mapping, parameters to use with query.
+
+        Note: If args is a sequence, then %s must be used as the
+        parameter placeholder in the query. If a mapping is used,
+        %(key)s must be used as the placeholder.
+
+        Returns string representing query that would be executed by the server
+        """
+        return self._mogrify(query, args).decode(self._get_db().encoding)
 
     def executemany(self, query, args):
         # type: (str, list) -> int
         """Execute a multi-row query.
 
         :param query: query to execute on server
         :param args:  Sequence of sequences or mappings.  It is used as parameter.
@@ -238,29 +249,27 @@
 
         self.rowcount = sum(self.execute(query, arg) for arg in args)
         return self.rowcount
 
     def _do_execute_many(
         self, prefix, values, postfix, args, max_stmt_length, encoding
     ):
-        conn = self._get_db()
-        escape = self._escape_args
         if isinstance(prefix, str):
             prefix = prefix.encode(encoding)
         if isinstance(values, str):
             values = values.encode(encoding)
         if isinstance(postfix, str):
             postfix = postfix.encode(encoding)
         sql = bytearray(prefix)
         args = iter(args)
-        v = values % escape(next(args), conn)
+        v = self._mogrify(values, next(args))
         sql += v
         rows = 0
         for arg in args:
-            v = values % escape(arg, conn)
+            v = self._mogrify(values, arg)
             if len(sql) + len(v) + len(postfix) + 1 > max_stmt_length:
                 rows += self.execute(sql + postfix)
                 sql = bytearray(prefix)
             else:
                 sql += b","
             sql += v
         rows += self.execute(sql + postfix)
@@ -312,14 +321,16 @@
         )
         self._query(q)
         return args
 
     def _query(self, q):
         db = self._get_db()
         self._result = None
+        self.rowcount = None
+        self.lastrowid = None
         db.query(q)
         self._do_get_result(db)
         self._post_get_result()
         self._executed = q
         return self.rowcount
 
     def _fetch_row(self, size=1):
```

### Comparing `mysqlclient-2.1.1/MySQLdb/times.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/times.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/PKG-INFO` & `mysqlclient-2.2.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: mysqlclient
-Version: 2.1.1
+Version: 2.2.0rc1
 Summary: Python interface to MySQL
-Home-page: https://github.com/PyMySQL/mysqlclient
-Author: Inada Naoki
-Author-email: songofacandy@gmail.com
-License: GPL
-Platform: ALL
+Author-email: Inada Naoki <songofacandy@gmail.com>
+License: GNU General Public License v2 (GPLv2)
+Project-URL: Project, https://github.com/PyMySQL/mysqlclient
+Project-URL: Documentation, https://mysqlclient.readthedocs.io/
+Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mysqlclient
 
 This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
 This project adds Python 3 support and fixed many bugs.
@@ -78,25 +77,24 @@
 
 ### macOS (Homebrew)
 
 Install MySQL and mysqlclient:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql
+$ brew install mysql pkg-config
 $ pip install mysqlclient
 ```
 
 If you don't want to install MySQL server, you can use mysql-client instead:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql-client
-$ echo 'export PATH="/usr/local/opt/mysql-client/bin:$PATH"' >> ~/.bash_profile
-$ export PATH="/usr/local/opt/mysql-client/bin:$PATH"
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
 $ pip install mysqlclient
 ```
 
 ### Linux
 
 **Note that this is a basic step.  I can not support complete step for build for all
 environment.  If you can see some error, you should fix it by yourself, or ask for
@@ -111,15 +109,15 @@
 
 ```
 $ pip install mysqlclient
 ```
 
 ### Customize build (POSIX)
 
-mysqlclient uses `mysql_config` or `mariadb_config` by default for finding
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
 compiler/linker flags.
 
 You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
 variables to customize compiler/linker options.
 
 ```
 $ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
```

### Comparing `mysqlclient-2.1.1/README.md` & `mysqlclient-2.2.0rc1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -46,25 +46,24 @@
 
 ### macOS (Homebrew)
 
 Install MySQL and mysqlclient:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql
+$ brew install mysql pkg-config
 $ pip install mysqlclient
 ```
 
 If you don't want to install MySQL server, you can use mysql-client instead:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql-client
-$ echo 'export PATH="/usr/local/opt/mysql-client/bin:$PATH"' >> ~/.bash_profile
-$ export PATH="/usr/local/opt/mysql-client/bin:$PATH"
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
 $ pip install mysqlclient
 ```
 
 ### Linux
 
 **Note that this is a basic step.  I can not support complete step for build for all
 environment.  If you can see some error, you should fix it by yourself, or ask for
@@ -79,15 +78,15 @@
 
 ```
 $ pip install mysqlclient
 ```
 
 ### Customize build (POSIX)
 
-mysqlclient uses `mysql_config` or `mariadb_config` by default for finding
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
 compiler/linker flags.
 
 You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
 variables to customize compiler/linker options.
 
 ```
 $ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
```

### Comparing `mysqlclient-2.1.1/doc/FAQ.rst` & `mysqlclient-2.2.0rc1/doc/FAQ.rst`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/doc/MySQLdb.constants.rst` & `mysqlclient-2.2.0rc1/doc/MySQLdb.constants.rst`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/doc/conf.py` & `mysqlclient-2.2.0rc1/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration -----------------------------------------------------
 
+nitpick_ignore = [
+    ("py:class", "datetime.date"),
+    ("py:class", "datetime.time"),
+    ("py:class", "datetime.datetime"),
+]
+
+
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = "1.0"
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ["sphinx.ext.autodoc"]
```

### Comparing `mysqlclient-2.1.1/doc/user_guide.rst` & `mysqlclient-2.2.0rc1/doc/user_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,30 @@
             override this with use_unicode=False, though you probably
             shouldn't.
 
             If not present, the default character set is used.
 
             *This must be a keyword parameter.*
 
+         collation
+            If ``charset`` and ``collation`` are both supplied, the
+            character set and collation for the current connection
+            will be set.
+
+            If omitted, empty string, or None, the default collation
+            for the ``charset`` is implied by the database server.
+
+            To learn more about the quiddities of character sets and
+            collations, consult the `MySQL docs
+            <https://dev.mysql.com/doc/refman/8.0/en/charset.html>`_
+            and `MariaDB docs
+            <https://mariadb.com/kb/en/character-sets/>`_
+
+            *This must be a keyword parameter.*
+
          sql_mode
             If present, the session SQL mode will be set to the given
             string. For more information on sql_mode, see the MySQL
             documentation. Only available for 4.1 and newer servers.
 
             If not present, the session SQL mode will be unchanged.
```

### Comparing `mysqlclient-2.1.1/mysqlclient.egg-info/PKG-INFO` & `mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: mysqlclient
-Version: 2.1.1
+Version: 2.2.0rc1
 Summary: Python interface to MySQL
-Home-page: https://github.com/PyMySQL/mysqlclient
-Author: Inada Naoki
-Author-email: songofacandy@gmail.com
-License: GPL
-Platform: ALL
+Author-email: Inada Naoki <songofacandy@gmail.com>
+License: GNU General Public License v2 (GPLv2)
+Project-URL: Project, https://github.com/PyMySQL/mysqlclient
+Project-URL: Documentation, https://mysqlclient.readthedocs.io/
+Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mysqlclient
 
 This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
 This project adds Python 3 support and fixed many bugs.
@@ -78,25 +77,24 @@
 
 ### macOS (Homebrew)
 
 Install MySQL and mysqlclient:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql
+$ brew install mysql pkg-config
 $ pip install mysqlclient
 ```
 
 If you don't want to install MySQL server, you can use mysql-client instead:
 
 ```
 # Assume you are activating Python 3 venv
-$ brew install mysql-client
-$ echo 'export PATH="/usr/local/opt/mysql-client/bin:$PATH"' >> ~/.bash_profile
-$ export PATH="/usr/local/opt/mysql-client/bin:$PATH"
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
 $ pip install mysqlclient
 ```
 
 ### Linux
 
 **Note that this is a basic step.  I can not support complete step for build for all
 environment.  If you can see some error, you should fix it by yourself, or ask for
@@ -111,15 +109,15 @@
 
 ```
 $ pip install mysqlclient
 ```
 
 ### Customize build (POSIX)
 
-mysqlclient uses `mysql_config` or `mariadb_config` by default for finding
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
 compiler/linker flags.
 
 You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
 variables to customize compiler/linker options.
 
 ```
 $ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
```

### Comparing `mysqlclient-2.1.1/tests/capabilities.py` & `mysqlclient-2.2.0rc1/tests/capabilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 """
 from time import time
 import unittest
 from configdb import connection_factory
 
 
 class DatabaseTest(unittest.TestCase):
-
     db_module = None
     connect_args = ()
     connect_kwargs = dict()
     create_table_extra = ""
     rows = 10
     debug = False
 
     def setUp(self):
-
         db = connection_factory(**self.connect_kwargs)
         self.connection = db
         self.cursor = db.cursor()
         self.BLOBUText = "".join([chr(i) for i in range(16384)])
         self.BLOBBinary = self.db_module.Binary(
             ("".join([chr(i) for i in range(256)] * 16)).encode("latin1")
         )
@@ -33,21 +31,21 @@
 
     def tearDown(self):
         if self.leak_test:
             import gc
 
             del self.cursor
             orphans = gc.collect()
-            self.failIf(
+            self.assertFalse(
                 orphans, "%d orphaned objects found after deleting cursor" % orphans
             )
 
             del self.connection
             orphans = gc.collect()
-            self.failIf(
+            self.assertFalse(
                 orphans, "%d orphaned objects found after deleting connection" % orphans
             )
 
     def table_exists(self, name):
         try:
             self.cursor.execute("select * from %s where 1=0" % name)
         except Exception:
@@ -63,15 +61,14 @@
         while True:
             name = self.quote_identifier("tb%08x" % i)
             if not self.table_exists(name):
                 return name
             i = i + 1
 
     def create_table(self, columndefs):
-
         """Create a table using a list of column definitions given in
         columndefs.
 
         generator must be a function taking arguments (row_number,
         col_number) returning a suitable data object for insertion
         into the table.
 
@@ -81,15 +78,15 @@
             "CREATE TABLE %s (%s) %s"
             % (self.table, ",\n".join(columndefs), self.create_table_extra)
         )
 
     def check_data_integrity(self, columndefs, generator):
         # insert
         self.create_table(columndefs)
-        insert_statement = "INSERT INTO %s VALUES (%s)" % (
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
             self.table,
             ",".join(["%s"] * len(columndefs)),
         )
         data = [
             [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
         ]
         self.cursor.executemany(insert_statement, data)
@@ -112,15 +109,15 @@
         def generator(row, col):
             if col == 0:
                 return row
             else:
                 return ("%i" % (row % 10)) * 255
 
         self.create_table(columndefs)
-        insert_statement = "INSERT INTO %s VALUES (%s)" % (
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
             self.table,
             ",".join(["%s"] * len(columndefs)),
         )
         data = [
             [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
         ]
         self.cursor.executemany(insert_statement, data)
@@ -130,34 +127,34 @@
         res = self.cursor.fetchall()
         self.assertEqual(len(res), self.rows)
         for i in range(self.rows):
             for j in range(len(columndefs)):
                 self.assertEqual(res[i][j], generator(i, j))
         delete_statement = "delete from %s where col1=%%s" % self.table
         self.cursor.execute(delete_statement, (0,))
-        self.cursor.execute("select col1 from %s where col1=%s" % (self.table, 0))
+        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
         res = self.cursor.fetchall()
         self.assertFalse(res, "DELETE didn't work")
         self.connection.rollback()
-        self.cursor.execute("select col1 from %s where col1=%s" % (self.table, 0))
+        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
         res = self.cursor.fetchall()
         self.assertTrue(len(res) == 1, "ROLLBACK didn't work")
         self.cursor.execute("drop table %s" % (self.table))
 
     def test_truncation(self):
         columndefs = ("col1 INT", "col2 VARCHAR(255)")
 
         def generator(row, col):
             if col == 0:
                 return row
             else:
                 return ("%i" % (row % 10)) * ((255 - self.rows // 2) + row)
 
         self.create_table(columndefs)
-        insert_statement = "INSERT INTO %s VALUES (%s)" % (
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
             self.table,
             ",".join(["%s"] * len(columndefs)),
         )
 
         try:
             self.cursor.execute(insert_statement, (0, "0" * 256))
         except self.connection.DataError:
```

### Comparing `mysqlclient-2.1.1/tests/configdb.py` & `mysqlclient-2.2.0rc1/tests/configdb.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/tests/dbapi20.py` & `mysqlclient-2.2.0rc1/tests/dbapi20.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 # - Now a subclass of TestCase, to avoid requiring the driver stub
 #   to use multiple inheritance
 # - Reversed the polarity of buggy test in test_description
 # - Test exception hierarchy correctly
 # - self.populate is now self._populate(), so if a driver stub
 #   overrides self.ddl1 this change propagates
 # - VARCHAR columns now have a width, which will hopefully make the
-#   DDL even more portible (this will be reversed if it causes more problems)
+#   DDL even more portable (this will be reversed if it causes more problems)
 # - cursor.rowcount being checked after various execute and fetchXXX methods
 # - Check for fetchall and fetchmany returning empty lists after results
 #   are exhausted (already checking for empty lists if select retrieved
 #   nothing
 # - Fix bugs in test_setoutputsize_basic and test_setinputsizes
 #
 
@@ -521,16 +521,15 @@
     ]
 
     def _populate(self):
         """Return a list of sql commands to setup the DB for the fetch
         tests.
         """
         populate = [
-            "insert into {}booze values ('{}')".format(self.table_prefix, s)
-            for s in self.samples
+            f"insert into {self.table_prefix}booze values ('{s}')" for s in self.samples
         ]
         return populate
 
     def test_fetchmany(self):
         con = self._connect()
         try:
             cur = con.cursor()
```

### Comparing `mysqlclient-2.1.1/tests/test_MySQLdb_capabilities.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_capabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import warnings
 
 
 warnings.filterwarnings("ignore")
 
 
 class test_MySQLdb(capabilities.DatabaseTest):
-
     db_module = MySQLdb
     connect_args = ()
     connect_kwargs = dict(
         use_unicode=True, sql_mode="ANSI,STRICT_TRANS_TABLES,TRADITIONAL"
     )
     create_table_extra = "ENGINE=INNODB CHARACTER SET UTF8"
     leak_test = False
```

### Comparing `mysqlclient-2.1.1/tests/test_MySQLdb_dbapi20.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/tests/test_MySQLdb_nonstandard.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_nonstandard.py`

 * *Files 24% similar despite different names*

```diff
@@ -110,7 +110,37 @@
     def test_fileno(self):
         self.assertGreaterEqual(self.conn.fileno(), 0)
 
     def test_context_manager(self):
         with connection_factory() as conn:
             self.assertFalse(conn.closed)
         self.assertTrue(conn.closed)
+
+
+class TestCollation(unittest.TestCase):
+    """Test charset and collation connection options."""
+
+    def setUp(self):
+        # Initialize a connection with a non-default character set and
+        # collation.
+        self.conn = connection_factory(
+            charset="utf8mb4",
+            collation="utf8mb4_esperanto_ci",
+        )
+
+    def tearDown(self):
+        self.conn.close()
+
+    def test_charset_collation(self):
+        c = self.conn.cursor()
+        c.execute(
+            """
+            SHOW VARIABLES WHERE
+            Variable_Name="character_set_connection" OR
+            Variable_Name="collation_connection";
+            """
+        )
+        row = c.fetchall()
+        charset = row[0][1]
+        collation = row[1][1]
+        self.assertEqual(charset, "utf8mb4")
+        self.assertEqual(collation, "utf8mb4_esperanto_ci")
```

### Comparing `mysqlclient-2.1.1/tests/test_MySQLdb_times.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_times.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/tests/test_connection.py` & `mysqlclient-2.2.0rc1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `mysqlclient-2.1.1/tests/test_cursor.py` & `mysqlclient-2.2.0rc1/tests/test_cursor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# import pytest
+import pytest
 import MySQLdb.cursors
 from configdb import connection_factory
 
 
 _conns = []
 _tables = []
 
@@ -14,15 +14,15 @@
 
 
 def teardown_function(function):
     if _tables:
         c = _conns[0]
         cur = c.cursor()
         for t in _tables:
-            cur.execute("DROP TABLE {}".format(t))
+            cur.execute(f"DROP TABLE {t}")
         cur.close()
         del _tables[:]
 
     for c in _conns:
         c.close()
     del _conns[:]
 
@@ -68,15 +68,15 @@
 
     # cursor._executed myst bee
     # """
     # insert into test (data)
     # values (0),(1),(2),(3),(4),(5),(6),(7),(8),(9)
     # """
     # list args
-    data = range(10)
+    data = [(i,) for i in range(10)]
     cursor.executemany("insert into test (data) values (%s)", data)
     assert cursor._executed.endswith(
         b",(7),(8),(9)"
     ), "execute many with %s not in one query"
 
     # dict args
     data_dict = [{"data": i} for i in range(10)]
@@ -146,7 +146,100 @@
     assert rows[0] == {"t1.a": 1, "t1.b": 1, "t1.c": 47, "t2.b": 1, "t2.c": 1}
     assert rows[1] == {"t1.a": 2, "t1.b": 2, "t1.c": 47, "t2.b": 2, "t2.c": 2}
 
     names1 = sorted(rows[0])
     names2 = sorted(rows[1])
     for a, b in zip(names1, names2):
         assert a is b
+
+
+def test_mogrify_without_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query = "SELECT VERSION()"
+    mogrified_query = cursor.mogrify(query)
+    cursor.execute(query)
+
+    assert mogrified_query == query
+    assert mogrified_query == cursor._executed.decode()
+
+
+def test_mogrify_with_tuple_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query_with_args = "SELECT %s, %s", (1, 2)
+    mogrified_query = cursor.mogrify(*query_with_args)
+    cursor.execute(*query_with_args)
+
+    assert mogrified_query == "SELECT 1, 2"
+    assert mogrified_query == cursor._executed.decode()
+
+
+def test_mogrify_with_dict_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query_with_args = "SELECT %(a)s, %(b)s", {"a": 1, "b": 2}
+    mogrified_query = cursor.mogrify(*query_with_args)
+    cursor.execute(*query_with_args)
+
+    assert mogrified_query == "SELECT 1, 2"
+    assert mogrified_query == cursor._executed.decode()
+
+
+# Test that cursor can be used without reading whole resultset.
+@pytest.mark.parametrize("Cursor", [MySQLdb.cursors.Cursor, MySQLdb.cursors.SSCursor])
+def test_cursor_discard_result(Cursor):
+    conn = connect()
+    cursor = conn.cursor(Cursor)
+
+    cursor.execute(
+        """\
+CREATE TABLE test_cursor_discard_result (
+    id INTEGER PRIMARY KEY AUTO_INCREMENT,
+    data VARCHAR(100)
+)"""
+    )
+    _tables.append("test_cursor_discard_result")
+
+    cursor.executemany(
+        "INSERT INTO test_cursor_discard_result (id, data) VALUES (%s, %s)",
+        [(i, f"row {i}") for i in range(1, 101)],
+    )
+
+    cursor.execute(
+        """\
+SELECT * FROM test_cursor_discard_result WHERE id <= 10;
+SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 11 AND 20;
+SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 21 AND 30;
+"""
+    )
+    cursor.nextset()
+    assert cursor.fetchone() == (11, "row 11")
+
+    cursor.execute(
+        "SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 31 AND 40"
+    )
+    assert cursor.fetchone() == (31, "row 31")
+
+
+def test_binary_prefix():
+    # https://github.com/PyMySQL/mysqlclient/issues/494
+    conn = connect(binary_prefix=True)
+    cursor = conn.cursor()
+
+    cursor.execute("DROP TABLE IF EXISTS test_binary_prefix")
+    cursor.execute(
+        """\
+CREATE TABLE test_binary_prefix (
+	id INTEGER NOT NULL AUTO_INCREMENT,
+	json JSON NOT NULL,
+	PRIMARY KEY (id)
+) CHARSET=utf8mb4"""
+    )
+
+    cursor.executemany(
+        "INSERT INTO test_binary_prefix (id, json) VALUES (%(id)s, %(json)s)",
+        ({"id": 1, "json": "{}"}, {"id": 2, "json": "{}"}),
+    )
```

