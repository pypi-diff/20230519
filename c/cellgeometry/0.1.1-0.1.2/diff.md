# Comparing `tmp/cellgeometry-0.1.1.tar.gz` & `tmp/cellgeometry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellgeometry-0.1.1.tar", max compression
+gzip compressed data, was "cellgeometry-0.1.2.tar", max compression
```

## Comparing `cellgeometry-0.1.1.tar` & `cellgeometry-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      192 2023-04-21 16:55:26.217313 cellgeometry-0.1.1/README.md
--rw-r--r--   0        0        0      633 2023-05-12 08:50:34.861687 cellgeometry-0.1.1/cellgeometry/Hello.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:04.415769 cellgeometry-0.1.1/cellgeometry/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-12 10:21:58.312224 cellgeometry-0.1.1/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py
--rw-r--r--   0        0        0     3579 2023-05-12 12:07:45.106598 cellgeometry-0.1.1/cellgeometry/pages/1-Load_Data.py
--rw-r--r--   0        0        0     3119 2023-05-12 12:11:02.657968 cellgeometry-0.1.1/cellgeometry/pages/Cell_Shear.py
--rw-r--r--   0        0        0      833 2023-04-28 10:21:32.130658 cellgeometry-0.1.1/cellgeometry/utils/basic.py
--rw-r--r--   0        0        0     3053 2023-05-12 11:37:16.304501 cellgeometry-0.1.1/cellgeometry/utils/data_utils.py
--rw-r--r--   0        0        0    10885 2023-05-12 10:58:27.165188 cellgeometry-0.1.1/cellgeometry/utils/experimental.py
--rw-r--r--   0        0        0      663 2023-05-18 00:37:52.731562 cellgeometry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 cellgeometry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      192 2023-04-21 16:55:26.217313 cellgeometry-0.1.2/README.md
+-rw-r--r--   0        0        0     2812 2023-05-19 10:35:18.782390 cellgeometry-0.1.2/cellgeometry/Hello.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:29:04.415769 cellgeometry-0.1.2/cellgeometry/__init__.py
+-rw-r--r--   0        0        0     7266 2023-05-18 09:18:10.013298 cellgeometry-0.1.2/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py
+-rw-r--r--   0        0        0     3684 2023-05-19 08:09:14.390504 cellgeometry-0.1.2/cellgeometry/pages/1-Load_Data.py
+-rw-r--r--   0        0        0     5460 2023-05-19 10:04:54.244923 cellgeometry-0.1.2/cellgeometry/pages/2-Cell_Shear.py
+-rw-r--r--   0        0        0     4102 2023-05-19 10:19:53.553784 cellgeometry-0.1.2/cellgeometry/pages/3-PCA.py
+-rw-r--r--   0        0        0      833 2023-04-28 10:21:32.130658 cellgeometry-0.1.2/cellgeometry/utils/basic.py
+-rw-r--r--   0        0        0     3069 2023-05-18 09:19:02.341117 cellgeometry-0.1.2/cellgeometry/utils/data_utils.py
+-rw-r--r--   0        0        0    10886 2023-05-18 09:19:02.405117 cellgeometry-0.1.2/cellgeometry/utils/experimental.py
+-rw-r--r--   0        0        0      665 2023-05-19 08:39:58.762560 cellgeometry-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 cellgeometry-0.1.2/PKG-INFO
```

### Comparing `cellgeometry-0.1.1/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py` & `cellgeometry-0.1.2/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,195 +22,223 @@
 
 from geomstats.learning.frechet_mean import FrechetMean
 from geomstats.learning.kmeans import RiemannianKMeans
 from geomstats.learning.mdm import RiemannianMinimumDistanceToMean
 from geomstats.learning.pca import TangentPCA
 
 import sys
-sys.path.append("/app/utils") 
+
+sys.path.append("/app/utils")
 
 # import utils
 from utils import experimental as experimental
 from utils import basic as basic
 
 
