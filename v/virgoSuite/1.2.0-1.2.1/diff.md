# Comparing `tmp/virgoSuite-1.2.0.tar.gz` & `tmp/virgoSuite-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgoSuite-1.2.0.tar", last modified: Thu May 18 21:53:11 2023, max compression
+gzip compressed data, was "virgoSuite-1.2.1.tar", last modified: Thu May 18 22:06:29 2023, max compression
```

## Comparing `virgoSuite-1.2.0.tar` & `virgoSuite-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.344264 virgoSuite-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.344264 virgoSuite-1.2.0/src/virgoSuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24735 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/sfdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-05-18 21:52:46.000000 virgoSuite-1.2.0/src/virgoSuite/sfdbV2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:53:11.348264 virgoSuite-1.2.0/src/virgoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 21:53:11.000000 virgoSuite-1.2.0/src/virgoSuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:06:29.844771 virgoSuite-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 22:06:12.000000 virgoSuite-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 22:06:29.844771 virgoSuite-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 22:06:12.000000 virgoSuite-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:06:29.844771 virgoSuite-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 22:06:12.000000 virgoSuite-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:06:29.840772 virgoSuite-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:06:29.844771 virgoSuite-1.2.1/src/virgoSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 22:06:12.000000 virgoSuite-1.2.1/src/virgoSuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-05-18 22:06:12.000000 virgoSuite-1.2.1/src/virgoSuite/sfdbV2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:06:29.844771 virgoSuite-1.2.1/src/virgoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 22:06:29.000000 virgoSuite-1.2.1/src/virgoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 22:06:29.000000 virgoSuite-1.2.1/src/virgoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:06:29.000000 virgoSuite-1.2.1/src/virgoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 22:06:29.000000 virgoSuite-1.2.1/src/virgoSuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 22:06:29.000000 virgoSuite-1.2.1/src/virgoSuite.egg-info/top_level.txt
```

### Comparing `virgoSuite-1.2.0/LICENSE` & `virgoSuite-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `virgoSuite-1.2.0/setup.py` & `virgoSuite-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `virgoSuite-1.2.0/src/virgoSuite/sfdb.py` & `virgoSuite-1.2.1/src/virgoSuite/sfdbV2.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,33 +15,26 @@
 # version 2, released 12 May 2017
 # installation instructions:
 # http://grwavsf.roma1.infn.it/snag/Snag2_UG.pdf
 
 import numpy as np
 import pandas
 import astropy.time
-import xarray
-import zarr
-from dask import delayed
 
 import os
 
 from fnmatch import fnmatch
 from pathlib import Path
 from typing import TextIO
 
-import matplotlib.pyplot as plt
-from tqdm.contrib.telegram import tqdm, trange
-import string
-from dask.diagnostics import ProgressBar
-
-
 import random
 import string
 
+import h5py
+
 
 def get_random_string(length: int) -> str:
     # choose from all lowercase letter
     letters = string.ascii_letters
     result_str = "".join(random.choice(letters) for i in range(length))
     return result_str
 
@@ -90,17 +83,17 @@
         return None
     elif n_elements == 1:
         out_variable = data_array[0]
     else:
         out_variable = data_array
 
     if (dt == "int") or (dt == "int32"):
-        return out_variable.astype("int32")
+        return out_variable.astype("int64")
     elif dt in ["float32", "double", "float", "float64", "single"]:
-        return out_variable.astype("float32")
+        return out_variable.astype("double")
 
 
 # =============================================================================
 # =============================================================================
 
 
 def read_block(fid: TextIO) -> tuple[dict, np.ndarray, np.ndarray, np.ndarray]:
@@ -219,17 +212,17 @@
 
     det = fread(fid, 1, "int32")  # detector
     if det == 0:
         detector = "Nautilus"
     elif det == 1:
         detector = "Virgo"
     elif det == 2:
-        detector = "Hanford"
+        detector = "Ligo Hanford"
     elif det == 3:
-        detector = "Livingston"
+        detector = "Ligo Livingston"
 
     gps_seconds = fread(fid, 1, "int32")  # gps_sec
     gps_nanoseconds = fread(fid, 1, "int32")  # gps_nsec
     gps_time = gps_seconds + gps_nanoseconds * 1e-9
 
     fft_lenght = fread(fid, 1, "double")  # tbase
     starting_fft_sample_index = fread(fid, 1, "int32")  # firstfrind
