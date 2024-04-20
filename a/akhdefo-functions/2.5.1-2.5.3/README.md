# Comparing `tmp/akhdefo_functions-2.5.1.tar.gz` & `tmp/akhdefo_functions-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.5.1.tar", last modified: Tue Apr  9 22:07:06 2024, max compression
+gzip compressed data, was "akhdefo_functions-2.5.3.tar", last modified: Sat Apr 20 15:52:50 2024, max compression
```

## Comparing `akhdefo_functions-2.5.1.tar` & `akhdefo_functions-2.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.879460 akhdefo_functions-2.5.1/
--rw-rw-rw-   0        0        0    10250 2024-04-09 22:07:06.879460 akhdefo_functions-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.1/README.md
--rw-rw-rw-   0        0        0     8986 2024-04-08 23:21:41.000000 akhdefo_functions-2.5.1/README_pypi.md
-drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.862402 akhdefo_functions-2.5.1/akhdefo_functions/
--rw-rw-rw-   0        0        0    53386 2024-04-07 00:24:07.000000 akhdefo_functions-2.5.1/akhdefo_functions/AkhdefoPlot.py
--rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Classification.py
--rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Coreg.py
--rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_GOI.py
--rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_TS.py
--rw-rw-rw-   0        0        0    76847 2024-04-06 22:26:04.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-   0        0        0   153494 2024-04-06 23:34:54.000000 akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Utilities.py
--rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.1/akhdefo_functions/Filter_PreProc.py
--rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.1/akhdefo_functions/Mosaic_Crop.py
--rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.1/akhdefo_functions/OpticalFlow.py
--rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.1/akhdefo_functions/Stacked_Velocity.py
--rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.1/akhdefo_functions/Unzip_CopyFiles.py
--rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.1/akhdefo_functions/Video_Streamer.py
--rw-rw-rw-   0        0        0      683 2024-04-09 18:00:35.000000 akhdefo_functions-2.5.1/akhdefo_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 22:07:06.877407 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/
--rw-rw-rw-   0        0        0    10250 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-04-09 22:07:06.000000 akhdefo_functions-2.5.1/akhdefo_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1236 2024-04-09 18:18:45.000000 akhdefo_functions-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 22:07:06.880456 akhdefo_functions-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3634 2024-04-09 19:57:03.000000 akhdefo_functions-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/
+-rw-rw-rw-   0        0        0     9914 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.3/README.md
+-rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.3/README_pypi.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.597880 akhdefo_functions-2.5.3/akhdefo_functions/
+-rw-rw-rw-   0        0        0    53716 2024-04-20 15:48:45.000000 akhdefo_functions-2.5.3/akhdefo_functions/AkhdefoPlot.py
+-rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Classification.py
+-rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Coreg.py
+-rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_GOI.py
+-rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_TS.py
+-rw-rw-rw-   0        0        0    76847 2024-04-06 22:26:04.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Tools.py
+-rw-rw-rw-   0        0        0   156103 2024-04-18 20:56:23.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.3/akhdefo_functions/Filter_PreProc.py
+-rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.3/akhdefo_functions/Mosaic_Crop.py
+-rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.3/akhdefo_functions/OpticalFlow.py
+-rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.3/akhdefo_functions/Stacked_Velocity.py
+-rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.3/akhdefo_functions/Unzip_CopyFiles.py
+-rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.3/akhdefo_functions/Video_Streamer.py
+-rw-rw-rw-   0        0        0      717 2024-04-20 15:52:36.000000 akhdefo_functions-2.5.3/akhdefo_functions/__init__.py
+-rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.3/akhdefo_functions/backend.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/
+-rw-rw-rw-   0        0        0     9914 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-04-19 23:45:20.000000 akhdefo_functions-2.5.3/setup.py
```

### Comparing `akhdefo_functions-2.5.1/PKG-INFO` & `akhdefo_functions-2.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: akhdefo_functions
-Version: 2.5.1
-Summary: Land Deformation Monitoring Using Optical Satellite Imagery
+Version: 2.5.3
+Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
-Author-email: Mahmud Mustafa Muhammad <mahmud.muhamm1@gmail.com>
+Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
-Project-URL: GitHub-Page, https://github.com/mahmudsfu/AkhDefo
-Project-URL: Bug Tracker, https://github.com/mahmudsfu/AkhDefo/issues
-Project-URL: ReadMe, https://akhdefo.readthedocs.io/en/latest/README.html
-Project-URL: Documentation-Homepage, https://akhdefo.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Akhdefo
 
 
 [<img src="https://akhdefo.readthedocs.io/en/latest/_images/akhdefo_logo.svg" alt="Akhdefo Project Image" align="right" width="200px"/>](https://akhdefo.readthedocs.io/en/latest/index.html)
@@ -198,15 +193,15 @@
    ```
 
 2. Create  Anaconda environment and install the following libraries with Anaconda
 
 ```yaml
 
 dependencies:
-  - python=3.8  # Assuming Python 3.8, can be changed as needed
+  - python  # Assuming Python 3.8, can be changed as needed
   - cmocean
   - pip
   - opencv
   - earthpy
   - flask
   - geopandas
   - glob2
```

### Comparing `akhdefo_functions-2.5.1/README.md` & `akhdefo_functions-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/README_pypi.md` & `akhdefo_functions-2.5.3/README_pypi.md`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
    ```
 
 2. Create  Anaconda environment and install the following libraries with Anaconda
 
 ```yaml
 
 dependencies:
-  - python=3.8  # Assuming Python 3.8, can be changed as needed
+  - python  # Assuming Python 3.8, can be changed as needed
   - cmocean
   - pip
   - opencv
   - earthpy
   - flask
   - geopandas
   - glob2
```

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/AkhdefoPlot.py` & `akhdefo_functions-2.5.3/akhdefo_functions/AkhdefoPlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from sklearn.linear_model import LinearRegression
 from datetime import datetime
 import math
 from ipywidgets import interact
 from ipywidgets import widgets
 import plotly.io as pio
 import re
-
+from matplotlib_scalebar.scalebar import ScaleBar
 
 import os
 import re
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import TwoSlopeNorm, Normalize
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
@@ -58,14 +58,16 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 import re
 from datetime import datetime
 
+
+
 def akhdefo_viewer(path_to_dem_file, raster_file, output_folder, title='', 
                    pixel_resolution_meters=3.125, output_file_name="", 
                    alpha=0.5, unit_conversion=None, no_data_mask=False, 
                    colormap='jet', min_value=None, max_value=None, 
                    normalize=False, colorbar_label=None, show_figure=True , aspect_raster=None, cmap_aspect=None, step=10):
     """
     Overlays a raster file on a DEM hillshade and saves the plot as a PNG image.
@@ -94,15 +96,15 @@
     None
     """
     try:
         
         with rasterio.open(path_to_dem_file) as src:
             # Number of bands
             band_count = src.count
-                
+            xres, yres=src.res
             if band_count >2:
                 dem = src.read(masked=True)
                 dem_transform = src.transform
                 hillshade=dem
                 
             else:
                 dem = src.read(1, masked=True)
@@ -111,15 +113,15 @@
                 hillshade = es.hillshade(dem)
                 
 
         with rasterio.open(raster_file) as src:
             raster = src.read(1, masked=True)
             raster_transform = src.transform
             raster_crs = src.crs
-            xres, yres=src.res
+    
 
         if no_data_mask:
             raster = np.ma.masked_where(raster == 0, raster)
 
         if unit_conversion:
             unit_type, unit_factor = _separate_floats_letters(unit_conversion)
             raster *= float(unit_factor)
@@ -278,27 +280,27 @@
     else:
         ax.set_xlabel('Easting')
         ax.set_ylabel('Northing')
 
     #ax.grid(True, which='major')
     ax.set_title(title)
 
-    # Add scale bar
-    if pixel_resolution_meters is not None:
-        scalebar = AnchoredSizeBar(ax.transData, 100, f'{100 * pixel_resolution_meters} m', 'lower right',
-                                   pad=0.6, color='black', frameon=True, size_vertical=1)
-        ax.add_artist(scalebar)
+   
+        
+    scalebar = ScaleBar(dx=pixel_resolution_meters, location='lower right', units='m',
+                        frameon=True, scale_loc='bottom', dimension='si-length', box_color='white', color='k', border_pad=1, box_alpha=0.65)  # Adjust parameters as needed
+   
+    ax.add_artist(scalebar)
       
     # Save the plot
     plt.savefig(os.path.join(output_folder, output_file_name), dpi=100, bbox_inches='tight')
 
 
 
 
-
 def plot_stackNetwork(src_folder="", output_folder="", cmap='tab20', date_plot_interval=(5, 30), marker_size=15):
     
     """
     Generates a scatter plot to visualize the time intervals between dates extracted from the filenames of .tif files.
     The function handles filenames containing single or multiple dates. For multiple dates, it calculates the interval 
     between the first and last date. For single dates, it calculates the interval between consecutive dates.
 
@@ -719,14 +721,15 @@
     dnames = [col for col in gdf.columns if col.startswith('D')]
     # Define path to dem data
     #dem_path = 'dem.tif'
 
     with rio.open(dem_path) as src:
         elevation = src.read(1)
         elevation = elevation.astype('float32')
+        xres, yres=src.res
         # Set masked values to np.nan
         elevation[elevation < 0.0] = np.nan
         
     # Create and plot the hillshade with earthpy
     hillshade = es.hillshade(elevation, azimuth=270, altitude=45)
 
     dem = rxr.open_rasterio(dem_path, masked=True)
@@ -739,15 +742,14 @@
     # Transforming the shapefile to the dem data crs
     gdf = gdf.to_crs(dem_crs)
     
     
     min=gdf[color_field].min()
     max=gdf[color_field].max()
     import matplotlib.colors as mcolors
-    from matplotlib_scalebar.scalebar import ScaleBar
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     
     
     if min < 0 and max >0 :
         if Set_fig_MinMax==True:
             min_n=MinMaxRange[0]
             max_n=MinMaxRange[1]
@@ -779,16 +781,17 @@
     
     divider = make_axes_locatable(ax1)
     cax = divider.append_axes('bottom', size='5%', pad=0.5)
     
     #fig, ax1 = plt.subplots(ncols=1, nrows=1, figsize=(10,5))
     ep.plot_bands( hillshade,cbar=False,title=basename,extent=dem_plotting_extent,ax=ax1, scale=False)
     img_main=ax1.scatter(gdf.x, gdf.y, c=gdf[color_field], alpha=opacity, s=point_size, picker=1, cmap=cmap, norm=offset)
-    scalebar = ScaleBar(1, "m", length_fraction=0.25, scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right')
-    ax1.add_artist(scalebar)
+    #scalebar = ScaleBar(dx=xres, units='m', location='lower right',frameon=False, scale_loc='bottom')
+    #scalebar = ScaleBar(xres, "m", scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right', ax=ax1)
+    #ax1.add_artist(scalebar)
     plt.grid(True)
     #ax.scatter(gdf.x, gdf.y, s= 0.5, c=gdf.VEL_MEAN ,picker=1)
     cb=fig.colorbar(img_main, ax=ax1, cax=cax, extend='both', orientation='horizontal')
     cb.set_label('mm/year', labelpad=2, x=0.5, rotation=0)
     
     global count
     count=0
@@ -1145,14 +1148,15 @@
     gdf = gpd.read_file(shapefile_path)
     gdf.crs
     # Define path to dem data
     #dem_path = 'dem.tif'
 
     with rio.open(dem_path) as src:
         elevation = src.read(1)
+        xres, yres=src.res
         elevation = elevation.astype('float32')
         # Set masked values to np.nan
         elevation[elevation < 0.0] = np.nan
     # Create and plot the hillshade with earthpy
     hillshade = es.hillshade(elevation, azimuth=275, altitude=30)
 
     dem = rxr.open_rasterio(dem_path, masked=True)
@@ -1168,15 +1172,14 @@
     if not os.path.exists(out_folder):
         os.makedirs(out_folder)
     
     if batch_plot==False:
         min=gdf[color_field].min()
         max=gdf[color_field].max()
         import matplotlib.colors as mcolors
-        from matplotlib_scalebar.scalebar import ScaleBar
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         
         
         if min < 0 and max >0 :
             if Set_fig_MinMax==True:
                 min_n=MinMaxRange[0]
                 max_n=MinMaxRange[1]
@@ -1220,16 +1223,17 @@
         else:
             x=gdf.geometry.x
             y=gdf.geometry.y
         #fig, ax1 = plt.subplots(ncols=1, nrows=1, figsize=(10,5))
         ep.plot_bands( hillshade,cbar=False,title=color_field,extent=dem_plotting_extent,ax=ax1, scale=False)
         
         img_main=ax1.scatter(x, y, c=gdf[color_field], alpha=opacity, s=point_size, picker=1, cmap=cmap, norm=offset)
-        scalebar = ScaleBar(1, "m", length_fraction=0.25, scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right')
-        ax1.add_artist(scalebar)
+        #scalebar = ScaleBar(xres, "m", scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right', ax=ax1)
+        #scalebar = ScaleBar(dx=xres, units='m', location='lower right',frameon=False, scale_loc='bottom')
+        #ax1.add_artist(scalebar)
         ax1.grid(True)
         #ax.scatter(gdf.x, gdf.y, s= 0.5, c=gdf.VEL_MEAN ,picker=1)
         cb=fig.colorbar(img_main, ax=ax1, cax=cax, extend='both', orientation='horizontal')
         cb.set_label(cbar_label, labelpad=2, x=0.5, rotation=0)
          # Rotate colorbar labels
         for label in cb.ax.get_xticklabels():
             label.set_rotation(25)
@@ -1240,16 +1244,17 @@
                 ax1.legend()
        
         
         if plot_inverse_Vel==True:
             #fig, ax2 =inverse_Velocity(path_to_shapefile)
             
             ep.plot_bands( hillshade,cbar=False,title=color_field,extent=dem_plotting_extent,ax=ax2, scale=False)
-            scalebar = ScaleBar(1, "m", length_fraction=0.25, scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right')
-            ax2.add_artist(scalebar)
+            #scalebar = ScaleBar(xres, "m", scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right', ax=ax2)
+            #scalebar = ScaleBar(dx=xres, units='m', location='lower right',frameon=False, scale_loc='bottom')
+            #ax2.add_artist(scalebar)
             ax2.set_title('Inverse Velocity')
             
             if os.path.exists(xml_file_path):
                 if x_ref is not None:
                     ax2.scatter(x_ref, y_ref, label=f"Reference VEL,VEL_STD: {vel:.2f},{vel_std:.2f}", color='k', marker='s')
                     ax2.legend()
             
@@ -1269,15 +1274,14 @@
         dnames = [col for col in gdf.columns if col.startswith('D')]
        
             
         for nd in gdf[dnames]:
             min=gdf[nd].min()
             max=gdf[nd].max()
             import matplotlib.colors as mcolors
-            from matplotlib_scalebar.scalebar import ScaleBar
             from mpl_toolkits.axes_grid1 import make_axes_locatable
             
             
             if min < 0 and max >0 :
                 if Set_fig_MinMax==True:
                     min_n=MinMaxRange[0]
                     max_n=MinMaxRange[1]
@@ -1323,16 +1327,17 @@
                 y=gdf.y
             else:
                 x=gdf.geometry.x
                 y=gdf.geometry.y
             #fig, ax1 = plt.subplots(ncols=1, nrows=1, figsize=(10,5))
             ep.plot_bands( hillshade,cbar=False,title=nd,extent=dem_plotting_extent,ax=ax1, scale=False)
             img_main=ax1.scatter(x, y, c=gdf[nd], alpha=opacity, s=point_size, picker=1, cmap=cmap, norm=offset)
-            scalebar = ScaleBar(1, "m", length_fraction=0.25, scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right')
-            ax1.add_artist(scalebar)
+            #scalebar = ScaleBar(xres, "m", scale_loc="right",border_pad=1,pad=0.5, box_color='white', box_alpha=0.5, location='lower right', ax=ax1)
+            #scalebar = ScaleBar(dx=xres, units='m', location='lower right',frameon=False, scale_loc='bottom')
+            #ax1.add_artist(scalebar)
             plt.grid(True)
             #ax.scatter(gdf.x, gdf.y, s= 0.5, c=gdf.VEL_MEAN ,picker=1)
             cb=fig.colorbar(img_main, ax=ax1, cax=cax, extend='both', orientation='horizontal')
             cb.set_label(cbar_label, labelpad=2, x=0.5, rotation=0)
             
             if os.path.exists(xml_file_path):
                 if x_ref is not None:
```

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Classification.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Classification.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Coreg.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Coreg.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_GOI.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_GOI.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_TS.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_TS.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Tools.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Tools.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Akhdefo_Utilities.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 from skimage.registration import phase_cross_correlation
 import matplotlib
 import pandas as pd
 import tempfile
 
 from scipy.ndimage import convolve
 import matplotlib
-matplotlib.use('Agg')
+#matplotlib.use('Agg')
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import subprocess
 from skimage.metrics import structural_similarity as ssim
 # import required libraries
 # from vidgear.gears import CamGear
@@ -167,14 +167,16 @@
 import time
 from shapely.geometry import box
 import os
 import geopandas as gpd
 from shapely.geometry import Point
 
 
+
+
 def Akhdefo_resample(input_raster="", output_raster="" , xres=3.125 , yres=3.125, SavFig=False , convert_units=None):
     """
     This program performs raster resampling for  rasters
    
     Parameters:
     ------------
 
@@ -482,15 +484,15 @@
     
     # Set the GeoDataFrame to the calculated UTM CRS
     gdf.to_crs(epsg_code, inplace=True)
     return gdf 
 
 def Auto_Variogram(data="", column_attribute="", latlon=False, aoi_shapefile="", pixel_size=20,num_chunks=10,overlap_percentage=0, out_fileName='interpolated_kriging', 
                    plot_folder='kriging_plots', geo_folder='geo_rasterFolder', smoothing_kernel=2, mask: [np.ndarray] = None , 
-                   UTM_Zone=None, krig_method='ordinary' , drift_functions='linear', detrend_data=None, use_zscore=None):
+                   UTM_Zone=None, krig_method='ordinary' , drift_functions='linear', detrend_data=None, use_zscore=None, binning=False):
     
      
     """
     This function performs automatic selection of the optimal variogram model for spatial data interpolation. 
     It also supports clipping of the interpolation results to a specified Area of Interest (AOI). The function 
     accepts both GeoDataFrame objects and file paths (specifically, shapefile paths) as input data sources.
 
@@ -571,31 +573,74 @@
 
     Dependencies:
     -------------
         Requires geopandas, gstools, pykrige, matplotlib, and rasterio libraries.
     
     """
     
