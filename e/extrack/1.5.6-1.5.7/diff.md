# Comparing `tmp/extrack-1.5.6.tar.gz` & `tmp/extrack-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrack-1.5.6.tar", last modified: Tue Dec 20 00:21:40 2022, max compression
+gzip compressed data, was "extrack-1.5.7.tar", last modified: Fri May 19 21:03:40 2023, max compression
```

## Comparing `extrack-1.5.6.tar` & `extrack-1.5.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-12-20 00:21:40.189936 extrack-1.5.6/
--rwxrwxrwx   0 francois  (1000) francois  (1000)     1074 2022-12-19 19:13:13.000000 extrack-1.5.6/LICENSE
--rwxrwxrwx   0 francois  (1000) francois  (1000)     6723 2022-12-20 00:21:40.185939 extrack-1.5.6/PKG-INFO
--rwxrwxrwx   0 francois  (1000) francois  (1000)     6081 2022-12-19 19:13:13.000000 extrack-1.5.6/README.md
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-12-20 00:21:39.758926 extrack-1.5.6/Tutorials/
--rwxrwxrwx   0 francois  (1000) francois  (1000)        1 2022-12-19 19:13:13.000000 extrack-1.5.6/Tutorials/__init__.py
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-12-20 00:21:40.034069 extrack-1.5.6/extrack/
--rwxrwxrwx   0 francois  (1000) francois  (1000)      367 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/__init__.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     6484 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/auto_fitting.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    23781 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/exporters.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    24031 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/histograms.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    40699 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/old_tracking.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     9076 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/readers.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    22606 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/refined_loc_old.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    25414 2022-12-19 19:26:11.000000 extrack-1.5.6/extrack/refined_localization.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    10688 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/simulate_tracks.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    89644 2022-12-20 00:20:38.000000 extrack-1.5.6/extrack/tracking.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    58805 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/tracking_0.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)       22 2022-12-19 22:26:21.000000 extrack-1.5.6/extrack/version.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     5227 2022-12-19 19:13:13.000000 extrack-1.5.6/extrack/visualization.py
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-12-20 00:21:40.157930 extrack-1.5.6/extrack.egg-info/
--rwxrwxrwx   0 francois  (1000) francois  (1000)     6723 2022-12-20 00:21:39.000000 extrack-1.5.6/extrack.egg-info/PKG-INFO
--rwxrwxrwx   0 francois  (1000) francois  (1000)      547 2022-12-20 00:21:39.000000 extrack-1.5.6/extrack.egg-info/SOURCES.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)        1 2022-12-20 00:21:39.000000 extrack-1.5.6/extrack.egg-info/dependency_links.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)       34 2022-12-20 00:21:39.000000 extrack-1.5.6/extrack.egg-info/requires.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)       18 2022-12-20 00:21:39.000000 extrack-1.5.6/extrack.egg-info/top_level.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)      104 2022-12-19 19:13:13.000000 extrack-1.5.6/pyproject.toml
--rwxrwxrwx   0 francois  (1000) francois  (1000)       38 2022-12-20 00:21:40.193932 extrack-1.5.6/setup.cfg
--rwxrwxrwx   0 francois  (1000) francois  (1000)     1049 2022-12-19 19:13:13.000000 extrack-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.794831 extrack-1.5.7/
+-rw-rw-rw-   0        0        0     1074 2023-05-19 15:53:57.000000 extrack-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     6889 2023-05-19 21:03:40.794831 extrack-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6083 2023-05-19 15:53:57.000000 extrack-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.725797 extrack-1.5.7/Tutorials/
+-rw-rw-rw-   0        0        0        1 2023-05-19 15:54:45.000000 extrack-1.5.7/Tutorials/__init__.py
+-rw-rw-rw-   0        0        0     3979 2023-05-19 15:54:45.000000 extrack-1.5.7/Tutorials/automated_fitting.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.757049 extrack-1.5.7/extrack/
+-rw-rw-rw-   0        0        0      367 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/__init__.py
+-rw-rw-rw-   0        0        0     6484 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/auto_fitting.py
+-rw-rw-rw-   0        0        0    23781 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/exporters.py
+-rw-rw-rw-   0        0        0    24031 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/histograms.py
+-rw-rw-rw-   0        0        0    40699 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/old_tracking.py
+-rw-rw-rw-   0        0        0    10492 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/readers.py
+-rw-rw-rw-   0        0        0    22606 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/refined_loc_old.py
+-rw-rw-rw-   0        0        0    25414 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/refined_localization.py
+-rw-rw-rw-   0        0        0    10688 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/simulate_tracks.py
+-rw-rw-rw-   0        0        0    73026 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/tracking.py
+-rw-rw-rw-   0        0        0    58805 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/tracking_0.py
+-rw-rw-rw-   0        0        0       22 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/version.py
+-rw-rw-rw-   0        0        0     5227 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.794831 extrack-1.5.7/extrack.egg-info/
+-rw-rw-rw-   0        0        0     6889 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-05-19 15:53:57.000000 extrack-1.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 21:03:40.794831 extrack-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-19 15:53:57.000000 extrack-1.5.7/setup.py
```

### Comparing `extrack-1.5.6/LICENSE` & `extrack-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/PKG-INFO` & `extrack-1.5.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: extrack
-Version: 1.5.6
-Summary: SPT kinetic modelling and states annotation of tracks
-Home-page: https://github.com/FrancoisSimon/ExTrack-python3
-Author: Francois Simon
-Author-email: simon.francois@protonmail.com
-Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ExTrack
 -------
 
 This repository contains the necessary scripts to run the method ExTrack. ExTrack is a method to detemine kinetics of particles able to transition between different motion states. It can assess diffusion coefficients, transition rates, localization error as well as annotating the probability for any track to be in each state for every time points. It can produce histograms of durations in each state to highlight no markovian transition kinetics. Eventually it can be used to refine the localization precision of tracks by considering the most likely positions which is especially efficient when the particle do not move.
 
 More details on the methods are available on BioarXiv https://www.biorxiv.org/content/10.1101/2022.07.13.499913v1.
 
@@ -60,15 +43,15 @@
 
 # Installation from this GitHub repository
 
 ## From Unix/Mac:
 
 `sudo apt install git` (if git is not installed)
 
-`git clone https://github.com/FrancoisSimon/ExTrack.git`
+`git clone https://github.com/vanTeeffelenLab/ExTrack.git`
 
 `cd ExTrack`
 
 `sudo python setup.py install`
 
 ## From Windows using anaconda prompt:
```

### Comparing `extrack-1.5.6/extrack/auto_fitting.py` & `extrack-1.5.7/extrack/auto_fitting.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/exporters.py` & `extrack-1.5.7/extrack/exporters.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/histograms.py` & `extrack-1.5.7/extrack/histograms.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/old_tracking.py` & `extrack-1.5.7/extrack/old_tracking.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/readers.py` & `extrack-1.5.7/extrack/readers.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,24 +96,24 @@
             for k, m in enumerate(opt_metrics_names):
                 del opt_metrics[m][l]
                 
     return traces, frames, opt_metrics
 
 def read_table(paths, # path of the file to read or list of paths to read multiple files.
                lengths = np.arange(5,40), # number of positions per track accepted (take the first position if longer than max
-               dist_th = 0.5, # maximum distance allowed for consecutive positions 
+               dist_th = np.inf, # maximum distance allowed for consecutive positions 
                frames_boundaries = [-np.inf, np.inf], # min and max frame values allowed for peak detection
                fmt = 'csv', # format of the document to be red, 'csv' or 'pkl', one can also just specify a separator e.g. ' '. 
-               colnames = ['POSITION_X', 'POSITION_Y', 'FRAME', 'TRACK_ID'], 
+               colnames = ['POSITION_X', 'POSITION_Y', 'FRAME', 'TRACK_ID'],  # if multiple columns are required to identify a track, the string used to identify the track ID can be replaced by a list of strings represening the column names e.g. ['TRACK_ID', 'Movie_ID']
                opt_colnames = [], # list of additional metrics to collect e.g. ['QUALITY', 'ID']
                remove_no_disp = True):
     
-    if type(paths) == type(''):
+    if type(paths) == str or type(paths) == np.str_:
         paths = [paths]
