# Comparing `tmp/dspawpy-0.9.3-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 72759 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat       21 b- defN 23-May-11 06:58 dspawpy/__init__.py
+Zip file size: 72830 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat       22 b- defN 23-May-19 03:15 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    29208 b- defN 23-Apr-25 05:34 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    21567 b- defN 23-May-11 06:31 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
 -rw-rw-rw-  2.0 fat     3592 b- defN 23-Apr-26 09:25 dspawpy/diffusion/neb.py
 -rw-rw-rw-  2.0 fat    53467 b- defN 23-Apr-26 09:25 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-Apr-25 05:34 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    52495 b- defN 23-May-11 06:32 dspawpy/io/read.py
+-rw-rw-rw-  2.0 fat    53127 b- defN 23-May-19 03:14 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-25 05:46 dspawpy/io/read_json.py
--rw-rw-rw-  2.0 fat    10343 b- defN 23-May-11 06:32 dspawpy/io/structure.py
--rw-rw-rw-  2.0 fat    25241 b- defN 23-Apr-26 09:44 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    25401 b- defN 23-May-11 06:32 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-May-19 03:14 dspawpy/io/structure.py
+-rw-rw-rw-  2.0 fat    25239 b- defN 23-May-15 08:44 dspawpy/io/utils.py
+-rw-rw-rw-  2.0 fat    25391 b- defN 23-May-17 10:21 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1761 b- defN 23-Apr-25 05:51 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     2496 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1583 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/RECORD
-20 files, 266193 bytes uncompressed, 70209 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat     2496 b- defN 23-May-19 03:16 dspawpy-0.9.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-19 03:16 dspawpy-0.9.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-19 03:16 dspawpy-0.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1583 b- defN 23-May-19 03:16 dspawpy-0.9.4.dist-info/RECORD
+20 files, 267007 bytes uncompressed, 70280 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.9.3.dist-info/METADATA
+Filename: dspawpy-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.3.dist-info/WHEEL
+Filename: dspawpy-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.3.dist-info/top_level.txt
+Filename: dspawpy-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.3.dist-info/RECORD
+Filename: dspawpy-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.3'
+__version__ = "0.9.4"
```

## dspawpy/io/read.py

```diff
@@ -14,15 +14,18 @@
 from pymatgen.electronic_structure.core import Orbital, Spin
 from pymatgen.electronic_structure.dos import CompleteDos, Dos
 from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
 from pymatgen.phonon.dos import PhononDos
 
 
 def get_band_data(
-    band_dir: str, syst_dir: str = None, efermi: float = None
+    band_dir: str,
+    syst_dir: str = None,
+    efermi: float = None,
+    shift_efermi: bool = False,
 ) -> BandStructureSymmLine:
     """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
 
     Parameters
     ----------
     band_dir : str
         能带文件路径，band.h5 / band.json
@@ -53,24 +56,24 @@
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
-            ) = _get_band_data_h5(band, iwan=True)
+            ) = _get_band_data_h5(band, iwan=True, shift_efermi=shift_efermi)
         elif "/BandInfo/NumberOfBand" in raw:
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
-            ) = _get_band_data_h5(band, iwan=False)
+            ) = _get_band_data_h5(band, iwan=False, shift_efermi=shift_efermi)
         else:
             print("BandInfo or WannBandInfo key not found in h5file!")
             return
     elif band_dir.endswith(".json"):
         with open(band_dir, "r") as fin:
             band = json.load(fin)
         if "WannBandInfo" in band.keys():
@@ -82,24 +85,24 @@
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
-            ) = _get_band_data_json(band, syst, iwan=True)
+            ) = _get_band_data_json(band, syst, iwan=True, shift_efermi=shift_efermi)
         elif "BandInfo" in band.keys():
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
-            ) = _get_band_data_json(band, iwan=False)
+            ) = _get_band_data_json(band, iwan=False, shift_efermi=shift_efermi)
         else:
             print("BandInfo or WannBandInfo key not found in json file!")
             return
     else:
         raise TypeError(f"{os.path.abspath(band_dir)} must be h5 or json file!")
 
     if efermi:  # 从h5直接读取的费米能级可能是错的，此时需要用户自行指定
@@ -1121,17 +1124,15 @@
     """
     # load_h5 -> Structure Obj
     lattice = np.asarray(hdf5[key + "/Lattice"]).reshape(3, 3)
     elements = hdf5[key + "/Elements"]
     positions = hdf5[key + "/Position"]
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = hdf5[key + "/CoordinateType"][0] == "Direct"
-
-    # replace '_1' or '_2' with '' in elements
-    # elements = [re.sub(r"_\d", "", e) for e in elements]
+    elements = [re.sub(r"_", "", e) for e in elements]
 
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
 def _get_structure_json(atominfo) -> Structure:
     """For single-step task
     Examples
@@ -1148,18 +1149,20 @@
     positions = []
     for atom in atominfo["Atoms"]:
         elements.append(atom["Element"])
         positions.extend(atom["Position"])
 
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = atominfo["CoordinateType"] == "Direct"
+    elements = [re.sub(r"_", "", e) for e in elements]
+
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
-def _get_band_data_h5(band: dict, iwan=False):
+def _get_band_data_h5(band: dict, iwan=False, shift_efermi=False):
     if iwan:
         bd = "WannBandInfo"
     else:
         bd = "BandInfo"
     number_of_band = band[f"/{bd}/NumberOfBand"][0]
     number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
     if (
@@ -1182,15 +1185,19 @@
             data = band[f"/{bd}/" + spin_key + "/BandEnergies"]
         elif f"/{bd}/" + spin_key + "/Band" in band:
             data = band[f"/{bd}/" + spin_key + "/Band"]
         else:
             print("Band key error")
             return
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-        eigenvals[spin] = band_data
+
+        if shift_efermi:
+            eigenvals[spin] = band_data - efermi
+        else:
+            eigenvals[spin] = band_data
 
     kpoints = np.asarray(band[f"/{bd}/CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
     structure = _get_structure(band, "/AtomInfo")
     labels_dict = {}
@@ -1225,20 +1232,23 @@
                             + str(orbit_index + 1)
                         ]
                         projection[:, :, orbit_index, atom_index] = (
                             np.asarray(project_data)
                             .reshape((number_of_kpoints, number_of_band))
                             .T
                         )
-                projections[spin] = projection
+                if shift_efermi:
+                    projections[spin] = projection - efermi
+                else:
+                    projections[spin] = projection
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
-def _get_band_data_json(band: dict, syst: dict = None, iwan=False):
+def _get_band_data_json(band: dict, syst: dict = None, iwan=False, shift_efermi=False):
     # syst is only required for wannier band structure
     if iwan:
         bd = "WannBandInfo"
         structure = _get_structure_json(syst["AtomInfo"])
     else:
         bd = "BandInfo"
         structure = _get_structure_json(band["AtomInfo"])
@@ -1268,15 +1278,18 @@
             data = band[f"{bd}"][spin_key]["Band"]
         else:
             print("Band key error")
             return
 
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
 
-        eigenvals[spin] = band_data
+        if shift_efermi:
+            eigenvals[spin] = band_data - efermi
+        else:
+            eigenvals[spin] = band_data
 
     kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
     labels_dict = {}
 
@@ -1304,15 +1317,18 @@
                     project_data = d["Contribution"]
                     projection[:, :, orbit_index, atom_index] = (
                         np.asarray(project_data)
                         .reshape((number_of_kpoints, number_of_band))
                         .T
                     )
 
-                projections[spin] = projection
+                if shift_efermi:
+                    projections[spin] = projection - efermi
+                else:
+                    projections[spin] = projection
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
 def _get_phonon_band_data_h5(band: dict):
     number_of_band = band["/BandInfo/NumberOfBand"][0]
     number_of_kpoints = band["/BandInfo/NumberOfQPoints"][0]
```

## dspawpy/io/structure.py

```diff
@@ -1,11 +1,12 @@
 """
 Functions to build structures
 """
 
+import re
 from typing import List, Union
 
 import numpy as np
 from pymatgen.core import Structure
 
 from dspawpy.io.read import get_lines_without_comment, get_sinfo
 
@@ -135,14 +136,17 @@
         strs = [Structure.from_file(df)]
     else:
         assert df.endswith(".h5") or df.endswith(".json"), "expecting h5/json file"
 
         Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
             datafile=df, si=si, ele=ele, ai=ai
         )  # returned positions, not scaled-positions
+        # remove _ from elements
+        elements = [re.sub(r"_", "", e) for e in elements]
+
         strs = []
         for i in range(Nstep):
             if D_mag_fix:
                 strs.append(
                     Structure(
                         lattices[i],
                         elements,
@@ -260,14 +264,16 @@
             mag_fix_dict[item] = values
 
     if lat_fixs != []:
         # replicate lat_fixs to N atoms
         mag_fix_dict["LatticeFixs"] = [lat_fixs for i in range(N)]
 
     coords = np.asarray(positions).reshape(-1, 3)
+    # remove _ from elements
+    elements = [re.sub(r"_", "", e) for e in elements]
 
     if mag_fix_dict == {}:
         return Structure(
             lattice, elements, coords, coords_are_cartesian=(not is_direct)
         )
     else:
         return Structure(
```

## dspawpy/io/utils.py

```diff
@@ -356,15 +356,14 @@
     --------
     >>> from dspawpy.io.utils import IdealGasThermo
     >>> thermo = IdealGasThermo(vib_energies=[0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
     ...                         geometry='linear', potentialenergy=0.,  # eV
     ...                         elements=['H', 'O'], positions=[[0, 0, 0], [0, 0, 1]],  # angstrom
     ...                         symmetrynumber=None, spin=None, Natom=None)
     >>> thermo.get_free_energy(298.15)  # K
-
     """
 
     # 读取elements数组代替atoms
     def __init__(
         self,
         vib_energies,
         geometry,
```

## dspawpy/io/write.py

```diff
@@ -268,16 +268,15 @@
             dataB = json.load(f3)
             rhoB = np.array(dataB["Rho"]["TotalCharge"])
     else:
         raise ValueError(f"file format must be either h5 or json: {B}")
 
     print(f"计算电荷差分...")
     rho = rhoAB - rhoA - rhoB
-    rho = np.array(rho).reshape(shape=(nGrids[0], nGrids[1], nGrids[2]))
-
+    rho = np.array(rho).reshape(nGrids[0], nGrids[1], nGrids[2])
     element = list(set(atom_symbol))
     element = sorted(set(atom_symbol), key=atom_symbol.index)
     element_num = np.zeros(len(element))
     for i in range(len(element)):
         element_num[i] = atom_symbol.count(element[i])
 
     latticeConstantMatrix = np.array(latticeConstantMatrix)
```

## Comparing `dspawpy-0.9.3.dist-info/METADATA` & `dspawpy-0.9.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
```

## Comparing `dspawpy-0.9.3.dist-info/RECORD` & `dspawpy-0.9.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-dspawpy/__init__.py,sha256=c60whb_Zk-Ow7zx5khIRULcdxxjoCXM2XCO4tAZztbk,21
+dspawpy/__init__.py,sha256=e56AvHfJCtG2ZwwINqsxINVbehWdKxMYgIDbjd7P-II,22
 dspawpy/plot.py,sha256=ocLkU08WfMb2fyETrBSSZvxZFSg2sPX8rLusXZLT5BM,29208
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/analysis/aimdtools.py,sha256=72N58P2EBA5z8EZwaY1W6ab8ZGZVwefQCjME8490HqU,21567
 dspawpy/analysis/vacf.py,sha256=g5IS6Q7QGYa17XBVnYEH-MubGSpkUsDPpMaI_ELacw4,20152
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/diffusion/neb.py,sha256=U6J7lSlE_xp1rCON5mgfWWi5DFHVZYVb5xjqLlGxXXI,3592
 dspawpy/diffusion/nebtools.py,sha256=tfQCQPUmZKELz7ImwyiJiiFfXahC9U3doarExspL-DU,53467
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/io/read.py,sha256=jZYWmjTtQde_Za5kbTt206_6w6yieXVx5ZN8Z1YfkWY,52495
+dspawpy/io/read.py,sha256=Cz90LbdguLQdyUl_gBEFn9zodD1zGijktPxPtw1fwFI,53127
 dspawpy/io/read_json.py,sha256=2bcNQP51SR2yMyFE7c2TIutYp93K8IH-dpLmH5yy4bo,7721
-dspawpy/io/structure.py,sha256=7iLLzyoaxRE3bCC1URKpx8QzoAx4CzwFXtA5wxX-jNA,10343
-dspawpy/io/utils.py,sha256=FdbFbZqKfnDOGBJ4OaKD-4IBAAlqjtQ0l1NppvkMKOM,25241
-dspawpy/io/write.py,sha256=-bHzDvE1Vr0x0kxZ8yJGQOmHQTjhkITG9dvUggOnxmU,25401
+dspawpy/io/structure.py,sha256=8W-vsSXA-TGWMdmK4TlihsZLpLfZhGuGSL6YqI_C5uA,10536
+dspawpy/io/utils.py,sha256=ff2182s8KQWQ53bHYdlWuXuN3lkDLAH6zrNub1t_9wA,25239
+dspawpy/io/write.py,sha256=8oQikD6Iyo7Bxy5_1Fl7SaSyZK3o6oBCwC82Raqa9cY,25391
 dspawpy/io/write_json.py,sha256=n3GhdDnFFtW7eY4U5u7czdlpbSWnsGP7WUD5eS1ZmqI,1761
-dspawpy-0.9.3.dist-info/METADATA,sha256=exrAYV7qeKIsMUMvlswVbxc9DIHBdmx4wRcpa1ibx8M,2496
-dspawpy-0.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-0.9.3.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-0.9.3.dist-info/RECORD,,
+dspawpy-0.9.4.dist-info/METADATA,sha256=fk-Ue_De2rX-dSS92nrpIZMQju_GOW-lW2qIQmHYL7k,2496
+dspawpy-0.9.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-0.9.4.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-0.9.4.dist-info/RECORD,,
```