-
-
-st.set_page_config(page_title="Elastic Metric for Cell Boundary Analysis", page_icon="📈")
+st.set_page_config(
+    page_title="Elastic Metric for Cell Boundary Analysis", page_icon="📈"
+)
 
 st.markdown("# Shape Analysis of Cancer Cells")
 st.sidebar.header("Shape Analysis of Cancer Cells")
 st.write(
     """This notebook studies Osteosarcoma (bone cancer) cells and the impact of drug treatment on their morphological shapes, by analyzing cell images obtained from fluorescence microscopy.
 
 This analysis relies on the elastic metric between discrete curves from Geomstats. We will study to which extent this metric can detect how the cell shape is associated with the response to treatment."""
 )
 
 dataset_name = "osteosarcoma"
 
-n_sampling_points = st.slider('Select the Number of Sampling Points', 0, 250, 100)
+n_sampling_points = st.slider("Select the Number of Sampling Points", 0, 250, 100)
 n_cells = 650
 # n_sampling_points = 100
 labels_a_name = "lines"
 labels_b_name = "treatments"
 
-quotient = ["rotation"] #["scaling"] #, "rotation"]
+quotient = ["rotation"]  # ["scaling"] #, "rotation"]
 do_not_quotient = False
 
 
 if dataset_name == "osteosarcoma":
