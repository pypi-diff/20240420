# Comparing `tmp/HyperRez-1.0.0.tar.gz` & `tmp/HyperRez-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyperRez-1.0.0.tar", last modified: Sun Feb 11 08:24:06 2024, max compression
+gzip compressed data, was "HyperRez-2.0.tar", last modified: Sat Apr 13 19:34:44 2024, max compression
```

## Comparing `HyperRez-1.0.0.tar` & `HyperRez-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 08:24:06.258330 HyperRez-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-02-11 08:24:06.204930 HyperRez-1.0.0/HyperRez/
--rw-rw-rw-   0        0        0     2206 2024-02-11 08:15:55.000000 HyperRez-1.0.0/HyperRez/__init__.py
--rw-rw-rw-   0        0        0     8024 2024-02-11 08:15:55.000000 HyperRez-1.0.0/HyperRez/inference_realesrgan.py
-drwxrwxrwx   0        0        0        0 2024-02-11 08:24:06.251404 HyperRez-1.0.0/HyperRez.egg-info/
--rw-rw-rw-   0        0        0     2402 2024-02-11 08:24:05.000000 HyperRez-1.0.0/HyperRez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-02-11 08:24:06.000000 HyperRez-1.0.0/HyperRez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 08:24:05.000000 HyperRez-1.0.0/HyperRez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-11 08:24:05.000000 HyperRez-1.0.0/HyperRez.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      118 2024-02-11 08:24:05.000000 HyperRez-1.0.0/HyperRez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-11 08:24:05.000000 HyperRez-1.0.0/HyperRez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-02-11 08:15:55.000000 HyperRez-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2402 2024-02-11 08:24:06.254215 HyperRez-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2024-02-11 08:15:55.000000 HyperRez-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-11 08:24:06.259313 HyperRez-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2193 2024-02-11 08:23:20.000000 HyperRez-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 19:34:44.758745 HyperRez-2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 19:34:44.756744 HyperRez-2.0/HyperRez/
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-13 19:34:04.000000 HyperRez-2.0/HyperRez/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7857 2024-04-13 19:34:04.000000 HyperRez-2.0/HyperRez/inference_realesrgan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 19:34:44.757745 HyperRez-2.0/HyperRez.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 19:34:44.000000 HyperRez-2.0/HyperRez.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-13 19:34:04.000000 HyperRez-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-13 19:34:44.757745 HyperRez-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-13 19:34:04.000000 HyperRez-2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 19:34:44.758745 HyperRez-2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-04-13 19:34:41.000000 HyperRez-2.0/setup.py
```

### Comparing `HyperRez-1.0.0/HyperRez/__init__.py` & `HyperRez-2.0/HyperRez/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import shutil
-import os
-import gradio as gr
-import cv2
-import math
-
-class ImageUpscaler:
-
-  def __init__(self):
-    pass
-
-  def upscale(self, image, scale_factor, model_version, _):
-    try:
-      shutil.rmtree("inputs")
-      shutil.rmtree("results")
-    except:
-      pass
-    os.mkdir("inputs")
-    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-    cv2.imwrite("inputs/image.jpg", image)
-    os.system(f"python -m HyperRez.inference_realesrgan -n RealESRGAN_x4plus -i inputs -o results --outscale {scale_factor} --face_enhance --face_enhance_model {model_version}")
-    filename = os.listdir("results")[0]
-    file_path = os.path.join("results", filename)
-    result_image = cv2.imread(file_path)
-    result_image = cv2.cvtColor(result_image, cv2.COLOR_BGR2RGB)
-    return result_image
-
-  def launchInterface(self):
-    interface = gr.Interface(
-        fn = self.upscale,
-        inputs = [
-            "image",
-            gr.Slider(2, 10, value = 2, label = "Upscale Factor", info = "Resolution upscaling factor"),
-            gr.Dropdown(
-                choices = ["v1.4", "v1.3", "v1.2"],
-                value = "v1.3",
-                label = "Model Version",
-                info = """
-                Model variants based on different functionalities (See detailed info below)
-                """
-            ),
-            gr.Markdown(
-                """
-                - **v1.4** :  More details and better identity.
-                - **v1.3** :  Better quality, natural outputs.
-                - **v1.2** :  Sharper outputs with slight beautification of faces.
-                """
-            )
-        ],
-        outputs = [
-            "image"
-        ],
-        title = "Sharpen Blurry Memories: Supercharge Your Images with Generative AI (GFPGAN + RealESRGAN)",
-        article = "HyperRez, a Python library built by Rauhan Ahmed Siddiqui, utilizes AI's power to upscale and enhance images. Leverage GFPGAN for face restoration and RealESRGAN for background upscaling, all deployed in a GPU-powered Gradio interface for lightning-fast results. Enhance your images like never before!",
-    )
-    interface.launch(debug = True)
+import shutil
+import os
+import gradio as gr
+import cv2
+import math
+
+class ImageUpscaler:
+
+  def __init__(self):
+    pass
+
+  def upscale(self, image, scale_factor, model_version, _):
+    try:
+      shutil.rmtree("inputs")
+      shutil.rmtree("results")
+    except:
+      pass
+    os.mkdir("inputs")
+    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+    cv2.imwrite("inputs/image.jpg", image)
+    os.system(f"python -m HyperRez.inference_realesrgan -n RealESRGAN_x4plus -i inputs -o results --outscale {scale_factor} --face_enhance --face_enhance_model {model_version}")
+    filename = os.listdir("results")[0]
+    file_path = os.path.join("results", filename)
+    result_image = cv2.imread(file_path)
+    result_image = cv2.cvtColor(result_image, cv2.COLOR_BGR2RGB)
+    return result_image
+
+  def launchInterface(self):
+    interface = gr.Interface(
+        fn = self.upscale,
+        inputs = [
+            "image",
+            gr.Slider(2, 10, value = 2, label = "Upscale Factor", info = "Resolution upscaling factor"),
+            gr.Dropdown(
+                choices = ["v1.4", "v1.3", "v1.2"],
+                value = "v1.3",
+                label = "Model Version",
+                info = """
+                Model variants based on different functionalities (See detailed info below)
+                """
+            ),
+            gr.Markdown(
+                """
+                - **v1.4** :  More details and better identity.
+                - **v1.3** :  Better quality, natural outputs.
+                - **v1.2** :  Sharper outputs with slight beautification of faces.
+                """
+            )
+        ],
+        outputs = [
+            "image"
+        ],
+        title = "Sharpen Blurry Memories: Supercharge Your Images with Generative AI (GFPGAN + RealESRGAN)",
+        article = "HyperRez, a Python library built by Rauhan Ahmed Siddiqui, utilizes AI's power to upscale and enhance images. Leverage GFPGAN for face restoration and RealESRGAN for background upscaling, all deployed in a GPU-powered Gradio interface for lightning-fast results. Enhance your images like never before!",
+    )
+    interface.launch(debug = True)
```

### Comparing `HyperRez-1.0.0/HyperRez/inference_realesrgan.py` & `HyperRez-2.0/HyperRez/inference_realesrgan.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import argparse
-import cv2
-import glob
-import os
-from basicsr.archs.rrdbnet_arch import RRDBNet
-from basicsr.utils.download_util import load_file_from_url
-
-from realesrgan import RealESRGANer
-from realesrgan.archs.srvgg_arch import SRVGGNetCompact
-
-
-def main():
-    """Inference demo for Real-ESRGAN.
-    """
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-i', '--input', type=str, default='inputs', help='Input image or folder')
-    parser.add_argument(
-        '-n',
-        '--model_name',
-        type=str,
-        default='RealESRGAN_x4plus',
-        help=('Model names: RealESRGAN_x4plus | RealESRNet_x4plus | RealESRGAN_x4plus_anime_6B | RealESRGAN_x2plus | '
-              'realesr-animevideov3 | realesr-general-x4v3'))
-    parser.add_argument('-o', '--output', type=str, default='results', help='Output folder')
-    parser.add_argument(
-        '-dn',
-        '--denoise_strength',
-        type=float,
-        default=0.5,
-        help=('Denoise strength. 0 for weak denoise (keep noise), 1 for strong denoise ability. '
-              'Only used for the realesr-general-x4v3 model'))
-    parser.add_argument('-s', '--outscale', type=float, default=4, help='The final upsampling scale of the image')
-    parser.add_argument(
-        '--model_path', type=str, default=None, help='[Option] Model path. Usually, you do not need to specify it')
-    parser.add_argument('--suffix', type=str, default='out', help='Suffix of the restored image')
-    parser.add_argument('-t', '--tile', type=int, default=0, help='Tile size, 0 for no tile during testing')
-    parser.add_argument('--tile_pad', type=int, default=10, help='Tile padding')
-    parser.add_argument('--pre_pad', type=int, default=0, help='Pre padding size at each border')
-    parser.add_argument('--face_enhance', action='store_true', help='Use GFPGAN to enhance face')
-    parser.add_argument('--face_enhance_model', type=str, help='GFPGAN model to be used')
-    parser.add_argument(
-        '--fp32', action='store_true', help='Use fp32 precision during inference. Default: fp16 (half precision).')
-    parser.add_argument(
-        '--alpha_upsampler',
-        type=str,
-        default='realesrgan',
-        help='The upsampler for the alpha channels. Options: realesrgan | bicubic')
-    parser.add_argument(
-        '--ext',
-        type=str,
-        default='auto',
-        help='Image extension. Options: auto | jpg | png, auto means using the same extension as inputs')
-    parser.add_argument(
-        '-g', '--gpu-id', type=int, default=None, help='gpu device to use (default=None) can be 0,1,2 for multi-gpu')
-
-    args = parser.parse_args()
-
-    # determine models according to model names
-    args.model_name = args.model_name.split('.')[0]
-    if args.model_name == 'RealESRGAN_x4plus':  # x4 RRDBNet model
-        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4)
-        netscale = 4
-        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.0/RealESRGAN_x4plus.pth']
-    elif args.model_name == 'RealESRNet_x4plus':  # x4 RRDBNet model
-        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4)
-        netscale = 4
-        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.1/RealESRNet_x4plus.pth']
-    elif args.model_name == 'RealESRGAN_x4plus_anime_6B':  # x4 RRDBNet model with 6 blocks
-        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4)
-        netscale = 4
-        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth']
-    elif args.model_name == 'RealESRGAN_x2plus':  # x2 RRDBNet model
-        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=2)
-        netscale = 2
-        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.1/RealESRGAN_x2plus.pth']
-    elif args.model_name == 'realesr-animevideov3':  # x4 VGG-style model (XS size)
-        model = SRVGGNetCompact(num_in_ch=3, num_out_ch=3, num_feat=64, num_conv=16, upscale=4, act_type='prelu')
-        netscale = 4
-        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-animevideov3.pth']
-    elif args.model_name == 'realesr-general-x4v3':  # x4 VGG-style model (S size)
-        model = SRVGGNetCompact(num_in_ch=3, num_out_ch=3, num_feat=64, num_conv=32, upscale=4, act_type='prelu')
-        netscale = 4
-        file_url = [
-            'https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-general-wdn-x4v3.pth',
-            'https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-general-x4v3.pth'
-        ]
-
-    # determine model paths
-    if args.model_path is not None:
-        model_path = args.model_path
-    else:
-        model_path = os.path.join('weights', args.model_name + '.pth')
-        if not os.path.isfile(model_path):
-            ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
-            for url in file_url:
-                # model_path will be updated
-                model_path = load_file_from_url(
-                    url=url, model_dir=os.path.join(ROOT_DIR, 'weights'), progress=True, file_name=None)
-
-    # use dni to control the denoise strength
-    dni_weight = None
-    if args.model_name == 'realesr-general-x4v3' and args.denoise_strength != 1:
-        wdn_model_path = model_path.replace('realesr-general-x4v3', 'realesr-general-wdn-x4v3')
-        model_path = [model_path, wdn_model_path]
-        dni_weight = [args.denoise_strength, 1 - args.denoise_strength]
-
-    # restorer
-    upsampler = RealESRGANer(
-        scale=netscale,
-        model_path=model_path,
-        dni_weight=dni_weight,
-        model=model,
-        tile=args.tile,
-        tile_pad=args.tile_pad,
-        pre_pad=args.pre_pad,
-        half=not args.fp32,
-        gpu_id=args.gpu_id)
-
-    if args.face_enhance:  # Use GFPGAN for face enhancement
-        from gfpgan import GFPGANer
-        face_enhancer = GFPGANer(
-            model_path=f'https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGAN{args.face_enhance_model}.pth',
-            upscale=args.outscale,
-            arch='clean',
-            channel_multiplier=2,
-            bg_upsampler=upsampler)
-    os.makedirs(args.output, exist_ok=True)
-
-    if os.path.isfile(args.input):
-        paths = [args.input]
-    else:
-        paths = sorted(glob.glob(os.path.join(args.input, '*')))
-
-    for idx, path in enumerate(paths):
-        imgname, extension = os.path.splitext(os.path.basename(path))
-        print('Testing', idx, imgname)
-
-        img = cv2.imread(path, cv2.IMREAD_UNCHANGED)
-        if len(img.shape) == 3 and img.shape[2] == 4:
-            img_mode = 'RGBA'
-        else:
-            img_mode = None
-
-        try:
-            if args.face_enhance:
-                _, _, output = face_enhancer.enhance(img, has_aligned=False, only_center_face=False, paste_back=True)
-            else:
-                output, _ = upsampler.enhance(img, outscale=args.outscale)
-        except RuntimeError as error:
-            print('Error', error)
-            print('If you encounter CUDA out of memory, try to set --tile with a smaller number.')
-        else:
-            if args.ext == 'auto':
-                extension = extension[1:]
-            else:
-                extension = args.ext
-            if img_mode == 'RGBA':  # RGBA images should be saved in png format
-                extension = 'png'
-            if args.suffix == '':
-                save_path = os.path.join(args.output, f'{imgname}.{extension}')
-            else:
-                save_path = os.path.join(args.output, f'{imgname}_{args.suffix}.{extension}')
-            cv2.imwrite(save_path, output)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import cv2
+import glob
+import os
+from basicsr.archs.rrdbnet_arch import RRDBNet
+from basicsr.utils.download_util import load_file_from_url
+
+from realesrgan import RealESRGANer
+from realesrgan.archs.srvgg_arch import SRVGGNetCompact
+
+
+def main():
+    """Inference demo for Real-ESRGAN.
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-i', '--input', type=str, default='inputs', help='Input image or folder')
+    parser.add_argument(
+        '-n',
+        '--model_name',
+        type=str,
+        default='RealESRGAN_x4plus',
+        help=('Model names: RealESRGAN_x4plus | RealESRNet_x4plus | RealESRGAN_x4plus_anime_6B | RealESRGAN_x2plus | '
+              'realesr-animevideov3 | realesr-general-x4v3'))
+    parser.add_argument('-o', '--output', type=str, default='results', help='Output folder')
+    parser.add_argument(
+        '-dn',
+        '--denoise_strength',
+        type=float,
+        default=0.5,
+        help=('Denoise strength. 0 for weak denoise (keep noise), 1 for strong denoise ability. '
+              'Only used for the realesr-general-x4v3 model'))
+    parser.add_argument('-s', '--outscale', type=float, default=4, help='The final upsampling scale of the image')
+    parser.add_argument(
+        '--model_path', type=str, default=None, help='[Option] Model path. Usually, you do not need to specify it')
+    parser.add_argument('--suffix', type=str, default='out', help='Suffix of the restored image')
+    parser.add_argument('-t', '--tile', type=int, default=0, help='Tile size, 0 for no tile during testing')
+    parser.add_argument('--tile_pad', type=int, default=10, help='Tile padding')
+    parser.add_argument('--pre_pad', type=int, default=0, help='Pre padding size at each border')
+    parser.add_argument('--face_enhance', action='store_true', help='Use GFPGAN to enhance face')
+    parser.add_argument('--face_enhance_model', type=str, help='GFPGAN model to be used')
+    parser.add_argument(
+        '--fp32', action='store_true', help='Use fp32 precision during inference. Default: fp16 (half precision).')
+    parser.add_argument(
+        '--alpha_upsampler',
+        type=str,
+        default='realesrgan',
+        help='The upsampler for the alpha channels. Options: realesrgan | bicubic')
+    parser.add_argument(
+        '--ext',
+        type=str,
+        default='auto',
+        help='Image extension. Options: auto | jpg | png, auto means using the same extension as inputs')
+    parser.add_argument(
+        '-g', '--gpu-id', type=int, default=None, help='gpu device to use (default=None) can be 0,1,2 for multi-gpu')
+
+    args = parser.parse_args()
+
+    # determine models according to model names
+    args.model_name = args.model_name.split('.')[0]
+    if args.model_name == 'RealESRGAN_x4plus':  # x4 RRDBNet model
+        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4)
+        netscale = 4
+        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.0/RealESRGAN_x4plus.pth']
+    elif args.model_name == 'RealESRNet_x4plus':  # x4 RRDBNet model
+        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4)
+        netscale = 4
+        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.1/RealESRNet_x4plus.pth']
+    elif args.model_name == 'RealESRGAN_x4plus_anime_6B':  # x4 RRDBNet model with 6 blocks
+        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4)
+        netscale = 4
+        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth']
+    elif args.model_name == 'RealESRGAN_x2plus':  # x2 RRDBNet model
+        model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=2)
+        netscale = 2
+        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.1/RealESRGAN_x2plus.pth']
+    elif args.model_name == 'realesr-animevideov3':  # x4 VGG-style model (XS size)
+        model = SRVGGNetCompact(num_in_ch=3, num_out_ch=3, num_feat=64, num_conv=16, upscale=4, act_type='prelu')
+        netscale = 4
+        file_url = ['https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-animevideov3.pth']
+    elif args.model_name == 'realesr-general-x4v3':  # x4 VGG-style model (S size)
+        model = SRVGGNetCompact(num_in_ch=3, num_out_ch=3, num_feat=64, num_conv=32, upscale=4, act_type='prelu')
+        netscale = 4
+        file_url = [
+            'https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-general-wdn-x4v3.pth',
+            'https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesr-general-x4v3.pth'
+        ]
+
+    # determine model paths
+    if args.model_path is not None:
+        model_path = args.model_path
+    else:
+        model_path = os.path.join('weights', args.model_name + '.pth')
+        if not os.path.isfile(model_path):
+            ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
+            for url in file_url:
+                # model_path will be updated
+                model_path = load_file_from_url(
+                    url=url, model_dir=os.path.join(ROOT_DIR, 'weights'), progress=True, file_name=None)
+
+    # use dni to control the denoise strength
+    dni_weight = None
+    if args.model_name == 'realesr-general-x4v3' and args.denoise_strength != 1:
+        wdn_model_path = model_path.replace('realesr-general-x4v3', 'realesr-general-wdn-x4v3')
+        model_path = [model_path, wdn_model_path]
+        dni_weight = [args.denoise_strength, 1 - args.denoise_strength]
+
+    # restorer
+    upsampler = RealESRGANer(
+        scale=netscale,
+        model_path=model_path,
+        dni_weight=dni_weight,
+        model=model,
+        tile=args.tile,
+        tile_pad=args.tile_pad,
+        pre_pad=args.pre_pad,
+        half=not args.fp32,
+        gpu_id=args.gpu_id)
+
+    if args.face_enhance:  # Use GFPGAN for face enhancement
+        from gfpgan import GFPGANer
+        face_enhancer = GFPGANer(
+            model_path=f'https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGAN{args.face_enhance_model}.pth',
+            upscale=args.outscale,
+            arch='clean',
+            channel_multiplier=2,
+            bg_upsampler=upsampler)
+    os.makedirs(args.output, exist_ok=True)
+
+    if os.path.isfile(args.input):
+        paths = [args.input]
+    else:
+        paths = sorted(glob.glob(os.path.join(args.input, '*')))
+
+    for idx, path in enumerate(paths):
+        imgname, extension = os.path.splitext(os.path.basename(path))
+        print('Testing', idx, imgname)
+
+        img = cv2.imread(path, cv2.IMREAD_UNCHANGED)
+        if len(img.shape) == 3 and img.shape[2] == 4:
+            img_mode = 'RGBA'
+        else:
+            img_mode = None
+
+        try:
+            if args.face_enhance:
+                _, _, output = face_enhancer.enhance(img, has_aligned=False, only_center_face=False, paste_back=True)
+            else:
+                output, _ = upsampler.enhance(img, outscale=args.outscale)
+        except RuntimeError as error:
+            print('Error', error)
+            print('If you encounter CUDA out of memory, try to set --tile with a smaller number.')
+        else:
+            if args.ext == 'auto':
+                extension = extension[1:]
+            else:
+                extension = args.ext
+            if img_mode == 'RGBA':  # RGBA images should be saved in png format
+                extension = 'png'
+            if args.suffix == '':
+                save_path = os.path.join(args.output, f'{imgname}.{extension}')
+            else:
+                save_path = os.path.join(args.output, f'{imgname}_{args.suffix}.{extension}')
+            cv2.imwrite(save_path, output)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `HyperRez-1.0.0/HyperRez.egg-info/PKG-INFO` & `HyperRez-2.0/HyperRez.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,61 @@
-Metadata-Version: 2.1
-Name: HyperRez
-Version: 1.0.0
-Summary: Sharpen Blurry Memories: Supercharge Your Images with HyperRez
-Home-page: https://github.com/RauhanAhmed/HyperRez
-Author: Rauhan Ahmed Siddiqui
-Author-email: rauhaan.siddiqui@gamil.com
-License: MIT
-Keywords: computer vision,pytorch,image restoration,super-resolution,esrgan,real-esrgan,gfpgan,gradio,image enhancer,image quality enhancement,image upscaler,image quality upscaler
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: basicsr>=1.4.2
-Requires-Dist: facexlib>=0.2.5
-Requires-Dist: realesrgan
-Requires-Dist: gradio
-Requires-Dist: gfpgan>=1.3.5
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: Pillow
-Requires-Dist: torch>=1.7
-Requires-Dist: torchvision
-Requires-Dist: tqdm
-
-
-# HyperRez: Sharpen Blurry Memories
-
-
-Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
-
-
-## Features
-
-- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
-- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
-- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
-- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
-
-
-## Screenshots
-
-![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
-
-![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
-
-![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
-
-## Installation
-```bash
-  pip install HyperRez
-```
-    
-## Usage
-
-```python
-from HyperRez import ImageUpscaler
-
-# Initialise the upscaler
-upscaler = ImageUpscaler()
-
-# Launch the Gradio Interface
-upscaler.launchInterface()
-```
-
-
-## Authors
-
-[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
-
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: HyperRez
+Version: 2.0
+Summary: Sharpen Blurry Memories: Supercharge Your Images with HyperRez
+Home-page: https://github.com/RauhanAhmed/HyperRez
+Author: Rauhan Ahmed Siddiqui
+Author-email: rauhaan.siddiqui@gamil.com
+License: MIT
+Keywords: computer vision,pytorch,image restoration,super-resolution,esrgan,real-esrgan,gfpgan,gradio,image enhancer,image quality enhancement,image upscaler,image quality upscaler
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# HyperRez: Sharpen Blurry Memories
+
+
+Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
+
+
+## Features
+
+- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
+- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
+- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
+- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
+
+
+## Screenshots
+
+![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
+
+![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
+
+![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
+
+## Installation
+```bash
+  pip install HyperRez
+```
+    
+## Usage
+
+```python
+from HyperRez import ImageUpscaler
+
+# Initialise the upscaler
+upscaler = ImageUpscaler()
+
+# Launch the Gradio Interface
+upscaler.launchInterface()
+```
+
+
+## Authors
+
+[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
+
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `HyperRez-1.0.0/PKG-INFO` & `HyperRez-2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,61 @@
-Metadata-Version: 2.1
-Name: HyperRez
-Version: 1.0.0
-Summary: Sharpen Blurry Memories: Supercharge Your Images with HyperRez
-Home-page: https://github.com/RauhanAhmed/HyperRez
-Author: Rauhan Ahmed Siddiqui
-Author-email: rauhaan.siddiqui@gamil.com
-License: MIT
-Keywords: computer vision,pytorch,image restoration,super-resolution,esrgan,real-esrgan,gfpgan,gradio,image enhancer,image quality enhancement,image upscaler,image quality upscaler
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: basicsr>=1.4.2
-Requires-Dist: facexlib>=0.2.5
-Requires-Dist: realesrgan
-Requires-Dist: gradio
-Requires-Dist: gfpgan>=1.3.5
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: Pillow
-Requires-Dist: torch>=1.7
-Requires-Dist: torchvision
-Requires-Dist: tqdm
-
-
-# HyperRez: Sharpen Blurry Memories
-
-
-Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
-
-
-## Features
-
-- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
-- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
-- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
-- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
-
-
-## Screenshots
-
-![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
-
-![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
-
-![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
-
-## Installation
-```bash
-  pip install HyperRez
-```
-    
-## Usage
-
-```python
-from HyperRez import ImageUpscaler
-
-# Initialise the upscaler
-upscaler = ImageUpscaler()
-
-# Launch the Gradio Interface
-upscaler.launchInterface()
-```
-
-
-## Authors
-
-[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
-
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: HyperRez
+Version: 2.0
+Summary: Sharpen Blurry Memories: Supercharge Your Images with HyperRez
+Home-page: https://github.com/RauhanAhmed/HyperRez
+Author: Rauhan Ahmed Siddiqui
+Author-email: rauhaan.siddiqui@gamil.com
+License: MIT
+Keywords: computer vision,pytorch,image restoration,super-resolution,esrgan,real-esrgan,gfpgan,gradio,image enhancer,image quality enhancement,image upscaler,image quality upscaler
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# HyperRez: Sharpen Blurry Memories
+
+
+Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
+
+
+## Features
+
+- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
+- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
+- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
+- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
+
+
+## Screenshots
+
+![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
+
+![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
+
+![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
+
+## Installation
+```bash
+  pip install HyperRez
+```
+    
+## Usage
+
+```python
+from HyperRez import ImageUpscaler
+
+# Initialise the upscaler
+upscaler = ImageUpscaler()
+
+# Launch the Gradio Interface
+upscaler.launchInterface()
+```
+
+
+## Authors
+
+[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
+
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `HyperRez-1.0.0/README.md` & `HyperRez-2.0/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-
-# HyperRez: Sharpen Blurry Memories
-
-
-Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
-
-
-## Features
-
-- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
-- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
-- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
-- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
-
-
-## Screenshots
-
-![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
-
-![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
-
-![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
-
-## Installation
-```bash
-  pip install HyperRez
-```
-    
-## Usage
-
-```python
-from HyperRez import ImageUpscaler
-
-# Initialise the upscaler
-upscaler = ImageUpscaler()
-
-# Launch the Gradio Interface
-upscaler.launchInterface()
-```
-
-
-## Authors
-
-[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
-
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+
+# HyperRez: Sharpen Blurry Memories
+
+
+Enhance and upscale your images effortlessly with HyperRez, a Python library crafted by Rauhan Ahmed Siddiqui. Leveraging the power of GFPGAN and RealESRGAN, state-of-the-art Generative Adversarial Networks, this library provides advanced image enhancement capabilities. Real-ESRGAN focuses on upscaling backgrounds, while GFPGAN excels in refining the faces of human subjects.
+
+
+## Features
+
+- **Dual Network Integration:** Combines Real-ESRGAN and GFPGAN for comprehensive image enhancement.
+- **Gradio Interface:** Seamlessly deployed into production using Gradio Interface for an interactive and user-friendly experience.
+- **GPU Acceleration:** Optimized for GPU processing, ensuring fast and efficient image enhancement (Note: Performance may be suboptimal on CPUs).
+- **PyPI Integration:** Available on PyPI as the "HyperRez" library for easy installation and use.
+
+
+## Screenshots
+
+![App Screenshot](https://i.ibb.co/wRTQwrt/Beige-and-White-Be-Yourself-Square-Pillow-2.png)
+
+![App Screenshot](https://i.ibb.co/VLsXqY6/Screenshot-2024-02-11-005136.png)
+
+![App Screenshot](https://i.ibb.co/BBKh0BR/Screenshot-2024-02-11-005236.png)
+
+## Installation
+```bash
+  pip install HyperRez
+```
+    
+## Usage
+
+```python
+from HyperRez import ImageUpscaler
+
+# Initialise the upscaler
+upscaler = ImageUpscaler()
+
+# Launch the Gradio Interface
+upscaler.launchInterface()
+```
+
+
+## Authors
+
+[Rauhan Ahmed Siddiqui](https://linkedin.com/in/rauhan-ahmed/)
+
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `HyperRez-1.0.0/setup.py` & `HyperRez-2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from setuptools import find_packages, setup
-
-import os
-import subprocess
-import time
-
-def readme():
-    with open('README.md', encoding='utf-8') as f:
-        content = f.read()
-    return content
-
-def get_git_hash():
-
-    def _minimal_ext_cmd(cmd):
-        # construct minimal environment
-        env = {}
-        for k in ['SYSTEMROOT', 'PATH', 'HOME']:
-            v = os.environ.get(k)
-            if v is not None:
-                env[k] = v
-        # LANGUAGE is used on win32
-        env['LANGUAGE'] = 'C'
-        env['LANG'] = 'C'
-        env['LC_ALL'] = 'C'
-        out = subprocess.Popen(cmd, stdout=subprocess.PIPE, env=env).communicate()[0]
-        return out
-
-    try:
-        out = _minimal_ext_cmd(['git', 'rev-parse', 'HEAD'])
-        sha = out.strip().decode('ascii')
-    except OSError:
-        sha = 'unknown'
-
-    return sha
-
-
-def get_hash():
-    if os.path.exists('.git'):
-        sha = get_git_hash()[:7]
-    else:
-        sha = 'unknown'
-
-    return sha
-
-def get_requirements(filename='requirements.txt'):
-    here = os.path.dirname(os.path.realpath(__file__))
-    with open(os.path.join(here, filename), 'r') as f:
-        requires = [line.replace('\n', '') for line in f.readlines()]
-    return requires
-
-if __name__ == '__main__':
-    setup(
-        name='HyperRez',
-        version="1.0.0",
-        description='Sharpen Blurry Memories: Supercharge Your Images with HyperRez',
-        long_description=readme(),
-        long_description_content_type='text/markdown',
-        author='Rauhan Ahmed Siddiqui',
-        author_email='rauhaan.siddiqui@gamil.com',
-        keywords='computer vision, pytorch, image restoration, super-resolution, esrgan, real-esrgan, gfpgan, gradio, image enhancer, image quality enhancement, image upscaler, image quality upscaler',
-        url='https://github.com/RauhanAhmed/HyperRez',
-        include_package_data=True,
-        packages=find_packages(exclude=('options', 'datasets', 'experiments', 'results', 'tb_logger', 'wandb')),
-        license='MIT',
-        setup_requires=['cython', 'numpy'],
-        install_requires=get_requirements(),
-        zip_safe=False)
+from setuptools import find_packages, setup
+
+import os
+import subprocess
+import time
+
+def readme():
+    with open('README.md', encoding='utf-8') as f:
+        content = f.read()
+    return content
+
+def get_git_hash():
+
+    def _minimal_ext_cmd(cmd):
+        # construct minimal environment
+        env = {}
+        for k in ['SYSTEMROOT', 'PATH', 'HOME']:
+            v = os.environ.get(k)
+            if v is not None:
+                env[k] = v
+        # LANGUAGE is used on win32
+        env['LANGUAGE'] = 'C'
+        env['LANG'] = 'C'
+        env['LC_ALL'] = 'C'
+        out = subprocess.Popen(cmd, stdout=subprocess.PIPE, env=env).communicate()[0]
+        return out
+
+    try:
+        out = _minimal_ext_cmd(['git', 'rev-parse', 'HEAD'])
+        sha = out.strip().decode('ascii')
+    except OSError:
+        sha = 'unknown'
+
+    return sha
+
+
+def get_hash():
+    if os.path.exists('.git'):
+        sha = get_git_hash()[:7]
+    else:
+        sha = 'unknown'
+
+    return sha
+
+def get_requirements(filename='requirements.txt'):
+    here = os.path.dirname(os.path.realpath(__file__))
+    with open(os.path.join(here, filename), 'r') as f:
+        requires = [line.replace('\n', '') for line in f.readlines()]
+    return requires
+
+if __name__ == '__main__':
+    setup(
+        name='HyperRez',
+        version="2.0",
+        description='Sharpen Blurry Memories: Supercharge Your Images with HyperRez',
+        long_description=readme(),
+        long_description_content_type='text/markdown',
+        author='Rauhan Ahmed Siddiqui',
+        author_email='rauhaan.siddiqui@gamil.com',
+        keywords='computer vision, pytorch, image restoration, super-resolution, esrgan, real-esrgan, gfpgan, gradio, image enhancer, image quality enhancement, image upscaler, image quality upscaler',
+        url='https://github.com/RauhanAhmed/HyperRez',
+        include_package_data=True,
+        packages=find_packages(exclude=('options', 'datasets', 'experiments', 'results', 'tb_logger', 'wandb')),
+        license='MIT',
+        setup_requires=['cython', 'numpy'],
+        install_requires=get_requirements(),
+        zip_safe=False)
```

