# Comparing `tmp/pyzjr-1.3.4.tar.gz` & `tmp/pyzjr-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.3.4.tar", last modified: Wed Mar 27 04:15:45 2024, max compression
+gzip compressed data, was "dist\pyzjr-1.3.5.tar", last modified: Sat Apr 20 07:27:26 2024, max compression
```

## Comparing `pyzjr-1.3.4.tar` & `pyzjr-1.3.5.tar`

### file list

```diff
@@ -1,197 +1,204 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/
--rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.4/LICENSE
--rw-rw-rw-   0        0        0     2931 2024-03-27 04:15:45.000000 pyzjr-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/models_img/
--rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.4/models_img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Math/
--rw-rw-rw-   0        0        0      694 2024-03-21 17:08:46.000000 pyzjr-1.3.4/pyzjr/Math/Numpy.py
--rw-rw-rw-   0        0        0      240 2024-03-16 15:32:39.000000 pyzjr-1.3.4/pyzjr/Math/__init__.py
--rw-rw-rw-   0        0        0     3438 2024-02-20 09:48:40.000000 pyzjr-1.3.4/pyzjr/Math/arithmetic.py
--rw-rw-rw-   0        0        0       88 2024-02-19 09:31:13.000000 pyzjr-1.3.4/pyzjr/Math/constant.py
--rw-rw-rw-   0        0        0     7362 2024-02-19 10:31:56.000000 pyzjr-1.3.4/pyzjr/Math/function.py
--rw-rw-rw-   0        0        0    19620 2024-02-19 09:52:53.000000 pyzjr-1.3.4/pyzjr/Math/point_line.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/Attention/
--rw-rw-rw-   0        0        0     2271 2024-03-04 07:16:29.000000 pyzjr-1.3.4/pyzjr/Models/Attention/A2.py
--rw-rw-rw-   0        0        0     1927 2024-03-09 14:59:27.000000 pyzjr-1.3.4/pyzjr/Models/Attention/AFT.py
--rw-rw-rw-   0        0        0     1911 2024-03-09 15:28:12.000000 pyzjr-1.3.4/pyzjr/Models/Attention/DANet.py
--rw-rw-rw-   0        0        0     5412 2024-03-09 15:10:59.000000 pyzjr-1.3.4/pyzjr/Models/Attention/MobileViT.py
--rw-rw-rw-   0        0        0     3105 2024-03-21 17:03:45.000000 pyzjr-1.3.4/pyzjr/Models/Attention/SE.py
--rw-rw-rw-   0        0        0     1933 2024-03-09 15:18:47.000000 pyzjr-1.3.4/pyzjr/Models/Attention/ViP.py
--rw-rw-rw-   0        0        0     1583 2024-03-16 15:41:22.000000 pyzjr-1.3.4/pyzjr/Models/Attention/__init__.py
--rw-rw-rw-   0        0        0     4795 2024-03-09 14:59:04.000000 pyzjr-1.3.4/pyzjr/Models/Attention/acmix.py
--rw-rw-rw-   0        0        0    12705 2024-03-09 15:00:08.000000 pyzjr-1.3.4/pyzjr/Models/Attention/axial.py
--rw-rw-rw-   0        0        0     3180 2024-03-04 07:32:10.000000 pyzjr-1.3.4/pyzjr/Models/Attention/bam.py
--rw-rw-rw-   0        0        0     3729 2024-03-04 12:35:57.000000 pyzjr-1.3.4/pyzjr/Models/Attention/cbam.py
--rw-rw-rw-   0        0        0     1635 2024-03-09 15:01:57.000000 pyzjr-1.3.4/pyzjr/Models/Attention/coord.py
--rw-rw-rw-   0        0        0     2175 2024-03-04 12:19:45.000000 pyzjr-1.3.4/pyzjr/Models/Attention/cot.py
--rw-rw-rw-   0        0        0     2688 2024-03-09 15:02:25.000000 pyzjr-1.3.4/pyzjr/Models/Attention/crisscross.py
--rw-rw-rw-   0        0        0    26854 2024-03-09 15:22:58.000000 pyzjr-1.3.4/pyzjr/Models/Attention/crossformer.py
--rw-rw-rw-   0        0        0    23025 2024-03-09 15:25:56.000000 pyzjr-1.3.4/pyzjr/Models/Attention/dat.py
--rw-rw-rw-   0        0        0     1340 2024-03-09 15:04:58.000000 pyzjr-1.3.4/pyzjr/Models/Attention/eca.py
--rw-rw-rw-   0        0        0     3752 2024-03-09 15:05:31.000000 pyzjr-1.3.4/pyzjr/Models/Attention/emsa.py
--rw-rw-rw-   0        0        0     1341 2024-03-09 15:06:14.000000 pyzjr-1.3.4/pyzjr/Models/Attention/external.py
--rw-rw-rw-   0        0        0     4161 2024-03-09 15:19:38.000000 pyzjr-1.3.4/pyzjr/Models/Attention/gfnet.py
--rw-rw-rw-   0        0        0     5444 2024-03-09 15:07:26.000000 pyzjr-1.3.4/pyzjr/Models/Attention/halo.py
--rw-rw-rw-   0        0        0    30578 2024-03-09 15:23:53.000000 pyzjr-1.3.4/pyzjr/Models/Attention/moat.py
--rw-rw-rw-   0        0        0     3670 2024-03-09 15:08:27.000000 pyzjr-1.3.4/pyzjr/Models/Attention/muse.py
--rw-rw-rw-   0        0        0     2281 2024-03-09 15:11:27.000000 pyzjr-1.3.4/pyzjr/Models/Attention/outlook.py
--rw-rw-rw-   0        0        0      985 2024-03-09 15:29:37.000000 pyzjr-1.3.4/pyzjr/Models/Attention/parnet.py
--rw-rw-rw-   0        0        0     4087 2024-03-09 15:13:38.000000 pyzjr-1.3.4/pyzjr/Models/Attention/polarized.py
--rw-rw-rw-   0        0        0     2296 2024-03-09 15:11:51.000000 pyzjr-1.3.4/pyzjr/Models/Attention/psa.py
--rw-rw-rw-   0        0        0      930 2024-03-09 14:57:03.000000 pyzjr-1.3.4/pyzjr/Models/Attention/residual.py
--rw-rw-rw-   0        0        0     2355 2024-03-09 14:52:15.000000 pyzjr-1.3.4/pyzjr/Models/Attention/s2.py
--rw-rw-rw-   0        0        0     3084 2024-03-09 15:15:20.000000 pyzjr-1.3.4/pyzjr/Models/Attention/self_att.py
--rw-rw-rw-   0        0        0     1784 2024-03-09 15:14:10.000000 pyzjr-1.3.4/pyzjr/Models/Attention/sge.py
--rw-rw-rw-   0        0        0     2637 2024-03-09 15:16:05.000000 pyzjr-1.3.4/pyzjr/Models/Attention/shuffle.py
--rw-rw-rw-   0        0        0      909 2024-03-09 15:16:39.000000 pyzjr-1.3.4/pyzjr/Models/Attention/simam.py
--rw-rw-rw-   0        0        0     2933 2024-03-09 15:17:26.000000 pyzjr-1.3.4/pyzjr/Models/Attention/simplified_self_att.py
--rw-rw-rw-   0        0        0     1863 2024-03-18 11:12:03.000000 pyzjr-1.3.4/pyzjr/Models/Attention/sk.py
--rw-rw-rw-   0        0        0     2349 2024-03-09 15:18:03.000000 pyzjr-1.3.4/pyzjr/Models/Attention/triplet.py
--rw-rw-rw-   0        0        0     2234 2024-03-04 13:24:57.000000 pyzjr-1.3.4/pyzjr/Models/Attention/ufo.py
--rw-rw-rw-   0        0        0      220 2024-03-16 15:32:39.000000 pyzjr-1.3.4/pyzjr/Models/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-03-21 16:32:55.000000 pyzjr-1.3.4/pyzjr/Models/_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/backbone/
--rw-rw-rw-   0        0        0     5692 2024-03-22 16:07:30.000000 pyzjr-1.3.4/pyzjr/Models/backbone/Darknet.py
--rw-rw-rw-   0        0        0    25919 2024-02-23 14:10:01.000000 pyzjr-1.3.4/pyzjr/Models/backbone/Ghostnet.py
--rw-rw-rw-   0        0        0     1953 2024-03-26 15:38:25.000000 pyzjr-1.3.4/pyzjr/Models/backbone/__init__.py
--rw-rw-rw-   0        0        0     1882 2024-03-22 15:32:04.000000 pyzjr-1.3.4/pyzjr/Models/backbone/alexnet.py
--rw-rw-rw-   0        0        0     7560 2024-02-23 14:18:22.000000 pyzjr-1.3.4/pyzjr/Models/backbone/conv2former.py
--rw-rw-rw-   0        0        0     6278 2024-02-23 14:18:22.000000 pyzjr-1.3.4/pyzjr/Models/backbone/densenet.py
--rw-rw-rw-   0        0        0    12808 2024-03-26 15:38:25.000000 pyzjr-1.3.4/pyzjr/Models/backbone/drn.py
--rw-rw-rw-   0        0        0    17934 2024-03-24 13:47:07.000000 pyzjr-1.3.4/pyzjr/Models/backbone/efficientnet.py
--rw-rw-rw-   0        0        0     7153 2024-02-27 16:01:26.000000 pyzjr-1.3.4/pyzjr/Models/backbone/fasternet.py
--rw-rw-rw-   0        0        0     5623 2024-02-23 14:18:22.000000 pyzjr-1.3.4/pyzjr/Models/backbone/googlenet.py
--rw-rw-rw-   0        0        0     1869 2024-02-04 04:44:18.000000 pyzjr-1.3.4/pyzjr/Models/backbone/lenet.py
--rw-rw-rw-   0        0        0     7048 2024-03-18 16:29:49.000000 pyzjr-1.3.4/pyzjr/Models/backbone/mnasnet.py
--rw-rw-rw-   0        0        0    16395 2024-02-16 16:51:01.000000 pyzjr-1.3.4/pyzjr/Models/backbone/mobilenet.py
--rw-rw-rw-   0        0        0     7217 2024-03-18 11:17:15.000000 pyzjr-1.3.4/pyzjr/Models/backbone/regnet.py
--rw-rw-rw-   0        0        0     8531 2024-02-25 16:59:56.000000 pyzjr-1.3.4/pyzjr/Models/backbone/resnet.py
--rw-rw-rw-   0        0        0    11356 2024-03-22 15:56:05.000000 pyzjr-1.3.4/pyzjr/Models/backbone/shufflenet.py
--rw-rw-rw-   0        0        0     4392 2024-03-04 12:30:07.000000 pyzjr-1.3.4/pyzjr/Models/backbone/squeezenet.py
--rw-rw-rw-   0        0        0     3996 2024-02-25 16:22:54.000000 pyzjr-1.3.4/pyzjr/Models/backbone/vgg.py
--rw-rw-rw-   0        0        0     4993 2024-03-26 15:31:29.000000 pyzjr-1.3.4/pyzjr/Models/backbone/xception.py
--rw-rw-rw-   0        0        0     2705 2024-03-22 15:32:04.000000 pyzjr-1.3.4/pyzjr/Models/backbone/zfnet.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/bricks/
--rw-rw-rw-   0        0        0     5637 2024-03-09 15:22:58.000000 pyzjr-1.3.4/pyzjr/Models/bricks/Initer.py
--rw-rw-rw-   0        0        0      358 2024-03-24 16:28:04.000000 pyzjr-1.3.4/pyzjr/Models/bricks/__init__.py
--rw-rw-rw-   0        0        0     1577 2024-03-04 09:07:17.000000 pyzjr-1.3.4/pyzjr/Models/bricks/classfier.py
--rw-rw-rw-   0        0        0    22575 2024-03-04 07:32:10.000000 pyzjr-1.3.4/pyzjr/Models/bricks/comblock.py
--rw-rw-rw-   0        0        0     2646 2024-03-26 15:25:44.000000 pyzjr-1.3.4/pyzjr/Models/bricks/conv_norm_act.py
--rw-rw-rw-   0        0        0     6828 2024-03-04 12:40:27.000000 pyzjr-1.3.4/pyzjr/Models/bricks/drop.py
--rw-rw-rw-   0        0        0     6669 2024-03-06 00:10:20.000000 pyzjr-1.3.4/pyzjr/Models/bricks/mlp.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/conv/
--rw-rw-rw-   0        0        0     1976 2024-03-21 15:48:24.000000 pyzjr-1.3.4/pyzjr/Models/conv/Depthwise_Conv.py
--rw-rw-rw-   0        0        0      508 2024-03-21 15:46:28.000000 pyzjr-1.3.4/pyzjr/Models/conv/Dilated_Conv.py
--rw-rw-rw-   0        0        0     1862 2024-02-29 10:04:41.000000 pyzjr-1.3.4/pyzjr/Models/conv/Partial_Conv.py
--rw-rw-rw-   0        0        0     2660 2024-02-29 10:02:23.000000 pyzjr-1.3.4/pyzjr/Models/conv/Ref_Conv.py
--rw-rw-rw-   0        0        0    11458 2024-02-29 09:11:02.000000 pyzjr-1.3.4/pyzjr/Models/conv/Snake_Conv.py
--rw-rw-rw-   0        0        0      295 2024-03-21 15:46:28.000000 pyzjr-1.3.4/pyzjr/Models/conv/__init__.py
--rw-rw-rw-   0        0        0     2979 2024-02-04 04:56:49.000000 pyzjr-1.3.4/pyzjr/Models/networks.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/sampling/
--rw-rw-rw-   0        0        0      756 2024-03-26 15:09:07.000000 pyzjr-1.3.4/pyzjr/Models/sampling/__init__.py
--rw-rw-rw-   0        0        0     4846 2024-03-04 13:48:54.000000 pyzjr-1.3.4/pyzjr/Models/sampling/adaptivepooling.py
--rw-rw-rw-   0        0        0     1393 2024-01-27 17:10:24.000000 pyzjr-1.3.4/pyzjr/Models/sampling/haarwavelet.py
--rw-rw-rw-   0        0        0     1828 2024-03-04 13:56:06.000000 pyzjr-1.3.4/pyzjr/Models/sampling/medianpooling.py
--rw-rw-rw-   0        0        0     4792 2024-02-26 15:35:21.000000 pyzjr-1.3.4/pyzjr/Models/sampling/standardpooling.py
--rw-rw-rw-   0        0        0      854 2024-03-01 15:33:22.000000 pyzjr-1.3.4/pyzjr/Models/sampling/strideconv.py
--rw-rw-rw-   0        0        0     3692 2024-02-29 15:43:47.000000 pyzjr-1.3.4/pyzjr/Models/sampling/strippooling.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/Models/segmentation/
--rw-rw-rw-   0        0        0       70 2024-02-27 16:31:33.000000 pyzjr-1.3.4/pyzjr/Models/segmentation/__init__.py
--rw-rw-rw-   0        0        0    24988 2024-03-17 06:46:22.000000 pyzjr-1.3.4/pyzjr/Models/segmentation/fcn.py
--rw-rw-rw-   0        0        0     3289 2024-02-29 09:20:12.000000 pyzjr-1.3.4/pyzjr/Models/segmentation/unet.py
--rw-rw-rw-   0        0        0     7095 2024-02-19 09:31:13.000000 pyzjr-1.3.4/pyzjr/PIC.py
--rw-rw-rw-   0        0        0    10349 2024-02-04 05:11:03.000000 pyzjr-1.3.4/pyzjr/Z.py
--rw-rw-rw-   0        0        0      914 2024-02-22 15:54:53.000000 pyzjr-1.3.4/pyzjr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/augmentation/
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/
--rw-rw-rw-   0        0        0      150 2024-02-18 17:28:31.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/__init__.py
--rw-rw-rw-   0        0        0      588 2024-02-13 15:36:04.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/_utils.py
--rw-rw-rw-   0        0        0     3576 2024-02-28 11:47:43.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/colormap.py
--rw-rw-rw-   0        0        0     3339 2023-11-04 05:34:46.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/colorspace.py
--rw-rw-rw-   0        0        0     7461 2024-02-22 15:54:53.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/cvplot.py
--rw-rw-rw-   0        0        0     7928 2024-01-08 12:38:29.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/findcolor.py
--rw-rw-rw-   0        0        0     1066 2024-02-13 17:07:55.000000 pyzjr-1.3.4/pyzjr/augmentation/Color/hex.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/
--rw-rw-rw-   0        0        0    13180 2024-02-28 11:24:23.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/Crack.py
--rw-rw-rw-   0        0        0     8307 2024-02-29 15:56:54.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/_Steger.py
--rw-rw-rw-   0        0        0      366 2024-02-19 10:23:26.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/__init__.py
--rw-rw-rw-   0        0        0     7681 2024-02-18 17:28:31.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/definition.py
--rw-rw-rw-   0        0        0     4827 2024-02-22 16:33:22.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/pixel.py
--rw-rw-rw-   0        0        0     1698 2024-02-19 10:23:26.000000 pyzjr-1.3.4/pyzjr/augmentation/Pixel/utils.py
--rw-rw-rw-   0        0        0      140 2024-02-13 15:41:38.000000 pyzjr-1.3.4/pyzjr/augmentation/__init__.py
--rw-rw-rw-   0        0        0    28643 2024-02-02 16:09:04.000000 pyzjr-1.3.4/pyzjr/augmentation/augments.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/
--rw-rw-rw-   0        0        0      306 2024-02-01 16:36:53.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-02-02 16:09:04.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/_utils.py
--rw-rw-rw-   0        0        0     3413 2024-02-28 11:40:46.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/normal.py
--rw-rw-rw-   0        0        0    10428 2024-03-21 17:03:45.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/opencv.py
--rw-rw-rw-   0        0        0    40747 2024-02-01 16:19:36.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/pillow.py
--rw-rw-rw-   0        0        0     6139 2024-03-21 17:03:45.000000 pyzjr-1.3.4/pyzjr/augmentation/transforms/tvision.py
--rw-rw-rw-   0        0        0     1084 2024-03-04 06:15:09.000000 pyzjr-1.3.4/pyzjr/augmentation/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/core/
--rw-rw-rw-   0        0        0      948 2024-03-04 13:45:57.000000 pyzjr-1.3.4/pyzjr/core/__init__.py
--rw-rw-rw-   0        0        0     2069 2024-03-04 13:45:57.000000 pyzjr-1.3.4/pyzjr/core/_str.py
--rw-rw-rw-   0        0        0      680 2023-10-07 12:04:40.000000 pyzjr-1.3.4/pyzjr/core/_utils.py
--rw-rw-rw-   0        0        0     3521 2024-02-01 15:27:28.000000 pyzjr-1.3.4/pyzjr/core/error.py
--rw-rw-rw-   0        0        0     1437 2024-01-09 08:22:16.000000 pyzjr-1.3.4/pyzjr/core/general.py
--rw-rw-rw-   0        0        0      357 2024-03-04 13:45:57.000000 pyzjr-1.3.4/pyzjr/core/helpers.py
--rw-rw-rw-   0        0        0     7254 2023-11-15 11:43:15.000000 pyzjr-1.3.4/pyzjr/core/lr_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/data/
--rw-rw-rw-   0        0        0     1486 2024-03-13 01:39:58.000000 pyzjr-1.3.4/pyzjr/data/Dataloader.py
--rw-rw-rw-   0        0        0     9590 2024-03-08 01:06:58.000000 pyzjr-1.3.4/pyzjr/data/Dataset.py
--rw-rw-rw-   0        0        0    12749 2024-01-23 12:25:01.000000 pyzjr-1.3.4/pyzjr/data/FM.py
--rw-rw-rw-   0        0        0      255 2024-02-29 16:04:29.000000 pyzjr-1.3.4/pyzjr/data/__init__.py
--rw-rw-rw-   0        0        0     7307 2024-02-10 09:22:56.000000 pyzjr-1.3.4/pyzjr/data/__tensor.py
--rw-rw-rw-   0        0        0     4064 2024-03-08 01:12:34.000000 pyzjr-1.3.4/pyzjr/data/basedataset.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/data/data_set/
--rw-rw-rw-   0        0        0     9436 2024-03-13 01:39:58.000000 pyzjr-1.3.4/pyzjr/data/data_set/Pascal_voc.py
--rw-rw-rw-   0        0        0        0 2024-02-29 16:00:47.000000 pyzjr-1.3.4/pyzjr/data/data_set/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-03-08 01:30:08.000000 pyzjr-1.3.4/pyzjr/data/data_set/config.py
--rw-rw-rw-   0        0        0    10938 2024-02-13 17:18:44.000000 pyzjr-1.3.4/pyzjr/data/io.py
--rw-rw-rw-   0        0        0     4327 2024-03-13 01:20:20.000000 pyzjr-1.3.4/pyzjr/data/printf.py
--rw-rw-rw-   0        0        0    14898 2024-01-07 17:19:56.000000 pyzjr-1.3.4/pyzjr/data/reader.py
--rw-rw-rw-   0        0        0     8822 2024-03-08 01:15:38.000000 pyzjr-1.3.4/pyzjr/data/voc.py
--rw-rw-rw-   0        0        0     1464 2024-03-10 15:38:02.000000 pyzjr-1.3.4/pyzjr/devices.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/dlearn/
--rw-rw-rw-   0        0        0      949 2024-03-11 15:45:28.000000 pyzjr-1.3.4/pyzjr/dlearn/__init__.py
--rw-rw-rw-   0        0        0     8571 2024-02-17 18:07:27.000000 pyzjr-1.3.4/pyzjr/dlearn/callbacklog.py
--rw-rw-rw-   0        0        0     8379 2024-03-13 01:39:58.000000 pyzjr-1.3.4/pyzjr/dlearn/callbacks.py
--rw-rw-rw-   0        0        0     1051 2024-03-11 15:59:35.000000 pyzjr-1.3.4/pyzjr/dlearn/savemodels.py
--rw-rw-rw-   0        0        0     4801 2024-03-11 15:21:20.000000 pyzjr-1.3.4/pyzjr/dlearn/strategy.py
--rw-rw-rw-   0        0        0     5941 2024-02-13 17:19:41.000000 pyzjr-1.3.4/pyzjr/dlearn/tools.py
--rw-rw-rw-   0        0        0     7360 2024-03-11 16:12:42.000000 pyzjr-1.3.4/pyzjr/dlearn/trainer.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/mediapipe/
--rw-rw-rw-   0        0        0     6577 2024-02-29 15:56:54.000000 pyzjr-1.3.4/pyzjr/mediapipe/HandTrack.py
--rw-rw-rw-   0        0        0      376 2024-01-25 07:15:10.000000 pyzjr-1.3.4/pyzjr/mediapipe/__init__.py
--rw-rw-rw-   0        0        0      631 2024-02-04 05:11:03.000000 pyzjr-1.3.4/pyzjr/mediapipe/const.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/nn/
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/nn/Metrics/
--rw-rw-rw-   0        0        0       54 2024-01-26 13:47:39.000000 pyzjr-1.3.4/pyzjr/nn/Metrics/__init__.py
--rw-rw-rw-   0        0        0    16237 2024-02-08 15:56:55.000000 pyzjr-1.3.4/pyzjr/nn/Metrics/classification.py
--rw-rw-rw-   0        0        0    11775 2024-03-17 07:10:00.000000 pyzjr-1.3.4/pyzjr/nn/Metrics/semantic.py
--rw-rw-rw-   0        0        0     5310 2024-02-17 05:51:33.000000 pyzjr-1.3.4/pyzjr/nn/Summary.py
--rw-rw-rw-   0        0        0      110 2024-02-26 15:37:23.000000 pyzjr-1.3.4/pyzjr/nn/__init__.py
--rw-rw-rw-   0        0        0    84332 2024-02-22 15:45:34.000000 pyzjr-1.3.4/pyzjr/nn/functional.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/
--rw-rw-rw-   0        0        0     2908 2024-03-04 07:50:15.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/OneHot.py
--rw-rw-rw-   0        0        0      183 2024-03-11 15:59:35.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/__init__.py
--rw-rw-rw-   0        0        0     7193 2024-03-04 07:50:15.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/avgweight.py
--rw-rw-rw-   0        0        0    15225 2024-02-20 09:56:56.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/learnrate.py
--rw-rw-rw-   0        0        0    13059 2024-02-26 16:29:06.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/loss_function.py
--rw-rw-rw-   0        0        0     3779 2024-01-28 10:43:32.000000 pyzjr-1.3.4/pyzjr/nn/torchutils/loss_utils.py
--rw-rw-rw-   0        0        0     3367 2024-02-22 15:48:11.000000 pyzjr-1.3.4/pyzjr/utils.py
--rw-rw-rw-   0        0        0       21 2024-03-27 04:15:38.000000 pyzjr-1.3.4/pyzjr/version.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr/videos/
--rw-rw-rw-   0        0        0       95 2023-11-12 10:19:39.000000 pyzjr-1.3.4/pyzjr/videos/__init__.py
--rw-rw-rw-   0        0        0     3796 2024-02-19 09:13:27.000000 pyzjr-1.3.4/pyzjr/videos/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2931 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5280 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-27 04:15:45.000000 pyzjr-1.3.4/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 04:15:45.000000 pyzjr-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2133 2024-03-27 04:15:38.000000 pyzjr-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/
+-rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-04-20 07:27:26.000000 pyzjr-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/models_img/
+-rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.5/models_img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Math/
+-rw-rw-rw-   0        0        0      689 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/Numpy.py
+-rw-rw-rw-   0        0        0      212 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/__init__.py
+-rw-rw-rw-   0        0        0     3438 2024-02-20 09:48:40.000000 pyzjr-1.3.5/pyzjr/Math/arithmetic.py
+-rw-rw-rw-   0        0        0      134 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/constant.py
+-rw-rw-rw-   0        0        0     7362 2024-02-19 10:31:56.000000 pyzjr-1.3.5/pyzjr/Math/function.py
+-rw-rw-rw-   0        0        0    19620 2024-02-19 09:52:53.000000 pyzjr-1.3.5/pyzjr/Math/point_line.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/
+-rw-rw-rw-   0        0        0     2271 2024-03-04 07:16:29.000000 pyzjr-1.3.5/pyzjr/Models/Attention/A2.py
+-rw-rw-rw-   0        0        0     1927 2024-03-09 14:59:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/AFT.py
+-rw-rw-rw-   0        0        0     1911 2024-03-09 15:28:12.000000 pyzjr-1.3.5/pyzjr/Models/Attention/DANet.py
+-rw-rw-rw-   0        0        0     5412 2024-03-09 15:10:59.000000 pyzjr-1.3.5/pyzjr/Models/Attention/MobileViT.py
+-rw-rw-rw-   0        0        0     3105 2024-03-21 17:03:45.000000 pyzjr-1.3.5/pyzjr/Models/Attention/SE.py
+-rw-rw-rw-   0        0        0     1933 2024-03-09 15:18:47.000000 pyzjr-1.3.5/pyzjr/Models/Attention/ViP.py
+-rw-rw-rw-   0        0        0     1589 2024-04-20 07:26:32.000000 pyzjr-1.3.5/pyzjr/Models/Attention/__init__.py
+-rw-rw-rw-   0        0        0     4795 2024-03-09 14:59:04.000000 pyzjr-1.3.5/pyzjr/Models/Attention/acmix.py
+-rw-rw-rw-   0        0        0    12705 2024-03-09 15:00:08.000000 pyzjr-1.3.5/pyzjr/Models/Attention/axial.py
+-rw-rw-rw-   0        0        0     3180 2024-03-04 07:32:10.000000 pyzjr-1.3.5/pyzjr/Models/Attention/bam.py
+-rw-rw-rw-   0        0        0     3729 2024-03-04 12:35:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/cbam.py
+-rw-rw-rw-   0        0        0     1635 2024-03-09 15:01:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/coord.py
+-rw-rw-rw-   0        0        0     2175 2024-03-04 12:19:45.000000 pyzjr-1.3.5/pyzjr/Models/Attention/cot.py
+-rw-rw-rw-   0        0        0     2688 2024-03-09 15:02:25.000000 pyzjr-1.3.5/pyzjr/Models/Attention/crisscross.py
+-rw-rw-rw-   0        0        0    26854 2024-03-09 15:22:58.000000 pyzjr-1.3.5/pyzjr/Models/Attention/crossformer.py
+-rw-rw-rw-   0        0        0    23025 2024-03-09 15:25:56.000000 pyzjr-1.3.5/pyzjr/Models/Attention/dat.py
+-rw-rw-rw-   0        0        0     1340 2024-03-09 15:04:58.000000 pyzjr-1.3.5/pyzjr/Models/Attention/eca.py
+-rw-rw-rw-   0        0        0     3752 2024-03-09 15:05:31.000000 pyzjr-1.3.5/pyzjr/Models/Attention/emsa.py
+-rw-rw-rw-   0        0        0     1341 2024-03-09 15:06:14.000000 pyzjr-1.3.5/pyzjr/Models/Attention/external.py
+-rw-rw-rw-   0        0        0     4161 2024-03-09 15:19:38.000000 pyzjr-1.3.5/pyzjr/Models/Attention/gfnet.py
+-rw-rw-rw-   0        0        0     5444 2024-03-09 15:07:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/halo.py
+-rw-rw-rw-   0        0        0    30578 2024-03-09 15:23:53.000000 pyzjr-1.3.5/pyzjr/Models/Attention/moat.py
+-rw-rw-rw-   0        0        0     3670 2024-03-09 15:08:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/muse.py
+-rw-rw-rw-   0        0        0     2281 2024-03-09 15:11:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/outlook.py
+-rw-rw-rw-   0        0        0      985 2024-03-09 15:29:37.000000 pyzjr-1.3.5/pyzjr/Models/Attention/parnet.py
+-rw-rw-rw-   0        0        0     4087 2024-03-09 15:13:38.000000 pyzjr-1.3.5/pyzjr/Models/Attention/polarized.py
+-rw-rw-rw-   0        0        0     2296 2024-03-09 15:11:51.000000 pyzjr-1.3.5/pyzjr/Models/Attention/psa.py
+-rw-rw-rw-   0        0        0      930 2024-03-09 14:57:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/residual.py
+-rw-rw-rw-   0        0        0     2355 2024-03-09 14:52:15.000000 pyzjr-1.3.5/pyzjr/Models/Attention/s2.py
+-rw-rw-rw-   0        0        0     3084 2024-03-09 15:15:20.000000 pyzjr-1.3.5/pyzjr/Models/Attention/self_att.py
+-rw-rw-rw-   0        0        0     1784 2024-03-09 15:14:10.000000 pyzjr-1.3.5/pyzjr/Models/Attention/sge.py
+-rw-rw-rw-   0        0        0     2637 2024-03-09 15:16:05.000000 pyzjr-1.3.5/pyzjr/Models/Attention/shuffle.py
+-rw-rw-rw-   0        0        0      909 2024-03-09 15:16:39.000000 pyzjr-1.3.5/pyzjr/Models/Attention/simam.py
+-rw-rw-rw-   0        0        0     2933 2024-03-09 15:17:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/simplified_self_att.py
+-rw-rw-rw-   0        0        0     1863 2024-03-18 11:12:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/sk.py
+-rw-rw-rw-   0        0        0     2349 2024-03-09 15:18:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/triplet.py
+-rw-rw-rw-   0        0        0     2234 2024-03-04 13:24:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/ufo.py
+-rw-rw-rw-   0        0        0      220 2024-03-16 15:32:39.000000 pyzjr-1.3.5/pyzjr/Models/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-03-21 16:32:55.000000 pyzjr-1.3.5/pyzjr/Models/_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/backbone/
+-rw-rw-rw-   0        0        0     5692 2024-03-22 16:07:30.000000 pyzjr-1.3.5/pyzjr/Models/backbone/Darknet.py
+-rw-rw-rw-   0        0        0    25919 2024-02-23 14:10:01.000000 pyzjr-1.3.5/pyzjr/Models/backbone/Ghostnet.py
+-rw-rw-rw-   0        0        0     1953 2024-03-26 15:38:25.000000 pyzjr-1.3.5/pyzjr/Models/backbone/__init__.py
+-rw-rw-rw-   0        0        0     1935 2024-04-01 07:58:53.000000 pyzjr-1.3.5/pyzjr/Models/backbone/alexnet.py
+-rw-rw-rw-   0        0        0     7560 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/conv2former.py
+-rw-rw-rw-   0        0        0     6278 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/densenet.py
+-rw-rw-rw-   0        0        0    12866 2024-04-01 09:42:37.000000 pyzjr-1.3.5/pyzjr/Models/backbone/drn.py
+-rw-rw-rw-   0        0        0    17934 2024-04-01 08:53:51.000000 pyzjr-1.3.5/pyzjr/Models/backbone/efficientnet.py
+-rw-rw-rw-   0        0        0     7210 2024-04-01 09:54:02.000000 pyzjr-1.3.5/pyzjr/Models/backbone/fasternet.py
+-rw-rw-rw-   0        0        0     5623 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/googlenet.py
+-rw-rw-rw-   0        0        0     1869 2024-02-04 04:44:18.000000 pyzjr-1.3.5/pyzjr/Models/backbone/lenet.py
+-rw-rw-rw-   0        0        0     7048 2024-03-18 16:29:49.000000 pyzjr-1.3.5/pyzjr/Models/backbone/mnasnet.py
+-rw-rw-rw-   0        0        0    16395 2024-02-16 16:51:01.000000 pyzjr-1.3.5/pyzjr/Models/backbone/mobilenet.py
+-rw-rw-rw-   0        0        0     9972 2024-04-18 15:14:36.000000 pyzjr-1.3.5/pyzjr/Models/backbone/nasnet.py
+-rw-rw-rw-   0        0        0     7217 2024-03-18 11:17:15.000000 pyzjr-1.3.5/pyzjr/Models/backbone/regnet.py
+-rw-rw-rw-   0        0        0     8910 2024-04-01 09:47:10.000000 pyzjr-1.3.5/pyzjr/Models/backbone/resnet.py
+-rw-rw-rw-   0        0        0    11356 2024-03-22 15:56:05.000000 pyzjr-1.3.5/pyzjr/Models/backbone/shufflenet.py
+-rw-rw-rw-   0        0        0     4392 2024-03-04 12:30:07.000000 pyzjr-1.3.5/pyzjr/Models/backbone/squeezenet.py
+-rw-rw-rw-   0        0        0     3996 2024-02-25 16:22:54.000000 pyzjr-1.3.5/pyzjr/Models/backbone/vgg.py
+-rw-rw-rw-   0        0        0     5866 2024-04-01 09:44:12.000000 pyzjr-1.3.5/pyzjr/Models/backbone/xception.py
+-rw-rw-rw-   0        0        0     2705 2024-03-22 15:32:04.000000 pyzjr-1.3.5/pyzjr/Models/backbone/zfnet.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/bricks/
+-rw-rw-rw-   0        0        0     5577 2024-04-01 09:57:01.000000 pyzjr-1.3.5/pyzjr/Models/bricks/Initer.py
+-rw-rw-rw-   0        0        0      426 2024-04-18 15:04:29.000000 pyzjr-1.3.5/pyzjr/Models/bricks/__init__.py
+-rw-rw-rw-   0        0        0     1577 2024-03-04 09:07:17.000000 pyzjr-1.3.5/pyzjr/Models/bricks/classfier.py
+-rw-rw-rw-   0        0        0    22575 2024-03-04 07:32:10.000000 pyzjr-1.3.5/pyzjr/Models/bricks/comblock.py
+-rw-rw-rw-   0        0        0     2646 2024-03-26 15:25:44.000000 pyzjr-1.3.5/pyzjr/Models/bricks/conv_norm_act.py
+-rw-rw-rw-   0        0        0     6828 2024-03-04 12:40:27.000000 pyzjr-1.3.5/pyzjr/Models/bricks/drop.py
+-rw-rw-rw-   0        0        0     6669 2024-03-06 00:10:20.000000 pyzjr-1.3.5/pyzjr/Models/bricks/mlp.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/conv/
+-rw-rw-rw-   0        0        0     1974 2024-04-18 13:35:49.000000 pyzjr-1.3.5/pyzjr/Models/conv/Depthwise_Conv.py
+-rw-rw-rw-   0        0        0      508 2024-03-21 15:46:28.000000 pyzjr-1.3.5/pyzjr/Models/conv/Dilated_Conv.py
+-rw-rw-rw-   0        0        0     1862 2024-02-29 10:04:41.000000 pyzjr-1.3.5/pyzjr/Models/conv/Partial_Conv.py
+-rw-rw-rw-   0        0        0     2660 2024-02-29 10:02:23.000000 pyzjr-1.3.5/pyzjr/Models/conv/Ref_Conv.py
+-rw-rw-rw-   0        0        0    11458 2024-02-29 09:11:02.000000 pyzjr-1.3.5/pyzjr/Models/conv/Snake_Conv.py
+-rw-rw-rw-   0        0        0      295 2024-03-21 15:46:28.000000 pyzjr-1.3.5/pyzjr/Models/conv/__init__.py
+-rw-rw-rw-   0        0        0     3029 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/Models/networks.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/sampling/
+-rw-rw-rw-   0        0        0      754 2024-04-05 14:24:23.000000 pyzjr-1.3.5/pyzjr/Models/sampling/__init__.py
+-rw-rw-rw-   0        0        0     4857 2024-04-05 16:18:30.000000 pyzjr-1.3.5/pyzjr/Models/sampling/adaptivepooling.py
+-rw-rw-rw-   0        0        0     1393 2024-01-27 17:10:24.000000 pyzjr-1.3.5/pyzjr/Models/sampling/haarwavelet.py
+-rw-rw-rw-   0        0        0     1828 2024-03-04 13:56:06.000000 pyzjr-1.3.5/pyzjr/Models/sampling/medianpooling.py
+-rw-rw-rw-   0        0        0     4792 2024-02-26 15:35:21.000000 pyzjr-1.3.5/pyzjr/Models/sampling/standardpooling.py
+-rw-rw-rw-   0        0        0      854 2024-03-01 15:33:22.000000 pyzjr-1.3.5/pyzjr/Models/sampling/strideconv.py
+-rw-rw-rw-   0        0        0     3692 2024-02-29 15:43:47.000000 pyzjr-1.3.5/pyzjr/Models/sampling/strippooling.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/
+-rw-rw-rw-   0        0        0       70 2024-02-27 16:31:33.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/__init__.py
+-rw-rw-rw-   0        0        0    24988 2024-03-17 06:46:22.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/fcn.py
+-rw-rw-rw-   0        0        0     3289 2024-02-29 09:20:12.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/unet.py
+-rw-rw-rw-   0        0        0     6378 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0    10349 2024-02-04 05:11:03.000000 pyzjr-1.3.5/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      896 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/
+-rw-rw-rw-   0        0        0    13180 2024-04-13 15:26:35.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/Crack.py
+-rw-rw-rw-   0        0        0     8307 2024-02-29 15:56:54.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/_Steger.py
+-rw-rw-rw-   0        0        0      366 2024-02-19 10:23:26.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/__init__.py
+-rw-rw-rw-   0        0        0     7681 2024-02-18 17:28:31.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/definition.py
+-rw-rw-rw-   0        0        0     4827 2024-02-22 16:33:22.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/pixel.py
+-rw-rw-rw-   0        0        0     1685 2024-04-13 15:00:07.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/utils.py
+-rw-rw-rw-   0        0        0      116 2024-04-13 14:32:14.000000 pyzjr-1.3.5/pyzjr/augmentation/__init__.py
+-rw-rw-rw-   0        0        0    28643 2024-02-02 16:09:04.000000 pyzjr-1.3.5/pyzjr/augmentation/augments.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/
+-rw-rw-rw-   0        0        0      306 2024-02-01 16:36:53.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2192 2024-02-02 16:09:04.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/_utils.py
+-rw-rw-rw-   0        0        0     3413 2024-02-28 11:40:46.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/normal.py
+-rw-rw-rw-   0        0        0    10459 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/opencv.py
+-rw-rw-rw-   0        0        0    40632 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/pillow.py
+-rw-rw-rw-   0        0        0     6139 2024-03-21 17:03:45.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/tvision.py
+-rw-rw-rw-   0        0        0     1084 2024-03-04 06:15:09.000000 pyzjr-1.3.5/pyzjr/augmentation/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/core/
+-rw-rw-rw-   0        0        0     1105 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/__init__.py
+-rw-rw-rw-   0        0        0     6991 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/__tensor.py
+-rw-rw-rw-   0        0        0      680 2023-10-07 12:04:40.000000 pyzjr-1.3.5/pyzjr/core/_utils.py
+-rw-rw-rw-   0        0        0     1889 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/error.py
+-rw-rw-rw-   0        0        0     2692 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/general.py
+-rw-rw-rw-   0        0        0      669 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/helpers.py
+-rw-rw-rw-   0        0        0     7254 2023-11-15 11:43:15.000000 pyzjr-1.3.5/pyzjr/core/lr_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/data/
+-rw-rw-rw-   0        0        0     1486 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/data/Dataloader.py
+-rw-rw-rw-   0        0        0     9590 2024-03-08 01:06:58.000000 pyzjr-1.3.5/pyzjr/data/Dataset.py
+-rw-rw-rw-   0        0        0    12147 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/data/FM.py
+-rw-rw-rw-   0        0        0      215 2024-04-14 15:31:09.000000 pyzjr-1.3.5/pyzjr/data/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/data/basedataset.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/data/data_set/
+-rw-rw-rw-   0        0        0     9436 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/data/data_set/Pascal_voc.py
+-rw-rw-rw-   0        0        0        0 2024-02-29 16:00:47.000000 pyzjr-1.3.5/pyzjr/data/data_set/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-03-08 01:30:08.000000 pyzjr-1.3.5/pyzjr/data/data_set/config.py
+-rw-rw-rw-   0        0        0    15340 2024-04-13 15:04:54.000000 pyzjr-1.3.5/pyzjr/data/reader.py
+-rw-rw-rw-   0        0        0      934 2024-04-14 15:26:14.000000 pyzjr-1.3.5/pyzjr/data/txt_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/devices/
+-rw-rw-rw-   0        0        0      498 2024-04-18 15:41:22.000000 pyzjr-1.3.5/pyzjr/devices/__init__.py
+-rw-rw-rw-   0        0        0     1572 2024-04-13 15:22:13.000000 pyzjr-1.3.5/pyzjr/devices/get_device.py
+-rw-rw-rw-   0        0        0     2888 2024-04-18 15:41:22.000000 pyzjr-1.3.5/pyzjr/devices/measures.py
+-rw-rw-rw-   0        0        0     1202 2024-04-13 15:53:39.000000 pyzjr-1.3.5/pyzjr/devices/systeminfo.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/dlearn/
+-rw-rw-rw-   0        0        0      949 2024-03-11 15:45:28.000000 pyzjr-1.3.5/pyzjr/dlearn/__init__.py
+-rw-rw-rw-   0        0        0     8571 2024-02-17 18:07:27.000000 pyzjr-1.3.5/pyzjr/dlearn/callbacklog.py
+-rw-rw-rw-   0        0        0     8379 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/dlearn/callbacks.py
+-rw-rw-rw-   0        0        0     1051 2024-03-11 15:59:35.000000 pyzjr-1.3.5/pyzjr/dlearn/savemodels.py
+-rw-rw-rw-   0        0        0     4801 2024-03-11 15:21:20.000000 pyzjr-1.3.5/pyzjr/dlearn/strategy.py
+-rw-rw-rw-   0        0        0     5955 2024-04-13 15:28:23.000000 pyzjr-1.3.5/pyzjr/dlearn/tools.py
+-rw-rw-rw-   0        0        0     7360 2024-03-11 16:12:42.000000 pyzjr-1.3.5/pyzjr/dlearn/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/
+-rw-rw-rw-   0        0        0      385 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/__init__.py
+-rw-rw-rw-   0        0        0    16237 2024-02-08 15:56:55.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/classification.py
+-rw-rw-rw-   0        0        0    11775 2024-03-17 07:10:00.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/semantic.py
+-rw-rw-rw-   0        0        0     9459 2024-04-18 15:17:33.000000 pyzjr-1.3.5/pyzjr/nn/Summary.py
+-rw-rw-rw-   0        0        0      123 2024-04-18 15:17:33.000000 pyzjr-1.3.5/pyzjr/nn/__init__.py
+-rw-rw-rw-   0        0        0    84332 2024-02-22 15:45:34.000000 pyzjr-1.3.5/pyzjr/nn/functional.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/
+-rw-rw-rw-   0        0        0     2908 2024-03-04 07:50:15.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/OneHot.py
+-rw-rw-rw-   0        0        0      183 2024-03-11 15:59:35.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/__init__.py
+-rw-rw-rw-   0        0        0     7193 2024-03-04 07:50:15.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/avgweight.py
+-rw-rw-rw-   0        0        0    15225 2024-02-20 09:56:56.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/learnrate.py
+-rw-rw-rw-   0        0        0    13059 2024-02-26 16:29:06.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/loss_function.py
+-rw-rw-rw-   0        0        0     3779 2024-01-28 10:43:32.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/loss_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/torch3D/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:38:41.000000 pyzjr-1.3.5/pyzjr/torch3D/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/torch3D/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:38:57.000000 pyzjr-1.3.5/pyzjr/torch3D/networks/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-20 07:26:32.000000 pyzjr-1.3.5/pyzjr/version.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/
+-rw-rw-rw-   0        0        0      410 2024-04-14 15:13:36.000000 pyzjr-1.3.5/pyzjr/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/color/
+-rw-rw-rw-   0        0        0     1418 2024-04-13 14:47:13.000000 pyzjr-1.3.5/pyzjr/visualize/color/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-04-13 14:43:57.000000 pyzjr-1.3.5/pyzjr/visualize/color/colormap.py
+-rw-rw-rw-   0        0        0     3339 2023-11-04 05:34:46.000000 pyzjr-1.3.5/pyzjr/visualize/color/colorspace.py
+-rw-rw-rw-   0        0        0     7471 2024-04-13 14:47:13.000000 pyzjr-1.3.5/pyzjr/visualize/color/cvplot.py
+-rw-rw-rw-   0        0        0     7937 2024-04-13 15:27:09.000000 pyzjr-1.3.5/pyzjr/visualize/color/findcolor.py
+-rw-rw-rw-   0        0        0     1066 2024-02-13 17:07:55.000000 pyzjr-1.3.5/pyzjr/visualize/color/hex.py
+-rw-rw-rw-   0        0        0    10985 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/visualize/io.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/
+-rw-rw-rw-   0        0        0     6556 2024-04-14 15:13:36.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/HandTrack.py
+-rw-rw-rw-   0        0        0      376 2024-01-25 07:15:10.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/__init__.py
+-rw-rw-rw-   0        0        0      631 2024-02-04 05:11:03.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/const.py
+-rw-rw-rw-   0        0        0     4327 2024-04-13 15:04:54.000000 pyzjr-1.3.5/pyzjr/visualize/printf.py
+-rw-rw-rw-   0        0        0     3367 2024-02-22 15:48:11.000000 pyzjr-1.3.5/pyzjr/visualize/utils.py
+-rw-rw-rw-   0        0        0     3796 2024-02-19 09:13:27.000000 pyzjr-1.3.5/pyzjr/visualize/video_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5460 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 07:27:26.000000 pyzjr-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2133 2024-04-20 07:27:04.000000 pyzjr-1.3.5/setup.py
```

### Comparing `pyzjr-1.3.4/LICENSE` & `pyzjr-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/PKG-INFO` & `pyzjr-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.4
+Version: 1.3.5
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.4/README.md` & `pyzjr-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Math/Numpy.py` & `pyzjr-1.3.5/pyzjr/Math/Numpy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import numpy as np
-
-npi = 3.141592653589793
-n2pi = 2 * npi
+from pyzjr.Math.constant import n2pi
 
 def rand(a=0., b=1.):
     """
     生成在指定范围内的随机浮点数,进行缩放和偏移来映射到[a, b)的范围
     a: 下界; b: 上界
     """
     return np.random.rand() * (b - a) + a
