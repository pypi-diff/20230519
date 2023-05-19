# Comparing `tmp/hpverif-2.6.3-py3-none-any.whl.zip` & `tmp/hpverif-2.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13754 bytes, number of entries: 15
+Zip file size: 14086 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3046 b- defN 23-May-08 14:15 hpverif/Calibraton.py
 -rw-r--r--  2.0 unx      449 b- defN 23-May-08 15:40 hpverif/Driver.py
 -rw-r--r--  2.0 unx     3961 b- defN 23-May-08 14:15 hpverif/FrameCapture.py
 -rw-r--r--  2.0 unx     2576 b- defN 23-May-08 14:15 hpverif/FrameCapturePLY.py
 -rw-r--r--  2.0 unx     3967 b- defN 23-May-08 14:15 hpverif/PointCloud.py
--rw-r--r--  2.0 unx     5584 b- defN 23-May-15 15:28 hpverif/Segmentation.py
+-rw-r--r--  2.0 unx     5584 b- defN 23-May-19 14:09 hpverif/Segmentation.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-May-08 14:15 hpverif/ShowFiles.py
--rw-r--r--  2.0 unx     9966 b- defN 23-May-15 15:57 hpverif/Theoretical_distance.py
--rw-r--r--  2.0 unx     1876 b- defN 23-May-15 15:57 hpverif/Verification.py
+-rw-r--r--  2.0 unx    11845 b- defN 23-May-19 18:28 hpverif/Theoretical_distance.py
+-rw-r--r--  2.0 unx     1907 b- defN 23-May-19 18:28 hpverif/Verification.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-08 14:15 hpverif/__init__.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-08 14:15 hpverif/driver.py
--rw-r--r--  2.0 unx      321 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1159 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/RECORD
-15 files, 35837 bytes uncompressed, 11854 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx      321 b- defN 23-May-19 18:29 hpverif-2.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 18:29 hpverif-2.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-19 18:29 hpverif-2.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1160 b- defN 23-May-19 18:29 hpverif-2.6.4.dist-info/RECORD
+15 files, 37748 bytes uncompressed, 12186 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: hpverif/__init__.py
 Comment: 
 
 Filename: hpverif/driver.py
 Comment: 
 
-Filename: hpverif-2.6.3.dist-info/METADATA
+Filename: hpverif-2.6.4.dist-info/METADATA
 Comment: 
 
-Filename: hpverif-2.6.3.dist-info/WHEEL
+Filename: hpverif-2.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: hpverif-2.6.3.dist-info/top_level.txt
+Filename: hpverif-2.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hpverif-2.6.3.dist-info/RECORD
+Filename: hpverif-2.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpverif/Theoretical_distance.py

