# Comparing `tmp/reflex-0.4.8a1.tar.gz` & `tmp/reflex-0.4.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.4.8a1.tar", max compression
+gzip compressed data, was "reflex-0.4.9a1.tar", max compression
```

## Comparing `reflex-0.4.8a1.tar` & `reflex-0.4.9a1.tar`

### file list

```diff
@@ -1,510 +1,498 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.8a1/LICENSE
--rw-r--r--   0        0        0     9568 2024-04-05 17:14:14.456384 reflex-0.4.8a1/README.md
--rw-r--r--   0        0        0     2922 2024-04-12 01:14:24.524384 reflex-0.4.8a1/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.8a1/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      861 2024-04-05 17:14:14.457193 reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.8a1/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.8a1/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.8a1/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.8a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.8a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.8a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.8a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.8a1/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.8a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.8a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.8a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.8a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0    21909 2024-04-12 01:14:12.255596 reflex-0.4.8a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5723 2024-04-05 17:14:14.458168 reflex-0.4.8a1/reflex/__init__.py
--rw-r--r--   0        0        0     7649 2024-04-06 01:20:11.620853 reflex-0.4.8a1/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.8a1/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.8a1/reflex/admin.py
--rw-r--r--   0        0        0    45016 2024-04-12 01:14:12.255992 reflex-0.4.8a1/reflex/app.py
--rw-r--r--   0        0        0     5010 2024-04-04 14:57:26.376271 reflex-0.4.8a1/reflex/app.pyi
--rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.8a1/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4250 2024-04-04 14:57:26.376408 reflex-0.4.8a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.8a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17037 2024-04-05 17:14:14.458702 reflex-0.4.8a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.8a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0    14024 2024-04-12 01:14:12.256301 reflex-0.4.8a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.8a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.8a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.8a1/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-04 14:57:26.376832 reflex-0.4.8a1/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.4.8a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.8a1/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-04-12 01:14:12.256423 reflex-0.4.8a1/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.8a1/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-04-12 01:14:12.256750 reflex-0.4.8a1/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.8a1/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-04-12 01:14:12.256848 reflex-0.4.8a1/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.8a1/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-04-12 01:14:12.257050 reflex-0.4.8a1/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.8a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-04-12 01:14:12.257244 reflex-0.4.8a1/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.8a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-04-12 01:14:12.257347 reflex-0.4.8a1/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.8a1/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-04 14:57:26.377962 reflex-0.4.8a1/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.8a1/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.8a1/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-04-12 01:14:12.257771 reflex-0.4.8a1/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.8a1/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-04-12 01:14:12.257918 reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-04-12 01:14:12.258034 reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-04-12 01:14:12.258149 reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-04-12 01:14:12.258264 reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12994 2024-04-12 01:14:12.258377 reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.258509 reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-04-12 01:14:12.258649 reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-04-12 01:14:12.258803 reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.8a1/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-04-12 01:14:12.258961 reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-04-12 01:14:12.259114 reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-04-12 01:14:12.259285 reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-04-12 01:14:12.259424 reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.8a1/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-04-12 01:14:12.259528 reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-04-12 01:14:12.259726 reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-04-12 01:14:12.259930 reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-04-12 01:14:12.260187 reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-04-12 01:14:12.260440 reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.8a1/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-04-12 01:14:12.260613 reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-04-12 01:14:12.260767 reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-04-12 01:14:12.260906 reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.380782 reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-04 14:57:26.380893 reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.8a1/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-04-12 01:14:12.261047 reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.8a1/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-04 14:57:26.381120 reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.8a1/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-04-12 01:14:12.261180 reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-04-12 01:14:12.261417 reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.8a1/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-04-12 01:14:12.261540 reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-04-12 01:14:12.261730 reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.8a1/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-04 14:57:26.381709 reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9357 2024-04-12 01:14:12.262316 reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.4.8a1/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-04-12 01:14:12.263294 reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-04-12 01:14:12.263866 reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.8a1/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-04 14:57:26.382156 reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.8a1/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.263981 reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.8a1/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-04-12 01:14:12.264203 reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-04 14:57:26.382551 reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.382659 reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.8a1/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-04-12 01:14:12.264318 reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.8a1/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-04-12 01:14:12.264413 reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.8a1/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-04-12 01:14:12.264513 reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.8a1/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-04-12 01:14:12.264634 reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.8a1/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-04-12 01:14:12.264741 reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.8a1/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-04-12 01:14:12.264933 reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.8a1/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-04-12 01:14:12.265035 reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-04-12 01:14:12.265136 reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.8a1/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-04-12 01:14:12.265267 reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-04-12 01:14:12.265632 reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.8a1/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.8a1/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-04-12 01:14:12.265841 reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.8a1/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-04-12 01:14:12.266058 reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.8a1/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-04 14:57:26.384173 reflex-0.4.8a1/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.8a1/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-04-12 01:14:12.266197 reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.8a1/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-04 14:57:26.384405 reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-04-12 01:14:12.266398 reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-04-12 01:14:12.266521 reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-04-12 01:14:12.266681 reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-04-12 01:14:12.266827 reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-04-12 01:14:12.266967 reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-04-12 01:14:12.267114 reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-04-12 01:14:12.267256 reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-04-12 01:14:12.267494 reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.8a1/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.8a1/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-04-12 01:14:12.267618 reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-04-12 01:14:12.267722 reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.8a1/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-04-12 01:14:12.267821 reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.8a1/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-04-12 01:14:12.267927 reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    66011 2024-04-12 01:14:12.268153 reflex-0.4.8a1/reflex/components/component.py
--rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.8a1/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.4.8a1/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-04 14:57:26.386284 reflex-0.4.8a1/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.8a1/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-04-12 01:14:12.268957 reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.8a1/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6291 2024-04-04 14:19:59.331531 reflex-0.4.8a1/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4642 2024-03-20 23:54:55.842359 reflex-0.4.8a1/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4149 2024-04-04 14:57:26.386549 reflex-0.4.8a1/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.8a1/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.8a1/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-04 14:57:26.386705 reflex-0.4.8a1/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.8a1/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.8a1/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.4.8a1/reflex/components/core/responsive.py
--rw-r--r--   0        0        0     9035 2024-04-12 01:14:12.269123 reflex-0.4.8a1/reflex/components/core/upload.py
--rw-r--r--   0        0        0     8596 2024-04-12 01:14:12.269265 reflex-0.4.8a1/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.4.8a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-04 14:19:59.332304 reflex-0.4.8a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31107 2024-04-04 14:57:26.387164 reflex-0.4.8a1/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-04 14:57:26.387318 reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.4.8a1/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.8a1/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.8a1/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.8a1/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.8a1/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.8a1/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.8a1/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-04-12 01:14:12.269384 reflex-0.4.8a1/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.8a1/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.8a1/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-04-12 01:14:12.269589 reflex-0.4.8a1/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20102 2024-04-05 17:14:14.460921 reflex-0.4.8a1/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99553 2024-04-12 01:14:12.269801 reflex-0.4.8a1/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.8a1/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-04-12 01:14:12.270476 reflex-0.4.8a1/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.8a1/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93567 2024-04-12 01:14:12.270712 reflex-0.4.8a1/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.8a1/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-04-12 01:14:12.270995 reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.8a1/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-04-12 01:14:12.271158 reflex-0.4.8a1/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.8a1/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-04-12 01:14:12.271357 reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.8a1/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-04-12 01:14:12.271561 reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.8a1/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-04-12 01:14:12.271965 reflex-0.4.8a1/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.8a1/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-04-12 01:14:12.272183 reflex-0.4.8a1/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.8a1/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.8a1/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-04-12 01:14:12.272607 reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.8a1/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.8a1/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34237 2024-04-04 14:57:26.389624 reflex-0.4.8a1/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37949 2024-04-12 01:14:12.272820 reflex-0.4.8a1/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.8a1/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    11448 2024-04-05 17:14:14.461428 reflex-0.4.8a1/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5278 2024-04-05 17:14:14.461583 reflex-0.4.8a1/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.8a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.8a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.8a1/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.8a1/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-04 14:57:26.390245 reflex-0.4.8a1/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.8a1/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.8a1/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-04-12 01:14:12.273046 reflex-0.4.8a1/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.8a1/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-04 14:57:26.390489 reflex-0.4.8a1/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.8a1/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-04-12 01:14:12.273179 reflex-0.4.8a1/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.8a1/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-04 14:57:26.390675 reflex-0.4.8a1/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.8a1/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.8a1/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-04-12 01:14:12.273411 reflex-0.4.8a1/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.8a1/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.8a1/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    26885 2024-04-12 01:14:12.273564 reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.8a1/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-04-12 01:14:12.273957 reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-04-12 01:14:12.274125 reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.8a1/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    47939 2024-04-12 01:14:12.274318 reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.8a1/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22784 2024-04-12 01:14:12.274470 reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.8a1/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16697 2024-04-12 01:14:12.275306 reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.8a1/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.8a1/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    24074 2024-04-12 01:14:12.275479 reflex-0.4.8a1/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    21283 2024-04-04 14:57:26.391843 reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-04 14:57:26.391969 reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0    40237 2024-02-17 20:02:02.428774 reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi
--rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-04 14:57:26.392096 reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0     5724 2024-02-17 20:02:02.429087 reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi
--rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-04 14:57:26.392242 reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9315 2024-04-04 14:57:26.392362 reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.8a1/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11758 2024-04-04 14:57:26.392476 reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-04 14:57:26.392589 reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.8a1/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-04 14:57:26.392715 reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-04 14:57:26.392804 reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-04 14:57:26.392918 reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0    44130 2024-02-17 20:02:02.432309 reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi
--rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-04 14:57:26.393065 reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-04 14:57:26.393223 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0    52185 2024-02-17 20:02:02.435613 reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi
--rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-04 14:57:26.393356 reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0    26453 2024-02-17 20:02:02.436260 reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi
--rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    11916 2024-04-04 14:57:26.393481 reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0    12021 2024-02-17 20:02:02.436631 reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi
--rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-04 14:57:26.393614 reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-04 14:57:26.393725 reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-04 14:57:26.393848 reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0    26222 2024-03-20 23:54:55.854920 reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi
--rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-04 14:57:26.393997 reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     6513 2024-02-17 20:02:02.439025 reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi
--rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.4.8a1/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-04 14:57:26.394155 reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-04 14:57:26.394306 reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-04 14:57:26.394440 reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-04 14:57:26.394593 reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.8a1/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-04 14:57:26.394744 reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    17321 2024-04-04 14:57:26.394873 reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-04 14:57:26.395020 reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    43043 2024-04-04 14:57:26.395140 reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0    43365 2024-02-17 20:02:02.442188 reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi
--rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-04 14:57:26.395307 reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7643 2024-04-04 14:57:26.395455 reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-04 14:57:26.395640 reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.395883 reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     6779 2024-04-04 14:57:26.396069 reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-04 14:57:26.396231 reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-04 14:57:26.396387 reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4889 2024-04-04 14:19:59.341578 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    29367 2024-04-04 14:57:26.396553 reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-04 14:57:26.396712 reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.396834 reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-04-04 14:57:26.396967 reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.8a1/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.8a1/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-04 14:57:26.397104 reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-04 14:57:26.397215 reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     8547 2024-02-17 20:02:02.446585 reflex-0.4.8a1/reflex/components/radix/themes/typography/em.pyi
--rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-04 14:57:26.397327 reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     8872 2024-02-17 20:02:02.446866 reflex-0.4.8a1/reflex/components/radix/themes/typography/kbd.pyi
--rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12063 2024-04-04 14:57:26.397447 reflex-0.4.8a1/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     8701 2024-02-17 20:02:02.447165 reflex-0.4.8a1/reflex/components/radix/themes/typography/quote.pyi
--rw-r--r--   0        0        0     8563 2024-02-17 20:02:02.447296 reflex-0.4.8a1/reflex/components/radix/themes/typography/strong.pyi
--rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-04 14:57:26.397579 reflex-0.4.8a1/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.8a1/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.8a1/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.275710 reflex-0.4.8a1/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.8a1/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-04-12 01:14:12.275922 reflex-0.4.8a1/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.8a1/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.276135 reflex-0.4.8a1/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.8a1/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.8a1/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-04-12 01:14:12.276362 reflex-0.4.8a1/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.8a1/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-04 14:57:26.398259 reflex-0.4.8a1/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.8a1/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-04-12 01:14:12.276538 reflex-0.4.8a1/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.8a1/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-04-12 01:14:12.276828 reflex-0.4.8a1/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.8a1/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-04-12 01:14:12.277140 reflex-0.4.8a1/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.8a1/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.8a1/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-04 14:57:26.398718 reflex-0.4.8a1/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.8a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.8a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.8a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.8a1/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.8a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.8a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    11082 2024-04-05 17:14:06.328847 reflex-0.4.8a1/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.4.8a1/reflex/config.pyi
--rw-r--r--   0        0        0     2128 2024-04-12 01:14:12.277275 reflex-0.4.8a1/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5833 2024-04-12 01:14:12.277500 reflex-0.4.8a1/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-05 17:14:14.462329 reflex-0.4.8a1/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.8a1/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.4.8a1/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.8a1/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.8a1/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.8a1/reflex/constants/event.py
--rw-r--r--   0        0        0     3223 2024-04-12 01:14:12.277858 reflex-0.4.8a1/reflex/constants/installer.py
--rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.8a1/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.8a1/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.8a1/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    31705 2024-04-11 18:27:43.382941 reflex-0.4.8a1/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    26537 2024-04-12 01:14:12.278011 reflex-0.4.8a1/reflex/event.py
--rw-r--r--   0        0        0      369 2024-04-12 01:14:12.278154 reflex-0.4.8a1/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     1647 2024-04-05 17:14:14.462793 reflex-0.4.8a1/reflex/experimental/hooks.py
--rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.4.8a1/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.8a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.8a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13116 2024-04-12 01:14:12.278614 reflex-0.4.8a1/reflex/model.py
--rw-r--r--   0        0        0     1921 2024-04-05 17:14:14.463098 reflex-0.4.8a1/reflex/page.py
--rw-r--r--   0        0        0    17828 2024-04-12 01:14:12.279090 reflex-0.4.8a1/reflex/reflex.py
--rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.8a1/reflex/route.py
--rw-r--r--   0        0        0   105642 2024-04-04 14:57:26.399697 reflex-0.4.8a1/reflex/state.py
--rw-r--r--   0        0        0     8834 2024-04-04 14:57:26.399846 reflex-0.4.8a1/reflex/style.py
--rw-r--r--   0        0        0    29808 2024-04-05 17:14:14.463602 reflex-0.4.8a1/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.8a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.8a1/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.4.8a1/reflex/utils/compat.py
--rw-r--r--   0        0        0     5168 2024-04-12 01:14:12.279640 reflex-0.4.8a1/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.8a1/reflex/utils/exceptions.py
--rw-r--r--   0        0        0     9969 2024-04-05 17:14:14.463946 reflex-0.4.8a1/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.4.8a1/reflex/utils/export.py
--rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.8a1/reflex/utils/format.py
--rw-r--r--   0        0        0     2277 2024-04-12 01:14:12.280013 reflex-0.4.8a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.8a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    46993 2024-04-12 01:14:12.280227 reflex-0.4.8a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    10050 2024-04-12 01:14:12.280420 reflex-0.4.8a1/reflex/utils/processes.py
--rw-r--r--   0        0        0    27674 2024-04-04 14:57:26.400476 reflex-0.4.8a1/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     8771 2024-04-11 18:27:43.383699 reflex-0.4.8a1/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4013 2024-04-04 14:57:26.400591 reflex-0.4.8a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    13679 2024-04-12 01:14:12.280735 reflex-0.4.8a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.8a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    67152 2024-04-04 14:57:26.400899 reflex-0.4.8a1/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.4.8a1/reflex/vars.pyi
--rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 reflex-0.4.8a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.4.9a1/LICENSE
+-rw-r--r--   0        0        0     9568 2024-04-05 17:14:14.456384 reflex-0.4.9a1/README.md
+-rw-r--r--   0        0        0     2922 2024-04-19 15:26:57.528066 reflex-0.4.9a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.4.9a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.4.9a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-05 17:14:14.457193 reflex-0.4.9a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.4.9a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.4.9a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.4.9a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.4.9a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.4.9a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.4.9a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.4.9a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2928 2024-02-17 20:02:02.399454 reflex-0.4.9a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10910 2024-03-20 23:54:55.829615 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8383 2024-03-20 23:54:55.830163 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.4.9a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.4.9a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.4.9a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.4.9a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.4.9a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.4.9a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.4.9a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.4.9a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.4.9a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.4.9a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.4.9a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.4.9a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.4.9a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.4.9a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      436 2024-02-06 00:51:31.970725 reflex-0.4.9a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.4.9a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.4.9a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.4.9a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.4.9a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.4.9a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.4.9a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.4.9a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.4.9a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.4.9a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.4.9a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.4.9a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.4.9a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0    21909 2024-04-12 01:14:12.255596 reflex-0.4.9a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5723 2024-04-05 17:14:14.458168 reflex-0.4.9a1/reflex/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-06 01:20:11.620853 reflex-0.4.9a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.4.9a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.4.9a1/reflex/admin.py
+-rw-r--r--   0        0        0    45016 2024-04-12 01:14:12.255992 reflex-0.4.9a1/reflex/app.py
+-rw-r--r--   0        0        0     5010 2024-04-04 14:57:26.376271 reflex-0.4.9a1/reflex/app.pyi
+-rw-r--r--   0        0        0     1152 2024-03-20 23:54:55.837204 reflex-0.4.9a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4250 2024-04-04 14:57:26.376408 reflex-0.4.9a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.4.9a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17037 2024-04-05 17:14:14.458702 reflex-0.4.9a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.4.9a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    14024 2024-04-12 01:14:12.256301 reflex-0.4.9a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      530 2024-02-17 20:02:02.404048 reflex-0.4.9a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.4.9a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.4.9a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-04 14:57:26.376832 reflex-0.4.9a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.4.9a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.4.9a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-04-12 01:14:12.256423 reflex-0.4.9a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.4.9a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-04-12 01:14:12.256750 reflex-0.4.9a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.4.9a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-04-12 01:14:12.256848 reflex-0.4.9a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.4.9a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-04-12 01:14:12.257050 reflex-0.4.9a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.4.9a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-04-12 01:14:12.257244 reflex-0.4.9a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.4.9a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-04-12 01:14:12.257347 reflex-0.4.9a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.4.9a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-04 14:57:26.377962 reflex-0.4.9a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.4.9a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.4.9a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-04-12 01:14:12.257771 reflex-0.4.9a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.4.9a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.4.9a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-04-12 01:14:12.257918 reflex-0.4.9a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.4.9a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-04-12 01:14:12.258034 reflex-0.4.9a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.4.9a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-04-12 01:14:12.258149 reflex-0.4.9a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.4.9a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-04-12 01:14:12.258264 reflex-0.4.9a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1505 2024-02-07 21:48:43.272557 reflex-0.4.9a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12994 2024-04-12 01:14:12.258377 reflex-0.4.9a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.4.9a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.258509 reflex-0.4.9a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.4.9a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-04-12 01:14:12.258649 reflex-0.4.9a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.4.9a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-04-12 01:14:12.258803 reflex-0.4.9a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.4.9a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3509 2024-02-07 21:48:43.274196 reflex-0.4.9a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-04-12 01:14:12.258961 reflex-0.4.9a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.4.9a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-04-12 01:14:12.259114 reflex-0.4.9a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.4.9a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-04-12 01:14:12.259285 reflex-0.4.9a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.4.9a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-04-12 01:14:12.259424 reflex-0.4.9a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.4.9a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.4.9a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-04-12 01:14:12.259528 reflex-0.4.9a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.4.9a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-04-12 01:14:12.259726 reflex-0.4.9a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.4.9a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-04-12 01:14:12.259930 reflex-0.4.9a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.4.9a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-04-12 01:14:12.260187 reflex-0.4.9a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.4.9a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-04-12 01:14:12.260440 reflex-0.4.9a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.4.9a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.4.9a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-04-12 01:14:12.260613 reflex-0.4.9a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.4.9a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-04-12 01:14:12.260767 reflex-0.4.9a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.4.9a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-04-12 01:14:12.260906 reflex-0.4.9a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.4.9a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.380782 reflex-0.4.9a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.4.9a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-04 14:57:26.380893 reflex-0.4.9a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.4.9a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-04-12 01:14:12.261047 reflex-0.4.9a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.4.9a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-04 14:57:26.381120 reflex-0.4.9a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.4.9a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-04-12 01:14:12.261180 reflex-0.4.9a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.4.9a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-04-12 01:14:12.261417 reflex-0.4.9a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.4.9a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-04-12 01:14:12.261540 reflex-0.4.9a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.4.9a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.4.9a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-04-12 01:14:12.261730 reflex-0.4.9a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.4.9a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-04 14:57:26.381709 reflex-0.4.9a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.4.9a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9357 2024-04-12 01:14:12.262316 reflex-0.4.9a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.4.9a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-04-12 01:14:12.263294 reflex-0.4.9a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.4.9a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-04-12 01:14:12.263866 reflex-0.4.9a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.4.9a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-04 14:57:26.382156 reflex-0.4.9a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.4.9a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-04-12 01:14:12.263981 reflex-0.4.9a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.4.9a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-04-12 01:14:12.264203 reflex-0.4.9a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.4.9a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-04 14:57:26.382551 reflex-0.4.9a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.4.9a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-04 14:57:26.382659 reflex-0.4.9a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.4.9a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.4.9a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-04-12 01:14:12.264318 reflex-0.4.9a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.4.9a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-04-12 01:14:12.264413 reflex-0.4.9a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.4.9a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-04-12 01:14:12.264513 reflex-0.4.9a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.4.9a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-04-12 01:14:12.264634 reflex-0.4.9a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.4.9a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-04-12 01:14:12.264741 reflex-0.4.9a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.4.9a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-04-12 01:14:12.264933 reflex-0.4.9a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.4.9a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-04-12 01:14:12.265035 reflex-0.4.9a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.4.9a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-04-12 01:14:12.265136 reflex-0.4.9a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.4.9a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-04-12 01:14:12.265267 reflex-0.4.9a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.4.9a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-04-12 01:14:12.265632 reflex-0.4.9a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.4.9a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.4.9a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-04-12 01:14:12.265841 reflex-0.4.9a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2461 2024-02-06 00:51:31.985395 reflex-0.4.9a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-04-12 01:14:12.266058 reflex-0.4.9a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.4.9a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-04 14:57:26.384173 reflex-0.4.9a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.4.9a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.4.9a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-04-12 01:14:12.266197 reflex-0.4.9a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.4.9a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-04 14:57:26.384405 reflex-0.4.9a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.4.9a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-04-12 01:14:12.266398 reflex-0.4.9a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.4.9a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-04-12 01:14:12.266521 reflex-0.4.9a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.4.9a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.4.9a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-04-12 01:14:12.266681 reflex-0.4.9a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.4.9a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-04-12 01:14:12.266827 reflex-0.4.9a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.4.9a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-04-12 01:14:12.266967 reflex-0.4.9a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.4.9a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-04-12 01:14:12.267114 reflex-0.4.9a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.4.9a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-04-12 01:14:12.267256 reflex-0.4.9a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.4.9a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-04-12 01:14:12.267494 reflex-0.4.9a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.4.9a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.4.9a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-04-12 01:14:12.267618 reflex-0.4.9a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.4.9a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-04-12 01:14:12.267722 reflex-0.4.9a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.4.9a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-04-12 01:14:12.267821 reflex-0.4.9a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.4.9a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-04-12 01:14:12.267927 reflex-0.4.9a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    66268 2024-04-19 15:24:58.765679 reflex-0.4.9a1/reflex/components/component.py
+-rw-r--r--   0        0        0      844 2024-03-20 23:54:55.841256 reflex-0.4.9a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.4.9a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    17164 2024-04-04 14:57:26.386284 reflex-0.4.9a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.4.9a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-04-12 01:14:12.268957 reflex-0.4.9a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.4.9a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6291 2024-04-04 14:19:59.331531 reflex-0.4.9a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4763 2024-04-17 23:04:42.683198 reflex-0.4.9a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4149 2024-04-04 14:57:26.386549 reflex-0.4.9a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4031 2024-02-06 00:51:31.992601 reflex-0.4.9a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1033 2024-02-17 20:02:02.418184 reflex-0.4.9a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-04 14:57:26.386705 reflex-0.4.9a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.4.9a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9989 2024-02-17 20:02:02.418463 reflex-0.4.9a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.4.9a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0     9035 2024-04-12 01:14:12.269123 reflex-0.4.9a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0     8596 2024-04-12 01:14:12.269265 reflex-0.4.9a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.4.9a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-04 14:19:59.332304 reflex-0.4.9a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31107 2024-04-04 14:57:26.387164 reflex-0.4.9a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.4.9a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-04 14:57:26.387318 reflex-0.4.9a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.4.9a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.4.9a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.4.9a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.4.9a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.4.9a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.4.9a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.4.9a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-04-12 01:14:12.269384 reflex-0.4.9a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.4.9a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.4.9a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-04-12 01:14:12.269589 reflex-0.4.9a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20102 2024-04-05 17:14:14.460921 reflex-0.4.9a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99553 2024-04-12 01:14:12.269801 reflex-0.4.9a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.4.9a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-04-12 01:14:12.270476 reflex-0.4.9a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.4.9a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93567 2024-04-12 01:14:12.270712 reflex-0.4.9a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.4.9a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-04-12 01:14:12.270995 reflex-0.4.9a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.4.9a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-04-12 01:14:12.271158 reflex-0.4.9a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.4.9a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-04-12 01:14:12.271357 reflex-0.4.9a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.4.9a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-04-12 01:14:12.271561 reflex-0.4.9a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.4.9a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-04-12 01:14:12.271965 reflex-0.4.9a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.4.9a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-04-12 01:14:12.272183 reflex-0.4.9a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.4.9a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.4.9a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-04-12 01:14:12.272607 reflex-0.4.9a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.4.9a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.4.9a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34237 2024-04-04 14:57:26.389624 reflex-0.4.9a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37949 2024-04-12 01:14:12.272820 reflex-0.4.9a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.4.9a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    11448 2024-04-05 17:14:14.461428 reflex-0.4.9a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5278 2024-04-05 17:14:14.461583 reflex-0.4.9a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.4.9a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.4.9a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.4.9a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.4.9a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-04 14:57:26.390245 reflex-0.4.9a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.4.9a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.4.9a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-04-12 01:14:12.273046 reflex-0.4.9a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.4.9a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-04 14:57:26.390489 reflex-0.4.9a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.4.9a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-04-12 01:14:12.273179 reflex-0.4.9a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.4.9a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-04 14:57:26.390675 reflex-0.4.9a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.4.9a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.4.9a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-04-12 01:14:12.273411 reflex-0.4.9a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.4.9a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.4.9a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    21406 2024-03-20 23:54:55.846431 reflex-0.4.9a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    26885 2024-04-12 01:14:12.273564 reflex-0.4.9a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.4.9a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-04-12 01:14:12.273957 reflex-0.4.9a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.4.9a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-04-12 01:14:12.274125 reflex-0.4.9a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4760 2024-03-20 23:54:55.847327 reflex-0.4.9a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    47939 2024-04-12 01:14:12.274318 reflex-0.4.9a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     3996 2024-03-20 23:54:55.847641 reflex-0.4.9a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22784 2024-04-12 01:14:12.274470 reflex-0.4.9a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5004 2024-03-20 23:54:55.848258 reflex-0.4.9a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16697 2024-04-12 01:14:12.275306 reflex-0.4.9a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.4.9a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-20 23:54:55.848920 reflex-0.4.9a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    24074 2024-04-12 01:14:12.275479 reflex-0.4.9a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     3007 2024-03-20 23:54:55.849383 reflex-0.4.9a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    21283 2024-04-04 14:57:26.391843 reflex-0.4.9a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     1776 2024-02-17 20:02:02.427848 reflex-0.4.9a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.4.9a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-04 14:57:26.391969 reflex-0.4.9a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.4.9a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-04 14:57:26.392096 reflex-0.4.9a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.4.9a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-04 14:57:26.392242 reflex-0.4.9a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      815 2024-02-17 20:02:02.429580 reflex-0.4.9a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9315 2024-04-04 14:57:26.392362 reflex-0.4.9a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1084 2024-02-17 20:02:02.429875 reflex-0.4.9a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11758 2024-04-04 14:57:26.392476 reflex-0.4.9a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.4.9a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-04 14:57:26.392589 reflex-0.4.9a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.4.9a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-04 14:57:26.392715 reflex-0.4.9a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.4.9a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-04 14:57:26.392804 reflex-0.4.9a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.4.9a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-04 14:57:26.392918 reflex-0.4.9a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.4.9a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-04 14:57:26.393065 reflex-0.4.9a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.4.9a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-04 14:57:26.393223 reflex-0.4.9a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.4.9a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-04 14:57:26.393356 reflex-0.4.9a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0     2789 2024-03-20 23:54:55.853758 reflex-0.4.9a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    11916 2024-04-04 14:57:26.393481 reflex-0.4.9a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.4.9a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-04 14:57:26.393614 reflex-0.4.9a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.4.9a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-04 14:57:26.393725 reflex-0.4.9a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     6253 2024-03-20 23:54:55.854319 reflex-0.4.9a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-04 14:57:26.393848 reflex-0.4.9a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.4.9a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-04 14:57:26.393997 reflex-0.4.9a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.4.9a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-04 14:57:26.394155 reflex-0.4.9a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.4.9a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-04 14:57:26.394306 reflex-0.4.9a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.4.9a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-04 14:57:26.394440 reflex-0.4.9a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.4.9a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-04 14:57:26.394593 reflex-0.4.9a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.4.9a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-04 14:57:26.394744 reflex-0.4.9a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2213 2024-03-20 23:54:55.858062 reflex-0.4.9a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    17321 2024-04-04 14:57:26.394873 reflex-0.4.9a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.4.9a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-04 14:57:26.395020 reflex-0.4.9a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     5106 2024-03-20 23:54:55.858542 reflex-0.4.9a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    43043 2024-04-04 14:57:26.395140 reflex-0.4.9a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.4.9a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-04 14:57:26.395307 reflex-0.4.9a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.4.9a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1201 2024-03-20 23:54:55.859150 reflex-0.4.9a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7643 2024-04-04 14:57:26.395455 reflex-0.4.9a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.4.9a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-04 14:57:26.395640 reflex-0.4.9a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      422 2024-03-20 23:54:55.859399 reflex-0.4.9a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.395883 reflex-0.4.9a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0      552 2024-02-07 21:48:43.319123 reflex-0.4.9a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     6779 2024-04-04 14:57:26.396069 reflex-0.4.9a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.4.9a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-04 14:57:26.396231 reflex-0.4.9a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.4.9a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-04 14:57:26.396387 reflex-0.4.9a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4889 2024-04-04 14:19:59.341578 reflex-0.4.9a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29367 2024-04-04 14:57:26.396553 reflex-0.4.9a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.4.9a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-04 14:57:26.396712 reflex-0.4.9a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      412 2024-03-20 23:54:55.861110 reflex-0.4.9a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8245 2024-04-04 14:57:26.396834 reflex-0.4.9a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1270 2024-03-20 23:54:55.861618 reflex-0.4.9a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-04-04 14:57:26.396967 reflex-0.4.9a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.4.9a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.4.9a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.4.9a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-04 14:57:26.397104 reflex-0.4.9a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.4.9a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-04 14:57:26.397215 reflex-0.4.9a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.4.9a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-04 14:57:26.397327 reflex-0.4.9a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     3154 2024-03-20 23:54:55.862398 reflex-0.4.9a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12063 2024-04-04 14:57:26.397447 reflex-0.4.9a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.4.9a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-04 14:57:26.397579 reflex-0.4.9a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.4.9a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.4.9a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.275710 reflex-0.4.9a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.4.9a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-04-12 01:14:12.275922 reflex-0.4.9a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.4.9a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-04-12 01:14:12.276135 reflex-0.4.9a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.4.9a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.4.9a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-04-12 01:14:12.276362 reflex-0.4.9a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.4.9a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-04 14:57:26.398259 reflex-0.4.9a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-02-06 00:51:32.028409 reflex-0.4.9a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-04-12 01:14:12.276538 reflex-0.4.9a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.4.9a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-04-12 01:14:12.276828 reflex-0.4.9a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.4.9a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-04-12 01:14:12.277140 reflex-0.4.9a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.4.9a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.4.9a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-04 14:57:26.398718 reflex-0.4.9a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.4.9a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.4.9a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3620 2024-02-06 00:51:32.029458 reflex-0.4.9a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.4.9a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.4.9a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.4.9a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    11082 2024-04-05 17:14:06.328847 reflex-0.4.9a1/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.4.9a1/reflex/config.pyi
+-rw-r--r--   0        0        0     2128 2024-04-12 01:14:12.277275 reflex-0.4.9a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5833 2024-04-12 01:14:12.277500 reflex-0.4.9a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-05 17:14:14.462329 reflex-0.4.9a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1599 2024-03-20 23:54:55.865089 reflex-0.4.9a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.4.9a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.4.9a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.4.9a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.4.9a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3223 2024-04-12 01:14:12.277858 reflex-0.4.9a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     1940 2024-03-20 23:54:55.865486 reflex-0.4.9a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.4.9a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.4.9a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    31705 2024-04-11 18:27:43.382941 reflex-0.4.9a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    26537 2024-04-12 01:14:12.278011 reflex-0.4.9a1/reflex/event.py
+-rw-r--r--   0        0        0      425 2024-04-19 15:24:58.765994 reflex-0.4.9a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     2196 2024-04-19 15:24:58.766647 reflex-0.4.9a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0     6770 2024-04-19 15:24:58.766984 reflex-0.4.9a1/reflex/experimental/layout.py
+-rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.4.9a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.4.9a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.4.9a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.4.9a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13116 2024-04-12 01:14:12.278614 reflex-0.4.9a1/reflex/model.py
+-rw-r--r--   0        0        0     1921 2024-04-05 17:14:14.463098 reflex-0.4.9a1/reflex/page.py
+-rw-r--r--   0        0        0    17828 2024-04-12 01:14:12.279090 reflex-0.4.9a1/reflex/reflex.py
+-rw-r--r--   0        0        0     2908 2024-03-20 23:54:55.866329 reflex-0.4.9a1/reflex/route.py
+-rw-r--r--   0        0        0   105642 2024-04-04 14:57:26.399697 reflex-0.4.9a1/reflex/state.py
+-rw-r--r--   0        0        0     8834 2024-04-04 14:57:26.399846 reflex-0.4.9a1/reflex/style.py
+-rw-r--r--   0        0        0    30556 2024-04-19 15:24:58.767239 reflex-0.4.9a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.4.9a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.4.9a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.4.9a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5168 2024-04-12 01:14:12.279640 reflex-0.4.9a1/reflex/utils/console.py
+-rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.4.9a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0     9969 2024-04-05 17:14:14.463946 reflex-0.4.9a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.4.9a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    22648 2024-03-20 23:54:55.867980 reflex-0.4.9a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2277 2024-04-12 01:14:12.280013 reflex-0.4.9a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.4.9a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    47242 2024-04-19 15:24:58.767513 reflex-0.4.9a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    10730 2024-04-19 15:24:58.767773 reflex-0.4.9a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    27674 2024-04-04 14:57:26.400476 reflex-0.4.9a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     9023 2024-04-17 23:04:42.684666 reflex-0.4.9a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4013 2024-04-04 14:57:26.400591 reflex-0.4.9a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    13679 2024-04-12 01:14:12.280735 reflex-0.4.9a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.4.9a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    67157 2024-04-19 15:24:58.768195 reflex-0.4.9a1/reflex/vars.py
+-rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.4.9a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 reflex-0.4.9a1/PKG-INFO
```

### Comparing `reflex-0.4.8a1/LICENSE` & `reflex-0.4.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/README.md` & `reflex-0.4.9a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/pyproject.toml` & `reflex-0.4.9a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.4.8a1"
+version = "0.4.9a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.4.9a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.4.9a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.4.9a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.4.9a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.4.9a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.4.9a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.4.9a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.4.9a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.4.9a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.4.9a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.4.9a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.4.9a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.4.9a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.4.9a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/.templates/web/utils/state.js` & `reflex-0.4.9a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/__init__.py` & `reflex-0.4.9a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/__init__.pyi` & `reflex-0.4.9a1/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/app.py` & `reflex-0.4.9a1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/app.pyi` & `reflex-0.4.9a1/reflex/app.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/app_module_for_backend.py` & `reflex-0.4.9a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/base.py` & `reflex-0.4.9a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/compiler/compiler.py` & `reflex-0.4.9a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/compiler/templates.py` & `reflex-0.4.9a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/compiler/utils.py` & `reflex-0.4.9a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/__init__.py` & `reflex-0.4.9a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/app_wrap.py` & `reflex-0.4.9a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/app_wrap.pyi` & `reflex-0.4.9a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/bare.py` & `reflex-0.4.9a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/body.pyi` & `reflex-0.4.9a1/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/document.py` & `reflex-0.4.9a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/document.pyi` & `reflex-0.4.9a1/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/fragment.pyi` & `reflex-0.4.9a1/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/head.pyi` & `reflex-0.4.9a1/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/link.py` & `reflex-0.4.9a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/link.pyi` & `reflex-0.4.9a1/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/meta.py` & `reflex-0.4.9a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/meta.pyi` & `reflex-0.4.9a1/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/script.py` & `reflex-0.4.9a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/base/script.pyi` & `reflex-0.4.9a1/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/__init__.py` & `reflex-0.4.9a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/base.py` & `reflex-0.4.9a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/base.pyi` & `reflex-0.4.9a1/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.py` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.py` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.4.9a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.py` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.4.9a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.py` & `reflex-0.4.9a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.4.9a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.4.9a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.4.9a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.py` & `reflex-0.4.9a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.4.9a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.4.9a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.4.9a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.py` & `reflex-0.4.9a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.4.9a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/__init__.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/button.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/button.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/editable.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/editable.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/email.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/form.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/form.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/input.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/input.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/multiselect.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/password.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/radio.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/radio.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/select.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/select.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/slider.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/slider.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/switch.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/switch.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.py` & `reflex-0.4.9a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.4.9a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/box.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/box.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/card.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/card.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/center.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/container.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/flex.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/flex.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/grid.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/grid.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/stack.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/stack.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.py` & `reflex-0.4.9a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.4.9a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/avatar.py` & `reflex-0.4.9a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/avatar.pyi` & `reflex-0.4.9a1/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/icon.py` & `reflex-0.4.9a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/icon.pyi` & `reflex-0.4.9a1/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/image.py` & `reflex-0.4.9a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/media/image.pyi` & `reflex-0.4.9a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.4.9a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.4.9a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/link.py` & `reflex-0.4.9a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/link.pyi` & `reflex-0.4.9a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.4.9a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.4.9a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.py` & `reflex-0.4.9a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.4.9a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/__init__.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.4.9a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.4.9a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/typography/heading.pyi` & `reflex-0.4.9a1/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.py` & `reflex-0.4.9a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.4.9a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/typography/span.pyi` & `reflex-0.4.9a1/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/chakra/typography/text.pyi` & `reflex-0.4.9a1/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/component.py` & `reflex-0.4.9a1/reflex/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,17 +658,19 @@
         # Validate all the children.
         validate_children(children)
 
         children = [
             (
                 child
                 if isinstance(child, Component)
-                else Fragment.create(*child)
-                if isinstance(child, tuple)
-                else Bare.create(contents=Var.create(child, _var_is_string=True))
+                else (
+                    Fragment.create(*child)
+                    if isinstance(child, tuple)
+                    else Bare.create(contents=Var.create(child, _var_is_string=True))
+                )
             )
             for child in children
         ]
 
         return cls(children=children, **props)
 
     def _add_style(self, style: dict):
