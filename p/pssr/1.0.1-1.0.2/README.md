# Comparing `tmp/pssr-1.0.1.tar.gz` & `tmp/pssr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.0.1.tar", max compression
+gzip compressed data, was "pssr-1.0.2.tar", max compression
```

## Comparing `pssr-1.0.1.tar` & `pssr-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.0.1/LICENSE
--rw-r--r--   0        0        0     1129 2024-04-17 01:46:32.503705 pssr-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.0.1/pssr/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/crappifiers.py
--rw-r--r--   0        0        0    23918 2024-04-17 21:06:33.049096 pssr-1.0.1/pssr/data.py
--rw-r--r--   0        0        0     2365 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/loss.py
--rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/__init__.py
--rw-r--r--   0        0        0     1538 2024-03-07 21:39:47.125640 pssr-1.0.1/pssr/models/_blocks.py
--rw-r--r--   0        0        0     3167 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/resunet.py
--rw-r--r--   0        0        0     5394 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/resuneta.py
--rw-r--r--   0        0        0    11190 2024-04-16 23:21:24.751072 pssr-1.0.1/pssr/predict.py
--rw-r--r--   0        0        0    12905 2024-04-16 23:21:24.751072 pssr-1.0.1/pssr/train.py
--rw-r--r--   0        0        0     1046 2024-04-17 21:22:52.443580 pssr-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 pssr-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-18 21:41:53.895012 pssr-1.0.2/README.md
+-rw-r--r--   0        0        0     4098 2024-04-20 03:36:20.880209 pssr-1.0.2/_pssr.py
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.0.2/pssr/__init__.py
+-rw-r--r--   0        0        0     2823 2024-04-19 21:36:59.885172 pssr-1.0.2/pssr/crappifiers.py
+-rw-r--r--   0        0        0    23918 2024-04-17 21:06:33.049096 pssr-1.0.2/pssr/data.py
+-rw-r--r--   0        0        0     2606 2024-04-18 23:21:37.910893 pssr-1.0.2/pssr/loss.py
+-rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/__init__.py
+-rw-r--r--   0        0        0     1538 2024-03-07 21:39:47.125640 pssr-1.0.2/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     3167 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/resunet.py
+-rw-r--r--   0        0        0     5394 2024-04-16 23:21:24.747072 pssr-1.0.2/pssr/models/resuneta.py
+-rw-r--r--   0        0        0    11172 2024-04-20 01:31:13.287411 pssr-1.0.2/pssr/predict.py
+-rw-r--r--   0        0        0    12859 2024-04-19 22:26:27.237887 pssr-1.0.2/pssr/train.py
+-rw-r--r--   0        0        0     1111 2024-04-20 03:02:24.140545 pssr-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 pssr-1.0.2/PKG-INFO
```

### Comparing `pssr-1.0.1/LICENSE` & `pssr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.0.1/README.md` & `pssr-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Point-Scanning Super-Resolution (**PSSR**)
 