+    import geopandas as gpd
+    import numpy as np
+    from shapely.geometry import box
+
+    def create_spatial_grid(geodataframe, grid_size):
+        crs_ini=geodata.crs
+        # Create a grid
+        # Create a grid
+        xmin, ymin, xmax, ymax = geodataframe.total_bounds
+        xgrid = np.arange(xmin, xmax + grid_size, grid_size)
+        ygrid = np.arange(ymin, ymax + grid_size, grid_size)
+        grid_cells = [box(x1, y1, x2, y2) for x1, x2 in zip(xgrid[:-1], xgrid[1:]) for y1, y2 in zip(ygrid[:-1], ygrid[1:])]
+        grid = gpd.GeoDataFrame(geometry=grid_cells, crs=geodataframe.crs)
+
+        # Spatial join points to the grid
+        joined_gdf = gpd.sjoin(geodataframe, grid, how="inner", op="within")
+        joined_gdf = joined_gdf.rename(columns={"index_right": "grid_id"})  # Rename 'index_right' to 'grid_id' to avoid ambiguity
+        joined_gdf.reset_index(drop=True, inplace=True)
+
+        # Select numeric columns to dissolve
+        numeric_cols = joined_gdf.select_dtypes(include=[np.number]).columns.tolist()
+        if 'grid_id' in numeric_cols:
+            numeric_cols.remove('grid_id')  # Ensure 'grid_id' is not included in the aggregation
+
+        # Dissolve by new grid ID and compute mean for each grid cell for numeric data only
+        binned_gdf = joined_gdf.dissolve(by="grid_id", aggfunc={col: 'mean' for col in numeric_cols})
+
+        # Calculate the centroid of each grid cell
+        binned_gdf['geometry'] = binned_gdf.geometry.centroid
+        
+        binned_gdf.crs=geodata.crs
+        return binned_gdf
+
+    
     if isinstance(data, str):
         if data[-4:] == '.shp':
             geodata = gpd.read_file(data)
             