-        
+
     tracks = {}
     frames = {}
     opt_metrics = {}
     for m in opt_colnames:
         opt_metrics[m] = {}
     nb_peaks = 0
     for l in lengths:
@@ -127,68 +127,84 @@
         if fmt == 'csv':
             data = pd.read_csv(path, sep=',')
         elif fmt == 'pkl':
             data = pd.read_pickle(path)
         else:
             data = pd.read_csv(path, sep = fmt)
         
+        if not (type(colnames[3]) == str or type(colnames[3]) == np.str_):
+            # in this case we remove the NA values for simplicity
+            None_ID = (data[colnames[3]] == 'None') + pd.isna(data[colnames[3]])
+            data = data.drop(data[np.any(None_ID,1)].index)
+                
+            new_ID = data[colnames[3][0]].astype(str)
+            
+            for k in range(1,len(colnames[3])):
+                new_ID = new_ID + '_' + data[colnames[3][k]].astype(str)
+            data['unique_ID'] = new_ID
+            colnames[3] = 'unique_ID'        
         try:
+            # in this case, peaks without an ID are assumed alone and are added a unique ID, only works if ID are integers
             None_ID = (data[colnames[3]] == 'None' ) + pd.isna(data[colnames[3]])
             max_ID = np.max(data[colnames[3]][(data[colnames[3]] != 'None' ) * (pd.isna(data[colnames[3]]) == False)].astype(int))
             data.loc[None_ID, colnames[3]] = np.arange(max_ID+1, max_ID+1 + np.sum(None_ID))
-            IDs = data[colnames[3]].astype(int)
         except:
             None_ID = (data[colnames[3]] == 'None' ) + pd.isna(data[colnames[3]])
             data = data.drop(data[None_ID].index)
         
+        IDs = data[colnames[3]].astype(str)
+
         data = data[colnames + opt_colnames]
         
         track_list = []
         for ID in np.unique(IDs):
             track_list.append(data[IDs == ID])
         
         zero_disp_tracks = 0
             
         try:
             for ID in np.unique(IDs):
+                
                 track = data[IDs == ID]
                 track = track.sort_values(colnames[2], axis = 0)
-                track_mat = track.values[:,:4].astype('float64')
+                track_mat = track.values[:,:3].astype('float64')
                 dists = np.sum((track_mat[1:, :2] - track_mat[:-1, :2])**2, axis = 1)**0.5
                 if track_mat[0, 2] >= frames_boundaries[0] and track_mat[0, 2] <= frames_boundaries[1] : #and np.all(dists<dist_th):
-                    if not np.all(dists<dist_th):
-                        zero_disp_tracks = 1
-                    
-                    if np.any([len(track_mat)]*len(lengths) == np.array(lengths)):
-                        l = len(track)
-                        tracks[str(l)].append(track_mat[:, 0:2])
-                        frames[str(l)].append(track_mat[:, 2])
-                        for m in opt_colnames:
-                            opt_metrics[m][str(l)].append(track[m].values)
-    
-                    elif len(track_mat) > np.max(lengths):
-                        l = np.max(lengths)
-                        tracks[str(l)].append(track_mat[:l, 0:2])
-                        frames[str(l)].append(track_mat[:l, 2])
-                        for m in opt_colnames:
-                            opt_metrics[m][str(l)].append(track[m].values[:l])           
+                    if not np.any(dists>dist_th):
+                        
+                        if np.any([len(track_mat)]*len(lengths) == np.array(lengths)):
+                            l = len(track)
+                            tracks[str(l)].append(track_mat[:, 0:2])
+                            frames[str(l)].append(track_mat[:, 2])
+                            for m in opt_colnames:
+                                opt_metrics[m][str(l)].append(track[m].values)
+        
+                        elif len(track_mat) > np.max(lengths):
+                            l = np.max(lengths)
+                            tracks[str(l)].append(track_mat[:l, 0:2])
+                            frames[str(l)].append(track_mat[:l, 2])
+                            for m in opt_colnames:
+                                opt_metrics[m][str(l)].append(track[m].values[:l]) 
+                        
+                        elif len(track_mat) < np.max(lengths) and len(track_mat) > np.min(lengths) : # in case where lengths between min(lengths) and max(lentghs) are not all present:
+                            l_idx =   np.argmin(np.floor(len(track_mat) / lengths))-1
+                            l = lengths[l_idx]
+                            tracks[str(l)].append(track_mat[:l, 0:2])
+                            frames[str(l)].append(track_mat[:l, 2])
         except :
             print('problem with file :', path)
         
     for l in list(tracks.keys()):
         if len(tracks[str(l)])>0:
+            print(l)
             tracks[str(l)] = np.array(tracks[str(l)])
             frames[str(l)] = np.array(frames[str(l)])
             for m in opt_colnames:
                 opt_metrics[m][str(l)] = np.array(opt_metrics[m][str(l)])
         else:
             del tracks[str(l)], frames[str(l)]
             for k, m in enumerate(opt_colnames):
                 del opt_metrics[m][str(l)]        
                     
     if zero_disp_tracks and not remove_no_disp:
         print('Warning: some tracks show no displacements. To be checked if normal or not. These tracks can be removed with remove_no_disp = True')
     return tracks, frames, opt_metrics
-
-
-
-
```

### Comparing `extrack-1.5.6/extrack/refined_loc_old.py` & `extrack-1.5.7/extrack/refined_loc_old.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/refined_localization.py` & `extrack-1.5.7/extrack/refined_localization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/simulate_tracks.py` & `extrack-1.5.7/extrack/simulate_tracks.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/tracking.py` & `extrack-1.5.7/extrack/tracking.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,16 +94,15 @@
 def first_log_integrale_dif(Ci, l2, cur_d2s):
     '''
     convolution of 2 normal laws = normal law (mean = sum of means and variance = sum of variances)
     '''
     s2_arr = l2+cur_d2s
     m_arr = Ci
     return m_arr, s2_arr
-#Cs = all_tracks['60']
-#Cs = args[0]
+
 def P_Cs_inter_bound_stats(Cs, LocErr, ds, Fs, TrMat, pBL=0.1, isBL = 1, cell_dims = [0.5], nb_substeps=1, frame_len = 4, do_preds = 0, min_len = 3) :
     '''
     compute the product of the integrals over Ri as previousily described
     work in log space to avoid overflow and underflow
     
     Cs : dim 0 = track ID, dim 1 : states, dim 2 : peaks postions through time,
     dim 3 : x, y position
@@ -387,33 +386,27 @@
     remove_axis.reverse()
         
     rm_axis = np.where(np.array(remove_axis))
     rm_axis = tuple(rm_axis[0]+1) # we add 1 as the first dim of our arrays is for the track ID
     
     new_LP = LP.reshape([nb_Tracks] + dims)
     max_LP = new_LP.max(axis = rm_axis,keepdims = True)
-    #log_integrated_term = log_integrated_term.reshape([nb_Tracks] + dims)
-    #max_LP2 = (new_LP + log_integrated_term).max(axis = rm_axis,keepdims = True)
-    #norm_weights = np.exp(new_LP + log_integrated_term - max_LP2)
     norm_weights = np.exp(new_LP - max_LP)
     Sum_weights = np.sum(norm_weights, axis = rm_axis, keepdims = True)
     weights = norm_weights / Sum_weights
     weights = weights.reshape(weights.shape + (1,)) # add a dim for weights to fit the shape of m_arr and s2_arr
 
     m_arr = m_arr.reshape([nb_Tracks] + dims + [nb_dims])
     s2_arr = s2_arr.reshape([s2_arr.shape[0]] + dims + [s2_arr.shape[-1]])
     new_m_arr = np.sum(weights * m_arr, axis = rm_axis)
     new_s2_arr = np.sum(weights * s2_arr , axis = rm_axis)
     
     LP = LP.reshape([nb_Tracks] + dims)
     new_LP = np.log(np.sum(np.exp(LP-max_LP), axis = rm_axis)) + np.squeeze(max_LP, axis = rm_axis)
 
-    #np.mean(np.std(m_arr, axis = rm_axis))
-    #np.mean(np.std(s2_arr**0.5, axis = rm_axis))
-    #np.mean(np.std(s2_arr**0.5))
     new_cur_Bs = cur_Bs.reshape([1] + dims + [cur_len])
     for i, axis in enumerate(rm_axis):
         new_cur_Bs = np.take(new_cur_Bs, indices = 0, axis = axis -  i)
     new_cur_Bs = np.delete(new_cur_Bs , tuple(fuse_pos), axis =  -1)
     new_cur_Bs = new_cur_Bs.reshape((1, np.product(new_cur_Bs.shape[1:-1]), cur_len - len(fuse_pos)))
 
     new_m_arr = new_m_arr.reshape((nb_Tracks, np.product(new_m_arr.shape[1:-1]), nb_dims))
@@ -438,19 +431,14 @@
     
     each step is made of substeps if nb_substeps > 1, and we increase the matrix
     of possible Bs : cur_Bs accordingly
     
     to be able to process long tracks with good accuracy, for each track we fuse m_arr and Ks
     of sequences of states equal exept for the state 'frame_len' steps ago.
     '''