```

### Comparing `pyzjr-1.3.4/pyzjr/Math/arithmetic.py` & `pyzjr-1.3.5/pyzjr/Math/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Math/function.py` & `pyzjr-1.3.5/pyzjr/Math/function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Math/point_line.py` & `pyzjr-1.3.5/pyzjr/Math/point_line.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/A2.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/A2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/AFT.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/AFT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/DANet.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/DANet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/MobileViT.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/MobileViT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/SE.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/SE.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/ViP.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/ViP.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/__init__.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .A2 import DoubleAttention
 from .bam import BAMAttention
 from .cbam import CBAMAttention, LightCBAMAttention
 from .se import SEAttention, EffectiveSEAttention, SqueezeExcitation
 from .ufo import UFOAttention
 from .cot import CoTAttention
 
-__all__ = ["BAMAttention", "SEAttention", "SqueezeExcitation", "EffectiveSEAttention",
-           "CBAMAttention", "LightCBAMAttention", "DoubleAttention", "UFOAttention",
-           "CoTAttention"]
+# __all__ = ["BAMAttention", "SEAttention", "SqueezeExcitation", "EffectiveSEAttention",
+#            "CBAMAttention", "LightCBAMAttention", "DoubleAttention", "UFOAttention",
+#            "CoTAttention"]
 
 from .s2 import S2Attention
 from .residual import ResidualAttention
 from .acmix import ACmixAttention
 from .AFT import AFT_FULL
 from .axial import AxialAttention, AxialImageTransformer
 from .coord import CoordAttention
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/acmix.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/acmix.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/axial.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/axial.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/bam.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/bam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/cbam.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/cbam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/coord.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/coord.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/cot.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/cot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/crisscross.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/crisscross.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/crossformer.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/crossformer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/dat.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/dat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/eca.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/eca.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/emsa.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/emsa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/external.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/external.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/gfnet.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/gfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/halo.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/halo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/moat.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/moat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/muse.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/muse.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/outlook.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/outlook.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/parnet.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/parnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/polarized.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/polarized.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/psa.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/psa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/residual.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/residual.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/s2.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/s2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/self_att.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/sge.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/sge.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/shuffle.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/shuffle.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/simam.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/simam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/simplified_self_att.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/simplified_self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/sk.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/sk.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/triplet.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/triplet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/Attention/ufo.py` & `pyzjr-1.3.5/pyzjr/Models/Attention/ufo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/_utils.py` & `pyzjr-1.3.5/pyzjr/Models/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/Darknet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/Darknet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/Ghostnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/Ghostnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/__init__.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/alexnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/alexnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """
+Copyright (c) 2023, Auorui.
+All rights reserved.
+
 论文原址： <https://proceedings.neurips.cc/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf>
 ImageNet Classification with Deep Convolutional Neural Networks
 """
 import torch
 import torch.nn as nn
 
 __all__ = ['AlexNet']
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/conv2former.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/conv2former.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/densenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/densenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/drn.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/drn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Dilated Residual Networks
     <https://arxiv.org/pdf/1705.09914.pdf>
