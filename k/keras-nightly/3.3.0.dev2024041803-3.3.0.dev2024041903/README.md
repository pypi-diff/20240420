# Comparing `tmp/keras_nightly-3.3.0.dev2024041803.tar.gz` & `tmp/keras_nightly-3.3.0.dev2024041903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.0.dev2024041803.tar", last modified: Thu Apr 18 03:21:30 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.0.dev2024041903.tar", last modified: Fri Apr 19 03:21:54 2024, max compression
```

## Comparing `keras_nightly-3.3.0.dev2024041803.tar` & `keras_nightly-3.3.0.dev2024041903.tar`

### file list

```diff
@@ -1,921 +1,921 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.152688 keras_nightly-3.3.0.dev2024041803/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-18 03:21:30.152688 keras_nightly-3.3.0.dev2024041803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.016687 keras_nightly-3.3.0.dev2024041803/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.020687 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.020687 keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.020687 keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.020687 keras_nightly-3.3.0.dev2024041803/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.020687 keras_nightly-3.3.0.dev2024041803/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.024687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.028687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.032687 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.036687 keras_nightly-3.3.0.dev2024041803/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.040687 keras_nightly-3.3.0.dev2024041803/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.044687 keras_nightly-3.3.0.dev2024041803/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.048687 keras_nightly-3.3.0.dev2024041803/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/activations/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.052687 keras_nightly-3.3.0.dev2024041803/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/applications_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.052687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.056687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/variables_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.056687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.060687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27716 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.064687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67427 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.068687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45948 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.068687 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.072687 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.076687 keras_nightly-3.3.0.dev2024041803/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.076687 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.076687 keras_nightly-3.3.0.dev2024041803/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.076687 keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.076687 keras_nightly-3.3.0.dev2024041803/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/export/export_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.080687 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/random_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.080687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.084687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.084687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.088688 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.092687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    25757 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    42038 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/masking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63526 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.092687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.096687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.096687 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.104688 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.108688 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.112688 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.116688 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.116688 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.116688 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.120688 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.120688 keras_nightly-3.3.0.dev2024041803/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/losses/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/losses/losses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.124688 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metric_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.124688 keras_nightly-3.3.0.dev2024041803/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/cloning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/functional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22761 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/sequential_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/variable_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.128688 keras_nightly-3.3.0.dev2024041803/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/linalg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/nn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   190182 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   278258 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/numpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.132688 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/lion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.136688 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.136688 keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.136688 keras_nightly-3.3.0.dev2024041803/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/random/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/random/seed_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.136688 keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.136688 keras_nightly-3.3.0.dev2024041803/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/object_registration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/serialization_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.140688 keras_nightly-3.3.0.dev2024041803/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.140688 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.140688 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    46440 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.144688 keras_nightly-3.3.0.dev2024041803/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/tree/tree_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/tree/tree_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.152688 keras_nightly-3.3.0.dev2024041803/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/code_stats_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/naming_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/keras/src/utils/tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 03:21:28.000000 keras_nightly-3.3.0.dev2024041803/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:21:30.152688 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-18 03:21:29.000000 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-18 03:21:29.000000 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:21:29.000000 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 03:21:29.000000 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 03:21:29.000000 keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 03:20:14.000000 keras_nightly-3.3.0.dev2024041803/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 03:21:30.152688 keras_nightly-3.3.0.dev2024041803/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-18 03:21:28.000000 keras_nightly-3.3.0.dev2024041803/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.772486 keras_nightly-3.3.0.dev2024041903/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.772486 keras_nightly-3.3.0.dev2024041903/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.776486 keras_nightly-3.3.0.dev2024041903/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/applications_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.776486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.780486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.780486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30159 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.784486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.788486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.792486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46016 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.792486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.796486 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.808486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.808486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.812486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.816486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.820486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.820486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.824486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.832486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.836486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.840486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.844486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.852486 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.856486 keras_nightly-3.3.0.dev2024041903/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/functional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22766 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.860486 keras_nightly-3.3.0.dev2024041903/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   279186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.876486 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.876486 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46440 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.880486 keras_nightly-3.3.0.dev2024041903/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 03:21:52.000000 keras_nightly-3.3.0.dev2024041903/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-19 03:21:52.000000 keras_nightly-3.3.0.dev2024041903/setup.py
```

### Comparing `keras_nightly-3.3.0.dev2024041803/LICENSE` & `keras_nightly-3.3.0.dev2024041903/LICENSE`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/PKG-INFO` & `keras_nightly-3.3.0.dev2024041903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024041803
+Version: 3.3.0.dev2024041903
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024041803/README.md` & `keras_nightly-3.3.0.dev2024041903/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/activation_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/activation_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/attention_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/attention_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/base_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/base_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/conv_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/conv_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/core_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/core_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/merge_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/merge_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/normalization_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/normalization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/pooling_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/pooling_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/regularization_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/regularization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/reshaping_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/reshaping_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/layer_benchmark/rnn_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/rnn_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/bert_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/bert_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/model_benchmark/image_classification_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/image_classification_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py` & `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from keras.src.ops.core import stop_gradient
 from keras.src.ops.core import unstack
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/applications/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/config/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from keras.src.ops.core import stop_gradient
 from keras.src.ops.core import unstack
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/random/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/api/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/activations/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/activations/activations.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/activations/activations_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/api_export.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/applications_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/applications_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/convnext.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/densenet.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/imagenet_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/nasnet.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/resnet.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/vgg16.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/vgg19.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/applications/xception.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/backend_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/compute_output_spec_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/compute_output_spec_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/dtypes_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/keras_tensor_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/name_scope_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/stateless_scope_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/variables.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/common/variables_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/config.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/exports.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/core.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/linalg.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     return jnp.linalg.det(a)
 
 
 def eig(x):
     return jnp.linalg.eig(x)
 
 
+def eigh(x):
+    return jnp.linalg.eigh(x)
+
+
 def inv(a):
     return jnp.linalg.inv(a)
 
 
 def lu_factor(x):
     lu_factor_fn = jsp.linalg.lu_factor
     if x.ndim > 2:
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/math.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,20 +335,20 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return jnp.arctanh(x)
 
 
-def argmax(x, axis=None):
-    return jnp.argmax(x, axis=axis)
+def argmax(x, axis=None, keepdims=False):
+    return jnp.argmax(x, axis=axis, keepdims=keepdims)
 
 
-def argmin(x, axis=None):
-    return jnp.argmin(x, axis=axis)
+def argmin(x, axis=None, keepdims=False):
+    return jnp.argmin(x, axis=axis, keepdims=keepdims)
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
     if x.ndim == 0:
         return jnp.argsort(x, axis=None)
     return jnp.argsort(x, axis=axis)
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/random.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/linalg.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     return np.linalg.det(a)
 
 
 def eig(a):
     return np.linalg.eig(a)
 
 
+def eigh(a):
+    return np.linalg.eigh(a)
+
+
 def inv(a):
     return np.linalg.inv(a)
 
 
 def lu_factor(a):
     if a.ndim == 2:
         return sl.lu_factor(a)
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,22 +223,22 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = x.astype(dtype)
     return np.arctanh(x)
 
 
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     axis = standardize_axis_for_numpy(axis)
-    return np.argmax(x, axis=axis).astype("int32")
+    return np.argmax(x, axis=axis, keepdims=keepdims).astype("int32")
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     axis = standardize_axis_for_numpy(axis)
-    return np.argmin(x, axis=axis).astype("int32")
+    return np.argmin(x, axis=axis, keepdims=keepdims).astype("int32")
 
 
 def argsort(x, axis=-1):
     axis = standardize_axis_for_numpy(axis)
     return np.argsort(x, axis=axis).astype("int32")
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/distribute_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     return tf.linalg.det(a)
 
 
 def eig(a):
     return tf.linalg.eig(a)
 
 
+def eigh(a):
+    return tf.linalg.eigh(a)
+
+
 def inv(a):
     return tf.linalg.inv(a)
 
 
 def lu_factor(a):
     lu, p = tf.linalg.lu(a)
     return lu, tf.math.invert_permutation(p)
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/name_scope_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,24 +741,43 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = tf.cast(x, dtype)
     return tf.math.atanh(x)
 
 
-def argmax(x, axis=None):
+def _keepdims(x, y, axis):
+    if axis is None:
+        shape = [1 for _ in range(len(x.shape))]
+    else:
+        shape = [tf.shape[i] for i in range(len(x.shape))]
+        for axis in tree.flatten(axis):
+            shape[axis] = 1
+    y = tf.reshape(y, shape)
+    return y
+
+
+def argmax(x, axis=None, keepdims=False):
+    _x = x
     if axis is None:
         x = tf.reshape(x, [-1])
-    return tf.cast(tf.argmax(x, axis=axis), dtype="int32")
+    y = tf.cast(tf.argmax(x, axis=axis), dtype="int32")
+    if keepdims:
+        y = _keepdims(_x, y, axis)
+    return y
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
+    _x = x
     if axis is None:
         x = tf.reshape(x, [-1])
-    return tf.cast(tf.argmin(x, axis=axis), dtype="int32")
+    y = tf.cast(tf.argmin(x, axis=axis), dtype="int32")
+    if keepdims:
+        y = _keepdims(_x, y, axis)
+    return y
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "bool":
         x = tf.cast(x, "uint8")
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/optimizer_distribute_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer_distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/saved_model_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/saved_model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/core.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     return torch.det(x)
 
 
 def eig(x):
     return torch.linalg.eig(x)
 
 
+def eigh(x):
+    return torch.linalg.eigh(x)
+
+
 def inv(x):
     return torch.linalg.inv(x)
 
 
 def lu_factor(x):
     LU, pivots = torch.linalg.lu_factor(x)
     # torch retuns pivots with 1-based indexing
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/math.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,32 +314,32 @@
 
 
 def arctanh(x):
     x = convert_to_tensor(x)
     return torch.arctanh(x)
 
 
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
 
     # TODO: torch.argmax doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = cast(x, "uint8")
 
-    return cast(torch.argmax(x, dim=axis), dtype="int32")
+    return cast(torch.argmax(x, dim=axis, keepdim=keepdims), dtype="int32")
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
 
     # TODO: torch.argmin doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = cast(x, "uint8")
 
-    return cast(torch.argmin(x, dim=axis), dtype="int32")
+    return cast(torch.argmin(x, dim=axis, keepdim=keepdims), dtype="int32")
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
 
     # TODO: torch.argsort doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/random.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/backup_and_restore_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/callback_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/csv_logger_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/early_stopping_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/history.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/lambda_callback_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/learning_rate_scheduler_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/model_checkpoint_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/remote_monitor_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/swap_ema_weights_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/tensorboard_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/callbacks/terminate_on_nan_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/constraints/constraints.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/constraints/constraints_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/imdb.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/mnist.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/datasets/reuters.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/distribution/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/dtype_policies/dtype_policy_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/export/export_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/export/export_lib_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/constant_initializers_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/initializer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/initializers/random_initializers_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/activation_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/elu_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/leaky_relu_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/prelu_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/relu_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/activations/softmax_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/additive_attention_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/attention_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/grouped_query_attention_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/attention/multi_head_attention_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/conv_transpose_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_transpose_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/depthwise_conv_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/convolutional/separable_conv_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/dense.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import ml_dtypes
 
 from keras.src import activations
-from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
 from keras.src import regularizers
 from keras.src.api_export import keras_export
@@ -343,14 +342,15 @@
         )
         self.kernel_scale = self.add_weight(
             name="kernel_scale",
             shape=(self.units,),
             initializer=kernel_scale_initializer,
             trainable=False,
         )
+        self._is_quantized = True
 
     def _float8_build(self):
         if not isinstance(
             self.dtype_policy, dtype_policies.QuantizedFloat8DTypePolicy
         ):
             raise TypeError(
                 "`self.dtype_policy` must be the type of "
@@ -392,14 +392,15 @@
         # gradients during training
         self.inputs_scale.overwrite_with_gradient = True
         self.inputs_amax_history.overwrite_with_gradient = True
         self.kernel_scale.overwrite_with_gradient = True
         self.kernel_amax_history.overwrite_with_gradient = True
         self.outputs_grad_scale.overwrite_with_gradient = True
         self.outputs_grad_amax_history.overwrite_with_gradient = True
+        self._is_quantized = True
 
     def quantized_call(self, inputs):
         if self.dtype_policy.quantization_mode == "int8":
             return self._int8_call(inputs)
         elif self.dtype_policy.quantization_mode == "float8":
             return self._float8_call(inputs)
         else:
@@ -548,16 +549,14 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            if backend.standardize_dtype(self._kernel.dtype) == "int8":
-                raise ValueError("`quantize` can only be done once per layer.")
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=0
             )
             kernel_scale = ops.squeeze(kernel_scale, axis=0)
@@ -568,16 +567,14 @@
             # large constant to the computation graph.
             self._int8_build(
                 kernel_shape,
                 lambda shape, dtype: kernel_value,
                 lambda shape, dtype: kernel_scale,
             )
         elif mode == "float8":
-            if hasattr(self, "inputs_amax_history"):
-                raise ValueError("`quantize` can only be done once per layer.")
             self._float8_build()
         else:
             raise NotImplementedError(
                 self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
         self._tracker.lock()
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/dense_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -416,18 +416,32 @@
         ("int8", "int8"),
         ("float8", "float8"),
     )
     def test_quantize_when_already_quantized(self, mode):
         layer = layers.Dense(units=2)
         layer.build((None, 2))
         layer.quantize(mode)
-        with self.assertRaisesRegex(
-            ValueError, "`quantize` can only be done once per layer."
-        ):
-            layer.quantize(mode)
+        for m in ["int8", "float8"]:
+            with self.assertRaisesRegex(
+                ValueError, "is already quantized with dtype_policy="
+            ):
+                layer.quantize(m)
+
+    @parameterized.named_parameters(
+        ("int8", "int8_from_float32"),
+        ("float8", "float8_from_float32"),
+    )
+    def test_quantize_when_already_quantized_using_dtype_argument(self, mode):
+        layer = layers.Dense(units=2, dtype=mode)
+        layer.build((None, 2))
+        for m in ["int8", "float8"]:
+            with self.assertRaisesRegex(
+                ValueError, "is already quantized with dtype_policy="
+            ):
+                layer.quantize(m)
 
     @parameterized.named_parameters(
         ("int8", "int8_from_float32", 3),
         ("float8", "float8_from_float32", 8),
     )
     def test_quantize_by_setting_dtype_policy(
         self, policy, expected_num_variables
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 import string
 
 import ml_dtypes
 import numpy as np
 
 from keras.src import activations
-from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
 from keras.src import regularizers
 from keras.src.api_export import keras_export
@@ -427,14 +426,15 @@
             kernel_scale_shape.pop(a)
         self.kernel_scale = self.add_weight(
             name="kernel_scale",
             shape=kernel_scale_shape,
             initializer=kernel_scale_initializer,
             trainable=False,
         )
+        self._is_quantized = True
 
     def _float8_build(self):
         if not isinstance(
             self.dtype_policy, dtype_policies.QuantizedFloat8DTypePolicy
         ):
             raise TypeError(
                 "`self.dtype_policy` must be the type of "
@@ -476,14 +476,15 @@
         # gradients during training
         self.inputs_scale.overwrite_with_gradient = True
         self.inputs_amax_history.overwrite_with_gradient = True
         self.kernel_scale.overwrite_with_gradient = True
         self.kernel_amax_history.overwrite_with_gradient = True
         self.outputs_grad_scale.overwrite_with_gradient = True
         self.outputs_grad_amax_history.overwrite_with_gradient = True
+        self._is_quantized = True
 
     def quantized_call(self, inputs):
         if self.dtype_policy.quantization_mode == "int8":
             return self._int8_call(inputs)
         elif self.dtype_policy.quantization_mode == "float8":
             return self._float8_call(inputs)
         else:
@@ -661,16 +662,14 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            if backend.standardize_dtype(self._kernel.dtype) == "int8":
-                raise ValueError("`quantize` can only be done once per layer.")
             (
                 self._input_reduced_axes,
                 self._kernel_reduced_axes,
                 self._input_transpose_axes,
                 self._kernel_transpose_axes,
                 self._input_expand_axes,
                 self._kernel_expand_axes,
@@ -705,16 +704,14 @@
             # large constant to the computation graph.
             self._int8_build(
                 kernel_shape,
                 lambda shape, dtype: kernel_value,
                 lambda shape, dtype: kernel_scale,
             )
         elif mode == "float8":
-            if hasattr(self, "inputs_amax_history"):
-                raise ValueError("`quantize` can only be done once per layer.")
             self._float8_build()
         else:
             raise NotImplementedError(
                 self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
         self._tracker.lock()
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/einsum_dense_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,23 +504,42 @@
     @parameterized.named_parameters(
         ("int8", "int8"),
         ("float8", "float8"),
     )
     def test_quantize_when_already_quantized(self, mode):
         layer = layers.EinsumDense(
             equation="ab,bcd->acd",
-            output_shape=(8, 32),
+            output_shape=(8, 16),
             bias_axes="d",
         )
         layer.build((None, 3))
         layer.quantize(mode)
-        with self.assertRaisesRegex(
-            ValueError, "`quantize` can only be done once per layer."
-        ):
-            layer.quantize(mode)
+        for m in ["int8", "float8"]:
+            with self.assertRaisesRegex(
+                ValueError, "is already quantized with dtype_policy="
+            ):
+                layer.quantize(m)
+
+    @parameterized.named_parameters(
+        ("int8", "int8_from_float32"),
+        ("float8", "float8_from_float32"),
+    )
+    def test_quantize_when_already_quantized_using_dtype_argument(self, mode):
+        layer = layers.EinsumDense(
+            equation="ab,bcd->acd",
+            output_shape=(8, 16),
+            bias_axes="d",
+            dtype=mode,
+        )
+        layer.build((None, 3))
+        for m in ["int8", "float8"]:
+            with self.assertRaisesRegex(
+                ValueError, "is already quantized with dtype_policy="
+            ):
+                layer.quantize(m)
 
     @parameterized.named_parameters(
         ("int8", "int8_from_float32", 3),
         ("float8", "float8_from_float32", 8),
     )
     def test_quantize_by_setting_dtype_policy(
         self, policy, expected_num_variables
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,15 @@
         )
         self.embeddings_scale = self.add_weight(
             name="embeddings_scale",
             shape=(self.output_dim,),
             initializer=embeddings_scale_initializer,
             trainable=False,
         )
+        self._is_quantized = True
 
     def quantized_call(self, inputs):
         if self.dtype_policy.quantization_mode == "int8":
             return self._int8_call(inputs)
         else:
             mode = self.dtype_policy.quantization_mode
             raise NotImplementedError(
@@ -370,16 +371,14 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            if backend.standardize_dtype(self._embeddings.dtype) == "int8":
-                raise ValueError("`quantize` can only be done once per layer.")
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._embeddings` to int8 and compute corresponding
             # scale
             embeddings_value, embeddings_scale = quantizers.abs_max_quantize(
                 self._embeddings, axis=0
             )
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/embedding_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,23 @@
             layer.quantize("int8")
 
     def test_quantize_when_already_quantized(self):
         layer = layers.Embedding(10, 16)
         layer.build()
         layer.quantize("int8")
         with self.assertRaisesRegex(
-            ValueError, "`quantize` can only be done once per layer."
+            ValueError, "is already quantized with dtype_policy="
+        ):
+            layer.quantize("int8")
+
+    def test_quantize_when_already_quantized_using_dtype_argument(self):
+        layer = layers.Embedding(10, 16, dtype="int8_from_float32")
+        layer.build()
+        with self.assertRaisesRegex(
+            ValueError, "is already quantized with dtype_policy="
         ):
             layer.quantize("int8")
 
     @parameterized.named_parameters(
         ("int8", "int8_from_float32", 2),
     )
     def test_quantize_by_setting_dtype_policy(
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/identity.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/identity_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/input_layer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/lambda_layer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/masking.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/masking_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/core/wrapper_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/input_spec.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1139,14 +1139,20 @@
     def _check_quantize_args(self, mode, compute_dtype):
         if not self.built:
             raise ValueError(
                 "Cannot quantize a layer that isn't yet built. "
                 f"Layer '{self.name}' (of type '{self.__class__.__name__}') "
                 "is not built yet."
             )
+        if getattr(self, "_is_quantized", False):
+            raise ValueError(
+                f"Layer '{self.name}' is already quantized with "
+                f"dtype_policy='{self.dtype_policy.name}'. "
+                f"Received: mode={mode}"
+            )
         if mode not in dtype_policies.QUANTIZATION_MODES:
             raise ValueError(
                 "Invalid quantization mode. "
                 f"Expected one of {dtype_policies.QUANTIZATION_MODES}. "
                 f"Received: mode={mode}"
             )
         if mode == "int8" and compute_dtype == "float16":
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/layer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/add.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/average.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/merging_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/merging_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/batch_normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/group_normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/layer_normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/spectral_normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/normalization/unit_normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/average_pooling_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_average_pooling_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/global_max_pooling_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/pooling/max_pooling_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/audio_preprocessing_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/category_encoding_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/center_crop_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/discretization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/feature_space_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashed_crossing_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/hashing_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/index_lookup_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/integer_lookup_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/normalization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_brightness_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_contrast_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_crop_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_flip_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_rotation_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_translation_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/random_zoom_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/rescaling_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/resizing_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/string_lookup_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/text_vectorization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/activity_regularization_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/alpha_dropout_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/dropout_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_dropout_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/gaussian_noise_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/regularization/spatial_dropout_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping1d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping2d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/cropping3d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/flatten_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/permute_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/repeat_vector_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/reshape_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling1d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling2d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/up_sampling3d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding1d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding2d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/reshaping/zero_padding3d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/bidirectional_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm1d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm2d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm3d_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/conv_lstm_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/dropout_rnn_cell_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/gru_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/lstm_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/rnn_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/simple_rnn_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/stacked_rnn_cells_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/layers/rnn/time_distributed_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/backend.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/layers.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/losses.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/json_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/legacy_h5_format_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/losses/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/losses/loss.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/losses/loss_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/losses/losses.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/losses/losses_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/accuracy_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/confusion_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/f_score_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/hinge_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/iou_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metric.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metric_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/probabilistic_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/reduction_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/metrics/regression_metrics_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/cloning.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/cloning_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/functional.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/functional_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/functional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/model.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         Args:
             filepath: `str` or `pathlib.Path` object.
                 Path where to save the model. Must end in `.weights.h5`.
             overwrite: Whether we should overwrite any existing model
                 at the target location, or instead ask the user
                 via an interactive prompt.
         """
-        return saving_api.save_weights(self, filepath, overwrite=True)
+        return saving_api.save_weights(self, filepath, overwrite=overwrite)
 
     @traceback_utils.filter_traceback
     def load_weights(self, filepath, skip_mismatch=False, **kwargs):
         """Load weights from a file saved via `save_weights()`.
 
         Weights are loaded based on the network's
         topology. This means the architecture should be the same as when the
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/model_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/sequential.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/sequential_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/models/variable_mapping_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/core.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/core_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/core_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/function.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/function_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/function_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/image.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/image_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/image_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/linalg.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
     def __init__(self):
         super().__init__()
 
     def call(self, x):
         return _eig(x)
 
     def compute_output_spec(self, x):
-        _assert_2d(x)
         _assert_square(x)
+        _assert_2d(x)
         return (
             KerasTensor(x.shape[:-1], x.dtype),
             KerasTensor(x.shape, x.dtype),
         )
 
 
 @keras_export(["keras.ops.eig", "keras.ops.linalg.eig"])
@@ -106,28 +106,68 @@
 
     Args:
         x: Input tensor of shape `(..., M, M)`.
 
     Returns:
         A tuple of two tensors: a tensor of shape `(..., M)` containing
         eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
-
     """
     if any_symbolic_tensors((x,)):
         return Eig().symbolic_call(x)
     return _eig(x)
 
 
 def _eig(x):
     x = backend.convert_to_tensor(x)
-    _assert_2d(x)
     _assert_square(x)
+    _assert_2d(x)
     return backend.linalg.eig(x)
 
 
+class Eigh(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _eigh(x)
+
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
+        return (
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
+        )
+
+
+@keras_export(["keras.ops.eigh", "keras.ops.linalg.eigh"])
+def eigh(x):
+    """Computes the eigenvalues and eigenvectors of a complex Hermitian.
+
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return Eigh().symbolic_call(x)
+    return _eigh(x)
+
+
+def _eigh(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eigh(x)
+
+
 class Inv(Operation):
 
     def __init__(self):
         super().__init__()
 
     def call(self, x):
         return _inv(x)
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/linalg_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,19 @@
 
     def test_eig(self):
         x = KerasTensor([None, 20, 20])
         w, v = linalg.eig(x)
         self.assertEqual(w.shape, (None, 20))
         self.assertEqual(v.shape, (None, 20, 20))
 
-        x = KerasTensor([None, None, 20])
-        with self.assertRaises(ValueError):
-            linalg.eig(x)
-
-        x = KerasTensor([None, 20, 15])
-        with self.assertRaises(ValueError):
-            linalg.eig(x)
+    def test_eigh(self):
+        x = KerasTensor([None, 20, 20])
+        w, v = linalg.eigh(x)
+        self.assertEqual(w.shape, (None, 20))
+        self.assertEqual(v.shape, (None, 20, 20))
 
     def test_inv(self):
         x = KerasTensor([None, 20, 20])
         out = linalg.inv(x)
         self.assertEqual(out.shape, (None, 20, 20))
 
         x = KerasTensor([None, None, 20])
@@ -204,14 +202,24 @@
         self.assertEqual(w.shape, (4, 3))
         self.assertEqual(v.shape, (4, 3, 3))
 
         x = KerasTensor([10, 20, 15])
         with self.assertRaises(ValueError):
             linalg.eig(x)
 
+    def test_eigh(self):
+        x = KerasTensor([4, 3, 3])
+        w, v = linalg.eigh(x)
+        self.assertEqual(w.shape, (4, 3))
+        self.assertEqual(v.shape, (4, 3, 3))
+
+        x = KerasTensor([10, 20, 15])
+        with self.assertRaises(ValueError):
+            linalg.eigh(x)
+
     def test_inv(self):
         x = KerasTensor([4, 3, 3])
         out = linalg.inv(x)
         self.assertEqual(out.shape, (4, 3, 3))
 
         x = KerasTensor([10, 20, 15])
         with self.assertRaises(ValueError):
@@ -342,14 +350,21 @@
                 with self.assertRaises(NotImplementedError):
                     linalg.eig(x)
                 return
         w, v = map(ops.convert_to_numpy, linalg.eig(x))
         x_reconstructed = (v * w[..., None, :]) @ v.transpose((0, 2, 1))
         self.assertAllClose(x_reconstructed, x, atol=1e-4)
 
+    def test_eigh(self):
+        x = np.random.rand(2, 3, 3)
+        x = x @ x.transpose((0, 2, 1))
+        w, v = map(ops.convert_to_numpy, linalg.eigh(x))
+        x_reconstructed = (v * w[..., None, :]) @ v.transpose((0, 2, 1))
+        self.assertAllClose(x_reconstructed, x, atol=1e-4)
+
     def test_inv(self):
         x = np.random.rand(4, 3, 3)
         x_inv = ops.convert_to_numpy(linalg.inv(x))
         x_reconstructed = x @ x_inv
         # high tolerance due to numerical instability
         self.assertAllClose(
             x_reconstructed, np.repeat(np.eye(3)[None], 4, 0), atol=1e-3
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/math.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/math_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/math_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/nn.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/nn_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/node.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/node_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/node_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/numpy.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         axis: An integer or tuple of integers that represent the axis along
             which a logical AND reduction is performed. The default
             (`axis=None`) is to perform a logical AND over all the dimensions
             of the input array. `axis` may be negative, in which case it counts
             for the last to the first axis.
         keepdims: If `True`, axes which are reduced are left in the result as
             dimensions with size one. With this option, the result will
-            broadcast correctly against the input array. Defaults to`False`.
+            broadcast correctly against the input array. Defaults to `False`.
 
     Returns:
         The tensor containing the logical AND reduction over the `axis`.
 
     Examples:
     >>> x = keras.ops.convert_to_tensor([True, False])
     >>> keras.ops.all(x)
@@ -412,15 +412,15 @@
         axis: An integer or tuple of integers that represent the axis along
             which a logical OR reduction is performed. The default
             (`axis=None`) is to perform a logical OR over all the dimensions
             of the input array. `axis` may be negative, in which case it counts
             for the last to the first axis.
         keepdims: If `True`, axes which are reduced are left in the result as
             dimensions with size one. With this option, the result will
-            broadcast correctly against the input array. Defaults to`False`.
+            broadcast correctly against the input array. Defaults to `False`.
 
     Returns:
         The tensor containing the logical OR reduction over the `axis`.
 
     Examples:
     >>> x = keras.ops.convert_to_tensor([True, False])
     >>> keras.ops.any(x)
@@ -959,37 +959,42 @@
     """
     if any_symbolic_tensors((x,)):
         return Arctanh().symbolic_call(x)
     return backend.numpy.arctanh(x)
 
 
 class Argmax(Operation):
-    def __init__(self, axis=None):
+    def __init__(self, axis=None, keepdims=False):
         super().__init__()
         self.axis = axis
+        self.keepdims = keepdims
 
     def call(self, x):
-        return backend.numpy.argmax(x, axis=self.axis)
+        return backend.numpy.argmax(x, axis=self.axis, keepdims=self.keepdims)
 
     def compute_output_spec(self, x):
+        if self.keepdims:
+            return KerasTensor(x.shape, dtype="int32")
         if self.axis is None:
             return KerasTensor([], dtype="int32")
         return KerasTensor(
             reduce_shape(x.shape, axis=[self.axis]), dtype="int32"
         )
 
 
 @keras_export(["keras.ops.argmax", "keras.ops.numpy.argmax"])
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     """Returns the indices of the maximum values along an axis.
 
     Args:
         x: Input tensor.
         axis: By default, the index is into the flattened tensor, otherwise
             along the specified axis.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one. Defaults to `False`.
 
     Returns:
         Tensor of indices. It has the same shape as `x`, with the dimension
         along `axis` removed.
 
     Example:
     >>> x = keras.ops.arange(6).reshape(2, 3) + 10
@@ -1000,42 +1005,47 @@
     array(5, dtype=int32)
     >>> keras.ops.argmax(x, axis=0)
     array([1, 1, 1], dtype=int32)
     >>> keras.ops.argmax(x, axis=1)
     array([2, 2], dtype=int32)
     """
     if any_symbolic_tensors((x,)):
-        return Argmax(axis=axis).symbolic_call(x)
-    return backend.numpy.argmax(x, axis=axis)
+        return Argmax(axis=axis, keepdims=keepdims).symbolic_call(x)
+    return backend.numpy.argmax(x, axis=axis, keepdims=keepdims)
 
 
 class Argmin(Operation):
-    def __init__(self, axis=None):
+    def __init__(self, axis=None, keepdims=False):
         super().__init__()
         self.axis = axis
+        self.keepdims = keepdims
 
     def call(self, x):
-        return backend.numpy.argmin(x, axis=self.axis)
+        return backend.numpy.argmin(x, axis=self.axis, keepdims=self.keepdims)
 
     def compute_output_spec(self, x):
+        if self.keepdims:
+            return KerasTensor(x.shape, dtype="int32")
         if self.axis is None:
             return KerasTensor([], dtype="int32")
         return KerasTensor(
             reduce_shape(x.shape, axis=[self.axis]), dtype="int32"
         )
 
 
 @keras_export(["keras.ops.argmin", "keras.ops.numpy.argmin"])
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     """Returns the indices of the minium values along an axis.
 
     Args:
         x: Input tensor.
         axis: By default, the index is into the flattened tensor, otherwise
             along the specified axis.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one. Defaults to `False`.
 
     Returns:
         Tensor of indices. It has the same shape as `x`, with the dimension
         along `axis` removed.
 
     Example:
     >>> x = keras.ops.arange(6).reshape(2, 3) + 10
@@ -1046,16 +1056,16 @@
     array(0, dtype=int32)
     >>> keras.ops.argmin(x, axis=0)
     array([0, 0, 0], dtype=int32)
     >>> keras.ops.argmin(x, axis=1)
     array([0, 0], dtype=int32)
     """
     if any_symbolic_tensors((x,)):
-        return Argmin(axis=axis).symbolic_call(x)
-    return backend.numpy.argmin(x, axis=axis)
+        return Argmin(axis=axis, keepdims=keepdims).symbolic_call(x)
+    return backend.numpy.argmin(x, axis=axis, keepdims=keepdims)
 
 
 class Argsort(Operation):
     def __init__(self, axis=-1):
         super().__init__()
         self.axis = axis
 
@@ -3161,15 +3171,15 @@
         stop: The end value of the sequence, unless `endpoint` is set to
             `False`. In that case, the sequence consists of all but the last
             of `num + 1` evenly spaced samples, so that `stop` is excluded.
             Note that the step size changes when `endpoint` is `False`.
         num: Number of samples to generate. Defaults to `50`. Must be
             non-negative.
         endpoint: If `True`, `stop` is the last sample. Otherwise, it is
-            not included. Defaults to`True`.
+            not included. Defaults to `True`.
         retstep: If `True`, return `(samples, step)`, where `step` is the
             spacing between samples.
         dtype: The type of the output tensor.
         axis: The axis in the result to store the samples. Relevant only if
             start or stop are array-like. Defaults to `0`.
 
     Note:
@@ -3498,15 +3508,15 @@
         start: The starting value of the sequence.
         stop: The final value of the sequence, unless `endpoint` is `False`.
             In that case, `num + 1` values are spaced over the interval in
             log-space, of which all but the last (a sequence of length `num`)
             are returned.
         num: Number of samples to generate. Defaults to `50`.
         endpoint: If `True`, `stop` is the last sample. Otherwise, it is not
-            included. Defaults to`True`.
+            included. Defaults to `True`.
         base: The base of the log space. Defaults to `10`.
         dtype: The type of the output tensor.
         axis: The axis in the result to store the samples. Relevant only
             if start or stop are array-like.
 
     Note:
         Torch backend does not support `axis` argument.
@@ -3601,16 +3611,16 @@
     """Return the maximum of a tensor or maximum along an axis.
 
     Args:
         x: Input tensor.
         axis: Axis or axes along which to operate. By default, flattened input
             is used.
         keepdims: If this is set to `True`, the axes which are reduced are left
-            in the result as dimensions with size one. Defaults to`False`.
-        initial: The minimum value of an output element. Defaults to`None`.
+            in the result as dimensions with size one. Defaults to `False`.
+        initial: The minimum value of an output element. Defaults to `None`.
 
     Returns:
         Maximum of `x`.
     """
     if any_symbolic_tensors((x,)):
         return Max(axis=axis, keepdims=keepdims, initial=initial).symbolic_call(
             x
@@ -3794,16 +3804,16 @@
     """Return the minimum of a tensor or minimum along an axis.
 
     Args:
         x: Input tensor.
         axis: Axis or axes along which to operate. By default, flattened input
             is used.
         keepdims: If this is set to `True`, the axes which are reduced are left
-            in the result as dimensions with size one. Defaults to`False`.
-        initial: The maximum value of an output element. Defaults to`None`.
+            in the result as dimensions with size one. Defaults to `False`.
+        initial: The maximum value of an output element. Defaults to `None`.
 
     Returns:
         Minimum of `x`.
     """
     if any_symbolic_tensors((x,)):
         return Min(axis=axis, keepdims=keepdims, initial=initial).symbolic_call(
             x
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/numpy_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1000,24 +1000,28 @@
     def test_arctanh(self):
         x = KerasTensor((None, 3))
         self.assertEqual(knp.arctanh(x).shape, (None, 3))
 
     def test_argmax(self):
         x = KerasTensor((None, 3))
         self.assertEqual(knp.argmax(x).shape, ())
+        self.assertEqual(knp.argmax(x, keepdims=True).shape, (None, 3))
 
         x = KerasTensor((None, 3, 3))
         self.assertEqual(knp.argmax(x, axis=1).shape, (None, 3))
+        self.assertEqual(knp.argmax(x, keepdims=True).shape, (None, 3, 3))
 
     def test_argmin(self):
         x = KerasTensor((None, 3))
         self.assertEqual(knp.argmin(x).shape, ())
+        self.assertEqual(knp.argmin(x, keepdims=True).shape, (None, 3))
 
         x = KerasTensor((None, 3, 3))
         self.assertEqual(knp.argmin(x, axis=1).shape, (None, 3))
+        self.assertEqual(knp.argmin(x, keepdims=True).shape, (None, 3, 3))
 
     def test_argsort(self):
         x = KerasTensor((None, 3))
         self.assertEqual(knp.argsort(x).shape, (None, 3))
 
         x = KerasTensor((None, 3, 3))
         self.assertEqual(knp.argsort(x, axis=1).shape, (None, 3, 3))
@@ -1563,18 +1567,20 @@
     def test_arctanh(self):
         x = KerasTensor((2, 3))
         self.assertEqual(knp.arctanh(x).shape, (2, 3))
 
     def test_argmax(self):
         x = KerasTensor((2, 3))
         self.assertEqual(knp.argmax(x).shape, ())
+        self.assertEqual(knp.argmax(x, keepdims=True).shape, (2, 3))
 
     def test_argmin(self):
         x = KerasTensor((2, 3))
         self.assertEqual(knp.argmin(x).shape, ())
+        self.assertEqual(knp.argmin(x, keepdims=True).shape, (2, 3))
 
     def test_argsort(self):
         x = KerasTensor((2, 3))
         self.assertEqual(knp.argsort(x).shape, (2, 3))
         self.assertEqual(knp.argsort(x, axis=None).shape, (6,))
 
     def test_array(self):
@@ -3040,25 +3046,39 @@
 
         self.assertAllClose(knp.Arctanh()(x), np.arctanh(x))
 
     def test_argmax(self):
         x = np.array([[1, 2, 3], [3, 2, 1]])
         self.assertAllClose(knp.argmax(x), np.argmax(x))
         self.assertAllClose(knp.argmax(x, axis=1), np.argmax(x, axis=1))
+        self.assertAllClose(
+            knp.argmax(x, keepdims=True), np.argmax(x, keepdims=True)
+        )
 
         self.assertAllClose(knp.Argmax()(x), np.argmax(x))
         self.assertAllClose(knp.Argmax(axis=1)(x), np.argmax(x, axis=1))
 
+        self.assertAllClose(knp.Argmax()(x), np.argmax(x))
+        self.assertAllClose(
+            knp.Argmax(keepdims=True)(x), np.argmax(x, keepdims=True)
+        )
+
     def test_argmin(self):
         x = np.array([[1, 2, 3], [3, 2, 1]])
         self.assertAllClose(knp.argmin(x), np.argmin(x))
         self.assertAllClose(knp.argmin(x, axis=1), np.argmin(x, axis=1))
+        self.assertAllClose(
+            knp.argmin(x, keepdims=True), np.argmin(x, keepdims=True)
+        )
 
         self.assertAllClose(knp.Argmin()(x), np.argmin(x))
         self.assertAllClose(knp.Argmin(axis=1)(x), np.argmin(x, axis=1))
+        self.assertAllClose(
+            knp.Argmin(keepdims=True)(x), np.argmin(x, keepdims=True)
+        )
 
     def test_argsort(self):
         x = np.array([[1, 2, 3], [4, 5, 6]])
         self.assertAllClose(knp.argsort(x), np.argsort(x))
         self.assertAllClose(knp.argsort(x, axis=1), np.argsort(x, axis=1))
         self.assertAllClose(knp.argsort(x, axis=None), np.argsort(x, axis=None))
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/operation_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/ops/symbolic_arguments_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adadelta_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adafactor_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adagrad_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adam.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adam_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamax_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/adamw_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/ftrl_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/lion.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/lion_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/loss_scale_optimizer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/nadam_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer_sparse_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_sparse_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/optimizer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/rmsprop_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/schedules/learning_rate_schedule_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/optimizers/sgd_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/quantizers/quantizers_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/random/random.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/random/random_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/random/random_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/random/seed_generator.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/random/seed_generator_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/regularizers/regularizers_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/object_registration.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/object_registration_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_api.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_api_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/saving_lib_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/saving/serialization_lib_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_case.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/testing/test_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/compile_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/generator_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/py_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/epoch_iterator_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/trainer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/trainers/trainer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/tree/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/tree/tree_api.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/tree/tree_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/__init__.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/audio_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/code_stats.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/code_stats_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/dtype_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/file_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/file_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/image_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/io_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/io_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/jax_layer_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/module_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/naming.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/naming_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/numerical_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/progbar.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/python_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/python_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/rng_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/sequence_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/summary_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/text_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/timeseries_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/torch_utils_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/tracking.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras/src/utils/tracking_test.py` & `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024041803
+Version: 3.3.0.dev2024041903
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024041803/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/pyproject.toml` & `keras_nightly-3.3.0.dev2024041903/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041803/setup.py` & `keras_nightly-3.3.0.dev2024041903/setup.py`

 * *Files identical despite different names*