+            
+            
             if geodata.crs == "EPSG:4326":
                 geodata=set_gdf_to_utm(geodata)
                 
+            if binning==True:
+            # Create the spatial grid
+                geodata = create_spatial_grid(geodata, pixel_size)
+            
             crs_ini=geodata.crs
            
             
         else:
             raise ValueError("Unsupported file format.")
     elif isinstance(data, gpd.GeoDataFrame):
         geodata = data
+       
         if geodata.crs == "EPSG:4326":
             geodata=set_gdf_to_utm(geodata)
-        
+         # Create the spatial grid
+        if binning==True:
+            geodata = create_spatial_grid(geodata, pixel_size)
     else:
         raise ValueError("Unsupported data type.")
     
     # Check for necessary columns in the shapefile
     #check_shapefile_columns(geodata, latlon)
     
     # Change the dtype of a specific column to float32
@@ -613,14 +658,17 @@
         # else:
         #     x=geodata.geometry.x
         #     y=geodata.geometry.y
             # x, y = utm_to_latlon(easting=geodata.geometry.x, northing=geodata.geometry.y, zone_number=10, zone_letter=UTM_Zone)
     else:
         x, y = geodata.geometry.x, geodata.geometry.y
 
+    
+    
+    
     z = geodata[column_attribute]
     
     # Ensure x, y, and z are float32
     x = x.astype(np.float32)
     y = y.astype(np.float32)
     z = geodata[column_attribute].astype(np.float32)
     
