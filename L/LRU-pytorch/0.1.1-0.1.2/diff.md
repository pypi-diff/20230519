# Comparing `tmp/LRU-pytorch-0.1.1.tar.gz` & `tmp/LRU-pytorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LRU-pytorch-0.1.1.tar", last modified: Sat Apr 15 16:42:17 2023, max compression
+gzip compressed data, was "LRU-pytorch-0.1.2.tar", last modified: Fri May 19 17:54:32 2023, max compression
```

## Comparing `LRU-pytorch-0.1.1.tar` & `LRU-pytorch-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 16:42:17.921331 LRU-pytorch-0.1.1/
--rw-rw-rw-   0        0        0     1072 2023-04-15 16:36:46.000000 LRU-pytorch-0.1.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 16:42:17.904331 LRU-pytorch-0.1.1/LRU_pytorch/
--rw-rw-rw-   0        0        0     3002 2023-04-15 16:36:46.000000 LRU-pytorch-0.1.1/LRU_pytorch/LRU.py
--rw-rw-rw-   0        0        0       32 2023-04-15 16:36:46.000000 LRU-pytorch-0.1.1/LRU_pytorch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 16:42:17.919330 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/
--rw-rw-rw-   0        0        0      790 2023-04-15 16:42:17.000000 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-15 16:42:17.000000 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 16:42:17.000000 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 16:42:17.000000 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 16:42:17.000000 LRU-pytorch-0.1.1/LRU_pytorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      790 2023-04-15 16:42:17.921331 LRU-pytorch-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-04-15 16:36:46.000000 LRU-pytorch-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-15 16:42:17.922331 LRU-pytorch-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-04-15 16:42:11.000000 LRU-pytorch-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:54:32.452300 LRU-pytorch-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 05:12:58.000000 LRU-pytorch-0.1.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 17:54:32.426300 LRU-pytorch-0.1.2/LRU_pytorch/
+-rw-rw-rw-   0        0        0     2984 2023-05-19 17:38:10.000000 LRU-pytorch-0.1.2/LRU_pytorch/LRU.py
+-rw-rw-rw-   0        0        0       33 2023-05-19 05:12:58.000000 LRU-pytorch-0.1.2/LRU_pytorch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:54:32.450300 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/
+-rw-rw-rw-   0        0        0      792 2023-05-19 17:54:32.000000 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-19 17:54:32.000000 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:54:32.000000 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 17:54:32.000000 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 17:54:32.000000 LRU-pytorch-0.1.2/LRU_pytorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      792 2023-05-19 17:54:32.452300 LRU-pytorch-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2023-05-19 05:12:58.000000 LRU-pytorch-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-19 17:54:32.453301 LRU-pytorch-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-19 17:53:35.000000 LRU-pytorch-0.1.2/setup.py
```

### Comparing `LRU-pytorch-0.1.1/LRU_pytorch/LRU.py` & `LRU-pytorch-0.1.2/LRU_pytorch/LRU.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,36 +19,35 @@
         B_im=torch.randn([state_features,in_features])/math.sqrt(2*in_features)
         self.B=nn.Parameter(torch.complex(B_re,B_im))
         C_re=torch.randn([out_features,state_features])/math.sqrt(state_features)
         C_im=torch.randn([out_features,state_features])/math.sqrt(state_features)
         self.C=nn.Parameter(torch.complex(C_re,C_im))
         self.state=torch.complex(torch.zeros(state_features),torch.zeros(state_features))
 
-    def forward(self, input):
-        self.state=self.state.to(self.B.device)
+    def forward(self, input,state=None):
+        self.state=self.state.to(self.B.device) if state==None else state
         Lambda_mod=torch.exp(-torch.exp(self.nu_log))
         Lambda_re=Lambda_mod*torch.cos(torch.exp(self.theta_log))
         Lambda_im=Lambda_mod*torch.sin(torch.exp(self.theta_log))
         Lambda=torch.complex(Lambda_re,Lambda_im)
         Lambda=Lambda.to(self.state.device)
         gammas=torch.exp(self.gamma_log).unsqueeze(-1).to(self.B.device)
         gammas=gammas.to(self.state.device)