-    #threshold = 0.2
-    #Cs, LocErr, ds, Fs, TrMat, pBL, isBL, cell_dims, nb_substeps, frame_len, min_len = args_prod[0]
-    #max_nb_states = 120
-    
-    #ds = np.array([0,0.004, 0.25])
     nb_Tracks = Cs.shape[0]
     nb_locs = Cs.shape[1] # number of localization per track
     
     dtype = 'float64'
     
     nb_dims = Cs.shape[2] # number of spatial dimensions (x, y) or (x, y, z)
     Cs = Cs[:,None].astype('float64')
@@ -524,27 +512,21 @@
     if nb_substeps > 1 and 0:
         cur_len = nb_substeps + 1
         fuse_pos = np.arange(1,nb_substeps)
         m_arr, s2_arr, LP, cur_Bs = fuse_tracks_general(m_arr, s2_arr, LP, cur_Bs, cur_len, nb_Tracks, fuse_pos = fuse_pos, nb_states = nb_states, nb_dims = nb_dims)
     
     current_step += 1
     
-    #TrMat = np.array([[0.9,0.1],[0.2,0.8]])
     while current_step <= nb_locs-1:
-        # update cur_Bs to describe the states at the next step:
-        # cur_Bs = get_all_Bs(current_step*nb_substeps+1 - removed_steps, nb_states)[None]
-        # cur_Bs = all_Bs[:,:nb_states**(current_step + nb_substeps - removed_steps),:current_step + nb_substeps - removed_steps]
-
         for iii in range(nb_substeps):
             #cur_Bs = np.concatenate((np.repeat(np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], nb_Tracks, 0), np.repeat(cur_Bs,nb_states,1)),-1)
             cur_Bs = np.concatenate((np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], np.repeat(cur_Bs,nb_states,1)),-1)
             new_states = np.repeat(np.mod(np.arange(cur_Bs_cat.shape[1]*nb_states, dtype = 'int8'),nb_states)[None,:,None,None] == np.arange(nb_states, dtype = 'int8')[None,None,None], cur_Bs_cat.shape[0], 0).astype('int8')
             cur_Bs_cat = np.concatenate((new_states, np.repeat(cur_Bs_cat,nb_states,1)),-2)
         
-        #np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states).shape
         cur_states = cur_Bs[:1,:,0:nb_substeps+1].astype(int)
         # compute the vector of diffusion stds knowing the states at the current step
         cur_d2s = ds[cur_states]**2
         cur_d2s = (cur_d2s[:,:,1:] + cur_d2s[:,:,:-1]) / 2 # assuming a transition at the middle of the substeps
         cur_d2s = cp.mean(cur_d2s, axis = 2)
         cur_d2s = cur_d2s[:,:,None]
         LT = get_Ts_from_Bs(cur_states, TrMat)
@@ -592,72 +574,38 @@
                                                                    nb_Tracks,
                                                                    nb_states = nb_states,
                                                                    nb_dims = nb_dims,
                                                                    do_preds = do_preds,
                                                                    threshold = threshold,
                                                                    frame_len = frame_len) # threshold on values normalized by sigma.
             # threshold on values normalized by sigma.
-            '''
-            t0 = time()
-            for k in range(30):
-                _,_,_,_,_ = fuse_tracks_th(m_arr,
-                                            s2_arr,
-                                            LP,
-                                            cur_Bs,
-                                            cur_Bs_cat,
-                                            nb_Tracks,
-                                            nb_states = nb_states,
-                                            nb_dims = nb_dims,
-                                            do_preds = do_preds,
-                                            threshold = threshold,
-                                            frame_len = frame_len) # threshold on values normalized by sigma.
-                print()
-            print('total time: ', time()-t0)
-            
-            t0 = time()
-            for k in range(100):
-                #cur_Bs = np.concatenate((np.repeat(np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], nb_Tracks, 0), np.repeat(cur_Bs,nb_states,1)),-1)
-                #new_cur_Bs = np.concatenate((np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], np.repeat(cur_Bs,nb_states,1)),-1)
-                new_states = np.repeat(np.mod(np.arange(cur_Bs_cat.shape[1]*nb_states),nb_states)[None,:,None,None] == np.arange(nb_states)[None,None,None], cur_Bs_cat.shape[0], 0).astype('float16')
-                a = np.repeat(cur_Bs_cat.astype('float16'), nb_states, 1)
-                new_cur_Bs_cat = np.concatenate((new_states, a),-2)
-            print('total time: ', (time()-t0)/3)
-            cur_Bs_cat.shape
-            '''
             cur_nb_Bs = len(cur_Bs[0])
             #print(current_step, m_arr.shape)
             removed_steps += 1
             
         current_step += 1
     
-    #print(m_arr.shape)
-    #print(time()-t0)
-    
     if not isBL:
         LL = 0
     else:
         for iii in range(nb_substeps):
             #cur_Bs = np.concatenate((np.repeat(np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], nb_Tracks, 0), np.repeat(cur_Bs,nb_states,1)),-1)
             cur_Bs = np.concatenate((np.mod(np.arange(cur_Bs.shape[1]*nb_states),nb_states)[None,:,None], np.repeat(cur_Bs,nb_states,1)),-1)
             new_states = np.repeat(np.mod(np.arange(cur_Bs_cat.shape[1]*nb_states, dtype = 'int8'),nb_states)[None,:,None,None] == np.arange(nb_states, dtype = 'int8')[None,None,None], cur_Bs_cat.shape[0], 0).astype('int8')
             cur_Bs_cat = np.concatenate((new_states, np.repeat(cur_Bs_cat,nb_states,1)),-2)
                 
         cur_states = cur_Bs[:,:,0:nb_substeps+1].astype(int)
         len(cur_Bs[0])
         LT = get_Ts_from_Bs(cur_states, TrMat)
-        #cur_states = cur_states[:,:,0]
         # repeat the previous matrix to account for the states variations due to the new position
         m_arr = cp.repeat(m_arr, nb_states**nb_substeps , axis = 1)
         s2_arr = cp.repeat(s2_arr, nb_states**nb_substeps, axis = 1)
         LP = cp.repeat(LP, nb_states**nb_substeps, axis = 1)
         
-        #LL = Lp_stay[np.argmax(np.all(cur_states[:,None] == sub_Bs[:,:,None],-1),1)] # pick the right proba of staying according to the current states
-        #end_p_stay = p_stay[np.argmax(np.all(cur_states[:,None:,:-1] == sub_Bs[:,:,None],-1),1)]
         end_p_stay = p_stay[cur_states[:,None:,:-1]][:,:,0]
-        end_p_stay.shape
         LL = cp.log(pBL + (1-end_p_stay) - pBL * (1-end_p_stay)) + LT
     
     new_s2_arr = cp.array((s2_arr + LocErr2[:,:, min(LocErr_index, nb_locs-current_step)]))
     log_integrated_term = cp.sum(-0.5*cp.log(2*np.pi*new_s2_arr) - (Cs[:,:,0] - m_arr)**2/(2*new_s2_arr),axis=2)
     #LF = cp.log(Fs[cur_Bs[:,:,0].astype(int)]) # Log proba of starting in a given state (fractions)
     #LF = cp.log(0.5)
     # cp.mean(cp.log(Fs[cur_Bs[:,:,:].astype(int)]), 2) # Log proba of starting in a given state (fractions)
