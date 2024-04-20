# Comparing `tmp/colabseg-0.0.2.tar.gz` & `tmp/colabseg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabseg-0.0.2.tar", last modified: Mon Jan 22 10:52:33 2024, max compression
+gzip compressed data, was "colabseg-0.0.3.tar", last modified: Sat Apr 20 20:35:17 2024, max compression
```

## Comparing `colabseg-0.0.2.tar` & `colabseg-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-01-22 10:52:33.227758 colabseg-0.0.2/
--rw-r--r--   0 vmaurer    (502) staff       (20)    11357 2023-10-26 08:37:24.000000 colabseg-0.0.2/LICENSE
--rw-r--r--   0 vmaurer    (502) staff       (20)      793 2024-01-22 10:52:33.227507 colabseg-0.0.2/PKG-INFO
--rw-r--r--   0 vmaurer    (502) staff       (20)     1843 2024-01-17 20:17:37.000000 colabseg-0.0.2/README.md
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-01-22 10:52:33.225092 colabseg-0.0.2/colabseg/
--rw-r--r--   0 vmaurer    (502) staff       (20)      267 2024-01-10 09:50:06.000000 colabseg-0.0.2/colabseg/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    59861 2023-11-01 14:00:29.000000 colabseg-0.0.2/colabseg/image_io.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     3736 2023-10-26 09:37:01.000000 colabseg-0.0.2/colabseg/microscope_db.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     7749 2024-01-10 09:50:06.000000 colabseg-0.0.2/colabseg/napari_integration.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    27948 2024-01-08 15:43:47.000000 colabseg-0.0.2/colabseg/new_gui_functions.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    12103 2024-01-09 10:24:35.000000 colabseg-0.0.2/colabseg/parametrization.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    11579 2024-01-08 14:11:53.000000 colabseg-0.0.2/colabseg/py3dmol_controls.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    46957 2024-01-10 09:50:06.000000 colabseg-0.0.2/colabseg/segmentation_gui.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    13009 2023-11-01 14:00:28.000000 colabseg-0.0.2/colabseg/tensorvoting_wrapper.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     6759 2023-11-01 14:00:28.000000 colabseg-0.0.2/colabseg/utilities.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-01-22 10:52:33.227243 colabseg-0.0.2/colabseg.egg-info/
--rw-r--r--   0 vmaurer    (502) staff       (20)      793 2024-01-22 10:52:33.000000 colabseg-0.0.2/colabseg.egg-info/PKG-INFO
--rw-r--r--   0 vmaurer    (502) staff       (20)      532 2024-01-22 10:52:33.000000 colabseg-0.0.2/colabseg.egg-info/SOURCES.txt
--rw-r--r--   0 vmaurer    (502) staff       (20)        1 2024-01-22 10:52:33.000000 colabseg-0.0.2/colabseg.egg-info/dependency_links.txt
--rw-r--r--   0 vmaurer    (502) staff       (20)      105 2024-01-22 10:52:33.000000 colabseg-0.0.2/colabseg.egg-info/requires.txt
--rw-r--r--   0 vmaurer    (502) staff       (20)       15 2024-01-22 10:52:33.000000 colabseg-0.0.2/colabseg.egg-info/top_level.txt
--rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-01-22 10:52:33.227810 colabseg-0.0.2/setup.cfg
--rw-r--r--   0 vmaurer    (502) staff       (20)     1235 2024-01-22 10:51:53.000000 colabseg-0.0.2/setup.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-01-22 10:52:33.226957 colabseg-0.0.2/tests/
--rw-r--r--   0 vmaurer    (502) staff       (20)       15 2023-10-26 08:37:25.000000 colabseg-0.0.2/tests/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     9529 2023-10-26 09:37:01.000000 colabseg-0.0.2/tests/test_segmentation_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     3166 2023-10-26 09:37:01.000000 colabseg-0.0.2/tests/test_utilities.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 20:35:17.461935 colabseg-0.0.3/
+-rw-r--r--   0 vmaurer    (502) staff       (20)    11357 2023-10-26 08:37:24.000000 colabseg-0.0.3/LICENSE
+-rw-r--r--   0 vmaurer    (502) staff       (20)      793 2024-04-20 20:35:17.461746 colabseg-0.0.3/PKG-INFO
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1843 2024-01-17 20:17:37.000000 colabseg-0.0.3/README.md
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 20:35:17.459426 colabseg-0.0.3/colabseg/
+-rw-r--r--   0 vmaurer    (502) staff       (20)      267 2024-01-10 09:50:06.000000 colabseg-0.0.3/colabseg/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    59861 2024-04-01 17:23:41.000000 colabseg-0.0.3/colabseg/image_io.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     3736 2023-10-26 09:37:01.000000 colabseg-0.0.3/colabseg/microscope_db.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    18988 2024-04-20 20:26:11.000000 colabseg-0.0.3/colabseg/napari_integration.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    29928 2024-04-20 20:26:11.000000 colabseg-0.0.3/colabseg/new_gui_functions.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    17700 2024-04-20 20:26:11.000000 colabseg-0.0.3/colabseg/parametrization.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13017 2024-03-30 10:51:57.000000 colabseg-0.0.3/colabseg/py3dmol_controls.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    57328 2024-04-20 20:28:27.000000 colabseg-0.0.3/colabseg/segmentation_gui.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13009 2023-11-01 14:00:28.000000 colabseg-0.0.3/colabseg/tensorvoting_wrapper.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)      940 2024-04-02 07:53:26.000000 colabseg-0.0.3/colabseg/test_surface.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     6759 2023-11-01 14:00:28.000000 colabseg-0.0.3/colabseg/utilities.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 20:35:17.461515 colabseg-0.0.3/colabseg.egg-info/
+-rw-r--r--   0 vmaurer    (502) staff       (20)      793 2024-04-20 20:35:17.000000 colabseg-0.0.3/colabseg.egg-info/PKG-INFO
+-rw-r--r--   0 vmaurer    (502) staff       (20)      557 2024-04-20 20:35:17.000000 colabseg-0.0.3/colabseg.egg-info/SOURCES.txt
+-rw-r--r--   0 vmaurer    (502) staff       (20)        1 2024-04-20 20:35:17.000000 colabseg-0.0.3/colabseg.egg-info/dependency_links.txt
+-rw-r--r--   0 vmaurer    (502) staff       (20)      105 2024-04-20 20:35:17.000000 colabseg-0.0.3/colabseg.egg-info/requires.txt
+-rw-r--r--   0 vmaurer    (502) staff       (20)       15 2024-04-20 20:35:17.000000 colabseg-0.0.3/colabseg.egg-info/top_level.txt
+-rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-04-20 20:35:17.461979 colabseg-0.0.3/setup.cfg
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1235 2024-04-20 20:31:06.000000 colabseg-0.0.3/setup.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 20:35:17.461207 colabseg-0.0.3/tests/
+-rw-r--r--   0 vmaurer    (502) staff       (20)       15 2023-10-26 08:37:25.000000 colabseg-0.0.3/tests/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     9529 2023-10-26 09:37:01.000000 colabseg-0.0.3/tests/test_segmentation_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     3166 2023-10-26 09:37:01.000000 colabseg-0.0.3/tests/test_utilities.py
```

### Comparing `colabseg-0.0.2/LICENSE` & `colabseg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/PKG-INFO` & `colabseg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabseg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Colab Seg 
 Author: Marc Siggel
 Author-email: marc.siggel@embl-hamburg.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `colabseg-0.0.2/README.md` & `colabseg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/colabseg/image_io.py` & `colabseg-0.0.3/colabseg/image_io.py`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/colabseg/microscope_db.py` & `colabseg-0.0.3/colabseg/microscope_db.py`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/colabseg/new_gui_functions.py` & `colabseg-0.0.3/colabseg/new_gui_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # ColabSeg - Interactive segmentation GUI
 #
 # Marc Siggel, December 2021
 
 import os
+import pickle
 import subprocess
 
 import h5py
 import numpy as np
 import open3d as o3d
 import scipy.spatial as spatial
 from scipy import interpolate
 from scipy.spatial.distance import cdist
 from pyntcloud import PyntCloud
 from tqdm.notebook import tqdm
+from sklearn.cluster import KMeans
 
 from .image_io import ImageIO
 from .parametrization import PARAMETRIZATION_TYPE
 from .utilities import (
     plane_fit,
     make_plot_array,
     R_2vect,
@@ -43,20 +45,22 @@
         self.position_list = []
         self.intensity_list = []
 
         # these are the point cloud data original data
         # TODO write reset function for this
         self.cluster_list_tv = []
         self.cluster_list_fits = []
+        self.cluster_list_fits_objects = []
 
         # do not need this rotated list really?
         # self.cluster_rotated_positions = []
         # this list is used for lated stuff
         self.cluster_list_tv_previous = []
         self.cluster_list_fits_previous = []
+        self.cluster_list_fits_objects_previous = []
 
         self.raw_tomogram_slice = []
         self.protein_positions_list = []
         self.analysis_properties = {}
         self.analysis_properties["minimal_distances"] = []
         self.analysis_properties["radii"] = []
         self.analysis_properties["normal_selection"] = []
@@ -87,36 +91,28 @@
         self.pixel_size = list(np.asarray(image.pixel) * 10)
         self.boxlength = image.length
         self.image_array = image.data
         return
 
     def convert_tomo(self, step_size=1):
         """optimized version of conversion code"""
-        unique = np.unique(self.image_array)
-        for u in tqdm(unique[unique != 0]):
-            where = np.where(self.image_array == u)
-            for i in range(0, len(where[0])):
-                self.position_list.append(
-                    np.array(
-                        [
-                            int(where[0][i]) * self.pixel_size[0],
-                            int(where[1][i]) * self.pixel_size[1],
-                            int(where[2][i]) * self.pixel_size[2],
-                        ]
-                    )
-                )
-                self.intensity_list.append(u)
 
-        for index in np.unique(self.intensity_list):
-            subset = np.take(
-                self.position_list, np.where(self.intensity_list == index)[0], axis=0
-            )
-            self.cluster_list_tv.append(subset)
+        non_zero = np.where(self.image_array > 0)
+        values = self.image_array[non_zero]
+        non_zero = np.array(non_zero).T
+        non_zero = np.multiply(non_zero, self.pixel_size)
+        self.position_list.extend([np.array(x) for x in non_zero.tolist()])
+        for u in tqdm(np.unique(values)):
+            indices = np.where(values == u)
+            points = non_zero[indices]
+            self.intensity_list.extend([u] * points.shape[0])
 
-        return
+            self.cluster_list_tv.append(points)
+
+        return None
 
     def load_point_cloud(self, filename):
         """Load a plain point cloud from a txt file.
         In case a user has some preprocessed input on hand
         """
         input_data = np.loadtxt(filename)
         if len(input_data[0]) < 3:
@@ -393,19 +389,44 @@
         if len(cluster_indices) < 2:
             return
         to_merge = []
         for i in cluster_indices:
             to_merge.append(self.cluster_list_tv[i])
         stacked_coordinates = np.vstack(np.asarray(to_merge))
 
-        cluster_indices = np.sort(np.asarray(cluster_indices))[::-1]
-        for i in cluster_indices:
+        new_clusters = np.sort(np.asarray(cluster_indices))[::-1]
+        for i in new_clusters:
             del self.cluster_list_tv[i]
         self.cluster_list_tv.append(stacked_coordinates)
-        return
+        return new_clusters, (len(self.cluster_list_tv) - 1,)
+
+    def split_clusters(self, cluster_indices=[]):
+        """Split one cluster by kmeans"""
+        to_merge = []
+        for i in cluster_indices:
+            to_merge.append(self.cluster_list_tv[i])
+        stacked_coordinates = np.vstack(np.asarray(to_merge))
+
+        for i in cluster_indices:
+            del self.cluster_list_tv[i]
+
+        clustering = KMeans(n_clusters=2).fit(stacked_coordinates)
+
+        new_indices = np.asarray(clustering.labels_)
+
+        for new_clusters in np.unique(new_indices):
+            self.cluster_list_tv.append(
+                stacked_coordinates[np.where(new_indices == new_clusters)]
+            )
+
+        new_clusters = np.unique(new_indices).size
+        total_clusters = len(self.cluster_list_tv)
+        added_clusters = list(range(total_clusters - new_clusters, total_clusters))
+
+        return cluster_indices, added_clusters
 
     def reload_original_values(self):
         """Reload the origial values"""
         self.cluster_list_tv = []
         for index in np.unique(self.intensity_list):
             subset = np.take(
                 self.position_list, np.where(self.intensity_list == index)[0], axis=0
@@ -413,14 +434,23 @@
             self.cluster_list_tv.append(subset)
         self.cluster_list_fits = []
 
     def delete_fit(self, fit_index):
         """delete a fit from data"""
         # self.cluster_list_fits = self.cluster_list_fits.pop(fit_index)
         del self.cluster_list_fits[fit_index]
+        if fit_index < len(self.cluster_list_fits_objects):
+            del self.cluster_list_fits_objects[fit_index]
+
+    def delete_multiple_fits(self, fit_index):
+        """delete a fit from data"""
+        # self.cluster_list_fits = self.cluster_list_fits.pop(fit_index)
+        fit_index = np.sort(np.asarray(fit_index))[::-1]
+        for index in fit_index:
+            self.delete_fit(index)
 
     def delete_multiple_clusters(self, cluster_indices):
         """delete Multiple clusters"""
         cluster_indices = np.sort(np.asarray(cluster_indices))[::-1]
         for index in cluster_indices:
             self.delete_cluster(index)
 
@@ -429,18 +459,20 @@
         # self.cluster_list_fits = self.cluster_list_fits.pop(fit_index)
         del self.cluster_list_tv[cluster_index]
 
     def backup_step_to_previous(self):
         """takes the current value and overwrites the previous step"""
         self.cluster_list_tv_previous = self.cluster_list_tv.copy()
         self.cluster_list_fits_previous = self.cluster_list_fits.copy()
+        self.cluster_list_fits_objects_previous = self.cluster_list_fits_objects.copy()
 
     def reload_previous_step(self):
         self.cluster_list_tv = self.cluster_list_tv_previous.copy()
         self.cluster_list_fits = self.cluster_list_fits_previous.copy()
+        self.cluster_list_fits_objects = self.cluster_list_fits_objects_previous
 
     @staticmethod
     def write_xyz(point_cloud, output_filename):
         """Write an XYZ file for viewing in VMD"""
         xyz_file = "{}\n".format(len(np.asarray(point_cloud)))
         xyz_file += "pointcloud as xyz positions\n"
         for position in np.asarray(point_cloud):
@@ -514,16 +546,19 @@
         """
         self.analysis_properties["normal_selection"] = []
         self.analysis_properties["surface_normals"] = []
         all_positions = []
         for i in cluster_indices:
             all_positions.append(self.cluster_list_tv[i])
         for j in fit_indices:
-            all_positions.append(self.cluster_list_fits[j])
+            converted_index = j - len(self.cluster_list_tv)
+            all_positions.append(self.cluster_list_fits[converted_index])
+
         all_positions = np.vstack(all_positions)
+
         pcd = o3d.geometry.PointCloud()
         pcd.points = o3d.utility.Vector3dVector(all_positions)
         pcd.estimate_normals()
         pcd.normalize_normals()
         pcd.orient_normals_consistent_tangent_plane(k=50)
         self.analysis_properties["normal_selection"] = np.asarray(all_positions)
         self.analysis_properties["surface_normals"] = np.asarray(pcd.normals)
@@ -535,25 +570,34 @@
         return
 
     def flip_normals(self):
         self.analysis_properties["surface_normals"] = self.analysis_properties[
             "surface_normals"
         ] * (-1)
 
-    def interpolate_membrane_closed_surface(self, shape_type, cluster_index=0):
+    def interpolate_membrane_closed_surface(
+        self,
+        shape_type,
+        cluster_index=0,
+        sampling_rate: float = 100,
+        compute_npoints: bool = False,
+    ):
         """Least square fit for a perfect sphere and adding of points.
         For vesicles and spherical viruses.
         """
-        interpxyz = (
-            PARAMETRIZATION_TYPE[shape_type]
-            .fit(np.asarray(self.cluster_list_tv)[cluster_index])
-            .sample(100)
-        )
+        model = PARAMETRIZATION_TYPE[shape_type]
+        model = model.fit(np.asarray(self.cluster_list_tv[cluster_index]))
+
+        if compute_npoints:
+            sampling_rate = model.points_per_sampling(sampling_rate)
+
+        interpxyz = model.sample(sampling_rate)
         self.cluster_list_fits.append(interpxyz)
-        return
+        self.cluster_list_fits_objects.append(model)
+        return None
 
     def save_hdf(self, filename):
         """write all class variables into hdf5 file format"""
         with h5py.File(filename, "w") as hf:
             hf.attrs["mrc_filename"] = self.mrc_filename
             hf.attrs["shape"] = self.shape
             hf.attrs["pixel_size"] = self.pixel_size
@@ -636,14 +680,25 @@
             for i in hf["cluster_list_fits_previous"]:
                 self.cluster_list_fits_previous.append(
                     np.asarray(hf["cluster_list_fits_previous"][i])
                 )
 
         return
 
+    @classmethod
+    def load_pickle(cls, filename: str):
+        with open(filename, "rb") as infile:
+            class_object = pickle.load(infile)
+        return class_object
+
+    def save_pickle(self, filename: str):
+        with open(filename, "wb") as ofile:
+            pickle.dump(self, ofile)
+        return None
+
     def extract_slice(self, filename, slice="center"):
         """Extract a slice from the original tomogram and visualize"""
         # TODO add manual selection of slices; currently disabled
         image = ImageIO()
         image.readMRC(filename, memmap=False)
         center_slice = int(image.shape[2] / 2)
         slice = np.flip(image.data[:, :, center_slice].T)
```