+code from: https://github.com/fyu/drn/blob/master/drn.py
 """
 import math
 import torch
 import torch.nn as nn
 
 __all__ = ["DRN", "DRN_A", "drn_a_50", "drn_c_26", "drn_c_42", "drn_c_58", "drn_d_22", "drn_d_24",
            "drn_d_38", "drn_d_40", "drn_d_54", "drn_d_56", "drn_d_105", "drn_d_107"]
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/efficientnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/fasternet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/fasternet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Paper address: <https://arxiv.org/pdf/2303.03667.pdf>
+Run, Don’t Walk: Chasing Higher FLOPS for Faster Neural Networks
+    <https://arxiv.org/pdf/2303.03667.pdf>
 Reference from: https://github.com/JierunChen/FasterNet/blob/master/models/fasternet.py
 Blog records: https://blog.csdn.net/m0_62919535/article/details/136334105
 """
 import torch
 import torch.nn as nn
 from pyzjr.Models.bricks import DropPath
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/googlenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/googlenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/lenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/lenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/mnasnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/mnasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/mobilenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/regnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/resnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/resnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,66 @@
 """
-论文原址： <https://arxiv.org/pdf/1512.03385.pdf>
 Deep Residual Learning for Image Recognition
-resnet50, resnet101, resnet152
+    <https://arxiv.org/pdf/1512.03385.pdf>
+resnet18, resnet34, resnet50, resnet101, resnet152
+(Optional addition of SE module)
+
+Blog records: https://blog.csdn.net/m0_62919535/article/details/132384303
 """
 import torch
 import torch.nn as nn