```diff
@@ -5,15 +5,15 @@
 
 class Theoretical_distance:
 
     def __init__ (self):
         pass
 
     def theoric_distance(self, mapa, point, angle_degrees, show):
-        #Carreguem mapa
+         #Carreguem mapa
         lines = self.loadMap(mapa)
 
         # Definim posició i angles (graus)
         #point, angle_degrees = (150, 100), 30
 
         #Ample de visió de la càmara d435i
         angle_FOV = 86/2
@@ -47,21 +47,21 @@
             interseccio_paret_aa.append(interseccio)
             if distancia > distancia_max: #Guardem el valor i index de la distancia maxima i per tant, cantonada
                 index_max = i-1
                 distancia_max = distancia
 
             if abs(distancia-d[i-1]) > 10: #Si hi ha salts de valors "grans" significa que la camara veu una columna
                 if not estam_veiem_columna: 
-                    print("entrem de la columna",i)
+                    #print("entrem de la columna",i)
                     index_columna_inici = i
                     estam_veiem_columna = True
                     hem_estat_columna = True
         
                 else:
-                    print("sortim de la columna",i)
+                    #print("sortim de la columna",i)
                     index_columna_final = i-1
                     estam_veiem_columna = False
 
             if distancia < distancia_min_c and estam_veiem_columna: #Veiem la cantonada de la columna
                 index_min_c = i
                 distancia_min_c = distancia
 
@@ -73,65 +73,84 @@
                 cares_columna = 1
             else:
                 cares_columna = 2
 
         plt.plot(angles,d)
         plt.xlabel("Degrees")
         plt.ylabel("Distancia")  
+        plt.xlim(-45,45)
+        plt.ylim(0, 300)
 
         #print(distancia_max,angles_distancia_max, index_max)
 
         
         #La paret es recte, per tant si el valor maxim esta al principi o al final, ja sabem que no topem cap cantonada
         #En el cas que el maxim no coincideixi amb inici o final, sabem que hi haura una cantonada
 
         if(abs(distancia_max-d[0]) < 0.01 or abs(distancia_max-d[len(scalar_angles)-1]) < 0.01):
             veiem_cantonada = False
         else:
             veiem_cantonada = True
 
         #--------------------< CALCUL DE LES DISTANCIES FINALS >--------------------
 
-        print("cares columna", cares_columna)
+        print("Faces the column:", cares_columna)
 
         if cares_columna == 0:
             if not veiem_cantonada: 
-                print("Veiem una paret")
+                print("Wall seen")
 
                 #Distancia mitja de la paret
                 dist = sum(d) / len(d)
 
             else:
-                print("Veiem cantonada (dues parets)")
+                print("Corner seen (2 walls)")
                 mean_1_np = np.mean(d[:index_max-1],dtype=np.float64)
                 mean_2_np = np.mean(d[index_max:],dtype=np.float64)
 
                 #Distacia mitja de les dues parets
-                dist = [mean_1_np, mean_2_np]
+
+                if index_max > len(scalar_angles)/2:
+                    dist = [mean_1_np, mean_2_np]
+                else:
+                    dist = [mean_2_np, mean_1_np]
+
 
         elif cares_columna == 1:
+            print("Column seen")
 
             mean_columna = np.mean(d[index_columna_inici:index_columna_final-1],dtype=np.float64)
             mean_paret_1 = np.mean(d[:index_columna_inici-1],dtype=np.float64)
             mean_paret_2 = np.mean(d[index_columna_final+1:],dtype=np.float64)
 
             #Distancia mitja de la de la columna i la dels dos trossos de paret
-            dist = [mean_columna, mean_paret_1, mean_paret_2]
+            if (len(scalar_angles) - index_columna_final > index_columna_inici):
+                dist = [mean_paret_2, mean_paret_1, mean_columna]
+            else:
+                dist = [mean_paret_1, mean_paret_2, mean_columna]
 
         elif cares_columna == 2:
-            print("Veiem columna amb dues cares")
+            print("2 faces of a column seen")
 
             mean_columna_a = np.mean(d[index_columna_inici:index_min_c-1],dtype=np.float64)
             mean_columna_b = np.mean(d[index_min_c:index_columna_final-1],dtype=np.float64)
             mean_paret_1 = np.mean(d[:index_columna_inici],dtype=np.float64)
             mean_paret_2 = np.mean(d[index_columna_final+1:],dtype=np.float64)
 
             #Distancia mitja de les dues cares (a i b) de la columna i la dels dos trossos de paret
-            dist = [mean_columna_a,mean_columna_b, mean_paret_1, mean_paret_2]
-
+            if index_columna_inici > len(scalar_angles) - index_columna_final:
+                if index_min_c - index_columna_inici > index_columna_final - index_min_c:
+                    dist = [ mean_paret_1, mean_paret_2, mean_columna_a,mean_columna_b]
+                else: 
+                    dist = [ mean_paret_1, mean_paret_2, mean_columna_b,mean_columna_a]
+            else: 
+                if index_min_c - index_columna_inici > index_columna_final - index_min_c:
+                    dist = [ mean_paret_2, mean_paret_1, mean_columna_a,mean_columna_b]
+                else: 
+                    dist = [ mean_paret_2, mean_paret_1, mean_columna_b,mean_columna_a]          
 
 
 
         #--------------------< REPRESENTACIÓ >--------------------
         if(show):
             #Creem mapa
             fig, ax = plt.subplots()
@@ -141,15 +160,15 @@
             for i in range(len(lines)):
                 x1, y1 = lines[i][0][0], lines[i][0][1]
                 x2, y2 = lines[i][1][0], lines[i][1][1]
                 ax.plot([x1, x2], [y1, y2], 'k-')
 
             #Mostrem distancia  
             #ax.plot([point[0],interseccio_paret[0]], [point[1],interseccio_paret[1]], 'g-', label=f'Central distance: {round(dist, 3)}' + ' cm.')
-            ax.scatter(point[0],point[1], label=f'Distance to object: {round(dist[0])}' + ' cm.', color='green', marker='o', s=30)
+            #ax.scatter(point[0],point[1], label=f'Distance to object: {round(dist[0])}' + ' cm.', color='green', marker='o', s=30)
 
             #Mostrem rang de visió de la càmara
             ax.plot([point[0],interseccio_paret_right[0]], [point[1],interseccio_paret_right[1]], 'r-', label=f'Field of view.')
             ax.plot([point[0],interseccio_paret_left[0]], [point[1],interseccio_paret_left[1]], 'r-')
 
             ax.legend(loc='upper left')
 
@@ -162,16 +181,22 @@
 
             #Establim valor de la distància teòrica
             #plt.text(interseccio_paret[0], interseccio_paret[1], f"{round(dist, 3)}" + " cm", ha='right', va='bottom')
             plt.text(point[0], point[1], f"{(point[0], point[1])}" + " cm  ", ha='right', va='bottom')
 
 
             plt.show()
+            self.print_distance(dist)
+
+        if cares_columna > 0:
+            columna = 1
+        else:
+            columna = 0
 
-        return dist
+        return dist, columna
     
     def line_intersection(self, line1, line2):
         x1, y1 = line1[0]
         x2, y2 = line1[1]
         x3, y3 = line2[0]
         x4, y4 = line2[1]
         det = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4)
@@ -226,8 +251,19 @@
         closest_distance = float("inf")
         for p in intersection_points:
             distance = self.distance_between_points(p, point)
             if distance < closest_distance:
                 closest_intersection_point = p
                 closest_distance = distance
 
-        return(closest_distance, closest_intersection_point)
+        return(closest_distance, closest_intersection_point)
+    
+    def print_distance(self,dist):
+        if isinstance(dist, float):
+            print("Distance to the wall: ",dist,"cm")
+        elif len(dist) == 2:
+            print("Distance to the most seen wall: ", dist[0],"cm", "\nDistance to the least seen wall: ", dist[1],"cm")
+        elif len(dist) == 3:
+            print("Distance to the most seen wall: ", dist[0],"cm", "\nDistance to the least seen wall: ", dist[1],"cm", "\nDistance to the column", dist[2],"cm")
+        elif len(dist) == 4:
+            print("Distance to the most seen wall: ", dist[0],"cm", "\nDistance to the least seen wall: ", dist[1],"cm", "\nDistance to the most seen face of the column: ", dist[2],"cm", "\nDistance to the least seen face of the column: ", dist[3],"cm")
+
```

