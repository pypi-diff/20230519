# Comparing `tmp/symgt-0.0.1.tar.gz` & `tmp/symgt-0.0.2.tar.gz`

## Comparing `symgt-0.0.1.tar` & `symgt-0.0.2.tar`

### file list

```diff
@@ -1,346 +1,478 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 symgt-0.0.1/Makefile
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 symgt-0.0.1/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/__future__.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/__future__.meta.json
--rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_codecs.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_codecs.meta.json
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_collections_abc.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_collections_abc.meta.json
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_ctypes.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_ctypes.meta.json
--rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_thread.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_thread.meta.json
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_warnings.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_warnings.meta.json
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/array.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/ast.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/ast.meta.json
--rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/codecs.meta.json
--rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/contextlib.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/contextlib.meta.json
--rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/dataclasses.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/dataclasses.meta.json
--rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/datetime.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/datetime.meta.json
--rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/enum.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/enum.meta.json
--rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/functools.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/functools.meta.json
--rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/genericpath.meta.json
--rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/io.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/math.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/math.meta.json
--rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/mmap.meta.json
--rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/pathlib.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/pathlib.meta.json
--rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/pickle.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/pickle.meta.json
--rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/posixpath.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/posixpath.meta.json
--rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/re.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/re.meta.json
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_compile.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_compile.meta.json
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_constants.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_constants.meta.json
--rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_parse.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sre_parse.meta.json
--rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/string.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/string.meta.json
--rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/subprocess.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/subprocess.meta.json
--rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/textwrap.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/textwrap.meta.json
--rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/threading.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/threading.meta.json
--rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/time.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/time.meta.json
--rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/types.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/typing_extensions.meta.json
--rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/warnings.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/warnings.meta.json
--rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/zipfile.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/zipfile.meta.json
--rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/collections/abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/collections/abc.meta.json
--rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/__init__.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/__init__.meta.json
--rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/charset.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/charset.meta.json
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/contentmanager.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/errors.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/errors.meta.json
--rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/header.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/header.meta.json
--rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/message.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/message.meta.json
--rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/policy.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/email/policy.meta.json
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/machinery.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/machinery.meta.json
--rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/__init__.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/decoder.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/decoder.meta.json
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/encoder.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/json/encoder.meta.json
--rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/logging/__init__.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/logging/__init__.meta.json
--rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/__init__.data.json
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_version.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_version.meta.json
--rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/version.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/version.meta.json
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/records.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/__init__.data.json
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/__init__.meta.json
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/algorithms.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/algorithms.meta.json
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/models.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/symgt/models.meta.json
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/__init__.meta.json
--rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/_log.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/_log.meta.json
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/async_case.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/async_case.meta.json
--rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/case.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/case.meta.json
--rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/loader.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/loader.meta.json
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/main.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/main.meta.json
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/result.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/result.meta.json
--rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/runner.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/runner.meta.json
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/signals.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/signals.meta.json
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/suite.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.1/.mypy_cache/3.9/unittest/suite.meta.json
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/__init__.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/models.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/README.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.1/src/symgt/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 symgt-0.0.1/tests/01_smoke_test:_IIDModel.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 symgt-0.0.1/tests/02_smoke_test:_ExchangeableModel.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 symgt-0.0.1/.gitignore
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 symgt-0.0.1/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 symgt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 symgt-0.0.2/Makefile
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 symgt-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/__future__.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/__future__.meta.json
+-rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_ast.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_ast.meta.json
+-rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_codecs.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_codecs.meta.json
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_collections_abc.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_ctypes.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_ctypes.meta.json
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_thread.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_thread.meta.json
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_warnings.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_warnings.meta.json
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/abc.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/abc.meta.json
+-rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/array.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/array.meta.json
+-rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/ast.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/ast.meta.json
+-rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/builtins.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/builtins.meta.json
+-rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/codecs.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/codecs.meta.json
+-rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/contextlib.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/contextlib.meta.json
+-rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/dataclasses.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/dataclasses.meta.json
+-rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/datetime.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/datetime.meta.json
+-rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/enum.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/enum.meta.json
+-rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/functools.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/functools.meta.json
+-rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/genericpath.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/genericpath.meta.json
+-rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/io.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/io.meta.json
+-rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/math.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/math.meta.json
+-rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/mmap.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/mmap.meta.json
+-rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/pathlib.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/pathlib.meta.json
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/pickle.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/pickle.meta.json
+-rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/posixpath.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/posixpath.meta.json
+-rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/re.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/re.meta.json
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_compile.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_compile.meta.json
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_constants.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_constants.meta.json
+-rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_parse.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sre_parse.meta.json
+-rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/string.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/string.meta.json
+-rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/subprocess.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/subprocess.meta.json
+-rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sys.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/sys.meta.json
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/textwrap.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/textwrap.meta.json
+-rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/threading.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/threading.meta.json
+-rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/time.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/time.meta.json
+-rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/types.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/types.meta.json
+-rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/typing.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/typing.meta.json
+-rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/typing_extensions.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/typing_extensions.meta.json
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/warnings.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/warnings.meta.json
+-rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/zipfile.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/zipfile.meta.json
+-rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/collections/__init__.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/collections/abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/collections/abc.meta.json
+-rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/__init__.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/__init__.meta.json
+-rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/charset.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/charset.meta.json
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/errors.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/errors.meta.json
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/header.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/header.meta.json
+-rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/message.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/message.meta.json
+-rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/policy.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/email/policy.meta.json
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/abc.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/abc.meta.json
+-rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/__init__.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/decoder.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/decoder.meta.json
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/encoder.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/json/encoder.meta.json
+-rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/logging/__init__.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_version.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/version.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/version.meta.json
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/os/__init__.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/os/__init__.meta.json
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/os/path.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/os/path.meta.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/__init__.data.json
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/__init__.meta.json
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/algorithms.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/algorithms.meta.json
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/group_testing.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/group_testing.meta.json
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/models.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/models.meta.json
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/symgt/utils.meta.json
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/_log.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/_log.meta.json
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/case.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/case.meta.json
+-rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/loader.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/main.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/main.meta.json
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/result.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/result.meta.json
+-rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/runner.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/signals.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/suite.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.2/.mypy_cache/3.9/unittest/suite.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/1387c30be4948c1e
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/139172a1d04f111c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/1406495b142569a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/148366360f53eba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/16329b066f0bd583
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/190b917587a7c715
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/191feee62b4e11ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/1ec41655458704a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/20118812b6ba52d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2340b19700a4d682
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/24818994cc746ede
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/276f09acfa09134a
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/29605448695c5466
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2c14827ec14ea571
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2ce5607f55d6c3d2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2e4f72d891b1c583
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2fb9857b45c0fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/2fd14eda1f2186e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/351e1c52599eaade
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/35a93401322147ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/37f502c8357e13c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/3ea1b58a9db201c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/3ea29ca91ddb52ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/3ff7d03df56c2c53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/434ff347ecd8136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/445a9c301e6f9922
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/47e8b9593cc01a2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/4922673566a1ee36
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/4924663384114806
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/4b16d2e9d3162c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/4cd3e54afda99d16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/50e745492e64fbfa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/51bc6c2f813c4147
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/52677450217c860f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/5626133dcb4a8553
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/5771968da8511143
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/582595bb7a93a07c
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/5b3817478e0fea4b
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/5dc13b6c60c12647
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/5e78700d4867768f
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/61167eff0eefb0fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/618a6571ecee9116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/62ae216b5fa8f055
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/687736531e4ff9e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/6e464cd6d0ac79e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/70c50d94ce87c73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/79023d84cdbdccb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/7b07818c62c7164f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/7d4fae75818fdb66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/7d61eaea3d9ef118
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/7e85677f179a32fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/7f86f736a9393197
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/823ef04562dcffe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/82e947b2b493e786
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/83cc80f689aeb0e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/86f6f7623ec62813
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/87bcfdb723a49105
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/8e896e417a2d97a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/9163bcdb52a16e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/9274cc4b6e089349
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/92c85442d1888809
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/92c8ce56a95a5f1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/93fc9952d5f794da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/954f916cbc19a590
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/99f1d2d12ed2e065
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/9a75fddda97013a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a0b4bfcb514e3b37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a23b3883903c9835
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a3ef884c778a2446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a4cb8fe5e077df67
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a6b46d2dc660c905
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a6d313b912c8881d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/a729f14f424b74d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ab53134327ceac20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ac77bbe64a8ec76b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/adf937274b462e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/b10b1e2cfbefc26d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/b41ac728d4354728
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/b45df67a50d78b3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/b4a04d8a26f2e09e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/b5b5df558cad5c02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/baf82b7c177bcd74
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/be0446b85513b904
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/be35430973bd4acd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/bfb62a4104eab15b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/c077729fc5e04c13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/c2459e9433efdb77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/c7995819f0135276
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/c8dfecf945738849
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/cb846bee59a8a692
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/cc45a31c7ce341e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/cfae1ce212715249
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/d01d1cb9c55b5449
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/d0c02fd910364fe2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/d70bf06c6eee23d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/d80e9eb705d1d2a8
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/d9f344e7ff2bb0b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/dc9e0757631346a8
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/dd7ffba10d230bb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ddaa030a177fb15b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/de0dbe297e743771
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/df2b0dba6b763be1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e2ae383648735d1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e41b924848c9544c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e4db83144022a2e9
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e504bf6f224509f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e66be7c82afe1fc0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e858e289b8c427c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e87047886e38588f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e89c4b5bdad82e8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e8c57a50b031ae28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/e8e608cfa0dc40f4
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/eaa603b09b9e063
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ec24ffbb3ec32139
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ed21d1e13549d12f
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/ed7cf892f44fb99f
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/f1f975d7f1eda925
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/f643355a40a865f8
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/f8f07e0dd2e7876f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/fb612fe627f4238f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/fb7d9ed212c385a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.2/.ruff_cache/content/fc9ebb71114cfe85
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/__init__.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/algorithms.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/models.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/README.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.2/src/symgt/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 symgt-0.0.2/tests/01_smoke_test:_IIDModel.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 symgt-0.0.2/tests/02_smoke_test:_ExchangeableModel.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 symgt-0.0.2/tests/03_smoke_test:_algorithms.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 symgt-0.0.2/tests/04_smoke_test:_utils.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 symgt-0.0.2/.gitignore
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 symgt-0.0.2/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 symgt-0.0.2/PKG-INFO
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/__future__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/__future__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/__future__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_ast.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_ast.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_codecs.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_codecs.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_collections_abc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_collections_abc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_ctypes.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_ctypes.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_thread.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_thread.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_thread.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_warnings.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_warnings.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/abc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/abc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/array.data.json` & `symgt-0.0.2/.mypy_cache/3.9/array.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/array.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/array.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/ast.data.json` & `symgt-0.0.2/.mypy_cache/3.9/ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/ast.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/builtins.data.json` & `symgt-0.0.2/.mypy_cache/3.9/builtins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/builtins.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/codecs.data.json` & `symgt-0.0.2/.mypy_cache/3.9/codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/codecs.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/contextlib.data.json` & `symgt-0.0.2/.mypy_cache/3.9/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/contextlib.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/dataclasses.data.json` & `symgt-0.0.2/.mypy_cache/3.9/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/dataclasses.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/datetime.data.json` & `symgt-0.0.2/.mypy_cache/3.9/datetime.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/datetime.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/enum.data.json` & `symgt-0.0.2/.mypy_cache/3.9/enum.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/enum.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/enum.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/functools.data.json` & `symgt-0.0.2/.mypy_cache/3.9/functools.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/functools.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/functools.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/genericpath.data.json` & `symgt-0.0.2/.mypy_cache/3.9/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/genericpath.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/io.data.json` & `symgt-0.0.2/.mypy_cache/3.9/io.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/io.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/io.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/math.data.json` & `symgt-0.0.2/.mypy_cache/3.9/math.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/math.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/math.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/mmap.data.json` & `symgt-0.0.2/.mypy_cache/3.9/mmap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/mmap.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/pathlib.data.json` & `symgt-0.0.2/.mypy_cache/3.9/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/pathlib.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/pickle.data.json` & `symgt-0.0.2/.mypy_cache/3.9/pickle.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/pickle.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/posixpath.data.json` & `symgt-0.0.2/.mypy_cache/3.9/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/posixpath.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/re.data.json` & `symgt-0.0.2/.mypy_cache/3.9/re.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/re.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/re.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_compile.data.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_compile.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_constants.data.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_constants.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_parse.data.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sre_parse.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/string.data.json` & `symgt-0.0.2/.mypy_cache/3.9/string.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/string.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/string.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/subprocess.data.json` & `symgt-0.0.2/.mypy_cache/3.9/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/subprocess.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sys.data.json` & `symgt-0.0.2/.mypy_cache/3.9/sys.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/sys.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/sys.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/textwrap.data.json` & `symgt-0.0.2/.mypy_cache/3.9/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/textwrap.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/threading.data.json` & `symgt-0.0.2/.mypy_cache/3.9/threading.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/threading.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/threading.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/time.data.json` & `symgt-0.0.2/.mypy_cache/3.9/time.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/time.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/time.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/types.data.json` & `symgt-0.0.2/.mypy_cache/3.9/types.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/types.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/types.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/typing.data.json` & `symgt-0.0.2/.mypy_cache/3.9/typing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/typing.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/typing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/typing_extensions.data.json` & `symgt-0.0.2/.mypy_cache/3.9/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/typing_extensions.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/warnings.data.json` & `symgt-0.0.2/.mypy_cache/3.9/warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/warnings.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/zipfile.data.json` & `symgt-0.0.2/.mypy_cache/3.9/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/zipfile.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_typeshed/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/_typeshed/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/collections/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/collections/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/collections/abc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/collections/abc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/ctypes/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/ctypes/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/charset.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/charset.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/contentmanager.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/contentmanager.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/errors.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/errors.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/header.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/header.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/header.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/message.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/message.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/message.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/policy.data.json` & `symgt-0.0.2/.mypy_cache/3.9/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/email/policy.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/abc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/abc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/machinery.data.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/machinery.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/metadata/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/importlib/metadata/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/decoder.data.json` & `symgt-0.0.2/.mypy_cache/3.9/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/decoder.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/encoder.data.json` & `symgt-0.0.2/.mypy_cache/3.9/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/json/encoder.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/logging/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/logging/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_pytesttester.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_pytesttester.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_version.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_version.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ctypeslib.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ctypeslib.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/version.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/version.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_array_like.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_callable.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_callable.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nbit.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_scalars.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_shape.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_shape.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/_inspect.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/_inspect.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/py3k.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/compat/py3k.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_asarray.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_asarray.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_internal.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_internal.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_type_aliases.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/arrayprint.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/arrayprint.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/defchararray.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/defchararray.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/einsumfunc.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/fromnumeric.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/function_base.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/function_base.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/multiarray.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/multiarray.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/numeric.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/numeric.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/numerictypes.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/numerictypes.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/overrides.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/overrides.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/records.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/records.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/shape_base.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/shape_base.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/umath.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/core/umath.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/helper.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/fft/helper.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/_version.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/_version.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraypad.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraypad.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraysetops.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arrayterator.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/format.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/format.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/function_base.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/function_base.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/histograms.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/histograms.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/index_tricks.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/mixins.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/mixins.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/npyio.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/npyio.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/polynomial.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/polynomial.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/scimath.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/scimath.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/shape_base.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/shape_base.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/twodim_base.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/type_check.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/type_check.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/ufunclike.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/utils.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/lib/utils.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/linalg.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/linalg/linalg.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/core.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/core.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/extras.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/extras.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/mrecords.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/ma/mrecords.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/legendre.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_generator.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_generator.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_mt19937.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_mt19937.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_pcg64.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_pcg64.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_philox.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_philox.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_sfc64.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/_sfc64.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/bit_generator.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/bit_generator.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/mtrand.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/random/mtrand.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/utils.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/typing/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/numpy/typing/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/os/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/os/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/os/path.data.json` & `symgt-0.0.2/.mypy_cache/3.9/os/path.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/os/path.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/__init__.data.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'names'": "{delete: ['ECost', 'ETests', 'U_from_q', 'dorfman_multiplicity_function', "*

 * *            "'dorfman_pool_size', 'integer_partition', 'optimal_multiplicity_function']}"}*

```diff
@@ -2,39 +2,24 @@
     ".class": "MypyFile",
     "_fullname": "symgt",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