+from pyzjr.Models.attention import SEAttention
+from pyzjr.Models.bricks import ConvBnReLU, ConvBn
 
 __all__ = ["ResNet", 'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152']
 
-class ConvBNReLU(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size=3, stride=1, padding=1):
-        super(ConvBNReLU, self).__init__()
-        self.conv = nn.Conv2d(in_channels=in_channels, out_channels=out_channels, kernel_size=kernel_size, stride=stride, padding=padding)
-        self.bn = nn.BatchNorm2d(num_features=out_channels)
-        self.relu = nn.ReLU(inplace=True)
-
-    def forward(self, x):
-        x = self.conv(x)
-        x = self.bn(x)
-        x = self.relu(x)
-        return x
-
-class ConvBN(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size=3, stride=1, padding=1):
-        super(ConvBN, self).__init__()
-        self.conv = nn.Conv2d(in_channels=in_channels, out_channels=out_channels, kernel_size=kernel_size, stride=stride, padding=padding)
-        self.bn = nn.BatchNorm2d(num_features=out_channels)
-
-    def forward(self, x):
-        x = self.conv(x)
-        x = self.bn(x)
-        return x
-
 def conv3x3(in_channels, out_channels, stride=1, groups=1, dilation=1):
     """3x3 convolution with padding:捕捉局部特征和空间相关性，学习更复杂的特征和抽象表示"""
     return nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=stride,
                      padding=dilation, groups=groups, bias=False, dilation=dilation)
 
 def conv1x1(in_channels, out_channels, stride=1):
     """1x1 convolution:实现降维或升维，调整通道数和执行通道间的线性变换"""
     return nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
 
 class BasicBlock(nn.Module):
     expansion = 1