-    cells, cell_shapes, labels_a, labels_b = experimental.load_treated_osteosarcoma_cells(
+    (
+        cells,
+        cell_shapes,
+        labels_a,
+        labels_b,
+    ) = experimental.load_treated_osteosarcoma_cells(
         n_cells=n_cells, n_sampling_points=n_sampling_points, quotient=quotient
     )
 else:
     pass
 
 
 labels_a_dict = {lab: i_lab for i_lab, lab in enumerate(np.unique(labels_a))}
 labels_b_dict = {lab: i_lab for i_lab, lab in enumerate(np.unique(labels_b))}
 
-print(f"Dictionary associated to label \"{labels_a_name}\":")
+print(f'Dictionary associated to label "{labels_a_name}":')
 print(labels_a_dict)
-print(f"Dictionary associated to label \"{labels_b_name}\":")
+print(f'Dictionary associated to label "{labels_b_name}":')
 print(labels_b_dict)
 
 if do_not_quotient:
     cell_shapes = cells
 
 n_cells_to_plot = 10
 
 fig = plt.figure(figsize=(16, 6))
 count = 1
 for label_b in np.unique(labels_b):
     for i_lab_a, label_a in enumerate(np.unique(labels_a)):
-        cell_data = [cell for cell, lab_a, lab_b in zip(cell_shapes, labels_a, labels_b) if lab_a == label_a and lab_b == label_b]
+        cell_data = [
+            cell
+            for cell, lab_a, lab_b in zip(cell_shapes, labels_a, labels_b)
+            if lab_a == label_a and lab_b == label_b
+        ]
         for i_to_plot in range(n_cells_to_plot):
             cell = gs.random.choice(a=cell_data)
-            fig.add_subplot(len(np.unique(labels_b)), len(np.unique(labels_a)) * n_cells_to_plot, count)
+            fig.add_subplot(
+                len(np.unique(labels_b)),
+                len(np.unique(labels_a)) * n_cells_to_plot,
+                count,
+            )
             count += 1
-            plt.plot(cell[:, 0], cell[:, 1], color=f"C{i_lab_a}" )
+            plt.plot(cell[:, 0], cell[:, 1], color=f"C{i_lab_a}")
             plt.axis("equal")
             plt.axis("off")
             if i_to_plot == n_cells_to_plot // 2:
                 plt.title(f"{label_a}   -   {label_b}", fontsize=20)
 st.pyplot(fig)
 
 # Define shape space
 R1 = Euclidean(dim=1)
 CLOSED_CURVES_SPACE = ClosedDiscreteCurves(R2)
 CURVES_SPACE = DiscreteCurves(R2)
 SRV_METRIC = CURVES_SPACE.srv_metric
 L2_METRIC = CURVES_SPACE.l2_curves_metric
 
 ELASTIC_METRIC = {}
-AS = [1, 2, 0.75, 0.5, 0.25, 0.01] #, 1.6] #, 1.4, 1.2, 1, 0.5, 0.2, 0.1]
-BS = [0.5, 1, 0.5, 0.5, 0.5, 0.5] #, 2, 2, 2, 2, 2, 2, 2]
+AS = [1, 2, 0.75, 0.5, 0.25, 0.01]  # , 1.6] #, 1.4, 1.2, 1, 0.5, 0.2, 0.1]
+BS = [0.5, 1, 0.5, 0.5, 0.5, 0.5]  # , 2, 2, 2, 2, 2, 2, 2]
 for a, b in zip(AS, BS):
     ELASTIC_METRIC[a, b] = DiscreteCurves(R2, a=a, b=b).elastic_metric
 METRICS = {}
 METRICS["Linear"] = L2_METRIC
 METRICS["SRV"] = SRV_METRIC
 
 means = {}
 
 means["Linear"] = gs.mean(cell_shapes, axis=0)
-means["SRV"] = FrechetMean(
-        metric=SRV_METRIC, 
-        method="default").fit(cell_shapes).estimate_
+means["SRV"] = (
+    FrechetMean(metric=SRV_METRIC, method="default").fit(cell_shapes).estimate_
+)
 
 for a, b in zip(AS, BS):
-    means[a, b] = FrechetMean(
-            metric=ELASTIC_METRIC[a, b], 
-            method="default").fit(cell_shapes).estimate_
-    
+    means[a, b] = (
+        FrechetMean(metric=ELASTIC_METRIC[a, b], method="default")
+        .fit(cell_shapes)
+        .estimate_
+    )
+
 st.header("Sample Means")
-st.markdown("We compare results when computing the mean cell versus the mean cell shapes with different elastic metrics.")
+st.markdown(
+    "We compare results when computing the mean cell versus the mean cell shapes with different elastic metrics."
+)
 fig = plt.figure(figsize=(18, 8))
 
 ncols = len(means) // 2
 
 for i, (mean_name, mean) in enumerate(means.items()):
-    ax = fig.add_subplot(2, ncols, i+1)
+    ax = fig.add_subplot(2, ncols, i + 1)
     ax.plot(mean[:, 0], mean[:, 1], "black")
     ax.set_aspect("equal")
     ax.axis("off")
     axs_title = mean_name
     if mean_name not in ["Linear", "SRV"]:
         a = mean_name[0]
         b = mean_name[1]
         ratio = a / (2 * b)
         mean_name = f"Elastic {mean_name}\n a / (2b) = {ratio}"
     ax.set_title(mean_name)
 
 st.pyplot(fig)
 
 
-
 fig = plt.figure(figsize=(18, 8))
 
 ncols = len(means) // 2
 
 for i, (mean_name, mean) in enumerate(means.items()):
-    ax = fig.add_subplot(2, ncols, i+1)
+    ax = fig.add_subplot(2, ncols, i + 1)
     mean = CLOSED_CURVES_SPACE.projection(mean)
     ax.plot(mean[:, 0], mean[:, 1], "black")
     ax.set_aspect("equal")
     ax.axis("off")
     axs_title = mean_name
     if mean_name not in ["Linear", "SRV"]:
         a = mean_name[0]
         b = mean_name[1]
         ratio = a / (2 * b)
         mean_name = f"Elastic {mean_name}\n a / (2b) = {ratio}"
     ax.set_title(mean_name)
 
 
-st.markdown("__Remark:__ Unfortunately, there are some numerical issues with the projection in the space of closed curves, as shown by the V-shaped results above.")
-            
-st.markdown("Since ratios of 1 give the same results as for the SRV metric, we only select AS, BS with a ratio that is not 1 for the elastic metrics.")
+st.markdown(
+    "__Remark:__ Unfortunately, there are some numerical issues with the projection in the space of closed curves, as shown by the V-shaped results above."
+)
 
-st.markdown("We also continue the analysis with the space of open curves, as opposed to the space of closed curves, for the numerical issues observed above.")
+st.markdown(
+    "Since ratios of 1 give the same results as for the SRV metric, we only select AS, BS with a ratio that is not 1 for the elastic metrics."
+)
 
+st.markdown(
+    "We also continue the analysis with the space of open curves, as opposed to the space of closed curves, for the numerical issues observed above."
+)
 
-NEW_AS = [0.75, 0.5, 0.25, 0.01] #, 1.6] #, 1.4, 1.2, 1, 0.5, 0.2, 0.1]
-NEW_BS = [0.5, 0.5, 0.5, 0.5] #, 2, 2, 2, 2, 2, 2, 2]
+
+NEW_AS = [0.75, 0.5, 0.25, 0.01]  # , 1.6] #, 1.4, 1.2, 1, 0.5, 0.2, 0.1]
+NEW_BS = [0.5, 0.5, 0.5, 0.5]  # , 2, 2, 2, 2, 2, 2, 2]
 
 st.markdown("## Distances to the Mean")
 
 # We multiply the distances by a 100, for visualization purposes. It amounts to a change of units.
 dists = {}
 
-dists["Linear"] = [100 * gs.linalg.norm(means["Linear"] - cell) / n_sampling_points for cell in cell_shapes]
+dists["Linear"] = [
+    100 * gs.linalg.norm(means["Linear"] - cell) / n_sampling_points
+    for cell in cell_shapes
+]
 
 dists["SRV"] = [
-    100 * SRV_METRIC.dist(means["SRV"], cell) / n_sampling_points for cell in cell_shapes
+    100 * SRV_METRIC.dist(means["SRV"], cell) / n_sampling_points
+    for cell in cell_shapes
 ]
 
 for a, b in zip(NEW_AS, NEW_BS):
-    dists[a, b] =  [
-    100 * ELASTIC_METRIC[a, b].dist(means[a, b], cell) / n_sampling_points for cell in cell_shapes
-]
+    dists[a, b] = [
+        100 * ELASTIC_METRIC[a, b].dist(means[a, b], cell) / n_sampling_points
+        for cell in cell_shapes
+    ]
 
 
 dists_summary = pd.DataFrame(
     data={
         labels_a_name: labels_a,
         labels_b_name: labels_b,
         "Linear": dists["Linear"],
         "SRV": dists["SRV"],
     }
 )
 
 for a, b in zip(NEW_AS, NEW_BS):
     dists_summary[f"Elastic({a}, {b})"] = dists[a, b]
 
-st.dataframe(dists_summary) 
+st.dataframe(dists_summary)
 # SAVEFIG = True
 # if SAVEFIG:
 #     figs_dir = os.path.join(work_dir, f"cells/saved_figs/{dataset_name}")
 #     if not os.path.exists(figs_dir):
 #         os.makedirs(figs_dir)
 #     print(f"Will save figs to {figs_dir}")
 #     from datetime import datetime
 
 #     now = datetime.now().strftime("%Y%m%d_%H_%M_%S")
-#     print(now)
+#     print(now)
```

### Comparing `cellgeometry-0.1.1/cellgeometry/pages/1-Load_Data.py` & `cellgeometry-0.1.2/cellgeometry/pages/1-Load_Data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import streamlit as st
 import pandas as pd
 import os
 import time
 import matplotlib.pyplot as plt
 
 import sys
-sys.path.append("/app/utils") 
+
+sys.path.append("/app/utils")
 
 from utils.data_utils import build_rois, find_all_instances
 
 current_time = time.localtime()
 
 year = time.strftime("%Y", current_time)
 day_of_year = time.strftime("%j", current_time)
 time_string = time.strftime("%H%M%S", current_time)
 
 current_time_string = f"{year}{day_of_year}-{time_string}"
 
 if "cells_list" not in st.session_state:
-   st.session_state["cells_list"] = True
+    st.session_state["cells_list"] = True
 
 st.write("# Load Your Cell Data 👋")
 
 st.markdown(
-"""
+    """
 ## Getting Started
 
 We currently support an ROI zip folder created by FIJI/ImageJ. What this means is you may have a folder structure as follows:
 ```
     └── Cropped_Images
         ├── Bottom_plank_0
         │   ├── Averaged_ROI
@@ -39,14 +40,15 @@
         │   └── ROIs  <---- Folder of zipped ROIs
 ```
 You can simply upload this ROIs folder and we will load your data for you. We plan on supporting data given in `xy` coordinate format from `JSON` and CSV/TXT files.
 Your chosen data structure __must__ contain `x` and `y` for the program to correctly parse and load your data.
 """
 )
 
+
 def get_files_from_folder(folder_path):
     """
     Retrieves a list of files from a specific folder.
 
     Parameters:
         folder_path (str): The path to the folder.
 
@@ -62,31 +64,34 @@
     files = []
     for filename in os.listdir(folder_path):
         if os.path.isfile(os.path.join(folder_path, filename)):
             files.append(os.path.join(folder_path, filename))
     return files
 
 
-
 # Specify the folder path for file uploads and save run with date and time
 upload_folder = f"/app/data/run-{current_time_string}"
 
 # Check if the upload folder exists, and create it if it doesn't
 if not os.path.exists(upload_folder):
     os.makedirs(upload_folder)
     st.info(f"Upload folder created: {upload_folder}")
 
 # Get the list of files in the upload folder
 files = get_files_from_folder(upload_folder)
 
 
-
 # Display the file uploader
-uploaded_files = st.file_uploader("Upload a file", type=["zip"], accept_multiple_files=True)
+uploaded_files = st.file_uploader(
+    "Upload a file", type=["zip"], accept_multiple_files=True
+)
 
+if not uploaded_files:
+  st.warning('Please upload a zipped file of ROIs')
+  st.stop()
 
 # Process the uploaded files
 if uploaded_files is not None:
     progress_bar = st.progress(0)
     total_files = len(uploaded_files)
     completed_files = 0
 
@@ -101,19 +106,21 @@
 
 
 # Build a dictionary of all the ROIs
 dict_rois = build_rois(upload_folder)
 
 # Extract the cells
 cells_list = []
-find_all_instances(dict_rois, 'x', 'y', cells_list)
+find_all_instances(dict_rois, "x", "y", cells_list)
 st.session_state["cells_list"] = cells_list
 
 st.write(f"Successfully Loaded {len(cells_list)} cells.")
 
 # Sanity check visualization
-cell_num = st.number_input(f"Visualize a cell. Pick a number between 0 and {len(cells_list)-1}", min_value=0)
+cell_num = st.number_input(
+    f"Visualize a cell. Pick a number between 0 and {len(cells_list)-1}", min_value=0
+)
 
 
 fig, ax = plt.subplots()
-ax.plot(cells_list[cell_num][:,0], cells_list[cell_num][:,1])
+ax.plot(cells_list[cell_num][:, 0], cells_list[cell_num][:, 1])
 st.pyplot(fig)
```

### Comparing `cellgeometry-0.1.1/cellgeometry/utils/basic.py` & `cellgeometry-0.1.2/cellgeometry/utils/basic.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.1/cellgeometry/utils/data_utils.py` & `cellgeometry-0.1.2/cellgeometry/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         >>> rois = build_rois(roi_directory)
         >>> print(rois)
         {'roi1': <ROI data>, 'roi2': <ROI data>, ...}
     """
     rois = {}
     for roi in sorted(os.listdir(path)):
         # print(roi.split(".")[0])
-        rois[roi.split(".")[0]] = read_roi_zip(os.path.join(path,roi))
+        rois[roi.split(".")[0]] = read_roi_zip(os.path.join(path, roi))
     return rois
 
 
 def find_key(dictionary, target_key):
     """
     Recursively searches for a key in a nested dictionary.
 
@@ -48,21 +48,21 @@
         ... }
         >>> result = find_key(data, 'key4')
         >>> print(result)
         value4
     """
     if target_key in dictionary:
         return dictionary[target_key]
-    
+
     for value in dictionary.values():
         if isinstance(value, dict):
             result = find_key(value, target_key)
             if result is not None:
                 return result
-    
+
     return None
 
 
 def find_all_instances(dictionary, target_key1, target_key2, results_list):
     """
     Recursively finds instances of two target keys in a nested dictionary and appends their corresponding values together.
 
@@ -93,8 +93,10 @@
     for key, value in dictionary.items():
         if key == target_key1 or key == target_key2:
             found_keys.add(key)
         elif isinstance(value, dict):
             find_all_instances(value, target_key1, target_key2, results_list)
 
     if {target_key1, target_key2}.issubset(found_keys):
-        results_list.append(np.array([dictionary[target_key1], dictionary[target_key2]]).T)
+        results_list.append(
+            np.array([dictionary[target_key1], dictionary[target_key2]]).T
+        )
```

### Comparing `cellgeometry-0.1.1/cellgeometry/utils/experimental.py` & `cellgeometry-0.1.2/cellgeometry/utils/experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
         else:
             for i_cell, cell_shape in enumerate(cell_shapes):
                 cell_shapes[i_cell] = _exhaustive_align(cell_shape, cell_shapes[0])
 
     return cells, cell_shapes, labels_a, labels_b
 
 
-
 def nolabel_preprocess(
     cells,
     # labels_a,
     # labels_b,
     n_cells,
     n_sampling_points,
     quotient=["scaling", "rotation"],
@@ -269,15 +268,15 @@
         if "scaling" not in quotient:
             for i_cell, cell_shape in enumerate(cells):
                 cell_shapes[i_cell] = _exhaustive_align(cell_shape, cells[0])
         else:
             for i_cell, cell_shape in enumerate(cell_shapes):
                 cell_shapes[i_cell] = _exhaustive_align(cell_shape, cell_shapes[0])
 
-    return cells, cell_shapes #, labels_a, labels_b
+    return cells, cell_shapes  # , labels_a, labels_b
 
 
 def load_treated_osteosarcoma_cells(
     n_cells=-1, n_sampling_points=10, quotient=["scaling", "rotation"]
 ):
     """Load dataset of osteosarcoma cells (bone cancer cells).
```

### Comparing `cellgeometry-0.1.1/pyproject.toml` & `cellgeometry-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cellgeometry"
-version = "0.1.1"
+version = "0.1.2"
 description = "Statistical Cell Shape Analysis"
 authors = ["Amil Khan <amil@ucsb.edu>", "Samuel Feinstein <sdfeinstein@ucsb.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/bioshape-lab/cells"
 homepage = "https://github.com/bioshape-lab/cells/tree/main/cells/streamlit"
 
@@ -12,15 +12,15 @@
 python = "^3.10"
 streamlit = "^1.21.0"
 numpy = "1.23.0"
 geomstats = "^2.5.0"
 scikit-image = "^0.20.0"
 matplotlib = "^3.7.1"
 numba = "^0.56.4"
-torch = "^2.0.0"
 autograd = "^1.5"
 read-roi = "^1.6.0"
+plotly = "^5.14.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cellgeometry-0.1.1/PKG-INFO` & `cellgeometry-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellgeometry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Statistical Cell Shape Analysis
 Home-page: https://github.com/bioshape-lab/cells/tree/main/cells/streamlit
 License: MIT
 Author: Amil Khan
 Author-email: amil@ucsb.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: autograd (>=1.5,<2.0)
 Requires-Dist: geomstats (>=2.5.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (==1.23.0)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: read-roi (>=1.6.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: streamlit (>=1.21.0,<2.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/bioshape-lab/cells
 Description-Content-Type: text/markdown
 
 # Cell Shape Analysis
 [![Docker](https://github.com/amilworks/cells/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/amilworks/cells/actions/workflows/docker-publish.yml)
```