-**PSSR** is a standardized [PyTorch](https://pytorch.org) workflow for super-resolution tasks using microscopy images.
+**PSSR** is a standardized [PyTorch](https://pytorch.org)-based workflow for super-resolution tasks using microscopy images.
 This is the official reimplementation of the methods described in the original paper: [Deep learning-based point-scanning super-resolution imaging](https://www.nature.com/articles/s41592-021-01080-z),
 containing various improvements and new features.
 
 The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://haydenstites.github.io/PSSR).
 
 If you have never used **PSSR** before, [Getting Started](https://haydenstites.github.io/PSSR/guide/start.html) outlines installation and basic usage.
 Full reference and explanations of all **PSSR** tools is available in [API Reference](https://haydenstites.github.io/PSSR/reference/api.html).
```

### Comparing `pssr-1.0.1/pssr/crappifiers.py` & `pssr-1.0.2/pssr/crappifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,12 @@
             spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0. 
         """
         self.intensity = intensity
         self.gain = gain
         self.spread = spread
         
     def crappify(self, image : np.ndarray):
-        image_max = max(1, image.max())
-        return self._interpolate(image, np.random.poisson(image/255*image_max)/image_max*255) + self.gain
+        return self._interpolate(image, np.random.poisson(image)) + self.gain
     
     def _interpolate(self, x, y):
         intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
         return x * (1 - intensity) + y * intensity
```

### Comparing `pssr-1.0.1/pssr/data.py` & `pssr-1.0.2/pssr/data.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.1/pssr/loss.py` & `pssr-1.0.2/pssr/loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
             mix (float) : Mix of SSIM loss in loss calculation. 1 is entirely SSIM, 0 is entirely L1 with Gaussian correction. Default is 0.8.
 
             win_size (int) : Size of Gaussian window. Must be odd. Default is 11.
 
             win_sigma (float) : Sigma for distribution of Gaussian window. Default is 1.5.
 
-            ms (bool) : Whether to use MS-SSIM over its SSIM. Default is True.
+            ms (bool) : Whether to use MS-SSIM over basic SSIM. Default is True.
 
             kwargs (dict[str, Any]) : Keyword arguments for pytorch_msssim.
         """
         super().__init__()
 
         kwargs = {} if kwargs is None else kwargs
         self.ssim = MS_SSIM(channel=channels, win_size=win_size, win_sigma=win_sigma, data_range=1, **kwargs) if ms else SSIM(channel=channels, win_size=win_size, win_sigma=win_sigma, data_range=1, **kwargs)
@@ -43,12 +43,19 @@
         x = 1 - self.ssim(input, target)
         if self.mix < 1:
             # Combine SSIM with L1 loss with applied Gaussian window for elementwise multiplication against non-reduced L1 loss
             l1 = F.conv2d(F.l1_loss(input, target, reduction="none"), self.gaussian.to(input.get_device()), groups=self.channels, padding=(self.win_size-1)//2).mean()  # F.conv2d with Gaussian filter
             x = self.mix*x + (1-self.mix)*l1
         return x
 
-def pixel_metric(mse : float, image_range : int):
+def pixel_metric(mse : float, image_range : int = 255):
+    r"""Simple metric for calculating average pixel error.
+    
+    Args:
+        mse (float) : Mean squared error between predicted and ground truth images.
+
+        image_range (int) : Value range of image. Default is 255.
+    """
     return math.sqrt(mse) * image_range
 
 def _psnr_metric(mse : float, max : float):
     return 20 * torch.log10(max / torch.sqrt(mse))
```

### Comparing `pssr-1.0.1/pssr/models/_blocks.py` & `pssr-1.0.2/pssr/models/_blocks.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.1/pssr/models/resunet.py` & `pssr-1.0.2/pssr/models/resunet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.1/pssr/models/resuneta.py` & `pssr-1.0.2/pssr/models/resuneta.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.1/pssr/predict.py` & `pssr-1.0.2/pssr/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             lr = dataset[idx] if dataset.is_lr else dataset[idx][1]
             lr = lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
             hr_hat = _pred_array(hr_hat).squeeze(0)
             
             if norm:
-                _, hr_hat = normalize_pred(np.mean(_pred_array(dataset[idx][0]), axis=0), np.mean(hr_hat, axis=0))
+                _, hr_hat = normalize_preds(np.mean(_pred_array(dataset[idx][0]), axis=0), np.mean(hr_hat, axis=0))
 
             hr_hat = Image.fromarray(hr_hat.astype(np.uint8).squeeze())
             hr_hat = hr_hat.crop([0,0,dataset.crop_res,dataset.crop_res])
 
             outs.append(hr_hat)
 
     if out_dir:
@@ -100,15 +100,14 @@
             remaining -= batch_size
             if remaining <= 0:
                 break
 
     os.makedirs("preds", exist_ok=True)
     collage.save(f"preds/{prefix+'_' if prefix else ''}collage_{n_images}.png")
 
-# TODO: Compute only over dataset.crop_res
 def test_metrics(model : nn.Module, dataset : Dataset, batch_size : int, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True, dataloader_kwargs = None):
     r"""Computes image restoration metrics of predicted vs ground truth images.
 
     Args:
         model (nn.Module) : Model recieve low-resolution images.
 
         dataset (Dataset) : Paired image dataset to load data from.
@@ -142,25 +141,18 @@
     progress = tqdm(val_dataloader)
     with torch.no_grad():
         for hr, lr in progress:
             hr, lr = hr.to(device), lr.to(device)
 
             hr_hat = model(lr)
 
-            hr, hr_hat = _pred_array(hr), _pred_array(hr_hat)
+            hr, hr_hat = _pred_array(hr)[:,:,:dataset.crop_res,:dataset.crop_res], _pred_array(hr_hat)[:,:,:dataset.crop_res,:dataset.crop_res]
 
             if norm:
-                hr_norms, hr_hat_norms = [], []
-                for idx in range(len(hr)):
-                    hr_norm, hr_hat_norm = normalize_pred(np.mean(hr[idx], axis=0), np.mean(hr_hat[idx], axis=0))
-
-                    hr_norms.append(hr_norm)
-                    hr_hat_norms.append(hr_hat_norm)
-                hr = np.asarray(hr_norms)[:, np.newaxis, :, :]
-                hr_hat = np.asarray(hr_hat_norms)[:, np.newaxis, :, :]
+                hr, hr_hat = normalize_preds(hr, hr_hat)
 
             for idx in range(len(hr)):
                 mse = np.mean((hr[idx]/image_range-hr_hat[idx]/image_range)**2) if use_mse else None
 
                 if "mse" in metrics:
                     metrics["mse"].append(mse)
                 if "pixel" in metrics:
@@ -169,69 +161,75 @@
                     metrics["psnr"].append(peak_signal_noise_ratio(hr[idx], hr_hat[idx], data_range=image_range))
                 if "ssim" in metrics:
                     metrics["ssim"].append(structural_similarity(hr[idx].squeeze(), hr_hat[idx].squeeze(), data_range=image_range))
 
     metrics = {metric:(sum(values)/len(values) if avg else values) for metric, values in metrics.items()}
     return metrics
 
-# TODO: Multichannel images
-def normalize_pred(hr : np.ndarray, hr_hat : np.ndarray, pmin : float = 0.1, pmax : float = 99.9):
+def normalize_preds(hr : np.ndarray, hr_hat : np.ndarray, pmin : float = 0.1, pmax : float = 99.9):
     r"""Normalizes prediction image intensities to ground truth for fair benchmarking.
 
     Args:
-        hr (ndarray) : High-resolution ground truth image as array.
+        hr (ndarray) : High-resolution ground truth images as array.
 
-        hr_hat (ndarray) : High-resolution prediction image as array.
+        hr_hat (ndarray) : High-resolution prediction images as array.
 
         pmin (float) : Percentile minimum image intensity. Default is 0.1.
 
         pmax (float) : Percentile maximum image intensity. Default is 99.9.
     
     Returns:
         hr_norm (ndarray) : Normalized high-resolution ground truth image.
 
         hr_hat_norm (ndarray) : Normalized high-resolution prediction image.
     """
-    # Same procedure as in intial PSSR implementation
-    hr = hr.astype(np.float32)
-    hr_hat = hr_hat.astype(np.float32)
+    assert len(hr.shape) == len(hr_hat.shape), "hr and hr_hat must have the same number of dimensions."
+    hr_shape = hr.shape
+    hr_hat_shape = hr_hat.shape
+
+    if len(hr.shape) < 3:
+        hr, hr_hat = hr[np.newaxis, ...], hr_hat[np.newaxis, ...]
+    hr, hr_hat = hr.reshape(-1, *hr.shape[-2:]), hr_hat.reshape(-1, *hr_hat.shape[-2:])
+    assert len(hr) == len(hr_hat), "hr and hr_hat must have the same number of images."
+
+    hr_norms, hr_hat_norms = [], []
+    for idx in range(len(hr)):
+        # Same procedure as in intial PSSR implementation
+        hr_norm = hr[idx].astype(np.float32)
+        hr_hat_norm = hr_hat[idx].astype(np.float32)
+
+        base_max = np.percentile(hr_norm, pmax)
+        base_mean = np.mean(hr_norm)
+
+        hr_norm = _normalize_minmax(hr_norm, pmin, pmax)
+
+        hr_hat_norm = hr_hat_norm - np.mean(hr_hat_norm)
+        hr_norm = hr_norm - np.mean(hr_norm)
+
+        scale = np.cov(cv2.resize(hr_hat_norm, hr_norm.shape).flatten(), hr_norm.flatten())[0, 1] / np.var(hr_hat_norm.flatten())
+        hr_hat_norm = scale * hr_hat_norm
+        
+        # Rescale to initial image intensity
+        hr_norm, hr_hat_norm = (hr_norm-hr_norm.min())*base_max, (hr_hat_norm-hr_norm.min())*base_max
+        hr_norm, hr_hat_norm = hr_norm/(hr_norm.mean()/base_mean), hr_hat_norm/(hr_hat_norm.mean()/base_mean)
 
-    base_max = np.percentile(hr, pmax)
-    base_mean = np.mean(hr)
-
-    hr = _normalize_minmax(hr, pmin, pmax)
-
-    hr_hat = hr_hat - np.mean(hr_hat)
-    hr = hr - np.mean(hr)
-
-    scale = np.cov(cv2.resize(hr_hat, hr.shape).flatten(), hr.flatten())[0, 1] / np.var(hr_hat.flatten())
-    hr_hat = scale * hr_hat
+        hr_norms.append(hr_norm)
+        hr_hat_norms.append(hr_hat_norm)
+    
+    hr, hr_hat = np.asarray(hr_norms).clip(0, 255), np.asarray(hr_hat_norms).clip(0, 255)
+    return hr.reshape(hr_shape), hr_hat.reshape(hr_hat_shape)
     
-    # Rescale to initial image intensity
-    hr, hr_hat = (hr-hr.min())*base_max, (hr_hat-hr.min())*base_max
-    hr, hr_hat = hr/(hr.mean()/base_mean), hr_hat/(hr_hat.mean()/base_mean)
-
-    return np.clip(hr, 0, 255), np.clip(hr_hat, 0, 255)
 
 def _collage_preds(lr, hr_hat, hr, norm : bool = True, max_images : int = 5, crop_res : int = None):
     crop_res = hr.shape[-1] if crop_res is None else crop_res
     lr, hr_hat, hr = _pred_array(lr)[:,:,:crop_res//4,:crop_res//4], _pred_array(hr_hat)[:,:,:crop_res,:crop_res], _pred_array(hr)[:,:,:crop_res,:crop_res]
 
     if norm:
-        lr_norms, hr_norms, hr_hat_norms = [], [], []
-        for idx in range(len(hr)):
-            hr_norm, hr_hat_norm = normalize_pred(np.mean(hr[idx], axis=0), np.mean(hr_hat[idx], axis=0))
-            _, lr_norm = normalize_pred(np.mean(hr[idx], axis=0), np.mean(lr[idx], axis=0))
-
-            lr_norms.append(lr_norm)
-            hr_hat_norms.append(hr_hat_norm)
-            hr_norms.append(hr_norm)
-        lr = np.asarray(lr_norms)[:, np.newaxis, :, :]
-        hr_hat = np.asarray(hr_hat_norms)[:, np.newaxis, :, :]
-        hr = np.asarray(hr_norms)[:, np.newaxis, :, :]
+        hr, hr_hat = normalize_preds(hr, hr_hat)
+        _, lr = normalize_preds(hr, lr)
 
     lr = _image_stack(lr, max_images)
     hr_hat = _image_stack(hr_hat, max_images)
     hr = _image_stack(hr, max_images)
 
     lr = lr.resize((hr.width, hr.height), Image.Resampling.NEAREST)
     if hr_hat.size != hr.size:
@@ -246,25 +244,23 @@
     for idx, image in enumerate(images):
         if raw:
             stack.paste(image, (0, height*idx))
         else:
             stack.paste(image, (width*idx, 0))
     return stack
 
-def _normalize_minmax(x, pmin=0.1, pmax=99.9, clip=False, eps=1e-20, dtype=np.float32):
+def _normalize_minmax(x, pmin=0.1, pmax=99.9, eps=1e-20, dtype=np.float32):
     # From csbdeep
     x_min = np.percentile(x, pmin, keepdims=True)
     x_max = np.percentile(x, pmax, keepdims=True)
 
     x = x.astype(dtype,copy=False)
     x_min = dtype(x_min) if np.isscalar(x_min) else x_min.astype(dtype,copy=False)
     x_max = dtype(x_max) if np.isscalar(x_max) else x_max.astype(dtype,copy=False)
     eps = dtype(eps)
 
     x = (x - x_min) / (x_max - x_min + eps)
-    if clip:
-        x = np.clip(x, 0, 1)
 
     return x
 
 def _pred_array(data):
     return np.clip(data.detach().cpu().numpy(), 0, 255).astype(np.uint8)
```

### Comparing `pssr-1.0.1/pssr/train.py` & `pssr-1.0.2/pssr/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch, os
+import torch, os, random
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
 from torch.utils.data import DataLoader, Dataset
 from pytorch_msssim import ssim
 from skopt import gp_minimize
 from skopt.space import Dimension
@@ -132,15 +132,17 @@
         clip : float = 3, 
         device : str = "cpu", 
         scheduler : torch.optim.lr_scheduler.LRScheduler = None, 
         clamp : bool = False, 
         log_frequency : int = 50, 
         dataloader_kwargs = None
     ):
-    r"""Trains an :class:`nn.Module` model as a crappifier on high-low-resolution paired data.
+    r"""EXPERIMENTAL, NOT CURRENTLY RECOMMENDED FOR MOST WORKFLOWS!
+    
+    Trains an :class:`nn.Module` model as a crappifier on high-low-resolution paired data.
     The model must output an image the same size as the input/have a `scale` value of 1.
     This is not necessary if you are using a :class:`Crappifier` instance as your crappifier.
 
     Args:
         model (nn.Module) : Model to train on paired data.
 
         dataset (Dataset) : Paired image dataset to load data from.
@@ -239,91 +241,86 @@
                 scheduler.step()
 
         collage = _collage_preds(lr, lr_hat, hr)
         os.makedirs("preds", exist_ok=True)
         collage.save(f"preds/pred{epoch}_loss{val_loss:.3f}.png")
     return losses
 
-def approximate_crappifier(crappifier : Crappifier, space : list[Dimension], dataset : Dataset, n_samples : int = 10, opt_kwargs = None):
+def approximate_crappifier(crappifier : Crappifier, space : list[Dimension], dataset : Dataset, max_images = None, opt_kwargs = None):
     r"""Approximates :class:`Crappifier` parameters from ground truth paired images. Uses Bayesian optimization because Crappifier functions are not differentiable.
 
     Args:
         crappifier (Crappifier) : Crappifier whose parameter space will be optimized.
 
         space (list[Dimension]) : List of parameter spaces for each crappifier parameter.
 
         dataset (Dataset) : Paired image dataset to load data from.
 
-        n_samples (int) : Number of image samples to average computations over for each optimization step. Default is 10.
+        max_images (int) : Number of image samples to average computations over for each optimization step. Default is None, using all images in dataset.
 
         opt_kwargs (dict[str, Any]) : Keyword arguments for skopt :meth:`gp_minimize`. Default is None
     """
-    opt_kwargs = {} if opt_kwargs is None else opt_kwargs
     space = [space] if type(space) is not list else space
+    n_samples = len(dataset) if max_images is None else min(max_images, len(dataset))
+    opt_kwargs = {} if opt_kwargs is None else opt_kwargs
 
     objective = _Crappifier_Objective(crappifier, dataset, n_samples).sample
 
     result = gp_minimize(objective, space, **opt_kwargs)
 
     return result
 
 class _Crappifier_Objective():
     def __init__(self, crappifier : Crappifier, dataset : Dataset, n_samples : int):
         self.crappifier = crappifier
         self.dataset = dataset
         self.n_samples = n_samples
 
-        self.idx = 0
-
     def sample(self, params):
+        sample_idx = list(range(len(self.dataset)))
+        random.shuffle(sample_idx)
+
         metrics = []
-        for idx in range(int(self.n_samples)):
+        for idx in sample_idx[:self.n_samples]:
             # Grab gound truth high and low resolution images
-            hr, lr = self.dataset[self.idx]
+            hr, lr = self.dataset[idx]
             hr, lr = np.asarray(hr, dtype=np.uint8), np.asarray(lr, dtype=np.uint8)
-
-            self.idx = self.idx + 1 if self.idx < len(self.dataset) - 1 else 0
             
             # Downsampled high resolution image is the baseline for noise profile comparison
-            ds_hr = np.asarray(Image.fromarray(np.squeeze(np.moveaxis(hr, 0, -1))).resize(lr.shape[-2:], Image.Resampling.BILINEAR))
-            if len(ds_hr.shape) > 2:
-                ds_hr = np.moveaxis(ds_hr, -1, 0)
+            ds_hr = np.stack([np.asarray(Image.fromarray(channel).resize(lr.shape[-2:], Image.Resampling.BILINEAR)) for channel in hr])
 
             # Generate artificial low resolution image using optimized crappifier parameters
             lr_hat = self.crappifier(*params).crappify(ds_hr)
-            if len(lr_hat.shape) < 3:
-                lr_hat = lr_hat[np.newaxis, :, :]
  
             # Generate distribution of noise values for both crappified and ground truth low resolution images
             # NOTE: Cant use SSIM or MSE on images as Crappifier noise levels will converge to zero because a noiseless downscaled image will be closer to ground truth than one with correct amount of noise
             pred_profile = lr_hat.astype(np.float32) - ds_hr.astype(np.float32)
             target_profile = lr.astype(np.float32) - ds_hr.astype(np.float32)
 
             bins = np.arange(-256, 256)
             pred_dist, _ = np.histogram(pred_profile.flatten(), bins)
             target_dist, _ = np.histogram(target_profile.flatten(), bins)
             
             # Aggregate errors of both noise distribution and mean noise profile value
             # We are not generating the noise, so spacial significance is low and mean value is used (spacial loss would underapproximate the correct amount of noise)
-            dist_error = (target_dist - pred_dist)**2
+            dist_error = np.mean((target_dist - pred_dist)**2) / (lr.shape[-1]**2)
             value_error = abs(target_profile.mean() - pred_profile.mean())
-            mse = (target_profile - pred_profile)**2
 
-            loss = (dist_error.mean() * value_error + mse.mean()) / (255**2)
+            loss = dist_error + value_error
             metrics.append(loss)
         return sum(metrics) / len(metrics)
 
 def _crappifier_loss(lr, lr_hat, ds_hr, hist_fn, ssim_loss):
     # Process outlined in approximate_crappifier
     pred_profile = lr_hat - ds_hr
     target_profile = lr - ds_hr
 
     pred_dist = hist_fn(pred_profile)
     target_dist = hist_fn(target_profile)
 
     # We are generating the noise, so a spacial criterion must be present (in a lower order as to optimize purely to the "noiseless" profile)
-    dist_error = F.mse_loss(pred_dist, target_dist)
+    dist_error = F.mse_loss(pred_dist, target_dist) / (lr.shape[-1]**2)
     profile_error = ssim_loss(pred_profile, target_profile)
     # value_error = F.l1_loss(pred_profile.view(pred_profile.shape[0], -1).mean(1), target_profile.view(target_profile.shape[0], -1).mean(1))
 
-    loss = dist_error * profile_error / (255**2)
+    loss = dist_error * profile_error
     return loss
```

### Comparing `pssr-1.0.1/pyproject.toml` & `pssr-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pssr"
-version = "1.0.1"
+version = "1.0.2"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/haydenstites/PSSR"
 documentation = "https://haydenstites.github.io/PSSR/"
 classifiers = [
@@ -14,23 +14,27 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Environment :: GPU :: NVIDIA CUDA",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Documentation :: Sphinx",
 ]
+include = ["_pssr.py"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 torch = "^2.0.0"
 numpy = "^1.26.4"
 pillow = "^10.2.0"
 czifile = "^2019.7.2"
 opencv-python = "^4.9.0.80"
 scikit-image = "^0.23.1"
 scikit-optimize = "^0.9.0"
 tqdm = "^4.66.2"
 pytorch-msssim = "^1.0.0"
 
+[tool.poetry.scripts]
+pssr = "_pssr:run"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.0.1/PKG-INFO` & `pssr-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/haydenstites/PSSR
 License: MIT
 Author: Hayden Stites
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -28,15 +28,15 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Documentation, https://haydenstites.github.io/PSSR/
 Project-URL: Repository, https://github.com/haydenstites/PSSR
 Description-Content-Type: text/markdown
 
 # Point-Scanning Super-Resolution (**PSSR**)
 
-**PSSR** is a standardized [PyTorch](https://pytorch.org) workflow for super-resolution tasks using microscopy images.
+**PSSR** is a standardized [PyTorch](https://pytorch.org)-based workflow for super-resolution tasks using microscopy images.
 This is the official reimplementation of the methods described in the original paper: [Deep learning-based point-scanning super-resolution imaging](https://www.nature.com/articles/s41592-021-01080-z),
 containing various improvements and new features.
 
 The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://haydenstites.github.io/PSSR).
 
 If you have never used **PSSR** before, [Getting Started](https://haydenstites.github.io/PSSR/guide/start.html) outlines installation and basic usage.
 Full reference and explanations of all **PSSR** tools is available in [API Reference](https://haydenstites.github.io/PSSR/reference/api.html).
```