-    def __init__(self, in_channels, out_channels, stride=1, downsample=None):
+    def __init__(self, in_channels, out_channels, stride=1, downsample=None, reduction=16, attn=False):
         super(BasicBlock, self).__init__()
-        self.convbnrelu1 = ConvBNReLU(in_channels, out_channels, kernel_size=3, stride=stride)
-        self.convbn1 = ConvBN(out_channels, out_channels, kernel_size=3)
+        self.convbnrelu1 = ConvBnReLU(in_channels, out_channels, kernel_size=3, stride=stride)
+        self.convbn1 = ConvBn(out_channels, out_channels, kernel_size=3)
         self.relu = nn.ReLU(inplace=True)
         self.downsample = downsample
         self.stride = stride
+        self.se = SEAttention(out_channels, reduction)
+        self.attn = attn
         self.conv_down = nn.Sequential(
             conv1x1(in_channels, out_channels * self.expansion, self.stride),
             nn.BatchNorm2d(out_channels * self.expansion),
         )
 
     def forward(self, x):
         residual = x
         out = self.convbnrelu1(x)
         out = self.convbn1(out)
+        if self.attn:
+            out = self.se(out)
 
         if self.downsample:
             residual = self.conv_down(x)
 
         out += residual
         out = self.relu(out)
 
         return out
 
 
 class Bottleneck(nn.Module):
     expansion = 4
-    def __init__(self, in_channels, out_channels, stride=1, downsample=None):
+    def __init__(self, in_channels, out_channels, stride=1, downsample=None, reduction=16, attn=False):
         super(Bottleneck, self).__init__()
         groups = 1
         base_width = 64
         dilation = 1
 
         width = int(out_channels * (base_width / 64.)) * groups   # wide = out_channels
         self.conv1 = conv1x1(in_channels, width)       # 降维通道数
@@ -83,14 +68,16 @@
         self.conv2 = conv3x3(width, width, stride, groups, dilation)
         self.bn2 = nn.BatchNorm2d(width)
         self.conv3 = conv1x1(width, out_channels * self.expansion)   # 升维通道数
         self.bn3 = nn.BatchNorm2d(out_channels * self.expansion)
         self.relu = nn.ReLU(inplace=True)
         self.downsample = downsample
         self.stride = stride
+        self.se = SEAttention(out_channels * self.expansion, reduction)
+        self.attn = attn
         self.conv_down = nn.Sequential(
             conv1x1(in_channels, out_channels * self.expansion, self.stride),
             nn.BatchNorm2d(out_channels * self.expansion),
         )
 
     def forward(self, x):
         residual = x
@@ -102,22 +89,33 @@
         out = self.conv2(out)
         out = self.bn2(out)
         out = self.relu(out)
 
         out = self.conv3(out)
         out = self.bn3(out)
 
+        if self.attn:
+            out = self.se(out)
+
         if self.downsample:
             residual = self.conv_down(x)
 
         out += residual
         out = self.relu(out)
 
         return out
 
+class SEBasicBlock(BasicBlock):
+    def __init__(self, in_channels, out_channels, stride=1, downsample=None, reduction=16):
+        super(SEBasicBlock, self).__init__(in_channels, out_channels, stride, downsample, reduction, attn=True)
+
+class SEBottleneck(Bottleneck):
+    def __init__(self, in_channels, out_channels, stride=1, downsample=None, reduction=16):
+        super(SEBottleneck, self).__init__(in_channels, out_channels, stride, downsample, reduction, attn=True)
+
 class ResNet(nn.Module):
     def __init__(self, block, layers, num_classes=1000, zero_init_residual=False,
                  groups=1, width_per_group=64):
         super(ResNet, self).__init__()
 
         self.inplanes = 64
         self.dilation = 1
@@ -182,33 +180,38 @@
 
         x = self.avgpool(x)
         x = torch.flatten(x, 1)
         x = self.fc(x)
 
         return x
 
-def resnet18(num_classes, **kwargs):
-    return ResNet(BasicBlock, [2, 2, 2, 2], num_classes=num_classes, **kwargs)
-
-def resnet34(num_classes, **kwargs):
-    return ResNet(BasicBlock, [3, 4, 6, 3], num_classes=num_classes, **kwargs)
-
-def resnet50(num_classes, **kwargs):
-    return ResNet(Bottleneck, [3, 4, 6, 3], num_classes=num_classes, **kwargs)
-
-def resnet101(num_classes, **kwargs):
-    return ResNet(Bottleneck, [3, 4, 23, 3], num_classes=num_classes, **kwargs)
-
-def resnet152(num_classes, **kwargs):
-    return ResNet(Bottleneck, [3, 8, 36, 3], num_classes=num_classes, **kwargs)
+def resnet18(num_classes, use_se=False, **kwargs):
+    block = SEBasicBlock if use_se else BasicBlock
+    return ResNet(block, [2, 2, 2, 2], num_classes=num_classes, **kwargs)
+
+def resnet34(num_classes, use_se=False, **kwargs):
+    block = SEBasicBlock if use_se else BasicBlock
+    return ResNet(block, [3, 4, 6, 3], num_classes=num_classes, **kwargs)
+
+def resnet50(num_classes, use_se=False, **kwargs):
+    block = SEBottleneck if use_se else Bottleneck
+    return ResNet(block, [3, 4, 6, 3], num_classes=num_classes, **kwargs)
+
+def resnet101(num_classes, use_se=False, **kwargs):
+    block = SEBottleneck if use_se else Bottleneck
+    return ResNet(block, [3, 4, 23, 3], num_classes=num_classes, **kwargs)
+
+def resnet152(num_classes, use_se=False, **kwargs):
+    block = SEBottleneck if use_se else Bottleneck
+    return ResNet(block, [3, 8, 36, 3], num_classes=num_classes, **kwargs)
 
 if __name__=="__main__":
     import torchsummary
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     input = torch.ones(2, 3, 224, 224).to(device)
-    net = resnet50(num_classes=4)
+    net = resnet34(num_classes=4, use_se=True)
     net = net.to(device)
     out = net(input)
     print(out)
     print(out.shape)
     torchsummary.summary(net, input_size=(3, 224, 224))
     # 50 Total params: 23,516,228
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/shufflenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/shufflenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/squeezenet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/vgg.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/xception.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/xception.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,185 @@
 """
+Copyright (c) 2023, Auorui.
+All rights reserved.
+
 Xception: Deep Learning with Depthwise Separable Convolutions
     <https://arxiv.org/pdf/1610.02357.pdf>
+
+Blog records: https://blog.csdn.net/m0_62919535/article/details/137065439
 """
 import torch
 import torch.nn as nn
 
+__all__ = ["Xception"]
+
 class SeparableConv2d(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=1, bias=False):
-        super(SeparableConv2d,self).__init__()
+    def __init__(self, in_channels, out_channels, kernel_size=3, stride=1, padding=0, dilation=1, bias=False):
+        super(SeparableConv2d, self).__init__()
         self.conv = nn.Conv2d(in_channels, in_channels, kernel_size, stride, padding,
                                dilation, groups=in_channels, bias=bias)
         self.pointwise = nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0,
                                    dilation=1, groups=1, bias=False)
 
-    def forward(self,x):
+    def forward(self, x):
         x = self.conv(x)
         x = self.pointwise(x)
         return x
 
-class Block(nn.Module):
-    def __init__(self, in_channels, out_channels, num_conv, strides=1, start_with_relu=True, channel_change=True):
-        super(Block, self).__init__()
-
-        if out_channels != in_channels or strides != 1:
-            self.shutcut = nn.Sequential(
-                nn.Conv2d(in_channels, out_channels, 1, stride=strides, bias=False),
-                nn.BatchNorm2d(out_channels)
-            )
-        else:
-            self.shutcut = nn.Sequential()
+class EntryFlow(nn.Module):
+    def __init__(self):
+        super(EntryFlow, self).__init__()
+
+        self.headconv = nn.Sequential(
+            nn.Conv2d(3, 32, 3, 2, bias=False),
+            nn.BatchNorm2d(32),
+            nn.ReLU(inplace=True),
+
+            nn.Conv2d(32, 64, 3, bias=False),
+            nn.BatchNorm2d(64),
+            nn.ReLU(inplace=True),
+        )
 
-        layers = []
-        channels = in_channels
+        self.residual_block1 = nn.Sequential(
+            SeparableConv2d(64, 128, 3, padding=1),
+            nn.BatchNorm2d(128),
+            nn.ReLU(inplace=True),
+            SeparableConv2d(128, 128, 3, padding=1),
+            nn.BatchNorm2d(128),
+            nn.MaxPool2d(3, stride=2, padding=1),
+        )
 
-        if channel_change:
-            layers.append(nn.ReLU(inplace=True))
-            layers.append(SeparableConv2d(in_channels, out_channels, 3, stride=1, padding=1))
-            layers.append(nn.BatchNorm2d(out_channels))
-            channels = out_channels
-
-        for i in range(num_conv - 1):
-            layers.append(nn.ReLU(inplace=True))
-            layers.append(SeparableConv2d(channels, channels, 3, stride=1, padding=1))
-            layers.append(nn.BatchNorm2d(channels))
-
-        if not channel_change:
-            layers.append(nn.ReLU(inplace=True))
-            layers.append(SeparableConv2d(in_channels, out_channels, 3, stride=1, padding=1))
-            layers.append(nn.BatchNorm2d(out_channels))
-
-        if start_with_relu:
-            layers = layers
-        else:
-            layers = layers[1:]
+        self.residual_block2 = nn.Sequential(
+            nn.ReLU(inplace=True),
+            SeparableConv2d(128, 256, 3, padding=1),
+            nn.BatchNorm2d(256),
+            nn.ReLU(inplace=True),
+            SeparableConv2d(256, 256, 3, padding=1),
+            nn.BatchNorm2d(256),
+            nn.MaxPool2d(3, stride=2, padding=1)
+        )
 
-        if strides != 1:
-            layers.append(nn.MaxPool2d(3, strides, 1))
+        self.residual_block3 = nn.Sequential(
+            nn.ReLU(inplace=True),
+            SeparableConv2d(256, 728, 3, padding=1),
+            nn.BatchNorm2d(728),
+            nn.ReLU(inplace=True),
+            SeparableConv2d(728, 728, 3, padding=1),
+            nn.BatchNorm2d(728),
+            nn.MaxPool2d(3, stride=2, padding=1)
+        )
 
-        self.layers = nn.Sequential(*layers)
+    def shortcut(self, inp, oup):
+        return nn.Sequential(
+            nn.Conv2d(inp, oup, 1, 2, bias=False),
+            nn.BatchNorm2d(oup)
+            )
 
     def forward(self, x):
-        layer = self.layers(x)
-        shutcut = self.shutcut(x)
-        out = layer + shutcut
-        return out
+        x = self.headconv(x)
+        residual = self.residual_block1(x)
+        shortcut_block1 = self.shortcut(64, 128)
+        x = residual + shortcut_block1(x)
+        residual = self.residual_block2(x)
+        shortcut_block2 = self.shortcut(128, 256)
+        x = residual + shortcut_block2(x)
+        residual = self.residual_block3(x)
+        shortcut_block3 = self.shortcut(256, 728)
+        x = residual + shortcut_block3(x)
 
+        return x
 