@@ -331,35 +324,29 @@
         "fft_index": fft_index,
         "window_type": window_type,
         "normalization_factor": normalization_factor,
         "window_normalization": window_normalization,
         "starting_fft_frequency": starting_fft_frequency,
         "subsampling_time": subsampling_time,
         "frequency_resolution": frequency_resolution,
-        "x": x,
-        "y": y,
-        "z": z,
-        "v_x": v_x,
-        "v_y": v_y,
-        "v_z": v_z,
+        "position": np.array([x, y, z]),
+        "velocity": np.array([v_x, v_y, v_z]),
         "number_of_zeroes": number_of_zeroes,
         "sat_howmany": sat_howmany,
         "spare1": spare1,
         "spare2": spare2,
         "spare3": spare3,
         "percentage_of_zeroes": percentage_of_zeroes,
         "spare5": spare5,
         "spare6": spare6,
         "lenght_of_averaged_time_spectrum": lenght_of_averaged_time_spectrum,
         "scientific_segment": scientific_segment,
-        "spare1": spare1,
+        "spare9": spare9,
     }
 
-    header = pandas.DataFrame.from_dict([header])
-
     if lenght_of_averaged_time_spectrum > 0:
         lsps = lenght_of_averaged_time_spectrum
         # This was tps
         periodogram = fread(
             fid,
             lsps,
             "float32",
@@ -387,231 +374,199 @@
     )
     fft_data = _[0::2] + 1j * _[1::2]
 
     # Here is important to specify to export data as float, otherwise the
     # precision will not be enough
     return (
         header,
-        periodogram.astype("float32"),
-        autoregressive_spectrum.astype("float32"),
+        periodogram,
+        autoregressive_spectrum,
         fft_data.astype("complex64"),
     )
 
 
 # =============================================================================
 # =============================================================================
 
 
-def load_file_sfdb(
-    path_to_sfdb: str,
-    # -----Telegram Bot Notifications------
-    telegram_notification: bool = False,
-    token: str = "",
-    chat_id: str = "",
-    # -------------------------------------
-) -> list[xarray.Dataset]:
+def sfdb_to_h5(
+    path_to_sfdb_database: str,
+    save_path: str,
+) -> np.ndarray:
     """
     SFDB to netCDF4
 
     Contert SFDB files into netCDF4.
     netCDF4 is like hdf5 but hadles multidimensional data with more ease.
 
     Parameters
     ----------
-    path_to_sfdb : str
+    path_to_sfdb_database : str
         path to the file.
     save_path : str
         path to save folder
 
     """
-    with open(path_to_sfdb) as fid:
-        if telegram_notification:
-            _range = trange(
-                200,
-                token=token,
-                chat_id=chat_id,
-            )
-        else:
-            _range = range(200)
-        for i in _range:
+    list_of_timestaps_in_block = []
+    with open(path_to_sfdb_database) as fid:
+        for i in range(200):
+            # for i in range(10):  # For test only
             # Any sfdb file contains multiple ffts, check all ffts until EOF
-            head, tps, sps, sft = read_block(fid)
+            (
+                head,
+                periodogram,
+                autoregressive_spectrum,
+                fft_data,
+            ) = read_block(fid)
 
             if head is None:
                 # Checking EOF
                 # This could happen in the case of an interruption in data
                 break
 
-            if i == 0:
-                header = head
-                periodogram = tps
-                autoregressive_spectrum = sps
-                fft_data = sft
-            else:
-                header = pandas.concat([header, head], ignore_index=True)
-                periodogram = np.vstack((periodogram, tps))
-                autoregressive_spectrum = np.vstack((autoregressive_spectrum, sps))
-                fft_data = np.vstack((fft_data, sft))
-
-    # ============================================
-    # Preparing data to be saved in the new format
-    # ============================================
-    data_frequencies = (
-        np.arange(
-            start=0,
-            stop=fft_data.shape[1],
-            step=1,
-            dtype=int,
-        )
-        * header.frequency_resolution[0]
-    )
-    spectrum_frequencies = (
-        np.arange(
-            start=0,
-            stop=periodogram.shape[1],
-            step=1,
-            dtype=int,
-        )
-        * header.frequency_resolution[0]
-        * header.reduction_factor[0]
-    )
+            fft_frequencies = (
+                np.arange(
+                    start=0,
+                    stop=len(fft_data),
+                    step=1,
+                    dtype=int,
+                )
+                * head["frequency_resolution"]
+            )
 