+        output=torch.empty([i for i in input.shape] +[self.out_features],device=self.B.device)
         #Handle input of (Batches,Seq_length, Input size)
         if input.dim()==3:
-            output=torch.empty([input.shape[0],input.shape[1],self.out_features])
             for i,batch in enumerate(input):
                 out_seq=torch.empty(input.shape[1],self.out_features)
                 for j,step in enumerate(batch):
                     self.state=(Lambda@self.state + gammas* self.B@step.to(dtype= self.B.dtype))
                     out_step= (self.C@self.state).real + self.D@step
                     out_seq[j]=out_step
                 self.state=torch.complex(torch.zeros_like(self.state.real),torch.zeros_like(self.state.real))
                 output[i]=out_seq
         #Handle input of (Seq_length, Input size)
         if input.dim()==2:
-            output=torch.empty([input.shape[0],self.out_features])
             for i,step in enumerate(input):
                 self.state=(Lambda@self.state + gammas* self.B@step.to(dtype= self.B.dtype))
                 out_step= (self.C@self.state).real + self.D@step
                 output[i]=out_step
             self.state=torch.complex(torch.zeros_like(self.state.real),torch.zeros_like(self.state.real))
         return output
```

### Comparing `LRU-pytorch-0.1.1/LRU_pytorch.egg-info/PKG-INFO` & `LRU-pytorch-0.1.2/LRU_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LRU-pytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Linear Recurrent Unit (LRU) - Pytorch
 Home-page: https://github.com/Gothos/LRU-pytorch
-Download-URL: https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1-alpha.tar.gz
+Download-URL: https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1.1-alpha.tar.gz
 Author: Vishnu Jaddipal
 Author-email: zeus.vj2003@gmail.com
 License: MIT
 Keywords: Artificial Intelligence,Deep Learning,Recurrent Neural Networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `LRU-pytorch-0.1.1/PKG-INFO` & `LRU-pytorch-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LRU-pytorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Linear Recurrent Unit (LRU) - Pytorch
 Home-page: https://github.com/Gothos/LRU-pytorch
-Download-URL: https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1-alpha.tar.gz
+Download-URL: https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1.1-alpha.tar.gz
 Author: Vishnu Jaddipal
 Author-email: zeus.vj2003@gmail.com
 License: MIT
 Keywords: Artificial Intelligence,Deep Learning,Recurrent Neural Networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `LRU-pytorch-0.1.1/setup.py` & `LRU-pytorch-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-
-from distutils.core import setup
-setup(
-  name = 'LRU-pytorch',         
-  packages = ['LRU_pytorch'],  
-  version = '0.1.1',     
-  license='MIT',       
-  description = 'Linear Recurrent Unit (LRU) - Pytorch',  
-  author = 'Vishnu Jaddipal',                  
-  author_email = 'zeus.vj2003@gmail.com',     
-  url = 'https://github.com/Gothos/LRU-pytorch',   
-  download_url = 'https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1-alpha.tar.gz',  
-  keywords = ['Artificial Intelligence', 'Deep Learning', 'Recurrent Neural Networks'],   
-  install_requires=[            
-          'torch>=1.13'
-      ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',      
-    'Intended Audience :: Developers',    
-    'Topic :: Scientific/Engineering :: Artificial Intelligence',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    
-  ],
-)
+
+from distutils.core import setup
+setup(
+  name = 'LRU-pytorch',         
+  packages = ['LRU_pytorch'],  
+  version = '0.1.2',     
+  license='MIT',       
+  description = 'Linear Recurrent Unit (LRU) - Pytorch',  
+  author = 'Vishnu Jaddipal',                  
+  author_email = 'zeus.vj2003@gmail.com',     
+  url = 'https://github.com/Gothos/LRU-pytorch',   
+  download_url = 'https://github.com/Gothos/LRU-pytorch/archive/refs/tags/v0.1.1-alpha.tar.gz',  
+  keywords = ['Artificial Intelligence', 'Deep Learning', 'Recurrent Neural Networks'],   
+  install_requires=[            
+          'torch>=1.13'
+      ],
+  classifiers=[
+    'Development Status :: 3 - Alpha',      
+    'Intended Audience :: Developers',    
+    'Topic :: Scientific/Engineering :: Artificial Intelligence',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    
+  ],
+)
```