@@ -1049,14 +1051,19 @@
             # Handle additional internal hooks (autofocus, etc).
             _imports.setdefault("react", set()).update(
                 {
                     ImportVar(tag="useRef"),
                     ImportVar(tag="useEffect"),
                 },
             )
+
+        user_hooks = self._get_hooks()
+        if user_hooks is not None and isinstance(user_hooks, Var):
+            _imports = imports.merge_imports(_imports, user_hooks._var_data.imports)  # type: ignore
+
         return _imports
 
     def _get_imports(self) -> imports.ImportDict:
         """Get all the libraries and fields that are used by the component.
 
         Returns:
             The imports needed by the component.
```

### Comparing `reflex-0.4.8a1/reflex/components/core/__init__.py` & `reflex-0.4.9a1/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/banner.py` & `reflex-0.4.9a1/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/banner.pyi` & `reflex-0.4.9a1/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/client_side_routing.py` & `reflex-0.4.9a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/client_side_routing.pyi` & `reflex-0.4.9a1/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/colors.py` & `reflex-0.4.9a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/cond.py` & `reflex-0.4.9a1/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/debounce.py` & `reflex-0.4.9a1/reflex/components/core/debounce.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 
         # Carry known props and event_triggers from the child.
         props_from_child = {
             p: getattr(child, p)
             for p in cls.get_props()
             if getattr(child, p, None) is not None
         }
-        props_from_child.update(child.event_triggers)
+        props[EventTriggers.ON_CHANGE] = child.event_triggers.pop(
+            EventTriggers.ON_CHANGE
+        )
         props = {**props_from_child, **props}
 
         # Carry all other child props directly via custom_attrs
         other_props = {
             p: getattr(child, p)
             for p in child.get_props()
             if p not in props_from_child and getattr(child, p) is not None
@@ -113,14 +115,15 @@
                     hooks=child._get_hooks_internal(),
                 ),
             ),
         )
 
         component = super().create(**props)
         component._get_style = child._get_style
+        component.event_triggers.update(child.event_triggers)
         return component
 
     def get_event_triggers(self) -> dict[str, Any]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
```

### Comparing `reflex-0.4.8a1/reflex/components/core/debounce.pyi` & `reflex-0.4.9a1/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/foreach.py` & `reflex-0.4.9a1/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/html.py` & `reflex-0.4.9a1/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/html.pyi` & `reflex-0.4.9a1/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/match.py` & `reflex-0.4.9a1/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/responsive.py` & `reflex-0.4.9a1/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/upload.py` & `reflex-0.4.9a1/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/core/upload.pyi` & `reflex-0.4.9a1/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/datadisplay/code.py` & `reflex-0.4.9a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/datadisplay/code.pyi` & `reflex-0.4.9a1/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.py` & `reflex-0.4.9a1/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.4.9a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/datadisplay/logo.py` & `reflex-0.4.9a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/constants/html.py` & `reflex-0.4.9a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/constants/react.py` & `reflex-0.4.9a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/constants/reflex.py` & `reflex-0.4.9a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/element.pyi` & `reflex-0.4.9a1/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/__init__.py` & `reflex-0.4.9a1/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/base.py` & `reflex-0.4.9a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/base.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/forms.py` & `reflex-0.4.9a1/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/forms.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/inline.py` & `reflex-0.4.9a1/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/inline.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/media.py` & `reflex-0.4.9a1/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/media.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/metadata.py` & `reflex-0.4.9a1/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/metadata.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/other.py` & `reflex-0.4.9a1/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/other.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/scripts.py` & `reflex-0.4.9a1/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/scripts.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/sectioning.py` & `reflex-0.4.9a1/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/sectioning.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/tables.py` & `reflex-0.4.9a1/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/tables.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/typography.py` & `reflex-0.4.9a1/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/el/elements/typography.pyi` & `reflex-0.4.9a1/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/gridjs/datatable.py` & `reflex-0.4.9a1/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/gridjs/datatable.pyi` & `reflex-0.4.9a1/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/lucide/icon.py` & `reflex-0.4.9a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/lucide/icon.pyi` & `reflex-0.4.9a1/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/markdown/markdown.py` & `reflex-0.4.9a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/markdown/markdown.pyi` & `reflex-0.4.9a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/moment/moment.py` & `reflex-0.4.9a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/moment/moment.pyi` & `reflex-0.4.9a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/base.pyi` & `reflex-0.4.9a1/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/image.py` & `reflex-0.4.9a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/image.pyi` & `reflex-0.4.9a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/link.pyi` & `reflex-0.4.9a1/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/video.py` & `reflex-0.4.9a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/next/video.pyi` & `reflex-0.4.9a1/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/plotly/plotly.py` & `reflex-0.4.9a1/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/plotly/plotly.pyi` & `reflex-0.4.9a1/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/base.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/base.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/form.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/form.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/progress.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/progress.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/slider.py` & `reflex-0.4.9a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/primitives/slider.pyi` & `reflex-0.4.9a1/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/base.py` & `reflex-0.4.9a1/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/base.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.py` & `reflex-0.4.9a1/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/__init__.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/alertdialog.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/select.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,52 @@
-"""Stub file for reflex/components/radix/themes/components/alertdialog.py"""
+"""Stub file for reflex/components/radix/themes/components/select.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, Literal
-from reflex import el
+from typing import Any, Dict, List, Literal, Union
+import reflex as rx
+from reflex.components.component import Component, ComponentNamespace
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import RadixThemesComponent
+from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
 
-LiteralContentSize = Literal["1", "2", "3", "4"]
-
-class AlertDialogRoot(RadixThemesComponent):
+class SelectRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
         ] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
         open: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -139,46 +85,55 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogRoot":