-class Xception(nn.Module):
-    def __init__(self, num_classes=1000):
-        super(Xception, self).__init__()
-        self.num_classes = num_classes
+class MiddleFlow(nn.Module):
+    def __init__(self):
+        super(MiddleFlow, self).__init__()
 
-        # Entry flow
-        self.entry_flow = nn.Sequential(
-            nn.Conv2d(3, 32, 3, 2, bias=False),
-            nn.BatchNorm2d(32),
+        self.shortcut = nn.Sequential()
+        self.conv1 = nn.Sequential(
             nn.ReLU(inplace=True),
+            SeparableConv2d(728, 728, 3, padding=1),
+            nn.BatchNorm2d(728),
 
-            nn.Conv2d(32, 64, 3, bias=False),
-            nn.BatchNorm2d(64),
             nn.ReLU(inplace=True),
+            SeparableConv2d(728, 728, 3, padding=1),
+            nn.BatchNorm2d(728),
 
-            Block(64, 128, 2, 2, start_with_relu=False, channel_change=True),
-            Block(128, 256, 2, 2, start_with_relu=True, channel_change=True),
-            Block(256, 728, 2, 2, start_with_relu=True, channel_change=True),
-        )
-
-        # Middle flow
-        self.middle_flow = nn.Sequential(
-            # repeated 8 times
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-            Block(728, 728, 3, 1, start_with_relu=True, channel_change=True),
-        )
-
-        # Exit flow
-        self.exit_flow = nn.Sequential(
-            Block(728, 1024, 2, 2, start_with_relu=True, channel_change=False),
+            nn.ReLU(inplace=True),
+            SeparableConv2d(728, 728, 3, padding=1),
+            nn.BatchNorm2d(728)
+        )
+
+    def forward(self, x):
+        residual = self.conv1(x)
+        input = self.shortcut(x)
+        return input + residual
+
+class ExitFlow(nn.Module):
+    def __init__(self):
+        super(ExitFlow, self).__init__()
 
+        self.residual_with_exit = nn.Sequential(
+            nn.ReLU(inplace=True),
+            SeparableConv2d(728, 728, 3, padding=1),
+            nn.BatchNorm2d(728),
+            nn.ReLU(inplace=True),
+            SeparableConv2d(728, 1024, 3, padding=1),
+            nn.BatchNorm2d(1024),
+            nn.MaxPool2d(3, stride=2, padding=1)
+        )
+
+        self.endconv = nn.Sequential(
             SeparableConv2d(1024, 1536, 3, 1, 1),
             nn.BatchNorm2d(1536),
             nn.ReLU(inplace=True),
 
             SeparableConv2d(1536, 2048, 3, 1, 1),
             nn.BatchNorm2d(2048),
             nn.ReLU(inplace=True),
 
             nn.AdaptiveAvgPool2d((1, 1)),
         )
 
+    def shortcut(self, inp, oup):
+        return nn.Sequential(
+            nn.Conv2d(inp, oup, 1, 2, bias=False),
+            nn.BatchNorm2d(oup)
+        )
+
+    def forward(self, x):
+        residual = self.residual_with_exit(x)
+        shortcut_block = self.shortcut(728, 1024)
+        output = residual + shortcut_block(x)
+        return self.endconv(output)
+
+
+class Xception(nn.Module):
+    def __init__(self, num_classes=1000):
+        super().__init__()
+        self.num_classes = num_classes
+
+        self.entry_flow = EntryFlow()
+        self.middle_flow = MiddleFlow()
+        self.exit_flow = ExitFlow()
         self.fc = nn.Linear(2048, num_classes)
 
     def forward(self, x):
         x = self.entry_flow(x)
-        x = self.middle_flow(x)
+        for i in range(8):
+            # Repeated 8 times
+            x = self.middle_flow(x)
         x = self.exit_flow(x)
-
         x = x.view(x.size(0), -1)
         out = self.fc(x)
+
         return out
 
 if __name__=='__main__':
     import torchsummary
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     input = torch.ones(2, 3, 224, 224).to(device)
     net = Xception(num_classes=4)
     net = net.to(device)
     out = net(input)
     print(out)
     print(out.shape)
     torchsummary.summary(net, input_size=(3, 224, 224))
-    # Xception Total params: 20,815,148
+    # Xception Total params: 19,838,076
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/backbone/zfnet.py` & `pyzjr-1.3.5/pyzjr/Models/backbone/zfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/Initer.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/Initer.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 
     # Clamp to ensure it's in the proper range
     tensor.clamp_(min=a, max=b)
     return tensor
 
 
 def trunc_normal_(tensor, mean=0., std=1., a=-2., b=2.):
-    # type: (Tensor, float, float, float, float) -> Tensor
     r"""Fills the input Tensor with values drawn from a truncated
     normal distribution. The values are effectively drawn from the
     normal distribution :math:`\mathcal{N}(\text{mean}, \text{std}^2)`
     with values outside :math:`[a, b]` redrawn until they are within
     the bounds. The method used for generating the random values works
     best when :math:`a \leq \text{mean} \leq b`.
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/classfier.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/classfier.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/comblock.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/comblock.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/conv_norm_act.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/conv_norm_act.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/drop.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/bricks/mlp.py` & `pyzjr-1.3.5/pyzjr/Models/bricks/mlp.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/conv/Depthwise_Conv.py` & `pyzjr-1.3.5/pyzjr/Models/conv/Depthwise_Conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         super().__init__(in_channels, out_channels, kernel_size, stride, padding, groups=math.gcd(in_channels, out_channels))
 
 class PWConv(nn.Conv2d):
     # Point-wise convolution class
     def __init__(self, in_channels, out_channels):
         super().__init__(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False)
 
-
 class DepthSepConv(nn.Module):
     """
     深度可分卷积: DW卷积 + PW卷积
     dw卷积, 当分组个数等于输入通道数时, 输出矩阵的通道输也变成了输入通道数
     pw卷积, 使用了1x1的卷积核与普通的卷积一样
     """
     def __init__(self, in_channels, out_channels, stride):
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/conv/Partial_Conv.py` & `pyzjr-1.3.5/pyzjr/Models/conv/Partial_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/conv/Ref_Conv.py` & `pyzjr-1.3.5/pyzjr/Models/conv/Ref_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/conv/Snake_Conv.py` & `pyzjr-1.3.5/pyzjr/Models/conv/Snake_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/networks.py` & `pyzjr-1.3.5/pyzjr/Models/networks.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     elif name == 'conv2former_s':
         net = Conv2Former_s(num_classes=num_classes)
     elif name == 'conv2former_l':
         net = Conv2Former_l(num_classes=num_classes)
     elif name == 'conv2former_b':
         net = Conv2Former_b(num_classes=num_classes)
     elif name == 'se_resnet18':
-        net = se_resnet18(num_classes=num_classes)
+        net = resnet18(num_classes=num_classes, use_se=True)
     elif name == 'se_resnet34':
-        net = se_resnet34(num_classes=num_classes)
+        net = resnet34(num_classes=num_classes, use_se=True)
     elif name == 'se_resnet50':
-        net = se_resnet50(num_classes=num_classes)
+        net = resnet50(num_classes=num_classes, use_se=True)
     elif name == 'se_resnet101':
-        net = se_resnet101(num_classes=num_classes)
+        net = resnet101(num_classes=num_classes, use_se=True)
     elif name == 'se_resnet152':
-        net = se_resnet152(num_classes=num_classes)
+        net = resnet152(num_classes=num_classes, use_se=True)
     else:
         print('the network name you have entered is not supported yet')
         sys.exit()
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     net.to(device)
 
     if weights != '':
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/__init__.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,13 @@
     AdaptiveCatAvgMaxPool2d, AdaptiveAvgMaxPool2d, FastAdaptiveAvgPool2d, SelectAdaptivePool2d
 from .standardpooling import MaxPool2d, AvgPool2d
 from .haarwavelet import HWDownsampling
 from .strideconv import StridedConv
 from .strippooling import StripPooling
 from .medianpooling import MedianPool2d
 
-
 # Downsampling processing module
 
 __all__ = ["adaptive_pool2d", "adaptive_avgmax_pool2d", "adaptive_catavgmax_pool2d",
            "AdaptiveAvgMaxPool2d", "AdaptiveCatAvgMaxPool2d", "FastAdaptiveAvgPool2d",
            "SelectAdaptivePool2d", "MaxPool2d", "AvgPool2d", "HWDownsampling", "StridedConv",
            "StripPooling", "MedianPool2d"]
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/adaptivepooling.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/adaptivepooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Copyright (c) 2024, Auorui.
 All rights reserved.
 Time: 2024-01-12 16:14
 
-组合池化, 并且有 ’可选择类型‘
+组合池化, 并且有  ’ 可选择类型 ‘
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 def adaptive_pool2d(input_tensor, output_size, pool_type='max'):
     """
@@ -88,27 +88,29 @@
 
     def forward(self, x):
         return adaptive_catavgmax_pool2d(x, self.output_size)
 
 class FastAdaptiveAvgPool2d(nn.Module):
     """
     自定义的自适应平均池化层
+
     Args:
         - flatten: 是否对结果进行扁平化
     """
     def __init__(self, flatten=False):
         super(FastAdaptiveAvgPool2d, self).__init__()
         self.flatten = flatten
 
     def forward(self, x):
         return x.mean((2, 3)) if self.flatten else x.mean((2, 3), keepdim=True)
 
 
 class SelectAdaptivePool2d(nn.Module):
-    """Selectable global pooling layer with dynamic input kernel size
+    """
+    Selectable global pooling layer with dynamic input kernel size
     """
     def __init__(self, output_size=1, pool_type='fast', flatten=False):
         super(SelectAdaptivePool2d, self).__init__()
         self.pool_type = pool_type or ''  # convert other falsy values to empty string for consistent TS typing
         self.flatten = flatten
         if pool_type == '':
             self.pool = nn.Identity()  # pass through
```

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/haarwavelet.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/haarwavelet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/medianpooling.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/medianpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/standardpooling.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/standardpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/strideconv.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/strideconv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/sampling/strippooling.py` & `pyzjr-1.3.5/pyzjr/Models/sampling/strippooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/segmentation/fcn.py` & `pyzjr-1.3.5/pyzjr/Models/segmentation/fcn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/Models/segmentation/unet.py` & `pyzjr-1.3.5/pyzjr/Models/segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/PIC.py` & `pyzjr-1.3.5/pyzjr/PIC.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,14 @@
 import pyzjr.Z as Z
 from pyzjr.Math import *
 from skimage.morphology import disk
 from skimage.filters import rank
 from skimage import measure
 from torchvision import transforms
 
-# def repairImg(img, hsvval, r=5,flags=Z.repair_NS):
-#     """
-#     * 用于修复图像
-#     :param img: 输入图像
-#     :param hsvval: hsv值,[[hmin, smin, vmin], [hmax, smax, vma]]
-#     :param r: 修复半径，即掩膜的像素周围需要参考的区域半径
-#     :param flags: 修复算法的标志,有Z.repair_NS、Z.repair_TELEA,默认为Z.repair_NS
-#     :param mode: 是否采用HSV例模式,默认为0,自定义模式,可通过Color下的TrackBar文件中获得
-#     :return: 返回修复后的图片,以及检测到物体
-#     """
-#     ColF=ColorFind()
-#     imgResult, mask = ColF.MaskZone(img, hsvval)
-#     dst = cv2.inpaint(img, mask, r, flags)
-#     return dst, imgResult
-
 
 def getContours(img, cThr=(100, 100), minArea=1000, filter=0, draw=True):
     """
     :param img: 输入图像
     :param cThr: 阈值
     :param minArea: 更改大小
     :param filter: 过滤
```

### Comparing `pyzjr-1.3.4/pyzjr/Z.py` & `pyzjr-1.3.5/pyzjr/Z.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Color/colorspace.py` & `pyzjr-1.3.5/pyzjr/visualize/color/colorspace.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Color/cvplot.py` & `pyzjr-1.3.5/pyzjr/visualize/color/cvplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import cv2
 import numpy as np
 import pyzjr.Z as Z
 
-__all__ = ["OverlayPng", "putBoxText", "cornerRect", "cvt2Center", "cvt2Corner", "AddText", "DrawPolygon", "DrawBboxPolygon"]
+__all__ = ["OverlayPng", "putBoxText", "cornerRect", "cvt2Center",
+           "cvt2Corner", "AddText", "DrawPolygon", "DrawBboxPolygon"]
 
 def OverlayPng(imgBack, imgFront, pos=(0, 0)):
     """
     叠加显示图片
     :param imgBack: 背景图像,无格式要求,3通道
     :param imgFront: png前置图片,读取方式必须使用 cv2.IMREAD_UNCHANGED = -1
     :param pos: 摆放位置
@@ -185,15 +186,14 @@
         plot_y,
         color=white,
         thickness=5,
     )
     img = cv2.rectangle(img, (xmin, ymin), (xmax, ymax), color=bboxcolor)
     return img
 
-
 """
            _oo0oo_
           o8888888o
           88" . "88
           (| -_- |)
           0\  =  /0
         ___/`---'\___
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Color/findcolor.py` & `pyzjr-1.3.5/pyzjr/visualize/color/findcolor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 All rights reserved.
 
 This module is based on HSV for color detection.
 """
 import cv2
 import numpy as np
 import logging
