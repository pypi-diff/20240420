# Comparing `tmp/noteshrunk-1.3.0.tar.gz` & `tmp/noteshrunk-1.4.0.tar.gz`

## Comparing `noteshrunk-1.3.0.tar` & `noteshrunk-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/CHANGELOG.md
--rwxr-xr-x   0        0        0    24255 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/src/noteshrunk.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/LICENSE
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    45903 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0    25034 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/src/noteshrunk.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/README.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    47774 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/PKG-INFO
```

### Comparing `noteshrunk-1.3.0/CHANGELOG.md` & `noteshrunk-1.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.3.0/src/noteshrunk.py` & `noteshrunk-1.4.0/src/noteshrunk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
-VERSION = '1.3.0'
+VERSION = '1.4.0'
 
 import argparse
 from concurrent.futures import ThreadPoolExecutor
 import os
 from pathlib import Path
 import random
 import re
@@ -14,16 +14,16 @@
 
 import argcomplete
 import numpy as np
 from PIL import Image
 from scipy.ndimage import median_filter
 from skimage import io
 from sklearn.cluster import KMeans
-from skimage.color import rgb2hsv
-from skimage.morphology import binary_opening, binary_closing, square, disk
+from skimage.filters import unsharp_mask
+from skimage.morphology import binary_opening, square, disk
 
 
 def parse_args():
     """
     Parses command line arguments.
 
     Returns:
@@ -105,50 +105,56 @@
         type=float,
         default=15,
         help="HSV saturation threshold (in percent) used for the background detection.")
     parser.add_argument(
         "-tv",
         "--threshold_value",
         type=float,
-        default=25,
+        default=20,
         help="HSV value threshold (in percent) used for the background detection.")
     parser.add_argument(
         '--denoise_median',
         action='store_true',
         default=False,
         help='Apply median denoising.')
     parser.add_argument(
-        '--denoise_closing',
+        '--denoise_opening',
         action='store_true',
         default=False,
-        help='Apply morphological closing on the (binary) background mask.')
+        help='Apply morphological opening on the (binary) background mask.')
     parser.add_argument(
-        '--denoise_opening',
+        '--unsharp_mask',
         action='store_true',
         default=False,
-        help='Apply morphological opening on the (binary) background mask.')
+        help='Apply unsharp masking with radius <-ur> and amount <-ua> to the V-channel of the output image in HSV representation.')
     parser.add_argument(
         "-ms",
         "--median_strength",
         type=int,
         default=3,
         help="Strength of median filtering")
     parser.add_argument(
-        "-cs",
-        "--closing_strength",
-        type=float,
-        default=3,
-        help="Strength of closing filtering / radius of the structuring element (disk)")
-    parser.add_argument(
         "-os",
         "--opening_strength",
         type=float,
         default=3,
         help="Strength of opening filtering / radius of the structuring element (disk)")
     parser.add_argument(
+        "-ua",
+        "--unsharp_amount",
+        type=float,
+        default=2,
+        help="The amount used for unsharp masking.")
+    parser.add_argument(
+        "-ur",
+        "--unsharp_radius",
+        type=float,
+        default=5,
+        help="The radius used for unsharp masking.")
+    parser.add_argument(
         '-k',
         '--keep_intermediate',
         action='store_true',
         default=False,
         help='Do not delete intermediate (single-page) PDFs afterwards.')
     parser.add_argument(
         '-v',
@@ -448,30 +454,23 @@
     image = image.reshape((-1, 3))
     foreground_mask = get_foreground_mask(
         image,
         background_color=color_palette[0],
         threshold_saturation=args.threshold_saturation,
         threshold_value=args.threshold_value)
 
+    # morphological opening of the binary foreground mask to remove e.g. dust speckles
     if args.denoise_opening:
         verbose_print(args, 'Applying opening ...')
         # disk(<1) results in id-operation or zero-matrix and is hence useless
         kernel = disk(
             args.opening_strength) if args.opening_strength >= 1 else square(2)
         foreground_mask = binary_opening(
             foreground_mask.reshape(shape[:-1]), kernel).flatten()
 
-    if args.denoise_closing:
-        verbose_print(args, 'Applying closing ...')
-        # disk(<1) results in id-operation or zero-matrix and is hence useless
-        kernel = disk(
-            args.opening_strength) if args.opening_strength >= 1 else square(2)
-        foreground_mask = binary_closing(
-            foreground_mask.reshape(shape[:-1]), kernel).flatten()
-
     labels = np.zeros(image.shape[0], dtype='uint8')
 
     verbose_print(args, 'Applying color palette ...')
     labels[foreground_mask] = kmeans_model.predict(image[foreground_mask]) + 1
 
     if args.saturate:
         verbose_print(args, 'Maximizing saturation ...')
@@ -482,24 +481,36 @@
         color_palette = color_palette.round(0).astype('uint8')
 
     image = color_palette[labels]
 
     # set background to the background color
     image[~foreground_mask] = color_palette[0]
 
+    if args.unsharp_mask:
+        verbose_print(args, 'Applying unsharp mask filtering ...')
+
+        image = np.array( Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV') )
+
+        #
+        tmp_max = np.max(image[:,:,2])
+        image[:,:,2] = (unsharp_mask(image[:,:,2],
+                                    radius=args.unsharp_radius,
+                                    amount=args.unsharp_amount) * tmp_max).round(0).astype('uint8')
+        image = np.array( Image.fromarray(image, mode='HSV').convert('RGB') ).reshape((-1,3))
+
     if args.denoise_median:
         verbose_print(args, 'Applying median filtering ...')
         # Median filtering is per color channel. In RGB space this would lead
         # to color deviations.
-        image = Image.fromarray(image.reshape(shape)).convert('HSV')
+        image = Image.fromarray(image.reshape(shape), mode='RGB').convert('HSV')
         image = median_filter(
             image,
             size=(args.median_strength, args.median_strength, 1)
         )
-        image = Image.fromarray(image, 'HSV').convert('RGB')
+        image = Image.fromarray(image, mode='HSV').convert('RGB')
         return np.array(image)
 
     else:
         return image.reshape(shape)
 
 
 def generate_random_string(length=8):
@@ -655,15 +666,16 @@
                    '-sOUTPUTFILE={}'.format(filename),
                    '-dBATCH'] + [str(f) for f in filename_paths]
 
         subprocess.run(command, check=True, capture_output=True)
 
     except subprocess.CalledProcessError as e:
         print(f"Error: {e}")
-        print("Please ensure that gs (ghostscript) is installed and accessible from the command line.")
+        print("Error:", e.stderr.decode('utf-8') if e.stderr is not None else None)
+        print("Stdout was:", e.stdout.decode('utf-8') if e.stdout is not None else None)
 
     verbose_print(args, 'Output written to', args.output)
 
 
 def process_image(file, output_filename, idx, args, global_palette=None):
     """
     Process a single image and save it as a PDF.
@@ -740,28 +752,35 @@
         intermediate_pdf_paths = []
 
         if not args.local_palette:
             color_palette, kmeans_model = create_palette(file_paths, args, use_global_palette=True)
 
         with ThreadPoolExecutor(max_workers=args.jobs) as executor:
 
+            threads = []
             for idx, file in enumerate(file_paths):
 
                 output_filename = args.output.parent / temp_dir / Path(file.name).with_suffix('.pdf')
 
                 # E.g. the same input file multiple times
                 if output_filename in intermediate_pdf_paths or output_filename.exists():
                     output_filename = rename_with_random_string(output_filename)
 
-                executor.submit(process_image, file=file, output_filename=output_filename, idx=idx, args=args,
-                                 global_palette=(color_palette, kmeans_model) if not args.local_palette else None)
+                threads.append(executor.submit(process_image, file=file, output_filename=output_filename, idx=idx, args=args,
+                                 global_palette=(color_palette, kmeans_model) if not args.local_palette else None))
 
                 intermediate_pdf_paths.append(output_filename)
 
             executor.shutdown(wait=True)
+            try:
+                for f in threads:
+                    f.result()  # This will raise a ValueError in case the thread crashed
+            except ValueError as e:
+                print(f"Caught an error: {e}")
+
 
         verbose_print(
             args,
             'Skipping the deletion of intermediate PDFs (folder {}).'.format(temp_dir),
             conditions=[args.keep_intermediate]
         )
```

### Comparing `noteshrunk-1.3.0/.gitignore` & `noteshrunk-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.3.0/LICENSE` & `noteshrunk-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.3.0/README.md` & `noteshrunk-1.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -64,232 +64,348 @@
 000003f0: 6f76 6520 7468 6520 6261 636b 6772 6f75  ove the backgrou
 00000400: 6e64 2028 7265 706c 6163 6520 7769 7468  nd (replace with
 00000410: 2077 6869 7465 292c 2065 6e68 616e 6369   white), enhanci
 00000420: 6e67 2076 6973 7561 6c20 636c 6172 6974  ng visual clarit
 00000430: 792e 0a2a 202a 2a44 656e 6f69 7369 6e67  y..* **Denoising
 00000440: 204f 7074 696f 6e73 3a2a 2a20 5072 6f76   Options:** Prov
 00000450: 6964 6573 206d 6564 6961 6e20 6669 6c74  ides median filt
