# Comparing `tmp/nrtk_explorer-0.1.0.tar.gz` & `tmp/nrtk_explorer-0.1.1.tar.gz`

## Comparing `nrtk_explorer-0.1.0.tar` & `nrtk_explorer-0.1.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.flake8
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    22291 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/screenshot.png
--rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/usage.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/desktop/run.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0    14912 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/quasar.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify2.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0  3685868 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/requirements.txt
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/hatch_build.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.flake8
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    22908 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/screenshot.png
+-rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/usage.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/quasar.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/vuetify2.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/vuetify3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/result_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/ml_models.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/requirements.txt
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/hatch_build.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.1/PKG-INFO
```

### Comparing `nrtk_explorer-0.1.0/CHANGELOG.md` & `nrtk_explorer-0.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.1.1 (2024-04-19)
+
+### Fix
+
+* fix(core): removed unused default dataset ([`5f870ef`](https://github.com/Kitware/nrtk-explorer/commit/5f870ef74d8445d786990641fdad12b8afa065f2))
+
+* fix(sample): sample dataset categories ([`e85de50`](https://github.com/Kitware/nrtk-explorer/commit/e85de50d59c26f97ddccf23c3d893353855a60d4))
+
+### Unknown
+
+* fix(workflow) workflow fixes ([`e7540f1`](https://github.com/Kitware/nrtk-explorer/commit/e7540f12e0f19e529b685160fc28d82a1567e8a6))
+
+* Auto-merge release back to main ([`f652c12`](https://github.com/Kitware/nrtk-explorer/commit/f652c1294fffc930fd6d06daa87d55386f812b0f))
+
+
 ## v0.1.0 (2024-04-19)
 
 ### Documentation
 
 * docs(readme): add usage section ([`7bfdbc4`](https://github.com/Kitware/nrtk-explorer/commit/7bfdbc4ad511eadda75c14aca3d310b2cd9a996a))
 
 * docs(readme): add usage example ([`b668617`](https://github.com/Kitware/nrtk-explorer/commit/b6686178eae2ea22be410260e4a3d1f1eb182403))
```

### Comparing `nrtk_explorer-0.1.0/CONTRIBUTING.rst` & `nrtk_explorer-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/screenshot.png` & `nrtk_explorer-0.1.1/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/usage.png` & `nrtk_explorer-0.1.1/usage.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/.github/workflows/ci.yml` & `nrtk_explorer-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/.github/workflows/create_release.yaml` & `nrtk_explorer-0.1.1/.github/workflows/create_release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: Create Release
 
 on:
   workflow_dispatch:
+  push:
+    branches:
+      - release
 
 jobs:
   push_to_release:
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: write
```

### Comparing `nrtk_explorer-0.1.0/bundles/desktop/README.md` & `nrtk_explorer-0.1.1/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.1.1/bundles/docker/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/bundles/docker/README.md` & `nrtk_explorer-0.1.1/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/examples/jupyter/show.ipynb` & `nrtk_explorer-0.1.1/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/applet.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/applet.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 HORIZONTAL_SPLIT_DEFAULT_VALUE = 17
 VERTICAL_SPLIT_DEFAULT_VALUE = 40
 
 DIR_NAME = os.path.dirname(nrtk_explorer.test_data.__file__)
 DEFAULT_DATASETS = [
     f"{DIR_NAME}/coco-od-2017/test_val2017.json",
-    f"{DIR_NAME}/OIRDS_v1_0/oirds.json",
 ]
 
 
 def image_id_to_meta(image_id):
     return f"{image_id}_meta"
```

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/embeddings.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/quasar.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/quasar.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify2.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/vuetify2.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/test/vuetify3.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/test/vuetify3.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/ml_models.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/ml_models.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.1.1/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.1.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.1.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.1.1/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/tests/conftest.py` & `nrtk_explorer-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/tests/test_embeddings.py` & `nrtk_explorer-0.1.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/tests/test_filtering.py` & `nrtk_explorer-0.1.1/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/tests/test_object_detector.py` & `nrtk_explorer-0.1.1/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/package-lock.json` & `nrtk_explorer-0.1.1/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/package.json` & `nrtk_explorer-0.1.1/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/vite.config.ts` & `nrtk_explorer-0.1.1/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/ImageDetection.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.1.1/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/types/index.ts` & `nrtk_explorer-0.1.1/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.1.1/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/LICENSE` & `nrtk_explorer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/README.md` & `nrtk_explorer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/hatch_build.py` & `nrtk_explorer-0.1.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.0/pyproject.toml` & `nrtk_explorer-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.1.0"
+version="0.1.1"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
@@ -124,16 +124,15 @@
   [ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"
   nvm install 20
   node -v
   npm -v
   python -m venv .venv
   source .venv/bin/activate
   pip install -U pip
-  python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
-  python -m pip install ".[package]"
+  python -m pip install "build<0.10.0" "python-semantic-release" "setuptools" "wheel"
   python -m build .
 """
 
 [tool.semantic_release.branches.main]
 match = "(release)"
 prerelease_token = "rc"
 prerelease = false
```

### Comparing `nrtk_explorer-0.1.0/PKG-INFO` & `nrtk_explorer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
```