+    ) -> "SelectRoot":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            open: The controlled open state of the dialog.
+            size: The size of the select: "1" | "2" | "3"
+            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
+            value: The controlled value of the select. Should be used in conjunction with on_change.
+            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
+            name: The name of the select control when submitting the form.
+            disabled: When True, prevents the user from interacting with select.
+            required: When True, indicates that the user must select a value before the owning form can be submitted.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class AlertDialogTrigger(RadixThemesComponent):
+class SelectTrigger(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft", "ghost"]],
+                Literal["classic", "surface", "soft", "ghost"],
+            ]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -233,20 +188,26 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -286,46 +247,49 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogTrigger":
+    ) -> "SelectTrigger":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            variant: Variant of the select trigger
+            color_scheme: The color of the select trigger
+            radius: The radius of the select trigger
+            placeholder: The placeholder of the select trigger
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class AlertDialogContent(el.Div, RadixThemesComponent):
+class SelectContent(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        variant: Optional[
+            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -380,83 +344,149 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        position: Optional[
+            Union[
+                Var[Literal["item-aligned", "popper"]],
+                Literal["item-aligned", "popper"],
+            ]
         ] = None,
-        force_mount: Optional[Union[Var[bool], bool]] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        side: Optional[
+            Union[
+                Var[Literal["top", "right", "bottom", "left"]],
+                Literal["top", "right", "bottom", "left"],
+            ]
         ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        side_offset: Optional[Union[Var[int], int]] = None,
+        align: Optional[
+            Union[
+                Var[Literal["start", "center", "end"]],
+                Literal["start", "center", "end"],
+            ]
         ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        align_offset: Optional[Union[Var[int], int]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_close_auto_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_escape_key_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_pointer_down_outside: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "SelectContent":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
+
+        Args:
+            *children: Child components.
+            variant: The variant of the select content
+            color_scheme: The color of the select content
+            high_contrast: Whether to render the select content with higher contrast color against background
+            position: The positioning mode to use, item-aligned is the default and behaves similarly to a native MacOS menu by positioning content relative to the active item. popper positions content in the same way as our other primitives, for example Popover or DropdownMenu.
+            side: The preferred side of the anchor to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled. Only available when position is set to popper.
+            side_offset: The distance in pixels from the anchor. Only available when position is set to popper.
+            align: The preferred alignment against the anchor. May change when collisions occur. Only available when position is set to popper.
+            align_offset: The vertical distance in pixels from the anchor. Only available when position is set to popper.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: Component properties.
+
+        Returns:
+            A new component instance.
+        """
+        ...
+
+class SelectGroup(RadixThemesComponent):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_close_auto_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
@@ -476,141 +506,136 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_auto_focus: Optional[
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "SelectGroup":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
+
+        Args:
+            *children: Child components.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: Component properties.
+
+        Returns:
+            A new component instance.
+        """
+        ...
+
+class SelectItem(RadixThemesComponent):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        value: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogContent":
+    ) -> "SelectItem":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            size: The size of the content.
-            force_mount: Whether to force mount the content on open.
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            value: The value given as data when submitting a form with a name.
+            disabled: Whether the select item is disabled
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class AlertDialogTitle(RadixThemesComponent):
+class SelectLabel(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -650,113 +675,46 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogTitle":
+    ) -> "SelectLabel":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class AlertDialogDescription(RadixThemesComponent):
+class SelectSeparator(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -796,45 +754,44 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogDescription":
+    ) -> "SelectSeparator":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class AlertDialogAction(RadixThemesComponent):
+class HighLevelSelect(SelectRoot):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        items: Optional[Union[Var[List[str]], List[str]]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[str], str]] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -889,24 +846,56 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft", "ghost"]],
+                Literal["classic", "surface", "soft", "ghost"],
+            ]
+        ] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
+        width: Optional[Union[Var[str], str]] = None,
+        position: Optional[
+            Union[
+                Var[Literal["item-aligned", "popper"]],
+                Literal["item-aligned", "popper"],
+            ]
+        ] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -935,52 +924,74 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_open_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogAction":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "HighLevelSelect":
+        """Create a select component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            items: The items of the select.
+            items: The items of the select.
+            placeholder: The placeholder of the select.
+            label: The label of the select.
+            color_scheme: The color of the select.
+            high_contrast: Whether to render the select with higher contrast color against background.
+            variant: The variant of the select.
+            radius: The radius of the select.
+            width: The width of the select.
+            position: The positioning mode to use. Default is "item-aligned".
+            size: The size of the select: "1" | "2" | "3"
+            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
+            value: The controlled value of the select. Should be used in conjunction with on_change.
+            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
+            name: The name of the select control when submitting the form.
+            disabled: When True, prevents the user from interacting with select.
+            required: When True, indicates that the user must select a value before the owning form can be submitted.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: Additional properties to apply to the select component.
 
         Returns:
-            A new component instance.
+            The select component.
         """
         ...
 
-class AlertDialogCancel(RadixThemesComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
+class Select(ComponentNamespace):
+    root = staticmethod(SelectRoot.create)
+    trigger = staticmethod(SelectTrigger.create)
+    content = staticmethod(SelectContent.create)
+    group = staticmethod(SelectGroup.create)
+    item = staticmethod(SelectItem.create)
+    separator = staticmethod(SelectSeparator.create)
+    label = staticmethod(SelectLabel.create)
+
+    @staticmethod
+    def __call__(
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        items: Optional[Union[Var[List[str]], List[str]]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[str], str]] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -1035,24 +1046,56 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft", "ghost"]],
+                Literal["classic", "surface", "soft", "ghost"],
+            ]
+        ] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
+        width: Optional[Union[Var[str], str]] = None,
+        position: Optional[
+            Union[
+                Var[Literal["item-aligned", "popper"]],
+                Literal["item-aligned", "popper"],
+            ]
+        ] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -1081,48 +1124,53 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_open_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AlertDialogCancel":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "HighLevelSelect":
+        """Create a select component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            items: The items of the select.
+            items: The items of the select.
+            placeholder: The placeholder of the select.
+            label: The label of the select.
+            color_scheme: The color of the select.
+            high_contrast: Whether to render the select with higher contrast color against background.
+            variant: The variant of the select.
+            radius: The radius of the select.
+            width: The width of the select.
+            position: The positioning mode to use. Default is "item-aligned".
+            size: The size of the select: "1" | "2" | "3"
+            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
+            value: The controlled value of the select. Should be used in conjunction with on_change.
+            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
+            name: The name of the select control when submitting the form.
+            disabled: When True, prevents the user from interacting with select.
+            required: When True, indicates that the user must select a value before the owning form can be submitted.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: Additional properties to apply to the select component.
 
         Returns:
-            A new component instance.
+            The select component.
         """
         ...
 
-class AlertDialog(SimpleNamespace):
-    root = staticmethod(AlertDialogRoot.create)
-    trigger = staticmethod(AlertDialogTrigger.create)
-    content = staticmethod(AlertDialogContent.create)
-    title = staticmethod(AlertDialogTitle.create)
-    description = staticmethod(AlertDialogDescription.create)
-    action = staticmethod(AlertDialogAction.create)
-    cancel = staticmethod(AlertDialogCancel.create)
-
-alert_dialog = AlertDialog()
+select = Select()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/aspectratio.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-"""Stub file for reflex/components/radix/themes/components/aspectratio.py"""
+"""Stub file for reflex/components/radix/themes/components/separator.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Union
+from typing import Literal
 from reflex.vars import Var
-from ..base import RadixThemesComponent
+from ..base import LiteralAccentColor, RadixThemesComponent
 
-class AspectRatio(RadixThemesComponent):
+LiteralSeperatorSize = Literal["1", "2", "3", "4"]
+
+class Separator(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -76,21 +80,26 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        ratio: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        decorative: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -130,33 +139,33 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "AspectRatio":
+    ) -> "Separator":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            ratio: The ratio of the width to the height of the element
+            size: The size of the select: "1" | "2" | "3" | "4"
+            color_scheme: The color of the select
+            orientation: The orientation of the separator.
+            decorative: When true, signifies that it is purely visual, carries no semantic meaning, and ensures it is not present in the accessibility tree.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-aspect_ratio = AspectRatio.create
+divider = separator = Separator.create
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/button.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/button.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/card.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/card.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/contextmenu.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,45 @@
-"""Stub file for reflex/components/radix/themes/components/contextmenu.py"""
+"""Stub file for reflex/components/radix/themes/components/dropdown_menu.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, List, Literal
+from typing import Any, Dict, List, Literal, Union
+from reflex.components.component import ComponentNamespace
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from ..base import LiteralAccentColor, RadixThemesComponent, RadixThemesTriggerComponent
 
-class ContextMenuRoot(RadixThemesComponent):
+LiteralDirType = Literal["ltr", "rtl"]
+LiteralSizeType = Literal["1", "2"]
+LiteralVariantType = Literal["solid", "soft"]
+LiteralSideType = Literal["top", "right", "bottom", "left"]
+LiteralAlignType = Literal["start", "center", "end"]
+LiteralStickyType = Literal["partial", "always"]
+
+class DropdownMenuRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
         modal: Optional[Union[Var[bool], bool]] = None,
+        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -136,115 +82,51 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuRoot":
+    ) -> "DropdownMenuRoot":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            modal: The modality of the context menu. When set to true, interaction with outside elements will be disabled and only menu content will be visible to screen readers.
+            default_open: The open state of the dropdown menu when it is initially rendered. Use when you do not need to control its open state.
+            open: The controlled open state of the dropdown menu. Must be used in conjunction with onOpenChange.
+            modal: The modality of the dropdown menu. When set to true, interaction with outside elements will be disabled and only menu content will be visible to screen readers. Defaults to True.
+            dir: The reading direction of submenus when applicable. If omitted, inherits globally from DirectionProvider or assumes LTR (left-to-right) reading mode.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenuTrigger(RadixThemesComponent):
+class DropdownMenuTrigger(RadixThemesTriggerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -284,47 +166,37 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuTrigger":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "DropdownMenuTrigger":
+        """Create a new RadixThemesTriggerComponent instance.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            disabled: Whether the trigger is disabled
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
-            custom_attrs: custom attribute
-            **props: Component properties.
+            children: The children of the component.
+            props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class ContextMenuContent(RadixThemesComponent):
+class DropdownMenuContent(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
+        variant: Optional[
+            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -379,27 +251,51 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
-        variant: Optional[
-            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
-        ] = None,
         high_contrast: Optional[Union[Var[bool], bool]] = None,
-        align_offset: Optional[Union[Var[int], int]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        loop: Optional[Union[Var[bool], bool]] = None,
+        force_mount: Optional[Union[Var[bool], bool]] = None,
+        side: Optional[
+            Union[
+                Var[Literal["top", "right", "bottom", "left"]],
+                Literal["top", "right", "bottom", "left"],
+            ]
+        ] = None,
+        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
+        align: Optional[
+            Union[
+                Var[Literal["start", "center", "end"]],
+                Literal["start", "center", "end"],
+            ]
+        ] = None,
+        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
         avoid_collisions: Optional[Union[Var[bool], bool]] = None,
+        collision_padding: Optional[
+            Union[
+                Var[Union[float, int, Dict[str, Union[float, int]]]],
+                Union[float, int, Dict[str, Union[float, int]]],
+            ]
+        ] = None,
+        arrow_padding: Optional[
+            Union[Var[Union[float, int]], Union[float, int]]
+        ] = None,
+        sticky: Optional[
+            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        ] = None,
+        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -454,118 +350,65 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuContent":
+    ) -> "DropdownMenuContent":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            size: Button size "1" - "4"
-            variant: Variant of button: "solid" | "soft" | "outline" | "ghost"
-            high_contrast: Whether to render the button with higher contrast color against background
-            align_offset: The vertical distance in pixels from the anchor.
-            avoid_collisions: When true, overrides the side and aligns preferences to prevent collisions with boundary edges.
+            size: Dropdown Menu Content size "1" - "2"
+            variant: Variant of Dropdown Menu Content: "solid" | "soft"
+            color_scheme: Override theme color for Dropdown Menu Content
+            high_contrast: Renders the Dropdown Menu Content in higher contrast
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
+            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
+            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
+            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and `avoid_collisions` is enabled.The position of the tooltip. Defaults to "top".
+            side_offset: The distance in pixels from the trigger. Defaults to 0.
+            align: The preferred alignment against the trigger. May change when collisions occur. Defaults to "center".
+            align_offset: An offset in pixels from the "start" or "end" alignment options.
+            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
+            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
+            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
+            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
+            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenuSub(RadixThemesComponent):
+class DropdownMenuSubTrigger(RadixThemesTriggerComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        text_value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -605,114 +448,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuSub":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "DropdownMenuSubTrigger":
+        """Create a new RadixThemesTriggerComponent instance.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
-            custom_attrs: custom attribute
-            **props: Component properties.
+            children: The children of the component.
+            props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class ContextMenuSubTrigger(RadixThemesComponent):
+class DropdownMenuSub(RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
+        open: Optional[Union[Var[bool], bool]] = None,
+        default_open: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -745,123 +514,78 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_open_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuSubTrigger":
+    ) -> "DropdownMenuSub":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            disabled: Whether the trigger is disabled
+            open: The controlled open state of the submenu. Must be used in conjunction with `on_open_change`.
+            default_open: The open state of the submenu when it is initially rendered. Use when you do not need to control its open state.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenuSubContent(RadixThemesComponent):
+class DropdownMenuSubContent(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        loop: Optional[Union[Var[bool], bool]] = None,
+        force_mount: Optional[Union[Var[bool], bool]] = None,
+        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
+        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
+        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
+        collision_padding: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Union[float, int, Dict[str, Union[float, int]]]],
+                Union[float, int, Dict[str, Union[float, int]]],
             ]
         ] = None,