### Comparing `colabseg-0.0.2/colabseg/py3dmol_controls.py` & `colabseg-0.0.3/colabseg/py3dmol_controls.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,57 @@
     """docstring for JupyterFrontend."""
 
     def __init__(self, width=1000, height=500):
         super(seg_visualization, self).__init__()
         # self.view = py3Dmol.view(js="https://3dmol.org/build/3Dmol.js", width=width, height=height)
         self.view = py3Dmol.view(width=width, height=height)
         self.downsample = 1
+        self.total_model = 0
+        self.hidden_models = set()
 
     def view_update(self):
         """Update view of molecules"""
         self.view.update()
         return
 
     def view_zoomto(self):
         """zoomTo shortcut"""
         self.view.zoomTo()
         return
 
+    def delete_model(self, model_index):
+        # Actually using view.removeModel appears to cause issues
+        # Perhaps this is a bug in how py3Dmol internally tracks models
+        self.view.setStyle(
+            {"model": model_index},
+            {"sphere": {"color": "white", "radius": "0", "opacity": "0"}},
+        )
+        self.hidden_models.add(model_index)
+        return None
+
+    def add_model(self, model, model_type="xyz", style=None) -> int:
+        if style is None:
+            style = {"sphere": {"color": "grey", "radius": "20", "opacity": "0.6"}}
+        self.view.addModel(model, model_type)
+        self.view.setStyle({"model": self.total_model}, style)
+        self.total_model += 1
+        return self.total_model - 1
+
+    def add_fit(self, model, model_type="xyz", style=None) -> int:
+        if style is None:
+            style = {"sphere": {"color": "blue", "radius": "20", "opacity": "0.4"}}
+        return self.add_model(model=model, model_type=model_type, style=style)
+
+    def removeAll(self):
+        self.view.removeAllModels()
+        self.view.removeAllShapes()
+        self.total_model = 0
+        self.hidden_models = set()
+        return None
+
     def add_bounding_box(self, boxlength):
         """draws a bounding box according to the tomogram size"""
         # TODO add calculation of box size here
         x, y, z = boxlength
         self.view.addLine(
             {
                 "color": "red",
@@ -166,38 +198,30 @@
     def load_all_models(self, cluster_list, start_index=0):
         """load all models from memory
         Use to initialize gui. Use to reload models after editing point cloud
         """
         for i, cluster_positions in enumerate(cluster_list):
             i = i + start_index
             xyz = self.make_xyz_string(cluster_positions[:: self.downsample])
-            self.view.addModel(xyz, "xyz")
-            self.view.setStyle(
-                {"model": i},
-                {"sphere": {"color": "grey", "radius": "20", "opacity": "0.6"}},
-            )
+            self.add_model(model=xyz, model_type="xyz")
         self.view.zoomTo()
         return
 
     def load_all_models_fit(self, cluster_list, start_index):
         """load all fir models from memory
         Use to initialize gui. Use to reload models after editing point cloud
         """
         for i, cluster_positions in enumerate(cluster_list):
             downsample_fit = int(np.round(len(cluster_positions) / 50000))
             if downsample_fit == 0:
                 downsample_fit = 1
-            print(downsample_fit)
+
             i = i + start_index
             xyz = self.make_xyz_string(cluster_positions[::downsample_fit])
-            self.view.addModel(xyz, "xyz")
-            self.view.setStyle(
-                {"model": i},
-                {"sphere": {"color": "blue", "radius": "20", "opacity": "0.4"}},
-            )
+            self.add_fit(model=xyz, model_type="xyz")
         self.view.zoomTo()
         return
 
     def load_protein_positions(self, protein_positions_list, start_index=0):
         """load all"""
         xyz = self.make_xyz_string_protein(protein_positions_list[0])
         self.view.addModel(xyz, "xyz")
@@ -205,15 +229,21 @@
             {"model": -1},
             {"sphere": {"color": "green", "radius": "40", "opacity": "0.8"}},
         )
         self.view.zoomTo()
         return
 
     def load_normal_positions(self, normal_positions, normal_vectors):
-        for position, normal in zip(normal_positions[::10], normal_vectors[::10] * 150):
+        # for position, normal in zip(normal_positions[::10], normal_vectors[::10] * 150):
+        random_normals = np.random.choice(
+            normal_positions.shape[0], size=100, replace=True
+        )
+        for index in random_normals:
+            position = normal_positions[index]
+            normal = normal_vectors[index] * 150
             self.view.addArrow(
                 {
                     "start": {"x": position[0], "y": position[1], "z": position[2]},
                     "end": {
                         "x": position[0] + normal[0],
                         "y": position[1] + normal[1],
                         "z": position[2] + normal[2],
@@ -262,36 +292,44 @@
         self.view.update()
         return
 
     def highlight_clusters(self, obj):
         """highlight cluster chosen with multi_select"""
         # NOTE old new are assigned by the slider widget
         for i in obj["old"]:
+            if i in self.hidden_models:
+                continue
             self.view.setStyle(
                 {"model": i},
                 {"sphere": {"color": "grey", "radius": "20", "opacity": "0.6"}},
             )
         #    self.view.update()
         for j in obj["new"]:
+            if j in self.hidden_models:
+                continue
             self.view.setStyle(
                 {"model": j}, {"sphere": {"color": "red", "radius": "20"}}
             )
         #    self.view.update()
         self.view.update()
         return
 
     def highlight_fits(self, obj):
         """highlight RBF fit chosen with selector"""
         for i in obj["old"]:
+            if i in self.hidden_models:
+                continue
             self.view.setStyle(
                 {"model": i},
                 {"sphere": {"color": "blue", "radius": "20", "opacity": "0.4"}},
             )
         #    self.view.update()
         for j in obj["new"]:
+            if j in self.hidden_models:
+                continue
             self.view.setStyle(
                 {"model": j}, {"sphere": {"color": "blue", "radius": "20"}}
             )
         self.view.update()
         return
 
     def update_highlight_clusters(self, indices):
```

### Comparing `colabseg-0.0.2/colabseg/segmentation_gui.py` & `colabseg-0.0.3/colabseg/segmentation_gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from .py3dmol_controls import seg_visualization
 from .napari_integration import NapariManager
 
 
 class JupyterFramework(object):
     """Docstring JupyterFramework for GUI"""
 
-    def __init__(self):
+    def __init__(self, width=2000, height=1000):
         self.all_widgets = {}
-        self.seg_visualization = seg_visualization()
+        self.seg_visualization = seg_visualization(width=width, height=height)
         self.data_structure = ColabSegData()
 
     def gui_elements_loading(self):
         """Load Loading interface"""
 
         self.all_widgets["input_mrc"] = widgets.Text(
-            value="test_file.mrc",
+            value="",
             placeholder="mrc or h5 file",
             description="Input Filename:",
             style={"description_width": "initial"},
             disabled=False,
         )
 
         self.all_widgets["load_mrc"] = widgets.Button(
@@ -45,14 +45,22 @@
             description="Load state h5",
             disabled=False,
             style={"description_width": "initial"},
             layout=widgets.Layout(width="200px"),
         )
         self.all_widgets["load_state_hdf"].on_click(self.load_state_hdf)
 
+        self.all_widgets["load_state_pickle"] = widgets.Button(
+            description="Load state pickle",
+            disabled=False,
+            style={"description_width": "initial"},
+            layout=widgets.Layout(width="200px"),
+        )
+        self.all_widgets["load_state_pickle"].on_click(self.load_pickle)
+
         self.all_widgets["load_point_cloud"] = widgets.Button(
             description="Load point cloud txt",
             disabled=False,
             style={"description_width": "initial"},
             layout=widgets.Layout(width="200px"),
         )
         self.all_widgets["load_point_cloud"].on_click(self.load_from_point_cloud)
@@ -68,47 +76,43 @@
         self.hbox_load = widgets.HBox(
             [
                 self.all_widgets["input_mrc"],
                 self.all_widgets["load_mrc"],
                 self.all_widgets["load_point_cloud"],
                 self.all_widgets["load_stl_file"],
                 self.all_widgets["load_state_hdf"],
+                self.all_widgets["load_state_pickle"],
             ]
         )
         display(self.hbox_load)
 
     def gui_elements_cluster_analysis(self):
         """Load Loading interface"""
         self.all_widgets["cluster_sel"] = widgets.SelectMultiple(
             options=[x for x in range(0, len(self.data_structure.cluster_list_tv), 1)],
             rows=10,
             description="Clusters:",
             disabled=False,
         )
-        self.all_widgets["cluster_sel"].observe(
-            self.seg_visualization.highlight_clusters, names="value"
-        )
-
+        self.all_widgets["cluster_sel"].observe(self.highlight_clusters, names="value")
         self.all_widgets["fit_sel"] = widgets.SelectMultiple(
             options=[
                 x
                 for x in range(
                     len(self.data_structure.cluster_list_tv),
                     len(self.data_structure.cluster_list_tv)
                     + len(self.data_structure.cluster_list_fits),
                     1,
                 )
             ],
             rows=10,
             description="Fits:",
             disabled=False,
         )
-        self.all_widgets["fit_sel"].observe(
-            self.seg_visualization.highlight_fits, names="value"
-        )
+        self.all_widgets["fit_sel"].observe(self.highlight_fits, names="value")
 
         self.all_widgets["rotate_flat"] = widgets.Button(description="Rotate Flat")
         self.all_widgets["rotate_flat"].on_click(self.rotate_flat)
 
         self.all_widgets["rotate_back"] = widgets.Button(description="Rotate Original")
         self.all_widgets["rotate_back"].on_click(self.rotate_back)
 
@@ -142,14 +146,19 @@
             description="Save Selected TXT"
         )
         self.all_widgets["save_clusters_txt"].on_click(self.save_clusters_txt)
 
         self.all_widgets["save_hdf"] = widgets.Button(description="Save State hdf5")
         self.all_widgets["save_hdf"].on_click(self.save_state_hdf)
 
+        self.all_widgets["save_pickle"] = widgets.Button(
+            description="Save State pickle"
+        )
+        self.all_widgets["save_pickle"].on_click(self.save_pickle)
+
         self.all_widgets["fit_rbf"] = widgets.Button(description="Fit RBF Fxn")
         self.all_widgets["fit_rbf"].on_click(self.fit_rbf)
 
         self.all_widgets["directionality_rbf"] = widgets.Dropdown(
             options=["xz", "yz", "xy"],
             value="xz",
             description="Membrane Dir.:",
@@ -164,24 +173,55 @@
 
         self.all_widgets["fit_cylinder"] = widgets.Button(description="Fit Cylinder")
         self.all_widgets["fit_cylinder"].on_click(self.fit_cylinder)
 
         self.all_widgets["crop_fit"] = widgets.Button(description="Crop fit around")
         self.all_widgets["crop_fit"].on_click(self.crop_fit)
 
+        self.all_widgets["fit_sampling_method"] = widgets.Dropdown(
+            options=["N points", "Average Distance"],
+            value="Average Distance",
+            description="Fit Sampling:",
+            style={"description_width": "initial"},
+        )
+
+        self.all_widgets["get_fit_normal_sampling"] = widgets.IntText(
+            value=20,
+            min=1,
+            description="Value",
+            disabled=False,
+            style={"description_width": "initial"},
+            layout=widgets.Layout(width="200px"),
+        )
+
+        self.all_widgets["sample_fit"] = widgets.Button(description="Sample Fit")
+        self.all_widgets["sample_fit"].on_click(self.sample_fit)
+
+        self.all_widgets["get_fit_normals"] = widgets.Button(description="Get Normals")
+        self.all_widgets["get_fit_normals"].on_click(self.get_fit_normals)
+
+        self.all_widgets["fit_normals"] = widgets.HBox(
+            [
+                self.all_widgets["sample_fit"],
+                self.all_widgets["get_fit_normals"],
+                self.all_widgets["fit_sampling_method"],
+                self.all_widgets["get_fit_normal_sampling"],
+            ]
+        )
+
         self.all_widgets["distance_tolerance"] = widgets.IntText(
             value=50,
             min=1,
-            description="Dist Toleracne:",
+            description="Dist Tolerance:",
             disabled=False,
             style={"description_width": "initial"},
             layout=widgets.Layout(width="150px"),
         )
 
-        self.all_widgets["delete_fit"] = widgets.Button(description="Delete fit")
+        self.all_widgets["delete_fit"] = widgets.Button(description="Delete fits")
         self.all_widgets["delete_fit"].on_click(self.delete_fit)
 
         self.all_widgets["trim_min"] = widgets.IntText(
             value=100, min=0, description="Trim Min:", disabled=False
         )
         self.all_widgets["trim_max"] = widgets.IntText(
             value=100, min=0, description="Trim Max:", disabled=False
@@ -200,14 +240,31 @@
             description="Delete Clusters"
         )
         self.all_widgets["delete_cluster"].on_click(self.delete_cluster)
 
         self.all_widgets["undo_step"] = widgets.Button(description="Undo last step")
         self.all_widgets["undo_step"].on_click(self.undo_step)
 
+        self.all_widgets["min_cluster_size"] = widgets.IntText(
+            value=100,
+            min=0,
+            description="Minimum Cluster Size",
+            style={"description_width": "initial"},
+            disabled=False,
+        )
+        self.all_widgets["highlight_clusters"] = widgets.Button(
+            description="Highlight Clusters"
+        )
+        self.all_widgets["highlight_clusters"].on_click(self.highlight_clusters_size)
+
+        self.all_widgets["plot_cluster_size"] = widgets.Button(
+            description="Plot Cluster Size"
+        )
+        self.all_widgets["plot_cluster_size"].on_click(self.plot_cluster_size)
+
         self.all_widgets["reset_input"] = widgets.Button(description="Rest to initial")
         self.all_widgets["reset_input"].on_click(self.reset_input)
 
         self.all_widgets["dbscan_eps"] = widgets.IntText(
             value=40,
             min=0,
             description="Neighbor Dist:",
@@ -260,50 +317,64 @@
         # # TODO: add hyperparameters for outlier removal
 
         self.all_widgets["merge_clusters"] = widgets.Button(
             description="Merge Clusters", style={"description_width": "initial"}
         )
         self.all_widgets["merge_clusters"].on_click(self.merge_clusters)
 
+        self.all_widgets["split_clusters"] = widgets.Button(
+            description="Split Cluster", style={"description_width": "initial"}
+        )
+        self.all_widgets["split_clusters"].on_click(self.split_clusters)
+
         self.all_widgets["load_raw_image_text"] = widgets.Text(
-            value="raw_image.mrc",
+            value="",
             placeholder="Type something",
             description="Raw mrc file:",
             disabled=False,
         )
 
         self.napari_manager = None
         self.all_widgets["load_raw_image_button"] = widgets.Button(
-            description="Open Napari", style={"description_width": "initial"}
+            description="Open Napari",
+            style={"description_width": "initial"},
         )
 
         def open_napari_wrapper(change):
-            open_tomo = self.data_structure.read_mrc(
-                self.all_widgets["load_raw_image_text"].value
-            ).data
+            open_tomo = None
+            if self.all_widgets["load_raw_image_text"].value != "":
+                open_tomo = self.data_structure.read_mrc(
+                    self.all_widgets["load_raw_image_text"].value
+                )
+
             self.napari_manager = NapariManager(
-                colabsegdata_instance=self.data_structure, display_data=open_tomo
+                colabsegdata_instance=self.data_structure,
+                display_data=open_tomo.data,
+                display_pixel_size=np.asarray(open_tomo.pixel) * 10,
             )
-            self.napari_manager.run()
+            # Not required since run from jupyter notebook
+            # self.napari_manager.run()
 
         self.all_widgets["load_raw_image_button"].on_click(open_napari_wrapper)
 
         def sync_napari_wrapper(change):
             if self.napari_manager is None:
                 return None
 
             data = self.napari_manager.export_data()
 
             mapping = {
                 "cluster_list_tv": "Cluster",
                 "cluster_list_fits": "Fit",
                 "protein_positions_list": "Protein",
+                "cluster_list_fits_objects": "Fits",
             }
             for key, value in mapping.items():
-                setattr(self.data_structure, key, [x for x in data.get(value, [[]])])
+                # setattr(self.data_structure, key, [x for x in data.get(value, [[]])])
+                setattr(self.data_structure, key, [x for x in data.get(value, [])])
 
             if self.napari_manager is not None:
                 self.napari_manager.close()
                 self.napari_manager = None
             self.reload_gui()
 
         self.all_widgets["save_raw_image_button"] = widgets.Button(
@@ -466,14 +537,15 @@
             [
                 self.all_widgets["select_all_clusters"],
                 self.all_widgets["save_as_integers"],
                 self.all_widgets["output_filename"],
                 self.all_widgets["save_clusters_mrc"],
                 self.all_widgets["save_clusters_txt"],
                 self.all_widgets["save_hdf"],
+                self.all_widgets["save_pickle"],
             ]
         )
 
         if self.data_structure.raw_tomogram_slice == []:
             plot_output = widgets.Output()
             plot_output.clear_output()
             with plot_output:
@@ -541,20 +613,22 @@
         self.all_widgets["fit_closed_surface"] = widgets.HBox(
             [
                 self.all_widgets["fit_sphere"],
                 self.all_widgets["fit_ellipsoid"],
                 self.all_widgets["fit_cylinder"],
             ]
         )
+
         self.all_widgets["fitting"] = widgets.VBox(
             [
                 self.all_widgets["fitting_rbf"],
                 self.all_widgets["fit_closed_surface"],
                 self.all_widgets["cropping"],
                 self.all_widgets["delete_fit"],
+                self.all_widgets["fit_normals"],
             ]
         )
         self.all_widgets["trimming"] = widgets.HBox(
             [
                 self.all_widgets["trim_max"],
                 self.all_widgets["trim_min"],
                 self.all_widgets["trim_top_bottom"],
@@ -567,14 +641,23 @@
             [
                 self.all_widgets["undo_step"],
                 self.all_widgets["reset_input"],
                 self.all_widgets["delete_cluster"],
                 self.all_widgets["merge_clusters"],
             ]
         )
+        self.all_widgets["cluster_highlight"] = widgets.VBox(
+            [
+                self.all_widgets["min_cluster_size"],
+                self.all_widgets["highlight_clusters"],
+                self.all_widgets["plot_cluster_size"],
+                self.all_widgets["split_clusters"],
+            ]
+        )
+
         self.all_widgets["outliers"] = widgets.VBox(
             [
                 self.all_widgets["edge_outlier_removal"],
                 self.all_widgets["control_stat_outlier_removal"],
                 self.all_widgets["control_dbscan_clustering"],
             ]
         )
@@ -595,15 +678,19 @@
                 self.all_widgets["analyze_sphere_radius_button"],
                 self.all_widgets["analysis_plot_figure"],
             ]
         )
 
         self.all_widgets["tab_nest"] = widgets.Tab()
         cluster_tab = widgets.HBox(
-            [self.all_widgets["cluster_sel"], self.all_widgets["undoing"]]
+            [
+                self.all_widgets["cluster_sel"],
+                self.all_widgets["undoing"],
+                self.all_widgets["cluster_highlight"],
+            ]
         )
         edit_tab = widgets.VBox(
             [self.all_widgets["trimming"], self.all_widgets["rotating"]]
         )
         point_edit_tab = widgets.HBox([self.all_widgets["outliers"]])
         fit_tab = widgets.HBox(
             [self.all_widgets["fit_sel"], self.all_widgets["fitting"]]
@@ -636,19 +723,30 @@
         display(self.all_widgets["tab_nest"])
 
         # organize into tabs
         # 3D visualizatiton GUI here
         self.seg_visualization.load_all_models(
             self.data_structure.cluster_list_tv, start_index=0
         )
+
+        total_options = [
+            *self.all_widgets["cluster_sel"].options,
+            *self.all_widgets["fit_sel"].options,
+        ]
+        self.model_mapping_table = dict(zip(total_options, total_options))
+        self.model_mapping_table_previous = self.model_mapping_table.copy()
         if len(self.data_structure.cluster_list_fits) > 0:
             self.seg_visualization.load_all_models_fit(
                 self.data_structure.cluster_list_fits,
                 start_index=len(self.data_structure.cluster_list_tv),
             )
+            self.cluster_fit_mapping_table = {
+                i: i for i in self.all_widgets["fit_sel"].options
+            }
+
         self.seg_visualization.add_bounding_box(self.data_structure.boxlength)
         if len(self.data_structure.protein_positions_list) > 0:
             self.seg_visualization.load_protein_positions(
                 self.data_structure.protein_positions_list, start_index=0
             )
         if len(self.data_structure.analysis_properties["normal_selection"]) > 0:
             self.seg_visualization.load_normal_positions(
@@ -657,27 +755,25 @@
             )
 
     def boot_gui(self):
         """Initial booting of the gui"""
         clear_output()
         # sets the downsampling value for the py3dmol module for large point clouds.
         self.update_downsampling()
-        self.seg_visualization.view.removeAllModels()
-        self.seg_visualization.view.removeAllShapes()
+        self.seg_visualization.removeAll()
         self.gui_elements_cluster_analysis()
         self.seg_visualization.view.update()
         return
 
     def reload_gui(self):
         """Reloads the entire gui after applying changes"""
         clear_output()
         # sets the downsampling value for the py3dmol module for large point clouds.
         self.update_downsampling()
-        self.seg_visualization.view.removeAllModels()
-        self.seg_visualization.view.removeAllShapes()
+        self.seg_visualization.removeAll()
         self.gui_elements_cluster_analysis()
         self.seg_visualization.view.update()
         self.seg_visualization.view.show()
         return
 
     def load_mrc_file(self, obj):
         """Load MRC file and populate backend"""
@@ -706,40 +802,40 @@
     def load_viz(self, obj):
         """Load Visualizations"""
         self.seg_visualization.load_model_from_file(self.all_widgets["input_mrc"].value)
         return
 
     def rotate_flat(self, obj):
         """Rotate Lamina Flat onto xy plane"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         self.data_structure.plain_fit_and_rotate_lamina(backward=False)
         self.reload_gui()
         # self.seg_visualization.load_all_models(self.data_structure.cluster_list_tv)
         # self.seg_visualization.add_bounding_box(self.data_structure.boxlength)
         # self.seg_visualization.highlight_clusters
         return
 
     def rotate_back(self, obj):
         """rotate Lamina back to original position"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         self.data_structure.plain_fit_and_rotate_lamina(backward=True)
         # self.seg_visualization.load_all_models(self.data_structure.cluster_list_tv)
         # self.seg_visualization.add_bounding_box(self.data_structure.boxlength)
         # self.seg_visualization.highlight_clusters
         self.reload_gui()
         return
 
     def trim_top_bottom(self, obj):
         """Above and below a certain value"""
         if (
             len(self.all_widgets["cluster_sel"].value) == 0
             and len(self.all_widgets["fit_sel"].value) == 0
         ):
             return
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         trim_min = self.all_widgets["trim_min"].value
         trim_max = self.all_widgets["trim_max"].value
 
         if len(self.all_widgets["cluster_sel"].value) != 0:
             self.data_structure.trim_cluster_egdes_cluster(
                 self.all_widgets["cluster_sel"].value, trim_min, trim_max
             )
@@ -760,14 +856,26 @@
         return
 
     def save_state_hdf(self, obj):
         """save state as hdf5 file"""
         self.data_structure.save_hdf(self.all_widgets["output_filename"].value)
         return
 
+    def load_pickle(self, obj):
+        """load state as hdf5"""
+        self.data_structure = ColabSegData.load_pickle(
+            self.all_widgets["input_mrc"].value
+        )
+        return None
+
+    def save_pickle(self, obj):
+        """save state as hdf5 file"""
+        self.data_structure.save_pickle(self.all_widgets["output_filename"].value)
+        return None
+
     def save_clusters_mrc(self, obj):
         """Saves an MRC file with the selected clusters and fits"""
         positions = []
 
         if self.all_widgets["select_all_clusters"].value == True:
             for cluster_tv in self.data_structure.cluster_list_tv:
                 positions.append(cluster_tv)
@@ -812,104 +920,257 @@
             positions = np.vstack(np.asarray(positions))
 
         self.data_structure.write_txt(
             positions, self.all_widgets["output_filename"].value
         )
         return
 
+    def highlight_clusters(self, obj):
+        new_obj = {}
+
+        new_obj["old"] = [self.model_mapping_table[i] for i in obj["old"]]
+        new_obj["new"] = [self.model_mapping_table[i] for i in obj["new"]]
+        self.seg_visualization.highlight_clusters(new_obj)
+        return None
+
+    def highlight_fits(self, obj):
+        new_obj = {}
+
+        new_obj["old"] = [self.model_mapping_table[i] for i in obj["old"]]
+        new_obj["new"] = [self.model_mapping_table[i] for i in obj["new"]]
+        self.seg_visualization.highlight_fits(new_obj)
+        return None
+
     def merge_clusters(self, obj):
         """Merge selected clusters"""
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) < 2:
             print("Not enough selected!")
             print("Please select at least 2 cluster for merging")
-        self.data_structure.merge_clusters(self.all_widgets["cluster_sel"].value)
-        self.reload_gui()
+            return None
+        removed, added = self.data_structure.merge_clusters(
+            self.all_widgets["cluster_sel"].value
+        )
+        self._delete_model(removed)
+        self._add_model(added)
+
+        self.seg_visualization.view_update()
         return
 
+    def split_clusters(self, obj):
+        """Split selected clusters"""
+        self.backup_step_to_previous()
+        if len(self.all_widgets["cluster_sel"].value) != 1:
+            print("Please only select a single cluster for splitting")
+            return None
+
+        removed, added = self.data_structure.split_clusters(
+            self.all_widgets["cluster_sel"].value
+        )
+        self._delete_model(removed)
+        self._add_model(added)
+
+        self.seg_visualization.view_update()
+        return None
+
+    def delete_cluster(self, obj):
+        self.backup_step_to_previous()
+        if len(self.all_widgets["cluster_sel"].value) == 0:
+            print("Nothing selected!")
+            print("Please select at least one cluster for deleting")
+            return None
+
+        self.data_structure.delete_multiple_clusters(
+            self.all_widgets["cluster_sel"].value
+        )
+        self._delete_model(self.all_widgets["cluster_sel"].value)
+        self.seg_visualization.view_update()
+        return None
+
+    def backup_step_to_previous(self):
+        self.model_mapping_table_previous = self.model_mapping_table.copy()
+        self.data_structure.backup_step_to_previous()
+        return None
+
+    def _delete_model(self, cluster_indices):
+        available_models = list(self.model_mapping_table.values())
+        for value in cluster_indices:
+            model_value = self.model_mapping_table[value]
+            available_models.remove(model_value)
+            self.seg_visualization.delete_model(model_value)
+
+        n_clusters = len(self.data_structure.cluster_list_tv)
+        clusters = [x for x in range(0, n_clusters)]
+        self.all_widgets["cluster_sel"].options = clusters
+
+        fits = [
+            n_clusters + x for x in range(0, len(self.data_structure.cluster_list_fits))
+        ]
+        self.all_widgets["fit_sel"].options = fits
+
+        models = [x for x in range(0, len(self.model_mapping_table), 1)]
+        self.model_mapping_table = dict(zip(models, available_models))
+        return None
+
+    def _add_model(self, cluster_indices):
+        downsample = self.seg_visualization.downsample
+        for value in cluster_indices:
+            xyz = self.seg_visualization.make_xyz_string(
+                self.data_structure.cluster_list_tv[value][::downsample]
+            )
+            model_index = self.seg_visualization.add_model(xyz)
+            self.model_mapping_table[value] = model_index
+        clusters = [x for x in range(0, len(self.data_structure.cluster_list_tv), 1)]
+        self.all_widgets["cluster_sel"].options = clusters
+        return None
+
     def reset_input(self, obj):
         """Reset input"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         self.data_structure.reload_original_values()
         self.reload_gui()
         return
 
     def undo_step(self, obj):
         """undo last step"""
+        self.model_mapping_table = self.model_mapping_table_previous
         self.data_structure.reload_previous_step()
         self.reload_gui()
         return
 
     def fit_rbf(self, obj):
         """fit RBF to selected clusters"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the fitting procedure!")
             return
         self.data_structure.interpolate_membrane_rbf(
             self.all_widgets["cluster_sel"].value,
             skip_to_downsample="auto",
             directionality=self.all_widgets["directionality_rbf"].value,
         )
         self.reload_gui()
         return
 
     def fit_sphere(self, obj):
         """Fit lstsq sphere to selected cluster"""
-        self.data_structure.backup_step_to_previous()
-        if len(self.all_widgets["cluster_sel"].value) != 1:
-            print("Nothing or too many clusters selected!")
-            print("Please select a single cluster for the fitting procedure!")
-            return
-        self.data_structure.interpolate_membrane_closed_surface(
-            "sphere", self.all_widgets["cluster_sel"].value
-        )
-        self.reload_gui()
-        return
+        return self.fit_parametrization(parametrization_type="sphere", obj=obj)
 
     def fit_ellipsoid(self, obj):
         """Fit lstsq ellipsoid to selected cluster"""
-        self.data_structure.backup_step_to_previous()
-        if len(self.all_widgets["cluster_sel"].value) != 1:
-            print("Nothing or too many clusters selected!")
-            print("Please select a single cluster for the fitting procedure!")
-            return
-        self.data_structure.interpolate_membrane_closed_surface(
-            "ellipsoid", self.all_widgets["cluster_sel"].value
-        )
-        self.reload_gui()
-        return
+        return self.fit_parametrization(parametrization_type="ellipsoid", obj=obj)
 
     def fit_cylinder(self, obj):
         """Fit lstsq ellipsoid to selected cluster"""
-        self.data_structure.backup_step_to_previous()
-        if len(self.all_widgets["cluster_sel"].value) != 1:
+        return self.fit_parametrization(parametrization_type="cylinder", obj=obj)
+
+    def fit_parametrization(self, parametrization_type, obj):
+        self.backup_step_to_previous()
+
+        if len(self.all_widgets["cluster_sel"].value) == 0:
             print("Nothing or too many clusters selected!")
-            print("Please select a single cluster for the fitting procedure!")
-            return
-        self.data_structure.interpolate_membrane_closed_surface(
-            "cylinder", self.all_widgets["cluster_sel"].value
-        )
-        self.reload_gui()
-        return
+            return None
 
-    def delete_fit(self, obj):
-        """deletes a selected fit"""
-        self.data_structure.backup_step_to_previous()
+        for cluster in self.all_widgets["cluster_sel"].value:
+            self.data_structure.interpolate_membrane_closed_surface(
+                parametrization_type,
+                cluster,
+                sampling_rate=self.all_widgets["get_fit_normal_sampling"].value,
+                compute_npoints=self.all_widgets["fit_sampling_method"].value
+                == "Average Distance",
+            )
+            added_data = self.data_structure.cluster_list_fits[-1]
+
+            xyz = self.seg_visualization.make_xyz_string(added_data)
+            model_index = self.seg_visualization.add_fit(xyz)
+
+            value = len(self.model_mapping_table)
+            self.model_mapping_table[value] = model_index
+
+        options = [
+            x
+            for x in range(
+                len(self.data_structure.cluster_list_tv),
+                len(self.data_structure.cluster_list_tv)
+                + len(self.data_structure.cluster_list_fits),
+                1,
+            )
+        ]
+        self.all_widgets["fit_sel"].options = options
+        self.seg_visualization.view_update()
+        return None
+
+    def sample_fit(self, obj):
         if len(self.all_widgets["fit_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the deleting procedure!")
-            return
-        self.data_structure.delete_fit(self.fit_idx_conv()[0])
+            return None
+
+        fit_index = self.all_widgets["fit_sel"].value[0]
+        fit_index = fit_index - len(self.data_structure.cluster_list_tv)
+        model = self.data_structure.cluster_list_fits_objects[fit_index]
+
+        n_points = self.all_widgets["get_fit_normal_sampling"].value
+        if self.all_widgets["fit_sampling_method"].value == "Average Distance":
+            n_points = model.points_per_sampling(n_points)
+
+        points = model.sample(n_points)
+        self.data_structure.cluster_list_fits[fit_index] = points
+
+        # downsample = self.seg_visualization.downsample
+        for value in self.all_widgets["fit_sel"].value:
+            model_value = self.model_mapping_table[value]
+            self.seg_visualization.delete_model(model_value)
+
+            xyz = self.seg_visualization.make_xyz_string(points)
+            model_index = self.seg_visualization.add_fit(xyz)
+            self.model_mapping_table[value] = model_index
+
+        self.seg_visualization.view_update()
+
+        return None
+
+    def get_fit_normals(self, obj):
+        if len(self.all_widgets["fit_sel"].value) != 1:
+            print("Nothing or too many clusters selected!")
+            print("Please select a single cluster for the deleting procedure!")
+            return None
+        self.backup_step_to_previous()
+        fit_index = self.all_widgets["fit_sel"].value[0]
+        fit_index = fit_index - len(self.data_structure.cluster_list_tv)
+        model = self.data_structure.cluster_list_fits_objects[fit_index]
+
+        n_points = self.all_widgets["get_fit_normal_sampling"].value
+        if self.all_widgets["fit_sampling_method"].value == "Average Distance":
+            n_points = model.points_per_sampling(n_points)
+
+        base_vectors = model.sample(n_points)
+        normal_vectors = model.compute_normal(base_vectors)
+        self.data_structure.analysis_properties["normal_selection"] = base_vectors
+        self.data_structure.analysis_properties["surface_normals"] = normal_vectors
         self.reload_gui()
-        return
+        return None
+
+    def delete_fit(self, obj):
+        """deletes a selected fit"""
+        self.backup_step_to_previous()
+        if len(self.all_widgets["fit_sel"].value) == 0:
+            print("Nothing selected!")
+            print("Please select at least one fit for deleting")
+            return None
+
+        self.data_structure.delete_multiple_fits(self.fit_idx_conv())
+        self._delete_model(self.all_widgets["fit_sel"].value)
+        self.seg_visualization.view_update()
+        return None
 
     def dbscan_recluster(self, obj):
         """run DBSCAN clustering and re-assign clusters"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the DBSCAN clustering!")
             return
         self.data_structure.dbscan_clustering(
             self.all_widgets["cluster_sel"].value[0],
             eps=self.all_widgets["dbscan_eps"].value,
@@ -917,15 +1178,15 @@
         )
         self.reload_gui()
         return
 
     def outlier_removal(self, obj):
         """remove statistical outliers"""
         # TODO: add selection parameters to interface
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the outlier removal!")
             return
         self.data_structure.statistical_outlier_removal(
             self.all_widgets["cluster_sel"].value[0],
             nb_neighbors=self.all_widgets["outlier_nb_neighbors"].value,
@@ -933,28 +1194,28 @@
         )
         self.reload_gui()
         return
 
     def remove_eigenvalue_outliers(self, obj):
         """remove edge outliers"""
         # TODO: add lambda variable to the selection
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the eigenvalue removal!")
             return
         self.data_structure.eigenvalue_outlier_removal(
             self.all_widgets["cluster_sel"].value[0]
         )
         self.reload_gui()
         return
 
     def crop_fit(self, obj):
         """Crop fit around fit"""
-        self.data_structure.backup_step_to_previous()
+        self.backup_step_to_previous()
         if len(self.all_widgets["cluster_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single cluster for the cropping!")
             return
         if len(self.all_widgets["fit_sel"].value) != 1:
             print("Nothing or too many clusters selected!")
             print("Please select a single fit for the cropping!")
@@ -963,26 +1224,14 @@
             cluster_index_tv=self.all_widgets["cluster_sel"].value[0],
             cluster_index_fit=self.fit_idx_conv()[0],
             distance_tolerance=self.all_widgets["distance_tolerance"].value,
         )
         self.reload_gui()
         return
 
-    def delete_cluster(self, obj):
-        self.data_structure.backup_step_to_previous()
-        if len(self.all_widgets["cluster_sel"].value) == 0:
-            print("Nothing selected!")
-            print("Please select at least one cluster for deleting")
-            return
-        self.data_structure.delete_multiple_clusters(
-            self.all_widgets["cluster_sel"].value
-        )
-        self.reload_gui()
-        return
-
     def fit_idx_conv(self):
         """Helper function to convert the index of a fit"""
         fit_indices = np.asarray(self.all_widgets["fit_sel"].value) - len(
             self.data_structure.cluster_list_tv
         )
         return fit_indices
 
@@ -1187,7 +1436,33 @@
 
     def flip_normals(self, obj):
         if len(self.data_structure.analysis_properties["surface_normals"]) == 0:
             print("no normals calculated. Use get normals first")
             return
         self.data_structure.flip_normals()
         self.reload_gui()
+
+    def highlight_clusters_size(self, obj):
+        cutoff = self.all_widgets["min_cluster_size"].value
+
+        indices = [
+            i
+            for i in range(len(self.data_structure.cluster_list_tv))
+            if self.data_structure.cluster_list_tv[i].shape[0] < cutoff
+        ]
+
+        self.all_widgets["cluster_sel"].value = indices
+        return None
+
+    def plot_cluster_size(self, obj):
+        sizes = [x.shape[0] for x in self.data_structure.cluster_list_tv]
+        plt.figure(dpi=100)
+        plt.hist(
+            sizes,
+            bins=20,
+            density=False,
+        )
+        plt.ylabel("Count")
+        plt.xlabel("Size")
+        plt.title("Distribution of cluster sizes")
+        plt.show()
+        return
```

### Comparing `colabseg-0.0.2/colabseg/tensorvoting_wrapper.py` & `colabseg-0.0.3/colabseg/tensorvoting_wrapper.py`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/colabseg/utilities.py` & `colabseg-0.0.3/colabseg/utilities.py`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/colabseg.egg-info/PKG-INFO` & `colabseg-0.0.3/colabseg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabseg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Colab Seg 
 Author: Marc Siggel
 Author-email: marc.siggel@embl-hamburg.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `colabseg-0.0.2/colabseg.egg-info/SOURCES.txt` & `colabseg-0.0.3/colabseg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 colabseg/microscope_db.py
 colabseg/napari_integration.py
 colabseg/new_gui_functions.py
 colabseg/parametrization.py
 colabseg/py3dmol_controls.py
 colabseg/segmentation_gui.py
 colabseg/tensorvoting_wrapper.py
+colabseg/test_surface.py
 colabseg/utilities.py
 colabseg.egg-info/PKG-INFO
 colabseg.egg-info/SOURCES.txt
 colabseg.egg-info/dependency_links.txt
 colabseg.egg-info/requires.txt
 colabseg.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `colabseg-0.0.2/setup.py` & `colabseg-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except:
     raise ImportError("setuptools is required. Install it with: pip install setuptools")
 
 
 # if sys.version_info < (3.9, 0):
 #    sys.exit('Python 3.9 is required! please install in your environment.')
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Colab Seg "
 LONG_DESCRIPTION = (
     "Segmentation toolbox GUI for membranes from cryo-electron tomography images"
 )
 
 # Setting up
 setup(
```

### Comparing `colabseg-0.0.2/tests/test_segmentation_backend.py` & `colabseg-0.0.3/tests/test_segmentation_backend.py`

 * *Files identical despite different names*

### Comparing `colabseg-0.0.2/tests/test_utilities.py` & `colabseg-0.0.3/tests/test_utilities.py`

 * *Files identical despite different names*