-    total_normalization = (
-        np.sqrt(2)
-        * header.normalization_factor
-        * header.window_normalization
-        / np.sqrt(1 - header.percentage_of_zeroes)
-    )
-    power_spectrum = np.square(
-        np.abs(np.einsum("ij, i -> ij", fft_data, total_normalization))
-    )
-    power_spectrum = np.einsum(
-        "ij, i -> ij", power_spectrum, header.scaling_factor**2
-    )
+            spectrum_frequencies = (
+                np.arange(
+                    start=0,
+                    stop=len(periodogram),
+                    step=1,
+                    dtype=int,
+                )
+                * head["frequency_resolution"]
+                * head["reduction_factor"]
+            )
 
-    # float64 slows down computation and cannot be handled by GPU
-    # so we are forced to take into account the possibility of overflow
-    # and truncation errors (RuntimeWarning: overflow)
-    # replace the eventual infinities with the maximum float32 number
-    power_spectrum[np.isinf(power_spectrum)] = np.finfo(
-        np.float32
-    ).max  # float32_max = 3.4028235e+38
-
-    # autoregressive_spectrum and periodogram are stored in sfdbs
-    # as square roots, so we need to make the square of them
-    autoregressive_spectrum = np.square(
-        np.einsum("ij, i -> ij", autoregressive_spectrum, header.scaling_factor)
-    )
-    periodogram = np.square(
-        np.einsum("ij, i -> ij", periodogram, header.scaling_factor)
-    )
+            total_normalization = (
+                np.sqrt(2)
+                * head["normalization_factor"]
+                * head["window_normalization"]
+                / np.sqrt(1 - head["percentage_of_zeroes"])
+            )
+            power_spectrum = np.square(np.abs(fft_data * total_normalization))
+            power_spectrum = power_spectrum * head["scaling_factor"] ** 2
 
-    # untill now, we have filtered and selected frequencies. so it was
-    # useful to have the main axis of the matrices on the dimension
-    # "frequency" from here on, we will need to iterate over "time".
-    # so it's useful to transpose everything
-    power_spectrum = np.transpose(power_spectrum)
-    autoregressive_spectrum = np.transpose(autoregressive_spectrum)
-    periodogram = np.transpose(periodogram)
-
-    # given the fact that out current data are really dirty, we place
-    # a condition on the median of the autoregressive spectrum, to be sure
-    # that it lies in the correct range.
-    # the periodogram can be higher than the autoregressive spectrum, because
-    # it suffers when there are bumps and unwanted impulses in the time domain
-    # the median is more robust than the average
-    autoregressive_spectrum_median = np.median(autoregressive_spectrum, axis=1)
-
-    # autoregressive_spectrum and periodogram must be more or less the
-    # same in this flat area they are different in the peaks, because by
-    # construction the autoregressive mean ignores them
-    # the autoregressive_spectrum can follow the noise nonstationarities
-    periodogram_median = np.median(periodogram, axis=1)
-
-    # HANDLING TIME
-    gps_time = astropy.time.Time(
-        val=header.gps_time,
-        format="gps",
-        scale="utc",
-    )
-    # ISO 8601 compliant date-time format: YYYY-MM-DD HH:MM:SS.sss
-    iso_time_values = gps_time.iso
-    # time of the first FFT of this file
-    human_readable_start_time = iso_time_values[0]
-    datetimes = pandas.to_datetime(iso_time_values)
-
-    # ================
-    # Saving to xarray
-    # ================
-    coordinate_names = ["detector", "time", "frequency"]
-    attributes = {
-        "FFT_lenght": header.fft_lenght[0],
-        "observing_run": "O3",  # TODO Remove hard coding
-        "calibration": "C01",  # TODO Remove hard coding
-        "start_ISO_time": str(human_readable_start_time),
-    }
+            # float64 slows down computation and cannot be handled by GPU
+            # so we are forced to take into account the possibility of overflow
+            # and truncation errors (RuntimeWarning: overflow)
+            # replace the eventual infinities with the maximum float32 number
+            power_spectrum[np.isinf(power_spectrum)] = np.finfo(
+                np.float32
+            ).max  # float32_max = 3.4028235e+38
+
+            # autoregressive_spectrum and periodogram are stored in sfdbs
+            # as square roots, so we need to make the square of them
+            autoregressive_spectrum = np.square(
+                autoregressive_spectrum * head["scaling_factor"]
+            )
+            periodogram = np.square(periodogram * head["scaling_factor"])
 
