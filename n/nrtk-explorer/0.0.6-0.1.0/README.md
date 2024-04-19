# Comparing `tmp/nrtk_explorer-0.0.6.tar.gz` & `tmp/nrtk_explorer-0.1.0.tar.gz`

## Comparing `nrtk_explorer-0.0.6.tar` & `nrtk_explorer-0.1.0.tar`

### file list

```diff
@@ -1,112 +1,117 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.flake8
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21233 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/screenshot.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/desktop/run.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16454 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0  3685868 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/requirements.txt
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/LICENSE
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/hatch_build.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.flake8
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    22291 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/screenshot.png
+-rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/usage.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0    14912 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/quasar.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify2.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/result_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/ml_models.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0  3685868 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/requirements.txt
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/hatch_build.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/PKG-INFO
```

### Comparing `nrtk_explorer-0.0.6/CHANGELOG.md` & `nrtk_explorer-0.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # CHANGELOG
 
 
 
+## v0.1.0 (2024-04-19)
+
+### Documentation
+
+* docs(readme): add usage section ([`7bfdbc4`](https://github.com/Kitware/nrtk-explorer/commit/7bfdbc4ad511eadda75c14aca3d310b2cd9a996a))
+
+* docs(readme): add usage example ([`b668617`](https://github.com/Kitware/nrtk-explorer/commit/b6686178eae2ea22be410260e4a3d1f1eb182403))
+
+### Feature
+
+* feat(web): add test apps ([`f58c6ea`](https://github.com/Kitware/nrtk-explorer/commit/f58c6eaf8b2cc27ea331afaa91423f81deeb551b))
+
+### Fix
+
+* fix(cli): update executable name to use - ([`cab041b`](https://github.com/Kitware/nrtk-explorer/commit/cab041b4ca675b0eaca9d6c02c93615a4f1806a8))
+
+* fix(dataset): better handling of dataset arg ([`b8bb107`](https://github.com/Kitware/nrtk-explorer/commit/b8bb1075b1a206118ce3c0d18ae726ee1f447dc8))
+
+### Unknown
+
+* Merge main to release ([`6e871d2`](https://github.com/Kitware/nrtk-explorer/commit/6e871d26b2039197bcc6b6e9c14c6e1495d6b9b0))
+
+* Auto-merge release back to main ([`2c3cd2b`](https://github.com/Kitware/nrtk-explorer/commit/2c3cd2b36508a43fccb595995ba5cc7a2ea9f7b1))
+
+
 ## v0.0.6 (2024-04-19)
 
 ### Fix
 
 * fix(nrtk-explorer): fix tests ([`2693689`](https://github.com/Kitware/nrtk-explorer/commit/269368975e16e21d9caf2575ebeba717c7ff7543))
 
 ### Unknown
```

### Comparing `nrtk_explorer-0.0.6/CONTRIBUTING.rst` & `nrtk_explorer-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/screenshot.png` & `nrtk_explorer-0.1.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/.github/workflows/ci.yml` & `nrtk_explorer-0.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/.github/workflows/create_release.yaml` & `nrtk_explorer-0.1.0/.github/workflows/create_release.yaml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/bundles/desktop/README.md` & `nrtk_explorer-0.1.0/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.1.0/bundles/docker/DEPLOY.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Trame deployment
 
 Trame applications can be deployed following different patterns.
 The one describe below is the simplest one and will only scale up to what the hardware is capable of handling.
-For infinit scaling feel free to consult [Kitware](https://www.kitware.com/contact/) for more guidance.
+For infinite scaling feel free to consult [Kitware](https://www.kitware.com/contact/) for more guidance.
 
 ## Docker
 
 This directory provide the core infrastructure for building docker images that can then be deployed your own way.
 But if you are looking for something more Heroku like we suggest using [CapRover](https://caprover.com/).
 
 ## Caprover
```

### Comparing `nrtk_explorer-0.0.6/bundles/docker/README.md` & `nrtk_explorer-0.1.0/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/examples/jupyter/show.ipynb` & `nrtk_explorer-0.1.0/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 Define your classes and create the instances that you need to expose
 """
 
 import logging
 from typing import Iterable
-from trame.app import get_server
+
 from trame.ui.quasar import QLayout
 from trame.widgets import quasar
 from trame.widgets import html
 from trame_server.utils.namespace import Translator
 from nrtk_explorer.library import images_manager
 from nrtk_explorer.library.filtering import FilterProtocol
 
@@ -57,29 +57,26 @@
 # ---------------------------------------------------------
 # Engine class
 # ---------------------------------------------------------
 
 
 class Engine(Applet):
     def __init__(self, server=None):
-        if server is None:
-            server = get_server()
-
         super().__init__(server)
 
         self.server.cli.add_argument(
             "--dataset",
             nargs="+",
             default=DEFAULT_DATASETS,
             help="Path of the json file describing the image dataset",
         )
 
         known_args, _ = self.server.cli.parse_known_args()
         self.input_paths = known_args.dataset
-        self.state.current_dataset = self.input_paths[0]
+        self.state.current_dataset = str(Path(self.input_paths[0]).resolve())
 
         self.context["image_objects"] = {}
         self.context["images_manager"] = images_manager.ImagesManager()
         self.context["annotations"] = {}
 
         self._ui = None
 
@@ -357,20 +354,7 @@
 
                                                     with quasar.QCardSection():
                                                         self._transforms_app.transformed_dataset_widget()
 
             self._ui = layout
 
         return self._ui
-
-
-def create_engine(server=None):
-    # Get or create server
-    if server is None:
-        server = get_server()
-
-    if isinstance(server, str):
-        server = get_server(server)
-
-    server.client_type = "vue3"
-
-    return Engine(server)
```

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/embeddings.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/transforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,19 +35,14 @@
     return f"{image_id}_meta"
 
 
 def image_id_to_result(image_id):
     return f"{image_id}_result"
 
 
-# ---------------------------------------------------------
-# Engine class
-# ---------------------------------------------------------
-
-
 DIR_NAME = os.path.dirname(nrtk_explorer.test_data.__file__)
 DATASET_DIRS = [
     f"{DIR_NAME}/OIRDS_v1_0/oirds.json",
     f"{DIR_NAME}/OIRDS_v1_0/oirds_test.json",
     f"{DIR_NAME}/OIRDS_v1_0/oirds_train.json",
 ]
 
@@ -120,15 +115,15 @@
         self._on_transform_fn = fn
 
     def on_transform(self, *args, **kwargs):
         if self._on_transform_fn:
             self._on_transform_fn(*args, **kwargs)
 
     def on_apply_transform(self, *args, **kwargs):
-        logger.info(">>> ENGINE(a): on_apply_transform")
+        logger.debug("on_apply_transform")
 
         current_transform = self.state.current_transform
         transformed_image_ids = []
         transform = self._transforms[current_transform]
         for image_id in self.state.source_image_ids:
             image = self.context["image_objects"][image_id]
 
@@ -269,15 +264,15 @@
             if self.state.has(meta_id) and self.state[meta_id] is not None:
                 self.state[meta_id] = None
 
             if image_id in self.context["image_objects"]:
                 del self.context["image_objects"][image_id]
 
     def on_current_dataset_change(self, current_dataset, **kwargs):
-        logger.info(f">>> ENGINE(a): on_current_dataset_change change {self.state}")
+        logger.debug(f"on_current_dataset_change change {self.state}")
 
         self.reset_data()
 
         with open(current_dataset) as f:
             dataset = json.load(f)
 
         categories = {}
@@ -293,15 +288,15 @@
         for i, image in enumerate(dataset["images"]):
             self.context.image_id_to_index[image["id"]] = i
 
         if self.is_standalone_app:
             self.context.images_manager = images_manager.ImagesManager()
 
     def on_feature_extraction_model_change(self, **kwargs):
-        logger.info(f">>> ENGINE(a): on_feature_extraction_model_change change {self.state}")
+        logger.debug(f">>> on_feature_extraction_model_change change {self.state}")
 
         feature_extraction_model = self.state.feature_extraction_model
 
         self.update_model_result(self.state.source_image_ids, feature_extraction_model)
         self.update_model_result(self.state.transformed_image_ids, feature_extraction_model)
 
     def update_model_result(self, image_ids, feature_extraction_model):
```

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/ml_models.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/ml_models.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json` & `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/tests/conftest.py` & `nrtk_explorer-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/tests/test_embeddings.py` & `nrtk_explorer-0.1.0/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/tests/test_filtering.py` & `nrtk_explorer-0.1.0/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/tests/test_object_detector.py` & `nrtk_explorer-0.1.0/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/package-lock.json` & `nrtk_explorer-0.1.0/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/package.json` & `nrtk_explorer-0.1.0/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/vite.config.ts` & `nrtk_explorer-0.1.0/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/ImageDetection.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.1.0/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/types/index.ts` & `nrtk_explorer-0.1.0/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.1.0/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/LICENSE` & `nrtk_explorer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/README.md` & `nrtk_explorer-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,35 +2,58 @@
 =============
 
 NRTK Explorer is a web application for exploring image datasets. It provides
 insights of a image dataset in [COCO][3] format and it evaluate image
 transformation and perturbation resilience of object recognition DL models. It
 is built using [trame][1] by the [kitware][2] team.
 
-![nrtk explorer](https://github.com/Kitware/nrtk-explorer/blob/d3df0ecf748664d806f09ad11e2bbd71a0bca1dd/screenshot.png?raw=true)
+![nrtk explorer](https://raw.githubusercontent.com/Kitware/nrtk-explorer/main/screenshot.png)
 
 Features
 --------
 
 - Explore image datasets in COCO format.
 - Apply parametrized image degradation (such as blur) to the images.
 - Benchmark dataset resilience with a differential PCA|UMAP analysis of the
   embeddings of the images and its transformation.
 - Evaluate object detection DL models in both the source images and its
   transformations.
 - When possible it will attempt to utilize the user GPU as much as possible to
   speedup its computations.
 
+Usage
+----------
+
+Usage example with virtual-env creation
+
+```bash
+# Setup python environment
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -U pip
+
+# install application
+pip install nrtk-explorer
+
+# get some sample data
+git clone https://github.com/vicentebolea/nrtk_explorer_datasets.git
+
+# Run the application on given dataset (908 images)
+nrtk-explorer --dataset ./nrtk_explorer_datasets/OIRDS_v1_0/oirds.json
+```
+
+![nrtk explorer usage](https://raw.githubusercontent.com/Kitware/nrtk-explorer/main/usage.png)
+
 Installing
 ----------
 
 Install it from pypi:
 
 ```bash
-pip install nrtk_explorer
+pip install nrtk-explorer
 ```
 
 Or, download and install it manually with:
 
 ```bash
 curl -OL https://github.com/Kitware/nrtk-explorer/archive/refs/heads/main.zip
 ```
@@ -40,15 +63,15 @@
 ```
 pip install -e .
 ```
 
 Run the application:
 
 ```
-nrtk_explorer
+nrtk-explorer
 ```
 
 CLI flags and options
 ---------------------
 
 - `-h|--help` show the help for the command line options, it inherit trame
   command line options and flags.
```

### Comparing `nrtk_explorer-0.0.6/hatch_build.py` & `nrtk_explorer-0.1.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.6/pyproject.toml` & `nrtk_explorer-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.0.6"
+version="0.1.0"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
@@ -64,25 +64,30 @@
 package = [
   "build<0.10.0",
   "python-semantic-release",
   "setuptools",
   "wheel",
 ]
 
+web = [
+  "trame-vtk",
+  "trame-vuetify",
+]
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.hooks.custom]
 
 [project.scripts]
-nrtk_explorer = "nrtk_explorer.app:main"
-nrtk_explorer_embeddings = "nrtk_explorer.app.embeddings:embeddings"
-nrtk_explorer_tranforms = "nrtk_explorer.app.transforms:transforms"
-nrtk_explorer_filtering = "nrtk_explorer.app.filtering:filtering"
+nrtk-explorer = "nrtk_explorer.app:main"
+nrtk-explorer-embeddings = "nrtk_explorer.app.embeddings:embeddings"
+nrtk-explorer-tranforms = "nrtk_explorer.app.transforms:transforms"
+nrtk-explorer-filtering = "nrtk_explorer.app.filtering:filtering"
 
 [tool.black]
 line-length = 99
 target-version = ['py39', 'py310', 'py311']
 include = '''
     \.pyi?$
 '''
```

### Comparing `nrtk_explorer-0.0.6/PKG-INFO` & `nrtk_explorer-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.0.6
+Version: 0.1.0
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
@@ -43,45 +43,71 @@
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: tabulate; extra == 'dev'
 Provides-Extra: package
 Requires-Dist: build<0.10.0; extra == 'package'
 Requires-Dist: python-semantic-release; extra == 'package'
 Requires-Dist: setuptools; extra == 'package'
 Requires-Dist: wheel; extra == 'package'
+Provides-Extra: web
+Requires-Dist: trame-vtk; extra == 'web'
+Requires-Dist: trame-vuetify; extra == 'web'
 Description-Content-Type: text/markdown
 
 NRTK EXPLORER
 =============
 
 NRTK Explorer is a web application for exploring image datasets. It provides
 insights of a image dataset in [COCO][3] format and it evaluate image
 transformation and perturbation resilience of object recognition DL models. It
 is built using [trame][1] by the [kitware][2] team.
 
-![nrtk explorer](https://github.com/Kitware/nrtk-explorer/blob/d3df0ecf748664d806f09ad11e2bbd71a0bca1dd/screenshot.png?raw=true)
+![nrtk explorer](https://raw.githubusercontent.com/Kitware/nrtk-explorer/main/screenshot.png)
 
 Features
 --------
 
 - Explore image datasets in COCO format.
 - Apply parametrized image degradation (such as blur) to the images.
 - Benchmark dataset resilience with a differential PCA|UMAP analysis of the
   embeddings of the images and its transformation.
 - Evaluate object detection DL models in both the source images and its
   transformations.
 - When possible it will attempt to utilize the user GPU as much as possible to
   speedup its computations.
 
+Usage
+----------
+
+Usage example with virtual-env creation
+
+```bash
+# Setup python environment
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -U pip
+
+# install application
+pip install nrtk-explorer
+
+# get some sample data
+git clone https://github.com/vicentebolea/nrtk_explorer_datasets.git
+
+# Run the application on given dataset (908 images)
+nrtk-explorer --dataset ./nrtk_explorer_datasets/OIRDS_v1_0/oirds.json
+```
+
+![nrtk explorer usage](https://raw.githubusercontent.com/Kitware/nrtk-explorer/main/usage.png)
+
 Installing
 ----------
 
 Install it from pypi:
 
 ```bash
-pip install nrtk_explorer
+pip install nrtk-explorer
 ```
 
 Or, download and install it manually with:
 
 ```bash
 curl -OL https://github.com/Kitware/nrtk-explorer/archive/refs/heads/main.zip
 ```
@@ -91,15 +117,15 @@
 ```
 pip install -e .
 ```
 
 Run the application:
 
 ```
-nrtk_explorer
+nrtk-explorer
 ```
 
 CLI flags and options
 ---------------------
 
 - `-h|--help` show the help for the command line options, it inherit trame
   command line options and flags.
```