@@ -670,15 +718,15 @@
 
     scores = {}
     #fig, (ax1, ax2, ax3) = plt.subplots(ncols=1, nrows=3, figsize=(15, 10))
     
 
     import matplotlib.gridspec as gridspec
     # Setting up a professional style
-    plt.style.use('seaborn-white')
+    #plt.style.use('seaborn-white')
     plt.rcParams.update({'font.size': 12})
     
     # Create a grid for the subplots
     fig = plt.figure(figsize=(18, 12))
     grid_fig = gridspec.GridSpec(2, 2, height_ratios=[1, 2])
 
     ax1=plt.subplot(grid_fig[0,:])
@@ -2014,15 +2062,15 @@
     adjusted_frame = frame + brightness
     adjusted_frame = np.clip(adjusted_frame, 0, 255).astype(np.uint8)
     return adjusted_frame
 
 import cv2
 import numpy as np
 import matplotlib
-matplotlib.use('WebAgg')
+#matplotlib.use('WebAgg')
 import matplotlib.pyplot as plt
 import subprocess
 from skimage.metrics import structural_similarity as ssim
 # import required libraries
 #from vidgear.gears import CamGear
 import time
 from scipy.ndimage import shift as shift_cor
@@ -3775,39 +3823,61 @@
     - If no points are within the AOI, no file is created, and a message is printed.
     
     """
 
     
     # Read point shapefile
     points = gpd.read_file(point_shapefile)
-   
-
-    # Read AOI polygon shapefile
+    
+    #print ('points CRS: ', points.crs)
+    
+     # Read AOI polygon shapefile
     aoi = gpd.read_file(aoi_shapefile)
+    
+    #print ('AOI CRS: ', aoi.crs)
+    
+    # Check if the CRS is not latlong (EPSG:4326)
+    if points.crs == "EPSG:4326":
+        print("The GeoDataFrame is not in latlong CRS format.")
+        points=set_gdf_to_utm(points)
+    else:
+        print("The GeoDataFrame is in latlong CRS format.")
+
+    #print ('points CRS: ', points.crs)
+    
+    
+
+
+    # Check if CRS transformation is needed
+    if points.crs != aoi.crs:
+        points = points.to_crs(aoi.crs)  # Match CRS of AOI
 
     # Dissolve the AOI polygon to a single geometry without specifying 'by'
     dissolved_aoi = aoi.dissolve()
     
      # Ensure both GeoDataFrames have the same CRS
     dissolved_aoi = dissolved_aoi.to_crs(points.crs)
 
     # Use geopandas.overlay to clip points by AOI polygon
     points_in_aoi = gpd.overlay(points, dissolved_aoi, how='intersection')
+    points_in_aoi.crs=points.crs
 
     # Check if the resulting GeoDataFrame is empty
     if not points_in_aoi.empty:
         # Create the output folder if it doesn't exist
         os.makedirs(output_folder, exist_ok=True)
 
         # Construct the output shapefile path
         output_filename = os.path.basename(point_shapefile).replace(".shp", "_clipped.shp")
         output_shapefile = os.path.join(output_folder, output_filename)
 
+        #print(points_in_aoi.crs, 'final crs')
+        
         # Save the clipped points to the output shapefile
-        points_in_aoi.to_file(output_shapefile)
+        points_in_aoi.to_file(output_shapefile, driver="ESRI Shapefile")
 
        
     else:
         print("The resulting GeoDataFrame is empty. No file will be written.")
         
 
 ####################
```

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Filter_PreProc.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Filter_PreProc.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Mosaic_Crop.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Mosaic_Crop.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/OpticalFlow.py` & `akhdefo_functions-2.5.3/akhdefo_functions/OpticalFlow.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Stacked_Velocity.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Stacked_Velocity.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Unzip_CopyFiles.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Unzip_CopyFiles.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/Video_Streamer.py` & `akhdefo_functions-2.5.3/akhdefo_functions/Video_Streamer.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions/__init__.py` & `akhdefo_functions-2.5.3/akhdefo_functions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 akhdefo_functions
 
 collection of python modules performs geospatial image processing to moniter land deformation
 """
 