-    data_coordinate_values = [
-        [header.detector[0]],
-        datetimes,
-        data_frequencies,
-    ]
-    spectrum_coordinate_values = [
-        [header.detector[0]],
-        datetimes,
-        spectrum_frequencies,
-    ]
-
-    periodogram = xarray.DataArray(
-        data=np.expand_dims(np.transpose(periodogram), axis=0),
-        dims=coordinate_names,
-        coords=spectrum_coordinate_values,
-    )
-    autoregressive_spectrum = xarray.DataArray(
-        data=np.expand_dims(np.transpose(autoregressive_spectrum), axis=0),
-        dims=coordinate_names,
-        coords=spectrum_coordinate_values,
-    )
-    spectrum_dataset = xarray.Dataset(
-        data_vars={
-            "periodogram": periodogram,
-            "autoregressive_spectrum": autoregressive_spectrum,
-        },
-        attrs=attributes,
-    )
+            # given the fact that out current data are really dirty, we place
+            # a condition on the median of the autoregressive spectrum, to be sure
+            # that it lies in the correct range.
+            # the periodogram can be higher than the autoregressive spectrum, because
+            # it suffers when there are bumps and unwanted impulses in the time domain
+            # the median is more robust than the average
+            #
+            # autoregressive_spectrum_median = np.median(autoregressive_spectrum, axis=1)
+
+            # autoregressive_spectrum and periodogram must be more or less the
+            # same in this flat area they are different in the peaks, because by
+            # construction the autoregressive mean ignores them
+            # the autoregressive_spectrum can follow the noise nonstationarities
+            #
+            # periodogram_median = np.median(periodogram, axis=1)
+
+            # HANDLING TIME
+            gps_time = astropy.time.Time(
+                val=head["gps_time"],
+                format="gps",
+                scale="utc",
+            )
+            # ISO 8601 compliant date-time format: YYYY-MM-DD HH:MM:SS.sss
+            iso_time_value = gps_time.isot
+            # time of the first FFT of this file
+            human_readable_start_time = iso_time_value.replace(":", ".")
+            datetimes = pandas.to_datetime(iso_time_value)
+
+            list_of_timestaps_in_block.append(iso_time_value.encode("utf8"))
+
+            # Setting compression level for FFT data files
+            compression_level = 9
+
+            # Creating the subfolder for the raw data and spectrum data
+            data_save_path = save_path + "/data"
+            spectrum_save_path = save_path + "/spectrum"
+
+            Path(data_save_path).mkdir(mode=777, exist_ok=True, parents=True)
+            Path(spectrum_save_path).mkdir(mode=777, exist_ok=True, parents=True)
+
+            # Saving FFT Data in hdf files
+            # =================================================================
+            with h5py.File(
+                f"{data_save_path}/{human_readable_start_time}.hdf5", mode="w"
+            ) as data_file_obj:
+                # Saving FFTs in hdf format with compression
+                fft_dataset = data_file_obj.create_dataset(
+                    "fft_data",
+                    data=fft_data,
+                    compression="gzip",
+                    compression_opts=compression_level,
+                )
 
-    power_spectrum = xarray.DataArray(
-        data=np.expand_dims(np.transpose(power_spectrum), axis=0),
-        dims=coordinate_names,
-        coords=data_coordinate_values,
-    )
+                # Adding time dependent metadata
+                for attribute_key, attribute in head.items():
+                    fft_dataset.attrs[attribute_key] = attribute
+
+            # Saving spectrum data
+            with h5py.File(
+                f"{spectrum_save_path}/{human_readable_start_time}.hdf5", mode="w"
+            ) as spectrum_file_obj:
+                # Spectrum data are stored inside "spectrum" group
+                spectrum = spectrum_file_obj.create_group("spectrum")
 