-from pyzjr.videos.utils import VideoCap
+from pyzjr.visualize.video_utils import VideoCap
 import pyzjr.Z as Z
 
 def empty(a):
     pass
 
 class ColorFind():
     def __init__(self, trackBar=False, name="Bars"):
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Color/hex.py` & `pyzjr-1.3.5/pyzjr/visualize/color/hex.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Pixel/Crack.py` & `pyzjr-1.3.5/pyzjr/augmentation/Pixel/Crack.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 in the semantic segmentation graph of neural networks.
 """
 import cv2
 import numpy as np
 
 import string
 import os
-from skimage.filters import threshold_otsu,median
-from skimage.morphology import skeletonize,dilation,disk
+from skimage.filters import threshold_otsu, median
+from skimage.morphology import skeletonize, dilation, disk
 from skimage import io, morphology, measure
 
 from pyzjr.augmentation.Pixel import SkeletonMap, incircle
-from pyzjr.augmentation.Color import putBoxText
+from pyzjr.visualize.color import putBoxText
 
 
 # 裂缝类型
 class CrackType():
     """直方图投影法推断裂缝类型,仅仅能区分线性裂缝和网状裂缝"""
     def __init__(self, threshold=3, HWratio=10, Histratio=0.5):
         """
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Pixel/_Steger.py` & `pyzjr-1.3.5/pyzjr/augmentation/Pixel/_Steger.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Pixel/definition.py` & `pyzjr-1.3.5/pyzjr/augmentation/Pixel/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Pixel/pixel.py` & `pyzjr-1.3.5/pyzjr/augmentation/Pixel/pixel.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/Pixel/utils.py` & `pyzjr-1.3.5/pyzjr/augmentation/Pixel/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math
 import cv2
 import numpy as np
 
 from skimage.morphology import medial_axis
 from scipy.ndimage import distance_transform_edt
 
 __all__ = ["DistanceTransform"]
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/augments.py` & `pyzjr-1.3.5/pyzjr/augmentation/augments.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/transforms/_utils.py` & `pyzjr-1.3.5/pyzjr/augmentation/transforms/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/transforms/normal.py` & `pyzjr-1.3.5/pyzjr/augmentation/transforms/normal.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/transforms/opencv.py` & `pyzjr-1.3.5/pyzjr/augmentation/transforms/opencv.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import torch
 import random
 import numpy as np
 from pyzjr.augmentation.augments import Centerzoom, horizontal_flip, vertical_flip, adjust_brightness_cv2, \
     adjust_gamma, augment_Hsv, hist_equalize, random_rotation, random_lighting, blur, gaussian_blur,\
     bilateral_blur, median_blur, random_crop, random_resize_crop
 