-00000460: 6572 696e 6720 616e 6420 6d6f 7270 686f  ering and morpho
-00000470: 6c6f 6769 6361 6c20 6f70 6572 6174 696f  logical operatio
-00000480: 6e73 2074 6f20 7265 6475 6365 206e 6f69  ns to reduce noi
-00000490: 7365 2061 6e64 2069 6d70 726f 7665 2069  se and improve i
-000004a0: 6d61 6765 2071 7561 6c69 7479 2e0a 2a20  mage quality..* 
-000004b0: 2a2a 5061 7261 6c6c 656c 2070 726f 6365  **Parallel proce
-000004c0: 7373 696e 673a 2a2a 2055 7469 6c69 7a65  ssing:** Utilize
-000004d0: 7320 6d75 6c74 6970 6c65 2043 5055 2063  s multiple CPU c
-000004e0: 6f72 6573 2066 6f72 2066 6173 7465 7220  ores for faster 
-000004f0: 7072 6f63 6573 7369 6e67 206f 6620 6d75  processing of mu
-00000500: 6c74 6970 6c65 2069 6d61 6765 732e 0a0a  ltiple images...
-00000510: 2323 2052 6571 7569 7265 6d65 6e74 730a  ## Requirements.
-00000520: 0a23 2323 2050 7974 686f 6e20 5061 636b  .### Python Pack
-00000530: 6167 6573 0a0a 2d20 6172 6763 6f6d 706c  ages..- argcompl
-00000540: 6574 650a 2d20 4e75 6d50 790a 2d20 5069  ete.- NumPy.- Pi
-00000550: 6c6c 6f77 2028 5049 4c20 466f 726b 290a  llow (PIL Fork).
-00000560: 2d20 5079 7468 6f6e 2033 0a2d 2073 6369  - Python 3.- sci
-00000570: 6b69 742d 696d 6167 650a 2d20 7363 696b  kit-image.- scik
-00000580: 6974 2d6c 6561 726e 0a2d 2053 6369 5079  it-learn.- SciPy
-00000590: 0a0a 2323 2320 4f74 6865 720a 0a2d 2047  ..### Other..- G
-000005a0: 686f 7374 7363 7269 7074 2028 6578 6563  hostscript (exec
-000005b0: 7574 6162 6c65 2060 6773 6020 696e 2050  utable `gs` in P
-000005c0: 4154 4820 2d20 666f 7220 5044 4620 6d65  ATH - for PDF me
-000005d0: 7267 696e 6729 0a0a 2323 2049 6e73 7461  rging)..## Insta
-000005e0: 6c6c 6174 696f 6e0a 0a60 6060 6261 7368  llation..```bash
-000005f0: 0a70 6970 7820 696e 7374 616c 6c20 6e6f  .pipx install no
-00000600: 7465 7368 7275 6e6b 0a60 6060 0a0a 2323  teshrunk.```..##
-00000610: 2055 7361 6765 0a0a 6060 600a 6e6f 7465   Usage..```.note
-00000620: 7368 7275 6e6b 205b 2d68 5d20 5b2d 6f20  shrunk [-h] [-o 
-00000630: 4f55 5450 5554 5d20 5b2d 775d 205b 2d73  OUTPUT] [-w] [-s
-00000640: 5d20 5b2d 6e20 4e5f 434f 4c4f 5253 5d20  ] [-n N_COLORS] 
-00000650: 5b2d 6420 4450 495d 205b 2d71 205b 312d  [-d DPI] [-q [1-
-00000660: 3130 305d 5d20 5b2d 6c5d 0a20 2020 2020  100]] [-l].     
-00000670: 2020 2020 2020 5b2d 7020 5045 5243 454e        [-p PERCEN
-00000680: 5441 4745 5d20 5b2d 6a20 4a4f 4253 5d20  TAGE] [-j JOBS] 
-00000690: 5b2d 795d 205b 2d74 7320 5448 5245 5348  [-y] [-ts THRESH
-000006a0: 4f4c 445f 5341 5455 5241 5449 4f4e 5d20  OLD_SATURATION] 
-000006b0: 5b2d 7476 2054 4852 4553 484f 4c44 5f56  [-tv THRESHOLD_V
-000006c0: 414c 5545 5d0a 2020 2020 2020 2020 2020  ALUE].          
-000006d0: 205b 2d2d 6465 6e6f 6973 655f 6d65 6469   [--denoise_medi
-000006e0: 616e 5d20 5b2d 2d64 656e 6f69 7365 5f63  an] [--denoise_c
-000006f0: 6c6f 7369 6e67 5d20 5b2d 2d64 656e 6f69  losing] [--denoi
-00000700: 7365 5f6f 7065 6e69 6e67 5d0a 2020 2020  se_opening].    
-00000710: 2020 2020 2020 205b 2d6d 7320 4d45 4449         [-ms MEDI
-00000720: 414e 5f53 5452 454e 4754 485d 205b 2d63  AN_STRENGTH] [-c
-00000730: 7320 434c 4f53 494e 475f 5354 5245 4e47  s CLOSING_STRENG
-00000740: 5448 5d20 5b2d 6f73 204f 5045 4e49 4e47  TH] [-os OPENING
-00000750: 5f53 5452 454e 4754 485d 0a20 2020 2020  _STRENGTH].     
-00000760: 2020 2020 2020 5b2d 6b5d 205b 2d76 5d20        [-k] [-v] 
-00000770: 5b2d 2d76 6572 7369 6f6e 5d20 6669 6c65  [--version] file
-00000780: 7320 5b66 696c 6573 202e 2e2e 5d0a 6060  s [files ...].``
-00000790: 600a 0a23 2323 2041 7267 756d 656e 7473  `..### Arguments
-000007a0: 0a0a 2a20 6066 696c 6573 603a 2041 206c  ..* `files`: A l
-000007b0: 6973 7420 6f66 2070 6174 6873 2074 6f20  ist of paths to 
-000007c0: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
-000007d0: 6669 6c65 732e 0a2a 2060 2d6f 602c 2060  files..* `-o`, `
-000007e0: 2d2d 6f75 7470 7574 603a 2050 6174 6820  --output`: Path 
-000007f0: 746f 2074 6865 206f 7574 7075 7420 5044  to the output PD
-00000800: 4620 6669 6c65 2028 6465 6661 756c 743a  F file (default:
-00000810: 2060 6f75 7470 7574 2e70 6466 6029 2e0a   `output.pdf`)..
-00000820: 2a20 602d 7760 2c20 602d 2d77 6869 7465  * `-w`, `--white
-00000830: 5f62 6163 6b67 726f 756e 6460 3a20 5573  _background`: Us
-00000840: 6520 7768 6974 6520 6261 636b 6772 6f75  e white backgrou
-00000850: 6e64 2069 6e73 7465 6164 206f 6620 646f  nd instead of do
-00000860: 6d69 6e61 6e74 2063 6f6c 6f72 2e0a 2a20  minant color..* 
-00000870: 602d 7360 2c20 602d 2d73 6174 7572 6174  `-s`, `--saturat
-00000880: 6560 3a20 4d61 7869 6d69 7a65 2073 6174  e`: Maximize sat
-00000890: 7572 6174 696f 6e20 696e 2074 6865 206f  uration in the o
-000008a0: 7574 7075 7420 696d 6167 652e 0a2a 2060  utput image..* `
-000008b0: 2d6e 602c 2060 2d2d 6e5f 636f 6c6f 7273  -n`, `--n_colors
-000008c0: 603a 204e 756d 6265 7220 6f66 2063 6f6c  `: Number of col
-000008d0: 6f72 7320 696e 2074 6865 2070 616c 6574  ors in the palet
-000008e0: 7465 2028 6465 6661 756c 743a 2038 292e  te (default: 8).
-000008f0: 0a2a 2060 2d64 602c 2060 2d2d 6470 6960  .* `-d`, `--dpi`
-00000900: 3a20 4450 4920 7661 6c75 6520 6f66 2074  : DPI value of t
-00000910: 6865 2069 6e70 7574 2069 6d61 6765 7320  he input images 
-00000920: 2864 6566 6175 6c74 3a20 3330 3029 2e0a  (default: 300)..
-00000930: 2a20 602d 7160 2c20 602d 2d71 7561 6c69  * `-q`, `--quali
-00000940: 7479 603a 204a 5045 4720 7175 616c 6974  ty`: JPEG qualit
-00000950: 7920 6f66 2074 6865 2069 6d61 6765 7320  y of the images 
-00000960: 656d 6265 6464 6564 2069 6e20 7468 6520  embedded in the 
-00000970: 5044 4620 2831 2d31 3030 2c20 6465 6661  PDF (1-100, defa
-00000980: 756c 743a 2037 3529 2e0a 2a20 602d 6c60  ult: 75)..* `-l`
-00000990: 2c20 602d 2d6c 6f63 616c 5f70 616c 6574  , `--local_palet
-000009a0: 7465 603a 2043 7265 6174 6520 616e 2069  te`: Create an i
-000009b0: 6e64 6976 6964 7561 6c20 636f 6c6f 7220  ndividual color 
-000009c0: 7061 6c65 7474 6520 666f 7220 6561 6368  palette for each
-000009d0: 2069 6d61 6765 2028 6279 2073 616d 706c   image (by sampl
-000009e0: 696e 6720 6120 2d70 2070 6572 6365 6e74  ing a -p percent
-000009f0: 6167 6520 6f66 2074 6865 2070 6978 656c  age of the pixel
-00000a00: 7320 6f66 2074 6861 7420 696d 6167 6529  s of that image)
-00000a10: 2069 6e73 7465 6164 206f 6620 6120 676c   instead of a gl
-00000a20: 6f62 616c 2070 616c 6574 7465 2028 6279  obal palette (by
-00000a30: 2073 616d 706c 696e 6720 6120 2d70 2070   sampling a -p p
-00000a40: 6572 6365 6e74 6167 6520 6f66 2074 6865  ercentage of the
-00000a50: 2070 6978 656c 7320 6f66 2065 6163 6820   pixels of each 
-00000a60: 696e 7075 7420 696d 6167 6529 2e0a 2a20  input image)..* 
-00000a70: 602d 7060 2c20 602d 2d70 6572 6365 6e74  `-p`, `--percent
-00000a80: 6167 6560 3a20 5065 7263 656e 7461 6765  age`: Percentage
-00000a90: 206f 6620 7069 7865 6c73 2074 6f20 7361   of pixels to sa
-00000aa0: 6d70 6c65 2066 726f 6d20 6561 6368 2069  mple from each i
-00000ab0: 6e70 7574 2069 6d61 6765 2066 6f72 2063  nput image for c
-00000ac0: 6f6c 6f72 2070 616c 6574 7465 2063 7265  olor palette cre
-00000ad0: 6174 696f 6e20 2864 6566 6175 6c74 3a20  ation (default: 
-00000ae0: 3130 292e 0a2a 2060 2d6a 602c 2060 2d2d  10)..* `-j`, `--
-00000af0: 6a6f 6273 603a 204e 756d 6265 7220 6f66  jobs`: Number of
-00000b00: 2074 6872 6561 6473 2074 6f20 7573 6520   threads to use 
-00000b10: 666f 7220 6d75 6c74 692d 7468 7265 6164  for multi-thread
-00000b20: 696e 6720 2864 6566 6175 6c74 3a20 6e75  ing (default: nu
-00000b30: 6d62 6572 206f 6620 4350 5520 636f 7265  mber of CPU core
-00000b40: 7329 2e0a 2a20 602d 7960 2c20 602d 2d6f  s)..* `-y`, `--o
-00000b50: 7665 7277 7269 7465 603a 204f 7665 7277  verwrite`: Overw
-00000b60: 7269 7465 2065 7869 7374 696e 6720 6669  rite existing fi
-00000b70: 6c65 7320 7769 7468 6f75 7420 6173 6b69  les without aski
-00000b80: 6e67 2e0a 2a20 602d 7473 602c 2060 2d2d  ng..* `-ts`, `--
-00000b90: 7468 7265 7368 6f6c 645f 7361 7475 7261  threshold_satura
-00000ba0: 7469 6f6e 603a 2048 5356 2073 6174 7572  tion`: HSV satur
-00000bb0: 6174 696f 6e20 7468 7265 7368 6f6c 6420  ation threshold 
-00000bc0: 2869 6e20 7065 7263 656e 7429 2075 7365  (in percent) use
-00000bd0: 6420 666f 7220 6261 636b 6772 6f75 6e64  d for background
-00000be0: 2064 6574 6563 7469 6f6e 2028 6465 6661   detection (defa
-00000bf0: 756c 743a 2031 3529 2e0a 2a20 602d 7476  ult: 15)..* `-tv
-00000c00: 602c 2060 2d2d 7468 7265 7368 6f6c 645f  `, `--threshold_
-00000c10: 7661 6c75 6560 3a20 4853 5620 7661 6c75  value`: HSV valu
-00000c20: 6520 7468 7265 7368 6f6c 6420 2869 6e20  e threshold (in 
-00000c30: 7065 7263 656e 7429 2075 7365 6420 666f  percent) used fo
-00000c40: 7220 6261 636b 6772 6f75 6e64 2064 6574  r background det
-00000c50: 6563 7469 6f6e 2028 6465 6661 756c 743a  ection (default:
-00000c60: 2032 3529 2e0a 2a20 602d 2d64 656e 6f69   25)..* `--denoi
-00000c70: 7365 5f6d 6564 6961 6e60 3a20 4170 706c  se_median`: Appl
-00000c80: 7920 6d65 6469 616e 2064 656e 6f69 7369  y median denoisi
-00000c90: 6e67 2e0a 2a20 602d 2d64 656e 6f69 7365  ng..* `--denoise
-00000ca0: 5f63 6c6f 7369 6e67 603a 2041 7070 6c79  _closing`: Apply
-00000cb0: 206d 6f72 7068 6f6c 6f67 6963 616c 2063   morphological c
-00000cc0: 6c6f 7369 6e67 206f 6e20 7468 6520 6261  losing on the ba
-00000cd0: 636b 6772 6f75 6e64 206d 6173 6b2e 0a2a  ckground mask..*
-00000ce0: 2060 2d2d 6465 6e6f 6973 655f 6f70 656e   `--denoise_open
-00000cf0: 696e 6760 3a20 4170 706c 7920 6d6f 7270  ing`: Apply morp
-00000d00: 686f 6c6f 6769 6361 6c20 6f70 656e 696e  hological openin
-00000d10: 6720 6f6e 2074 6865 2062 6163 6b67 726f  g on the backgro
-00000d20: 756e 6420 6d61 736b 2e0a 2a20 602d 6d73  und mask..* `-ms
-00000d30: 602c 2060 2d2d 6d65 6469 616e 5f73 7472  `, `--median_str
-00000d40: 656e 6774 6860 3a20 5374 7265 6e67 7468  ength`: Strength
-00000d50: 206f 6620 6d65 6469 616e 2066 696c 7465   of median filte
-00000d60: 7269 6e67 2028 6465 6661 756c 743a 2033  ring (default: 3
-00000d70: 292e 0a2a 2060 2d63 7360 2c20 602d 2d63  )..* `-cs`, `--c
-00000d80: 6c6f 7369 6e67 5f73 7472 656e 6774 6860  losing_strength`
-00000d90: 3a20 5374 7265 6e67 7468 206f 6620 636c  : Strength of cl
-00000da0: 6f73 696e 6720 6669 6c74 6572 696e 6720  osing filtering 
-00000db0: 2f20 7261 6469 7573 206f 6620 7468 6520  / radius of the 
-00000dc0: 7374 7275 6374 7572 696e 6720 656c 656d  structuring elem
-00000dd0: 656e 7420 2864 6973 6b2c 2064 6566 6175  ent (disk, defau
-00000de0: 6c74 3a20 3329 2e0a 2a20 602d 6f73 602c  lt: 3)..* `-os`,
-00000df0: 2060 2d2d 6f70 656e 696e 675f 7374 7265   `--opening_stre
-00000e00: 6e67 7468 603a 2053 7472 656e 6774 6820  ngth`: Strength 
-00000e10: 6f66 206f 7065 6e69 6e67 2066 696c 7465  of opening filte
-00000e20: 7269 6e67 202f 2072 6164 6975 7320 6f66  ring / radius of
-00000e30: 2074 6865 2073 7472 7563 7475 7269 6e67   the structuring
-00000e40: 2065 6c65 6d65 6e74 2028 6469 736b 2c20   element (disk, 
-00000e50: 6465 6661 756c 743a 2033 292e 0a2a 2060  default: 3)..* `
-00000e60: 2d6b 602c 2060 2d2d 6b65 6570 5f69 6e74  -k`, `--keep_int
-00000e70: 6572 6d65 6469 6174 6560 3a20 4b65 6570  ermediate`: Keep
-00000e80: 2074 6865 2069 6e74 6572 6d65 6469 6174   the intermediat
-00000e90: 6520 7369 6e67 6c65 2d70 6167 6520 5044  e single-page PD
-00000ea0: 4673 2e0a 2a20 602d 7660 2c20 602d 2d76  Fs..* `-v`, `--v
-00000eb0: 6572 626f 7365 603a 2056 6572 626f 7365  erbose`: Verbose
-00000ec0: 206f 7574 7075 742e 0a2a 2060 2d2d 7665   output..* `--ve
-00000ed0: 7273 696f 6e60 3a20 5368 6f77 2070 726f  rsion`: Show pro
-00000ee0: 6772 616d 2076 6572 7369 6f6e 2061 6e64  gram version and
-00000ef0: 2065 7869 742e 0a0a 2323 2045 7861 6d70   exit...## Examp
-00000f00: 6c65 730a 0a31 2e20 2043 6f6d 7072 6573  les..1.  Compres
-00000f10: 7320 6120 7369 6e67 6c65 2069 6d61 6765  s a single image
-00000f20: 2077 6974 6820 6465 6661 756c 7420 7365   with default se
-00000f30: 7474 696e 6773 3a0a 0a20 2020 2060 6060  ttings:..    ```
-00000f40: 6261 7368 0a20 2020 206e 6f74 6573 6872  bash.    noteshr
-00000f50: 756e 6b20 696e 7075 742e 706e 670a 2020  unk input.png.  
-00000f60: 2020 6060 600a 0a32 2e20 2043 6f6d 7072    ```..2.  Compr
-00000f70: 6573 7320 6d75 6c74 6970 6c65 2069 6d61  ess multiple ima
-00000f80: 6765 7320 7769 7468 2061 2077 6869 7465  ges with a white
-00000f90: 2062 6163 6b67 726f 756e 6420 616e 6420   background and 
-00000fa0: 3136 2063 6f6c 6f72 733a 0a0a 2020 2020  16 colors:..    
-00000fb0: 6060 6062 6173 680a 2020 2020 6e6f 7465  ```bash.    note
-00000fc0: 7368 7275 6e6b 202d 7720 2d6e 2031 3620  shrunk -w -n 16 
-00000fd0: 696d 6167 6531 2e6a 7067 2069 6d61 6765  image1.jpg image
-00000fe0: 322e 706e 670a 2020 2020 6060 600a 0a33  2.png.    ```..3
-00000ff0: 2e20 2043 6f6d 7072 6573 7320 696d 6167  .  Compress imag
-00001000: 6573 2075 7369 6e67 2061 206c 6f63 616c  es using a local
-00001010: 2063 6f6c 6f72 2070 616c 6574 7465 2061   color palette a
-00001020: 6e64 206b 6565 7020 696e 7465 726d 6564  nd keep intermed
-00001030: 6961 7465 2066 696c 6573 2077 6869 6c65  iate files while
-00001040: 2064 6973 6162 6c69 6e67 206d 756c 7469   disabling multi
-00001050: 2d74 6872 6561 6469 6e67 3a0a 2020 2020  -threading:.    
-00001060: 6060 6062 6173 680a 2020 2020 6e6f 7465  ```bash.    note
-00001070: 7368 7275 6e6b 202d 6c20 2d6a 2031 202d  shrunk -l -j 1 -
-00001080: 6b20 2a2e 6a70 670a 2020 2020 6060 600a  k *.jpg.    ```.
-00001090: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
-000010a0: 0a0a 436f 6e74 7269 6275 7469 6f6e 7320  ..Contributions 
-000010b0: 6172 6520 7765 6c63 6f6d 6521 2050 6c65  are welcome! Ple
-000010c0: 6173 6520 6665 656c 2066 7265 6520 746f  ase feel free to
-000010d0: 2073 7562 6d69 7420 6973 7375 6573 206f   submit issues o
-000010e0: 7220 7075 6c6c 2072 6571 7565 7374 7320  r pull requests 
-000010f0: 6f6e 2074 6865 2047 6974 4875 6220 7265  on the GitHub re
-00001100: 706f 7369 746f 7279 2e0a 0a23 2320 4163  pository...## Ac
-00001110: 6b6e 6f77 6c65 6467 656d 656e 7473 0a0a  knowledgements..
-00001120: 5468 6973 2070 726f 6a65 6374 2075 7469  This project uti
-00001130: 6c69 7a65 7320 6f70 656e 2d73 6f75 7263  lizes open-sourc
-00001140: 6520 736f 6674 7761 7265 2066 726f 6d20  e software from 
-00001150: 7468 6520 5079 7468 6f6e 2063 6f6d 6d75  the Python commu
-00001160: 6e69 7479 2e0a 5370 6563 6961 6c20 7468  nity..Special th
-00001170: 616e 6b73 2074 6f20 7468 6520 6465 7665  anks to the deve
-00001180: 6c6f 7065 7273 2061 6e64 206d 6169 6e74  lopers and maint
-00001190: 6169 6e65 7273 206f 6620 7468 6520 7265  ainers of the re
-000011a0: 7175 6972 6564 206c 6962 7261 7269 6573  quired libraries
-000011b0: 2061 7320 7765 6c6c 2061 7320 5b6d 7a75   as well as [mzu
-000011c0: 636b 6572 2773 5d28 6874 7470 733a 2f2f  cker's](https://
-000011d0: 6769 7468 7562 2e63 6f6d 2f6d 7a75 636b  github.com/mzuck
-000011e0: 6572 2f6e 6f74 6573 6872 696e 6b29 2069  er/noteshrink) i
-000011f0: 6e69 7469 616c 2070 726f 6772 616d 2e0a  nitial program..
-00001200: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
-00001210: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-00001220: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00001230: 4d49 5420 4c69 6365 6e73 652e 2053 6565  MIT License. See
-00001240: 2074 6865 2060 4c49 4345 4e53 4560 2066   the `LICENSE` f
-00001250: 696c 6520 666f 7220 6465 7461 696c 732e  ile for details.
-00001260: 0a                                       .
+00000460: 6572 696e 672c 206d 6f72 7068 6f6c 6f67  ering, morpholog
+00000470: 6963 616c 206f 7065 6e69 6e67 2061 6e64  ical opening and
+00000480: 2075 6e73 6861 7270 206d 6173 6b69 6e67   unsharp masking
+00000490: 2074 6f20 7265 6475 6365 206e 6f69 7365   to reduce noise
+000004a0: 2061 6e64 2069 6d70 726f 7665 2069 6d61   and improve ima
+000004b0: 6765 2071 7561 6c69 7479 2e0a 2a20 2a2a  ge quality..* **
+000004c0: 5061 7261 6c6c 656c 2070 726f 6365 7373  Parallel process
+000004d0: 696e 673a 2a2a 2055 7469 6c69 7a65 7320  ing:** Utilizes 
+000004e0: 6d75 6c74 6970 6c65 2043 5055 2063 6f72  multiple CPU cor
+000004f0: 6573 2066 6f72 2066 6173 7465 7220 7072  es for faster pr
+00000500: 6f63 6573 7369 6e67 206f 6620 6d75 6c74  ocessing of mult
+00000510: 6970 6c65 2069 6d61 6765 732e 0a0a 2323  iple images...##
+00000520: 2045 7861 6d70 6c65 730a 0a23 2323 2047   Examples..### G
+00000530: 656e 6572 6963 2045 7861 6d70 6c65 0a0a  eneric Example..
+00000540: 3c74 6162 6c65 3e0a 2020 3c74 723e 0a20  <table>.  <tr>. 
+00000550: 2020 203c 7464 2077 6964 7468 3d22 3530     <td width="50
+00000560: 2522 3e3c 696d 6720 7372 633d 2265 7861  %"><img src="exa
+00000570: 6d70 6c65 732f 6578 616d 706c 655f 312d  mples/example_1-
+00000580: 6f72 6967 2e6a 7067 2220 616c 743d 224f  orig.jpg" alt="O
+00000590: 7269 6769 6e61 6c20 496d 6167 6522 2077  riginal Image" w
+000005a0: 6964 7468 3d22 3430 3022 2068 6569 6768  idth="400" heigh
+000005b0: 743d 2235 3730 222f 3e3c 2f74 643e 0a20  t="570"/></td>. 
+000005c0: 2020 203c 7464 2077 6964 7468 3d22 3530     <td width="50
+000005d0: 2522 3e3c 696d 6720 7372 633d 2265 7861  %"><img src="exa
+000005e0: 6d70 6c65 732f 6578 616d 706c 655f 312d  mples/example_1-
+000005f0: 6e73 2e6a 7067 2220 616c 743d 2250 726f  ns.jpg" alt="Pro
+00000600: 6365 7373 6564 2049 6d61 6765 2220 7769  cessed Image" wi
+00000610: 6474 683d 2234 3030 2220 6865 6967 6874  dth="400" height
+00000620: 3d22 3537 3022 2f3e 3c2f 7464 3e0a 2020  ="570"/></td>.  
+00000630: 3c2f 7472 3e0a 2020 3c74 723e 0a20 2020  </tr>.  <tr>.   
+00000640: 203c 7464 3e4f 7269 6769 6e61 6c20 496d   <td>Original Im
+00000650: 6167 653c 2f74 643e 0a20 2020 203c 7464  age</td>.    <td
+00000660: 3e3c 636f 6465 3e6e 6f74 6573 6872 756e  ><code>noteshrun
+00000670: 6b20 2d77 202d 7320 2d2d 756e 7368 6172  k -w -s --unshar
+00000680: 705f 6d61 736b 202d 7572 2032 202d 7561  p_mask -ur 2 -ua
+00000690: 2031 3c2f 636f 6465 3e3c 2f74 643e 0a20   1</code></td>. 
+000006a0: 203c 2f74 723e 0a3c 2f74 6162 6c65 3e0a   </tr>.</table>.
+000006b0: 0a49 6d61 6765 2053 6f75 7263 653a 2068  .Image Source: h
+000006c0: 7474 7073 3a2f 2f63 6f6d 6d6f 6e73 2e77  ttps://commons.w
+000006d0: 696b 696d 6564 6961 2e6f 7267 2f77 696b  ikimedia.org/wik
+000006e0: 692f 4669 6c65 3a42 5245 414b 4641 5354  i/File:BREAKFAST
+000006f0: 5f28 6865 6c64 5f62 7929 5f4e 4950 504f  _(held_by)_NIPPO
+00000700: 4e5f 5955 5345 4e5f 4b41 4953 4841 5f2d  N_YUSEN_KAISHA_-
+00000710: 5f53 2e53 2e4b 4f42 455f 4d41 5255 5f28  _S.S.KOBE_MARU_(
+00000720: 6174 295f 454e 5f52 4f55 5445 5f28 5353  at)_EN_ROUTE_(SS
+00000730: 295f 284e 5950 4c5f 4861 6465 732d 3237  )_(NYPL_Hades-27
+00000740: 3438 3333 2d34 3639 3130 3829 2e6a 7067  4833-469108).jpg
+00000750: 0a0a 2323 2320 4669 6e65 202f 204c 6f77  ..### Fine / Low
+00000760: 2052 6573 6f6c 7574 696f 6e20 5465 7874   Resolution Text
+00000770: 0a0a 4d6f 7270 686f 6c6f 6769 6361 6c20  ..Morphological 
+00000780: 4f70 656e 696e 6720 7377 616c 6c6f 7773  Opening swallows
+00000790: 2066 696e 6520 7374 7275 6374 7572 6573   fine structures
+000007a0: 2c20 6275 7420 756e 7368 6172 7020 6d61  , but unsharp ma
+000007b0: 736b 696e 6720 6865 6c70 7320 7072 6573  sking helps pres
+000007c0: 6572 7665 2074 6865 6d2e 0a0a 3c74 6162  erve them...<tab
+000007d0: 6c65 3e0a 2020 3c74 723e 0a20 2020 203c  le>.  <tr>.    <
+000007e0: 7464 3e3c 696d 6720 7372 633d 2265 7861  td><img src="exa
+000007f0: 6d70 6c65 732f 6578 616d 706c 655f 322d  mples/example_2-
+00000800: 6f72 6967 2e6a 7067 2220 616c 743d 224f  orig.jpg" alt="O
+00000810: 7269 6769 6e61 6c20 496d 6167 6522 2077  riginal Image" w
+00000820: 6964 7468 3d22 3937 3022 2068 6569 6768  idth="970" heigh
+00000830: 743d 2232 3137 222f 3e3c 2f74 643e 0a20  t="217"/></td>. 
+00000840: 203c 2f74 723e 0a20 203c 7472 3e0a 2020   </tr>.  <tr>.  
+00000850: 2020 3c74 643e 3c63 6f64 653e 4f72 6967    <td><code>Orig
+00000860: 696e 616c 2049 6d61 6765 2028 6f77 6e29  inal Image (own)
+00000870: 3c2f 636f 6465 3e3c 2f74 643e 0a20 203c  </code></td>.  <
+00000880: 2f74 723e 0a20 203c 7472 3e0a 2020 2020  /tr>.  <tr>.    
+00000890: 3c74 643e 3c69 6d67 2073 7263 3d22 6578  <td><img src="ex
+000008a0: 616d 706c 6573 2f65 7861 6d70 6c65 5f32  amples/example_2
+000008b0: 2d6f 7065 6e69 6e67 2e6a 7067 2220 616c  -opening.jpg" al
+000008c0: 743d 224d 6f72 7068 6f6c 6f67 6963 616c  t="Morphological
+000008d0: 204f 7065 6e69 6e67 2220 7769 6474 683d   Opening" width=
+000008e0: 2239 3730 2220 6865 6967 6874 3d22 3231  "970" height="21
+000008f0: 3722 2f3e 3c2f 7464 3e0a 2020 3c2f 7472  7"/></td>.  </tr
+00000900: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00000910: 3e3c 636f 6465 3e6e 6f74 6573 6872 756e  ><code>noteshrun
+00000920: 6b20 2d77 202d 2d64 656e 6f69 7365 5f6f  k -w --denoise_o
+00000930: 7065 6e69 6e67 202d 6f73 202e 393c 2f63  pening -os .9</c
+00000940: 6f64 653e 3c2f 7464 3e0a 2020 3c2f 7472  ode></td>.  </tr
+00000950: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00000960: 3e3c 696d 6720 7372 633d 2265 7861 6d70  ><img src="examp
+00000970: 6c65 732f 6578 616d 706c 655f 322d 756e  les/example_2-un
+00000980: 7368 6172 702e 6a70 6722 2061 6c74 3d22  sharp.jpg" alt="
+00000990: 556e 7368 6172 7020 4d61 736b 696e 6722  Unsharp Masking"
+000009a0: 2077 6964 7468 3d22 3937 3022 2068 6569   width="970" hei
+000009b0: 6768 743d 2232 3137 222f 3e3c 2f74 643e  ght="217"/></td>
+000009c0: 0a20 203c 2f74 723e 0a20 203c 7472 3e0a  .  </tr>.  <tr>.
+000009d0: 2020 2020 3c74 643e 3c63 6f64 653e 6e6f      <td><code>no
+000009e0: 7465 7368 7275 6e6b 202d 7720 2d2d 756e  teshrunk -w --un
+000009f0: 7368 6172 705f 6d61 736b 203c 2f63 6f64  sharp_mask </cod
+00000a00: 653e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  e></td>.  </tr>.
+00000a10: 3c2f 7461 626c 653e 0a0a 2323 2320 4164  </table>..### Ad
+00000a20: 7661 6e63 6564 2045 7861 6d70 6c65 0a0a  vanced Example..
+00000a30: 3c74 6162 6c65 3e0a 2020 3c74 723e 0a20  <table>.  <tr>. 
+00000a40: 2020 203c 7464 2077 6964 7468 3d22 3530     <td width="50
+00000a50: 2522 3e3c 696d 6720 7372 633d 2265 7861  %"><img src="exa
+00000a60: 6d70 6c65 732f 6578 616d 706c 655f 332d  mples/example_3-
+00000a70: 6f72 6967 2e6a 7067 2220 616c 743d 224f  orig.jpg" alt="O
+00000a80: 7269 6769 6e61 6c20 496d 6167 6522 2077  riginal Image" w
+00000a90: 6964 7468 3d22 3430 3022 2068 6569 6768  idth="400" heigh
+00000aa0: 743d 2234 3836 222f 3e3c 2f74 643e 0a20  t="486"/></td>. 
+00000ab0: 2020 203c 7464 2077 6964 7468 3d22 3530     <td width="50
+00000ac0: 2522 3e3c 696d 6720 7372 633d 2265 7861  %"><img src="exa
+00000ad0: 6d70 6c65 732f 6578 616d 706c 655f 332d  mples/example_3-
+00000ae0: 6164 7661 6e63 6564 2e6a 7067 2220 616c  advanced.jpg" al
+00000af0: 743d 2250 726f 6365 7373 6564 2049 6d61  t="Processed Ima
+00000b00: 6765 2220 7769 6474 683d 2234 3030 2220  ge" width="400" 
+00000b10: 6865 6967 6874 3d22 3438 3622 2f3e 3c2f  height="486"/></
+00000b20: 7464 3e0a 2020 3c2f 7472 3e0a 2020 3c74  td>.  </tr>.  <t
+00000b30: 723e 0a20 2020 203c 7464 3e4f 7269 6769  r>.    <td>Origi
+00000b40: 6e61 6c20 496d 6167 653c 2f74 643e 0a20  nal Image</td>. 
+00000b50: 2020 203c 7464 3e3c 636f 6465 3e6e 6f74     <td><code>not
+00000b60: 6573 6872 756e 6b20 2d77 202d 7320 2d74  eshrunk -w -s -t
+00000b70: 7620 3330 202d 2d64 656e 6f69 7365 5f6f  v 30 --denoise_o
+00000b80: 7065 6e69 6e67 202d 6f73 2031 2e36 202d  pening -os 1.6 -
+00000b90: 6e20 3620 2d70 2031 3030 2065 7861 6d70  n 6 -p 100 examp
+00000ba0: 6c65 5f33 2d6f 7269 672e 6a70 673c 2f63  le_3-orig.jpg</c
+00000bb0: 6f64 653e 3c2f 7464 3e0a 2020 3c2f 7472  ode></td>.  </tr
+00000bc0: 3e0a 3c2f 7461 626c 653e 0a0a 496d 6167  >.</table>..Imag
+00000bd0: 6520 536f 7572 6365 3a20 6874 7470 733a  e Source: https:
+00000be0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7a75  //github.com/mzu
+00000bf0: 636b 6572 2f6e 6f74 6573 6872 696e 6b2f  cker/noteshrink/
+00000c00: 626c 6f62 2f6d 6173 7465 722f 6578 616d  blob/master/exam
+00000c10: 706c 6573 2f6e 6f74 6573 4131 2e6a 7067  ples/notesA1.jpg
+00000c20: 0a0a 2323 2320 4675 7274 6865 7220 4578  ..### Further Ex
+00000c30: 616d 706c 6573 0a0a 312e 2020 436f 6d70  amples..1.  Comp
+00000c40: 7265 7373 2061 2073 696e 676c 6520 696d  ress a single im
+00000c50: 6167 6520 7769 7468 2064 6566 6175 6c74  age with default
+00000c60: 2073 6574 7469 6e67 733a 0a0a 2020 2020   settings:..    
+00000c70: 6060 6062 6173 680a 2020 2020 6e6f 7465  ```bash.    note
+00000c80: 7368 7275 6e6b 2069 6e70 7574 2e70 6e67  shrunk input.png
+00000c90: 0a20 2020 2060 6060 0a0a 322e 2020 436f  .    ```..2.  Co
+00000ca0: 6d70 7265 7373 206d 756c 7469 706c 6520  mpress multiple 
+00000cb0: 696d 6167 6573 2077 6974 6820 6120 7768  images with a wh
+00000cc0: 6974 6520 6261 636b 6772 6f75 6e64 2061  ite background a
+00000cd0: 6e64 2031 3620 636f 6c6f 7273 3a0a 0a20  nd 16 colors:.. 
+00000ce0: 2020 2060 6060 6261 7368 0a20 2020 206e     ```bash.    n
+00000cf0: 6f74 6573 6872 756e 6b20 2d77 202d 6e20  oteshrunk -w -n 
+00000d00: 3136 2069 6d61 6765 312e 6a70 6720 696d  16 image1.jpg im
+00000d10: 6167 6532 2e70 6e67 0a20 2020 2060 6060  age2.png.    ```
+00000d20: 0a0a 332e 2020 436f 6d70 7265 7373 2069  ..3.  Compress i
+00000d30: 6d61 6765 7320 7573 696e 6720 6120 6c6f  mages using a lo
+00000d40: 6361 6c20 636f 6c6f 7220 7061 6c65 7474  cal color palett
+00000d50: 6520 616e 6420 6b65 6570 2069 6e74 6572  e and keep inter
+00000d60: 6d65 6469 6174 6520 6669 6c65 7320 7768  mediate files wh
+00000d70: 696c 6520 6469 7361 626c 696e 6720 6d75  ile disabling mu
+00000d80: 6c74 692d 7468 7265 6164 696e 673a 0a20  lti-threading:. 
+00000d90: 2020 2060 6060 6261 7368 0a20 2020 206e     ```bash.    n
+00000da0: 6f74 6573 6872 756e 6b20 2d6c 202d 6a20  oteshrunk -l -j 
+00000db0: 3120 2d6b 202a 2e6a 7067 0a20 2020 2060  1 -k *.jpg.    `
+00000dc0: 6060 0a0a 2323 2052 6571 7569 7265 6d65  ``..## Requireme
+00000dd0: 6e74 730a 0a23 2323 2050 7974 686f 6e20  nts..### Python 
+00000de0: 5061 636b 6167 6573 0a0a 2d20 6172 6763  Packages..- argc
+00000df0: 6f6d 706c 6574 650a 2d20 4e75 6d50 790a  omplete.- NumPy.
+00000e00: 2d20 5069 6c6c 6f77 2028 5049 4c20 466f  - Pillow (PIL Fo
+00000e10: 726b 290a 2d20 5079 7468 6f6e 2033 0a2d  rk).- Python 3.-
+00000e20: 2073 6369 6b69 742d 696d 6167 650a 2d20   scikit-image.- 
+00000e30: 7363 696b 6974 2d6c 6561 726e 0a2d 2053  scikit-learn.- S
+00000e40: 6369 5079 0a0a 2323 2320 4f74 6865 720a  ciPy..### Other.
+00000e50: 0a2d 2047 686f 7374 7363 7269 7074 2028  .- Ghostscript (
+00000e60: 6578 6563 7574 6162 6c65 2060 6773 6020  executable `gs` 
+00000e70: 696e 2050 4154 4820 2d20 666f 7220 5044  in PATH - for PD
+00000e80: 4620 6d65 7267 696e 6729 0a0a 2323 2049  F merging)..## I
+00000e90: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
+00000ea0: 6261 7368 0a70 6970 7820 696e 7374 616c  bash.pipx instal
+00000eb0: 6c20 6e6f 7465 7368 7275 6e6b 0a60 6060  l noteshrunk.```
+00000ec0: 0a0a 2323 2055 7361 6765 0a0a 6060 600a  ..## Usage..```.
+00000ed0: 6e6f 7465 7368 7275 6e6b 205b 2d68 5d20  noteshrunk [-h] 
+00000ee0: 5b2d 6f20 4f55 5450 5554 5d20 5b2d 775d  [-o OUTPUT] [-w]
+00000ef0: 205b 2d73 5d20 5b2d 6e20 4e5f 434f 4c4f   [-s] [-n N_COLO
+00000f00: 5253 5d20 5b2d 6420 4450 495d 205b 2d71  RS] [-d DPI] [-q
+00000f10: 205b 312d 3130 305d 5d20 5b2d 6c5d 0a20   [1-100]] [-l]. 
+00000f20: 2020 2020 2020 2020 2020 5b2d 7020 5045            [-p PE
+00000f30: 5243 454e 5441 4745 5d20 5b2d 6a20 4a4f  RCENTAGE] [-j JO
+00000f40: 4253 5d20 5b2d 795d 0a20 2020 2020 2020  BS] [-y].       
+00000f50: 2020 2020 5b2d 7473 2054 4852 4553 484f      [-ts THRESHO
+00000f60: 4c44 5f53 4154 5552 4154 494f 4e5d 205b  LD_SATURATION] [
+00000f70: 2d74 7620 5448 5245 5348 4f4c 445f 5641  -tv THRESHOLD_VA
+00000f80: 4c55 455d 0a20 2020 2020 2020 2020 2020  LUE].           
+00000f90: 5b2d 2d64 656e 6f69 7365 5f6d 6564 6961  [--denoise_media
+00000fa0: 6e5d 205b 2d2d 6465 6e6f 6973 655f 6f70  n] [--denoise_op
+00000fb0: 656e 696e 675d 205b 2d2d 756e 7368 6172  ening] [--unshar
+00000fc0: 705f 6d61 736b 5d0a 2020 2020 2020 2020  p_mask].        
+00000fd0: 2020 205b 2d6d 7320 4d45 4449 414e 5f53     [-ms MEDIAN_S
+00000fe0: 5452 454e 4754 485d 205b 2d63 7320 434c  TRENGTH] [-cs CL
+00000ff0: 4f53 494e 475f 5354 5245 4e47 5448 5d20  OSING_STRENGTH] 
+00001000: 5b2d 7561 2055 4e53 4841 5250 5f41 4d4f  [-ua UNSHARP_AMO
+00001010: 554e 545d 205b 2d75 7220 554e 5348 4152  UNT] [-ur UNSHAR
+00001020: 505f 5241 4449 5553 5d0a 2020 2020 2020  P_RADIUS].      
+00001030: 2020 2020 205b 2d6b 5d20 5b2d 765d 205b       [-k] [-v] [
+00001040: 2d2d 7665 7273 696f 6e5d 2066 696c 6573  --version] files
+00001050: 205b 6669 6c65 7320 2e2e 2e5d 0a60 6060   [files ...].```
+00001060: 0a0a 2323 2320 4172 6775 6d65 6e74 730a  ..### Arguments.
+00001070: 0a2a 2060 6669 6c65 7360 3a20 4120 6c69  .* `files`: A li
+00001080: 7374 206f 6620 7061 7468 7320 746f 2074  st of paths to t
+00001090: 6865 2069 6e70 7574 2069 6d61 6765 2066  he input image f
+000010a0: 696c 6573 2e0a 2a20 602d 6f60 2c20 602d  iles..* `-o`, `-
+000010b0: 2d6f 7574 7075 7460 3a20 5061 7468 2074  -output`: Path t
+000010c0: 6f20 7468 6520 6f75 7470 7574 2050 4446  o the output PDF
+000010d0: 2066 696c 6520 2864 6566 6175 6c74 3a20   file (default: 
+000010e0: 606f 7574 7075 742e 7064 6660 292e 0a2a  `output.pdf`)..*
+000010f0: 2060 2d77 602c 2060 2d2d 7768 6974 655f   `-w`, `--white_
+00001100: 6261 636b 6772 6f75 6e64 603a 2055 7365  background`: Use
+00001110: 2077 6869 7465 2062 6163 6b67 726f 756e   white backgroun
+00001120: 6420 696e 7374 6561 6420 6f66 2064 6f6d  d instead of dom
+00001130: 696e 616e 7420 636f 6c6f 722e 0a2a 2060  inant color..* `
+00001140: 2d73 602c 2060 2d2d 7361 7475 7261 7465  -s`, `--saturate
+00001150: 603a 204d 6178 696d 697a 6520 7361 7475  `: Maximize satu
+00001160: 7261 7469 6f6e 2069 6e20 7468 6520 6f75  ration in the ou
+00001170: 7470 7574 2069 6d61 6765 2e0a 2a20 602d  tput image..* `-
+00001180: 6e60 2c20 602d 2d6e 5f63 6f6c 6f72 7360  n`, `--n_colors`
+00001190: 3a20 4e75 6d62 6572 206f 6620 636f 6c6f  : Number of colo
+000011a0: 7273 2069 6e20 7468 6520 7061 6c65 7474  rs in the palett
+000011b0: 6520 2864 6566 6175 6c74 3a20 3829 2e0a  e (default: 8)..
+000011c0: 2a20 602d 6460 2c20 602d 2d64 7069 603a  * `-d`, `--dpi`:
+000011d0: 2044 5049 2076 616c 7565 206f 6620 7468   DPI value of th
+000011e0: 6520 696e 7075 7420 696d 6167 6573 2028  e input images (
+000011f0: 6465 6661 756c 743a 2033 3030 292e 0a2a  default: 300)..*
+00001200: 2060 2d71 602c 2060 2d2d 7175 616c 6974   `-q`, `--qualit
+00001210: 7960 3a20 4a50 4547 2071 7561 6c69 7479  y`: JPEG quality
+00001220: 206f 6620 7468 6520 696d 6167 6573 2065   of the images e
+00001230: 6d62 6564 6465 6420 696e 2074 6865 2050  mbedded in the P
+00001240: 4446 2028 312d 3130 302c 2064 6566 6175  DF (1-100, defau
+00001250: 6c74 3a20 3735 292e 0a2a 2060 2d6c 602c  lt: 75)..* `-l`,
+00001260: 2060 2d2d 6c6f 6361 6c5f 7061 6c65 7474   `--local_palett
+00001270: 6560 3a20 4372 6561 7465 2061 6e20 696e  e`: Create an in
+00001280: 6469 7669 6475 616c 2063 6f6c 6f72 2070  dividual color p
+00001290: 616c 6574 7465 2066 6f72 2065 6163 6820  alette for each 
+000012a0: 696d 6167 6520 2862 7920 7361 6d70 6c69  image (by sampli
+000012b0: 6e67 2061 202d 7020 7065 7263 656e 7461  ng a -p percenta
+000012c0: 6765 206f 6620 7468 6520 7069 7865 6c73  ge of the pixels
+000012d0: 206f 6620 7468 6174 2069 6d61 6765 2920   of that image) 
+000012e0: 696e 7374 6561 6420 6f66 2061 2067 6c6f  instead of a glo
+000012f0: 6261 6c20 7061 6c65 7474 6520 2862 7920  bal palette (by 
+00001300: 7361 6d70 6c69 6e67 2061 202d 7020 7065  sampling a -p pe
+00001310: 7263 656e 7461 6765 206f 6620 7468 6520  rcentage of the 
+00001320: 7069 7865 6c73 206f 6620 6561 6368 2069  pixels of each i
+00001330: 6e70 7574 2069 6d61 6765 292e 0a2a 2060  nput image)..* `
+00001340: 2d70 602c 2060 2d2d 7065 7263 656e 7461  -p`, `--percenta
+00001350: 6765 603a 2050 6572 6365 6e74 6167 6520  ge`: Percentage 
+00001360: 6f66 2070 6978 656c 7320 746f 2073 616d  of pixels to sam
+00001370: 706c 6520 6672 6f6d 2065 6163 6820 696e  ple from each in
+00001380: 7075 7420 696d 6167 6520 666f 7220 636f  put image for co
+00001390: 6c6f 7220 7061 6c65 7474 6520 6372 6561  lor palette crea
+000013a0: 7469 6f6e 2028 6465 6661 756c 743a 2031  tion (default: 1
+000013b0: 3029 2e0a 2a20 602d 6a60 2c20 602d 2d6a  0)..* `-j`, `--j
+000013c0: 6f62 7360 3a20 4e75 6d62 6572 206f 6620  obs`: Number of 
+000013d0: 7468 7265 6164 7320 746f 2075 7365 2066  threads to use f
+000013e0: 6f72 206d 756c 7469 2d74 6872 6561 6469  or multi-threadi
+000013f0: 6e67 2028 6465 6661 756c 743a 206e 756d  ng (default: num
+00001400: 6265 7220 6f66 2043 5055 2063 6f72 6573  ber of CPU cores
+00001410: 292e 0a2a 2060 2d79 602c 2060 2d2d 6f76  )..* `-y`, `--ov
+00001420: 6572 7772 6974 6560 3a20 4f76 6572 7772  erwrite`: Overwr
+00001430: 6974 6520 6578 6973 7469 6e67 2066 696c  ite existing fil
+00001440: 6573 2077 6974 686f 7574 2061 736b 696e  es without askin
+00001450: 672e 0a2a 2060 2d74 7360 2c20 602d 2d74  g..* `-ts`, `--t
+00001460: 6872 6573 686f 6c64 5f73 6174 7572 6174  hreshold_saturat
+00001470: 696f 6e60 3a20 4853 5620 7361 7475 7261  ion`: HSV satura
+00001480: 7469 6f6e 2074 6872 6573 686f 6c64 2028  tion threshold (
+00001490: 696e 2070 6572 6365 6e74 2920 7573 6564  in percent) used
+000014a0: 2066 6f72 2062 6163 6b67 726f 756e 6420   for background 
+000014b0: 6465 7465 6374 696f 6e20 2864 6566 6175  detection (defau
+000014c0: 6c74 3a20 3135 292e 0a2a 2060 2d74 7660  lt: 15)..* `-tv`
+000014d0: 2c20 602d 2d74 6872 6573 686f 6c64 5f76  , `--threshold_v
+000014e0: 616c 7565 603a 2048 5356 2076 616c 7565  alue`: HSV value
+000014f0: 2074 6872 6573 686f 6c64 2028 696e 2070   threshold (in p
+00001500: 6572 6365 6e74 2920 7573 6564 2066 6f72  ercent) used for
+00001510: 2062 6163 6b67 726f 756e 6420 6465 7465   background dete
+00001520: 6374 696f 6e20 2864 6566 6175 6c74 3a20  ction (default: 
+00001530: 3235 292e 0a2a 2060 2d2d 6465 6e6f 6973  25)..* `--denois
+00001540: 655f 6d65 6469 616e 603a 2041 7070 6c79  e_median`: Apply
+00001550: 206d 6564 6961 6e20 6465 6e6f 6973 696e   median denoisin
+00001560: 6720 6f6e 2074 6865 206f 7574 7075 7420  g on the output 
+00001570: 696d 6167 6520 7769 7468 2073 7472 656e  image with stren
+00001580: 6774 6820 602d 6d73 602e 0a2a 2060 2d6d  gth `-ms`..* `-m
+00001590: 7360 2c20 602d 2d6d 6564 6961 6e5f 7374  s`, `--median_st
+000015a0: 7265 6e67 7468 603a 2053 7472 656e 6774  rength`: Strengt
+000015b0: 6820 6f66 206d 6564 6961 6e20 6669 6c74  h of median filt
+000015c0: 6572 696e 6720 2864 6566 6175 6c74 3a20  ering (default: 
+000015d0: 3329 2e0a 2a20 602d 2d64 656e 6f69 7365  3)..* `--denoise
+000015e0: 5f6f 7065 6e69 6e67 603a 2041 7070 6c79  _opening`: Apply
+000015f0: 206d 6f72 7068 6f6c 6f67 6963 616c 206f   morphological o
+00001600: 7065 6e69 6e67 206f 6e20 7468 6520 6261  pening on the ba
+00001610: 636b 6772 6f75 6e64 206d 6173 6b20 7769  ckground mask wi
+00001620: 7468 2073 7472 656e 6774 6820 602d 6f73  th strength `-os
+00001630: 602e 0a2a 2060 2d6f 7360 2c20 602d 2d6f  `..* `-os`, `--o
+00001640: 7065 6e69 6e67 5f73 7472 656e 6774 6860  pening_strength`
+00001650: 3a20 5374 7265 6e67 7468 206f 6620 6f70  : Strength of op
+00001660: 656e 696e 6720 6669 6c74 6572 696e 6720  ening filtering 
+00001670: 2f20 7261 6469 7573 206f 6620 7468 6520  / radius of the 
+00001680: 7374 7275 6374 7572 696e 6720 656c 656d  structuring elem
+00001690: 656e 7420 2864 6973 6b2c 2064 6566 6175  ent (disk, defau
+000016a0: 6c74 3a20 3329 2e0a 2a20 602d 2d75 6e73  lt: 3)..* `--uns
+000016b0: 6861 7270 5f6d 6173 6b60 3a20 4170 706c  harp_mask`: Appl
+000016c0: 7920 756e 7368 6172 7020 6d61 736b 696e  y unsharp maskin
+000016d0: 6720 6f6e 2074 6865 2066 696e 616c 2069  g on the final i
+000016e0: 6d61 6765 2077 6974 6820 7261 6469 7573  mage with radius
+000016f0: 2060 2d75 7260 2061 6e64 2061 6d6f 756e   `-ur` and amoun
+00001700: 7420 602d 7561 602e 0a2a 2060 2d75 7260  t `-ua`..* `-ur`
+00001710: 2c20 602d 7561 603a 2052 6164 6975 7320  , `-ua`: Radius 
+00001720: 616e 6420 416d 6f75 6e74 2075 7365 6420  and Amount used 
+00001730: 666f 7220 756e 7368 6172 7020 6d61 736b  for unsharp mask
+00001740: 696e 672e 0a2a 2060 2d6b 602c 2060 2d2d  ing..* `-k`, `--
+00001750: 6b65 6570 5f69 6e74 6572 6d65 6469 6174  keep_intermediat
+00001760: 6560 3a20 4b65 6570 2074 6865 2069 6e74  e`: Keep the int
+00001770: 6572 6d65 6469 6174 6520 7369 6e67 6c65  ermediate single
+00001780: 2d70 6167 6520 5044 4673 2e0a 2a20 602d  -page PDFs..* `-
+00001790: 7660 2c20 602d 2d76 6572 626f 7365 603a  v`, `--verbose`:
+000017a0: 2056 6572 626f 7365 206f 7574 7075 742e   Verbose output.
+000017b0: 0a2a 2060 2d2d 7665 7273 696f 6e60 3a20  .* `--version`: 
+000017c0: 5368 6f77 2070 726f 6772 616d 2076 6572  Show program ver
+000017d0: 7369 6f6e 2061 6e64 2065 7869 742e 0a0a  sion and exit...
+000017e0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+000017f0: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
+00001800: 7265 2077 656c 636f 6d65 2120 506c 6561  re welcome! Plea
+00001810: 7365 2066 6565 6c20 6672 6565 2074 6f20  se feel free to 
+00001820: 7375 626d 6974 2069 7373 7565 7320 6f72  submit issues or
+00001830: 2070 756c 6c20 7265 7175 6573 7473 206f   pull requests o
+00001840: 6e20 7468 6520 4769 7448 7562 2072 6570  n the GitHub rep
+00001850: 6f73 6974 6f72 792e 0a0a 2323 2041 636b  ository...## Ack
+00001860: 6e6f 776c 6564 6765 6d65 6e74 730a 0a54  nowledgements..T
+00001870: 6869 7320 7072 6f6a 6563 7420 7574 696c  his project util
+00001880: 697a 6573 206f 7065 6e2d 736f 7572 6365  izes open-source
+00001890: 2073 6f66 7477 6172 6520 6672 6f6d 2074   software from t
+000018a0: 6865 2050 7974 686f 6e20 636f 6d6d 756e  he Python commun
+000018b0: 6974 792e 0a53 7065 6369 616c 2074 6861  ity..Special tha
+000018c0: 6e6b 7320 746f 2074 6865 2064 6576 656c  nks to the devel
+000018d0: 6f70 6572 7320 616e 6420 6d61 696e 7461  opers and mainta
+000018e0: 696e 6572 7320 6f66 2074 6865 2072 6571  iners of the req
+000018f0: 7569 7265 6420 6c69 6272 6172 6965 7320  uired libraries 
+00001900: 6173 2077 656c 6c20 6173 205b 6d7a 7563  as well as [mzuc
+00001910: 6b65 7227 735d 2868 7474 7073 3a2f 2f67  ker's](https://g
+00001920: 6974 6875 622e 636f 6d2f 6d7a 7563 6b65  ithub.com/mzucke
+00001930: 722f 6e6f 7465 7368 7269 6e6b 2920 696e  r/noteshrink) in
+00001940: 6974 6961 6c20 7072 6f67 7261 6d2e 0a0a  itial program...
+00001950: 2323 204c 6963 656e 7365 0a0a 5468 6973  ## License..This
+00001960: 2070 726f 6a65 6374 2069 7320 6c69 6365   project is lice
+00001970: 6e73 6564 2075 6e64 6572 2074 6865 204d  nsed under the M
+00001980: 4954 204c 6963 656e 7365 2e20 5365 6520  IT License. See 
+00001990: 7468 6520 604c 4943 454e 5345 6020 6669  the `LICENSE` fi
+000019a0: 6c65 2066 6f72 2064 6574 6169 6c73 2e0a  le for details..
```