-    # We need to separate real part and imaginary part,
-    # since netcdf4 doesn't have support for complex numbers
+                periodogram_dset = spectrum.create_dataset(
+                    "periodogram", data=periodogram
+                )
+                ar_spectrum_dset = spectrum.create_dataset(
+                    "autoregressive_spectrum", data=autoregressive_spectrum
+                )
 
-    real_fft_data = xarray.DataArray(
-        data=np.expand_dims(np.real(fft_data), axis=0),
-        dims=coordinate_names,
-        coords=data_coordinate_values,
-    )
-    imag_fft_data = xarray.DataArray(
-        data=np.expand_dims(np.imag(fft_data), axis=0),
-        dims=coordinate_names,
-        coords=data_coordinate_values,
-    )
-    data_dataset = xarray.Dataset(
-        data_vars={
-            "real_fft_data": real_fft_data,
-            "imag_fft_data": imag_fft_data,
-            "power_spectrum": power_spectrum,
-        },
-        attrs=attributes,
-    )
+                # Adding time dependent metadata
+                for attribute_key, attribute in head.items():
+                    spectrum.attrs[attribute_key] = attribute
+
+    # Adding a file with the frequencies of data
+    with h5py.File(
+        f"{data_save_path}/frequencies.hdf5", mode="w"
+    ) as fft_frequencies_file:
+        fft_frequencies_file.create_dataset(
+            "frequencies",
+            data=fft_frequencies,
+            compression="gzip",
+            compression_opts=compression_level,
+        )
+    # Adding a file with the frequencies of spectrum
+    with h5py.File(
+        f"{spectrum_save_path}/frequencies.hdf5", mode="w"
+    ) as spectrum_frequencies_file:
+        spectrum_frequencies_file.create_dataset(
+            "frequencies",
+            data=spectrum_frequencies,
+        )
 
-    return data_dataset, spectrum_dataset
+    return list_of_timestaps_in_block
 
 
 # =============================================================================
 # =============================================================================
 
 
 def list_sfdb_in_directory(path: str) -> list:
@@ -627,127 +582,58 @@
     return file_names
 
 
 # =============================================================================
 # =============================================================================
 
 