@@ -670,182 +618,14 @@
     P = np.exp(pred_LP)
     sum_P = np.sum(P, axis = 1, keepdims = True)[:,:,None]
     if do_preds :
         preds = np.sum(P[:,:,None,None]*cur_Bs_cat, axis = 1) / sum_P
         preds = preds[:,::-1]
     return LP, cur_Bs_cat, preds
 
-"""
-np.argmax(cur_Bs_cat,3)[:,:,-10:]
-
-cur_Bs_cat.shape
-
-cur_Bs_cat[0,:,:10,1]
-
-cur_Bs_cat[0,:,:,1]
-m_arr.shape
-plt.figure()
-
-ID = -1
-
-plt.scatter(m_arr[ID, :, 0], s2_arr[ID, :, 0]**0.5)
-for B_ID in range(cur_Bs_cat.shape[1]):
-    plt.annotate(list(np.argmax(cur_Bs_cat,3)[ID, B_ID, -10:]), np.array([m_arr[ID, B_ID, 0], s2_arr[ID, B_ID, 0]**0.5]))
-
-plt.figure()
-plt.scatter(m_arr[ID, :, 0], s2_arr[ID, :, 0]**0.5)
-for B_ID in range(cur_Bs_cat.shape[1]):
-    plt.annotate(cur_Bs_cat[ID,B_ID,:,1], np.array([m_arr[ID, B_ID, 0], s2_arr[ID, B_ID, 0]**0.5]))
-
-m_arr.shape
-
-plt.figure()
-plt.scatter(m_arr[ID, :, 1], s2_arr[ID, :, 0]**0.5)
-for B_ID in range(cur_Bs_cat.shape[1]):
-    plt.annotate(np.round(cur_Bs_cat[ID, B_ID, :, 1], 2), np.array([m_arr[ID, B_ID, 1], s2_arr[ID, B_ID, 0]**0.5]))
-
-
-np.argmax(cur_Bs_cat,3)[ID,:,-10:].shape
-list(np.argmax(cur_Bs_cat,3)[ID,:,-10:])
-
-ID = 4
-
-LP[ID]
-cur_Bs_cat[ID,1]
-
-preds = np.sum(P[:,:,None,None]*cur_Bs_cat, axis = 1) / sum_P
-
-preds.shape
-cur_Bs_cat.shape
-
-np.mean(np.sum(preds[:,5],1) >0.9999)
-
-ID+=1
-for ID in range(200):
-    plt.plot(Cs[ID,0,:,0], Cs[ID,0,:,1], 'k:', alpha = 0.5)
-    plt.scatter(Cs[ID,0,:,0], Cs[ID,0,:,1], c = cm.jet(preds[ID,:,0]))
-    plt.gca().set_aspect('equal', adjustable='datalim')
-
-np.std(Cs[ID,0], 0)
-
-
-cur_Bs_cat[ID, np.argmax(P[ID])]
-
-
-preds[0]
-
-cur_Bs_cat[3,10]
-cur_Bs_cat.shape
-cur_Bs_cat[:,:,:,state]
-P.shape
-np.mean((cur_Bs_cat>0)*(cur_Bs_cat<1))
-
-"""
-
-"""
-def fuse_tracks_th(m_arr, s2_arr, LP, cur_Bs, nb_Tracks, preds, nb_states = 2, nb_dims = 2, do_preds = 1, threshold = 0.05):
-    '''
-    The probabilities of the pairs of tracks must be added
-    I chose to define the updated m_arr and s2_arr as the weighted average (of the variance for s2_arr)
-    but other methods may be better
-    As I must divid by a sum of exponentials which can be equal to zero because of underflow
-    I correct the values in the exponetial to keep the maximal exp value at 0
-    '''
-    # cut the matrixes so the resulting matrices only vary for their last state
-    
-    s_arr = s2_arr**0.5
-    
-    groups = []
-    grouped_IDs = []
-
-    for Bs_ID in range(m_arr.shape[1]):
-        if not np.isin(Bs_ID, grouped_IDs):
-            cur_m_arr = m_arr[:,Bs_ID]
-            cur_s_arr = s_arr[:,Bs_ID]
-            
-            m_mask = np.mean((np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr) < threshold, (0, 2)) == 1
-            s_mask = ((cur_s_arr[:,None] > (1 - threshold) * s_arr)*(cur_s_arr[:,None] < (1 + threshold) * s_arr))[0,:,0]
-            args = np.where(m_mask * s_mask)[0]
-            
-            args = args[np.isin(args, grouped_IDs) == False] # remove elements that already belongs to a group
-            
-            groups.append(args)
-            grouped_IDs = grouped_IDs + list(args)
-
-    
-    np.sum(cur_Bs)
-    np.sum(LP)
-    np.sum(m_arr)
-    np.sum(s2_arr)
-    np.where(s2_arr == 0)
-    
-    if len(grouped_IDs) != m_arr.shape[1]:
-        raise ValueError('problem with grouping: len(grouped_IDs)=' + str(len(grouped_IDs)) + ' and m_arr.shape[1]=' + str( m_arr.shape[1]))
-    '''
-    np.sort(grouped_IDs)
-    
-    np.abs(m_arr - cur_m_arr[:,None]).shape
-    (np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr)[:,28]
-    
-    ((np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr) < threshold).shape
-    
-    ((np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr) < threshold).shape
-    
-    np.mean((np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr) < threshold, (0, 2))[28]
-    
-    (np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr)[:,28] < threshold
-    
-    (np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr) < threshold
-    
-    np.where((np.sum(np.abs(m_arr - cur_m_arr[:,None]), 2, keepdims = True)/s_arr)[:,28] != 0)
-    
-    np.abs(m_arr - cur_m_arr[:,None])[459]
-    m_arr[459]
-    
-    LP[459,]
-    cur_Bs[459, 28]
-    
-    m_arr.shape
-    '''
-    subgroups = []
-    for group in groups:
-        for state in range(nb_states):
-            subgroup = group[cur_Bs[:, group][0,:,0] == state]
-            if len(subgroup)>0:
-                subgroups.append(subgroup)
-    
-    nb_subgroups = len(subgroups)
-    if do_preds == 0:
-        new_cur_Bs = np.zeros((1, nb_subgroups, 1), dtype=(int))-1
-    else:
-        new_cur_Bs = np.zeros((nb_Tracks, nb_subgroups, cur_Bs.shape[2]))-1
-    new_m_arr = np.zeros((nb_Tracks, nb_subgroups, m_arr.shape[2]))
-    new_s2_arr = np.zeros((nb_Tracks, nb_subgroups, s2_arr.shape[2]))
-    new_LP = np.zeros((nb_Tracks, nb_subgroups))
-    
-    #subgroup = subgroups[14]
-    #Bs_ID = 14
-    for Bs_ID, subgroup in enumerate(subgroups):
-        #if len(subgroup)>1:
-        #    fsdsdff
-        max_LP = LP[:, subgroup].max(axis = 1, keepdims = True)
-        weights = np.exp(LP[:, subgroup] - max_LP)
-        
-        if do_preds == 0:
-            new_cur_Bs[:, Bs_ID] = cur_Bs[:, subgroup[:1], 0]
-        else:
-            new_cur_Bs[:, Bs_ID] = (np.sum(weights[:,:,None] * cur_Bs[:, subgroup, :], 1) / np.sum(weights, 1, keepdims = True))
-        
-        new_m_arr[:, Bs_ID] = np.sum(weights[:,:,None] * m_arr[:, subgroup, :], 1) / np.sum(weights, 1, keepdims = True)
-        new_s2_arr[:, Bs_ID] = np.sum(weights[:,:,None] * s2_arr[:, subgroup, :], 1) / np.sum(weights, 1, keepdims = True)
-        new_LP[:, Bs_ID] = np.sum(LP[:, subgroup],1)
-    
-    return new_m_arr, new_s2_arr, new_LP, new_cur_Bs
-"""
-
 def fuse_tracks_th(m_arr, s2_arr, LP, cur_Bs, cur_Bs_cat, nb_Tracks, nb_states = 2, nb_dims = 2, do_preds = 1, threshold = 0.2, frame_len = 6):
     '''
     The probabilities of the pairs of tracks must be added
     I chose to define the updated m_arr and s2_arr as the weighted average (of the variance for s2_arr)
     but other methods may be better
     As I must divid by a sum of exponentials which can be equal to zero because of underflow
     I correct the values in the exponetial to keep the maximal exp value at 0
@@ -894,41 +674,15 @@
                 subgroups.append(subgroup)
     
     # part that is too time consuming, find a way to make it faster
     nb_subgroups = len(subgroups)
     new_cur_Bs = np.empty((1, nb_subgroups, 1), dtype=(int))
     if not do_preds:
         cur_Bs_cat = cur_Bs_cat[:,:,:frame_len]
-    '''
-    new_cur_Bs_cat = np.zeros((nb_Tracks, nb_subgroups, cur_Bs_cat.shape[2], nb_dims), dtype = cur_Bs_cat.dtype)
 