-from pyzjr.core.error import _check_img_is_opencv, convert_to_tuple
+from pyzjr.core.error import _check_img_is_opencv
+from pyzjr.core.helpers import convert_to_tuple
 from pyzjr.Math import rand
 
 __all__ = ["OpencvToTensor",
            "OpencvResize",
            "OpencvSquareResize",
            "OpencvCenterzoom",
            "OpencvHorizontalFlip",
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/transforms/pillow.py` & `pyzjr-1.3.5/pyzjr/augmentation/transforms/pillow.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module is based on PIL implemented transformations.
 """
 import torch
 from PIL import Image, ImageOps, ImageEnhance, ImageFilter
 import random
 from pyzjr.core import _check_img_is_plt, is_pil,_check_img_is_ndarray, _check_parameter_is_tuple_and_list_or_single_2, \
-    _check_input_is_tensor, get_image_size, check_dtype, _get_image_num_channels
+    _check_input_is_tensor, get_image_size, _get_image_num_channels, is_int
 from ._utils import Images, Compose
 import numpy as np
 
 __all__ = ["PILToTensor",
            "NdarryToPIL",
            "TensorToPIL",
            "MeanStdNormalize",
@@ -910,16 +910,15 @@
         >>> transforms = Compose([GaussianBlur(2), PILToTensor(), TensorToPIL()])
         >>> transformed_image = transforms(image)
     """
     def __init__(self, radius):
         self.radius = radius
 
     def apply_gaussian_blur(self, img, radius):
-        type = check_dtype(radius)
-        if type.is_int():
+        if is_int(radius):
             blurred_img = img.filter(ImageFilter.GaussianBlur(radius))
             return blurred_img
 
     def __call__(self, img):
         _check_img_is_plt(img)
         return self.apply_gaussian_blur(img, self.radius)
 
@@ -945,19 +944,18 @@
         self.padding = padding
         self.padding_mode = padding_mode
         self.fill_value = fill_value
         if self.padding_mode not in ['constant', 'edge', 'reflect', 'symmetric']:
             raise ValueError("Padding mode should be 'constant', 'edge', 'reflect', or 'symmetric'.")
 
     def pad(self, img, padding, padding_mode, fill_value):
-        type = check_dtype(padding)
-        if type.is_int():
+        if is_int(padding):
             top = bottom = left = right = padding
 
-        elif type.is_list_or_tuple():
+        elif is_list_or_tuple():
             if len(padding) == 2:
                 left = right = padding[0]
                 top = bottom = padding[1]
             elif len(padding) == 4:
                 left, top, right, bottom = padding
             else:
                 raise ValueError("The size of the padding list or tuple should be 2 or 4.")
@@ -1001,16 +999,15 @@
 
     Examples:
         >>> transforms = Compose([ResizedCrop(224, (10, 10, 100, 100)), PILToTensor(), TensorToPIL()])
         >>> transformed_image = transforms(image)
     """
     def __init__(self, sizes, box):
         super(ResizedCrop, self).__init__(sizes)
-        type = check_dtype(sizes)
-        if type.is_int():
+        if is_int(sizes):
             self.sizes = [sizes, sizes]
         self.box = box
 
     def crop_img(self, img, x, y, width, height):
         return img.crop((x, y, x + width, y + height))
 
     def resize_img(self, img, size):
```

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/transforms/tvision.py` & `pyzjr-1.3.5/pyzjr/augmentation/transforms/tvision.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/augmentation/utils.py` & `pyzjr-1.3.5/pyzjr/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/core/_utils.py` & `pyzjr-1.3.5/pyzjr/core/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/core/lr_scheduler.py` & `pyzjr-1.3.5/pyzjr/core/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/Dataloader.py` & `pyzjr-1.3.5/pyzjr/data/Dataloader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/Dataset.py` & `pyzjr-1.3.5/pyzjr/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/FM.py` & `pyzjr-1.3.5/pyzjr/data/FM.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 import datetime
 import csv
 from os import getcwd
 import win32com.client, gc
 from datetime import datetime
 from pathlib import Path
 import logging
-import re
 
 __all__=[
     # def
     "get_logger",
     "getFilePath",
     "mkdir",
     "logdir",
     "Data2csv",
-    "is_url",
-    "is_ascii",
     "file_age",
     "file_date",
     "file_size",
     # class
     "Microsoft2PDF",
 ]
 
@@ -300,32 +297,14 @@
         """Add worksheet order to file name"""
         return file[:file.rfind('.')] + "_worksheet" + str(i) + ".pdf"
 
     def toFileJoin(self, file):
         """Connect the file path and file name to the complete file path"""
         return os.path.join(self.filePath, 'pdf', file[:file.rfind('.')] + ".pdf")
 
-URL_REGEX = re.compile(r'http://|https://|ftp://|file://|file:\\')
-
-def is_url(filename):
-    """Return True if string is an http or ftp path."""
-    return (isinstance(filename, str) and
-            URL_REGEX.match(filename) is not None)
-
-def is_ascii(s):
-    """
-    Check if the string is composed of only ASCII characters.
-    Args:
-        s (str): String to be checked.
-    Returns:
-        bool: True if the string is composed only of ASCII characters, False otherwise.
-    """
-    s = str(s)
-    return all(ord(c) < 128 for c in s)
-
 def file_age(path, detail=False):
     """Returns the number of days since the last file update."""
     dt = (datetime.now() - datetime.fromtimestamp(Path(path).stat().st_mtime))  # delta
     se = 0
     if detail:
         se = dt.seconds / 86400
     return f"{dt.days + se} days"
```

### Comparing `pyzjr-1.3.4/pyzjr/data/__tensor.py` & `pyzjr-1.3.5/pyzjr/core/__tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 import torch
 import numpy as np
-from pyzjr.core.general import is_numpy, is_tensor
-from pyzjr.core.error import check_dtype
-
-__all__=[    "hwc_and_chw",
-             "to_bchw",
-             "image_to_tensor",
-             "imagelist_to_tensor",
-             "tensor_to_image",
-             "img2tensor",
-             "label2tensor",
-             "SumExceptBatch"
-        ]
-
+from pyzjr.core.general import is_numpy, is_tensor, is_nonnegative_int
 
 def SumExceptBatch(x, num_batch_dims=1):
     """
     求和“x”中除第一个“num_batch_dims”维度外的所有元素。
     case:
     x1 = torch.tensor([[1, 2], [3, 4]])
     result1 = SumExceptBatch(x1, num_batch_dims=1)
     >> tensor([3, 7])
     """
-    check = check_dtype(num_batch_dims)
-    if not check.is_nonnegative_int():
+    if not is_nonnegative_int(num_batch_dims):
         raise TypeError("Number of batch dimensions must be a non-negative integer.")
     reduce_dims = list(range(num_batch_dims, x.ndimension()))
     return torch.sum(x, dim=reduce_dims)
 
 
 def hwc_and_chw(img):
     """
```

### Comparing `pyzjr-1.3.4/pyzjr/data/basedataset.py` & `pyzjr-1.3.5/pyzjr/data/basedataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 import random
 import numpy as np
 from pathlib import Path
 from PIL import Image
 from pyzjr.core import to_2tuple
 from torch.utils.data import Dataset
-from pyzjr.data.__tensor import img2tensor, label2tensor
+from pyzjr.core.__tensor import img2tensor, label2tensor
 
 class BaseDataset(Dataset):
     """A simple dataset class with the same functionality as torch.utils.data.Dataset"""
     def __init__(self):
         pass
 
     def __getitem__(self, idx):
```

### Comparing `pyzjr-1.3.4/pyzjr/data/data_set/Pascal_voc.py` & `pyzjr-1.3.5/pyzjr/data/data_set/Pascal_voc.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/data_set/config.py` & `pyzjr-1.3.5/pyzjr/data/data_set/config.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/io.py` & `pyzjr-1.3.5/pyzjr/visualize/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 All rights reserved.
 
 This module is applied to image reading and display.
 """
 import os
 import cv2
 import imghdr
+import torch
 import numpy as np
 from urllib import request
-import torch
 from matplotlib import pyplot as plt
-from pyzjr.data.FM import is_url
+from pyzjr.core import is_url
 plt.rcParams['font.sans-serif'] = ['SimHei']
 plt.rcParams['axes.unicode_minus'] = False
 from pathlib import Path
 from pyzjr.core import is_gray_image, is_pil
 
-__all__ = ["ImagesReader", "imwrite", "imshowplt", "StackedCV2", "StackedImages", "Stackedplt", "Stackedtorch",
-
-           "plot_line", "bar_chart", "scatter_plot",]
+__all__ = ["ImagesReader", "imwrite", "imshowplt", "StackedCV2", "StackedImages", "Stackedplt",
+           "Stackedtorch", "plot_line", "bar_chart", "scatter_plot", "url2cvImage"]
 
 RGB2BGR  = cv2.COLOR_RGB2BGR
 BGR2RGB  = cv2.COLOR_BGR2RGB
 BGR2GRAY = cv2.COLOR_BGR2GRAY
 RGB2GRAY = cv2.COLOR_RGB2GRAY
 GRAY2BGR = cv2.COLOR_GRAY2BGR
 BGR2HSV  = cv2.COLOR_BGR2HSV
@@ -69,34 +68,35 @@
 
         if self.flip is not None:
             self.image = cv2.flip(self.image, self.flip)
         if self.torgb:
             self.image = cv2.cvtColor(self.image, cv2.COLOR_BGR2RGB)
         return self.image
 
-    def display(self, winname):
+    def display(self, winname, param=False):
         """Displays an image in the specified window."""
         _imshow = cv2.imshow  # copy to avoid recursion errors
         _imshow(winname.encode('unicode_escape').decode(), self.image)
-        print(f"\033[94m{self.param()}")
+        if param:
+            print(f"\033[94m{self.param()}")
         cv2.waitKey(0)
 
     def param(self, idx=None):
         properties = {}
         if isinstance(self.filename, str):
             properties['name'] = os.path.basename(self.filename)
             properties['format'] = imghdr.what(self.filename)
             properties['fsize'] = os.path.getsize(self.filename)
         properties["shape"] = self.image.shape
         properties["dtype"] = self.image.dtype
         properties["channels"] = self.image.shape[2] if len(self.image.shape) == 3 else 1
         properties["resolution"] = (self.image.shape[1], self.image.shape[0])
         return properties if idx is None else properties[idx]
 
-def url2cvimg(url):
+def url2cvImage(url):
     if is_url(url):
         res = request.urlopen(url, timeout=3)
     else:
         raise ValueError("[url2imgcv2]:The current input parameter does not conform to the URL format")
     try:
         image = np.asarray(bytearray(res.read()), dtype="uint8")
         image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
```

### Comparing `pyzjr-1.3.4/pyzjr/data/printf.py` & `pyzjr-1.3.5/pyzjr/visualize/printf.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/data/reader.py` & `pyzjr-1.3.5/pyzjr/data/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,22 @@
         cdd = getcwd()
         imgfile = [os.path.join(cdd, file).replace("\\", "/") for file in imgfile]
         allfile = [os.path.join(cdd, file).replace("\\", "/") for file in allfile]
     return imgfile, allfile
 
 def timestr():
     """Generate a formatted datetime string."""
-    return f"{datetime.datetime.now():%Y_%m_%d_%H_%M_%S}"
+    return f"{datetime.datetime.now():%Y_%m_%d_%H_%M_%S}".replace(":", "_")
+
+def alphabetlabels(capital=False):
+    """字符标签"""
+    alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
+    uppercase_alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+
+    return uppercase_alphabet if capital else alphabet
 
 def pathstr(path_str):
     """
     path_str = 'D:/PythonProject/Torchproject/Lasercenterline/line/20231013-LaserLine_txt/test_2/imges/Image_1.jpg'
     D:\
     PythonProject
     Torchproject
```

### Comparing `pyzjr-1.3.4/pyzjr/devices.py` & `pyzjr-1.3.5/pyzjr/devices/get_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import torch
 import gc
 
-def cpu():
+def Central_Processing_Unit():
     """
     Returns the CPU device.
 
     Returns:
         torch.device: The CPU device.
     """
     return torch.device('cpu')
 
-def gpu(i=0, cuda=True):
+def Graphics_Processing_Unit(i=0, cuda=True):
     """
     If cuda is true and gpu is available, return gpu (i); otherwise, return cpu()
     :param i: Index i, indicating which GPU block to use
     :param cuda: Boolean value indicating whether to use cuda, if not, CPU can be used, set to False
     """
     if cuda and torch.cuda.is_available() and torch.cuda.device_count() >= i + 1:
         return torch.device(f'cuda:{i}')
@@ -28,25 +28,29 @@
     devices = []
     for i in range(torch.cuda.device_count()):
         devices.append(i)
     return devices if devices else [torch.device('cpu')]
 
 def num_workers(batch_size):
     """
-    确定用于数据加载的并行工作进程的数量
+    Determine the number of parallel worker processes used for data loading
     """
-    num_workers = min([os.cpu_count(), batch_size if batch_size > 1 else 0, 8])
-    return num_workers
+    return min([os.cpu_count(), batch_size if batch_size > 1 else 0, 8])
 
 def release_memory(*args):
     """
     Function to release memory resources, particularly useful when working with PyTorch and CUDA.
     """
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
     if not isinstance(args, list):
         args = list(args)
     for i in range(len(args)):
         args[i] = None
     gc.collect()
     return args
 
+
+CPU = cpu = Central_Processing_Unit
+GPU = gpu = Graphics_Processing_Unit
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/__init__.py` & `pyzjr-1.3.5/pyzjr/dlearn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/callbacklog.py` & `pyzjr-1.3.5/pyzjr/dlearn/callbacklog.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/callbacks.py` & `pyzjr-1.3.5/pyzjr/dlearn/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/savemodels.py` & `pyzjr-1.3.5/pyzjr/dlearn/savemodels.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/strategy.py` & `pyzjr-1.3.5/pyzjr/dlearn/strategy.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/tools.py` & `pyzjr-1.3.5/pyzjr/dlearn/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pyzjr.videos.utils import Timer
-from pyzjr.data.printf import colorstr
 import time
 import torch
 import argparse
 import torch.nn as nn
+from pyzjr.visualize.video_utils import Timer
+from pyzjr.visualize.printf import colorstr
 try:
     import thop  # for FLOPs computation
 except ImportError:
     thop = None
 
 __all__ = ["Runcodes", "LoadingBar", "show_config", "GPU_INFO", "time_sync", "profile"]
```

### Comparing `pyzjr-1.3.4/pyzjr/dlearn/trainer.py` & `pyzjr-1.3.5/pyzjr/dlearn/trainer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/mediapipe/HandTrack.py` & `pyzjr-1.3.5/pyzjr/visualize/mediapipe/HandTrack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cv2 as cv
 import mediapipe as mp
 import pyzjr.Z as Z
-from pyzjr.mediapipe.const import HandLandmark
-from pyzjr.augmentation.Color import cornerRect
+from pyzjr.visualize.mediapipe.const import HandLandmark
+from pyzjr.visualize.color import cornerRect
 
 class Hands():
     def __init__(self,NumHands=2,minDetconfid=0.5,minTrackconfid=0.5,StaticMode=False):
         self.NumHands = NumHands
         self.minDetconfid = minDetconfid
         self.minTrackconfid = minTrackconfid
         self.StaticMode = StaticMode
@@ -135,16 +135,16 @@
             return info
 
 def EuclideanDis(pts1, pts2):
     distance = ((pts2[0] - pts1[0]) ** 2 + (pts2[1] - pts1[1]) ** 2) ** 0.5
     center = ((pts1[0] + pts2[0]) / 2, (pts1[1] + pts2[1]) / 2)
     return distance, center
 
-def mainHands():
-    from pyzjr.videos.utils import VideoCap
+if __name__=="__main__":
+    from pyzjr.visualize.video_utils import VideoCap
     Vap=VideoCap()
     Vap.CapInit()
     detector = Hands()
     while True:
         img = Vap.read()
         hands, img = detector.findHands(img)
         if hands:
@@ -153,11 +153,8 @@
             fingers = detector.gesture(hand1)
             if len(hands) == 2:
                 hand2 = hands[1]
                 lmList2 = hand2["lmList"]
                 info, img = detector.fingerSpace(lmList1[8], lmList2[8], img)
         cv.imshow("Image", img)
         if cv.waitKey(1) == Z.Esc:
-            break
-
-if __name__=="__main__":
-    mainHands()
+            break
```

### Comparing `pyzjr-1.3.4/pyzjr/mediapipe/const.py` & `pyzjr-1.3.5/pyzjr/visualize/mediapipe/const.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/Metrics/classification.py` & `pyzjr-1.3.5/pyzjr/nn/Metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/Metrics/semantic.py` & `pyzjr-1.3.5/pyzjr/nn/Metrics/semantic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/functional.py` & `pyzjr-1.3.5/pyzjr/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/torchutils/OneHot.py` & `pyzjr-1.3.5/pyzjr/nn/torchutils/OneHot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/torchutils/avgweight.py` & `pyzjr-1.3.5/pyzjr/nn/torchutils/avgweight.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/torchutils/learnrate.py` & `pyzjr-1.3.5/pyzjr/nn/torchutils/learnrate.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/torchutils/loss_function.py` & `pyzjr-1.3.5/pyzjr/nn/torchutils/loss_function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/nn/torchutils/loss_utils.py` & `pyzjr-1.3.5/pyzjr/nn/torchutils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/utils.py` & `pyzjr-1.3.5/pyzjr/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr/videos/utils.py` & `pyzjr-1.3.5/pyzjr/visualize/video_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.4/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.3.5/pyzjr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.4
+Version: 1.3.5
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.4/pyzjr.egg-info/SOURCES.txt` & `pyzjr-1.3.5/pyzjr.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 README.md
 setup.py
 models_img/__init__.py
 pyzjr/PIC.py
 pyzjr/Z.py
 pyzjr/__init__.py
-pyzjr/devices.py
-pyzjr/utils.py
 pyzjr/version.py
 pyzjr.egg-info/PKG-INFO
 pyzjr.egg-info/SOURCES.txt
 pyzjr.egg-info/dependency_links.txt
 pyzjr.egg-info/requires.txt
 pyzjr.egg-info/top_level.txt
 pyzjr/Math/Numpy.py
@@ -72,14 +70,15 @@
 pyzjr/Models/backbone/efficientnet.py
 pyzjr/Models/backbone/fasternet.py
 pyzjr/Models/backbone/ghostnet.py
 pyzjr/Models/backbone/googlenet.py
 pyzjr/Models/backbone/lenet.py
 pyzjr/Models/backbone/mnasnet.py
 pyzjr/Models/backbone/mobilenet.py
+pyzjr/Models/backbone/nasnet.py
 pyzjr/Models/backbone/regnet.py
 pyzjr/Models/backbone/resnet.py
 pyzjr/Models/backbone/shufflenet.py
 pyzjr/Models/backbone/squeezenet.py
 pyzjr/Models/backbone/vgg.py
 pyzjr/Models/backbone/xception.py
 pyzjr/Models/backbone/zfnet.py
@@ -105,73 +104,78 @@
 pyzjr/Models/sampling/strippooling.py
 pyzjr/Models/segmentation/__init__.py
 pyzjr/Models/segmentation/fcn.py
 pyzjr/Models/segmentation/unet.py
 pyzjr/augmentation/__init__.py
 pyzjr/augmentation/augments.py
 pyzjr/augmentation/utils.py
-pyzjr/augmentation/Color/__init__.py
-pyzjr/augmentation/Color/_utils.py
-pyzjr/augmentation/Color/colormap.py
-pyzjr/augmentation/Color/colorspace.py
-pyzjr/augmentation/Color/cvplot.py
-pyzjr/augmentation/Color/findcolor.py
-pyzjr/augmentation/Color/hex.py
 pyzjr/augmentation/Pixel/Crack.py
 pyzjr/augmentation/Pixel/_Steger.py
 pyzjr/augmentation/Pixel/__init__.py
 pyzjr/augmentation/Pixel/definition.py
 pyzjr/augmentation/Pixel/pixel.py
 pyzjr/augmentation/Pixel/utils.py
 pyzjr/augmentation/transforms/__init__.py
 pyzjr/augmentation/transforms/_utils.py
 pyzjr/augmentation/transforms/normal.py
 pyzjr/augmentation/transforms/opencv.py
 pyzjr/augmentation/transforms/pillow.py
 pyzjr/augmentation/transforms/tvision.py
 pyzjr/core/__init__.py
-pyzjr/core/_str.py
+pyzjr/core/__tensor.py
 pyzjr/core/_utils.py
 pyzjr/core/error.py
 pyzjr/core/general.py
 pyzjr/core/helpers.py
 pyzjr/core/lr_scheduler.py
 pyzjr/data/Dataloader.py
 pyzjr/data/Dataset.py
 pyzjr/data/FM.py
 pyzjr/data/__init__.py
-pyzjr/data/__tensor.py
 pyzjr/data/basedataset.py
 pyzjr/data/dataloader.py
 pyzjr/data/dataset.py
-pyzjr/data/io.py
-pyzjr/data/printf.py
 pyzjr/data/reader.py
-pyzjr/data/voc.py
+pyzjr/data/txt_utils.py
 pyzjr/data/data_set/Pascal_voc.py
 pyzjr/data/data_set/__init__.py
 pyzjr/data/data_set/config.py
+pyzjr/devices/__init__.py
+pyzjr/devices/get_device.py
+pyzjr/devices/measures.py
+pyzjr/devices/systeminfo.py
 pyzjr/dlearn/__init__.py
 pyzjr/dlearn/callbacklog.py
 pyzjr/dlearn/callbacks.py
 pyzjr/dlearn/savemodels.py
 pyzjr/dlearn/strategy.py
 pyzjr/dlearn/tools.py
 pyzjr/dlearn/trainer.py
 pyzjr/math/__init__.py
-pyzjr/mediapipe/HandTrack.py
-pyzjr/mediapipe/__init__.py
-pyzjr/mediapipe/const.py
 pyzjr/nn/Summary.py
 pyzjr/nn/__init__.py
 pyzjr/nn/functional.py
 pyzjr/nn/Metrics/__init__.py
 pyzjr/nn/Metrics/classification.py
 pyzjr/nn/Metrics/semantic.py
 pyzjr/nn/torchutils/OneHot.py
 pyzjr/nn/torchutils/__init__.py
 pyzjr/nn/torchutils/avgweight.py
 pyzjr/nn/torchutils/learnrate.py
 pyzjr/nn/torchutils/loss_function.py
 pyzjr/nn/torchutils/loss_utils.py
-pyzjr/videos/__init__.py
-pyzjr/videos/utils.py
+pyzjr/torch3D/__init__.py
+pyzjr/torch3D/networks/__init__.py
+pyzjr/visualize/__init__.py
+pyzjr/visualize/io.py
+pyzjr/visualize/printf.py
+pyzjr/visualize/utils.py
+pyzjr/visualize/video_utils.py
+pyzjr/visualize/color/__init__.py
+pyzjr/visualize/color/colormap.py
+pyzjr/visualize/color/colorspace.py
+pyzjr/visualize/color/cvplot.py
+pyzjr/visualize/color/findcolor.py
+pyzjr/visualize/color/hex.py
+pyzjr/visualize/mediapipe/HandTrack.py
+pyzjr/visualize/mediapipe/__init__.py
+pyzjr/visualize/mediapipe/const.py
```

### Comparing `pyzjr-1.3.4/setup.py` & `pyzjr-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # from pyzjr.version import __version__
-VERSION = "1.3.4"
+VERSION = "1.3.5"
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
```