-def convert_sfdb(
-    path_to_sfdb: str,
+def convert_sfdb_database(
+    path_to_sfdb_database: str,
     output_path: str,
-    output_database_format: list = "all",
-    telegram_notifications: bool = False,
-    token: str = "",
-    chat_id: str = "",
-    compression: bool = False,
 ) -> None:
     # First we check whether a directory or a file are provided
-    is_a_File = os.path.isfile(path_to_sfdb)
-    is_a_directory = os.path.isdir(path_to_sfdb)
+    is_a_File = os.path.isfile(path_to_sfdb_database)
+    is_a_directory = os.path.isdir(path_to_sfdb_database)
     if (not is_a_File) and (not is_a_directory):
         raise TypeError("Please check the path to the sfdb database.")
 
-    # Supported save type
-    supported_save_formats = [
-        "zarr",
-        "Zarr",
-        "ZARR",
-        "netcdf",
-        "netCDF4",
-        "CDF4",
-        "all",
-    ]
-
-    if output_database_format not in supported_save_formats:
-        raise Exception(
-            f"Save format not supported yet!\nPlease select a valid format from the following list:\n{supported_save_formats}"
-        )
-    elif output_database_format == "all":
-        output_database_format = ["zarr", "netcdf"]
-
     # Opening the file (files)
     if is_a_File:
-        file_list = [path_to_sfdb]
+        file_name_list = [path_to_sfdb_database]
     elif is_a_directory:
-        file_list = list_sfdb_in_directory(path_to_sfdb)
-    if len(file_list) == 1:
-        print(f"{len(file_list)} files was found.")
-    elif len(file_list) > 1:
-        print(f"{len(file_list)} files were found.")
+        file_name_list = list_sfdb_in_directory(path_to_sfdb_database)
 
-    print(f"Starting conversion...")
-
-    if telegram_notifications:
-        file_list = tqdm(file_list, token=token, chat_id=chat_id)
-
-    for file in file_list:
-        print(f"Processing : {file}")
-        data, spectrum = load_file_sfdb(
-            file,
-            telegram_notification=telegram_notifications,
-            token=token,
-            chat_id=chat_id,
-        )
+    if len(file_name_list) == 1:
+        print(f"{len(file_name_list)} file was found.")
+    elif len(file_name_list) > 1:
+        print(f"{len(file_name_list)} files were found.")
 
-        calibration = data.calibration
-        run = data.observing_run
-
-        # Supports multiple save formats
-        if isinstance(output_database_format, str):
-            output_database_format = [output_database_format]
-        elif not isinstance(output_database_format, (list, str)):
-            raise TypeError("Please enter a valid format string or list of strings")
-
-        for save_format in output_database_format:
-            if (
-                (save_format == "zarr")
-                or (save_format == "Zarr")
-                or (save_format == "ZARR")
-            ):
-                print("Support for zarr has been haulted.")
-                print("Skipping.")
-                """
-
-                save_path = output_path + f"/DATABASE/zarr/fft_data.zarr"
-                save_path = zarr.storage.NestedDirectoryStore(
-                    path=save_path, dimension_separator="/"
-                )
-                data.to_zarr(
-                    save_path,
-                    mode="w",
-                )
-
-                save_path = output_path + f"/DATABASE/zarr/spectrum.zarr"
-                save_path = zarr.storage.NestedDirectoryStore(
-                    path=save_path, dimension_separator="/"
-                )
-                spectrum.to_zarr(
-                    save_path,
-                    mode="w",
-                )"""
-
-            elif (
-                (save_format == "netCDF4")
-                or (save_format == "CDF4")
-                or (save_format == "netcdf")
-            ):
-                print("Saving to netCDF4...")
-                # encoding = {"gzip": True, "complevel": 9}
-                # encoding = {"gzip": True, "compression_opts": 9}  # h5py
-
-                save_path = output_path + f"/DATABASE/netcdf/{run}/{calibration}/FFT/"
-                Path(save_path).mkdir(parents=True, exist_ok=True)
-                data.to_netcdf(
-                    save_path + f"{get_random_string(15)}.netCDF4",
-                    mode="w",
-                    engine="netcdf4",
-                )
+    print(f"Starting conversion...")
 
-                save_path = (
-                    output_path + f"/DATABASE/netcdf/{run}/{calibration}/SPECTRUM/"
-                )
-                Path(save_path).mkdir(parents=True, exist_ok=True)
-                spectrum.to_netcdf(
-                    save_path + f"{get_random_string(15)}.netCDF4",
-                    mode="w",
-                    engine="netcdf4",
-                )
+    timestamp_list_database = [0] * len(file_name_list)
+    for j, file_name in enumerate(file_name_list):
+        print(f"Processing : {file_name}")
+
+        print("Extracting data from path...")
+        print("Please make sure that the path to the files is:")
+        print("/*/*/[detector]/sfdb/[run]/[calibration]/[cleaning]/*/[sfdb-files]")
+        print("or")
+        print("/*/*/[detector]/sfdb/[run]/[calibration]/*/[sfdb-files]")
+
+        path_splitted = file_name.strip("\n").split("/")
+        detector = str(path_splitted[path_splitted.index("sfdb") - 1])
+        run = str(path_splitted[path_splitted.index("sfdb") + 1])
+        calibration = str(path_splitted[path_splitted.index("sfdb") + 2])
+
+        save_path = output_path + f"/{detector}/hdf5/{run}/{calibration}"
+
+        if len(path_splitted) > 8:
+            cleaning = str(path_splitted[path_splitted.index("sfdb") + 3])
+            save_path = save_path + f"{cleaning}"
+
+        Path(save_path).mkdir(mode=777, exist_ok=True, parents=True)
+        timestap_list_block = sfdb_to_h5(file_name, save_path=save_path)
+        timestamp_list_database[j] = timestap_list_block
+
+    timestamp_list_database = np.concatenate(timestamp_list_database)
+    with h5py.File(save_path + "/timeseries.hdf", "w") as timeseries_file:
+        timeseries_file.create_dataset("times", data=timestamp_list_database)
```