## hpverif/Verification.py

```diff
@@ -39,21 +39,21 @@
        # km.CalculateKMeans(matrix, k)
     
     def pointCloud (self, dp, filename):
         pc = PointCloud()
         return pc.createPointCloud(0.001*np.asanyarray(dp.get_data()),filename)
         
     
-    def segmentation (self, filename, min, max , fact):
+    def segmentation (self, filename, min, max , fact, column):
         seg = Segmentation(filename,min,max,fact)
         dist_pared, dist_obj_plane, segment=seg.planeSegmentation()
         dist_obj_incline=0
-        if(segment==1):
+        if(segment==1) and column==1 :
             dist_obj_incline= seg.segmentation()
         return dist_pared,dist_obj_plane, dist_obj_incline
     
 
     def dist_teorica(self, mapa, point, angle_degrees, show):
         d = Theoretical_distance()
-        dist = d.theoric_distance(mapa, point, angle_degrees,show)
+        dist,col = d.theoric_distance(mapa, point, angle_degrees,show)
         print("Distància teorica: " + str(dist))
-        return dist
+        return dist,col
```

## Comparing `hpverif-2.6.3.dist-info/RECORD` & `hpverif-2.6.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 hpverif/Calibraton.py,sha256=3_apH-bhEFaYuS4uhOipNU8I4CG_9ubnpSvyJvvmeXA,3046
 hpverif/Driver.py,sha256=Ra-CMqpmRVMUhNoB5H3lYtz7_u5kHI8_umIvbVjOrco,449
 hpverif/FrameCapture.py,sha256=TH7-3ZDrAwIEckOjmM6oeYtGcD0cfx_4GgG78qHeWhk,3961
 hpverif/FrameCapturePLY.py,sha256=PK6Ki_7RZrIizsvZXJL4ixMeVrMG6ESU7vKrMOafbKA,2576
 hpverif/PointCloud.py,sha256=TreRhzS2rbdM2SovJZz-gXDRSpSfxRdqrqNp7fRb04Y,3967
 hpverif/Segmentation.py,sha256=eZFBV1NC5ALDI9fvfiyeRcSWdmDvcBM2KhMIJpXF9Ow,5584
 hpverif/ShowFiles.py,sha256=vofjelAT-1kIfQC6KB6B_Vu-NljtjvZeV-uidOOOslk,2443
-hpverif/Theoretical_distance.py,sha256=3Trsaf8zK-SxfDJYXpV7qUdHWIfDUa72WmesJIugLMc,9966
-hpverif/Verification.py,sha256=H6gtRaBNU239j56JVoWV3GxVjIAO7g3WOqljHnN-Bmk,1876
+hpverif/Theoretical_distance.py,sha256=shDSR6ezTDLddXXdGawYxBtSs0sNPFM5tD7xrzoRMfM,11845
+hpverif/Verification.py,sha256=4ONcnYcshiDQqGT1z9uE9CebuzkJ11KYwoJfyt6yb50,1907
 hpverif/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hpverif/driver.py,sha256=-Y_3y4xh1Gtygx3AruRyzaBszP15mLxSS0toIuZ_qO8,389
-hpverif-2.6.3.dist-info/METADATA,sha256=ywzPw_ucV-1P6evwgKec3OnC09Lr85M_K_DjgBSxRPc,321
-hpverif-2.6.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hpverif-2.6.3.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
-hpverif-2.6.3.dist-info/RECORD,,
+hpverif-2.6.4.dist-info/METADATA,sha256=8iasobf-A50Vtvo2_Jgb9dHnBELAfRuXTinX139ewWE,321
+hpverif-2.6.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hpverif-2.6.4.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
+hpverif-2.6.4.dist-info/RECORD,,
```