-        "ECost": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.ECost",
-            "kind": "Gdef"
-        },
-        "ETests": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.ETests",
-            "kind": "Gdef"
-        },
         "ExchangeableModel": {
             ".class": "SymbolTableNode",
             "cross_ref": "symgt.models.ExchangeableModel",
             "kind": "Gdef"
         },
         "IIDModel": {
             ".class": "SymbolTableNode",
             "cross_ref": "symgt.models.IIDModel",
             "kind": "Gdef"
         },
-        "U_from_q": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.U_from_q",
-            "kind": "Gdef"
-        },
         "__all__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
@@ -149,32 +134,11 @@
                     ".class": "Instance",
                     "args": [
                         "builtins.str"
                     ],
                     "type_ref": "builtins.list"
                 }
             }
-        },
-        "dorfman_multiplicity_function": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.dorfman_multiplicity_function",
-            "kind": "Gdef"
-        },
-        "dorfman_pool_size": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.dorfman_pool_size",
-            "kind": "Gdef"
-        },
-        "integer_partition": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.integer_partition",
-            "kind": "Gdef"
-        },
-        "optimal_multiplicity_function": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "symgt.algorithms.optimal_multiplicity_function",
-            "kind": "Gdef",
-            "module_public": false
         }
     },
     "path": "src/symgt/__init__.py"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/result.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.681060606060606%*

 * *Differences: {"'data_mtime'": '1684343458',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 3), (4, 4)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 20)]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'collections.abc'), (2, 'unittest'), (3, "*

 * *                   "'_typeshed'), (4, 'typing'), (7, 'types')], delete: [4, 1, 0]}",*

 * * "'hash'": "'c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767'",*

 * * "'id'": "'unittest.result'",*

 * * "'ignore_all'": 'True',*

 * * "'interface_hash'": "'d2489c54b11c542774e5e2697113 […]*

```diff
@@ -1,35 +1,44 @@
 {
-    "data_mtime": 1684439954,
+    "data_mtime": 1684343458,
     "dep_lines": [
         1,
+        3,
+        1,
         2,
+        4,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        20,
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "symgt.models",
-        "symgt.algorithms",
+        "unittest.case",
+        "collections.abc",
+        "unittest",
+        "_typeshed",
+        "typing",
         "builtins",
         "abc",
-        "typing"
+        "types"
     ],
-    "hash": "9751c26ea4e29c5f0f98a10c65a453f97e1308b3e250d2e8786e6a0a16547538",
-    "id": "symgt",
-    "ignore_all": false,
-    "interface_hash": "bbc88d8eff5ac8f25fcdc456476f8d7708d703c7d5ffe4e47c33fdb680ca6868",
-    "mtime": 1684439950,
+    "hash": "c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767",
+    "id": "unittest.result",
+    "ignore_all": true,
+    "interface_hash": "d2489c54b11c542774e5e2697113bf786523f06d344274c5c31626fc9dd87143",
+    "mtime": 1684343449,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/__init__.py",
+    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi",
     "plugin_data": null,
-    "size": 451,
+    "size": 1721,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/algorithms.data.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/utils.data.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8300801917989418%*

 * *Differences: {"'_fullname'": "'symgt.utils'",*

 * * "'names'": "{'ECost': {'node': {'arg_names': {insert: [(1, 'multfn')], delete: [0]}, 'fullname': "*

 * *            "'symgt.utils.ECost', 'type': {'arg_names': {insert: [(1, 'multfn')], delete: [0]}}}}, "*

 * *            "'ETests': {'node': {'arg_names': {insert: [(1, 'h')], delete: [0]}, 'fullname': "*

 * *            "'symgt.utils.ETests', 'type': {'arg_names': {insert: [(1, 'h')], delete: [0]}, "*

 * *            "'arg_types': {insert: [(1, 'builtins.int')], delete: [0]}}}}, 'U_from_q': {' […]*

```diff
@@ -1,10 +1,10 @@
 {
     ".class": "MypyFile",
-    "_fullname": "symgt.algorithms",
+    "_fullname": "symgt.utils",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
         "ECost": {
             ".class": "SymbolTableNode",
@@ -13,30 +13,30 @@
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0,
                     0
                 ],
                 "arg_names": [
-                    "multfn",
-                    "q"
+                    "q",
+                    "multfn"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "symgt.algorithms.ECost",
+                "fullname": "symgt.utils.ECost",
                 "name": "ECost",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0
                     ],
                     "arg_names": [
-                        "multfn",
-                        "q"
+                        "q",
+                        "multfn"
                     ],
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
                                 {
                                     ".class": "AnyType",
@@ -95,33 +95,32 @@
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0,
                     0
                 ],
                 "arg_names": [
-                    "h",
-                    "q"
+                    "q",
+                    "h"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "symgt.algorithms.ETests",
+                "fullname": "symgt.utils.ETests",
                 "name": "ETests",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0
                     ],
                     "arg_names": [
-                        "h",
-                        "q"
+                        "q",
+                        "h"
                     ],
                     "arg_types": [
-                        "builtins.int",
                         {
                             ".class": "Instance",
                             "args": [
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
@@ -131,15 +130,16 @@
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
                                     "type_of_any": 4
                                 }
                             ],
                             "type_ref": "numpy.ndarray"
-                        }
+                        },
+                        "builtins.int"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
@@ -149,34 +149,29 @@
                     "ret_type": "builtins.float",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "List": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.List",
-            "kind": "Gdef"
-        },
         "U_from_q": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0
                 ],
                 "arg_names": [
                     "q"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "symgt.algorithms.U_from_q",
+                "fullname": "symgt.utils.U_from_q",
                 "name": "U_from_q",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
                     "arg_names": [
@@ -239,15 +234,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "symgt.algorithms.__annotations__",
+                "fullname": "symgt.utils.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -264,176 +259,74 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "symgt.algorithms.__doc__",
+                "fullname": "symgt.utils.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "symgt.algorithms.__file__",
+                "fullname": "symgt.utils.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "symgt.algorithms.__name__",
+                "fullname": "symgt.utils.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "symgt.algorithms.__package__",
+                "fullname": "symgt.utils.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "dorfman_multiplicity_function": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    0
-                ],
-                "arg_names": [
-                    "n",
-                    "prevalence"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "symgt.algorithms.dorfman_multiplicity_function",
-                "name": "dorfman_multiplicity_function",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        0
-                    ],
-                    "arg_names": [
-                        "n",
-                        "prevalence"
-                    ],
-                    "arg_types": [
-                        "builtins.int",
-                        "builtins.float"
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "dorfman_multiplicity_function",
-                    "ret_type": {
-                        ".class": "Instance",
-                        "args": [
-                            "builtins.int"
-                        ],
-                        "type_ref": "builtins.list"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "dorfman_pool_size": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "prevalence",
-                    "max_pool_size"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "symgt.algorithms.dorfman_pool_size",
-                "name": "dorfman_pool_size",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "prevalence",
-                        "max_pool_size"
-                    ],
-                    "arg_types": [
-                        "builtins.float",
-                        "builtins.int"
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "dorfman_pool_size",
-                    "ret_type": "builtins.int",
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "integer_partition": {
+        "intpart_from_multfn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0
                 ],
                 "arg_names": [
                     "multfn"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "symgt.algorithms.integer_partition",
-                "name": "integer_partition",
+                "fullname": "symgt.utils.intpart_from_multfn",
+                "name": "intpart_from_multfn",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
                     "arg_names": [
                         "multfn"
@@ -462,104 +355,40 @@
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "integer_partition",
+                    "name": "intpart_from_multfn",
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
-                            "builtins.int"
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 4
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 4
+                            }
                         ],
-                        "type_ref": "builtins.list"
+                        "type_ref": "numpy.ndarray"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "np": {
             ".class": "SymbolTableNode",
             "cross_ref": "numpy",
             "kind": "Gdef"
-        },
-        "optimal_multiplicity_function": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "q",
-                    "subpopulations"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "symgt.algorithms.optimal_multiplicity_function",
-                "name": "optimal_multiplicity_function",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "q",
-                        "subpopulations"
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "Instance",
-                            "args": [
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
-                                }
-                            ],
-                            "type_ref": "numpy.ndarray"
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "optimal_multiplicity_function",
-                    "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
         }
     },