-__version__ = "2.5.1"
+__version__ = "2.5.3"
 __author__ = 'Mahmud Mustafa Muhammad: mahmud.muhamm1@gmail.com'
 __credits__ = 'Simon Fraser university-Department of Earth Sciences'
 
 
+
+
+from  .backend import*
 from .AkhdefoPlot import*
 from .Akhdefo_Tools import*
 from .Akhdefo_TS import*
 from .Filter_PreProc import*
 from .Mosaic_Crop import*
 from .OpticalFlow import*
 from .Stacked_Velocity import*
@@ -21,7 +24,10 @@
 from .Akhdefo_Utilities import*
 from .Akhdefo_Classification import*
 from .Akhdefo_GOI import*
 from .Video_Streamer import*
 
 
 
+
+
+
```

### Comparing `akhdefo_functions-2.5.1/akhdefo_functions.egg-info/PKG-INFO` & `akhdefo_functions-2.5.3/akhdefo_functions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: akhdefo-functions
-Version: 2.5.1
-Summary: Land Deformation Monitoring Using Optical Satellite Imagery
+Version: 2.5.3
+Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
-Author-email: Mahmud Mustafa Muhammad <mahmud.muhamm1@gmail.com>
+Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
-Project-URL: GitHub-Page, https://github.com/mahmudsfu/AkhDefo
-Project-URL: Bug Tracker, https://github.com/mahmudsfu/AkhDefo/issues
-Project-URL: ReadMe, https://akhdefo.readthedocs.io/en/latest/README.html
-Project-URL: Documentation-Homepage, https://akhdefo.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Akhdefo
 
 
 [<img src="https://akhdefo.readthedocs.io/en/latest/_images/akhdefo_logo.svg" alt="Akhdefo Project Image" align="right" width="200px"/>](https://akhdefo.readthedocs.io/en/latest/index.html)
@@ -198,15 +193,15 @@
    ```
 
 2. Create  Anaconda environment and install the following libraries with Anaconda
 
 ```yaml
 
 dependencies:
-  - python=3.8  # Assuming Python 3.8, can be changed as needed
+  - python  # Assuming Python 3.8, can be changed as needed
   - cmocean
   - pip
   - opencv
   - earthpy
   - flask
   - geopandas
   - glob2
```

### Comparing `akhdefo_functions-2.5.1/pyproject.toml` & `akhdefo_functions-2.5.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,58 @@
+import subprocess
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+from setuptools import Command, setup
 
 
-
-[project]
-name = "akhdefo_functions"
-version = "2.5.1"
-authors = [
-  { name="Mahmud Mustafa Muhammad", email="mahmud.muhamm1@gmail.com" },
-]
-description = "Land Deformation Monitoring Using Optical Satellite Imagery"
-readme = "./README_pypi.md"
-requires-python = ">=3.7"
-
-classifiers = [
-    'Development Status :: 3 - Alpha',
+class BuildDoc(Command):
+    """A custom command to build Sphinx documentation."""
+    
+    description = 'build Sphinx documentation'
+    user_options = []
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        subprocess.call(['sphinx-build', '-b', 'html', 'docs', 'docs/_build/html'])
+
+
+# Define command class for building Sphinx documentation
+cmdclass = {'build_sphinx': BuildDoc}
+
+# Read the long description from the README file
+with open("./README_pypi.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+# Setup configuration
+setup(
+    name='akhdefo_functions',
+    version='2.5.3',
+    description='Land Deformation Monitoring Using Optical and SAR Satellite Imagery',
+    url='https://github.com/mahmudsfu/AkhDefo',
+    author='Mahmud Mustafa Muhammad',
+    author_email='mahmud.muhamm1@gmail.com',
+    license='Academic Free License (AFL)',
+    packages=['akhdefo_functions'],
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    zip_safe=False,
+    classifiers=[
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Academic Free License (AFL)',  
         'Operating System :: Microsoft :: Windows :: Windows 10',
         'Operating System :: POSIX :: Linux',        
-        'Programming Language :: Python :: 3',  'Programming Language :: Python :: 3.6',  
-        'Programming Language :: Python :: 3.7', "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-]
-
-[project.urls]
-"GitHub-Page" = "https://github.com/mahmudsfu/AkhDefo"
-"Bug Tracker" = "https://github.com/mahmudsfu/AkhDefo/issues"
-"ReadMe" = "https://akhdefo.readthedocs.io/en/latest/README.html"
-"Documentation-Homepage" = "https://akhdefo.readthedocs.io/en/latest/"
-
-
-
+        'Programming Language :: Python :: 3',  
+        'Programming Language :: Python :: 3.6',  
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ], 
+    cmdclass=cmdclass 
+    
+)
```

