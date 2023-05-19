# Comparing `tmp/pypiwrap-0.3.0.tar.gz` & `tmp/pypiwrap-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypiwrap-0.3.0.tar", last modified: Wed Nov  2 02:24:49 2022, max compression
+gzip compressed data, was "pypiwrap-1.0.0.tar", last modified: Fri May 19 20:55:58 2023, max compression
```

## Comparing `pypiwrap-0.3.0.tar` & `pypiwrap-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 02:24:49.925030 pypiwrap-0.3.0/
--rw-rw-rw-   0        0        0     1091 2022-09-16 14:49:10.000000 pypiwrap-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1726 2022-11-02 02:24:49.925030 pypiwrap-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      836 2022-10-22 17:47:35.000000 pypiwrap-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-02 02:24:49.818104 pypiwrap-0.3.0/pypiwrap/
--rw-rw-rw-   0        0        0      371 2022-10-22 17:52:35.000000 pypiwrap-0.3.0/pypiwrap/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-10-29 03:00:41.000000 pypiwrap-0.3.0/pypiwrap/client.py
--rw-rw-rw-   0        0        0      824 2022-10-29 02:59:11.000000 pypiwrap-0.3.0/pypiwrap/exceptions.py
--rw-rw-rw-   0        0        0     9044 2022-10-28 04:35:49.000000 pypiwrap-0.3.0/pypiwrap/objects.py
--rw-rw-rw-   0        0        0     1894 2022-10-28 04:37:42.000000 pypiwrap-0.3.0/pypiwrap/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:24:49.890683 pypiwrap-0.3.0/pypiwrap.egg-info/
--rw-rw-rw-   0        0        0     1726 2022-11-02 02:24:49.000000 pypiwrap-0.3.0/pypiwrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2022-11-02 02:24:49.000000 pypiwrap-0.3.0/pypiwrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 02:24:49.000000 pypiwrap-0.3.0/pypiwrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-11-02 02:24:49.000000 pypiwrap-0.3.0/pypiwrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-02 02:24:49.000000 pypiwrap-0.3.0/pypiwrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      814 2022-11-02 02:24:49.928024 pypiwrap-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-10-22 17:54:13.000000 pypiwrap-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:55:58.874885 pypiwrap-1.0.0/
+-rw-rw-rw-   0        0        0     1096 2023-05-14 03:36:05.000000 pypiwrap-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3061 2023-05-19 20:55:58.869895 pypiwrap-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-05-19 20:00:08.000000 pypiwrap-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 20:55:58.763844 pypiwrap-1.0.0/pypiwrap/
+-rw-rw-rw-   0        0        0      223 2023-05-19 02:41:25.000000 pypiwrap-1.0.0/pypiwrap/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-05-19 20:05:16.000000 pypiwrap-1.0.0/pypiwrap/client.py
+-rw-rw-rw-   0        0        0     1138 2023-05-18 03:25:19.000000 pypiwrap-1.0.0/pypiwrap/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:55:58.852936 pypiwrap-1.0.0/pypiwrap/objects/
+-rw-rw-rw-   0        0        0      113 2023-05-16 04:05:47.000000 pypiwrap-1.0.0/pypiwrap/objects/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-05-15 23:46:04.000000 pypiwrap-1.0.0/pypiwrap/objects/base.py
+-rw-rw-rw-   0        0        0     7507 2023-05-19 04:20:57.000000 pypiwrap-1.0.0/pypiwrap/objects/pypi.py
+-rw-rw-rw-   0        0        0     2641 2023-05-19 02:56:28.000000 pypiwrap-1.0.0/pypiwrap/objects/simple.py
+-rw-rw-rw-   0        0        0     2157 2023-05-15 23:30:18.000000 pypiwrap-1.0.0/pypiwrap/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:55:58.826061 pypiwrap-1.0.0/pypiwrap.egg-info/
+-rw-rw-rw-   0        0        0     3061 2023-05-19 20:55:58.000000 pypiwrap-1.0.0/pypiwrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-05-19 20:55:58.000000 pypiwrap-1.0.0/pypiwrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 20:55:58.000000 pypiwrap-1.0.0/pypiwrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-19 20:55:58.000000 pypiwrap-1.0.0/pypiwrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 20:55:58.000000 pypiwrap-1.0.0/pypiwrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      968 2023-05-19 20:38:34.000000 pypiwrap-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 20:55:58.875879 pypiwrap-1.0.0/setup.cfg
```

### Comparing `pypiwrap-0.3.0/LICENSE` & `pypiwrap-1.0.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ángel Carias
+Copyright (c) 2021-2023 Ángel Carias
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pypiwrap-0.3.0/README.md` & `pypiwrap-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # pypiwrap
 
 ![PyPi - Downloads](https://img.shields.io/pypi/dw/pypiwrap?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/pypiwrap?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/aescarias/pypiwrap?style=flat-square)
-![Lines of code](https://img.shields.io/tokei/lines/github/aescarias/pypiwrap?style=flat-square)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pypiwrap?style=flat-square)
 
-A simple API wrapper for the Python Package Index (PyPi).
+A simple API wrapper for the Python Package Index (PyPI), including a simple interface to get project and release data.
 
-It includes a minimal interface for users to get information about Python packages.
+- [Documentation](https://aescarias.github.io/pypiwrap)
+- [PyPI](https://pypi.org/project/pypiwrap)
 
 ## Installation
 
-Install `pypiwrap` via `pip` by using `pip install pypiwrap` or equivalent methods.
+**Python 3.7 or higher is required.**
+
+Install `pypiwrap` through `pip`:
+
+- On Linux/macOS, `python3 -m pip install pypiwrap`
+- On Windows, `py -3 -m pip install pypiwrap`
 
 ## Example
 
 ```py
 import pypiwrap
 
-wrap = pypiwrap.Client()
+wrap = pypiwrap.PyPIClient()
 project = wrap.get_project("requests")
 
 print(project.name) # requests
 print(project.author) # Kenneth Reitz
 print(project.summary) # Python HTTP for Humans.
 ```
```

### Comparing `pypiwrap-0.3.0/pypiwrap/objects.py` & `pypiwrap-1.0.0/pypiwrap/objects/pypi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,31 @@
 from __future__ import annotations
-
-from datetime import datetime
 from dataclasses import dataclass
+from datetime import datetime
+from typing import Any
 
-from . import utils 
-from .utils import Size
-
-
-class Base:
-    """The base class for other pypiwrap objects"""
-    
-    @classmethod
-    def _from_raw(cls, data: dict):
-        return cls(**utils.remove_additional(cls, data.copy()))
-    
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def _build_repr(self, *args, **kwargs) -> str:
-        arg_string = " ".join(map(repr, args))
-        kwarg_string = " ".join(f"{k}={repr(v)}" for k, v in kwargs.items())
-        final = (self.__class__.__name__, arg_string, kwarg_string)
-
-        return "<" + ' '.join(filter(None, final)).strip() + ">"
+from .base import APIObject
+from ..utils import Size, iso_to_datetime, remove_additional
     
 
 @dataclass
-class Project(Base):
+class Project(APIObject):
     """A PyPi project"""
 
     author: str
     """The author of the project"""
 
     author_email: str
     """The email of the project's author"""
 
     bugtrack_url: str | None
     """A bug tracking URL if available"""
 
     classifiers: list[str]
-    """A list of PyPi classifiers for the project.
-    Valid values are provided at https://pypi.org/classifiers.
-    """
+    """A list of PyPi [classifiers](https://pypi.org/classifiers) for this project"""
 
     description: str
     """A description of the project"""
     
     description_content_type: str | None
     """The content type of the description if available"""
 
@@ -73,55 +53,54 @@
     name: str
     """The name of the project"""
 
     package_url: str
     """The PyPi package URL"""
 
     platform: str | None
-    """The release's platform target if any specifically"""
+    """The release's platform target if any specified"""
 
     project_urls: dict[str, str]
-    """A mapping of URLs relating to the project"""
+    """A mapping of labels to URLs relating to the project"""
 
     project_url: str
     """The PyPi project's URL"""
 
     release_url: str
     """The project URL relating to this specific release"""
 
     requires_dist: list[str]
     """A list of required distributions or dependencies in a format similar to a requirements file"""
 
     requires_python: str | None
-    """The version required for this release"""
+    """The Python version required for this release"""
 
     summary: str
     """A short summary of the project"""
 
     version: str
     """The version of the project"""
 
     yanked: bool
     """Whether this release was 'yanked' or removed from circulation"""
 
     yanked_reason: str | None
     """The reason the release was yanked if applicable"""
 
     file_urls: list[ReleaseFile]
-    """A list of file URLs for this release"""
+    """A list of files for this release"""
 
     vulnerabilities: list[Vulnerability]
     """A list of vulnerabilities for this release if any"""
 
     last_serial: int
 
     @classmethod
     def _from_raw(cls, data: dict) -> Project:
-        data = data.copy()
-        info = utils.remove_additional(cls, data["info"])
+        info = remove_additional(cls, data["info"].copy())
 
         vulns = list(map(Vulnerability._from_raw, data["vulnerabilities"]))
         files = list(map(ReleaseFile._from_raw, data["urls"]))
 
         if not data["info"].get("requires_dist"):
             data["info"]["requires_dist"] = []
 
@@ -136,24 +115,64 @@
             summary=self.summary, 
             version=self.version, 
             package_url=self.package_url
         )
 
 
 @dataclass
-class ReleaseFile(Base):
+class Vulnerability(APIObject):
+    """A vulnerability in a project or release"""
+
+    aliases: list[str]
+    """The names used to refer to this vulnerability"""
+
+    details: str
+    """Details about the vulnerability"""
+
+    fixed_in: list[str]
+    """Releases where this vulnerability was fixed"""
+
+    id: str
+    """Identifier for this vulnerability"""
+    
+    link: str
+    """An URL where more information is provided about the vulnerability"""
+    
+    source: str
+    """The source from where this vulnerability report was obtained"""
+
+    summary: str | None
+    """A short summary of the vulnerability if available"""
+
+    withdrawn: datetime | None = None
+    """The datetime this vulnerability was withdrawn"""
+
+    @classmethod
+    def _from_raw(cls, data: dict) -> Vulnerability:
+        if data.get("withdrawn") is not None:
+            data["withdrawn"] = iso_to_datetime(data["withdrawn"])
+
+        return cls(**remove_additional(cls, data))
+    
+    def __repr__(self) -> str:
+        return self._build_repr(id=self.id, source=self.source, withdrawn=self.withdrawn)
+    
+
+@dataclass
+class ReleaseFile(APIObject):
     """A file part of a release"""
 
     comment_text: str
     """A comment for this release"""
 
     digests: dict[str, str]
     """A mapping of hashes corresponding to this release file.
 
-    The keys available can vary but should always members of ``hashlib.algorithms_guaranteed``
+    Most commonly, the digests available are ``md5``, ``sha256``, and ``blake2b_256``. 
+    The keys available must be members of :attr:`hashlib.algorithms_guaranteed`.
     """
     
     # downloads: int
     # md5_digest: str
 
     filename: str
     """The filename for this release file"""
@@ -161,156 +180,83 @@
     has_sig: bool
     """Whether this release file has a PGP signature attached to it"""
 
     package_type: str  # API: packagetype
     """The type of release file. It can be either of:
     
     - ``sdist``: A source distribution (generally a .tar.gz file)
-    - ``bdist_*``: A built distribution where `*` is generally `wheel` or `egg`
+    - ``bdist_*``: A built distribution where `*` is either `wheel` or `egg`
     """
 
     python_version: str
     """The general Python version target for this file.
     
     It is `source` for source distributions and a version target for built distributions.
     """
 
     requires_python: str
-    """The required version constraints for this file"""
+    """The Python version constraints for this file"""
 
     size: Size
     """The size of the release file"""
 
     upload_time: datetime
     """The time this file was uploaded on"""
     
     upload_time_tz: datetime # API: upload_time_iso_8601
-    """The time this file was uploaded on in a format compliant with ISO 8601 and in UTC"""
+    """The time this file was uploaded on in UTC and compliant with ISO 8601"""
 
     url: str
     """The URL for this release file"""
 
     yanked: bool
-    """Whether this package has been yanked"""
+    """Whether this package was yanked"""
 
     yanked_reason: str | None
-    """If the package was yanked, the reason for such"""
+    """Why the package was yanked if applicable"""
 
     @classmethod
     def _from_raw(cls, data: dict) -> ReleaseFile:
         data = data.copy()
 
         # Converting values to appropriate types
-        data["size"] = Size.from_bytes(data["size"])
-        data["upload_time_iso_8601"] = utils.iso_to_datetime(data["upload_time_iso_8601"])
+        data["size"] = Size.from_int(data["size"])
+        data["upload_time_iso_8601"] = iso_to_datetime(data["upload_time_iso_8601"])
         data["upload_time"] = datetime.fromisoformat(data["upload_time"])
 
         # Renaming values to appropriate
         data["upload_time_tz"] = data.pop("upload_time_iso_8601")
         data["package_type"] = data.pop("packagetype")
 
-        # Remove unneeded/unimplemented
-        data = utils.remove_additional(cls, data)
-        return cls(**data)
+        return cls(**remove_additional(cls, data))
 
     def __repr__(self) -> str:
         return self._build_repr(self.filename, 
             size=self.size.si, 
             package_type=self.package_type
         )
 
 
 @dataclass
-class Vulnerability(Base):
-    """A vulnerability in a project or release"""
-
-    aliases: str
-    """The names used to refer to this vulnerability"""
-
-    details: str
-    """Details about the vulnerability"""
-
-    fixed_in: list[str]
-    """Releases where this vulnerability was fixed"""
-
-    id: str
-    """Identifier for this vulnerability"""
-    
-    link: str
-    """An URL where more information is provided about the vulnerability"""
-    
-    source: str
-    """The source from where this vulnerability report was obtained"""
-
-    summary: str | None
-    """A short summary of the vulnerability if available"""
-
-    def __repr__(self) -> str:
-        return self._build_repr(id=self.id, source=self.source)
-
-
-@dataclass
-class DistributionFile(Base):
-    """A file for a package distribution"""
-
-    filename: str
-    """The filename of the distribution"""
-
-    url: str
-    """The download URL for the file"""
-
-    hashes: dict[str, str]
-    """A mapping of common hashes for the file. Similar to :attr:`ReleaseFile.digests`."""
-
-    requires_python: str | None = None
-    """If specified, the version constraints for this file"""
-
-    dist_info_metadata: bool | dict[str, str] | None = None
-    """
-    - If a boolean, whether this file has associated metadata
-    - If a dictionary, a mapping of hashes to encoded metadata file hashes
-    """
-
-    has_sig: bool | None = None  # API: gpg_sig
-    """Whether a GPG signature is included with the file"""
-
-    yanked: bool | str | None = None
-    """
-    - If a boolean, represents whether the file was yanked
-    - If a string, represents the yanking reason
-    """
-
-    @classmethod
-    def _from_raw(cls, data: dict) -> DistributionFile:
-        # Certain API attributes, like requires-python, must be converted
-        # to snake_case before unpacking
-        result = { k.replace("-", "_"): v for k, v in data.items() }
-        result["has_sig"] = result.get("gpg_sig")
-
-        return cls(**utils.remove_additional(cls, result))
-
-    def __repr__(self) -> str:
-        return self._build_repr(self.filename, url=self.url)
-
-
-@dataclass
-class Stats(Base):
-    """A PyPi statistics object. It currently only stores the top packages by size."""
+class Stats(APIObject):
+    """Statistics about PyPI"""
 
     total_size: Size
-    """The current size of all packages on PyPi combined"""
-
+    """The total size of all packages on PyPI combined"""
+    
     top_packages: dict[str, Size]
-    """The packages with the largest sizes"""
-
+    """Mapping of top packages sorted by size"""
+    
     @classmethod
-    def _from_raw(cls, data: dict) -> Stats:
-        size = Size.from_bytes(data["total_packages_size"])
-        pkgs = { 
-            k: Size.from_bytes(v["size"]) 
-            for k, v in data["top_packages"].items() 
-        }
- 
-        return cls(size, pkgs)
+    def _from_raw(cls, data: dict[str, Any]) -> Stats:
+        top_pkgs_sort = sorted(data["top_packages"].items(), 
+                               key=lambda it: it[1]["size"])
+
+        top_pkgs = { name: Size.from_int(pkg["size"]) for name, pkg in top_pkgs_sort } 
+        
+        return cls(
+            total_size=Size.from_int(data["total_packages_size"]),
+            top_packages=top_pkgs   
+        )
     
     def __repr__(self) -> str:
-        return self._build_repr(total_size=self.total_size)
+        return self._build_repr(total_size=self.total_size.si)
```

### Comparing `pypiwrap-0.3.0/pypiwrap/utils.py` & `pypiwrap-1.0.0/pypiwrap/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,40 +10,46 @@
 IEC_SUFFIXES = ["B", "KiB", "MiB", "GiB", "TiB"]
 
 
 class Size(NamedTuple):
     """A tuple that includes human-readable representations of a file size"""
 
     bytes: int
+    """The size represented in bytes"""
     iec: str
-    """The size represented with an IEC prefix (KiB, MiB)"""
+    """The size represented in binary/IEC units (KiB, MiB)"""
     si: str
-    """The size represented with an SI prefix (KB, MB)"""
+    """The size represented in decimal/SI units (KB, MB)"""
 
     @classmethod
-    def from_bytes(cls, num: int) -> Size:
+    def from_int(cls, num: int) -> Size:
         return Size(
             num, 
             iec=bytes_to_readable(num, 'iec'), 
             si=bytes_to_readable(num, 'si')
         )
 
+    def __int__(self) -> int:
+        return self.bytes
+
 
 def iso_to_datetime(iso: str) -> datetime:
+    """Convert an ISO 8601 string to a datetime object"""
     return datetime.strptime(iso, "%Y-%m-%dT%H:%M:%S.%f%z")
 
 def gpg_from_url(url: str) -> str | None:
     """Gets the GPG signature of a file from its URL if available"""
 
     rs = requests.get(url + ".asc")
     if rs.ok:
         return rs.text
 
 # where unit is either of 'si' or 'iec'
 def bytes_to_readable(num: float, unit: str = 'si') -> str:
+    """Converts a number (in bytes) to a human-readable string representation"""
     if unit == 'iec':
         suffixes = IEC_SUFFIXES
         step_unit = 1024
     else:
         suffixes = SI_SUFFIXES
         step_unit = 1000
 
@@ -52,15 +58,15 @@
     for suffix in suffixes:
         if num < step_unit:
             break
         num /= step_unit
     
     return f"{num:.2f} {suffix or suffixes[-1]}"
 
-def remove_additional(cls: type[Any], data: dict) -> dict:
+def remove_additional(cls: type[Any], data: dict[str, Any]) -> dict[str, Any]:
     """Takes any dataclass and a dictionary that can unpack to it
     and strips any additional keys not part of the dataclass"""
 
     result = data.copy()
     names = [field.name for field in dataclasses.fields(cls)]
 
     for key in data:
```