-    "path": "src/symgt/algorithms.py"
+    "path": "src/symgt/utils.py"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/algorithms.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/utils.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7533333333333334%*

 * *Differences: {"'data_mtime'": '1684473065',*

 * * "'dep_lines'": '{insert: [(1, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(12, 'typing')], delete: [1]}",*

 * * "'hash'": "'69b9bb4565230c169e8176d470e6def667a06eac5ac11bf122eeaf6521c8e76f'",*

 * * "'id'": "'symgt.utils'",*

 * * "'interface_hash'": "'a81ff2be0f7b5a295c9beaec8996ff9343354aa63ac231ee2e3b41136457c152'",*

 * * "'mtime'": '1684473551',*

 * * "'path'": "'src/symgt/utils.py'",*

 * * "'size'": '2091'}*

```diff
@@ -1,12 +1,12 @@
 {
-    "data_mtime": 1684447070,
+    "data_mtime": 1684473065,
     "dep_lines": [
         1,
-        4,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
@@ -15,48 +15,48 @@
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        5,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "numpy",
-        "typing",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "numpy._typing",
         "numpy._typing._array_like",
         "numpy._typing._dtype_like",
         "numpy._typing._nested_sequence",
         "pickle",
+        "typing",
         "typing_extensions"
     ],
-    "hash": "831f06bfaee1db4985c1fd2376c4857766fda79ae66881f6074db4a3951ad9d7",
-    "id": "symgt.algorithms",
+    "hash": "69b9bb4565230c169e8176d470e6def667a06eac5ac11bf122eeaf6521c8e76f",
+    "id": "symgt.utils",
     "ignore_all": false,
-    "interface_hash": "7ecbcb5d41de3a8098217fb01e094d55b2347af67262606dce927de59e1062da",
-    "mtime": 1684447051,
+    "interface_hash": "a81ff2be0f7b5a295c9beaec8996ff9343354aa63ac231ee2e3b41136457c152",
+    "mtime": 1684473551,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/algorithms.py",
+    "path": "src/symgt/utils.py",
     "plugin_data": null,
-    "size": 5384,
+    "size": 2091,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/models.data.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/models.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/symgt/models.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/models.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1684450247'}*

```diff
@@ -56,15 +56,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "7aedb860a2c6b13e832b72f1d9566f76f05521abd3cf41929e1dfa4e8417364a",
     "id": "symgt.models",
     "ignore_all": false,
     "interface_hash": "0e80c76e9a8836fc6df896fd0c5a0a2e7bc40ea3c838d493650ea4810808e512",