-    new_m_arr = np.zeros((nb_Tracks, nb_subgroups, m_arr.shape[2]),  dtype = m_arr.dtype)
-    new_s2_arr = np.zeros((nb_Tracks, nb_subgroups, s2_arr.shape[2]),  dtype = s2_arr.dtype)
-    new_LP = np.zeros((nb_Tracks, nb_subgroups),  dtype = LP.dtype)
-    
-    for Bs_ID, subgroup in enumerate(subgroups):
-        
-        max_LP = LP[:, subgroup].max(axis = 1, keepdims = True)
-        weights = np.exp(LP[:, subgroup] - max_LP)
-        sum_weights = np.sum(weights, 1, keepdims = True)
-        new_cur_Bs[:, Bs_ID] = cur_Bs[:, subgroup[:1], 0]
-        
-        new_cur_Bs_cat[:, Bs_ID] = (np.sum(weights[:,:,None,None] * cur_Bs_cat[:, subgroup, :], 1) / sum_weights[:,:,None])
-        #new_cur_Bs[:, Bs_ID] = (np.sum(weights[:,:,None] * cur_Bs[:, subgroup, :], 1) / )
-        
-        new_m_arr[:, Bs_ID] = np.sum(weights[:,:,None] * m_arr[:, subgroup, :], 1) / sum_weights
-        new_s2_arr[:, Bs_ID] = np.sum(weights[:,:,None] * s2_arr[:, subgroup, :], 1) / sum_weights
-        new_LP[:, Bs_ID] = np.log(np.sum(np.exp(LP[:, subgroup]-max_LP), axis = 1)) + np.squeeze(max_LP, axis = 1)
-
-    # part that is too time consuming, find a way to make it faster
-    nb_subgroups = len(subgroups)
-    new_cur_Bs = np.zeros((1, nb_subgroups, 1), dtype=(int))
-    if not do_preds:
-        cur_Bs_cat = cur_Bs_cat[:,:,:frame_len]
-    '''  
     new_cur_Bs_cat = np.zeros((nb_Tracks, nb_subgroups, cur_Bs_cat.shape[2], nb_states), dtype = cur_Bs_cat.dtype)
     
     new_m_arr = np.zeros((nb_Tracks, nb_subgroups, m_arr.shape[2]),  dtype = m_arr.dtype)
     new_s2_arr = np.zeros((nb_Tracks, nb_subgroups, s2_arr.shape[2]),  dtype = s2_arr.dtype)
     new_LP = np.zeros((nb_Tracks, nb_subgroups),  dtype = LP.dtype)
     
     for Bs_ID, subgroup in enumerate(subgroups):
@@ -1060,34 +814,30 @@
         if k == len(all_tracks)-1:
             isBL = 0 # last position correspond to tracks which didn't disapear within maximum track length
         else:
             isBL = 1
         Css = all_tracks[k]
         if input_LocErr != None:
             sigs = LocErr[k]
-        nb_max = 50
+        nb_max = 500
         for n in range(int(np.ceil(len(Css)/nb_max))):
             Csss.append(Css[n*nb_max:(n+1)*nb_max])
             if input_LocErr != None:
                 sigss.append(sigs[n*nb_max:(n+1)*nb_max])
             if Css.shape[1] == max_len:
                 isBLs.append(0) # last position correspond to tracks which didn't disapear within maximum track length
             else:
                 isBLs.append(1)
-    #Csss.reverse()
-    #sigss.reverse()
     do_preds = 1
     args_prod = np.array(list(product(Csss, [0], [ds], [Fs], [TrMat],[pBL], [0],[cell_dims], [nb_substeps], [frame_len], [do_preds], [min_len])), dtype=object)
     args_prod[:, 6] = isBLs
     if input_LocErr != None:
         args_prod[:,1] = sigss
     else:
         args_prod[:,1] = LocErr
-
-    Cs, LocErr, ds, Fs, TrMat,pBL,isBL, cell_dims, nb_substeps, frame_len, do_preds, min_len = args_prod[3]
     
     if workers >= 2:
         with multiprocessing.Pool(workers) as pool:
             all_pred_Bs = pool.map(Pool_star_P_inter, args_prod)
     else:
         all_pred_Bs = []
         for args in args_prod:
@@ -1211,14 +961,15 @@
                     sigss.append(sigs[n*nb_max:(n+1)*nb_max])
                 if Css.shape[1] == max_len:
                     isBLs.append(0) # last position correspond to tracks which didn't disapear within maximum track length
                 else:
                     isBLs.append(1)
         Csss.reverse()
         sigss.reverse()
+        isBLs.reverse()
         
         args_prod = np.array(list(product(Csss, [0], [ds], [Fs], [TrMat],[pBL], [0],[cell_dims], [nb_substeps], [frame_len], [min_len], [threshold], [max_nb_states])), dtype=object)
         args_prod[:, 6] = isBLs
         if input_LocErr != None:
             args_prod[:,1] = sigss
         else:
             args_prod[:,1] = LocErr
@@ -1243,15 +994,15 @@
             print('.', end='')
         out = - Cum_P # normalize by the number of tracks and number of displacements
     else:
         out = np.inf
         print('x',end='')
         if verbose == 1:
             q = [param + ' = ' + str(np.round(params[param].value, 4)) for param in params]
-            print(Cum_P, q)
+            print(q)
     if np.isnan(out):
         out = np.inf
         print('input parameters give nans, you may want to pick more suitable parameter initial values')
     #print(time() - t0)
     return out
 
 def get_params(nb_states = 2,
@@ -1496,39 +1247,15 @@
                         params[param].value = cur_params[param].value
                         L = cur_L
                         momentum[param] = np.abs(momentum[param]-1)
                         history.append({'params': params, 'L': L, 'steps': steps, 'momentum': momentum})
                         steps[param] = steps[param]*0.8
                     else: # if none of the values tested are better, we reduce the step size and redo an iteration
                         steps[param] = steps[param]*0.5
-                    #    step = np.min([steps[param] * (params[param].value - params[param].min), steps[param] * (params[param].max - params[param].value)])
-                    #    cur_steps = [- step, step]
-                    #    cur_params[param].value = params[param].value + cur_steps[momentum[param]]
-                    #    cur_L = - cum_Proba_Cs(cur_params, *args)
-                    #    if cur_L > L:
-                    #        params[param].value = cur_params[param].value
-                    #        L = cur_L
-                    #        history.append({'params': params, 'L': L})
-                    #    else:
-                    #        cur_params[param].value = params[param].value + cur_steps[np.abs(momentum[param]-1)]
-                    #        cur_L = -cum_Proba_Cs(cur_params, *args)
-                    #        if cur_L > L:
-                    #            params[param].value = cur_params[param].value
-                    #            L = cur_L
-                    #            momentum[param] = np.abs(momentum[param]-1)
-                    #            history.append({'params': params, 'L': L})
-                    #        else: # if none of the values tested are better, we reduce the step size
-                    #            steps[param] = steps[param]*0.5
-        #print('L', L)
-        #q = ''
-        #for param in params:
-        #    q = q + param + ':' + str(np.round(params[param].value, 6)) + ', '
-        #print(q)
-        #print('steps:' , steps)
-
+                
     class Fit(object):
         pass
 
     fit = Fit()
     fit.params = params
     fit.residual = [L]
     fit.history = history
@@ -1549,75 +1276,33 @@
                   steady_state = False,
                   cell_dims = [1], # list of dimensions limit for the field of view (FOV) of the cell in um, a membrane protein in a typical e-coli cell in tirf would have a cell_dims = [0.5,3], in case of cytosolic protein one should imput the depth of the FOV e.g. [0.3] for tirf or [0.8] for hilo
                   input_LocErr = None, 
                   threshold = 0.2, 
                   max_nb_states = 120):
     
     '''