-        loop: Optional[Union[Var[bool], bool]] = None,
+        arrow_padding: Optional[
+            Union[Var[Union[float, int]], Union[float, int]]
+        ] = None,
+        sticky: Optional[
+            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        ] = None,
+        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -913,46 +637,52 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuSubContent":
+    ) -> "DropdownMenuSubContent":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            loop: When true, keyboard navigation will loop from last item to first, and vice versa.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
+            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
+            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
+            side_offset: The distance in pixels from the trigger. Defaults to 0.
+            align_offset: An offset in pixels from the "start" or "end" alignment options.
+            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
+            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
+            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
+            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
+            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenuItem(RadixThemesComponent):
+class DropdownMenuItem(RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -1008,20 +738,22 @@
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
         shortcut: Optional[Union[Var[str], str]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        text_value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -1057,118 +789,58 @@
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_select: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuItem":
+    ) -> "DropdownMenuItem":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            color_scheme: Override theme color for Dropdown Menu Item
             shortcut: Shortcut to render a menu item as a link
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
+            disabled: When true, prevents the user from interacting with the item.
+            text_value: Optional text used for typeahead purposes. By default the typeahead behavior will use the .textContent of the item. Use this when the content is complex, or you have non-textual content inside.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenuSeparator(RadixThemesComponent):
+class DropdownMenuSeparator(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -1208,42 +880,39 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ContextMenuSeparator":
+    ) -> "DropdownMenuSeparator":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class ContextMenu(SimpleNamespace):
-    root = staticmethod(ContextMenuRoot.create)
-    trigger = staticmethod(ContextMenuTrigger.create)
-    content = staticmethod(ContextMenuContent.create)
-    sub = staticmethod(ContextMenuSub.create)
-    sub_trigger = staticmethod(ContextMenuSubTrigger.create)
-    sub_content = staticmethod(ContextMenuSubContent.create)
-    item = staticmethod(ContextMenuItem.create)
-    separator = staticmethod(ContextMenuSeparator.create)
+class DropdownMenu(ComponentNamespace):
+    root = staticmethod(DropdownMenuRoot.create)
+    trigger = staticmethod(DropdownMenuTrigger.create)
+    content = staticmethod(DropdownMenuContent.create)
+    sub_trigger = staticmethod(DropdownMenuSubTrigger.create)
+    sub = staticmethod(DropdownMenuSub.create)
+    sub_content = staticmethod(DropdownMenuSubContent.create)
+    item = staticmethod(DropdownMenuItem.create)
+    separator = staticmethod(DropdownMenuSeparator.create)
 
-context_menu = ContextMenu()
+menu = dropdown_menu = DropdownMenu()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,150 @@
-"""Stub file for reflex/components/radix/themes/components/dropdown_menu.py"""
+"""Stub file for reflex/components/radix/themes/components/text_field.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Literal, Union
-from reflex.components.component import ComponentNamespace
+from typing import Any, Dict, Literal
+from reflex.components import el
+from reflex.components.component import Component, ComponentNamespace
+from reflex.components.core.debounce import DebounceInput
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent, RadixThemesTriggerComponent
+from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
 
-LiteralDirType = Literal["ltr", "rtl"]
-LiteralSizeType = Literal["1", "2"]
-LiteralVariantType = Literal["solid", "soft"]
-LiteralSideType = Literal["top", "right", "bottom", "left"]
-LiteralAlignType = Literal["start", "center", "end"]
-LiteralStickyType = Literal["partial", "always"]
+LiteralTextFieldSize = Literal["1", "2", "3"]
+LiteralTextFieldVariant = Literal["classic", "surface", "soft"]
 
-class DropdownMenuRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class TextFieldRoot(el.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        modal: Optional[Union[Var[bool], bool]] = None,
-        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
+            ]
+        ] = None,
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
+            ]
+        ] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -72,130 +182,148 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuRoot":
+    ) -> "TextFieldRoot":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            default_open: The open state of the dropdown menu when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the dropdown menu. Must be used in conjunction with onOpenChange.
-            modal: The modality of the dropdown menu. When set to true, interaction with outside elements will be disabled and only menu content will be visible to screen readers. Defaults to True.
-            dir: The reading direction of submenus when applicable. If omitted, inherits globally from DirectionProvider or assumes LTR (left-to-right) reading mode.
+            size: Text field size "1" - "3"
+            variant: Variant of text field: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for text field
+            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class DropdownMenuTrigger(RadixThemesTriggerComponent):
+class TextFieldInput(el.Input, TextFieldRoot):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        accept: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        alt: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        auto_complete: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        auto_focus: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        capture: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        checked: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        default_checked: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        dirname: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        disabled: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        form_action: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_enc_type: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_method: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_no_validate: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        form_target: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        list: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        max: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        max_length: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        min_length: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        min: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        multiple: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        name: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        pattern: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        placeholder: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        read_only: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        required: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        size: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        src: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        step: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        type: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        use_map: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        value: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "DropdownMenuTrigger":
-        """Create a new RadixThemesTriggerComponent instance.
-
-        Args:
-            children: The children of the component.
-            props: The properties of the component.
-
-        Returns:
-            The new RadixThemesTriggerComponent instance.
-        """
-        ...
-
-class DropdownMenuContent(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
         variant: Optional[
-            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
+            Union[
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
+            ]
         ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
@@ -251,77 +379,88 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        loop: Optional[Union[Var[bool], bool]] = None,
-        force_mount: Optional[Union[Var[bool], bool]] = None,
-        side: Optional[
+        radius: Optional[
             Union[
-                Var[Literal["top", "right", "bottom", "left"]],
-                Literal["top", "right", "bottom", "left"],
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
             ]
         ] = None,
-        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        align: Optional[
-            Union[
-                Var[Literal["start", "center", "end"]],
-                Literal["start", "center", "end"],
-            ]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
-        collision_padding: Optional[
-            Union[
-                Var[Union[float, int, Dict[str, Union[float, int]]]],
-                Union[float, int, Dict[str, Union[float, int]]],
-            ]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        arrow_padding: Optional[
-            Union[Var[Union[float, int]], Union[float, int]]
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        sticky: Optional[
-            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_click: Optional[
+        on_change: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_close_auto_focus: Optional[
+        on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus_outside: Optional[
+        on_key_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_interact_outside: Optional[
+        on_key_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -340,143 +479,160 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "TextFieldInput":
+        """Create an Input component.
 
         Args:
-            *children: Child components.
-            size: Dropdown Menu Content size "1" - "2"
-            variant: Variant of Dropdown Menu Content: "solid" | "soft"
-            color_scheme: Override theme color for Dropdown Menu Content
-            high_contrast: Renders the Dropdown Menu Content in higher contrast
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
-            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
-            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and `avoid_collisions` is enabled.The position of the tooltip. Defaults to "top".
-            side_offset: The distance in pixels from the trigger. Defaults to 0.
-            align: The preferred alignment against the trigger. May change when collisions occur. Defaults to "center".
-            align_offset: An offset in pixels from the "start" or "end" alignment options.
-            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
-            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
-            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
-            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
-            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
+            *children: The children of the component.
+            accept: Accepted types of files when the input is file type
+            alt: Alternate text for input type="image"
+            auto_complete: Whether the input should have autocomplete enabled
+            auto_focus: Automatically focuses the input when the page loads
+            capture: Captures media from the user (camera or microphone)
+            checked: Indicates whether the input is checked (for checkboxes and radio buttons)
+            default_checked: The initial value (for checkboxes and radio buttons)
+            default_value: The initial value for a text field
+            dirname: Name part of the input to submit in 'dir' and 'name' pair when form is submitted
+            disabled: Disables the input
+            form: Associates the input with a form (by id)
+            form_action: URL to send the form data to (for type="submit" buttons)
+            form_enc_type: How the form data should be encoded when submitting to the server (for type="submit" buttons)
+            form_method: HTTP method to use for sending form data (for type="submit" buttons)
+            form_no_validate: Bypasses form validation when submitting (for type="submit" buttons)
+            form_target: Specifies where to display the response after submitting the form (for type="submit" buttons)
+            list: References a datalist for suggested options
+            max: Specifies the maximum value for the input
+            max_length: Specifies the maximum number of characters allowed in the input
+            min_length: Specifies the minimum number of characters required in the input
+            min: Specifies the minimum value for the input
+            multiple: Indicates whether multiple values can be entered in an input of the type email or file
+            name: Name of the input, used when sending form data
+            pattern: Regex pattern the input's value must match to be valid
+            placeholder: Placeholder text in the input
+            read_only: Indicates whether the input is read-only
+            required: Indicates that the input is required
+            size: Text field size "1" - "3"
+            src: URL for image inputs
+            step: Specifies the legal number intervals for an input
+            type: Specifies the type of input
+            use_map: Name of the image map used with the input
+            value: Value of the input
+            variant: Variant of text field: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for text field
+            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
+    def get_event_triggers(self) -> Dict[str, Any]: ...
 
-class DropdownMenuSubTrigger(RadixThemesTriggerComponent):
+class TextFieldSlot(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        text_value: Optional[Union[Var[str], str]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
+            ]
         ] = None,
-        **props
-    ) -> "DropdownMenuSubTrigger":
-        """Create a new RadixThemesTriggerComponent instance.
-
-        Args:
-            children: The children of the component.
-            props: The properties of the component.
-
-        Returns:
-            The new RadixThemesTriggerComponent instance.
-        """
-        ...
-
-class DropdownMenuSub(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        open: Optional[Union[Var[bool], bool]] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -514,101 +670,165 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSub":
+    ) -> "TextFieldSlot":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            open: The controlled open state of the submenu. Must be used in conjunction with `on_open_change`.
-            default_open: The open state of the submenu when it is initially rendered. Use when you do not need to control its open state.
+            color_scheme: Override theme color for text field slot
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class DropdownMenuSubContent(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Input(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        loop: Optional[Union[Var[bool], bool]] = None,
-        force_mount: Optional[Union[Var[bool], bool]] = None,
-        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
-        collision_padding: Optional[
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        variant: Optional[
             Union[
-                Var[Union[float, int, Dict[str, Union[float, int]]]],
-                Union[float, int, Dict[str, Union[float, int]]],
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
             ]
         ] = None,
-        arrow_padding: Optional[
-            Union[Var[Union[float, int]], Union[float, int]]
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
+            ]
         ] = None,
-        sticky: Optional[
-            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
         ] = None,
-        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
+        auto_complete: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        max_length: Optional[Union[Var[str], str]] = None,
+        min_length: Optional[Union[Var[str], str]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        read_only: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
+        type: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus_outside: Optional[
+        on_key_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_interact_outside: Optional[
+        on_key_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -627,62 +847,71 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSubContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Input":
+        """Create an Input component.
 
         Args:
-            *children: Child components.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
-            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
-            side_offset: The distance in pixels from the trigger. Defaults to 0.
-            align_offset: An offset in pixels from the "start" or "end" alignment options.
-            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
-            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
-            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
-            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
-            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
+            size: Text field size "1" - "3"
+            variant: Variant of text field: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for text field
+            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            auto_complete: Whether the input should have autocomplete enabled
+            default_value: The value of the input when initially rendered.
+            disabled: Disables the input
+            max_length: Specifies the maximum number of characters allowed in the input
+            min_length: Specifies the minimum number of characters required in the input
+            name: Name of the input, used when sending form data
+            placeholder: Placeholder text in the input
+            read_only: Indicates whether the input is read-only
+            required: Indicates that the input is required
+            type: Specifies the type of input
+            value: Value of the input
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-class DropdownMenuItem(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
+
+class TextField(ComponentNamespace):
+    root = staticmethod(TextFieldRoot.create)
+    input = staticmethod(TextFieldInput.create)
+    slot = staticmethod(TextFieldSlot.create)
+
+    @staticmethod
+    def __call__(
         *children,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
+            ]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -737,124 +966,59 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        shortcut: Optional[Union[Var[str], str]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
+        auto_complete: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
         disabled: Optional[Union[Var[bool], bool]] = None,
-        text_value: Optional[Union[Var[str], str]] = None,
+        max_length: Optional[Union[Var[str], str]] = None,
+        min_length: Optional[Union[Var[str], str]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        read_only: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
+        type: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
+        on_key_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_select: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        **props
-    ) -> "DropdownMenuItem":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
-
-        Args:
-            *children: Child components.
-            color_scheme: Override theme color for Dropdown Menu Item
-            shortcut: Shortcut to render a menu item as a link
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            disabled: When true, prevents the user from interacting with the item.
-            text_value: Optional text used for typeahead purposes. By default the typeahead behavior will use the .textContent of the item. Use this when the content is complex, or you have non-textual content inside.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Component properties.
-
-        Returns:
-            A new component instance.
-        """
-        ...
-
-class DropdownMenuSeparator(RadixThemesComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
+        on_key_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -880,39 +1044,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSeparator":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Input":
+        """Create an Input component.
 
         Args:
-            *children: Child components.
+            size: Text field size "1" - "3"
+            variant: Variant of text field: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for text field
+            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            auto_complete: Whether the input should have autocomplete enabled
+            default_value: The value of the input when initially rendered.
+            disabled: Disables the input
+            max_length: Specifies the maximum number of characters allowed in the input
+            min_length: Specifies the minimum number of characters required in the input
+            name: Name of the input, used when sending form data
+            placeholder: Placeholder text in the input
+            read_only: Indicates whether the input is read-only
+            required: Indicates that the input is required
+            type: Specifies the type of input
+            value: Value of the input
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenu(ComponentNamespace):
-    root = staticmethod(DropdownMenuRoot.create)
-    trigger = staticmethod(DropdownMenuTrigger.create)
-    content = staticmethod(DropdownMenuContent.create)
-    sub_trigger = staticmethod(DropdownMenuSubTrigger.create)
-    sub = staticmethod(DropdownMenuSub.create)
-    sub_content = staticmethod(DropdownMenuSubContent.create)
-    item = staticmethod(DropdownMenuItem.create)
-    separator = staticmethod(DropdownMenuSeparator.create)
-
-menu = dropdown_menu = DropdownMenu()
+text_field = TextField()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/dropdownmenu.pyi` & `reflex-0.4.9a1/reflex/components/recharts/cartesian.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,226 @@
-"""Stub file for reflex/components/radix/themes/components/dropdownmenu.py"""
+"""Stub file for reflex/components/recharts/cartesian.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, List, Literal, Union
+from typing import Any, Dict, List, Union
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from .recharts import (
+    LiteralAnimationEasing,
+    LiteralAreaType,
+    LiteralDirection,
+    LiteralIfOverflow,
+    LiteralInterval,
+    LiteralLayout,
+    LiteralLineType,
+    LiteralOrientationTopBottom,
+    LiteralOrientationTopBottomLeftRight,
+    LiteralPolarRadiusType,
+    LiteralScale,
+    LiteralShape,
+    Recharts,
+)
 
-LiteralDirType = Literal["ltr", "rtl"]
-LiteralSizeType = Literal["1", "2"]
-LiteralVariantType = Literal["solid", "soft"]
-LiteralSideType = Literal["top", "right", "bottom", "left"]
-LiteralAlignType = Literal["start", "center", "end"]
-LiteralStickyType = Literal["partial", "always"]
-
-class DropdownMenuRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Axis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        hide: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[
+            Union[Var[Literal["top", "bottom"]], Literal["top", "bottom"]]
+        ] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_decimals: Optional[Union[Var[bool], bool]] = None,
+        allow_data_overflow: Optional[Union[Var[bool], bool]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        axis_line: Optional[Union[Var[bool], bool]] = None,
+        tick_line: Optional[Union[Var[bool], bool]] = None,
+        mirror: Optional[Union[Var[bool], bool]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        scale: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
                 ],
             ]
         ] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        modal: Optional[Union[Var[bool], bool]] = None,
-        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
+        unit: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        name: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
+        on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_click: Optional[
+        on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
+        on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_double_click: Optional[
+        on_mouse_move: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus: Optional[
+        on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mount: Optional[
+        on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_down: Optional[
+        **props
+    ) -> "Axis":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique in an area chart.
+            hide: If set true, the axis do not display in the chart.
+            orientation: The orientation of axis 'top' | 'bottom'
+            type_: The type of axis 'number' | 'category'
+            allow_decimals: Allow the ticks of XAxis to be decimals or not.
+            allow_data_overflow: When domain of the axis is specified and the type of the axis is 'number', if allowDataOverflow is set to be false, the domain will be adjusted when the minimum value of data is smaller than domain[0] or the maximum value of data is greater than domain[1] so that the axis displays all data values. If set to true, graphic elements (line, area, bars) will be clipped to conform to the specified domain.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            axis_line: If set false, no axis line will be drawn. If set a object, the option is the configuration of axis line.
+            tick_line: If set false, no axis tick lines will be drawn. If set a object, the option is the configuration of tick lines.
+            mirror: If set true, flips ticks around the axis line, displaying the labels inside the chart instead of outside.
+            reversed: Reverse the ticks or not.
+            scale: If 'auto' set, the scale function is decided by the type of chart, and the props type. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold' | Function
+            unit: The unit of data displayed in the axis. This option will be used to represent an index unit in a scatter chart.
+            name: The name of data displayed in the axis. This option will be used to represent an index in a scatter chart.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class XAxis(Axis):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        hide: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[
+            Union[Var[Literal["top", "bottom"]], Literal["top", "bottom"]]
+        ] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_decimals: Optional[Union[Var[bool], bool]] = None,
+        allow_data_overflow: Optional[Union[Var[bool], bool]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        axis_line: Optional[Union[Var[bool], bool]] = None,
+        tick_line: Optional[Union[Var[bool], bool]] = None,
+        mirror: Optional[Union[Var[bool], bool]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        scale: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
+                    ]
+                ],
+                Literal[
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
+                ],
+            ]
+        ] = None,
+        unit: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        name: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -133,131 +230,222 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
+        **props
+    ) -> "XAxis":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique in an area chart.
+            hide: If set true, the axis do not display in the chart.
+            orientation: The orientation of axis 'top' | 'bottom'
+            type_: The type of axis 'number' | 'category'
+            allow_decimals: Allow the ticks of XAxis to be decimals or not.
+            allow_data_overflow: When domain of the axis is specified and the type of the axis is 'number', if allowDataOverflow is set to be false, the domain will be adjusted when the minimum value of data is smaller than domain[0] or the maximum value of data is greater than domain[1] so that the axis displays all data values. If set to true, graphic elements (line, area, bars) will be clipped to conform to the specified domain.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            axis_line: If set false, no axis line will be drawn. If set a object, the option is the configuration of axis line.
+            tick_line: If set false, no axis tick lines will be drawn. If set a object, the option is the configuration of tick lines.
+            mirror: If set true, flips ticks around the axis line, displaying the labels inside the chart instead of outside.
+            reversed: Reverse the ticks or not.
+            scale: If 'auto' set, the scale function is decided by the type of chart, and the props type. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold' | Function
+            unit: The unit of data displayed in the axis. This option will be used to represent an index unit in a scatter chart.
+            name: The name of data displayed in the axis. This option will be used to represent an index in a scatter chart.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class YAxis(Axis):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        hide: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[
+            Union[Var[Literal["top", "bottom"]], Literal["top", "bottom"]]
+        ] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_decimals: Optional[Union[Var[bool], bool]] = None,
+        allow_data_overflow: Optional[Union[Var[bool], bool]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        axis_line: Optional[Union[Var[bool], bool]] = None,
+        tick_line: Optional[Union[Var[bool], bool]] = None,
+        mirror: Optional[Union[Var[bool], bool]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        scale: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
+                    ]
+                ],
+                Literal[
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
+                ],
+            ]
+        ] = None,
+        unit: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        name: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
+        on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_scroll: Optional[
+        on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_unmount: Optional[
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "YAxis":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            default_open: The open state of the dropdown menu when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the dropdown menu. Must be used in conjunction with onOpenChange.
-            modal: The modality of the dropdown menu. When set to true, interaction with outside elements will be disabled and only menu content will be visible to screen readers. Defaults to True.
-            dir: The reading direction of submenus when applicable. If omitted, inherits globally from DirectionProvider or assumes LTR (left-to-right) reading mode.
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique in an area chart.
+            hide: If set true, the axis do not display in the chart.
+            orientation: The orientation of axis 'top' | 'bottom'
+            type_: The type of axis 'number' | 'category'
+            allow_decimals: Allow the ticks of XAxis to be decimals or not.
+            allow_data_overflow: When domain of the axis is specified and the type of the axis is 'number', if allowDataOverflow is set to be false, the domain will be adjusted when the minimum value of data is smaller than domain[0] or the maximum value of data is greater than domain[1] so that the axis displays all data values. If set to true, graphic elements (line, area, bars) will be clipped to conform to the specified domain.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            axis_line: If set false, no axis line will be drawn. If set a object, the option is the configuration of axis line.
+            tick_line: If set false, no axis tick lines will be drawn. If set a object, the option is the configuration of tick lines.
+            mirror: If set true, flips ticks around the axis line, displaying the labels inside the chart instead of outside.
+            reversed: Reverse the ticks or not.
+            scale: If 'auto' set, the scale function is decided by the type of chart, and the props type. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold' | Function
+            unit: The unit of data displayed in the axis. This option will be used to represent an index unit in a scatter chart.
+            name: The name of data displayed in the axis. This option will be used to represent an index in a scatter chart.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuTrigger(RadixThemesComponent):
+class ZAxis(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        range: Optional[Union[Var[List[int]], List[int]]] = None,
+        unit: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        name: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        scale: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
                 ],
             ]
         ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -297,177 +485,671 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuTrigger":
-        """Create a new component instance.
+    ) -> "ZAxis":
+        """Create the component.
 
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+        Args:
+            *children: The children of the component.
+            data_key: The key of data displayed in the axis.
+            range: The range of axis.
+            unit: The unit of data displayed in the axis. This option will be used to represent an index unit in a scatter chart.
+            name: The name of data displayed in the axis. This option will be used to represent an index in a scatter chart.
+            scale: If 'auto' set, the scale function is decided by the type of chart, and the props type.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Brush(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        stroke: Optional[Union[Var[str], str]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x: Optional[Union[Var[int], int]] = None,
+        y: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
+        data: Optional[Union[Var[List[Any]], List[Any]]] = None,
+        traveller_width: Optional[Union[Var[int], int]] = None,
+        gap: Optional[Union[Var[int], int]] = None,
+        start_index: Optional[Union[Var[int], int]] = None,
+        end_index: Optional[Union[Var[int], int]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Brush":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
+            *children: The children of the component.
+            stroke: Stroke color
+            data_key: The key of data displayed in the axis.
+            x: The x-coordinate of brush.
+            y: The y-coordinate of brush.
+            width: The width of brush.
+            height: The height of brush.
+            data: The data domain of brush, [min, max].
+            traveller_width: The width of each traveller.
+            gap: The data with gap of refreshing chart. If the option is not set, the chart will be refreshed every time
+            start_index: The default start index of brush. If the option is not set, the start index will be 0.
+            end_index: The default end index of brush. If the option is not set, the end index will be 1.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Cartesian(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Cartesian":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuContent(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Area(Cartesian):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        stroke: Optional[Union[Var[str], str]] = None,
+        stroke_width: Optional[Union[Var[int], int]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        type_: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "basis",
+                        "basisClosed",
+                        "basisOpen",
+                        "bumpX",
+                        "bumpY",
+                        "bump",
+                        "linear",
+                        "linearClosed",
+                        "natural",
+                        "monotoneX",
+                        "monotoneY",
+                        "monotone",
+                        "step",
+                        "stepBefore",
+                        "stepAfter",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "basis",
+                    "basisClosed",
+                    "basisOpen",
+                    "bumpX",
+                    "bumpY",
+                    "bump",
+                    "linear",
+                    "linearClosed",
+                    "natural",
+                    "monotoneX",
+                    "monotoneY",
+                    "monotone",
+                    "step",
+                    "stepBefore",
+                    "stepAfter",
                 ],
             ]
         ] = None,
-        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
-        variant: Optional[
-            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
-        ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        loop: Optional[Union[Var[bool], bool]] = None,
-        force_mount: Optional[Union[Var[bool], bool]] = None,
-        side: Optional[
+        dot: Optional[Union[Var[bool], bool]] = None,
+        active_dot: Optional[Union[Var[bool], bool]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        stack_id: Optional[Union[Var[str], str]] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Area":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            stroke: The color of the line stroke.
+            stroke_width: The width of the line stroke.
+            fill: The color of the area fill.
+            type_: The interpolation type of area. And customized interpolation function can be set to type. 'basis' | 'basisClosed' | 'basisOpen' | 'bumpX' | 'bumpY' | 'bump' | 'linear' | 'linearClosed' | 'natural' | 'monotoneX' | 'monotoneY' | 'monotone' | 'step' | 'stepBefore' | 'stepAfter' |
+            dot: If false set, dots will not be drawn. If true set, dots will be drawn which have the props calculated internally.
+            active_dot: The dot is shown when user enter an area chart and this chart has tooltip. If false set, no active dot will not be drawn. If true set, active dot will be drawn which have the props calculated internally.
+            label: If false set, labels will not be drawn. If true set, labels will be drawn which have the props calculated internally.
+            stack_id: The stack id of area, when two areas have the same value axis and same stackId, then the two areas area stacked in order.
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Bar(Cartesian):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        stroke: Optional[Union[Var[str], str]] = None,
+        stroke_width: Optional[Union[Var[int], int]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        background: Optional[Union[Var[bool], bool]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        stack_id: Optional[Union[Var[str], str]] = None,
+        bar_size: Optional[Union[Var[int], int]] = None,
+        max_bar_size: Optional[Union[Var[int], int]] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Bar":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            stroke: The color of the line stroke.
+            stroke_width: The width of the line stroke.
+            fill: The width of the line stroke.
+            background: If false set, background of bars will not be drawn. If true set, background of bars will be drawn which have the props calculated internally.
+            label: If false set, labels will not be drawn. If true set, labels will be drawn which have the props calculated internally.
+            stack_id: The stack id of bar, when two areas have the same value axis and same stackId, then the two areas area stacked in order.
+            bar_size: Size of the bar
+            max_bar_size: Max size of the bar
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Line(Cartesian):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        type_: Optional[
             Union[
-                Var[Literal["top", "right", "bottom", "left"]],
-                Literal["top", "right", "bottom", "left"],
+                Var[
+                    Literal[
+                        "basis",
+                        "basisClosed",
+                        "basisOpen",
+                        "bumpX",
+                        "bumpY",
+                        "bump",
+                        "linear",
+                        "linearClosed",
+                        "natural",
+                        "monotoneX",
+                        "monotoneY",
+                        "monotone",
+                        "step",
+                        "stepBefore",
+                        "stepAfter",
+                    ]
+                ],
+                Literal[
+                    "basis",
+                    "basisClosed",
+                    "basisOpen",
+                    "bumpX",
+                    "bumpY",
+                    "bump",
+                    "linear",
+                    "linearClosed",
+                    "natural",
+                    "monotoneX",
+                    "monotoneY",
+                    "monotone",
+                    "step",
+                    "stepBefore",
+                    "stepAfter",
+                ],
             ]
         ] = None,
-        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        align: Optional[
+        stroke: Optional[Union[Var[str], str]] = None,
+        stoke_width: Optional[Union[Var[int], int]] = None,
+        dot: Optional[Union[Var[bool], bool]] = None,
+        active_dot: Optional[Union[Var[bool], bool]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        hide: Optional[Union[Var[bool], bool]] = None,
+        connect_nulls: Optional[Union[Var[bool], bool]] = None,
+        layout: Optional[
             Union[
-                Var[Literal["start", "center", "end"]],
-                Literal["start", "center", "end"],
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
             ]
         ] = None,
-        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
-        collision_padding: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Line":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            type_: The interpolation type of line. And customized interpolation function can be set to type. It's the same as type in Area.
+            stroke: The color of the line stroke.
+            stoke_width: The width of the line stroke.
+            dot: The dot is shown when mouse enter a line chart and this chart has tooltip. If false set, no active dot will not be drawn. If true set, active dot will be drawn which have the props calculated internally.
+            active_dot: The dot is shown when user enter an area chart and this chart has tooltip. If false set, no active dot will not be drawn. If true set, active dot will be drawn which have the props calculated internally.
+            label: If false set, labels will not be drawn. If true set, labels will be drawn which have the props calculated internally.
+            hide: Hides the line when true, useful when toggling visibility state via legend.
+            connect_nulls: Whether to connect a graph line across null points.
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Scatter(Cartesian):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        z_axis_id: Optional[Union[Var[str], str]] = None,
+        line: Optional[Union[Var[bool], bool]] = None,
+        shape: Optional[
             Union[
-                Var[Union[float, int, Dict[str, Union[float, int]]]],
-                Union[float, int, Dict[str, Union[float, int]]],
+                Var[
+                    Literal[
+                        "square",
+                        "circle",
+                        "cross",
+                        "diamond",
+                        "star",
+                        "triangle",
+                        "wye",
+                    ]
+                ],
+                Literal[
+                    "square", "circle", "cross", "diamond", "star", "triangle", "wye"
+                ],
             ]
         ] = None,
-        arrow_padding: Optional[
-            Union[Var[Union[float, int]], Union[float, int]]
+        line_type: Optional[
+            Union[Var[Literal["joint", "fitting"]], Literal["joint", "fitting"]]
         ] = None,
-        sticky: Optional[
-            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        fill: Optional[Union[Var[str], str]] = None,
+        name: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
         ] = None,
-        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
+        on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Scatter":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: The source data, in which each element is an object.
+            z_axis_id: The id of z-axis which is corresponding to the data.
+            line: If false set, line will not be drawn. If true set, line will be drawn which have the props calculated internally.
+            shape: If a string set, specified symbol will be used to show scatter item. 'circle' | 'cross' | 'diamond' | 'square' | 'star' | 'triangle' | 'wye'
+            line_type: If 'joint' set, line will generated by just jointing all the points. If 'fitting' set, line will be generated by fitting algorithm. 'joint' | 'fitting'
+            fill: The fill
+            name: the name
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Funnel(Cartesian):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        animation_begin: Optional[Union[Var[int], int]] = None,
+        animation_duration: Optional[Union[Var[int], int]] = None,
+        animation_easing: Optional[
+            Union[
+                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
+                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
+            ]
+        ] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_close_auto_focus: Optional[
+        on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
+        on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_double_click: Optional[
+        on_mouse_move: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
+        on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus: Optional[
+        on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus_outside: Optional[
+        **props
+    ) -> "Funnel":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: The source data, in which each element is an object.
+            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
+            animation_duration: Specifies the duration of animation, the unit of this option is ms.
+            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
+            layout: The layout of bar in the chart, usually inherited from parent. 'horizontal' | 'vertical'
+            data_key: The key of a group of data which should be unique in an area chart.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            style: The type of icon in legend. If set to 'none', no legend item will be rendered. 'line' | 'plainline' | 'square' | 'rect'| 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye' | 'none'optional  legend_type: Var[LiteralLegendType]  The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class ErrorBar(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        direction: Optional[
+            Union[Var[Literal["x", "y", "both"]], Literal["x", "y", "both"]]
+        ] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        stroke_width: Optional[Union[Var[int], int]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_interact_outside: Optional[
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -486,141 +1168,66 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "ErrorBar":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            size: Dropdown Menu Content size "1" - "2"
-            variant: Variant of Dropdown Menu Content: "solid" | "soft"
-            high_contrast: Renders the Dropdown Menu Content in higher contrast
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
-            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
-            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and `avoid_collisions` is enabled.The position of the tooltip. Defaults to "top".
-            side_offset: The distance in pixels from the trigger. Defaults to 0.
-            align: The preferred alignment against the trigger. May change when collisions occur. Defaults to "center".
-            align_offset: An offset in pixels from the "start" or "end" alignment options.
-            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
-            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
-            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
-            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
-            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
+            *children: The children of the component.
+            direction: The direction of error bar. 'x' | 'y' | 'both'
+            data_key: The key of a group of data which should be unique in an area chart.
+            width: The width of the error bar ends.
+            stroke: The stroke color of error bar.
+            stroke_width: The stroke width of error bar.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuSubTrigger(RadixThemesComponent):
+class Reference(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x: Optional[Union[Var[str], str]] = None,
+        y: Optional[Union[Var[str], str]] = None,
+        if_overflow: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["discard", "hidden", "visible", "extendDomain"]],
+                Literal["discard", "hidden", "visible", "extendDomain"],
             ]
         ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        text_value: Optional[Union[Var[str], str]] = None,
+        is_front: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -660,119 +1267,61 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSubTrigger":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Reference":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            disabled: When true, prevents the user from interacting with the item.
-            text_value: Optional text used for typeahead purposes. By default the typeahead behavior will use the .textContent of the item. Use this when the content is complex, or you have non-textual content inside.
+            *children: The children of the component.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            x: If set a string or a number, a vertical line perpendicular to the x-axis specified by xAxisId will be drawn. If the specified x-axis is a number axis, the type of x must be Number. If the specified x-axis is a category axis, the value of x must be one of the categorys, otherwise no line will be drawn.
+            y: If set a string or a number, a horizontal line perpendicular to the y-axis specified by yAxisId will be drawn. If the specified y-axis is a number axis, the type of y must be Number. If the specified y-axis is a category axis, the value of y must be one of the categorys, otherwise no line will be drawn.
+            if_overflow: Defines how to draw the reference line if it falls partly outside the canvas. If set to 'discard', the reference line will not be drawn at all. If set to 'hidden', the reference line will be clipped to the canvas. If set to 'visible', the reference line will be drawn completely. If set to 'extendDomain', the domain of the overflown axis will be extended such that the reference line fits into the canvas.
+            is_front: If set true, the line will be rendered in front of bars in BarChart, etc.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuSub(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class ReferenceLine(Reference):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        stroke_width: Optional[Union[Var[int], int]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x: Optional[Union[Var[str], str]] = None,
+        y: Optional[Union[Var[str], str]] = None,
+        if_overflow: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["discard", "hidden", "visible", "extendDomain"]],
+                Literal["discard", "hidden", "visible", "extendDomain"],
             ]
         ] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
+        is_front: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -805,168 +1354,245 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSub":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "ReferenceLine":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            open: The controlled open state of the submenu. Must be used in conjunction with `on_open_change`.
-            default_open: The open state of the submenu when it is initially rendered. Use when you do not need to control its open state.
+            *children: The children of the component.
+            stroke_width: The width of the stroke.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            x: If set a string or a number, a vertical line perpendicular to the x-axis specified by xAxisId will be drawn. If the specified x-axis is a number axis, the type of x must be Number. If the specified x-axis is a category axis, the value of x must be one of the categorys, otherwise no line will be drawn.
+            y: If set a string or a number, a horizontal line perpendicular to the y-axis specified by yAxisId will be drawn. If the specified y-axis is a number axis, the type of y must be Number. If the specified y-axis is a category axis, the value of y must be one of the categorys, otherwise no line will be drawn.
+            if_overflow: Defines how to draw the reference line if it falls partly outside the canvas. If set to 'discard', the reference line will not be drawn at all. If set to 'hidden', the reference line will be clipped to the canvas. If set to 'visible', the reference line will be drawn completely. If set to 'extendDomain', the domain of the overflown axis will be extended such that the reference line fits into the canvas.
+            is_front: If set true, the line will be rendered in front of bars in BarChart, etc.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuSubContent(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class ReferenceDot(Reference):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x: Optional[Union[Var[str], str]] = None,
+        y: Optional[Union[Var[str], str]] = None,
+        if_overflow: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["discard", "hidden", "visible", "extendDomain"]],
+                Literal["discard", "hidden", "visible", "extendDomain"],
             ]
         ] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        loop: Optional[Union[Var[bool], bool]] = None,
-        force_mount: Optional[Union[Var[bool], bool]] = None,
-        side_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        align_offset: Optional[Union[Var[Union[float, int]], Union[float, int]]] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
-        collision_padding: Optional[
-            Union[
-                Var[Union[float, int, Dict[str, Union[float, int]]]],
-                Union[float, int, Dict[str, Union[float, int]]],
-            ]
+        is_front: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        arrow_padding: Optional[
-            Union[Var[Union[float, int]], Union[float, int]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        sticky: Optional[
-            Union[Var[Literal["partial", "always"]], Literal["partial", "always"]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hide_when_detached: Optional[Union[Var[bool], bool]] = None,
+        **props
+    ) -> "ReferenceDot":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            x: If set a string or a number, a vertical line perpendicular to the x-axis specified by xAxisId will be drawn. If the specified x-axis is a number axis, the type of x must be Number. If the specified x-axis is a category axis, the value of x must be one of the categorys, otherwise no line will be drawn.
+            y: If set a string or a number, a horizontal line perpendicular to the y-axis specified by yAxisId will be drawn. If the specified y-axis is a number axis, the type of y must be Number. If the specified y-axis is a category axis, the value of y must be one of the categorys, otherwise no line will be drawn.
+            if_overflow: Defines how to draw the reference line if it falls partly outside the canvas. If set to 'discard', the reference line will not be drawn at all. If set to 'hidden', the reference line will be clipped to the canvas. If set to 'visible', the reference line will be drawn completely. If set to 'extendDomain', the domain of the overflown axis will be extended such that the reference line fits into the canvas.
+            is_front: If set true, the line will be rendered in front of bars in BarChart, etc.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class ReferenceArea(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        stroke: Optional[Union[Var[str], str]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        fill_opacity: Optional[Union[Var[float], float]] = None,
+        x_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y_axis_id: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x1: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        x2: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y1: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        y2: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        if_overflow: Optional[
+            Union[
+                Var[Literal["discard", "hidden", "visible", "extendDomain"]],
+                Literal["discard", "hidden", "visible", "extendDomain"],
+            ]
+        ] = None,
+        is_front: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
+        on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus: Optional[
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_focus_outside: Optional[
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "ReferenceArea":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            stroke: Stroke color
+            fill: Fill color
+            fill_opacity: The opacity of area.
+            x_axis_id: The id of x-axis which is corresponding to the data.
+            y_axis_id: The id of y-axis which is corresponding to the data.
+            x1: A boundary value of the area. If the specified x-axis is a number axis, the type of x must be Number. If the specified x-axis is a category axis, the value of x must be one of the categorys. If one of x1 or x2 is invalidate, the area will cover along x-axis.
+            x2: A boundary value of the area. If the specified x-axis is a number axis, the type of x must be Number. If the specified x-axis is a category axis, the value of x must be one of the categorys. If one of x1 or x2 is invalidate, the area will cover along x-axis.
+            y1: A boundary value of the area. If the specified y-axis is a number axis, the type of y must be Number. If the specified y-axis is a category axis, the value of y must be one of the categorys. If one of y1 or y2 is invalidate, the area will cover along y-axis.
+            y2: A boundary value of the area. If the specified y-axis is a number axis, the type of y must be Number. If the specified y-axis is a category axis, the value of y must be one of the categorys. If one of y1 or y2 is invalidate, the area will cover along y-axis.
+            if_overflow: Defines how to draw the reference line if it falls partly outside the canvas. If set to 'discard', the reference line will not be drawn at all. If set to 'hidden', the reference line will be clipped to the canvas. If set to 'visible', the reference line will be drawn completely. If set to 'extendDomain', the domain of the overflown axis will be extended such that the reference line fits into the canvas.
+            is_front: If set true, the line will be rendered in front of bars in BarChart, etc.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Grid(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        x: Optional[Union[Var[int], int]] = None,
+        y: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_interact_outside: Optional[
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
@@ -985,138 +1611,63 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSubContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Grid":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            loop: When True, keyboard navigation will loop from last item to first, and vice versa. Defaults to False.
-            force_mount: Used to force mounting when more control is needed. Useful when controlling animation with React animation libraries.
-            side_offset: The distance in pixels from the trigger. Defaults to 0.
-            align_offset: An offset in pixels from the "start" or "end" alignment options.
-            avoid_collisions: When true, overrides the side and align preferences to prevent collisions with boundary edges. Defaults to True.
-            collision_padding: The distance in pixels from the boundary edges where collision detection should occur. Accepts a number (same for all sides), or a partial padding object, for example: { "top": 20, "left": 20 }. Defaults to 0.
-            arrow_padding: The padding between the arrow and the edges of the content. If your content has border-radius, this will prevent it from overflowing the corners. Defaults to 0.
-            sticky: The sticky behavior on the align axis. "partial" will keep the content in the boundary as long as the trigger is at least partially in the boundary whilst "always" will keep the content in the boundary regardless. Defaults to "partial".
-            hide_when_detached: Whether to hide the content when the trigger becomes fully occluded. Defaults to False.
+            *children: The children of the component.
+            x: The x-coordinate of grid.
+            y: The y-coordinate of grid.
+            width: The width of grid.
+            height: The height of grid.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuItem(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class CartesianGrid(Grid):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        shortcut: Optional[Union[Var[str], str]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        text_value: Optional[Union[Var[str], str]] = None,
+        horizontal: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        vertical: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        fill_opacity: Optional[Union[Var[float], float]] = None,
+        stroke_dasharray: Optional[Union[Var[str], str]] = None,
+        x: Optional[Union[Var[int], int]] = None,
+        y: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -1152,124 +1703,79 @@
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_select: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuItem":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "CartesianGrid":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            shortcut: Shortcut to render a menu item as a link
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior. Defaults to False.
-            disabled: When true, prevents the user from interacting with the item.
-            text_value: Optional text used for typeahead purposes. By default the typeahead behavior will use the .textContent of the item. Use this when the content is complex, or you have non-textual content inside.
+            *children: The children of the component.
+            horizontal: The horizontal line configuration.
+            vertical: The vertical line configuration.
+            fill: The background of grid.
+            fill_opacity: The opacity of the background used to fill the space between grid lines
+            stroke_dasharray: The pattern of dashes and gaps used to paint the lines of the grid
+            x: The x-coordinate of grid.
+            y: The y-coordinate of grid.
+            width: The width of grid.
+            height: The height of grid.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class DropdownMenuSeparator(RadixThemesComponent):
+class CartesianAxis(Grid):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        orientation: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["top", "bottom", "left", "right"]],
+                Literal["top", "bottom", "left", "right"],
+            ]
+        ] = None,
+        axis_line: Optional[Union[Var[bool], bool]] = None,
+        tick_line: Optional[Union[Var[bool], bool]] = None,
+        tick_size: Optional[Union[Var[int], int]] = None,
+        interval: Optional[
+            Union[
+                Var[Literal["preserveStart", "preserveEnd", "preserveStartEnd"]],
+                Literal["preserveStart", "preserveEnd", "preserveStartEnd"],
             ]
         ] = None,
+        ticks: Optional[Union[Var[bool], bool]] = None,
+        label: Optional[Union[Var[str], str]] = None,
+        mirror: Optional[Union[Var[bool], bool]] = None,
+        tick_margin: Optional[Union[Var[int], int]] = None,
+        x: Optional[Union[Var[int], int]] = None,
+        y: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -1309,42 +1815,37 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "DropdownMenuSeparator":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "CartesianAxis":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            *children: The children of the component.
+            orientation: The orientation of axis 'top' | 'bottom' | 'left' | 'right'
+            axis_line: If set false, no axis line will be drawn. If set a object, the option is the configuration of axis line.
+            tick_line: If set false, no axis tick lines will be drawn. If set a object, the option is the configuration of tick lines.
+            tick_size: The length of tick line.
+            interval: If set 0, all the ticks will be shown. If set preserveStart", "preserveEnd" or "preserveStartEnd", the ticks which is to be shown or hidden will be calculated automatically.
+            ticks: If set false, no ticks will be drawn.
+            label: If set a string or a number, default label will be drawn, and the option is content.
+            mirror: If set true, flips ticks around the axis line, displaying the labels inside the chart instead of outside.
+            tick_margin: The margin between tick line and tick.
+            x: The x-coordinate of grid.
+            y: The y-coordinate of grid.
+            width: The width of grid.
+            height: The height of grid.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-class DropdownMenu(SimpleNamespace):
-    root = staticmethod(DropdownMenuRoot.create)
-    trigger = staticmethod(DropdownMenuTrigger.create)
-    content = staticmethod(DropdownMenuContent.create)
-    sub_trigger = staticmethod(DropdownMenuSubTrigger.create)
-    sub = staticmethod(DropdownMenuSub.create)
-    sub_content = staticmethod(DropdownMenuSubContent.create)
-    item = staticmethod(DropdownMenuItem.create)
-    separator = staticmethod(DropdownMenuSeparator.create)
-
-dropdown_menu = DropdownMenu()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/hovercard.pyi` & `reflex-0.4.9a1/reflex/components/recharts/polar.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,59 @@
-"""Stub file for reflex/components/radix/themes/components/hovercard.py"""
+"""Stub file for reflex/components/recharts/polar.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, Literal
-from reflex import el
+from typing import Any, Dict, List, Union
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import RadixThemesComponent
+from .recharts import (
+    LiteralAnimationEasing,
+    LiteralGridType,
+    LiteralPolarRadiusType,
+    LiteralScale,
+    Recharts,
+)
 
-class HoverCardRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Pie(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        open_delay: Optional[Union[Var[int], int]] = None,
-        close_delay: Optional[Union[Var[int], int]] = None,
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        start_angle: Optional[Union[Var[int], int]] = None,
+        end_angle: Optional[Union[Var[int], int]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        padding_angle: Optional[Union[Var[int], int]] = None,
+        name_key: Optional[Union[Var[str], str]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        label_line: Optional[Union[Var[bool], bool]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -127,130 +61,76 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "HoverCardRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Pie":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
-            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
-            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
+            *children: The children of the component.
+            data: data
+            data_key: The key of each sector's value.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The inner radius of pie, which can be set to a percent value.
+            outer_radius: The outer radius of pie, which can be set to a percent value.
+            start_angle: The angle of first sector.
+            end_angle: The direction of sectors. 1 means clockwise and -1 means anticlockwise.
+            min_angle: The minimum angle of each unzero data.
+            padding_angle: The angle between two sectors.
+            name_key: The key of each sector's name.
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn.
+            label_line: If false set, label lines will not be drawn.
+            fill: fill color
+            stroke: stroke color
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class HoverCardTrigger(RadixThemesComponent):
+class Radar(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        points: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        dot: Optional[Union[Var[bool], bool]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        fill_opacity: Optional[Union[Var[float], float]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        animation_begin: Optional[Union[Var[int], int]] = None,
+        animation_duration: Optional[Union[Var[int], int]] = None,
+        animation_easing: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
+                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
             ]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -290,167 +170,199 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardTrigger":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Radar":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique in a radar chart.
+            points: The coordinates of all the vertexes of the radar shape, like [{ x, y }].
+            dot: If false set, dots will not be drawn
+            stroke: Stoke color
+            fill: Fill color
+            fill_opacity: opacity
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn
+            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
+            animation_duration: Specifies the duration of animation, the unit of this option is ms.
+            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class HoverCardContent(el.Div, RadixThemesComponent):
+class RadialBar(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        side: Optional[
-            Union[
-                Var[Literal["top", "right", "bottom", "left"]],
-                Literal["top", "right", "bottom", "left"],
-            ]
-        ] = None,
-        side_offset: Optional[Union[Var[int], int]] = None,
-        align: Optional[
-            Union[
-                Var[Literal["start", "center", "end"]],
-                Literal["start", "center", "end"],
-            ]
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        background: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        avoid_collisions: Optional[Union[Var[bool], bool]] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        **props
+    ) -> "RadialBar":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: The source data which each element is an object.
+            min_angle: Min angle of each bar. A positive value between 0 and 360.
+            legend_type: Type of legend
+            label: If false set, labels will not be drawn.
+            background: If false set, background sector will not be drawn.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class PolarAngleAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        axis_line_type: Optional[Union[Var[str], str]] = None,
+        tick_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        ticks: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        orient: Optional[Union[Var[str], str]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        **props
+    ) -> "PolarAngleAxis":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data_key: The key of a group of data which should be unique to show the meaning of angle axis.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            radius: The outer radius of circle grid. If set a percentage, the final value is obtained by multiplying the percentage of maxRadius which is calculated by the width, height, cx, cy.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            axis_line_type: The type of axis line.
+            tick_line: If false set, tick lines will not be drawn. If true set, tick lines will be drawn which have the props calculated internally. If object set, tick lines will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            ticks: The array of every tick's value and angle.
+            orient: The orientation of axis text.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class PolarGrid(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        polar_angles: Optional[Union[Var[List[int]], List[int]]] = None,
+        polar_radius: Optional[Union[Var[List[int]], List[int]]] = None,
+        grid_type: Optional[
+            Union[Var[Literal["polygon", "circle"]], Literal["polygon", "circle"]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -490,161 +402,109 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HoverCardContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "PolarGrid":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            side: The preferred side of the trigger to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
-            side_offset: The distance in pixels from the trigger.
-            align: The preferred alignment against the trigger. May change when collisions occur.
-            avoid_collisions: Whether or not the hover card should avoid collisions with its trigger.
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The radius of the inner polar grid.
+            outer_radius: The radius of the outer polar grid.
+            polar_angles: The array of every line grid's angle.
+            polar_radius: The array of every line grid's radius.
+            grid_type: The type of polar grids. 'polygon' | 'circle'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class HoverCard(SimpleNamespace):
-    root = staticmethod(HoverCardRoot.create)
-    trigger = staticmethod(HoverCardTrigger.create)
-    content = staticmethod(HoverCardContent.create)
-
-    @staticmethod
-    def __call__(
+class PolarRadiusAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        angle: Optional[Union[Var[int], int]] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[Union[Var[str], str]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        tick_count: Optional[Union[Var[int], int]] = None,
+        scale: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
                 ],
             ]
         ] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        open_delay: Optional[Union[Var[int], int]] = None,
-        close_delay: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -652,49 +512,36 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "HoverCardRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "PolarRadiusAxis":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            default_open: The open state of the hover card when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the hover card. Must be used in conjunction with onOpenChange.
-            open_delay: The duration from when the mouse enters the trigger until the hover card opens.
-            close_delay: The duration from when the mouse leaves the trigger until the hover card closes.
+            *children: The children of the component.
+            angle: The angle of radial direction line to display axis text.
+            type_: The type of axis line. 'number' | 'category'
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            cx: The x-coordinate of center.
+            cy: The y-coordinate of center.
+            reversed: If set to true, the ticks of this axis are reversed.
+            orientation: The orientation of axis text.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            tick_count: The count of ticks.
+            scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-hover_card = HoverCard()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/iconbutton.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-"""Stub file for reflex/components/radix/themes/components/iconbutton.py"""
+"""Stub file for reflex/components/radix/themes/typography/link.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
-from reflex.components.component import Component
-from reflex.components.core.match import Match
-from reflex.components.lucide import Icon
-from reflex.style import Style
+from reflex.components.component import Component, MemoizationLeaf
+from reflex.components.core.cond import cond
+from reflex.components.el.elements.inline import A
+from reflex.components.next.link import NextLink
+from reflex.utils import imports
 from reflex.vars import Var
-from ..base import (
-    LiteralAccentColor,
-    LiteralRadius,
-    LiteralVariant,
-    RadixThemesComponent,
-)
+from ..base import LiteralAccentColor, RadixThemesComponent
+from .base import LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
-LiteralButtonSize = Literal["1", "2", "3", "4"]
+LiteralLinkUnderline = Literal["auto", "hover", "always"]
+next_link = NextLink.create()
 
-class IconButton(el.Button, RadixThemesComponent):
+class Link(RadixThemesComponent, A, MemoizationLeaf):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         size: Optional[
-            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+            Union[
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        weight: Optional[
+            Union[
+                Var[Literal["light", "regular", "medium", "bold"]],
+                Literal["light", "regular", "medium", "bold"],
+            ]
         ] = None,
-        variant: Optional[
+        trim: Optional[
             Union[
-                Var[Literal["classic", "solid", "soft", "surface", "outline", "ghost"]],
-                Literal["classic", "solid", "soft", "surface", "outline", "ghost"],
+                Var[Literal["normal", "start", "end", "both"]],
+                Literal["normal", "start", "end", "both"],
+            ]
+        ] = None,
+        underline: Optional[
+            Union[
+                Var[Literal["auto", "hover", "always"]],
+                Literal["auto", "hover", "always"],
             ]
         ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
@@ -98,43 +110,34 @@
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
         high_contrast: Optional[Union[Var[bool], bool]] = None,
-        radius: Optional[
-            Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
-            ]
-        ] = None,
-        auto_focus: Optional[
+        is_external: Optional[Union[Var[bool], bool]] = None,
+        download: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        form_action: Optional[
+        href: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        href_lang: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        form_enc_type: Optional[
+        media: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        form_method: Optional[
+        ping: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        referrer_policy: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        form_no_validate: Optional[
+        rel: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        shape: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        form_target: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        name: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        type: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        value: Optional[
+        target: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -174,15 +177,14 @@
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -222,36 +224,36 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "IconButton":
-        """Create a IconButton component.
+    ) -> "Link":
+        """Create a Link component.
 
         Args:
             *children: The children of the component.
             as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            size: Button size "1" - "4"
-            variant: Variant of button: "classic" | "solid" | "soft" | "surface" | "outline" | "ghost"
-            color_scheme: Override theme color for button
-            high_contrast: Whether to render the button with higher contrast color against background
-            radius: Override theme radius for button: "none" | "small" | "medium" | "large" | "full"
-            auto_focus: Automatically focuses the button when the page loads
-            disabled: Disables the button
-            form: Associates the button with a form (by id)
-            form_action: URL to send the form data to (for type="submit" buttons)
-            form_enc_type: How the form data should be encoded when submitting to the server (for type="submit" buttons)
-            form_method: HTTP method to use for sending form data (for type="submit" buttons)
-            form_no_validate: Bypasses form validation when submitting (for type="submit" buttons)
-            form_target: Specifies where to display the response after submitting the form (for type="submit" buttons)
-            name: Name of the button, used when sending form data
-            type: Type of the button (submit, reset, or button)
-            value: Value of the button, used when sending form data
+            size: Text size: "1" - "9"
+            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
+            underline: Sets the visibility of the underline affordance: "auto" | "hover" | "always"
+            color_scheme: Overrides the accent color inherited from the Theme.
+            high_contrast: Whether to render the text with higher contrast color
+            is_external: If True, the link will open in a new tab
+            download: Specifies that the target (the file specified in the href attribute) will be downloaded when a user clicks on the hyperlink.
+            href: Specifies the URL of the page the link goes to
+            href_lang: Specifies the language of the linked document
+            media: Specifies what media/device the linked document is optimized for
+            ping: Specifies which referrer is sent when fetching the resource
+            referrer_policy: Specifies the relationship between the current document and the linked document
+            rel: Specifies the relationship between the linked document and the current document
+            shape: Specifies the shape of the area
+            target: Specifies where to open the linked document
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -265,20 +267,17 @@
             tab_index: Defines the position of the current element in the tabbing order.
             title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Raises:
-            ValueError: If no children are passed.
+            ValueError: in case of missing children
 
         Returns:
-            The IconButton component.
+            Component: The link component
         """
         ...
-
-icon_button = IconButton.create
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/radiogroup.pyi` & `reflex-0.4.9a1/reflex/components/recharts/general.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,50 @@
-"""Stub file for reflex/components/radix/themes/components/radiogroup.py"""
-
+"""Stub file for reflex/components/recharts/general.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, List, Literal, Optional, Union
-import reflex as rx
-from reflex.components.component import Component
-from reflex.components.radix.themes.layout.flex import Flex
-from reflex.components.radix.themes.typography.text import Text
+from typing import Any, Dict, List, Union
+from reflex.components.component import MemoizationLeaf
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, LiteralSpacing, RadixThemesComponent
-
-LiteralFlexDirection = Literal["row", "column", "row-reverse", "column-reverse"]
+from .recharts import (
+    LiteralIconType,
+    LiteralLayout,
+    LiteralLegendAlign,
+    LiteralPosition,
+    LiteralVerticalAlign,
+    Recharts,
+)
 
-class RadioGroupRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class ResponsiveContainer(Recharts, MemoizationLeaf):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
-            ]
-        ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
+        aspect: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        height: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        min_width: Optional[Union[Var[int], int]] = None,
+        min_height: Optional[Union[Var[int], int]] = None,
+        debounce: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -156,117 +80,166 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RadioGroupRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "ResponsiveContainer":
+        """Create a new memoization leaf component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            size: The size of the radio group: "1" | "2" | "3"
-            variant: The variant of the radio group
-            high_contrast: Whether to render the radio group with higher contrast color against background
-            value: The controlled value of the radio item to check. Should be used in conjunction with on_change.
-            default_value: The initial value of checked radio item. Should be used in conjunction with on_change.
-            disabled: Whether the radio group is disabled
-            name: The name of the group. Submitted with its owning form as part of a name/value pair.
-            required: Whether the radio group is required
-            style: Props to rename  The style of the component.
+            *children: The children of the component.
+            aspect: The aspect ratio of the container. The final aspect ratio of the SVG element will be (width / height) * aspect. Number
+            width: The width of chart container. Can be a number or string
+            height: The height of chart container. Number
+            min_width: The minimum width of chart container.
+            min_height: The minimum height of chart container. Number
+            debounce: If specified a positive number, debounced function will be used to handle the resize event.
+            style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The memoization leaf
         """
         ...
 
-class RadioGroupItem(RadixThemesComponent):
+class Legend(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        align: Optional[
+            Union[
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
+            ]
+        ] = None,
+        vertical_align: Optional[
+            Union[
+                Var[Literal["top", "middle", "bottom"]],
+                Literal["top", "middle", "bottom"],
+            ]
+        ] = None,
+        icon_size: Optional[Union[Var[int], int]] = None,
+        icon_type: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "line",
+                        "plainline",
+                        "square",
+                        "rect",
+                        "circle",
+                        "cross",
+                        "diamond",
+                        "star",
+                        "triangle",
+                        "wye",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "line",
+                    "plainline",
+                    "square",
+                    "rect",
+                    "circle",
+                    "cross",
+                    "diamond",
+                    "star",
+                    "triangle",
+                    "wye",
                 ],
             ]
         ] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
+        chart_width: Optional[Union[Var[int], int]] = None,
+        chart_height: Optional[Union[Var[int], int]] = None,
+        margin: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Legend":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            width: The width of legend container. Number
+            height: The height of legend container. Number
+            layout: The layout of legend items. 'horizontal' | 'vertical'
+            align: The alignment of legend items in 'horizontal' direction, which can be 'left', 'center', 'right'.
+            vertical_align: The alignment of legend items in 'vertical' direction, which can be 'top', 'middle', 'bottom'.
+            icon_size: The size of icon in each legend item.
+            icon_type: The type of icon in each legend item. 'line' | 'plainline' | 'square' | 'rect' | 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye'
+            chart_width: The width of chart container, usually calculated internally.
+            chart_height: The height of chart container, usually calculated internally.
+            margin: The margin of chart container, usually calculated internally.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class GraphingTooltip(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        separator: Optional[Union[Var[str], str]] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        filter_null: Optional[Union[Var[bool], bool]] = None,
+        cursor: Optional[Union[Var[bool], bool]] = None,
+        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        active: Optional[Union[Var[bool], bool]] = None,
+        position: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        coordinate: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -311,136 +284,95 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RadioGroupItem":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "GraphingTooltip":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            value: The value of the radio item to check. Should be used in conjunction with on_change.
-            disabled: When true, prevents the user from interacting with the radio item.
-            required: When true, indicates that the user must check the radio item before the owning form can be submitted.
+            *children: The children of the component.
+            separator: The separator between name and value.
+            offset: The offset size of tooltip. Number
+            filter_null: When an item of the payload has value null or undefined, this item won't be displayed.
+            cursor: If set false, no cursor will be drawn when tooltip is active.
+            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
+            active: If set true, the tooltip is displayed. If set false, the tooltip is hidden, usually calculated internally.
+            position: If this field is set, the tooltip position will be fixed and will not move anymore.
+            coordinate: The coordinate of tooltip which is usually calculated internally.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class HighLevelRadioGroup(RadixThemesComponent):
+class Label(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        items: Optional[Union[Var[List[str]], List[str]]] = None,
-        direction: Optional[
-            Union[
-                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
-                Literal["row", "column", "row-reverse", "column-reverse"],
-            ]
-        ] = None,
-        spacing: Optional[
-            Union[
-                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
-            ]
-        ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
-            ]
-        ] = None,
-        color_scheme: Optional[
+        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        position: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "top",
+                        "left",
+                        "right",
+                        "bottom",
+                        "inside",
+                        "outside",
+                        "insideLeft",
+                        "insideRight",
+                        "insideTop",
+                        "insideBottom",
+                        "insideTopLeft",
+                        "insideBottomLeft",
+                        "insideTopRight",
+                        "insideBottomRight",
+                        "insideStart",
+                        "insideEnd",
+                        "end",
+                        "center",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "top",
+                    "left",
+                    "right",
+                    "bottom",
+                    "inside",
+                    "outside",
+                    "insideLeft",
+                    "insideRight",
+                    "insideTop",
+                    "insideBottom",
+                    "insideTopLeft",
+                    "insideBottomLeft",
+                    "insideTopRight",
+                    "insideBottomRight",
+                    "insideStart",
+                    "insideEnd",
+                    "end",
+                    "center",
                 ],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -485,141 +417,92 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HighLevelRadioGroup":
-        """Create a radio group component.
+    ) -> "Label":
+        """Create the component.
 
         Args:
-            items: The items of the radio group.
-            items: The items of the radio group.
-            direction: The direction of the radio group.
-            spacing: The gap between the items of the radio group.
-            size: The size of the radio group.
-            variant: The variant of the radio group
-            color_scheme: The color of the radio group
-            high_contrast: Whether to render the radio group with higher contrast color against background
-            value: The controlled value of the radio item to check. Should be used in conjunction with on_change.
-            default_value: The initial value of checked radio item. Should be used in conjunction with on_change.
-            disabled: Whether the radio group is disabled
-            name: The name of the group. Submitted with its owning form as part of a name/value pair.
-            required: Whether the radio group is required
-            style: Props to rename  The style of the component.
+            *children: The children of the component.
+            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
+            value: The value of label, which can be specified by this props or the children of <Label />
+            offset: The offset of label which can be specified by this props or the children of <Label />
+            position: The position of label which can be specified by this props or the children of <Label />
+            style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Additional properties to apply to the accordion item.
+            **props: The props of the component.
 
         Returns:
-            The created radio group component.
+            The component.
         """
         ...
 
-class RadioGroup(SimpleNamespace):
-    root = staticmethod(RadioGroupRoot.create)
-    item = staticmethod(RadioGroupItem.create)
-
-    @staticmethod
-    def __call__(
+class LabelList(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
         *children,
-        items: Optional[Union[Var[List[str]], List[str]]] = None,
-        direction: Optional[
-            Union[
-                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
-                Literal["row", "column", "row-reverse", "column-reverse"],
-            ]
-        ] = None,
-        spacing: Optional[
-            Union[
-                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
-            ]
-        ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
-            ]
-        ] = None,
-        color_scheme: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        position: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "top",
+                        "left",
+                        "right",
+                        "bottom",
+                        "inside",
+                        "outside",
+                        "insideLeft",
+                        "insideRight",
+                        "insideTop",
+                        "insideBottom",
+                        "insideTopLeft",
+                        "insideBottomLeft",
+                        "insideTopRight",
+                        "insideBottomRight",
+                        "insideStart",
+                        "insideEnd",
+                        "end",
+                        "center",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "top",
+                    "left",
+                    "right",
+                    "bottom",
+                    "inside",
+                    "outside",
+                    "insideLeft",
+                    "insideRight",
+                    "insideTop",
+                    "insideBottom",
+                    "insideTopLeft",
+                    "insideBottomLeft",
+                    "insideTopRight",
+                    "insideBottomRight",
+                    "insideStart",
+                    "insideEnd",
+                    "end",
+                    "center",
                 ],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -664,38 +547,29 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HighLevelRadioGroup":
-        """Create a radio group component.
+    ) -> "LabelList":
+        """Create the component.
 
         Args:
-            items: The items of the radio group.
-            items: The items of the radio group.
-            direction: The direction of the radio group.
-            spacing: The gap between the items of the radio group.
-            size: The size of the radio group.
-            variant: The variant of the radio group
-            color_scheme: The color of the radio group
-            high_contrast: Whether to render the radio group with higher contrast color against background
-            value: The controlled value of the radio item to check. Should be used in conjunction with on_change.
-            default_value: The initial value of checked radio item. Should be used in conjunction with on_change.
-            disabled: Whether the radio group is disabled
-            name: The name of the group. Submitted with its owning form as part of a name/value pair.
-            required: Whether the radio group is required
-            style: Props to rename  The style of the component.
+            *children: The children of the component.
+            data_key: The key of a group of label values in data.
+            position: The position of each label relative to it view box。"Top" | "left" | "right" | "bottom" | "inside" | "outside" | "insideLeft" | "insideRight" | "insideTop" | "insideBottom" | "insideTopLeft" | "insideBottomLeft" | "insideTopRight" | "insideBottomRight" | "insideStart" | "insideEnd" | "end" | "center"
+            offset: The offset to the specified "position"
+            fill: Color of the fill
+            stroke: Color of the stroke
+            style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Additional properties to apply to the accordion item.
+            **props: The props of the component.
 
         Returns:
-            The created radio group component.
+            The component.
         """
         ...
-
-radio_group = RadioGroup()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/scrollarea.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,46 @@
-"""Stub file for reflex/components/radix/themes/components/scrollarea.py"""
+"""Stub file for reflex/components/radix/themes/components/switch.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Literal
+from typing import Any, Dict, Literal
+from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import RadixThemesComponent
+from ..base import LiteralAccentColor, RadixThemesComponent
 
-class ScrollArea(RadixThemesComponent):
+LiteralSwitchSize = Literal["1", "2", "3"]
+
+class Switch(RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        default_checked: Optional[Union[Var[bool], bool]] = None,
+        checked: Optional[Union[Var[bool], bool]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        required: Optional[Union[Var[bool], bool]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        size: Optional[
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        ] = None,
+        variant: Optional[
+            Union[
+                Var[Literal["classic", "surface", "soft"]],
+                Literal["classic", "surface", "soft"],
+            ]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -76,37 +95,32 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        scrollbars: Optional[
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        radius: Optional[
             Union[
-                Var[Literal["vertical", "horizontal", "both"]],
-                Literal["vertical", "horizontal", "both"],
+                Var[Literal["none", "small", "full"]], Literal["none", "small", "full"]
             ]
         ] = None,
-        type_: Optional[
-            Union[
-                Var[Literal["auto", "always", "scroll", "hover"]],
-                Literal["auto", "always", "scroll", "hover"],
-            ]
-        ] = None,
-        scroll_hide_delay: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -142,35 +156,41 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ScrollArea":
+    ) -> "Switch":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            scrollbars: The alignment of the scroll area
-            type_: Describes the nature of scrollbar visibility, similar to how the scrollbar preferences in MacOS control visibility of native scrollbars. "auto" | "always" | "scroll" | "hover"
-            scroll_hide_delay: If type is set to either "scroll" or "hover", this prop determines the length of time, in milliseconds, before the scrollbars are hidden after the user stops interacting with scrollbars.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            default_checked: Whether the switch is checked by default
+            checked: Whether the switch is checked
+            disabled: If true, prevent the user from interacting with the switch
+            required: If true, the user must interact with the switch to submit the form
+            name: The name of the switch (when submitting a form)
+            value: The value associated with the "on" position
+            size: Switch size "1" - "4"
+            variant: Variant of switch: "classic" | "surface" | "soft"
+            color_scheme: Override theme color for switch
+            high_contrast: Whether to render the switch with higher contrast color against background
+            radius: Override theme radius for switch: "none" | "small" | "full"
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-scroll_area = ScrollArea.create
+switch = Switch.create
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/select.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/select.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,119 @@
-"""Stub file for reflex/components/radix/themes/components/select.py"""
+"""Stub file for reflex/components/radix/themes/typography/text.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Literal, Union
-import reflex as rx
-from reflex.components.component import Component, ComponentNamespace
-from reflex.constants import EventTriggers
+from typing import Literal
+from reflex import el
+from reflex.components.component import ComponentNamespace
 from reflex.vars import Var
-from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
+from ..base import LiteralAccentColor, RadixThemesComponent
+from .base import LiteralTextAlign, LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
-class SelectRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+LiteralType = Literal[
+    "p",
+    "label",
+    "div",
+    "span",
+    "b",
+    "i",
+    "u",
+    "abbr",
+    "cite",
+    "del",
+    "em",
+    "ins",
+    "kbd",
+    "mark",
+    "s",
+    "samp",
+    "sub",
+    "sup",
+]
+
+class Text(el.Span, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        as_: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "p",
+                        "label",
+                        "div",
+                        "span",
+                        "b",
+                        "i",
+                        "u",
+                        "abbr",
+                        "cite",
+                        "del",
+                        "em",
+                        "ins",
+                        "kbd",
+                        "mark",
+                        "s",
+                        "samp",
+                        "sub",
+                        "sup",
+                    ]
+                ],
+                Literal[
+                    "p",
+                    "label",
+                    "div",
+                    "span",
+                    "b",
+                    "i",
+                    "u",
+                    "abbr",
+                    "cite",
+                    "del",
+                    "em",
+                    "ins",
+                    "kbd",
+                    "mark",
+                    "s",
+                    "samp",
+                    "sub",
+                    "sup",
+                ],
+            ]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        size: Optional[
+            Union[
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
         ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        weight: Optional[
+            Union[
+                Var[Literal["light", "regular", "medium", "bold"]],
+                Literal["light", "regular", "medium", "bold"],
+            ]
         ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        align: Optional[
+            Union[
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
+            ]
         ] = None,
-        **props
-    ) -> "SelectRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
-
-        Args:
-            *children: Child components.
-            size: The size of the select: "1" | "2" | "3"
-            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
-            value: The controlled value of the select. Should be used in conjunction with on_change.
-            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
-            name: The name of the select control when submitting the form.
-            disabled: When True, prevents the user from interacting with select.
-            required: When True, indicates that the user must select a value before the owning form can be submitted.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Component properties.
-
-        Returns:
-            A new component instance.
-        """
-        ...
-
-class SelectTrigger(RadixThemesComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        variant: Optional[
+        trim: Optional[
             Union[
-                Var[Literal["classic", "surface", "soft", "ghost"]],
-                Literal["classic", "surface", "soft", "ghost"],
+                Var[Literal["normal", "start", "end", "both"]],
+                Literal["normal", "start", "end", "both"],
             ]
         ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
@@ -188,21 +170,55 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
-        radius: Optional[
-            Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
-            ]
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -247,48 +263,135 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectTrigger":
+    ) -> "Text":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            variant: Variant of the select trigger
-            color_scheme: The color of the select trigger
-            radius: The radius of the select trigger
-            placeholder: The placeholder of the select trigger
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            as_: Change the default rendered element into a semantically appropriate alternative (cannot be used with asChild)
+            size: Text size: "1" - "9"
+            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            align: Alignment of text in element: "left" | "center" | "right"
+            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
+            color_scheme: Overrides the accent color inherited from the Theme.
+            high_contrast: Whether to render the text with higher contrast color
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class SelectContent(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Span(Text):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        variant: Optional[
-            Union[Var[Literal["solid", "soft"]], Literal["solid", "soft"]]
+        as_: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "p",
+                        "label",
+                        "div",
+                        "span",
+                        "b",
+                        "i",
+                        "u",
+                        "abbr",
+                        "cite",
+                        "del",
+                        "em",
+                        "ins",
+                        "kbd",
+                        "mark",
+                        "s",
+                        "samp",
+                        "sub",
+                        "sup",
+                    ]
+                ],
+                Literal[
+                    "p",
+                    "label",
+                    "div",
+                    "span",
+                    "b",
+                    "i",
+                    "u",
+                    "abbr",
+                    "cite",
+                    "del",
+                    "em",
+                    "ins",
+                    "kbd",
+                    "mark",
+                    "s",
+                    "samp",
+                    "sub",
+                    "sup",
+                ],
+            ]
+        ] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        size: Optional[
+            Union[
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        weight: Optional[
+            Union[
+                Var[Literal["light", "regular", "medium", "bold"]],
+                Literal["light", "regular", "medium", "bold"],
+            ]
+        ] = None,
+        align: Optional[
+            Union[
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
+            ]
+        ] = None,
+        trim: Optional[
+            Union[
+                Var[Literal["normal", "start", "end", "both"]],
+                Literal["normal", "start", "end", "both"],
+            ]
         ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
@@ -345,58 +448,72 @@
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
         high_contrast: Optional[Union[Var[bool], bool]] = None,
-        position: Optional[
-            Union[
-                Var[Literal["item-aligned", "popper"]],
-                Literal["item-aligned", "popper"],
-            ]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        side: Optional[
-            Union[
-                Var[Literal["top", "right", "bottom", "left"]],
-                Literal["top", "right", "bottom", "left"],
-            ]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        side_offset: Optional[Union[Var[int], int]] = None,
-        align: Optional[
-            Union[
-                Var[Literal["start", "center", "end"]],
-                Literal["start", "center", "end"],
-            ]
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        align_offset: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_close_auto_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_escape_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
@@ -416,59 +533,112 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_pointer_down_outside: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectContent":
+    ) -> "Span":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            variant: The variant of the select content
-            color_scheme: The color of the select content
-            high_contrast: Whether to render the select content with higher contrast color against background
-            position: The positioning mode to use, item-aligned is the default and behaves similarly to a native MacOS menu by positioning content relative to the active item. popper positions content in the same way as our other primitives, for example Popover or DropdownMenu.
-            side: The preferred side of the anchor to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled. Only available when position is set to popper.
-            side_offset: The distance in pixels from the anchor. Only available when position is set to popper.
-            align: The preferred alignment against the anchor. May change when collisions occur. Only available when position is set to popper.
-            align_offset: The vertical distance in pixels from the anchor. Only available when position is set to popper.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            as_: Change the default rendered element into a semantically appropriate alternative (cannot be used with asChild)
+            size: Text size: "1" - "9"
+            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            align: Alignment of text in element: "left" | "center" | "right"
+            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
+            color_scheme: Overrides the accent color inherited from the Theme.
+            high_contrast: Whether to render the text with higher contrast color
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class SelectGroup(RadixThemesComponent):
+class Em(el.Em, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -513,43 +683,103 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectGroup":
+    ) -> "Em":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class SelectItem(RadixThemesComponent):
+class Kbd(el.Kbd, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
+        size: Optional[
+            Union[
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -594,43 +824,99 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectItem":
+    ) -> "Kbd":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            value: The value given as data when submitting a form with a name.
-            disabled: Whether the select item is disabled
+            size: Text size: "1" - "9"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class SelectLabel(RadixThemesComponent):
+class Quote(el.Q, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        cite: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -675,41 +961,98 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectLabel":
+    ) -> "Quote":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
+            cite: Specifies the source URL of the quote.
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class SelectSeparator(RadixThemesComponent):
+class Strong(el.Strong, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -754,244 +1097,132 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SelectSeparator":
+    ) -> "Strong":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class HighLevelSelect(SelectRoot):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
+class TextNamespace(ComponentNamespace):
+    em = staticmethod(Em.create)
+    kbd = staticmethod(Kbd.create)
+    quote = staticmethod(Quote.create)
+    strong = staticmethod(Strong.create)
+    span = staticmethod(Span.create)
+
+    @staticmethod
+    def __call__(
         *children,
-        items: Optional[Union[Var[List[str]], List[str]]] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        as_: Optional[
             Union[
                 Var[
                     Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                        "p",
+                        "label",
+                        "div",
+                        "span",
+                        "b",
+                        "i",
+                        "u",
+                        "abbr",
+                        "cite",
+                        "del",
+                        "em",
+                        "ins",
+                        "kbd",
+                        "mark",
+                        "s",
+                        "samp",
+                        "sub",
+                        "sup",
                     ]
                 ],
                 Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                    "p",
+                    "label",
+                    "div",
+                    "span",
+                    "b",
+                    "i",
+                    "u",
+                    "abbr",
+                    "cite",
+                    "del",
+                    "em",
+                    "ins",
+                    "kbd",
+                    "mark",
+                    "s",
+                    "samp",
+                    "sub",
+                    "sup",
                 ],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        variant: Optional[
+        size: Optional[
             Union[
-                Var[Literal["classic", "surface", "soft", "ghost"]],
-                Literal["classic", "surface", "soft", "ghost"],
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
             ]
         ] = None,
-        radius: Optional[
+        weight: Optional[
             Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
+                Var[Literal["light", "regular", "medium", "bold"]],
+                Literal["light", "regular", "medium", "bold"],
             ]
         ] = None,
-        width: Optional[Union[Var[str], str]] = None,
-        position: Optional[
+        align: Optional[
             Union[
-                Var[Literal["item-aligned", "popper"]],
-                Literal["item-aligned", "popper"],
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
             ]
         ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        trim: Optional[
+            Union[
+                Var[Literal["normal", "start", "end", "both"]],
+                Literal["normal", "start", "end", "both"],
+            ]
         ] = None,
-        **props
-    ) -> "HighLevelSelect":
-        """Create a select component.
-
-        Args:
-            items: The items of the select.
-            items: The items of the select.
-            placeholder: The placeholder of the select.
-            label: The label of the select.
-            color_scheme: The color of the select.
-            high_contrast: Whether to render the select with higher contrast color against background.
-            variant: The variant of the select.
-            radius: The radius of the select.
-            width: The width of the select.
-            position: The positioning mode to use. Default is "item-aligned".
-            size: The size of the select: "1" | "2" | "3"
-            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
-            value: The controlled value of the select. Should be used in conjunction with on_change.
-            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
-            name: The name of the select control when submitting the form.
-            disabled: When True, prevents the user from interacting with select.
-            required: When True, indicates that the user must select a value before the owning form can be submitted.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: Additional properties to apply to the select component.
-
-        Returns:
-            The select component.
-        """
-        ...
-
-class Select(ComponentNamespace):
-    root = staticmethod(SelectRoot.create)
-    trigger = staticmethod(SelectTrigger.create)
-    content = staticmethod(SelectContent.create)
-    group = staticmethod(SelectGroup.create)
-    item = staticmethod(SelectItem.create)
-    separator = staticmethod(SelectSeparator.create)
-    label = staticmethod(SelectLabel.create)
-
-    @staticmethod
-    def __call__(
-        *children,
-        items: Optional[Union[Var[List[str]], List[str]]] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[str], str]] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -1047,55 +1278,63 @@
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
         high_contrast: Optional[Union[Var[bool], bool]] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft", "ghost"]],
-                Literal["classic", "surface", "soft", "ghost"],
-            ]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        radius: Optional[
-            Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
-            ]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        width: Optional[Union[Var[str], str]] = None,
-        position: Optional[
-            Union[
-                Var[Literal["item-aligned", "popper"]],
-                Literal["item-aligned", "popper"],
-            ]
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        default_open: Optional[Union[Var[bool], bool]] = None,
-        open: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -1124,53 +1363,60 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_open_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "HighLevelSelect":
-        """Create a select component.
+    ) -> "Text":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            items: The items of the select.
-            items: The items of the select.
-            placeholder: The placeholder of the select.
-            label: The label of the select.
-            color_scheme: The color of the select.
-            high_contrast: Whether to render the select with higher contrast color against background.
-            variant: The variant of the select.
-            radius: The radius of the select.
-            width: The width of the select.
-            position: The positioning mode to use. Default is "item-aligned".
-            size: The size of the select: "1" | "2" | "3"
-            default_value: The value of the select when initially rendered. Use when you do not need to control the state of the select.
-            value: The controlled value of the select. Should be used in conjunction with on_change.
-            default_open: The open state of the select when it is initially rendered. Use when you do not need to control its open state.
-            open: The controlled open state of the select. Must be used in conjunction with on_open_change.
-            name: The name of the select control when submitting the form.
-            disabled: When True, prevents the user from interacting with select.
-            required: When True, indicates that the user must select a value before the owning form can be submitted.
+            *children: Child components.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            as_: Change the default rendered element into a semantically appropriate alternative (cannot be used with asChild)
+            size: Text size: "1" - "9"
+            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            align: Alignment of text in element: "left" | "center" | "right"
+            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
+            color_scheme: Overrides the accent color inherited from the Theme.
+            high_contrast: Whether to render the text with higher contrast color
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Additional properties to apply to the select component.
+            **props: Component properties.
 
         Returns:
-            The select component.
+            A new component instance.
         """
         ...
 
-select = Select()
+text = TextNamespace()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.4.9a1/reflex/components/recharts/recharts.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,101 @@
-"""Stub file for reflex/components/radix/themes/components/separator.py"""
+"""Stub file for reflex/components/recharts/recharts.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from reflex.components.component import Component, MemoizationLeaf, NoSSRComponent
 
-LiteralSeperatorSize = Literal["1", "2", "3", "4"]
-
-class Separator(RadixThemesComponent):
+class Recharts(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3", "4"]], Literal["1", "2", "3", "4"]]
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        decorative: Optional[Union[Var[bool], bool]] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Recharts":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class RechartsCharts(NoSSRComponent, MemoizationLeaf):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -139,33 +140,126 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Separator":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "RechartsCharts":
+        """Create a new memoization leaf component.
 
         Args:
-            *children: Child components.
-            size: The size of the select: "1" | "2" | "3" | "4"
-            color_scheme: The color of the select
-            orientation: The orientation of the separator.
-            decorative: When true, signifies that it is purely visual, carries no semantic meaning, and ensures it is not present in the accessibility tree.
+            *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The memoization leaf
         """
         ...
 
-divider = separator = Separator.create
+LiteralAnimationEasing = Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]
+LiteralIfOverflow = Literal["discard", "hidden", "visible", "extendDomain"]
+LiteralShape = Literal[
+    "square", "circle", "cross", "diamond", "star", "triangle", "wye"
+]
+LiteralLineType = Literal["joint", "fitting"]
+LiteralOrientation = Literal["top", "bottom", "left", "right", "middle"]
+LiteralOrientationLeftRightMiddle = Literal["left", "right", "middle"]
+LiteralOrientationTopBottom = Literal["top", "bottom"]
+LiteralOrientationTopBottomLeftRight = Literal["top", "bottom", "left", "right"]
+LiteralScale = Literal[
+    "auto",
+    "linear",
+    "pow",
+    "sqrt",
+    "log",
+    "identity",
+    "time",
+    "band",
+    "point",
+    "ordinal",
+    "quantile",
+    "quantize",
+    "utc",
+    "sequential",
+    "threshold",
+]
+LiteralLayout = Literal["horizontal", "vertical"]
+LiteralPolarRadiusType = Literal["number", "category"]
+LiteralGridType = Literal["polygon", "circle"]
+LiteralPosition = Literal[
+    "top",
+    "left",
+    "right",
+    "bottom",
+    "inside",
+    "outside",
+    "insideLeft",
+    "insideRight",
+    "insideTop",
+    "insideBottom",
+    "insideTopLeft",
+    "insideBottomLeft",
+    "insideTopRight",
+    "insideBottomRight",
+    "insideStart",
+    "insideEnd",
+    "end",
+    "center",
+]
+LiteralIconType = Literal[
+    "line",
+    "plainline",
+    "square",
+    "rect",
+    "circle",
+    "cross",
+    "diamond",
+    "star",
+    "triangle",
+    "wye",
+]
+LiteralLegendType = [
+    "line",
+    "plainline",
+    "square",
+    "rect",
+    "circle",
+    "cross",
+    "diamond",
+    "star",
+    "triangle",
+    "wye",
+    "none",
+]
+LiteralLegendAlign = Literal["left", "center", "right"]
+LiteralVerticalAlign = Literal["top", "middle", "bottom"]
+LiteralStackOffset = Literal["expand", "none", "wiggle", "silhouette"]
+LiteralBarChartStackOffset = Literal["expand", "none", "wiggle", "silhouette", "sign"]
+LiteralComposedChartBaseValue = Literal["dataMin", "dataMax", "auto"]
+LiteralAxisType = Literal["number", "category"]
+LiteralAreaType = Literal[
+    "basis",
+    "basisClosed",
+    "basisOpen",
+    "bumpX",
+    "bumpY",
+    "bump",
+    "linear",
+    "linearClosed",
+    "natural",
+    "monotoneX",
+    "monotoneY",
+    "monotone",
+    "step",
+    "stepBefore",
+    "stepAfter",
+]
+LiteralDirection = Literal["x", "y", "both"]
+LiteralInterval = Literal["preserveStart", "preserveEnd", "preserveStartEnd"]
+LiteralSyncMethod = Literal["index", "value"]
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,117 @@
-"""Stub file for reflex/components/radix/themes/components/switch.py"""
+"""Stub file for reflex/components/radix/themes/layout/grid.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, Literal
-from reflex.constants import EventTriggers
+from typing import Dict, Literal
+from reflex import el
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from ..base import LiteralAlign, LiteralJustify, LiteralSpacing, RadixThemesComponent
 
-LiteralSwitchSize = Literal["1", "2", "3"]
+LiteralGridFlow = Literal["row", "column", "dense", "row-dense", "column-dense"]
 
-class Switch(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class Grid(el.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
-        default_checked: Optional[Union[Var[bool], bool]] = None,
-        checked: Optional[Union[Var[bool], bool]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
-            ]
-        ] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+        columns: Optional[Union[Var[str], str]] = None,
+        rows: Optional[Union[Var[str], str]] = None,
+        flow: Optional[
+            Union[
+                Var[Literal["row", "column", "dense", "row-dense", "column-dense"]],
+                Literal["row", "column", "dense", "row-dense", "column-dense"],
+            ]
+        ] = None,
+        align: Optional[
+            Union[
+                Var[Literal["start", "center", "end", "baseline", "stretch"]],
+                Literal["start", "center", "end", "baseline", "stretch"],
+            ]
+        ] = None,
+        justify: Optional[
+            Union[
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        radius: Optional[
+        spacing: Optional[
             Union[
-                Var[Literal["none", "small", "full"]], Literal["none", "small", "full"]
+                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
             ]
         ] = None,
+        spacing_x: Optional[
+            Union[
+                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        spacing_y: Optional[
+            Union[
+                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -156,41 +147,52 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Switch":
+    ) -> "Grid":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
             as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            default_checked: Whether the switch is checked by default
-            checked: Whether the switch is checked
-            disabled: If true, prevent the user from interacting with the switch
-            required: If true, the user must interact with the switch to submit the form
-            name: The name of the switch (when submitting a form)
-            value: The value associated with the "on" position
-            size: Switch size "1" - "4"
-            variant: Variant of switch: "classic" | "surface" | "soft"
-            color_scheme: Override theme color for switch
-            high_contrast: Whether to render the switch with higher contrast color against background
-            radius: Override theme radius for switch: "none" | "small" | "full"
+            columns: Number of columns
+            rows: Number of rows
+            flow: How the grid items are layed out: "row" | "column" | "dense" | "row-dense" | "column-dense"
+            align: Alignment of children along the main axis: "start" | "center" | "end" | "baseline" | "stretch"
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            spacing: Gap between children: "0" - "9"
+            spacing_x: Gap between children horizontal: "0" - "9"
+            spacing_y: Gap between children vertical: "0" - "9"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
-
-switch = Switch.create
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/table.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/table.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/text_field.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/textfield.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,46 @@
-"""Stub file for reflex/components/radix/themes/components/textfield.py"""
+"""Stub file for reflex/components/radix/themes/layout/stack.py"""
 # ------------------- DO NOT EDIT ----------------------
-# This file was generated by `scripts/pyi_generator.py`!
+# This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from types import SimpleNamespace
-from typing import Any, Dict, Literal
-import reflex as rx
-from reflex.components import el
 from reflex.components.component import Component
-from reflex.components.core.debounce import DebounceInput
-from reflex.components.lucide.icon import Icon
-from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
+from ..base import LiteralAlign, LiteralSpacing
+from .flex import Flex, LiteralFlexDirection
 
-LiteralTextFieldSize = Literal["1", "2", "3"]
-LiteralTextFieldVariant = Literal["classic", "surface", "soft"]
-
-class TextFieldRoot(el.Div, RadixThemesComponent):
+class Stack(Flex):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
+        spacing: Optional[LiteralSpacing] = "2",
+        align: Optional[LiteralAlign] = "start",
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        direction: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
             ]
         ] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
+        justify: Optional[
             Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
             ]
         ] = None,
-        radius: Optional[
+        wrap: Optional[
             Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
             ]
         ] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -146,15 +80,14 @@
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
@@ -194,27 +127,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TextFieldRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Stack":
+        """Create a new instance of the component.
 
         Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            size: Text field size "1" - "3"
-            variant: Variant of text field: "classic" | "surface" | "soft"
-            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -228,174 +159,47 @@
             tab_index: Defines the position of the current element in the tabbing order.
             title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the stack.
 
         Returns:
-            A new component instance.
+            The stack component.
         """
         ...
 
-class TextFieldInput(el.Input, TextFieldRoot):
+class VStack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        accept: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        alt: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        auto_complete: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        auto_focus: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        capture: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        checked: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        dirname: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        disabled: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        form_action: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        form_enc_type: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        form_method: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        form_no_validate: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        form_target: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        list: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        max: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        max_length: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        min_length: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        min: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        multiple: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        name: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        pattern: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        placeholder: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        read_only: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        required: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        size: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        src: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        step: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        type: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        use_map: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        value: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        variant: Optional[
+        spacing: Optional[LiteralSpacing] = "2",
+        align: Optional[LiteralAlign] = "start",
+        direction: Optional[
             Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
             ]
         ] = None,
-        color_scheme: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        justify: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
             ]
         ] = None,
-        radius: Optional[
+        wrap: Optional[
             Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
             ]
         ] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -435,40 +239,30 @@
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_key_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -492,53 +286,25 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TextFieldInput":
-        """Create an Input component.
+    ) -> "VStack":
+        """Create a new instance of the component.
 
         Args:
-            *children: The children of the component.
-            accept: Accepted types of files when the input is file type
-            alt: Alternate text for input type="image"
-            auto_complete: Whether the input should have autocomplete enabled
-            auto_focus: Automatically focuses the input when the page loads
-            capture: Captures media from the user (camera or microphone)
-            checked: Indicates whether the input is checked (for checkboxes and radio buttons)
-            dirname: Name part of the input to submit in 'dir' and 'name' pair when form is submitted
-            disabled: Disables the input
-            form: Associates the input with a form (by id)
-            form_action: URL to send the form data to (for type="submit" buttons)
-            form_enc_type: How the form data should be encoded when submitting to the server (for type="submit" buttons)
-            form_method: HTTP method to use for sending form data (for type="submit" buttons)
-            form_no_validate: Bypasses form validation when submitting (for type="submit" buttons)
-            form_target: Specifies where to display the response after submitting the form (for type="submit" buttons)
-            list: References a datalist for suggested options
-            max: Specifies the maximum value for the input
-            max_length: Specifies the maximum number of characters allowed in the input
-            min_length: Specifies the minimum number of characters required in the input
-            min: Specifies the minimum value for the input
-            multiple: Indicates whether multiple values can be entered in an input of the type email or file
-            name: Name of the input, used when sending form data
-            pattern: Regex pattern the input's value must match to be valid
-            placeholder: Placeholder text in the input
-            read_only: Indicates whether the input is read-only
-            required: Indicates that the input is required
-            size: Text field size "1" - "3"
-            src: URL for image inputs
-            step: Specifies the legal number intervals for an input
-            type: Specifies the type of input
-            use_map: Name of the image map used with the input
-            value: Value of the input
-            variant: Variant of text field: "classic" | "surface" | "soft"
-            color_scheme: Override theme color for text field
-            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -552,484 +318,110 @@
             tab_index: Defines the position of the current element in the tabbing order.
             title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
-            custom_attrs: custom attribute
-            **props: The properties of the component.
-
-        Returns:
-            The component.
-        """
-        ...
-    def get_event_triggers(self) -> Dict[str, Any]: ...
-
-class TextFieldSlot(RadixThemesComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        color: Optional[Union[Var[str], str]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        **props
-    ) -> "TextFieldSlot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
-
-        Args:
-            *children: Child components.
-            color: map to CSS default color property.
-            color_scheme: map to radix color property.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The properties of the stack.
 
         Returns:
-            A new component instance.
+            The stack component.
         """
         ...
 
-class Input(RadixThemesComponent):
+class HStack(Stack):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        icon: Optional[Union[Var[str], str]] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
-        ] = None,
-        variant: Optional[
+        spacing: Optional[LiteralSpacing] = "2",
+        align: Optional[LiteralAlign] = "start",
+        direction: Optional[
             Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
+                Var[Literal["row", "column", "row-reverse", "column-reverse"]],
+                Literal["row", "column", "row-reverse", "column-reverse"],
             ]
         ] = None,
-        color_scheme: Optional[
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        justify: Optional[
             Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
+                Var[Literal["start", "center", "end", "between"]],
+                Literal["start", "center", "end", "between"],
             ]
         ] = None,
-        radius: Optional[
+        wrap: Optional[
             Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
+                Var[Literal["nowrap", "wrap", "wrap-reverse"]],
+                Literal["nowrap", "wrap", "wrap-reverse"],
             ]
         ] = None,
-        auto_complete: Optional[Union[Var[bool], bool]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        max_length: Optional[Union[Var[str], str]] = None,
-        min_length: Optional[Union[Var[str], str]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_key_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "Input":
-        """Create an Input component.
-
-        Args:
-            icon: The icon to render before the input.
-            size: Text field size "1" - "3"
-            variant: Variant of text field: "classic" | "surface" | "soft"
-            color_scheme: Override theme color for text field
-            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
-            auto_complete: Whether the input should have autocomplete enabled
-            default_value: The value of the input when initially rendered.
-            disabled: Disables the input
-            max_length: Specifies the maximum number of characters allowed in the input
-            min_length: Specifies the minimum number of characters required in the input
-            name: Name of the input, used when sending form data
-            placeholder: Placeholder text in the input
-            required: Indicates that the input is required
-            value: Value of the input
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
-            custom_attrs: custom attribute
-            **props: The properties of the component.
-
-        Returns:
-            The component.
-        """
-        ...
-    def get_event_triggers(self) -> Dict[str, Any]: ...
-
-class TextField(SimpleNamespace):
-    root = staticmethod(TextFieldRoot.create)
-    input = staticmethod(TextFieldInput.create)
-    slot = staticmethod(TextFieldSlot.create)
-
-    @staticmethod
-    def __call__(
-        *children,
-        icon: Optional[Union[Var[str], str]] = None,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "surface", "soft"]],
-                Literal["classic", "surface", "soft"],
-            ]
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        radius: Optional[
-            Union[
-                Var[Literal["none", "small", "medium", "large", "full"]],
-                Literal["none", "small", "medium", "large", "full"],
-            ]
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        auto_complete: Optional[Union[Var[bool], bool]] = None,
-        default_value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        max_length: Optional[Union[Var[str], str]] = None,
-        min_length: Optional[Union[Var[str], str]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        placeholder: Optional[Union[Var[str], str]] = None,
-        required: Optional[Union[Var[bool], bool]] = None,
-        value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
-        _rename_props: Optional[Dict[str, str]] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_key_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_key_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -1053,40 +445,46 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Input":
-        """Create an Input component.
+    ) -> "HStack":
+        """Create a new instance of the component.
 
         Args:
-            icon: The icon to render before the input.
-            size: Text field size "1" - "3"
-            variant: Variant of text field: "classic" | "surface" | "soft"
-            color_scheme: Override theme color for text field
-            radius: Override theme radius for text field: "none" | "small" | "medium" | "large" | "full"
-            auto_complete: Whether the input should have autocomplete enabled
-            default_value: The value of the input when initially rendered.
-            disabled: Disables the input
-            max_length: Specifies the maximum number of characters allowed in the input
-            min_length: Specifies the minimum number of characters required in the input
-            name: Name of the input, used when sending form data
-            placeholder: Placeholder text in the input
-            required: Indicates that the input is required
-            value: Value of the input
+            *children: The children of the stack.
+            spacing: The spacing between each stack item.
+            align: The alignment of the stack items.
+            direction: How child items are layed out: "row" | "column" | "row-reverse" | "column-reverse"
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
+            wrap: Whether children should wrap when they reach the end of their container: "nowrap" | "wrap" | "wrap-reverse"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
-            _rename_props: props to change the name of
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The properties of the stack.
 
         Returns:
-            The component.
+            The stack component.
         """
         ...
-
-text_field = TextField()
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.4.9a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,108 @@
-"""Stub file for reflex/components/radix/themes/layout/grid.py"""
+"""Stub file for reflex/components/radix/themes/typography/code.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Dict, Literal
 from reflex import el
 from reflex.vars import Var
-from ..base import LiteralAlign, LiteralJustify, LiteralSpacing, RadixThemesComponent
+from ..base import LiteralAccentColor, LiteralVariant, RadixThemesComponent
+from .base import LiteralTextSize, LiteralTextWeight
 
-LiteralGridFlow = Literal["row", "column", "dense", "row-dense", "column-dense"]
-
-class Grid(el.Div, RadixThemesComponent):
+class Code(el.Code, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        columns: Optional[Union[Var[str], str]] = None,
-        rows: Optional[Union[Var[str], str]] = None,
-        flow: Optional[
-            Union[
-                Var[Literal["row", "column", "dense", "row-dense", "column-dense"]],
-                Literal["row", "column", "dense", "row-dense", "column-dense"],
-            ]
-        ] = None,
-        align: Optional[
-            Union[
-                Var[Literal["start", "center", "end", "baseline", "stretch"]],
-                Literal["start", "center", "end", "baseline", "stretch"],
-            ]
-        ] = None,
-        justify: Optional[
-            Union[
-                Var[Literal["start", "center", "end", "between"]],
-                Literal["start", "center", "end", "between"],
-            ]
-        ] = None,
-        spacing: Optional[
-            Union[
-                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
-            ]
-        ] = None,
-        spacing_x: Optional[
+        variant: Optional[
             Union[
-                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
+                Var[Literal["classic", "solid", "soft", "surface", "outline", "ghost"]],
+                Literal["classic", "solid", "soft", "surface", "outline", "ghost"],
             ]
         ] = None,
-        spacing_y: Optional[
+        size: Optional[
             Union[
-                Var[Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
+                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
+                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+            ]
+        ] = None,
+        weight: Optional[
+            Union[
+                Var[Literal["light", "regular", "medium", "bold"]],
+                Literal["light", "regular", "medium", "bold"],
+            ]
+        ] = None,
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
             ]
         ] = None,
+        high_contrast: Optional[Union[Var[bool], bool]] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         content_editable: Optional[
@@ -147,31 +187,27 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Grid":
+    ) -> "Code":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            columns: Number of columns
-            rows: Number of rows
-            flow: How the grid items are layed out: "row" | "column" | "dense" | "row-dense" | "column-dense"
-            align: Alignment of children along the main axis: "start" | "center" | "end" | "baseline" | "stretch"
-            justify: Alignment of children along the cross axis: "start" | "center" | "end" | "between"
-            spacing: Gap between children: "0" - "9"
-            spacing_x: Gap between children horizontal: "0" - "9"
-            spacing_y: Gap between children vertical: "0" - "9"
+            variant: The visual variant to apply: "solid" | "soft" | "outline" | "ghost"
+            size: Text size: "1" - "9"
+            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            color_scheme: Overrides the accent color inherited from the Theme.
+            high_contrast: Whether to render the text with higher contrast color
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/layout/stack.py` & `reflex-0.4.9a1/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.py` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-"""Stub file for reflex/components/radix/themes/typography/code.py"""
+"""Stub file for reflex/components/radix/themes/typography/heading.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from reflex import el
 from reflex.vars import Var
-from ..base import LiteralAccentColor, LiteralVariant, RadixThemesComponent
-from .base import LiteralTextSize, LiteralTextWeight
+from ..base import LiteralAccentColor, RadixThemesComponent
+from .base import LiteralTextAlign, LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
-class Code(el.Code, RadixThemesComponent):
+class Heading(el.H1, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        variant: Optional[
-            Union[
-                Var[Literal["classic", "solid", "soft", "surface", "outline", "ghost"]],
-                Literal["classic", "solid", "soft", "surface", "outline", "ghost"],
-            ]
-        ] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
+        as_: Optional[Union[Var[str], str]] = None,
         size: Optional[
             Union[
                 Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
                 Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
             ]
         ] = None,
         weight: Optional[
             Union[
                 Var[Literal["light", "regular", "medium", "bold"]],
                 Literal["light", "regular", "medium", "bold"],
             ]
         ] = None,
+        align: Optional[
+            Union[
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
+            ]
+        ] = None,
+        trim: Optional[
+            Union[
+                Var[Literal["normal", "start", "end", "both"]],
+                Literal["normal", "start", "end", "both"],
+            ]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -187,25 +195,28 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Code":
+    ) -> "Heading":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            variant: The visual variant to apply: "solid" | "soft" | "outline" | "ghost"
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            as_: Change the default rendered element into a semantically appropriate alternative (cannot be used with asChild)
             size: Text size: "1" - "9"
             weight: Thickness of text: "light" | "regular" | "medium" | "bold"
+            align: Alignment of text in element: "left" | "center" | "right"
+            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
             color_scheme: Overrides the accent color inherited from the Theme.
             high_contrast: Whether to render the text with higher contrast color
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.py` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.4.9a1/reflex/components/suneditor/editor.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,177 +1,166 @@
-"""Stub file for reflex/components/radix/themes/typography/heading.py"""
+"""Stub file for reflex/components/suneditor/editor.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import el
+import enum
+from typing import Any, Dict, List, Literal, Optional, Union
+from reflex.base import Base
+from reflex.components.component import Component, NoSSRComponent
+from reflex.constants import EventTriggers
+from reflex.utils.format import to_camel_case
+from reflex.utils.imports import ImportVar
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
-from .base import LiteralTextAlign, LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
-class Heading(el.H1, RadixThemesComponent):
+class EditorButtonList(list, enum.Enum):
+    BASIC = [["font", "fontSize"], ["fontColor"], ["horizontalRule"], ["link", "image"]]
+    FORMATTING = [
+        ["undo", "redo"],
+        ["bold", "underline", "italic", "strike", "subscript", "superscript"],
+        ["removeFormat"],
+        ["outdent", "indent"],
+        ["fullScreen", "showBlocks", "codeView"],
+        ["preview", "print"],
+    ]
+    COMPLEX = [
+        ["undo", "redo"],
+        ["font", "fontSize", "formatBlock"],
+        ["bold", "underline", "italic", "strike", "subscript", "superscript"],
+        ["removeFormat"],
+        "/",
+        ["fontColor", "hiliteColor"],
+        ["outdent", "indent"],
+        ["align", "horizontalRule", "list", "table"],
+        ["link", "image", "video"],
+        ["fullScreen", "showBlocks", "codeView"],
+        ["preview", "print"],
+        ["save", "template"],
+    ]
+
+class EditorOptions(Base):
+    default_tag: Optional[str]
+    mode: Optional[str]
+    rtl: Optional[bool]
+    button_list: Optional[List[Union[List[str], str]]]
+
+class Editor(NoSSRComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
-        as_: Optional[Union[Var[str], str]] = None,
-        size: Optional[
-            Union[
-                Var[Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"]],
-                Literal["1", "2", "3", "4", "5", "6", "7", "8", "9"],
-            ]
-        ] = None,
-        weight: Optional[
-            Union[
-                Var[Literal["light", "regular", "medium", "bold"]],
-                Literal["light", "regular", "medium", "bold"],
-            ]
-        ] = None,
-        align: Optional[
-            Union[
-                Var[Literal["left", "center", "right"]],
-                Literal["left", "center", "right"],
-            ]
-        ] = None,
-        trim: Optional[
-            Union[
-                Var[Literal["normal", "start", "end", "both"]],
-                Literal["normal", "start", "end", "both"],
-            ]
-        ] = None,
-        color_scheme: Optional[
+        lang: Optional[
             Union[
                 Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
+                    Union[
+                        Literal[
+                            "en",
+                            "da",
+                            "de",
+                            "es",
+                            "fr",
+                            "ja",
+                            "ko",
+                            "pt_br",
+                            "ru",
+                            "zh_cn",
+                            "ro",
+                            "pl",
+                            "ckb",
+                            "lv",
+                            "se",
+                            "ua",
+                            "he",
+                            "it",
+                        ],
+                        dict,
                     ]
                 ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
+                Union[
+                    Literal[
+                        "en",
+                        "da",
+                        "de",
+                        "es",
+                        "fr",
+                        "ja",
+                        "ko",
+                        "pt_br",
+                        "ru",
+                        "zh_cn",
+                        "ro",
+                        "pl",
+                        "ckb",
+                        "lv",
+                        "se",
+                        "ua",
+                        "he",
+                        "it",
+                    ],
+                    dict,
                 ],
             ]
         ] = None,
-        high_contrast: Optional[Union[Var[bool], bool]] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        width: Optional[Union[Var[str], str]] = None,
+        height: Optional[Union[Var[str], str]] = None,
+        placeholder: Optional[Union[Var[str], str]] = None,
+        auto_focus: Optional[Union[Var[bool], bool]] = None,
+        set_options: Optional[Union[Var[Dict], Dict]] = None,
+        set_all_plugins: Optional[Union[Var[bool], bool]] = None,
+        set_contents: Optional[Union[Var[str], str]] = None,
+        append_contents: Optional[Union[Var[str], str]] = None,
+        set_default_style: Optional[Union[Var[str], str]] = None,
+        disable: Optional[Union[Var[bool], bool]] = None,
+        hide: Optional[Union[Var[bool], bool]] = None,
+        hide_toolbar: Optional[Union[Var[bool], bool]] = None,
+        disable_toolbar: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_copy: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_cut: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_input: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_load: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -188,58 +177,62 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_paste: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_resize_editor: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        toggle_code_view: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        toggle_full_screen: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "Heading":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Editor":
+        """Create an instance of Editor. No children allowed.
 
         Args:
-            *children: Child components.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            as_: Change the default rendered element into a semantically appropriate alternative (cannot be used with asChild)
-            size: Text size: "1" - "9"
-            weight: Thickness of text: "light" | "regular" | "medium" | "bold"
-            align: Alignment of text in element: "left" | "center" | "right"
-            trim: Removes the leading trim space: "normal" | "start" | "end" | "both"
-            color_scheme: Overrides the accent color inherited from the Theme.
-            high_contrast: Whether to render the text with higher contrast color
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            set_options(Optional[EditorOptions]): Configuration object to further configure the instance.
+            lang: Language of the editor.  Alternatively to a string, a dict of your language can be passed to this prop.  Please refer to the library docs for this.  options: "en" | "da" | "de" | "es" | "fr" | "ja" | "ko" | "pt_br" |   "ru" | "zh_cn" | "ro" | "pl" | "ckb" | "lv" | "se" | "ua" | "he" | "it"  default : "en"
+            name: This is used to set the HTML form name of the editor.  This means on HTML form submission,  it will be submitted together with contents of the editor by the name provided.
+            default_value: Sets the default value of the editor.  This is useful if you don't want the on_change method to be called on render.  If you want the on_change method to be called on render please use the set_contents prop
+            width: Sets the width of the editor.  px and percentage values are accepted, eg width="100%" or width="500px"  default: 100%
+            height: Sets the height of the editor.  px and percentage values are accepted, eg height="100%" or height="100px"
+            placeholder: Sets the placeholder of the editor.
+            auto_focus: Should the editor receive focus when initialized?
+            set_options: Pass an EditorOptions instance to modify the behaviour of Editor even more.
+            set_all_plugins: Whether all SunEditor plugins should be loaded.  default: True
+            set_contents: Set the content of the editor.  Note: To set the initial contents of the editor  without calling the on_change event,  please use the default_value prop.  set_contents is used to set the contents of the editor programmatically.  You must be aware that, when the set_contents's prop changes,  the on_change event is triggered.
+            append_contents: Append editor content
+            set_default_style: Sets the default style of the editor's edit area
+            disable: Disable the editor  default: False
+            hide: Hide the editor  default: False
+            hide_toolbar: Hide the editor toolbar  default: False
+            disable_toolbar: Disable the editor toolbar  default: False
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: Any properties to be passed to the Editor
 
         Returns:
-            A new component instance.
+            An Editor instance.
+
+        Raises:
+            ValueError: If set_options is a state Var.
         """
         ...
```

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/link.py` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/radix/themes/typography/text.py` & `reflex-0.4.9a1/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/react_player/audio.pyi` & `reflex-0.4.9a1/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/react_player/react_player.py` & `reflex-0.4.9a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/react_player/react_player.pyi` & `reflex-0.4.9a1/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/react_player/video.pyi` & `reflex-0.4.9a1/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/__init__.py` & `reflex-0.4.9a1/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/cartesian.py` & `reflex-0.4.9a1/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/charts.py` & `reflex-0.4.9a1/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/charts.pyi` & `reflex-0.4.9a1/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/general.py` & `reflex-0.4.9a1/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/polar.py` & `reflex-0.4.9a1/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/recharts/recharts.py` & `reflex-0.4.9a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/suneditor/editor.py` & `reflex-0.4.9a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/tags/iter_tag.py` & `reflex-0.4.9a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/tags/tag.py` & `reflex-0.4.9a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/components/tags/tagless.py` & `reflex-0.4.9a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/config.py` & `reflex-0.4.9a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/config.pyi` & `reflex-0.4.9a1/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/__init__.py` & `reflex-0.4.9a1/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/base.py` & `reflex-0.4.9a1/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/base.pyi` & `reflex-0.4.9a1/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/colors.py` & `reflex-0.4.9a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/compiler.py` & `reflex-0.4.9a1/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/config.py` & `reflex-0.4.9a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/custom_components.py` & `reflex-0.4.9a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/event.py` & `reflex-0.4.9a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/installer.py` & `reflex-0.4.9a1/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/route.py` & `reflex-0.4.9a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/constants/style.py` & `reflex-0.4.9a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/custom_components/custom_components.py` & `reflex-0.4.9a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/event.py` & `reflex-0.4.9a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/experimental/hooks.py` & `reflex-0.4.9a1/reflex/experimental/hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,30 @@
     if v is None:
         return
 
     if isinstance(tags, str):
         tags = [tags]
 
     v._var_data = VarData(  # type: ignore
-        imports={"react": [ImportVar(tag=tag) for tag in tags]},
+        imports={"react": [ImportVar(tag=tag, install=False) for tag in tags]},
     )
 
 
 def const(name, value) -> Var | None:
     """Create a constant Var.
 
     Args:
         name: The name of the constant.
         value: The value of the constant.
 
     Returns:
         The constant Var.
     """
+    if isinstance(name, list):
+        return Var.create(f"const [{', '.join(name)}] = {value}")
     return Var.create(f"const {name} = {value}")
 
 
 def useCallback(func, deps) -> Var | None:
     """Create a useCallback hook with a function and dependencies.
 
     Args:
@@ -69,7 +71,23 @@
 
     Returns:
         The useRef hook.
     """
     v = Var.create(f"useRef({default})")
     _add_react_import(v, "useRef")
     return v
+
+
+def useState(var_name, default=None) -> Var | None:
+    """Create a useState hook with a variable name and setter name.
+
+    Args:
+        var_name: The name of the variable.
+        default: The default value of the variable.
+
+    Returns:
+        A useState hook.
+    """
+    setter_name = f"set{var_name.capitalize()}"
+    v = const([var_name, setter_name], f"useState({default})")
+    _add_react_import(v, "useState")
+    return v
```

### Comparing `reflex-0.4.8a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.4.9a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/middleware/middleware.py` & `reflex-0.4.9a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/model.py` & `reflex-0.4.9a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/page.py` & `reflex-0.4.9a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/reflex.py` & `reflex-0.4.9a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/route.py` & `reflex-0.4.9a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/state.py` & `reflex-0.4.9a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/style.py` & `reflex-0.4.9a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/testing.py` & `reflex-0.4.9a1/reflex/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,26 +108,29 @@
 
 
 @dataclasses.dataclass
 class AppHarness:
     """AppHarness executes a reflex app in-process for testing."""
 
     app_name: str
-    app_source: Optional[types.FunctionType | types.ModuleType] | str
+    app_source: Optional[
+        types.FunctionType | types.ModuleType | str | functools.partial
+    ]
     app_path: pathlib.Path
     app_module_path: pathlib.Path
     app_module: Optional[types.ModuleType] = None
     app_instance: Optional[reflex.App] = None
     frontend_process: Optional[subprocess.Popen] = None
     frontend_url: Optional[str] = None
     frontend_output_thread: Optional[threading.Thread] = None
     backend_thread: Optional[threading.Thread] = None
     backend: Optional[uvicorn.Server] = None
     state_manager: Optional[StateManagerMemory | StateManagerRedis] = None
     _frontends: list["WebDriver"] = dataclasses.field(default_factory=list)
+    _decorated_pages: list = dataclasses.field(default_factory=list)
 
     @classmethod
     def create(
         cls,
         root: pathlib.Path,
         app_source: Optional[types.FunctionType | types.ModuleType | str] = None,
         app_name: Optional[str] = None,
@@ -145,23 +148,29 @@
             ValueError: when app_source is a string and app_name is not provided.
 
         Returns:
             AppHarness instance
         """
         if app_name is None:
             if app_source is None:
-                app_name = root.name.lower()
+                app_name = root.name
             elif isinstance(app_source, functools.partial):
-                app_name = app_source.func.__name__.lower()
+                keywords = app_source.keywords
+                slug_suffix = "_".join([str(v) for v in keywords.values()])
+                func_name = app_source.func.__name__
+                app_name = f"{func_name}_{slug_suffix}"
+                app_name = re.sub(r"[^a-zA-Z0-9_]", "_", app_name)
             elif isinstance(app_source, str):
                 raise ValueError(
                     "app_name must be provided when app_source is a string."
                 )
             else:
-                app_name = app_source.__name__.lower()
+                app_name = app_source.__name__
+
+            app_name = app_name.lower()
         return cls(
             app_name=app_name,
             app_source=app_source,
             app_path=root,
             app_module_path=root / app_name / f"{app_name}.py",
         )
 
@@ -226,19 +235,23 @@
                     template=reflex.constants.Templates.DEFAULT,
                     loglevel=reflex.constants.LogLevel.INFO,
                 )
                 self.app_module_path.write_text(source_code)
         with chdir(self.app_path):
             # ensure config and app are reloaded when testing different app
             reflex.config.get_config(reload=True)
-            # Clean out any `rx.page` decorators from other tests.
-            reflex.app.DECORATED_PAGES.clear()
+            # Save decorated pages before importing the test app module
+            before_decorated_pages = reflex.app.DECORATED_PAGES.copy()
             # Ensure the AppHarness test does not skip State assignment due to running via pytest
             os.environ.pop(reflex.constants.PYTEST_CURRENT_TEST, None)
             self.app_module = reflex.utils.prerequisites.get_compiled_app(reload=True)
+            # Save the pages that were added during testing
+            self._decorated_pages = [
+                p for p in reflex.app.DECORATED_PAGES if p not in before_decorated_pages
+            ]
         self.app_instance = self.app_module.app
         if isinstance(self.app_instance._state_manager, StateManagerRedis):
             # Create our own redis connection for testing.
             self.state_manager = StateManagerRedis.create(self.app_instance.state)
         else:
             self.state_manager = self.app_instance._state_manager
 
@@ -392,14 +405,18 @@
         if self.backend_thread is not None:
             self.backend_thread.join()
         if self.frontend_output_thread is not None:
             self.frontend_output_thread.join()
         for driver in self._frontends:
             driver.quit()
 
+        # Cleanup decorated pages added during testing
+        for page in self._decorated_pages:
+            reflex.app.DECORATED_PAGES.remove(page)
+
     def __exit__(self, *excinfo) -> None:
         """Contextmanager protocol for `stop()`.
 
         Args:
             excinfo: sys.exc_info captured in the context block
         """
         self.stop()
```

### Comparing `reflex-0.4.8a1/reflex/utils/build.py` & `reflex-0.4.9a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/compat.py` & `reflex-0.4.9a1/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/console.py` & `reflex-0.4.9a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/exec.py` & `reflex-0.4.9a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/export.py` & `reflex-0.4.9a1/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/format.py` & `reflex-0.4.9a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/imports.py` & `reflex-0.4.9a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/path_ops.py` & `reflex-0.4.9a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/prerequisites.py` & `reflex-0.4.9a1/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,23 +564,25 @@
 def update_next_config(export=False, transpile_packages: Optional[List[str]] = None):
     """Update Next.js config from Reflex config.
 
     Args:
         export: if the method run during reflex export.
         transpile_packages: list of packages to transpile via next.config.js.
     """
-    next_config_file = os.path.join(constants.Dirs.WEB, constants.Next.CONFIG_FILE)
+    next_config_file = Path(constants.Dirs.WEB, constants.Next.CONFIG_FILE)
 
     next_config = _update_next_config(
         get_config(), export=export, transpile_packages=transpile_packages
     )
 
-    with open(next_config_file, "w") as file:
-        file.write(next_config)
-        file.write("\n")
+    # Overwriting the next.config.js triggers a full server reload, so make sure
+    # there is actually a diff.
+    orig_next_config = next_config_file.read_text() if next_config_file.exists() else ""
+    if orig_next_config != next_config:
+        next_config_file.write_text(next_config)
 
 
 def _update_next_config(
     config: Config, export: bool = False, transpile_packages: Optional[List[str]] = None
 ):
     next_config = {
         "basePath": config.frontend_path or "",
@@ -815,22 +817,24 @@
     Args:
         packages: A list of package names to be installed.
         config: The config object.
 
     Example:
         >>> install_frontend_packages(["react", "react-dom"], get_config())
     """
-    # unsupported archs will use npm anyway. so we dont have to run npm twice
+    # unsupported archs(arm and 32bit machines) will use npm anyway. so we dont have to run npm twice
     fallback_command = (
-        get_package_manager()
-        if constants.IS_WINDOWS and constants.IS_WINDOWS_BUN_SUPPORTED_MACHINE
+        get_install_package_manager()
+        if not constants.IS_WINDOWS
+        or constants.IS_WINDOWS
+        and constants.IS_WINDOWS_BUN_SUPPORTED_MACHINE
         else None
     )
     processes.run_process_with_fallback(
-        [get_install_package_manager(), "install", "--loglevel", "silly"],
+        [get_install_package_manager(), "install"],  # type: ignore
         fallback=fallback_command,
         show_status_message="Installing base frontend packages",
         cwd=constants.Dirs.WEB,
         shell=constants.IS_WINDOWS,
     )
 
     if config.tailwind is not None:
```

### Comparing `reflex-0.4.8a1/reflex/utils/processes.py` & `reflex-0.4.9a1/reflex/utils/processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import collections
 import contextlib
 import os
 import signal
 import subprocess
 from concurrent import futures
+from pathlib import Path
 from typing import Callable, Generator, List, Optional, Tuple, Union
 
 import psutil
 import typer
 from redis.exceptions import RedisError
 
 from reflex import constants
@@ -141,14 +142,15 @@
     }
     kwargs = {
         "env": env,
         "stderr": None if show_logs else subprocess.STDOUT,
         "stdout": None if show_logs else subprocess.PIPE,
         "universal_newlines": True,
         "encoding": "UTF-8",
+        "errors": "replace",  # Avoid UnicodeDecodeError in unknown command output
         **kwargs,
     }
     console.debug(f"Running command: {args}")
     fn = subprocess.run if run else subprocess.Popen
     return fn(args, **kwargs)
 
 
@@ -198,21 +200,27 @@
     Args:
         *fns: The functions to run.
     """
     with run_concurrently_context(*fns):
         pass
 
 
-def stream_logs(message: str, process: subprocess.Popen, progress=None):
+def stream_logs(
+    message: str,
+    process: subprocess.Popen,
+    progress=None,
+    suppress_errors: bool = False,
+):
     """Stream the logs for a process.
 
     Args:
         message: The message to display.
         process: The process.
         progress: The ongoing progress bar if one is being used.
+        suppress_errors: If True, do not exit if errors are encountered (for fallback).
 
     Yields:
         The lines of the process output.
 
     Raises:
         Exit: If the process failed.
     """
@@ -228,15 +236,15 @@
             yield line
 
     # Check if the process failed (not printing the logs for SIGINT).
 
     # Windows uvicorn bug
     # https://github.com/reflex-dev/reflex/issues/2335
     accepted_return_codes = [0, -2, 15] if constants.IS_WINDOWS else [0, -2]
-    if process.returncode not in accepted_return_codes:
+    if process.returncode not in accepted_return_codes and not suppress_errors:
         console.error(f"{message} failed with exit code {process.returncode}")
         for line in logs:
             console.error(line, end="")
         console.error("Run with [bold]--loglevel debug [/bold] for the full log.")
         raise typer.Exit(1)
 
 
@@ -247,23 +255,24 @@
         message: The message to display.
         process: The process.
     """
     for _ in stream_logs(message, process):
         pass
 
 
-def show_status(message: str, process: subprocess.Popen):
+def show_status(message: str, process: subprocess.Popen, suppress_errors: bool = False):
     """Show the status of a process.
 
     Args:
         message: The initial message to display.
         process: The process.
+        suppress_errors: If True, do not exit if errors are encountered (for fallback).
     """
     with console.status(message) as status:
-        for line in stream_logs(message, process):
+        for line in stream_logs(message, process, suppress_errors=suppress_errors):
             status.update(f"{message} {line}")
 
 
 def show_progress(message: str, process: subprocess.Popen, checkpoints: List[str]):
     """Show a progress bar for a process.
 
     Args:
@@ -285,42 +294,54 @@
 
 
 def atexit_handler():
     """Display a custom message with the current time when exiting an app."""
     console.log("Reflex app stopped.")
 
 
+def get_command_with_loglevel(command: list[str]) -> list[str]:
+    """Add the right loglevel flag to the designated command.
+     npm uses --loglevel <level>, Bun doesnt use the --loglevel flag and
+     runs in debug mode by default.
+
+    Args:
+        command:The command to add loglevel flag.
+
+    Returns:
+        The updated command list
+    """
+    npm_path = path_ops.get_npm_path()
+    npm_path = str(Path(npm_path).resolve()) if npm_path else npm_path
+
+    if command[0] == npm_path:
+        return command + ["--loglevel", "silly"]
+    return command
+
+
 def run_process_with_fallback(args, *, show_status_message, fallback=None, **kwargs):
     """Run subprocess and retry using fallback command if initial command fails.
 
     Args:
         args: A string, or a sequence of program arguments.
         show_status_message: The status message to be displayed in the console.
         fallback: The fallback command to run.
         kwargs: Kwargs to pass to new_process function.
     """
-
-    def execute_process(process):
-        if not constants.IS_WINDOWS:
-            show_status(show_status_message, process)
-        else:
-            process.wait()
-            if process.returncode != 0:
-                error_output = process.stderr if process.stderr else process.stdout
-                error_message = f"Error occurred during subprocess execution: {' '.join(args)}\n{error_output.read() if error_output else ''}"
-                # Only show error in debug mode.
-                if console.is_debug():
-                    console.error(error_message)
-
-                # retry with fallback command.
-                fallback_args = [fallback, *args[1:]] if fallback else None
-                console.warn(
-                    f"There was an error running command: {args}. Falling back to: {fallback_args}."
-                )
-                if fallback_args:
-                    process = new_process(fallback_args, **kwargs)
-                    execute_process(process)
-            else:
-                show_status(show_status_message, process)
-
-    process = new_process(args, **kwargs)
-    execute_process(process)
+    process = new_process(get_command_with_loglevel(args), **kwargs)
+    if fallback is None:
+        # No fallback given, or this _is_ the fallback command.
+        show_status(show_status_message, process)
+    else:
+        # Suppress errors for initial command, because we will try to fallback
+        show_status(show_status_message, process, suppress_errors=True)
+        if process.returncode != 0:
+            # retry with fallback command.
+            fallback_args = [fallback, *args[1:]]
+            console.warn(
+                f"There was an error running command: {args}. Falling back to: {fallback_args}."
+            )
+            run_process_with_fallback(
+                fallback_args,
+                show_status_message=show_status_message,
+                fallback=None,
+                **kwargs,
+            )
```

### Comparing `reflex-0.4.8a1/reflex/utils/pyi_generator.py` & `reflex-0.4.9a1/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/serializers.py` & `reflex-0.4.9a1/reflex/utils/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import json
 import types as builtin_types
 import warnings
 from datetime import date, datetime, time, timedelta
 from enum import Enum
+from pathlib import Path
 from typing import Any, Callable, Dict, List, Set, Tuple, Type, Union, get_type_hints
 
 from reflex.base import Base
 from reflex.constants.colors import Color, format_color
 from reflex.utils import exceptions, format, types
 
 # Mapping from type to a serializer.
@@ -230,14 +231,27 @@
     Returns:
         The serialized datetime.
     """
     return str(dt)
 
 
 @serializer
+def serialize_path(path: Path):
+    """Serialize a pathlib.Path to a JSON string.
+
+    Args:
+        path: The path to serialize.
+
+    Returns:
+        The serialized path.
+    """
+    return str(path.as_posix())
+
+
+@serializer
 def serialize_enum(en: Enum) -> str:
     """Serialize a enum to a JSON string.
 
     Args:
         en: The enum to serialize.
 
     Returns:
```

### Comparing `reflex-0.4.8a1/reflex/utils/telemetry.py` & `reflex-0.4.9a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/types.py` & `reflex-0.4.9a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/utils/watch.py` & `reflex-0.4.9a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/reflex/vars.py` & `reflex-0.4.9a1/reflex/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1336,15 +1336,15 @@
 
         Raises:
             TypeError: If the var is not a valid type: dict, list, tuple or str.
 
         Returns:
             A var representing the contain check.
         """
-        if not (types._issubclass(self._var_type, Union[dict, list, tuple, str])):
+        if not (types._issubclass(self._var_type, Union[dict, list, tuple, str, set])):
             raise TypeError(
                 f"Var {self._var_full_name} of type {self._var_type} does not support contains check."
             )
         method = (
             "hasOwnProperty"
             if types.get_base_class(self._var_type) == dict
             else "includes"
```

### Comparing `reflex-0.4.8a1/reflex/vars.pyi` & `reflex-0.4.9a1/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.4.8a1/PKG-INFO` & `reflex-0.4.9a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.4.8a1
+Version: 0.4.9a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