-    "mtime": 1684439954,
+    "mtime": 1684450247,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/__init__.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/__init__.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/_log.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/_log.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/async_case.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/async_case.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/case.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/case.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/loader.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/loader.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/main.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/main.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/result.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/result.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/signals.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7958333333333333%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 3), (4, 4)], delete: [4, 1, 0]}',*

 * * "'dep_prios'": '{delete: [6]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.result'), (4, 'typing_extensions')], delete: [7, 3, "*

 * *                   '0]}',*

 * * "'hash'": "'eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c'",*

 * * "'id'": "'unittest.signals'",*

 * * "'interface_hash'": "'86e1cc6b2b33a3f36be50112f0dc6de3164d947d5bae956669fea81619186462'",*

 * * "'path'": "'/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/sit […]*

```diff
@@ -1,43 +1,40 @@
 {
     "data_mtime": 1684343458,
     "dep_lines": [
         1,
-        3,
-        1,
         2,
-        4,
         1,
+        3,
+        4,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         20,
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "unittest.case",
+        "unittest.result",
         "collections.abc",
         "unittest",
-        "_typeshed",
         "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "types"
+        "abc"
     ],
-    "hash": "c3c84d157ab204cd3b00b3faf4d64cc85ad50fd622145a8032cde2378d31e767",
-    "id": "unittest.result",
+    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
+    "id": "unittest.signals",
     "ignore_all": true,
-    "interface_hash": "d2489c54b11c542774e5e2697113bf786523f06d344274c5c31626fc9dd87143",
+    "interface_hash": "86e1cc6b2b33a3f36be50112f0dc6de3164d947d5bae956669fea81619186462",
     "mtime": 1684343449,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi",
+    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
     "plugin_data": null,
-    "size": 1721,
+    "size": 488,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/runner.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/runner.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/signals.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/signals.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/suite.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 1), (5, 1)], delete: [2]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (6, 30)], delete: [3]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (7, 'typing')], delete: [3]}",*

 * * "'hash'": "'82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e'",*

 * * "'id'": "'unittest.suite'",*

 * * "'interface_hash'": "'9916fb1e8b3be752543760164ef567d207764e60d25de2267f89a51f85553ad7'",*

 * * "'path'": "'/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/types […]*

```diff
@@ -1,40 +1,43 @@
 {
     "data_mtime": 1684343458,
     "dep_lines": [
         1,
         2,
-        1,
         3,
+        1,
         4,
         1,
+        1,
         1
     ],
     "dep_prios": [
         10,
+        10,
         5,
         20,
         5,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
+        "unittest.case",
         "unittest.result",
         "collections.abc",
         "unittest",
-        "typing",
         "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
-    "id": "unittest.signals",
+    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
+    "id": "unittest.suite",
     "ignore_all": true,
-    "interface_hash": "86e1cc6b2b33a3f36be50112f0dc6de3164d947d5bae956669fea81619186462",
+    "interface_hash": "9916fb1e8b3be752543760164ef567d207764e60d25de2267f89a51f85553ad7",
     "mtime": 1684343449,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
+    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
     "plugin_data": null,
-    "size": 488,
+    "size": 983,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/suite.data.json` & `symgt-0.0.2/.mypy_cache/3.9/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/.mypy_cache/3.9/unittest/suite.meta.json` & `symgt-0.0.2/.mypy_cache/3.9/symgt/group_testing.meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.655807820204105%*

 * *Differences: {"'data_mtime'": '1684471031',*

 * * "'dep_lines'": '{insert: [(2, 1), (3, 1), (4, 1), (5, 1), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1)], delete: [4, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30), (4, 30), (5, 30), (6, 30), (7, 30), (8, 30), (9, 30), '*

 * *                '(10, 30), (11, 30)], delete: [4, 3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'numpy'), (2, '_typeshed'), (4, 'array'), (5, 'ctypes'), (6, "*

 * *                   "'mmap'), (7, 'numpy._typing'), (8, 'numpy._typing._array_lik […]*

```diff
@@ -1,44 +1,62 @@
 {
-    "data_mtime": 1684343458,
+    "data_mtime": 1684471031,
     "dep_lines": [
         1,
-        2,
-        3,
         1,
-        4,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
-        10,
-        5,
-        20,
-        5,
         5,
         30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "unittest.case",
-        "unittest.result",
-        "collections.abc",
-        "unittest",
-        "typing_extensions",
+        "numpy",
         "builtins",
+        "_typeshed",
         "abc",
-        "typing"
+        "array",
+        "ctypes",
+        "mmap",
+        "numpy._typing",
+        "numpy._typing._array_like",
+        "numpy._typing._dtype_like",
+        "numpy._typing._nested_sequence",
+        "pickle",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
-    "id": "unittest.suite",
-    "ignore_all": true,
-    "interface_hash": "9916fb1e8b3be752543760164ef567d207764e60d25de2267f89a51f85553ad7",
-    "mtime": 1684343449,
+    "hash": "d910411f8c5c3ef54ae6be480f0b5fcb37a062eecae7b0ba5ee54b056a6a0d77",
+    "id": "symgt.group_testing",
+    "ignore_all": false,
+    "interface_hash": "bd659cc6e1e98ccefb27d92580ac9837431d431836c4b87f1f04300199b09ecd",
+    "mtime": 1684471017,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/Users/nicholascharleslandolfi/workspace/symgt/symgt_env/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
+    "path": "src/symgt/group_testing.py",
     "plugin_data": null,
-    "size": 983,
+    "size": 1463,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.1/src/.DS_Store` & `symgt-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/src/symgt/models.py` & `symgt-0.0.2/src/symgt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
         if not isinstance(n, int):
             raise TypeError("`n` should be a positive integer.")
         if n <= 0:
             raise ValueError("`n` should be a positive integer.")
         if len(alpha) != n + 1:
             raise ValueError("len of `alpha` should be `n+1`.")
-        if not np.allclose(np.sum(alpha), 1.):
+        if not np.allclose(np.sum(alpha), 1.0):
             raise ValueError("`np.sum(alpha)` should be `1`.")
 
         self.n = n
         self.alpha = np.asarray(alpha).astype(np.float64)
 
     def __str__(self):
         return f"ExchangeableModel(n={self.n}, alpha=...)"
```

### Comparing `symgt-0.0.1/tests/01_smoke_test:_IIDModel.py` & `symgt-0.0.2/tests/01_smoke_test:_IIDModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/tests/02_smoke_test:_ExchangeableModel.py` & `symgt-0.0.2/tests/02_smoke_test:_ExchangeableModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.1/pyproject.toml` & `symgt-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "symgt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "N. C. Landolfi", email="crews.fixture.0f@icloud.com"},
 ]
 description = "A package for group testing against symmetric distributions."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `symgt-0.0.1/PKG-INFO` & `symgt-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: symgt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for group testing against symmetric distributions.
 Project-URL: Homepage, https://github.com/nlandolfi/symgt
 Author-email: "N. C. Landolfi" <crews.fixture.0f@icloud.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # symgt
 
-The symgt python package. Only Python 3.
+A package for group testing against symmetric distributions. Python 3.
 
 ```
 pip install symgt
 ```
```