-    vary_params = {'LocErr' : [True, True], 'D0' : True, 'D1' : True, 'F0' : True, 'p01' : True, 'p10' : True, 'pBL' : True}
-    estimated_vals =  {'LocErr' : [0.025, 0.03], 'D0' : 1e-20, 'D1' : 0.05, 'F0' : 0.45, 'p01' : 0.05, 'p10' : 0.05, 'pBL' : 0.1}
-    min_values = {'LocErr' : [0.007, 0.007], 'D0' : 1e-12, 'D1' : 0.00001, 'F0' : 0.001, 'p01' : 0.001, 'p10' : 0.001, 'pBL' : 0.001}
-    max_values = {'LocErr' : [0.6, 0.6], 'D0' : 1, 'D1' : 10, 'F0' : 0.999, 'p01' : 1., 'p10' : 1., 'pBL' : 0.99}
-    
     fitting the parameters to the data set
     arguments:
-    all_tracks: dict describing the tracks with track length as keys (number of time positions, e.g. '23') of 3D arrays: dim 0 = track, dim 1 = time position, dim 2 = x, y position.
-    dt: time in between frames.
-    cell_dims: dimension limits (um).
-    nb_substeps: number of virtual transition steps in between consecutive 2 positions.
-    nb_states: number of states. estimated_vals, min_values, max_values should be changed accordingly to describe all states and transitions.
-    frame_len: number of frames for which the probability is perfectly computed. See method of the paper for more details.
-    verbose: if 1, print the intermediate values for each iteration of the fit.
+    all_tracks: Dictionary describing the tracks with track length as keys (number of time positions, e.g. '23') of 3D arrays: dim 0 = track, dim 1 = time position, dim 2 = x, y position. This means 15 tracks of 7 time points in 2D will correspond to an array of shape [15,7,2].
+    dt: Time in between frames.
+    params: Parameters previously instanciated.
+    nb_states: Number of states. vary_params, estimated_vals, min_values, max_values should be changed accordingly to describe all states and transitions.
+    nb_substeps: Number of considered transition steps in between consecutive 2 positions.
+    frame_len: Number of frames for which the probability is perfectly computed. See method of the paper for more details.
+    verbose: If 1, print the intermediate values for each iteration of the fit.
     steady_state: True if tracks are considered at steady state (fractions independent of time), this is most likely not true as tracks join and leave the FOV.
-    vary_params: dict specifying if each parameters should be changed (True) or not (False).
-    estimated_vals: initial values of the fit. (stay constant if parameter fixed by vary_params). estimated_vals must be in between min_values and max_values even if fixed.
-    min_values: minimal values for the fit.
-    max_values: maximal values for the fit.
+    workers: Number of workers used for the fitting, allows to speed up computation. Do not work from windows at the moment.
+    input_LocErr: Optional peakwise localization errors used as an input with the same format than all_tracks.
+    cell_dims: Dimension limits (um) (default [1], can also be [1,2] for instance in case of two limiting dimensions).
+    threshold: threshold for the fusion of the sequences of states (default value = 0.2). The threshold is applied to mu the mean position and s the standard deviation of the particle position (see the article for more details).
+    max_nb_states: maximum number of sequences of states to consider.
+    method: Optimization method used by the lmfit package (default = 'BFGS'). Other methods may not work.
+
     outputs:
     model_fit: lmfit model
