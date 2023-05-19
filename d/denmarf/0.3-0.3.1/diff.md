# Comparing `tmp/denmarf-0.3.tar.gz` & `tmp/denmarf-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ka-lok.lo/projects/stronglensing/denmarf/dist/.tmp-wef45j9o/denmarf-0.3.tar", last modified: Thu May 18 06:16:56 2023, max compression
+gzip compressed data, was "/home/ka-lok.lo/projects/stronglensing/denmarf/dist/.tmp-lrdsolhn/denmarf-0.3.1.tar", last modified: Fri May 19 06:48:04 2023, max compression
```

## Comparing `denmarf-0.3.tar` & `denmarf-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-18 06:16:56.000000 denmarf-0.3/
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     1071 2022-01-03 22:58:43.000000 denmarf-0.3/LICENSE
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      192 2023-05-18 06:16:56.000000 denmarf-0.3/PKG-INFO
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     3228 2023-02-17 23:28:35.000000 denmarf-0.3/README.md
-drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf/
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       98 2023-04-18 20:46:28.000000 denmarf-0.3/denmarf/__init__.py
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     9077 2023-05-18 06:01:59.000000 denmarf-0.3/denmarf/density.py
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     7676 2023-04-18 18:53:13.000000 denmarf-0.3/denmarf/flows.py
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     1860 2023-04-18 18:53:13.000000 denmarf-0.3/denmarf/transform.py
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      937 2023-04-18 18:53:13.000000 denmarf-0.3/denmarf/utils.py
-drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      192 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/PKG-INFO
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      274 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/SOURCES.txt
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)        1 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/dependency_links.txt
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       14 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/requires.txt
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)        8 2023-05-18 06:16:56.000000 denmarf-0.3/denmarf.egg-info/top_level.txt
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       38 2023-05-18 06:16:56.000000 denmarf-0.3/setup.cfg
--rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      357 2023-02-17 23:29:04.000000 denmarf-0.3/setup.py
+drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-19 06:48:04.000000 denmarf-0.3.1/
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     1071 2022-01-03 22:58:43.000000 denmarf-0.3.1/LICENSE
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      194 2023-05-19 06:48:04.000000 denmarf-0.3.1/PKG-INFO
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     4050 2023-05-19 06:11:24.000000 denmarf-0.3.1/README.md
+drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf/
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       98 2023-04-18 20:46:28.000000 denmarf-0.3.1/denmarf/__init__.py
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)    13010 2023-05-19 05:56:47.000000 denmarf-0.3.1/denmarf/density.py
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     7676 2023-04-18 18:53:13.000000 denmarf-0.3.1/denmarf/flows.py
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     4046 2023-05-19 05:56:47.000000 denmarf-0.3.1/denmarf/transform.py
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)     1791 2023-05-19 05:56:47.000000 denmarf-0.3.1/denmarf/utils.py
+drwxrwxr-x   0 ka-lok.lo (44040) ka-lok.lo (44040)        0 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      194 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/PKG-INFO
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      274 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)        1 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       23 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/requires.txt
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)        8 2023-05-19 06:48:04.000000 denmarf-0.3.1/denmarf.egg-info/top_level.txt
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)       38 2023-05-19 06:48:04.000000 denmarf-0.3.1/setup.cfg
+-rw-rw-r--   0 ka-lok.lo (44040) ka-lok.lo (44040)      398 2023-05-19 06:34:30.000000 denmarf-0.3.1/setup.py
```

### Comparing `denmarf-0.3/LICENSE` & `denmarf-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `denmarf-0.3/denmarf/density.py` & `denmarf-0.3.1/denmarf/density.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,14 +18,29 @@
     def __init__(
         self,
         seed=None,
         device="cpu",
         use_cuda=True,
         bounded=False,
     ):
+        """Initialize the density estimate.
+        
+        Parameters
+        ----------
+        seed : int, optional
+            Random seed.
+        device : str, optional
+            Device to be used. Can be "cpu", "cuda", or "{cpu/cuda}:{device ordinal}".
+        use_cuda : bool, optional
+            Whether to use CUDA if available.
+        bounded : bool, optional
+            Whether the distribution is bounded. If True, the distribution will be transformed to the unbounded space
+            using logistic transformation.
+        
+        """
         self.device = determine_device(device, use_cuda)
 
         if seed is not None:
             # Calling this will take care of everything
             torch.manual_seed(seed)
 
         self.model = None
@@ -33,14 +48,31 @@
 
     @staticmethod
     def construct_model(
         num_features,
         num_blocks,
         num_hidden,
     ):
+        """Construct the pytorch model.
+
+        Parameters
+        ----------
+        num_features : int
+            Number of features.
+        num_blocks : int
+            Number of blocks.
+        num_hidden : int
+            Number of hidden units.
+
+        Returns
+        -------
+        model : torch.nn.Module
+            Pytorch model.
+
+        """
         # Build the pytorch model
         modules = []
         for _ in range(num_blocks):
             modules += [
                 fnn.MADE(num_features, num_hidden, None, act="tanh"),
                 fnn.BatchNormFlow(num_features),
                 fnn.Reverse(num_features)
@@ -67,14 +99,47 @@
         learning_rate=1e-3,
         weight_decay=1e-6,
         batch_size=None,
         p_train=0.5,
         p_test=0.1,
         verbose=True,
     ):
+        """Fit the density estimate to the data.
+        
+        Parameters
+        ----------
+        X : numpy.ndarray
+            Training samples.
+        bounded : bool, optional
+            Whether the distribution is bounded. If True, the distribution will be transformed to the unbounded space
+            using logistic transformation.
+        lower_bounds : numpy.ndarray, optional
+            Lower bounds of the bounded distribution.
+        upper_bounds : numpy.ndarray, optional
+            Upper bounds of the bounded distribution.
+        num_blocks : int, optional
+            Number of blocks.
+        num_hidden : int, optional
+            Number of hidden units.
+        num_epochs : int, optional
+            Number of epochs.
+        learning_rate : float, optional
+            Learning rate.
+        weight_decay : float, optional
+            Weight decay.
+        batch_size : int, optional
+            Batch size.
+        p_train : float, optional
+            Percentage (0 < p_train < 1.0) of training samples.
+        p_test : float, optional
+            Percentage (0 < p_test < 1.0) of test samples. The rest of the samples will be used for validation.
+        verbose : bool, optional
+            Whether to print progress.
+
+        """
         X = np.asarray(X)
         assert len(X.shape) == 2, "X must be of shape (n_samples, n_features)"
 
         # Set batch_size to something reasonable, maybe splitting the training samples into 10 sets?
         if batch_size is None:
             batch_size = int(0.1*X.shape[0])
 
@@ -195,28 +260,67 @@
         if verbose:
             print("best average log likelihood: {:.3f}".format(-best_validation_loss))
         self.model = best_model
 
         return self
 
     def save(self, filename="density_estimate.pickle"):
+        """Save the density estimate to a file.
+        
+        Parameters
+        ----------
+        filename : str
+            Filename to save the density estimate to.
+        
+        """
         torch.save(self, filename)
 
     @staticmethod
     def from_file(
             filename="density_estimate.pickle",
             device="cpu",
             use_cuda=True,
         ):
+        """Load a density estimate from a file.
+
+        Parameters
+        ----------
+        filename : str
+            Filename to load the density estimate from.
+        device : str
+            Device to load the density estimate to. Does not have
+            to be the same architecture as the one used to train the model.
+        use_cuda : bool
+            Whether to use CUDA.
+        
+        Returns
+        -------
+        density_estimate : DensityEstimate
+            The loaded density estimate.
+
+        """
         pytorch_device = determine_device(device, use_cuda)
         de = torch.load(filename, map_location=pytorch_device)
         de.device = pytorch_device
         return de
 
     def score_samples(self, X):
+        """Compute the log likelihood of each sample in X.
+        
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Samples to compute the log likelihood for.
+            
+        Returns
+        -------
+        log_likelihoods : array-like, shape (n_samples,)
+            Log likelihoods of each sample in X.
+            
+        """
         assert len(X.shape) == 2, "X must be of shape (n_samples, n_features)"
         logpdf = np.zeros(X.shape[0])
         X = X.astype(np.float32)
 
         if self.bounded:
             # Check if X is within the bounds
             valid_indices_lower_bounds = np.less_equal(
@@ -235,17 +339,43 @@
         
         X_torch = torch.from_numpy(X).to(self.device)
         logpdf += self.model.log_probs(X_torch).detach().cpu().numpy()
 
         return logpdf
 
     def score(self, X):
+        """Compute the total log likelihood of samples in X.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Samples to compute the log likelihood for.
+
+        Returns
+        -------
+        log_likelihood : float
+            Total log likelihood of samples in X.
+
+        """
         return np.sum(self.score_samples(X))
 
     def sample(self, n_samples=1):
+        """Sample from the density estimate.
+
+        Parameters
+        ----------
+        n_samples : int
+            Number of samples to generate.
+
+        Returns
+        -------
+        samples : array-like, shape (n_samples, n_features)
+            Samples from the density estimate.
+
+        """
         self.model.eval()
 
         # NOTE: always return samples to CPU
         with torch.no_grad():
             generated_samples = self.model.sample(n_samples).detach().cpu().numpy().astype(np.float32)
 
         if self.bounded:
```

### Comparing `denmarf-0.3/denmarf/flows.py` & `denmarf-0.3.1/denmarf/flows.py`

 * *Files identical despite different names*