### Comparing `noteshrunk-1.3.0/PKG-INFO` & `noteshrunk-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.3.0
+Version: 1.4.0
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -703,17 +703,93 @@
 
 ## Features
 
 * **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes.
 * **Background Detection and Removal:** Identifies and removes the background color.
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
 * **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
-* **Denoising Options:** Provides median filtering and morphological operations to reduce noise and improve image quality.
+* **Denoising Options:** Provides median filtering, morphological opening and unsharp masking to reduce noise and improve image quality.
 * **Parallel processing:** Utilizes multiple CPU cores for faster processing of multiple images.
 
+## Examples
+
+### Generic Example
+
+<table>
+  <tr>
+    <td width="50%"><img src="examples/example_1-orig.jpg" alt="Original Image" width="400" height="570"/></td>
+    <td width="50%"><img src="examples/example_1-ns.jpg" alt="Processed Image" width="400" height="570"/></td>
+  </tr>
+  <tr>
+    <td>Original Image</td>
+    <td><code>noteshrunk -w -s --unsharp_mask -ur 2 -ua 1</code></td>
+  </tr>
+</table>
+
+Image Source: https://commons.wikimedia.org/wiki/File:BREAKFAST_(held_by)_NIPPON_YUSEN_KAISHA_-_S.S.KOBE_MARU_(at)_EN_ROUTE_(SS)_(NYPL_Hades-274833-469108).jpg
+
+### Fine / Low Resolution Text
+
+Morphological Opening swallows fine structures, but unsharp masking helps preserve them.
+
+<table>
+  <tr>
+    <td><img src="examples/example_2-orig.jpg" alt="Original Image" width="970" height="217"/></td>
+  </tr>
+  <tr>
+    <td><code>Original Image (own)</code></td>
+  </tr>
+  <tr>
+    <td><img src="examples/example_2-opening.jpg" alt="Morphological Opening" width="970" height="217"/></td>
+  </tr>
+  <tr>
+    <td><code>noteshrunk -w --denoise_opening -os .9</code></td>
+  </tr>
+  <tr>
+    <td><img src="examples/example_2-unsharp.jpg" alt="Unsharp Masking" width="970" height="217"/></td>
+  </tr>
+  <tr>
+    <td><code>noteshrunk -w --unsharp_mask </code></td>
+  </tr>
+</table>
+
+### Advanced Example
+
+<table>
+  <tr>
+    <td width="50%"><img src="examples/example_3-orig.jpg" alt="Original Image" width="400" height="486"/></td>
+    <td width="50%"><img src="examples/example_3-advanced.jpg" alt="Processed Image" width="400" height="486"/></td>
+  </tr>
+  <tr>
+    <td>Original Image</td>
+    <td><code>noteshrunk -w -s -tv 30 --denoise_opening -os 1.6 -n 6 -p 100 example_3-orig.jpg</code></td>
+  </tr>
+</table>
+
+Image Source: https://github.com/mzucker/noteshrink/blob/master/examples/notesA1.jpg
+
+### Further Examples
+
+1.  Compress a single image with default settings:
+
+    ```bash
+    noteshrunk input.png
+    ```
+
+2.  Compress multiple images with a white background and 16 colors:
+
+    ```bash
+    noteshrunk -w -n 16 image1.jpg image2.png
+    ```
+
+3.  Compress images using a local color palette and keep intermediate files while disabling multi-threading:
+    ```bash
+    noteshrunk -l -j 1 -k *.jpg
+    ```
+
 ## Requirements
 
 ### Python Packages
 
 - argcomplete
 - NumPy
 - Pillow (PIL Fork)