-    
-    in case of 3 states models vary_params, estimated_vals, min_values and max_values can be replaced :
-    
-    vary_params = {'LocErr' : True, 'D0' : False, 'D1' :  True, 'D2' : True, 'F0' : True, 'F1' : True, 'p01' : True, 'p02' : True, 'p10' : True,'p12' :  True,'p20' :  True, 'p21' : True, 'pBL' : True},
-    estimated_vals = {'LocErr' : 0.023, 'D0' : 1e-20, 'D1' : 0.02, 'D2' :  0.1, 'F0' : 0.33,  'F1' : 0.33, 'p01' : 0.1, 'p02' : 0.1, 'p10' :0.1, 'p12' : 0.1, 'p20' :0.1, 'p21' :0.1, 'pBL' : 0.1},
-    min_values = {'LocErr' : 0.007, 'D0' : 1e-20, 'D1' : 0.0000001, 'D2' :  0.000001, 'F0' : 0.001,  'F1' : 0.001, 'p01' : 0.001, 'p02' : 0.001, 'p10' :0.001, 'p12' : 0.001, 'p20' :0.001, 'p21' :0.001, 'pBL' : 0.001},
-    max_values = {'LocErr' : 0.6, 'D0' : 1e-20, 'D1' : 1, 'D2' :  10, 'F0' : 0.999,  'F1' : 0.999, 'p01' : 1, 'p02' : 1, 'p10' : 1, 'p12' : 1, 'p20' : 1, 'p21' : 1, 'pBL' : 0.99}
-    
-    in case of 4 states models :
-    
-    vary_params = {'LocErr' : True, 'D0' : True, 'D1' : True, 'D2' :  True, 'D3' : True, 'F0' : True,  'F1' : True, 'F2' : True, 'p01' : True, 'p02' : True, 'p03' : True, 'p10' : True, 'p12' : True, 'p13' : True, 'p20' :True, 'p21' :True, 'p23' : True, 'p30' :True, 'p31' :True, 'p32' : True, 'pBL' : True}
-    estimated_vals = {'LocErr' : 0.023, 'D0' : 1e-20, 'D1' : 0.02, 'D2' :  0.1, 'D3' : 0.5, 'F0' : 0.1,  'F1' : 0.2, 'F2' : 0.3, 'p01' : 0.1, 'p02' : 0.1, 'p03' : 0.1, 'p10' :0.1, 'p12' : 0.1, 'p13' : 0.1, 'p20' :0.1, 'p21' :0.1, 'p23' : 0.1, 'p30' :0.1, 'p31' :0.1, 'p32' : 0.1, 'pBL' : 0.1}
-    min_values = {'LocErr' : 0.005, 'D0' : 0, 'D1' : 0, 'D2' :  0.001, 'D3' : 0.001, 'F0' : 0.001,  'F1' : 0.001, 'F2' : 0.001, 'p01' : 0.001, 'p02' : 0.001, 'p03' : 0.001, 'p10' :0.001, 'p12' : 0.001, 'p13' : 0.001, 'p20' :0.001, 'p21' :0.001, 'p23' : 0.001, 'p30' :0.001, 'p31' :0.001, 'p32' : 0.001, 'pBL' : 0.001}
-    max_values = {'LocErr' : 0.023, 'D0' : 1, 'D1' : 1, 'D2' :  10, 'D3' : 100, 'F0' : 0.999,  'F1' : 0.999, 'F2' : 0.999, 'p01' : 1, 'p02' : 1, 'p03' : 1, 'p10' :1, 'p12' : 1, 'p13' : 1, 'p20' : 1, 'p21' : 1, 'p23' : 1, 'p30' : 1, 'p31' : 1, 'p32' : 1, 'pBL' : 0.99}
-    '''
-    '''
-    if nb_states == 2:
-        if not (len(min_values) == 7 and len(max_values) == 7 and len(estimated_vals) == 7 and len(vary_params) == 7):
-            raise ValueError('estimated_vals, min_values, max_values and vary_params should all containing 7 parameters')
-    elif nb_states == 3:
-        if len(vary_params) != 13:
-            vary_params = {'LocErr' : True, 'D0' : True, 'D1' :  True, 'D2' : True, 'F0' : True, 'F1' : True, 'p01' : True, 'p02' : True, 'p10' : True,'p12' :  True,'p20' :  True, 'p21' : True, 'pBL' : True},
-        if len(estimated_vals) != 13:
-            estimated_vals = {'LocErr' : 0.023, 'D0' : 1e-20, 'D1' : 0.02, 'D2' :  0.1, 'F0' : 0.33,  'F1' : 0.33, 'p01' : 0.1, 'p02' : 0.1, 'p10' :0.1, 'p12' : 0.1, 'p20' :0.1, 'p21' :0.1, 'pBL' : 0.1},
-        if len(min_values) != 13:
-            min_values = {'LocErr' : 0.007, 'D0' : 1e-20, 'D1' : 0.0000001, 'D2' :  0.000001, 'F0' : 0.001,  'F1' : 0.001, 'p01' : 0.001, 'p02' : 0.001, 'p10' :0.001, 'p12' : 0.001, 'p20' :0.001, 'p21' :0.001, 'pBL' : 0.001},
-        if len(max_values) != 13:
-            max_values = {'LocErr' : 0.023, 'D0' : 1, 'D1' : 1, 'D2' :  10, 'F0' : 0.999,  'F1' : 0.999, 'p01' : 1, 'p02' : 1, 'p10' :1, 'p12' : 1, 'p20' : 1, 'p21' : 1, 'pBL' : 0.99}
-    elif nb_states == 4:
-        if len(vary_params) != 21:
-            vary_params = {'LocErr' : True, 'D0' : True, 'D1' : True, 'D2' :  True, 'D3' : True, 'F0' : True,  'F1' : True, 'F2' : True, 'p01' : True, 'p02' : True, 'p03' : True, 'p10' : True, 'p12' : True, 'p13' : True, 'p20' :True, 'p21' :True, 'p23' : True, 'p30' :True, 'p31' :True, 'p32' : True, 'pBL' : True}
-        if len(estimated_vals) != 21:
-            estimated_vals = {'LocErr' : 0.023, 'D0' : 1e-20, 'D1' : 0.02, 'D2' :  0.1, 'D3' : 0.5, 'F0' : 0.1,  'F1' : 0.2, 'F2' : 0.3, 'p01' : 0.1, 'p02' : 0.1, 'p03' : 0.1, 'p10' :0.1, 'p12' : 0.1, 'p13' : 0.1, 'p20' :0.1, 'p21' :0.1, 'p23' : 0.1, 'p30' :0.1, 'p31' :0.1, 'p32' : 0.1, 'pBL' : 0.1}
-        if len(min_values) != 21:
-            min_values = {'LocErr' : 0.005, 'D0' : 0, 'D1' : 0, 'D2' :  0.001, 'D3' : 0.001, 'F0' : 0.001,  'F1' : 0.001, 'F2' : 0.001, 'p01' : 0.001, 'p02' : 0.001, 'p03' : 0.001, 'p10' :0.001, 'p12' : 0.001, 'p13' : 0.001, 'p20' :0.001, 'p21' :0.001, 'p23' : 0.001, 'p30' :0.001, 'p31' :0.001, 'p32' : 0.001, 'pBL' : 0.001}
-        if len(max_values) != 21:
-            max_values = {'LocErr' : 0.023, 'D0' : 1, 'D1' : 1, 'D2' :  10, 'D3' : 100, 'F0' : 0.999,  'F1' : 0.999, 'F2' : 0.999, 'p01' : 1, 'p02' : 1, 'p03' : 1, 'p10' :1, 'p12' : 1, 'p13' : 1, 'p20' : 1, 'p21' : 1, 'p23' : 1, 'p30' : 1, 'p31' : 1, 'p32' : 1, 'pBL' : 0.99}
-    
-    if not str(all_tracks.__class__) == "<class 'dict'>":
-        raise ValueError('all_tracks should be a dictionary of arrays with n there number of steps as keys')
     '''
     
     if params == None:
         params = generate_params(nb_states = nb_states,
                                LocErr_type = 1,
                                LocErr_bounds = [0.005, 0.1], # the initial guess on LocErr will be the geometric mean of the boundaries
                                D_max = 3, # maximal diffusion length allowed
@@ -1635,17 +1320,14 @@
                 sorted_LocErrs.append(input_LocErr[l])
     all_tracks = sorted_tracks
     if len(all_tracks) < 1:
         raise ValueError('No track could be detected. The loaded tracks seem empty. Errors often come from wrong input paths.')
 
     if input_LocErr != None:
         input_LocErr = sorted_LocErrs
-    #if frame_len <= nb_substeps:
-    #    print('Warning frame_len has to be at least nb_substeps + 1')
-    #    frame_len = nb_substeps + 1
     
     fit = minimize(cum_Proba_Cs, params, args=(all_tracks, dt, cell_dims,input_LocErr, nb_states, nb_substeps, frame_len, verbose, workers, Matrix_type, threshold, max_nb_states), method = method, nan_policy = 'propagate')
     if verbose == 0:
         print('')
         
     '''
     #to inverse state indexes:
