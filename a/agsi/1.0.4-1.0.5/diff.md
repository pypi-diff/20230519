# Comparing `tmp/agsi-1.0.4.tar.gz` & `tmp/agsi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.0.4.tar", last modified: Thu May 18 10:06:10 2023, max compression
+gzip compressed data, was "agsi-1.0.5.tar", last modified: Thu May 18 10:48:34 2023, max compression
```

## Comparing `agsi-1.0.4.tar` & `agsi-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.4/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:06:10.523172 agsi-1.0.4/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.4/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.4/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    13918 2023-05-18 10:00:01.000000 agsi-1.0.4/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.4/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   970300 2023-05-18 10:02:54.000000 agsi-1.0.4/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      325 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/top_level.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/dist/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     7045 2023-05-17 09:28:46.000000 agsi-1.0.4/dist/agsi-1.0.3.tar.gz
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-18 10:06:10.523172 agsi-1.0.4/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-18 10:05:58.000000 agsi-1.0.4/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:48:34.209498 agsi-1.0.5/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.5/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:48:34.209498 agsi-1.0.5/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.5/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:48:34.205498 agsi-1.0.5/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.5/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:48:34.209498 agsi-1.0.5/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    14067 2023-05-18 10:45:51.000000 agsi-1.0.5/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.5/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.5/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   970300 2023-05-18 10:02:54.000000 agsi-1.0.5/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.5/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.5/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:48:34.205498 agsi-1.0.5/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:48:34.000000 agsi-1.0.5/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-18 10:48:34.000000 agsi-1.0.5/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-18 10:48:34.000000 agsi-1.0.5/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-18 10:48:34.000000 agsi-1.0.5/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-18 10:48:34.000000 agsi-1.0.5/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-18 10:48:34.209498 agsi-1.0.5/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-18 10:48:32.000000 agsi-1.0.5/setup.py
```

### Comparing `agsi-1.0.4/README.md` & `agsi-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.0.4/agsi/data/FarmData.py` & `agsi-1.0.5/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
           # Iterate through rows and populate modalities and data fields
           for row in reader:
               info = {'owner': None, 'area': None,'data_path': {}}
               info['owner'] = row['farm_name']
               info['farm_id'] =row['farm_id']
               info['area'] = None
+              info['shp'] =row['shp']
               timestamp=row['time']
               
               info['data_path'][timestamp]={}
               for column in row:
                   # Check if the column name contains 'drone_' and get the resolution from the column name
                   if 'drone_' in column:
                       modality = column
@@ -109,14 +110,15 @@
                           image_path = row[column]
                           image_path = convert_path(image_path)
                           if column not in info['data_path'][timestamp]:
                               info['data_path'][timestamp][column]=image_path
 
               if info['farm_id'] in all_info:      
                 all_info[info['farm_id']]['data_path'][timestamp]=info['data_path'][timestamp]
+                all_info[info['farm_id']]['shp']=row['shp']
               else:
                 all_info[info['farm_id']]=info
 
       return all_info
   
   def __get_blocks_info__(self,block_csv_path):
         # Open CSV file
@@ -220,20 +222,20 @@
       farm_image_path=convert_path(farm_image_path)
       raster=open_tiff(farm_image_path)
       if only_rgb:
         return raster.read([1,2,3])
       else:
          return raster
     else: #to be implemented when accessing satellite images not in use right now.
-
-      shp_file=self.farm_df[self.farm_df["farm_id"]==self.farm_id]["shp_file"].values[0]
-      polygon=open_tiff(shp_file)['geometry'].values[0]
-      clipped_chip=get_clipped_chip(self.full_image_path,[polygon])
-      return clipped_chip,self.block
-
+      farm_image_path=self.info['data_path'][timestamp][modality_type]
+      farm_image_path=convert_path(farm_image_path)
+      shp_file=self.info["shp"]
+      polygon=open_shp(shp_file,"epsg:3857")['geometry'].values[0]
+      clipped_chip=get_clipped_chip(farm_image_path,[polygon])
+      return clipped_chip
   def visualize_blocks(self,modality_type="drone",resolution=75,timestamp=None):
 
     """
   Displays the farm image with the block polygons overlaid.
 
   Args:
       clip (bool, optional): Whether to clip the farm image to the extent of the block polygons. Defaults to True.
@@ -274,18 +276,14 @@
 
   def get_block_by_name(self,block_name):
   
     for block_key,block_obj in self.blocks.items():
       if block_obj.info['block_name']==block_name:
           return block_obj      
             
-
-
-
-    
 class Block():
 
   def __init__(self,block_info,farm_info):
       
       """
         A subclass of FarmData that represents a block and provides methods to access and manipulate block information.
```

### Comparing `agsi-1.0.4/agsi/data/utils.py` & `agsi-1.0.5/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.0.4/agsi/demo_V2.ipynb` & `agsi-1.0.5/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