@@ -732,17 +808,18 @@
 pipx install noteshrunk
 ```
 
 ## Usage
 
 ```
 noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]] [-l]
-           [-p PERCENTAGE] [-j JOBS] [-y] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
-           [--denoise_median] [--denoise_closing] [--denoise_opening]
-           [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-os OPENING_STRENGTH]
+           [-p PERCENTAGE] [-j JOBS] [-y]
+           [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
+           [--denoise_median] [--denoise_opening] [--unsharp_mask]
+           [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-ua UNSHARP_AMOUNT] [-ur UNSHARP_RADIUS]
            [-k] [-v] [--version] files [files ...]
 ```
 
 ### Arguments
 
 * `files`: A list of paths to the input image files.
 * `-o`, `--output`: Path to the output PDF file (default: `output.pdf`).
@@ -753,43 +830,24 @@
 * `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-100, default: 75).
 * `-l`, `--local_palette`: Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).
 * `-p`, `--percentage`: Percentage of pixels to sample from each input image for color palette creation (default: 10).
 * `-j`, `--jobs`: Number of threads to use for multi-threading (default: number of CPU cores).
 * `-y`, `--overwrite`: Overwrite existing files without asking.
 * `-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for background detection (default: 15).
 * `-tv`, `--threshold_value`: HSV value threshold (in percent) used for background detection (default: 25).
-* `--denoise_median`: Apply median denoising.
-* `--denoise_closing`: Apply morphological closing on the background mask.
-* `--denoise_opening`: Apply morphological opening on the background mask.
+* `--denoise_median`: Apply median denoising on the output image with strength `-ms`.
 * `-ms`, `--median_strength`: Strength of median filtering (default: 3).
-* `-cs`, `--closing_strength`: Strength of closing filtering / radius of the structuring element (disk, default: 3).
+* `--denoise_opening`: Apply morphological opening on the background mask with strength `-os`.
 * `-os`, `--opening_strength`: Strength of opening filtering / radius of the structuring element (disk, default: 3).
+* `--unsharp_mask`: Apply unsharp masking on the final image with radius `-ur` and amount `-ua`.
+* `-ur`, `-ua`: Radius and Amount used for unsharp masking.
 * `-k`, `--keep_intermediate`: Keep the intermediate single-page PDFs.
 * `-v`, `--verbose`: Verbose output.
 * `--version`: Show program version and exit.
 
-## Examples
-
-1.  Compress a single image with default settings:
-
-    ```bash
-    noteshrunk input.png
-    ```
-
-2.  Compress multiple images with a white background and 16 colors:
-
-    ```bash
-    noteshrunk -w -n 16 image1.jpg image2.png
-    ```
-
-3.  Compress images using a local color palette and keep intermediate files while disabling multi-threading:
-    ```bash
-    noteshrunk -l -j 1 -k *.jpg
-    ```
-
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues or pull requests on the GitHub repository.
 
 ## Acknowledgements
 
 This project utilizes open-source software from the Python community.
```