```

### Comparing `extrack-1.5.6/extrack/tracking_0.py` & `extrack-1.5.7/extrack/tracking_0.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack/visualization.py` & `extrack-1.5.7/extrack/visualization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.6/extrack.egg-info/PKG-INFO` & `extrack-1.5.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-Metadata-Version: 2.1
-Name: extrack
-Version: 1.5.6
-Summary: SPT kinetic modelling and states annotation of tracks
-Home-page: https://github.com/FrancoisSimon/ExTrack-python3
-Author: Francois Simon
-Author-email: simon.francois@protonmail.com
-Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-ExTrack
--------
-
-This repository contains the necessary scripts to run the method ExTrack. ExTrack is a method to detemine kinetics of particles able to transition between different motion states. It can assess diffusion coefficients, transition rates, localization error as well as annotating the probability for any track to be in each state for every time points. It can produce histograms of durations in each state to highlight no markovian transition kinetics. Eventually it can be used to refine the localization precision of tracks by considering the most likely positions which is especially efficient when the particle do not move.
-
-More details on the methods are available on BioarXiv https://www.biorxiv.org/content/10.1101/2022.07.13.499913v1.
-
-ExTrack has been designed and implemented by François Simon in the laboratory of Sven van Teeffelen at University of Montreal. ExTrack is primarerly implemented as a python package. An additional version of ExTrack is available on Fiji via Trackmate thanks to Jean-Yves Tinevez with reduced functionality https://sites.imagej.net/TrackMate-ExTrack/. 
-
-See the Wiki section for more information on how to install and use ExTrack.
-
-https://pypi.org/project/extrack/
-
-# Dependencies
-
-- numpy
-- lmfit
-- xmltodict
-- matplotlib
-- pandas
-
-Optional: jupyter, cupy
-
-# Installation (from pip)
-
-(needs to be run in anaconda prompt for anaconda users on windows)
-
-## Install dependencies
-
-`pip install numpy lmfit xmltodict matplotlib pandas`
-
-## Install ExTrack
-
-`pip install extrack`
-
-https://pypi.org/project/extrack/
-
-the current version (1.5) has working but oudated version of the position refinement method. It may only work for 2-state models. This will be updated as soon as possible.
-
-## Input file format
-
-ExTrack can deal with tracks saved with TrackMate xml format or csv format by using the integrated readers https://github.com/vanTeeffelenLab/ExTrack/wiki/Loading-data-sets.
-
-# Installation from this GitHub repository
-
-## From Unix/Mac:
-
-`sudo apt install git` (if git is not installed)
-
-`git clone https://github.com/FrancoisSimon/ExTrack.git`
-
-`cd ExTrack`
-
-`sudo python setup.py install`
-
-## From Windows using anaconda prompt:
-
-Need to install git if not already installed.
-
-`git clone https://github.com/vanTeeffelenLab/ExTrack.git` One can also just manually download the package if git is not installed. Once extracted the folder may be named ExTrack-main
-
-`cd ExTrack` or cd `ExTrack-main`
-
-`python setup.py install` from the ExTrack directory
-
-# Tutorial
-
-Tutorials for the python package of ExTrack are available.
-
-A first tutorial allows the user to have an overview of all the possibilities of the different modules of ExTrack (https://github.com/vanTeeffelenLab/ExTrack/blob/main/Tutorials/Tutorial_ExTrack.ipynb). This jupyter notebook tutorial shows the whole pipeline:
-- Loading data sets (https://github.com/vanTeeffelenLab/ExTrack/wiki/Loading-data-sets).
-- Initialize parameters of the model (https://github.com/vanTeeffelenLab/ExTrack/wiki/Parameters-for-fitting).
-- Fitting.
-- Probabilistic state annotation.
-- Histograms of state duration.
-- Position refinement.
-- Saving results.
-
-from loading data sets to saving results
-at these location: 
-- tests/test_extrack.py
-- or Tutorials/tutorial_extrack.ipynb
-
-These contain the most important modules in a comprehensive framework. We recommand following the tutorial tutorial_extrack.ipynb which uses Jupyter notebook as it is more didactic. One has to install jupyter to use it: `pip install jupyter` in the anaconda prompt for conda users. 
-
-**Document here how to open a Jupyter notebook**
-
-# Usage
-## Main functions
-
-extrack.tracking.param_fitting : performs the fit to infer the parameters of a given data set.
-
-extrack.visualization.visualize_states_durations : plot histograms of the duration in each state.
-
-extrack.tracking.predict_Bs : predicts the states of the tracks.
-
-## Extra functions
-
-extrack.simulate_tracks.sim_FOV : allows to simulate tracks.
-
-extrack.exporters.extrack_2_pandas : turn the outputs from ExTrack to a pandas dataframe. outputed dataframe can be save with dataframe.to_csv(save_path)
-
-extrack.exporters.save_extrack_2_xml : save extrack data to xml file (trackmate format).
-
-extrack.visualization.visualize_tracks : show all tracks in a single plot.
-
-extrack.visualization.plot_tracks : show the longest tracks on separated plots
-
-## Caveats
-
-# References
-
-# License
-This program is released under the GNU General Public License version 3 or upper (GPLv3+).
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-# Parallelization
-
-Multiple CPU Parallelization can be performed in get_2DSPT_params with the argument worker the number of cores used for the job (equal to 1 by default).
-Warning: Do not work on windows.
-
-GPU parallelization used to be available but may not be compatible with the current CPU parallelization, GPU parallelization uses the package cupy which can be installed as described here : https://github.com/cupy/cupy. The cupy version will depend on your cuda version which itself must be compatible with your GPU driver and GPU. Usage of cupy requires a change in the module extrack/tracking (line 4) : GPU_computing = True
-
-# Deploying (developer only)
-
-# Authors
-Francois Simon
-
-# Bugs/suggestions
-Send to bugtracker or to email.
-
-# to do
-
-- Redo the script for Refined positions to match the current version.
-- Try approximations based on 'm' and 's' values instead of fixed window length.
+Metadata-Version: 2.1
+Name: extrack
+Version: 1.5.7
+Summary: SPT kinetic modelling and states annotation of tracks
+Home-page: https://github.com/FrancoisSimon/ExTrack-python3
+Author: Francois Simon
+Author-email: simon.francois@protonmail.com
+Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ExTrack
+-------
+
+This repository contains the necessary scripts to run the method ExTrack. ExTrack is a method to detemine kinetics of particles able to transition between different motion states. It can assess diffusion coefficients, transition rates, localization error as well as annotating the probability for any track to be in each state for every time points. It can produce histograms of durations in each state to highlight no markovian transition kinetics. Eventually it can be used to refine the localization precision of tracks by considering the most likely positions which is especially efficient when the particle do not move.
+
+More details on the methods are available on BioarXiv https://www.biorxiv.org/content/10.1101/2022.07.13.499913v1.
+
+ExTrack has been designed and implemented by François Simon in the laboratory of Sven van Teeffelen at University of Montreal. ExTrack is primarerly implemented as a python package. An additional version of ExTrack is available on Fiji via Trackmate thanks to Jean-Yves Tinevez with reduced functionality https://sites.imagej.net/TrackMate-ExTrack/. 
+
+See the Wiki section for more information on how to install and use ExTrack.
+
+https://pypi.org/project/extrack/
+
+# Dependencies
+
+- numpy
+- lmfit
+- xmltodict
+- matplotlib
+- pandas
+
+Optional: jupyter, cupy
+
+# Installation (from pip)
+
+(needs to be run in anaconda prompt for anaconda users on windows)
+
+## Install dependencies
+
+`pip install numpy lmfit xmltodict matplotlib pandas`
+
+## Install ExTrack
+
+`pip install extrack`
+
+https://pypi.org/project/extrack/
+
+the current version (1.5) has working but oudated version of the position refinement method. It may only work for 2-state models. This will be updated as soon as possible.
+
+## Input file format
+
+ExTrack can deal with tracks saved with TrackMate xml format or csv format by using the integrated readers https://github.com/vanTeeffelenLab/ExTrack/wiki/Loading-data-sets.
+
+# Installation from this GitHub repository
+
+## From Unix/Mac:
+
+`sudo apt install git` (if git is not installed)
+
+`git clone https://github.com/vanTeeffelenLab/ExTrack.git`
+
+`cd ExTrack`
+
+`sudo python setup.py install`
+
+## From Windows using anaconda prompt:
+
+Need to install git if not already installed.
+
+`git clone https://github.com/vanTeeffelenLab/ExTrack.git` One can also just manually download the package if git is not installed. Once extracted the folder may be named ExTrack-main
+
+`cd ExTrack` or cd `ExTrack-main`
+
+`python setup.py install` from the ExTrack directory
+
+# Tutorial
+
+Tutorials for the python package of ExTrack are available.
+
+A first tutorial allows the user to have an overview of all the possibilities of the different modules of ExTrack (https://github.com/vanTeeffelenLab/ExTrack/blob/main/Tutorials/Tutorial_ExTrack.ipynb). This jupyter notebook tutorial shows the whole pipeline:
+- Loading data sets (https://github.com/vanTeeffelenLab/ExTrack/wiki/Loading-data-sets).
+- Initialize parameters of the model (https://github.com/vanTeeffelenLab/ExTrack/wiki/Parameters-for-fitting).
+- Fitting.
+- Probabilistic state annotation.
+- Histograms of state duration.
+- Position refinement.
+- Saving results.
+
+from loading data sets to saving results
+at these location: 
+- tests/test_extrack.py
+- or Tutorials/tutorial_extrack.ipynb
+
+These contain the most important modules in a comprehensive framework. We recommand following the tutorial tutorial_extrack.ipynb which uses Jupyter notebook as it is more didactic. One has to install jupyter to use it: `pip install jupyter` in the anaconda prompt for conda users. 
+
+**Document here how to open a Jupyter notebook**
+
+# Usage
+## Main functions
+
+extrack.tracking.param_fitting : performs the fit to infer the parameters of a given data set.
+
+extrack.visualization.visualize_states_durations : plot histograms of the duration in each state.
+
+extrack.tracking.predict_Bs : predicts the states of the tracks.
+
+## Extra functions
+
+extrack.simulate_tracks.sim_FOV : allows to simulate tracks.
+
+extrack.exporters.extrack_2_pandas : turn the outputs from ExTrack to a pandas dataframe. outputed dataframe can be save with dataframe.to_csv(save_path)
+
+extrack.exporters.save_extrack_2_xml : save extrack data to xml file (trackmate format).
+
+extrack.visualization.visualize_tracks : show all tracks in a single plot.
+
+extrack.visualization.plot_tracks : show the longest tracks on separated plots
+
+## Caveats
+
+# References
+
+# License
+This program is released under the GNU General Public License version 3 or upper (GPLv3+).
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+# Parallelization
+
+Multiple CPU Parallelization can be performed in get_2DSPT_params with the argument worker the number of cores used for the job (equal to 1 by default).
+Warning: Do not work on windows.
+
+GPU parallelization used to be available but may not be compatible with the current CPU parallelization, GPU parallelization uses the package cupy which can be installed as described here : https://github.com/cupy/cupy. The cupy version will depend on your cuda version which itself must be compatible with your GPU driver and GPU. Usage of cupy requires a change in the module extrack/tracking (line 4) : GPU_computing = True
+
+# Deploying (developer only)
+
+# Authors
+Francois Simon
+
+# Bugs/suggestions
+Send to bugtracker or to email.
+
+# to do
+
+- Redo the script for Refined positions to match the current version.
+- Try approximations based on 'm' and 's' values instead of fixed window length.
```

### Comparing `extrack-1.5.6/setup.py` & `extrack-1.5.7/setup.py`

 * *Files identical despite different names*

