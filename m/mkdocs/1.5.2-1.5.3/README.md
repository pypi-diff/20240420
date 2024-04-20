# Comparing `tmp/mkdocs-1.5.2.tar.gz` & `tmp/mkdocs-1.5.3.tar.gz`

## Comparing `mkdocs-1.5.2.tar` & `mkdocs-1.5.3.tar`

### file list

```diff
@@ -1,236 +1,248 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/__init__.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/__main__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/exceptions.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/localization.py
--rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/py.typed
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/theme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/__init__.py
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/build.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/get_deps.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/gh_deploy.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/new.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/commands/serve.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/__init__.py
--rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/base.py
--rw-r--r--   0        0        0    43938 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/config_options.py
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/config/defaults.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/prebuild-index.js
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/search_index.py
--rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ar.js
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.da.js
--rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.de.js
--rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.du.js
--rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.es.js
--rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fi.js
--rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fr.js
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.hu.js
--rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.it.js
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ja.js
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.jp.js
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.multi.js
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.nl.js
--rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.no.js
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.pt.js
--rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ro.js
--rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ru.js
--rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.sv.js
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.th.js
--rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.tr.js
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.vi.js
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/tinyseg.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/main.js
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/contrib/search/templates/search/worker.js
--rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/livereload/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/__init__.py
--rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/files.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/nav.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/pages.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/structure/toc.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/templates/sitemap.xml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/__init__.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/base.py
--rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/build_tests.py
--rw-r--r--   0        0        0    25007 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/cli_tests.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/get_deps_tests.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/gh_deploy_tests.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration.py
--rw-r--r--   0        0        0    25502 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/livereload_tests.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/localization_tests.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/new_tests.py
--rw-r--r--   0        0        0    10915 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/plugin_tests.py
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/search_tests.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/theme_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/__init__.py
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/base_tests.py
--rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_options_legacy_tests.py
--rw-r--r--   0        0        0    82667 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_options_tests.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/config/config_tests.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/projects.yaml
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/mkdocs.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/custom.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/tweak.css
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/documentation/tweak.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/minimal/mkdocs.yml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/minimal/docs/testing.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/mkdocs.yml
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/image.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/index.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/metadata.md
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/non-index.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/page-title.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/pageTitle.md
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/image.png
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/index.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub2/index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/mkdocs.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/index.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/Übersicht.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/integration/unicode/docs/♪.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/__init__.py
--rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/file_tests.py
--rw-r--r--   0        0        0    19090 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/nav_tests.py
--rw-r--r--   0        0        0    52573 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/page_tests.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/structure/toc_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/__init__.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/babel_stub_tests.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/templates_tests.py
--rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/tests/utils/utils_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/babel.cfg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/__init__.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/base.html
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/content.html
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/keyboard-modal.html
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/main.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/messages.pot
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/mkdocs_theme.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/nav-sub.html
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/search-modal.html
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/toc.html
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/base.css
--rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/css/font-awesome.min.css
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/img/favicon.ico
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/img/grid.png
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/base.js
--rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/bootstrap.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/base.html
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/breadcrumbs.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/footer.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/main.html
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/messages.pot
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/mkdocs_theme.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/nav.html
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/search.html
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/searchbox.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/toc.html
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/versions.html
--rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme_extra.js
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/babel_stub.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/cache.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/filters.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/meta.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/templates.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.2/mkdocs/utils/yaml.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.2/.gitignore
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.2/LICENSE
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.2/README.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.2/hatch_build.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 mkdocs-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/__main__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/exceptions.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/localization.py
+-rw-r--r--   0        0        0    22701 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/py.typed
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/theme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/__init__.py
+-rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/build.py
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/get_deps.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/gh_deploy.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/new.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/commands/serve.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/config/__init__.py
+-rw-r--r--   0        0        0    13151 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/config/base.py
+-rw-r--r--   0        0        0    44043 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/config/config_options.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/config/defaults.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/__init__.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/prebuild-index.js
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/search_index.py
+-rw-r--r--   0        0        0    24542 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ar.js
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.da.js
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.de.js
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.du.js
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.es.js
+-rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.fi.js
+-rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.fr.js
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.hi.js
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.hu.js
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.hy.js
+-rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.it.js
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ja.js
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.jp.js
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.kn.js
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ko.js
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.multi.js
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.nl.js
+-rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.no.js
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.pt.js
+-rw-r--r--   0        0        0    23157 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ro.js
+-rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ru.js
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.sa.js
+-rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.sv.js
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ta.js
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.te.js
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.th.js
+-rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.tr.js
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.vi.js
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.zh.js
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/tinyseg.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/templates/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/templates/search/main.js
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/contrib/search/templates/search/worker.js
+-rw-r--r--   0        0        0    13160 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/livereload/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/structure/__init__.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/structure/files.py
+-rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/structure/nav.py
+-rw-r--r--   0        0        0    17713 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/structure/pages.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/structure/toc.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/templates/sitemap.xml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/__init__.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/base.py
+-rw-r--r--   0        0        0    34742 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/build_tests.py
+-rw-r--r--   0        0        0    25007 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/cli_tests.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/get_deps_tests.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/gh_deploy_tests.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration.py
+-rw-r--r--   0        0        0    25504 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/livereload_tests.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/localization_tests.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/new_tests.py
+-rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/plugin_tests.py
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/search_tests.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/theme_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/config/__init__.py
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/config/base_tests.py
+-rw-r--r--   0        0        0    55357 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/config/config_options_legacy_tests.py
+-rw-r--r--   0        0        0    82736 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/config/config_options_tests.py
+-rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/config/config_tests.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/projects.yaml
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/mkdocs.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/documentation/custom.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/documentation/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/documentation/tweak.css
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/documentation/tweak.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/minimal/mkdocs.yml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/minimal/docs/testing.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/mkdocs.yml
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/image.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/index.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/metadata.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/non-index.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/page-title.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/pageTitle.md
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/image.png
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/index.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub2/index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/unicode/mkdocs.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/unicode/docs/index.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/unicode/docs/Übersicht.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/integration/unicode/docs/♪.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/structure/__init__.py
+-rw-r--r--   0        0        0    34212 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/structure/file_tests.py
+-rw-r--r--   0        0        0    20096 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/structure/nav_tests.py
+-rw-r--r--   0        0        0    52585 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/structure/page_tests.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/structure/toc_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/utils/babel_stub_tests.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/utils/templates_tests.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/tests/utils/utils_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/babel.cfg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/__init__.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/base.html
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/content.html
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/keyboard-modal.html
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/main.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/messages.pot
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/nav-sub.html
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/search-modal.html
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/toc.html
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/css/base.css
+-rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/css/font-awesome.min.css
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/img/favicon.ico
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/img/grid.png
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/js/base.js
+-rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/js/bootstrap.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/base.html
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/breadcrumbs.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/footer.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/main.html
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/messages.pot
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/nav.html
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/search.html
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/searchbox.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/toc.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/versions.html
+-rw-r--r--   0        0        0   135539 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/js/theme_extra.js
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    13376 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/babel_stub.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/cache.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/filters.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/meta.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/templates.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 mkdocs-1.5.3/mkdocs/utils/yaml.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.5.3/LICENSE
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 mkdocs-1.5.3/README.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.5.3/hatch_build.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 mkdocs-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mkdocs-1.5.3/PKG-INFO
```

### Comparing `mkdocs-1.5.2/mkdocs/__main__.py` & `mkdocs-1.5.3/mkdocs/__main__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/exceptions.py` & `mkdocs-1.5.3/mkdocs/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/localization.py` & `mkdocs-1.5.3/mkdocs/localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import logging
 import os
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
-import jinja2
 from jinja2.ext import Extension, InternationalizationExtension
 
 from mkdocs.config.base import ValidationError
 
+if TYPE_CHECKING:
+    import jinja2
+
 try:
     from babel.core import Locale, UnknownLocaleError
     from babel.support import NullTranslations, Translations
 
     has_babel = True
 except ImportError:  # pragma: no cover
     from mkdocs.utils.babel_stub import Locale, UnknownLocaleError
@@ -33,15 +35,15 @@
         )
 
 
 def parse_locale(locale: str) -> Locale:
     try:
         return Locale.parse(locale, sep='_')
     except (ValueError, UnknownLocaleError, TypeError) as e:
-        raise ValidationError(f'Invalid value for locale: {str(e)}')
+        raise ValidationError(f'Invalid value for locale: {e}')
 
 
 def install_translations(
     env: jinja2.Environment, locale: Locale, theme_dirs: Sequence[str]
 ) -> None:
     if has_babel:
         env.add_extension('jinja2.ext.i18n')
```

### Comparing `mkdocs-1.5.2/mkdocs/plugins.py` & `mkdocs-1.5.3/mkdocs/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import EntryPoint, entry_points
 else:
     from importlib_metadata import EntryPoint, entry_points
 
 if TYPE_CHECKING:
+    import jinja2.environment
+
     if sys.version_info >= (3, 8):
         from typing import Literal
     else:
         from typing_extensions import Literal
 
-import jinja2.environment
-
 from mkdocs import utils
 from mkdocs.config.base import Config, ConfigErrors, ConfigWarnings, LegacyConfig, PlainConfigSchema
 
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.livereload import LiveReloadServer
     from mkdocs.structure.files import Files
```

### Comparing `mkdocs-1.5.2/mkdocs/theme.py` & `mkdocs-1.5.3/mkdocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/commands/build.py` & `mkdocs-1.5.3/mkdocs/commands/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import mkdocs
 from mkdocs import utils
 from mkdocs.exceptions import Abort, BuildError
 from mkdocs.structure.files import File, Files, InclusionLevel, _set_exclusions, get_files
 from mkdocs.structure.nav import Navigation, get_navigation
 from mkdocs.structure.pages import Page
-from mkdocs.utils import DuplicateFilter  # noqa - legacy re-export
+from mkdocs.utils import DuplicateFilter  # noqa: F401 - legacy re-export
 from mkdocs.utils import templates
 
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
 
 if TYPE_CHECKING:
     from mkdocs.livereload import LiveReloadServer
@@ -371,8 +371,8 @@
     finally:
         logger.removeHandler(warning_counter)
 
 
 def site_directory_contains_stale_files(site_directory: str) -> bool:
     """Check if the site directory contains stale files from a previous build."""
 
-    return True if os.path.exists(site_directory) and os.listdir(site_directory) else False
+    return bool(os.path.exists(site_directory) and os.listdir(site_directory))
```

### Comparing `mkdocs-1.5.2/mkdocs/commands/get_deps.py` & `mkdocs-1.5.3/mkdocs/commands/get_deps.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,8 @@
                     if dist_name:
                         warning += f" from '{dist_name}'"
                     log.info(warning)
                 else:
                     log.warning(warning)
 
     for pkg in sorted(packages_to_install):
-        print(pkg)
+        print(pkg)  # noqa: T201
```

### Comparing `mkdocs-1.5.2/mkdocs/commands/gh_deploy.py` & `mkdocs-1.5.3/mkdocs/commands/gh_deploy.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/commands/new.py` & `mkdocs-1.5.3/mkdocs/commands/new.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/commands/serve.py` & `mkdocs-1.5.3/mkdocs/commands/serve.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/config/base.py` & `mkdocs-1.5.3/mkdocs/config/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/config/config_options.py` & `mkdocs-1.5.3/mkdocs/config/config_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def __repr__(self) -> str:
         return f"{type(self).__name__}: {self.option_type}"
 
     def pre_validation(self, config: Config, key_name: str):
         self._config = config
         self._key_name = key_name
 
-    def run_validation(self, value: object) -> Dict[str, T]:
+    def run_validation(self, value: object) -> dict[str, T]:
         if value is None:
             if self.required or self.default is None:
                 raise ValidationError("Required configuration not provided.")
             value = self.default
         if not isinstance(value, dict):
             raise ValidationError(f"Expected a dict of items, but a {type(value)} was given.")
         if not value:  # Optimization for empty list
@@ -1088,15 +1088,17 @@
         if '/' in name:  # It's already specified with a namespace.
             # Special case: allow to explicitly skip namespaced loading:
             if name.startswith('/'):
                 name = name[1:]
         else:
             # Attempt to load with prepended namespace for the current theme.
             if self.theme_key and self._config:
-                current_theme = self._config[self.theme_key]['name']
+                current_theme = self._config[self.theme_key]
+                if not isinstance(current_theme, str):
+                    current_theme = current_theme['name']
                 if current_theme:
                     expanded_name = f'{current_theme}/{name}'
                     if expanded_name in self.installed_plugins:
                         name = expanded_name
         return (name, self.load_plugin(name, config))
 
     def load_plugin(self, name: str, config) -> plugins.BasePlugin:
```

### Comparing `mkdocs-1.5.2/mkdocs/config/defaults.py` & `mkdocs-1.5.3/mkdocs/config/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-from typing import IO, Dict
+from typing import IO, TYPE_CHECKING, Dict
 
-import mkdocs.structure.pages
 from mkdocs.config import base
 from mkdocs.config import config_options as c
 from mkdocs.utils.yaml import get_yaml_loader, yaml_load
 
+if TYPE_CHECKING:
+    import mkdocs.structure.pages
+
 
 # NOTE: The order here is important. During validation some config options
 # depend on others. So, if config option A depends on B, then A should be
 # listed higher in the schema.
 class MkDocsConfig(base.Config):
     """The configuration of MkDocs itself (the root object of mkdocs.yml)."""
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/__init__.py` & `mkdocs-1.5.3/mkdocs/contrib/search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 return lang_part
 
     def run_validation(self, value: object):
         if isinstance(value, str):
             value = [value]
         if not isinstance(value, list):
             raise c.ValidationError('Expected a list of language codes.')
-        for lang in list(value):
+        for lang in value[:]:
             if lang != 'en':
                 lang_detected = self.get_lunr_supported_lang(lang)
                 if not lang_detected:
                     log.info(f"Option search.lang '{lang}' is not supported, falling back to 'en'")
                     value.remove(lang)
                     if 'en' not in value:
                         value.append('en')
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/prebuild-index.js` & `mkdocs-1.5.3/mkdocs/contrib/search/prebuild-index.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/search_index.py` & `mkdocs-1.5.3/mkdocs/contrib/search/search_index.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ar.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ar.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -139,15 +139,15 @@
 
             /*remove elongating character and test that the word does not contain non-arabic characters.
             If the word contains special characters, don't stem. */
             self.cleanWord = function() {
                 var wordCharacters = "\u0621-\u065b\u0671\u0640";
                 var testRegex = new RegExp("[^" + wordCharacters + "]");
                 self.word = self.word
-                    .replace('\u0640', '');
+                    .replace(new RegExp('\u0640', 'g'), '');
                 if (testRegex.test(word)) {
                     return true;
                 }
                 return false;
             }
 
             self.removeDiacritics = function() {
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.da.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.da.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.de.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.de.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.du.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.du.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.es.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.es.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fi.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.fr.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.hu.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.it.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ja.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.multi.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.nl.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.no.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.no.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.pt.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ro.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ro.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (1588)*

 * *Files 0% similar despite different names*

```diff
@@ -1220,228 +1220,229 @@
 00004c30: 323b 0a20 2020 2020 2020 2020 2020 2020  2;.             
 00004c40: 2020 2020 2020 2020 2069 6620 2821 7362           if (!sb
 00004c50: 702e 6571 5f73 5f62 2831 2c20 2275 2229  p.eq_s_b(1, "u")
 00004c60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 00004c70: 2020 2020 2020 2020 2020 6272 6561 6b3b            break;
 00004c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004c90: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00004ca0: 2020 2020 2020 2020 2063 6173 6520 323a           case 2:
-00004cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cc0: 2020 2020 2073 6270 2e73 6c69 6365 5f64       sbp.slice_d
-00004cd0: 656c 2829 3b0a 2020 2020 2020 2020 2020  el();.          
-00004ce0: 2020 2020 2020 2020 2020 6272 6561 6b3b            break;
-00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00004d10: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00004d20: 2073 6270 2e6c 696d 6974 5f62 6163 6b77   sbp.limit_backw
-00004d30: 6172 6420 3d20 765f 313b 0a20 2020 2020  ard = v_1;.     
-00004d40: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00004d50: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00004d60: 6675 6e63 7469 6f6e 2072 5f76 6f77 656c  function r_vowel
-00004d70: 5f73 7566 6669 7828 2920 7b0a 2020 2020  _suffix() {.    
-00004d80: 2020 2020 2020 2020 7661 7220 616d 6f6e          var amon
-00004d90: 675f 7661 723b 0a20 2020 2020 2020 2020  g_var;.         
-00004da0: 2020 2073 6270 2e6b 6574 203d 2073 6270     sbp.ket = sbp
-00004db0: 2e63 7572 736f 723b 0a20 2020 2020 2020  .cursor;.       
-00004dc0: 2020 2020 2061 6d6f 6e67 5f76 6172 203d       among_var =
-00004dd0: 2073 6270 2e66 696e 645f 616d 6f6e 675f   sbp.find_among_
-00004de0: 6228 615f 352c 2035 293b 0a20 2020 2020  b(a_5, 5);.     
-00004df0: 2020 2020 2020 2069 6620 2861 6d6f 6e67         if (among
-00004e00: 5f76 6172 2920 7b0a 2020 2020 2020 2020  _var) {.        
-00004e10: 2020 2020 2020 7362 702e 6272 6120 3d20        sbp.bra = 
-00004e20: 7362 702e 6375 7273 6f72 3b0a 2020 2020  sbp.cursor;.    
-00004e30: 2020 2020 2020 2020 2020 6966 2028 725f            if (r_
-00004e40: 5256 2829 2026 2620 616d 6f6e 675f 7661  RV() && among_va
-00004e50: 7220 3d3d 2031 290a 2020 2020 2020 2020  r == 1).        
-00004e60: 2020 2020 2020 2020 7362 702e 736c 6963          sbp.slic
-00004e70: 655f 6465 6c28 293b 0a20 2020 2020 2020  e_del();.       
-00004e80: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00004e90: 207d 0a20 2020 2020 2020 2020 2074 6869   }.          thi
-00004ea0: 732e 7374 656d 203d 2066 756e 6374 696f  s.stem = functio
-00004eb0: 6e28 2920 7b0a 2020 2020 2020 2020 2020  n() {.          
-00004ec0: 2020 7661 7220 765f 3120 3d20 7362 702e    var v_1 = sbp.
-00004ed0: 6375 7273 6f72 3b0a 2020 2020 2020 2020  cursor;.        
-00004ee0: 2020 2020 725f 7072 656c 7564 6528 293b      r_prelude();
-00004ef0: 0a20 2020 2020 2020 2020 2020 2073 6270  .            sbp
-00004f00: 2e63 7572 736f 7220 3d20 765f 313b 0a20  .cursor = v_1;. 
-00004f10: 2020 2020 2020 2020 2020 2072 5f6d 6172             r_mar
-00004f20: 6b5f 7265 6769 6f6e 7328 293b 0a20 2020  k_regions();.   
-00004f30: 2020 2020 2020 2020 2073 6270 2e6c 696d           sbp.lim
-00004f40: 6974 5f62 6163 6b77 6172 6420 3d20 765f  it_backward = v_
-00004f50: 313b 0a20 2020 2020 2020 2020 2020 2073  1;.            s
-00004f60: 6270 2e63 7572 736f 7220 3d20 7362 702e  bp.cursor = sbp.
-00004f70: 6c69 6d69 743b 0a20 2020 2020 2020 2020  limit;.         
-00004f80: 2020 2072 5f73 7465 705f 3028 293b 0a20     r_step_0();. 
-00004f90: 2020 2020 2020 2020 2020 2073 6270 2e63             sbp.c
-00004fa0: 7572 736f 7220 3d20 7362 702e 6c69 6d69  ursor = sbp.limi
-00004fb0: 743b 0a20 2020 2020 2020 2020 2020 2072  t;.            r
-00004fc0: 5f73 7461 6e64 6172 645f 7375 6666 6978  _standard_suffix
-00004fd0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-00004fe0: 7362 702e 6375 7273 6f72 203d 2073 6270  sbp.cursor = sbp
-00004ff0: 2e6c 696d 6974 3b0a 2020 2020 2020 2020  .limit;.        
-00005000: 2020 2020 6966 2028 2142 5f73 7461 6e64      if (!B_stand
-00005010: 6172 645f 7375 6666 6978 5f72 656d 6f76  ard_suffix_remov
-00005020: 6564 2920 7b0a 2020 2020 2020 2020 2020  ed) {.          
-00005030: 2020 2020 7362 702e 6375 7273 6f72 203d      sbp.cursor =
-00005040: 2073 6270 2e6c 696d 6974 3b0a 2020 2020   sbp.limit;.    
-00005050: 2020 2020 2020 2020 2020 725f 7665 7262            r_verb
-00005060: 5f73 7566 6669 7828 293b 0a20 2020 2020  _suffix();.     
-00005070: 2020 2020 2020 2020 2073 6270 2e63 7572           sbp.cur
-00005080: 736f 7220 3d20 7362 702e 6c69 6d69 743b  sor = sbp.limit;
-00005090: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000050a0: 2020 2020 2020 2020 2020 2072 5f76 6f77             r_vow
-000050b0: 656c 5f73 7566 6669 7828 293b 0a20 2020  el_suffix();.   
-000050c0: 2020 2020 2020 2020 2073 6270 2e63 7572           sbp.cur
-000050d0: 736f 7220 3d20 7362 702e 6c69 6d69 745f  sor = sbp.limit_
-000050e0: 6261 636b 7761 7264 3b0a 2020 2020 2020  backward;.      
-000050f0: 2020 2020 2020 725f 706f 7374 6c75 6465        r_postlude
-00005100: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-00005110: 7265 7475 726e 2074 7275 653b 0a20 2020  return true;.   
-00005120: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00005130: 207d 3b0a 0a20 2020 2020 202f 2a20 616e   };..      /* an
-00005140: 6420 7265 7475 726e 2061 2066 756e 6374  d return a funct
-00005150: 696f 6e20 7468 6174 2073 7465 6d73 2061  ion that stems a
-00005160: 2077 6f72 6420 666f 7220 7468 6520 6375   word for the cu
-00005170: 7272 656e 7420 6c6f 6361 6c65 202a 2f0a  rrent locale */.
-00005180: 2020 2020 2020 7265 7475 726e 2066 756e        return fun
-00005190: 6374 696f 6e28 746f 6b65 6e29 207b 0a20  ction(token) {. 
-000051a0: 2020 2020 2020 202f 2f20 666f 7220 6c75         // for lu
-000051b0: 6e72 2076 6572 7369 6f6e 2032 0a20 2020  nr version 2.   
-000051c0: 2020 2020 2069 6620 2874 7970 656f 6620       if (typeof 
-000051d0: 746f 6b65 6e2e 7570 6461 7465 203d 3d3d  token.update ===
-000051e0: 2022 6675 6e63 7469 6f6e 2229 207b 0a20   "function") {. 
-000051f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005200: 746f 6b65 6e2e 7570 6461 7465 2866 756e  token.update(fun
-00005210: 6374 696f 6e28 776f 7264 2920 7b0a 2020  ction(word) {.  
-00005220: 2020 2020 2020 2020 2020 7374 2e73 6574            st.set
-00005230: 4375 7272 656e 7428 776f 7264 293b 0a20  Current(word);. 
-00005240: 2020 2020 2020 2020 2020 2073 742e 7374             st.st
-00005250: 656d 2829 3b0a 2020 2020 2020 2020 2020  em();.          
-00005260: 2020 7265 7475 726e 2073 742e 6765 7443    return st.getC
-00005270: 7572 7265 6e74 2829 3b0a 2020 2020 2020  urrent();.      
-00005280: 2020 2020 7d29 0a20 2020 2020 2020 207d      }).        }
-00005290: 2065 6c73 6520 7b20 2f2f 2066 6f72 206c   else { // for l
-000052a0: 756e 7220 7665 7273 696f 6e20 3c3d 2031  unr version <= 1
-000052b0: 0a20 2020 2020 2020 2020 2073 742e 7365  .          st.se
-000052c0: 7443 7572 7265 6e74 2874 6f6b 656e 293b  tCurrent(token);
-000052d0: 0a20 2020 2020 2020 2020 2073 742e 7374  .          st.st
-000052e0: 656d 2829 3b0a 2020 2020 2020 2020 2020  em();.          
-000052f0: 7265 7475 726e 2073 742e 6765 7443 7572  return st.getCur
-00005300: 7265 6e74 2829 3b0a 2020 2020 2020 2020  rent();.        
-00005310: 7d0a 2020 2020 2020 7d0a 2020 2020 7d29  }.      }.    })
-00005320: 2829 3b0a 0a20 2020 206c 756e 722e 5069  ();..    lunr.Pi
-00005330: 7065 6c69 6e65 2e72 6567 6973 7465 7246  peline.registerF
-00005340: 756e 6374 696f 6e28 6c75 6e72 2e72 6f2e  unction(lunr.ro.
-00005350: 7374 656d 6d65 722c 2027 7374 656d 6d65  stemmer, 'stemme
-00005360: 722d 726f 2729 3b0a 0a20 2020 206c 756e  r-ro');..    lun
-00005370: 722e 726f 2e73 746f 7057 6f72 6446 696c  r.ro.stopWordFil
-00005380: 7465 7220 3d20 6c75 6e72 2e67 656e 6572  ter = lunr.gener
-00005390: 6174 6553 746f 7057 6f72 6446 696c 7465  ateStopWordFilte
-000053a0: 7228 2761 6365 6120 6163 6561 7374 6120  r('acea aceasta 
-000053b0: 6163 6561 7374 c483 2061 6365 6561 2061  aceast.. aceea a
-000053c0: 6365 6920 6163 6569 6120 6163 656c 2061  cei aceia acel a
-000053d0: 6365 6c61 2061 6365 6c65 2061 6365 6c65  cela acele acele
-000053e0: 6120 6163 6573 7420 6163 6573 7461 2061  a acest acesta a
-000053f0: 6365 7374 6520 6163 6573 7465 6120 6163  ceste acestea ac
-00005400: 65c5 9f74 6920 6163 65c5 9f74 6961 2061  e..ti ace..tia a
-00005410: 636f 6c6f 2061 636f 7264 2061 6375 6d20  colo acord acum 
-00005420: 6169 2061 6961 2061 6962 c483 2061 6963  ai aia aib.. aic
-00005430: 6920 616c 2061 6c65 2061 6c65 6120 616c  i al ale alea al
-00005440: 7463 6576 6120 616c 7463 696e 6576 6120  tceva altcineva 
-00005450: 616d 2061 7220 6172 6520 6173 656d 656e  am ar are asemen
-00005460: 6561 2061 7374 6120 6173 7465 6120 6173  ea asta astea as
-00005470: 74c4 837a 6920 6173 7570 7261 2061 7520  t..zi asupra au 
-00005480: 6176 6561 2061 7665 6d20 6176 65c5 a369  avea avem ave..i
-00005490: 2061 7a69 2061 c59f 2061 c59f 6164 6172   azi a.. a..adar
-000054a0: 2061 c5a3 6920 6269 6e65 2062 7563 7572   a..i bine bucur
-000054b0: 2062 756e c483 2063 6120 6361 7265 2063   bun.. ca care c
-000054c0: 6175 7420 6365 2063 656c 2063 6576 6120  aut ce cel ceva 
-000054d0: 6368 6961 7220 6369 6e63 6920 6369 6e65  chiar cinci cine
-000054e0: 2063 696e 6576 6120 636f 6e74 7261 2063   cineva contra c
-000054f0: 7520 6375 6d20 6375 6d76 6120 6375 72c3  u cum cumva cur.
-00005500: a26e 6420 6375 72c3 ae6e 6420 63c3 a26e  .nd cur..nd c..n
-00005510: 6420 63c3 a274 2063 c3a2 7465 2063 c3a2  d c..t c..te c..
-00005520: 7476 6120 63c3 a2c5 a369 2063 c3ae 6e64  tva c....i c..nd
-00005530: 2063 c3ae 7420 63c3 ae74 6520 63c3 ae74   c..t c..te c..t
-00005540: 7661 2063 c3ae c5a3 6920 63c4 8320 63c4  va c....i c.. c.
-00005550: 8363 6920 63c4 8372 6569 2063 c483 726f  .ci c..rei c..ro
-00005560: 7220 63c4 8372 7569 2063 c483 7472 6520  r c..rui c..tre 
-00005570: 6461 2064 6163 c483 2064 6172 2064 6174  da dac.. dar dat
-00005580: 6f72 6974 c483 2064 6174 c483 2064 6175  orit.. dat.. dau
-00005590: 2064 6520 6465 6369 2064 656a 6120 6465   de deci deja de
-000055a0: 6f61 7265 6365 2064 6570 6172 7465 2064  oarece departe d
-000055b0: 65c5 9f69 2064 696e 2064 696e 6169 6e74  e..i din dinaint
-000055c0: 6561 2064 696e 7472 2d20 6469 6e74 7265  ea dintr- dintre
-000055d0: 2064 6f69 2064 6f69 6c65 6120 646f 75c4   doi doilea dou.
-000055e0: 8320 6472 6570 7420 6475 70c4 8320 64c4  . drept dup.. d.
-000055f0: 8320 6561 2065 6920 656c 2065 6c65 2065  . ea ei el ele e
-00005600: 7261 6d20 6573 7465 2065 7520 65c5 9f74  ram este eu e..t
-00005610: 6920 6661 6365 2066 6174 6120 6669 2066  i face fata fi f
-00005620: 6965 2066 6965 6361 7265 2066 6969 2066  ie fiecare fii f
-00005630: 696d 2066 6975 2066 69c5 a369 2066 7275  im fiu fi..i fru
-00005640: 6d6f 7320 66c4 8372 c483 2067 7261 c5a3  mos f..r.. gra..
-00005650: 6965 2068 616c 62c4 8320 6961 7220 6965  ie halb.. iar ie
-00005660: 7269 206c 6120 6c65 206c 6920 6c6f 7220  ri la le li lor 
-00005670: 6c75 6920 6cc3 a26e 67c4 8320 6cc3 ae6e  lui l..ng.. l..n
-00005680: 67c4 8320 6d61 6920 6d65 6120 6d65 6920  g.. mai mea mei 
-00005690: 6d65 6c65 206d 6572 6575 206d 6575 206d  mele mereu meu m
-000056a0: 6920 6d69 6520 6d69 6e65 206d 756c 7420  i mie mine mult 
-000056b0: 6d75 6c74 c483 206d 756c c5a3 6920 6d75  mult.. mul..i mu
-000056c0: 6cc5 a375 6d65 7363 206d c3a2 696e 6520  l..umesc m..ine 
-000056d0: 6dc3 ae69 6e65 206d c483 206e 6520 6e65  m..ine m.. ne ne
-000056e0: 766f 6965 206e 6963 6920 6e69 63c4 8369  voie nici nic..i
-000056f0: 6572 6920 6e69 6d65 6e69 206e 696d 6572  eri nimeni nimer
-00005700: 6920 6e69 6d69 6320 6e69 c59f 7465 206e  i nimic ni..te n
-00005710: 6f61 7374 7265 206e 6f61 7374 72c4 8320  oastre noastr.. 
-00005720: 6e6f 6920 6e6f 726f 6320 6e6f 7374 7275  noi noroc nostru
-00005730: 206e 6f75 c483 206e 6fc5 9f74 7269 206e   nou.. no..tri n
-00005740: 7520 6f70 7420 6f72 6920 6f72 6963 6172  u opt ori oricar
-00005750: 6520 6f72 6963 6520 6f72 6963 696e 6520  e orice oricine 
-00005760: 6f72 6963 756d 206f 7269 63c3 a26e 6420  oricum oric..nd 
-00005770: 6f72 6963 c3a2 7420 6f72 6963 c3ae 6e64  oric..t oric..nd
-00005780: 206f 7269 63c3 ae74 206f 7269 756e 6465   oric..t oriunde
-00005790: 2070 6174 7261 2070 6174 7275 2070 6174   patra patru pat
-000057a0: 7275 6c65 6120 7065 2070 656e 7472 7520  rulea pe pentru 
-000057b0: 7065 7374 6520 7069 6320 706f 6174 6520  peste pic poate 
-000057c0: 706f 7420 7072 6561 2070 7269 6d61 2070  pot prea prima p
-000057d0: 7269 6d75 6c20 7072 696e 2070 75c5 a369  rimul prin pu..i
-000057e0: 6e20 7075 c5a3 696e 6120 7075 c5a3 696e  n pu..ina pu..in
-000057f0: c483 2070 c3a2 6ec4 8320 70c3 ae6e c483  .. p..n.. p..n..
-00005800: 2072 6f67 2073 6120 7361 6c65 2073 6175   rog sa sale sau
-00005810: 2073 6520 7370 6174 6520 7370 7265 2073   se spate spre s
-00005820: 7562 2073 756e 7420 7375 6e74 656d 2073  ub sunt suntem s
-00005830: 756e 7465 c5a3 6920 7375 74c4 8320 73c3  unte..i sut.. s.
-00005840: ae6e 7420 73c3 ae6e 7465 6d20 73c3 ae6e  .nt s..ntem s..n
-00005850: 7465 c5a3 6920 73c4 8320 73c4 8369 2073  te..i s.. s..i s
-00005860: c483 7520 7461 2074 616c 6520 7465 2074  ..u ta tale te t
-00005870: 696d 7020 7469 6e65 2074 6f61 7465 2074  imp tine toate t
-00005880: 6f61 74c4 8320 746f 7420 746f 7475 c59f  oat.. tot totu..
-00005890: 6920 746f c5a3 6920 7472 6569 2074 7265  i to..i trei tre
-000058a0: 6961 2074 7265 696c 6561 2074 7520 74c4  ia treilea tu t.
-000058b0: 8369 2074 c483 7520 756e 2075 6e61 2075  .i t..u un una u
-000058c0: 6e64 6520 756e 6465 7661 2075 6e65 6920  nde undeva unei 
-000058d0: 756e 6569 6120 756e 656c 6520 756e 656f  uneia unele uneo
-000058e0: 7269 2075 6e69 6920 756e 6f72 2075 6e6f  ri unii unor uno
-000058f0: 7261 2075 6e75 2075 6e75 6920 756e 7569  ra unu unui unui
-00005900: 6120 756e 756c 2076 6920 766f 6173 7472  a unul vi voastr
-00005910: 6520 766f 6173 7472 c483 2076 6f69 2076  e voastr.. voi v
-00005920: 6f73 7472 7520 766f 75c4 8320 766f c59f  ostru vou.. vo..
-00005930: 7472 6920 7672 656d 6520 7672 656f 2076  tri vreme vreo v
-00005940: 7265 756e 2076 c483 207a 6563 6520 7a65  reun v.. zece ze
-00005950: 726f 207a 6920 7a69 6365 20c3 ae69 20c3  ro zi zice ..i .
-00005960: ae6c 20c3 ae6d 6920 c3ae 6d70 6f74 7269  .l ..mi ..mpotri
-00005970: 7661 20c3 ae6e 2020 c3ae 6e61 696e 7465  va ..n  ..nainte
-00005980: 20c3 ae6e 6169 6e74 6561 20c3 ae6e 636f   ..naintea ..nco
-00005990: 7472 6f20 c3ae 6e63 c3a2 7420 c3ae 6e63  tro ..nc..t ..nc
-000059a0: c3ae 7420 c3ae 6e74 7265 20c3 ae6e 7472  ..t ..ntre ..ntr
-000059b0: 7563 c3a2 7420 c3ae 6e74 7275 63c3 ae74  uc..t ..ntruc..t
-000059c0: 20c3 aec5 a369 20c4 836c 6120 c483 6c65   ....i ..la ..le
-000059d0: 6120 c483 7374 6120 c483 7374 6561 20c4  a ..sta ..stea .
-000059e0: 83c5 9f74 6961 20c5 9f61 7074 6520 c59f  ...tia ..apte ..
-000059f0: 6173 6520 c59f 6920 c59f 7469 7520 c5a3  ase ..i ..tiu ..
-00005a00: 6920 c5a3 6965 272e 7370 6c69 7428 2720  i ..ie'.split(' 
-00005a10: 2729 293b 0a0a 2020 2020 6c75 6e72 2e50  '));..    lunr.P
-00005a20: 6970 656c 696e 652e 7265 6769 7374 6572  ipeline.register
-00005a30: 4675 6e63 7469 6f6e 286c 756e 722e 726f  Function(lunr.ro
-00005a40: 2e73 746f 7057 6f72 6446 696c 7465 722c  .stopWordFilter,
-00005a50: 2027 7374 6f70 576f 7264 4669 6c74 6572   'stopWordFilter
-00005a60: 2d72 6f27 293b 0a20 207d 3b0a 7d29 29    -ro');.  };.}))
+00004ca0: 2020 2020 2020 2020 2020 2063 6173 6520             case 
+00004cb0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00004cc0: 2020 2020 2020 2020 2073 6270 2e73 6c69           sbp.sli
+00004cd0: 6365 5f64 656c 2829 3b0a 2020 2020 2020  ce_del();.      
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 6272 6561 6b3b 0a20 2020 2020 2020 2020  break;.         
+00004d00: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004d10: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004d20: 2020 2020 2020 2073 6270 2e6c 696d 6974         sbp.limit
+00004d30: 5f62 6163 6b77 6172 6420 3d20 765f 313b  _backward = v_1;
+00004d40: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00004d50: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+00004d60: 2020 2020 2020 6675 6e63 7469 6f6e 2072        function r
+00004d70: 5f76 6f77 656c 5f73 7566 6669 7828 2920  _vowel_suffix() 
+00004d80: 7b0a 2020 2020 2020 2020 2020 2020 7661  {.            va
+00004d90: 7220 616d 6f6e 675f 7661 723b 0a20 2020  r among_var;.   
+00004da0: 2020 2020 2020 2020 2073 6270 2e6b 6574           sbp.ket
+00004db0: 203d 2073 6270 2e63 7572 736f 723b 0a20   = sbp.cursor;. 
+00004dc0: 2020 2020 2020 2020 2020 2061 6d6f 6e67             among
+00004dd0: 5f76 6172 203d 2073 6270 2e66 696e 645f  _var = sbp.find_
+00004de0: 616d 6f6e 675f 6228 615f 352c 2035 293b  among_b(a_5, 5);
+00004df0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004e00: 2861 6d6f 6e67 5f76 6172 2920 7b0a 2020  (among_var) {.  
+00004e10: 2020 2020 2020 2020 2020 2020 7362 702e              sbp.
+00004e20: 6272 6120 3d20 7362 702e 6375 7273 6f72  bra = sbp.cursor
+00004e30: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00004e40: 6966 2028 725f 5256 2829 2026 2620 616d  if (r_RV() && am
+00004e50: 6f6e 675f 7661 7220 3d3d 2031 290a 2020  ong_var == 1).  
+00004e60: 2020 2020 2020 2020 2020 2020 2020 7362                sb
+00004e70: 702e 736c 6963 655f 6465 6c28 293b 0a20  p.slice_del();. 
+00004e80: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00004e90: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004ea0: 2020 2074 6869 732e 7374 656d 203d 2066     this.stem = f
+00004eb0: 756e 6374 696f 6e28 2920 7b0a 2020 2020  unction() {.    
+00004ec0: 2020 2020 2020 2020 7661 7220 765f 3120          var v_1 
+00004ed0: 3d20 7362 702e 6375 7273 6f72 3b0a 2020  = sbp.cursor;.  
+00004ee0: 2020 2020 2020 2020 2020 725f 7072 656c            r_prel
+00004ef0: 7564 6528 293b 0a20 2020 2020 2020 2020  ude();.         
+00004f00: 2020 2073 6270 2e63 7572 736f 7220 3d20     sbp.cursor = 
+00004f10: 765f 313b 0a20 2020 2020 2020 2020 2020  v_1;.           
+00004f20: 2072 5f6d 6172 6b5f 7265 6769 6f6e 7328   r_mark_regions(
+00004f30: 293b 0a20 2020 2020 2020 2020 2020 2073  );.            s
+00004f40: 6270 2e6c 696d 6974 5f62 6163 6b77 6172  bp.limit_backwar
+00004f50: 6420 3d20 765f 313b 0a20 2020 2020 2020  d = v_1;.       
+00004f60: 2020 2020 2073 6270 2e63 7572 736f 7220       sbp.cursor 
+00004f70: 3d20 7362 702e 6c69 6d69 743b 0a20 2020  = sbp.limit;.   
+00004f80: 2020 2020 2020 2020 2072 5f73 7465 705f           r_step_
+00004f90: 3028 293b 0a20 2020 2020 2020 2020 2020  0();.           
+00004fa0: 2073 6270 2e63 7572 736f 7220 3d20 7362   sbp.cursor = sb
+00004fb0: 702e 6c69 6d69 743b 0a20 2020 2020 2020  p.limit;.       
+00004fc0: 2020 2020 2072 5f73 7461 6e64 6172 645f       r_standard_
+00004fd0: 7375 6666 6978 2829 3b0a 2020 2020 2020  suffix();.      
+00004fe0: 2020 2020 2020 7362 702e 6375 7273 6f72        sbp.cursor
+00004ff0: 203d 2073 6270 2e6c 696d 6974 3b0a 2020   = sbp.limit;.  
+00005000: 2020 2020 2020 2020 2020 6966 2028 2142            if (!B
+00005010: 5f73 7461 6e64 6172 645f 7375 6666 6978  _standard_suffix
+00005020: 5f72 656d 6f76 6564 2920 7b0a 2020 2020  _removed) {.    
+00005030: 2020 2020 2020 2020 2020 7362 702e 6375            sbp.cu
+00005040: 7273 6f72 203d 2073 6270 2e6c 696d 6974  rsor = sbp.limit
+00005050: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00005060: 725f 7665 7262 5f73 7566 6669 7828 293b  r_verb_suffix();
+00005070: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
+00005080: 6270 2e63 7572 736f 7220 3d20 7362 702e  bp.cursor = sbp.
+00005090: 6c69 6d69 743b 0a20 2020 2020 2020 2020  limit;.         
+000050a0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000050b0: 2072 5f76 6f77 656c 5f73 7566 6669 7828   r_vowel_suffix(
+000050c0: 293b 0a20 2020 2020 2020 2020 2020 2073  );.            s
+000050d0: 6270 2e63 7572 736f 7220 3d20 7362 702e  bp.cursor = sbp.
+000050e0: 6c69 6d69 745f 6261 636b 7761 7264 3b0a  limit_backward;.
+000050f0: 2020 2020 2020 2020 2020 2020 725f 706f              r_po
+00005100: 7374 6c75 6465 2829 3b0a 2020 2020 2020  stlude();.      
+00005110: 2020 2020 2020 7265 7475 726e 2074 7275        return tru
+00005120: 653b 0a20 2020 2020 2020 2020 207d 0a20  e;.          }. 
+00005130: 2020 2020 2020 207d 3b0a 0a20 2020 2020         };..     
+00005140: 202f 2a20 616e 6420 7265 7475 726e 2061   /* and return a
+00005150: 2066 756e 6374 696f 6e20 7468 6174 2073   function that s
+00005160: 7465 6d73 2061 2077 6f72 6420 666f 7220  tems a word for 
+00005170: 7468 6520 6375 7272 656e 7420 6c6f 6361  the current loca
+00005180: 6c65 202a 2f0a 2020 2020 2020 7265 7475  le */.      retu
+00005190: 726e 2066 756e 6374 696f 6e28 746f 6b65  rn function(toke
+000051a0: 6e29 207b 0a20 2020 2020 2020 202f 2f20  n) {.        // 
+000051b0: 666f 7220 6c75 6e72 2076 6572 7369 6f6e  for lunr version
+000051c0: 2032 0a20 2020 2020 2020 2069 6620 2874   2.        if (t
+000051d0: 7970 656f 6620 746f 6b65 6e2e 7570 6461  ypeof token.upda
+000051e0: 7465 203d 3d3d 2022 6675 6e63 7469 6f6e  te === "function
+000051f0: 2229 207b 0a20 2020 2020 2020 2020 2072  ") {.          r
+00005200: 6574 7572 6e20 746f 6b65 6e2e 7570 6461  eturn token.upda
+00005210: 7465 2866 756e 6374 696f 6e28 776f 7264  te(function(word
+00005220: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00005230: 7374 2e73 6574 4375 7272 656e 7428 776f  st.setCurrent(wo
+00005240: 7264 293b 0a20 2020 2020 2020 2020 2020  rd);.           
+00005250: 2073 742e 7374 656d 2829 3b0a 2020 2020   st.stem();.    
+00005260: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005270: 742e 6765 7443 7572 7265 6e74 2829 3b0a  t.getCurrent();.
+00005280: 2020 2020 2020 2020 2020 7d29 0a20 2020            }).   
+00005290: 2020 2020 207d 2065 6c73 6520 7b20 2f2f       } else { //
+000052a0: 2066 6f72 206c 756e 7220 7665 7273 696f   for lunr versio
+000052b0: 6e20 3c3d 2031 0a20 2020 2020 2020 2020  n <= 1.         
+000052c0: 2073 742e 7365 7443 7572 7265 6e74 2874   st.setCurrent(t
+000052d0: 6f6b 656e 293b 0a20 2020 2020 2020 2020  oken);.         
+000052e0: 2073 742e 7374 656d 2829 3b0a 2020 2020   st.stem();.    
+000052f0: 2020 2020 2020 7265 7475 726e 2073 742e        return st.
+00005300: 6765 7443 7572 7265 6e74 2829 3b0a 2020  getCurrent();.  
+00005310: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+00005320: 2020 2020 7d29 2829 3b0a 0a20 2020 206c      })();..    l
+00005330: 756e 722e 5069 7065 6c69 6e65 2e72 6567  unr.Pipeline.reg
+00005340: 6973 7465 7246 756e 6374 696f 6e28 6c75  isterFunction(lu
+00005350: 6e72 2e72 6f2e 7374 656d 6d65 722c 2027  nr.ro.stemmer, '
+00005360: 7374 656d 6d65 722d 726f 2729 3b0a 0a20  stemmer-ro');.. 
+00005370: 2020 206c 756e 722e 726f 2e73 746f 7057     lunr.ro.stopW
+00005380: 6f72 6446 696c 7465 7220 3d20 6c75 6e72  ordFilter = lunr
+00005390: 2e67 656e 6572 6174 6553 746f 7057 6f72  .generateStopWor
+000053a0: 6446 696c 7465 7228 2761 6365 6120 6163  dFilter('acea ac
+000053b0: 6561 7374 6120 6163 6561 7374 c483 2061  easta aceast.. a
+000053c0: 6365 6561 2061 6365 6920 6163 6569 6120  ceea acei aceia 
+000053d0: 6163 656c 2061 6365 6c61 2061 6365 6c65  acel acela acele
+000053e0: 2061 6365 6c65 6120 6163 6573 7420 6163   acelea acest ac
+000053f0: 6573 7461 2061 6365 7374 6520 6163 6573  esta aceste aces
+00005400: 7465 6120 6163 65c5 9f74 6920 6163 65c5  tea ace..ti ace.
+00005410: 9f74 6961 2061 636f 6c6f 2061 636f 7264  .tia acolo acord
+00005420: 2061 6375 6d20 6169 2061 6961 2061 6962   acum ai aia aib
+00005430: c483 2061 6963 6920 616c 2061 6c65 2061  .. aici al ale a
+00005440: 6c65 6120 616c 7463 6576 6120 616c 7463  lea altceva altc
+00005450: 696e 6576 6120 616d 2061 7220 6172 6520  ineva am ar are 
+00005460: 6173 656d 656e 6561 2061 7374 6120 6173  asemenea asta as
+00005470: 7465 6120 6173 74c4 837a 6920 6173 7570  tea ast..zi asup
+00005480: 7261 2061 7520 6176 6561 2061 7665 6d20  ra au avea avem 
+00005490: 6176 65c5 a369 2061 7a69 2061 c59f 2061  ave..i azi a.. a
+000054a0: c59f 6164 6172 2061 c5a3 6920 6269 6e65  ..adar a..i bine
+000054b0: 2062 7563 7572 2062 756e c483 2063 6120   bucur bun.. ca 
+000054c0: 6361 7265 2063 6175 7420 6365 2063 656c  care caut ce cel
+000054d0: 2063 6576 6120 6368 6961 7220 6369 6e63   ceva chiar cinc
+000054e0: 6920 6369 6e65 2063 696e 6576 6120 636f  i cine cineva co
+000054f0: 6e74 7261 2063 7520 6375 6d20 6375 6d76  ntra cu cum cumv
+00005500: 6120 6375 72c3 a26e 6420 6375 72c3 ae6e  a cur..nd cur..n
+00005510: 6420 63c3 a26e 6420 63c3 a274 2063 c3a2  d c..nd c..t c..
+00005520: 7465 2063 c3a2 7476 6120 63c3 a2c5 a369  te c..tva c....i
+00005530: 2063 c3ae 6e64 2063 c3ae 7420 63c3 ae74   c..nd c..t c..t
+00005540: 6520 63c3 ae74 7661 2063 c3ae c5a3 6920  e c..tva c....i 
+00005550: 63c4 8320 63c4 8363 6920 63c4 8372 6569  c.. c..ci c..rei
+00005560: 2063 c483 726f 7220 63c4 8372 7569 2063   c..ror c..rui c
+00005570: c483 7472 6520 6461 2064 6163 c483 2064  ..tre da dac.. d
+00005580: 6172 2064 6174 6f72 6974 c483 2064 6174  ar datorit.. dat
+00005590: c483 2064 6175 2064 6520 6465 6369 2064  .. dau de deci d
+000055a0: 656a 6120 6465 6f61 7265 6365 2064 6570  eja deoarece dep
+000055b0: 6172 7465 2064 65c5 9f69 2064 696e 2064  arte de..i din d
+000055c0: 696e 6169 6e74 6561 2064 696e 7472 2d20  inaintea dintr- 
+000055d0: 6469 6e74 7265 2064 6f69 2064 6f69 6c65  dintre doi doile
+000055e0: 6120 646f 75c4 8320 6472 6570 7420 6475  a dou.. drept du
+000055f0: 70c4 8320 64c4 8320 6561 2065 6920 656c  p.. d.. ea ei el
+00005600: 2065 6c65 2065 7261 6d20 6573 7465 2065   ele eram este e
+00005610: 7520 65c5 9f74 6920 6661 6365 2066 6174  u e..ti face fat
+00005620: 6120 6669 2066 6965 2066 6965 6361 7265  a fi fie fiecare
+00005630: 2066 6969 2066 696d 2066 6975 2066 69c5   fii fim fiu fi.
+00005640: a369 2066 7275 6d6f 7320 66c4 8372 c483  .i frumos f..r..
+00005650: 2067 7261 c5a3 6965 2068 616c 62c4 8320   gra..ie halb.. 
+00005660: 6961 7220 6965 7269 206c 6120 6c65 206c  iar ieri la le l
+00005670: 6920 6c6f 7220 6c75 6920 6cc3 a26e 67c4  i lor lui l..ng.
+00005680: 8320 6cc3 ae6e 67c4 8320 6d61 6920 6d65  . l..ng.. mai me
+00005690: 6120 6d65 6920 6d65 6c65 206d 6572 6575  a mei mele mereu
+000056a0: 206d 6575 206d 6920 6d69 6520 6d69 6e65   meu mi mie mine
+000056b0: 206d 756c 7420 6d75 6c74 c483 206d 756c   mult mult.. mul
+000056c0: c5a3 6920 6d75 6cc5 a375 6d65 7363 206d  ..i mul..umesc m
+000056d0: c3a2 696e 6520 6dc3 ae69 6e65 206d c483  ..ine m..ine m..
+000056e0: 206e 6520 6e65 766f 6965 206e 6963 6920   ne nevoie nici 
+000056f0: 6e69 63c4 8369 6572 6920 6e69 6d65 6e69  nic..ieri nimeni
+00005700: 206e 696d 6572 6920 6e69 6d69 6320 6e69   nimeri nimic ni
+00005710: c59f 7465 206e 6f61 7374 7265 206e 6f61  ..te noastre noa
+00005720: 7374 72c4 8320 6e6f 6920 6e6f 726f 6320  str.. noi noroc 
+00005730: 6e6f 7374 7275 206e 6f75 c483 206e 6fc5  nostru nou.. no.
+00005740: 9f74 7269 206e 7520 6f70 7420 6f72 6920  .tri nu opt ori 
+00005750: 6f72 6963 6172 6520 6f72 6963 6520 6f72  oricare orice or
+00005760: 6963 696e 6520 6f72 6963 756d 206f 7269  icine oricum ori
+00005770: 63c3 a26e 6420 6f72 6963 c3a2 7420 6f72  c..nd oric..t or
+00005780: 6963 c3ae 6e64 206f 7269 63c3 ae74 206f  ic..nd oric..t o
+00005790: 7269 756e 6465 2070 6174 7261 2070 6174  riunde patra pat
+000057a0: 7275 2070 6174 7275 6c65 6120 7065 2070  ru patrulea pe p
+000057b0: 656e 7472 7520 7065 7374 6520 7069 6320  entru peste pic 
+000057c0: 706f 6174 6520 706f 7420 7072 6561 2070  poate pot prea p
+000057d0: 7269 6d61 2070 7269 6d75 6c20 7072 696e  rima primul prin
+000057e0: 2070 75c5 a369 6e20 7075 c5a3 696e 6120   pu..in pu..ina 
+000057f0: 7075 c5a3 696e c483 2070 c3a2 6ec4 8320  pu..in.. p..n.. 
+00005800: 70c3 ae6e c483 2072 6f67 2073 6120 7361  p..n.. rog sa sa
+00005810: 6c65 2073 6175 2073 6520 7370 6174 6520  le sau se spate 
+00005820: 7370 7265 2073 7562 2073 756e 7420 7375  spre sub sunt su
+00005830: 6e74 656d 2073 756e 7465 c5a3 6920 7375  ntem sunte..i su
+00005840: 74c4 8320 73c3 ae6e 7420 73c3 ae6e 7465  t.. s..nt s..nte
+00005850: 6d20 73c3 ae6e 7465 c5a3 6920 73c4 8320  m s..nte..i s.. 
+00005860: 73c4 8369 2073 c483 7520 7461 2074 616c  s..i s..u ta tal
+00005870: 6520 7465 2074 696d 7020 7469 6e65 2074  e te timp tine t
+00005880: 6f61 7465 2074 6f61 74c4 8320 746f 7420  oate toat.. tot 
+00005890: 746f 7475 c59f 6920 746f c5a3 6920 7472  totu..i to..i tr
+000058a0: 6569 2074 7265 6961 2074 7265 696c 6561  ei treia treilea
+000058b0: 2074 7520 74c4 8369 2074 c483 7520 756e   tu t..i t..u un
+000058c0: 2075 6e61 2075 6e64 6520 756e 6465 7661   una unde undeva
+000058d0: 2075 6e65 6920 756e 6569 6120 756e 656c   unei uneia unel
+000058e0: 6520 756e 656f 7269 2075 6e69 6920 756e  e uneori unii un
+000058f0: 6f72 2075 6e6f 7261 2075 6e75 2075 6e75  or unora unu unu
+00005900: 6920 756e 7569 6120 756e 756c 2076 6920  i unuia unul vi 
+00005910: 766f 6173 7472 6520 766f 6173 7472 c483  voastre voastr..
+00005920: 2076 6f69 2076 6f73 7472 7520 766f 75c4   voi vostru vou.
+00005930: 8320 766f c59f 7472 6920 7672 656d 6520  . vo..tri vreme 
+00005940: 7672 656f 2076 7265 756e 2076 c483 207a  vreo vreun v.. z
+00005950: 6563 6520 7a65 726f 207a 6920 7a69 6365  ece zero zi zice
+00005960: 20c3 ae69 20c3 ae6c 20c3 ae6d 6920 c3ae   ..i ..l ..mi ..
+00005970: 6d70 6f74 7269 7661 20c3 ae6e 2020 c3ae  mpotriva ..n  ..
+00005980: 6e61 696e 7465 20c3 ae6e 6169 6e74 6561  nainte ..naintea
+00005990: 20c3 ae6e 636f 7472 6f20 c3ae 6e63 c3a2   ..ncotro ..nc..
+000059a0: 7420 c3ae 6e63 c3ae 7420 c3ae 6e74 7265  t ..nc..t ..ntre
+000059b0: 20c3 ae6e 7472 7563 c3a2 7420 c3ae 6e74   ..ntruc..t ..nt
+000059c0: 7275 63c3 ae74 20c3 aec5 a369 20c4 836c  ruc..t ....i ..l
+000059d0: 6120 c483 6c65 6120 c483 7374 6120 c483  a ..lea ..sta ..
+000059e0: 7374 6561 20c4 83c5 9f74 6961 20c5 9f61  stea ....tia ..a
+000059f0: 7074 6520 c59f 6173 6520 c59f 6920 c59f  pte ..ase ..i ..
+00005a00: 7469 7520 c5a3 6920 c5a3 6965 272e 7370  tiu ..i ..ie'.sp
+00005a10: 6c69 7428 2720 2729 293b 0a0a 2020 2020  lit(' '));..    
+00005a20: 6c75 6e72 2e50 6970 656c 696e 652e 7265  lunr.Pipeline.re
+00005a30: 6769 7374 6572 4675 6e63 7469 6f6e 286c  gisterFunction(l
+00005a40: 756e 722e 726f 2e73 746f 7057 6f72 6446  unr.ro.stopWordF
+00005a50: 696c 7465 722c 2027 7374 6f70 576f 7264  ilter, 'stopWord
+00005a60: 4669 6c74 6572 2d72 6f27 293b 0a20 207d  Filter-ro');.  }
+00005a70: 3b0a 7d29 29                             ;.}))
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.ru.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.ru.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (2551)*

 * *Files 0% similar despite different names*

```diff
@@ -666,530 +666,530 @@
 00002990: 2020 2020 2020 2020 2020 6966 2028 2173            if (!s
 000029a0: 6270 2e65 715f 735f 6228 312c 2022 5c75  bp.eq_s_b(1, "\u
 000029b0: 3034 3446 2229 290a 2020 2020 2020 2020  044F")).        
 000029c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
 000029d0: 7475 726e 2066 616c 7365 3b0a 2020 2020  turn false;.    
 000029e0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
 000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 6361 7365 2032 3a0a 2020 2020 2020 2020  case 2:.        
-00002a10: 2020 2020 2020 2020 2020 7362 702e 736c            sbp.sl
-00002a20: 6963 655f 6465 6c28 293b 0a20 2020 2020  ice_del();.     
-00002a30: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00002a40: 616b 3b0a 2020 2020 2020 2020 2020 2020  ak;.            
-00002a50: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00002a60: 2020 7265 7475 726e 2074 7275 653b 0a20    return true;. 
-00002a70: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002a80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002a90: 6661 6c73 653b 0a20 2020 2020 2020 2020  false;.         
-00002aa0: 207d 0a0a 2020 2020 2020 2020 2020 6675   }..          fu
-00002ab0: 6e63 7469 6f6e 2072 5f70 6572 6665 6374  nction r_perfect
-00002ac0: 6976 655f 6765 7275 6e64 2829 207b 0a20  ive_gerund() {. 
-00002ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002ae0: 6e20 6861 6272 3228 615f 302c 2039 293b  n habr2(a_0, 9);
-00002af0: 0a20 2020 2020 2020 2020 207d 0a0a 2020  .          }..  
-00002b00: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00002b10: 2068 6162 7231 2861 2c20 6e29 207b 0a20   habr1(a, n) {. 
-00002b20: 2020 2020 2020 2020 2020 2076 6172 2061             var a
-00002b30: 6d6f 6e67 5f76 6172 3b0a 2020 2020 2020  mong_var;.      
-00002b40: 2020 2020 2020 7362 702e 6b65 7420 3d20        sbp.ket = 
-00002b50: 7362 702e 6375 7273 6f72 3b0a 2020 2020  sbp.cursor;.    
-00002b60: 2020 2020 2020 2020 616d 6f6e 675f 7661          among_va
-00002b70: 7220 3d20 7362 702e 6669 6e64 5f61 6d6f  r = sbp.find_amo
-00002b80: 6e67 5f62 2861 2c20 6e29 3b0a 2020 2020  ng_b(a, n);.    
-00002b90: 2020 2020 2020 2020 6966 2028 616d 6f6e          if (amon
-00002ba0: 675f 7661 7229 207b 0a20 2020 2020 2020  g_var) {.       
-00002bb0: 2020 2020 2020 2073 6270 2e62 7261 203d         sbp.bra =
-00002bc0: 2073 6270 2e63 7572 736f 723b 0a20 2020   sbp.cursor;.   
-00002bd0: 2020 2020 2020 2020 2020 2069 6620 2861             if (a
-00002be0: 6d6f 6e67 5f76 6172 203d 3d20 3129 0a20  mong_var == 1). 
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002c00: 6270 2e73 6c69 6365 5f64 656c 2829 3b0a  bp.slice_del();.
-00002c10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00002c20: 7475 726e 2074 7275 653b 0a20 2020 2020  turn true;.     
-00002c30: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002c40: 2020 2020 2072 6574 7572 6e20 6661 6c73       return fals
-00002c50: 653b 0a20 2020 2020 2020 2020 207d 0a0a  e;.          }..
-00002c60: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
-00002c70: 6f6e 2072 5f61 646a 6563 7469 7665 2829  on r_adjective()
-00002c80: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
-00002c90: 6574 7572 6e20 6861 6272 3128 615f 312c  eturn habr1(a_1,
-00002ca0: 2032 3629 3b0a 2020 2020 2020 2020 2020   26);.          
-00002cb0: 7d0a 0a20 2020 2020 2020 2020 2066 756e  }..          fun
-00002cc0: 6374 696f 6e20 725f 6164 6a65 6374 6976  ction r_adjectiv
-00002cd0: 616c 2829 207b 0a20 2020 2020 2020 2020  al() {.         
-00002ce0: 2020 2076 6172 2061 6d6f 6e67 5f76 6172     var among_var
-00002cf0: 3b0a 2020 2020 2020 2020 2020 2020 6966  ;.            if
-00002d00: 2028 725f 6164 6a65 6374 6976 6528 2929   (r_adjective())
-00002d10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00002d20: 2068 6162 7232 2861 5f32 2c20 3829 3b0a   habr2(a_2, 8);.
-00002d30: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00002d40: 7475 726e 2074 7275 653b 0a20 2020 2020  turn true;.     
-00002d50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002d60: 2020 2020 2072 6574 7572 6e20 6661 6c73       return fals
-00002d70: 653b 0a20 2020 2020 2020 2020 207d 0a0a  e;.          }..
-00002d80: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
-00002d90: 6f6e 2072 5f72 6566 6c65 7869 7665 2829  on r_reflexive()
-00002da0: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
-00002db0: 6574 7572 6e20 6861 6272 3128 615f 332c  eturn habr1(a_3,
-00002dc0: 2032 293b 0a20 2020 2020 2020 2020 207d   2);.          }
-00002dd0: 0a0a 2020 2020 2020 2020 2020 6675 6e63  ..          func
-00002de0: 7469 6f6e 2072 5f76 6572 6228 2920 7b0a  tion r_verb() {.
-00002df0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002e00: 726e 2068 6162 7232 2861 5f34 2c20 3436  rn habr2(a_4, 46
-00002e10: 293b 0a20 2020 2020 2020 2020 207d 0a0a  );.          }..
-00002e20: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
-00002e30: 6f6e 2072 5f6e 6f75 6e28 2920 7b0a 2020  on r_noun() {.  
-00002e40: 2020 2020 2020 2020 2020 6861 6272 3128            habr1(
-00002e50: 615f 352c 2033 3629 3b0a 2020 2020 2020  a_5, 36);.      
-00002e60: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
-00002e70: 2066 756e 6374 696f 6e20 725f 6465 7269   function r_deri
-00002e80: 7661 7469 6f6e 616c 2829 207b 0a20 2020  vational() {.   
-00002e90: 2020 2020 2020 2020 2076 6172 2061 6d6f           var amo
-00002ea0: 6e67 5f76 6172 3b0a 2020 2020 2020 2020  ng_var;.        
-00002eb0: 2020 2020 7362 702e 6b65 7420 3d20 7362      sbp.ket = sb
-00002ec0: 702e 6375 7273 6f72 3b0a 2020 2020 2020  p.cursor;.      
-00002ed0: 2020 2020 2020 616d 6f6e 675f 7661 7220        among_var 
-00002ee0: 3d20 7362 702e 6669 6e64 5f61 6d6f 6e67  = sbp.find_among
-00002ef0: 5f62 2861 5f36 2c20 3229 3b0a 2020 2020  _b(a_6, 2);.    
-00002f00: 2020 2020 2020 2020 6966 2028 616d 6f6e          if (amon
-00002f10: 675f 7661 7229 207b 0a20 2020 2020 2020  g_var) {.       
-00002f20: 2020 2020 2020 2073 6270 2e62 7261 203d         sbp.bra =
-00002f30: 2073 6270 2e63 7572 736f 723b 0a20 2020   sbp.cursor;.   
-00002f40: 2020 2020 2020 2020 2020 2069 6620 2872             if (r
-00002f50: 5f52 3228 2920 2626 2061 6d6f 6e67 5f76  _R2() && among_v
-00002f60: 6172 203d 3d20 3129 0a20 2020 2020 2020  ar == 1).       
-00002f70: 2020 2020 2020 2020 2073 6270 2e73 6c69           sbp.sli
-00002f80: 6365 5f64 656c 2829 3b0a 2020 2020 2020  ce_del();.      
-00002f90: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002fa0: 2020 7d0a 0a20 2020 2020 2020 2020 2066    }..          f
-00002fb0: 756e 6374 696f 6e20 725f 7469 6479 5f75  unction r_tidy_u
-00002fc0: 7028 2920 7b0a 2020 2020 2020 2020 2020  p() {.          
-00002fd0: 2020 7661 7220 616d 6f6e 675f 7661 723b    var among_var;
-00002fe0: 0a20 2020 2020 2020 2020 2020 2073 6270  .            sbp
-00002ff0: 2e6b 6574 203d 2073 6270 2e63 7572 736f  .ket = sbp.curso
-00003000: 723b 0a20 2020 2020 2020 2020 2020 2061  r;.            a
-00003010: 6d6f 6e67 5f76 6172 203d 2073 6270 2e66  mong_var = sbp.f
-00003020: 696e 645f 616d 6f6e 675f 6228 615f 372c  ind_among_b(a_7,
-00003030: 2034 293b 0a20 2020 2020 2020 2020 2020   4);.           
-00003040: 2069 6620 2861 6d6f 6e67 5f76 6172 2920   if (among_var) 
-00003050: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003060: 7362 702e 6272 6120 3d20 7362 702e 6375  sbp.bra = sbp.cu
-00003070: 7273 6f72 3b0a 2020 2020 2020 2020 2020  rsor;.          
-00003080: 2020 2020 7377 6974 6368 2028 616d 6f6e      switch (amon
-00003090: 675f 7661 7229 207b 0a20 2020 2020 2020  g_var) {.       
-000030a0: 2020 2020 2020 2020 2063 6173 6520 313a           case 1:
-000030b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030c0: 2020 2073 6270 2e73 6c69 6365 5f64 656c     sbp.slice_del
-000030d0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-000030e0: 2020 2020 2020 7362 702e 6b65 7420 3d20        sbp.ket = 
-000030f0: 7362 702e 6375 7273 6f72 3b0a 2020 2020  sbp.cursor;.    
-00003100: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003110: 2028 2173 6270 2e65 715f 735f 6228 312c   (!sbp.eq_s_b(1,
-00003120: 2022 5c75 3034 3344 2229 290a 2020 2020   "\u043D")).    
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 6272 6561 6b3b 0a20 2020 2020 2020 2020  break;.         
-00003150: 2020 2020 2020 2020 2073 6270 2e62 7261           sbp.bra
-00003160: 203d 2073 6270 2e63 7572 736f 723b 0a20   = sbp.cursor;. 
-00003170: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003180: 6173 6520 323a 0a20 2020 2020 2020 2020  ase 2:.         
-00003190: 2020 2020 2020 2020 2069 6620 2821 7362           if (!sb
-000031a0: 702e 6571 5f73 5f62 2831 2c20 225c 7530  p.eq_s_b(1, "\u0
-000031b0: 3433 4422 2929 0a20 2020 2020 2020 2020  43D")).         
-000031c0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000031d0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000031e0: 2020 6361 7365 2033 3a0a 2020 2020 2020    case 3:.      
-000031f0: 2020 2020 2020 2020 2020 2020 7362 702e              sbp.
-00003200: 736c 6963 655f 6465 6c28 293b 0a20 2020  slice_del();.   
-00003210: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00003220: 7265 616b 3b0a 2020 2020 2020 2020 2020  reak;.          
-00003230: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00003240: 2020 7d0a 2020 2020 2020 2020 2020 7d0a    }.          }.
-00003250: 2020 2020 2020 2020 2020 7468 6973 2e73            this.s
-00003260: 7465 6d20 3d20 6675 6e63 7469 6f6e 2829  tem = function()
-00003270: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
-00003280: 5f6d 6172 6b5f 7265 6769 6f6e 7328 293b  _mark_regions();
-00003290: 0a20 2020 2020 2020 2020 2020 2073 6270  .            sbp
-000032a0: 2e63 7572 736f 7220 3d20 7362 702e 6c69  .cursor = sbp.li
-000032b0: 6d69 743b 0a20 2020 2020 2020 2020 2020  mit;.           
-000032c0: 2069 6620 2873 6270 2e63 7572 736f 7220   if (sbp.cursor 
-000032d0: 3c20 495f 7056 290a 2020 2020 2020 2020  < I_pV).        
-000032e0: 2020 2020 2020 7265 7475 726e 2066 616c        return fal
-000032f0: 7365 3b0a 2020 2020 2020 2020 2020 2020  se;.            
-00003300: 7362 702e 6c69 6d69 745f 6261 636b 7761  sbp.limit_backwa
-00003310: 7264 203d 2049 5f70 563b 0a20 2020 2020  rd = I_pV;.     
-00003320: 2020 2020 2020 2069 6620 2821 725f 7065         if (!r_pe
-00003330: 7266 6563 7469 7665 5f67 6572 756e 6428  rfective_gerund(
-00003340: 2929 207b 0a20 2020 2020 2020 2020 2020  )) {.           
-00003350: 2020 2073 6270 2e63 7572 736f 7220 3d20     sbp.cursor = 
-00003360: 7362 702e 6c69 6d69 743b 0a20 2020 2020  sbp.limit;.     
-00003370: 2020 2020 2020 2020 2069 6620 2821 725f           if (!r_
-00003380: 7265 666c 6578 6976 6528 2929 0a20 2020  reflexive()).   
-00003390: 2020 2020 2020 2020 2020 2020 2073 6270               sbp
-000033a0: 2e63 7572 736f 7220 3d20 7362 702e 6c69  .cursor = sbp.li
-000033b0: 6d69 743b 0a20 2020 2020 2020 2020 2020  mit;.           
-000033c0: 2020 2069 6620 2821 725f 6164 6a65 6374     if (!r_adject
-000033d0: 6976 616c 2829 2920 7b0a 2020 2020 2020  ival()) {.      
-000033e0: 2020 2020 2020 2020 2020 7362 702e 6375            sbp.cu
-000033f0: 7273 6f72 203d 2073 6270 2e6c 696d 6974  rsor = sbp.limit
-00003400: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00003410: 2020 6966 2028 2172 5f76 6572 6228 2929    if (!r_verb())
-00003420: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00003430: 2020 2020 2073 6270 2e63 7572 736f 7220       sbp.cursor 
-00003440: 3d20 7362 702e 6c69 6d69 743b 0a20 2020  = sbp.limit;.   
-00003450: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003460: 5f6e 6f75 6e28 293b 0a20 2020 2020 2020  _noun();.       
-00003470: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003480: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003490: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000034a0: 2020 2020 2073 6270 2e63 7572 736f 7220       sbp.cursor 
-000034b0: 3d20 7362 702e 6c69 6d69 743b 0a20 2020  = sbp.limit;.   
-000034c0: 2020 2020 2020 2020 2073 6270 2e6b 6574           sbp.ket
-000034d0: 203d 2073 6270 2e63 7572 736f 723b 0a20   = sbp.cursor;. 
-000034e0: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-000034f0: 6270 2e65 715f 735f 6228 312c 2022 5c75  bp.eq_s_b(1, "\u
-00003500: 3034 3338 2229 2920 7b0a 2020 2020 2020  0438")) {.      
-00003510: 2020 2020 2020 2020 7362 702e 6272 6120          sbp.bra 
-00003520: 3d20 7362 702e 6375 7273 6f72 3b0a 2020  = sbp.cursor;.  
-00003530: 2020 2020 2020 2020 2020 2020 7362 702e              sbp.
-00003540: 736c 6963 655f 6465 6c28 293b 0a20 2020  slice_del();.   
-00003550: 2020 2020 2020 2020 207d 2065 6c73 650a           } else.
-00003560: 2020 2020 2020 2020 2020 2020 2020 7362                sb
-00003570: 702e 6375 7273 6f72 203d 2073 6270 2e6c  p.cursor = sbp.l
-00003580: 696d 6974 3b0a 2020 2020 2020 2020 2020  imit;.          
-00003590: 2020 725f 6465 7269 7661 7469 6f6e 616c    r_derivational
-000035a0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-000035b0: 7362 702e 6375 7273 6f72 203d 2073 6270  sbp.cursor = sbp
-000035c0: 2e6c 696d 6974 3b0a 2020 2020 2020 2020  .limit;.        
-000035d0: 2020 2020 725f 7469 6479 5f75 7028 293b      r_tidy_up();
-000035e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000035f0: 7572 6e20 7472 7565 3b0a 2020 2020 2020  urn true;.      
-00003600: 2020 2020 7d0a 2020 2020 2020 2020 7d3b      }.        };
-00003610: 0a0a 2020 2020 2020 2f2a 2061 6e64 2072  ..      /* and r
-00003620: 6574 7572 6e20 6120 6675 6e63 7469 6f6e  eturn a function
-00003630: 2074 6861 7420 7374 656d 7320 6120 776f   that stems a wo
-00003640: 7264 2066 6f72 2074 6865 2063 7572 7265  rd for the curre
-00003650: 6e74 206c 6f63 616c 6520 2a2f 0a20 2020  nt locale */.   
-00003660: 2020 2072 6574 7572 6e20 6675 6e63 7469     return functi
-00003670: 6f6e 2874 6f6b 656e 2920 7b0a 2020 2020  on(token) {.    
-00003680: 2020 2020 2f2f 2066 6f72 206c 756e 7220      // for lunr 
-00003690: 7665 7273 696f 6e20 320a 2020 2020 2020  version 2.      
-000036a0: 2020 6966 2028 7479 7065 6f66 2074 6f6b    if (typeof tok
-000036b0: 656e 2e75 7064 6174 6520 3d3d 3d20 2266  en.update === "f
-000036c0: 756e 6374 696f 6e22 2920 7b0a 2020 2020  unction") {.    
-000036d0: 2020 2020 2020 7265 7475 726e 2074 6f6b        return tok
-000036e0: 656e 2e75 7064 6174 6528 6675 6e63 7469  en.update(functi
-000036f0: 6f6e 2877 6f72 6429 207b 0a20 2020 2020  on(word) {.     
-00003700: 2020 2020 2020 2073 742e 7365 7443 7572         st.setCur
-00003710: 7265 6e74 2877 6f72 6429 3b0a 2020 2020  rent(word);.    
-00003720: 2020 2020 2020 2020 7374 2e73 7465 6d28          st.stem(
-00003730: 293b 0a20 2020 2020 2020 2020 2020 2072  );.            r
-00003740: 6574 7572 6e20 7374 2e67 6574 4375 7272  eturn st.getCurr
-00003750: 656e 7428 293b 0a20 2020 2020 2020 2020  ent();.         
-00003760: 207d 290a 2020 2020 2020 2020 7d20 656c   }).        } el
-00003770: 7365 207b 202f 2f20 666f 7220 6c75 6e72  se { // for lunr
-00003780: 2076 6572 7369 6f6e 203c 3d20 310a 2020   version <= 1.  
-00003790: 2020 2020 2020 2020 7374 2e73 6574 4375          st.setCu
-000037a0: 7272 656e 7428 746f 6b65 6e29 3b0a 2020  rrent(token);.  
-000037b0: 2020 2020 2020 2020 7374 2e73 7465 6d28          st.stem(
-000037c0: 293b 0a20 2020 2020 2020 2020 2072 6574  );.          ret
-000037d0: 7572 6e20 7374 2e67 6574 4375 7272 656e  urn st.getCurren
-000037e0: 7428 293b 0a20 2020 2020 2020 207d 0a20  t();.        }. 
-000037f0: 2020 2020 207d 0a20 2020 207d 2928 293b       }.    })();
-00003800: 0a0a 2020 2020 6c75 6e72 2e50 6970 656c  ..    lunr.Pipel
-00003810: 696e 652e 7265 6769 7374 6572 4675 6e63  ine.registerFunc
-00003820: 7469 6f6e 286c 756e 722e 7275 2e73 7465  tion(lunr.ru.ste
-00003830: 6d6d 6572 2c20 2773 7465 6d6d 6572 2d72  mmer, 'stemmer-r
-00003840: 7527 293b 0a0a 2020 2020 6c75 6e72 2e72  u');..    lunr.r
-00003850: 752e 7374 6f70 576f 7264 4669 6c74 6572  u.stopWordFilter
-00003860: 203d 206c 756e 722e 6765 6e65 7261 7465   = lunr.generate
-00003870: 5374 6f70 576f 7264 4669 6c74 6572 2827  StopWordFilter('
-00003880: d0b0 d0bb d0bb d0be 20d0 b1d0 b5d0 b720  ........ ...... 
-00003890: d0b1 d0bb d0b8 d0b7 d0ba d0be 20d0 b1d0  ............ ...
-000038a0: bed0 bbd0 b5d0 b520 d0b1 d0be d0bb d18c  ....... ........
-000038b0: d188 d0b5 20d0 b1d1 83d0 b4d0 b5d0 bc20  .... .......... 
-000038c0: d0b1 d183 d0b4 d0b5 d182 20d0 b1d1 83d0  .......... .....
-000038d0: b4d0 b5d1 82d0 b520 d0b1 d183 d0b4 d0b5  ....... ........
-000038e0: d188 d18c 20d0 b1d1 83d0 b4d1 82d0 be20  .... .......... 
-000038f0: d0b1 d183 d0b4 d183 20d0 b1d1 83d0 b4d1  ........ .......
-00003900: 83d1 8220 d0b1 d183 d0b4 d18c 20d0 b1d1  ... ........ ...
-00003910: 8b20 d0b1 d18b d0b2 d0b0 d0b5 d182 20d0  . ............ .
-00003920: b1d1 8bd0 b2d1 8c20 d0b1 d18b d0bb 20d0  ....... ...... .
-00003930: b1d1 8bd0 bbd0 b020 d0b1 d18b d0bb d0b8  ....... ........
-00003940: 20d0 b1d1 8bd0 bbd0 be20 d0b1 d18b d182   ........ ......
-00003950: d18c 20d0 b220 d0b2 d0b0 d0b6 d0bd d0b0  .. .. ..........
-00003960: d18f 20d0 b2d0 b0d0 b6d0 bdd0 bed0 b520  .. ............ 
-00003970: d0b2 d0b0 d0b6 d0bd d18b d0b5 20d0 b2d0  ............ ...
-00003980: b0d0 b6d0 bdd1 8bd0 b920 d0b2 d0b0 d0bc  ......... ......
-00003990: 20d0 b2d0 b0d0 bcd0 b820 d0b2 d0b0 d181   ........ ......
-000039a0: 20d0 b2d0 b0d1 8820 d0b2 d0b0 d188 d0b0   ...... ........
-000039b0: 20d0 b2d0 b0d1 88d0 b520 d0b2 d0b0 d188   ........ ......
-000039c0: d0b8 20d0 b2d0 b2d0 b5d1 80d1 8520 d0b2  .. .......... ..
-000039d0: d0b4 d0b0 d0bb d0b8 20d0 b2d0 b4d1 80d1  ........ .......
-000039e0: 83d0 b320 d0b2 d0b5 d0b4 d18c 20d0 b2d0  ... ........ ...
-000039f0: b5d0 b7d0 b4d0 b520 d0b2 d0b5 d181 d18c  ....... ........
-00003a00: 20d0 b2d0 bdd0 b8d0 b720 d0b2 d0bd d0b8   ........ ......
-00003a10: d0b7 d183 20d0 b2d0 be20 d0b2 d0be d0ba  .... .... ......
-00003a20: d180 d183 d0b3 20d0 b2d0 bed0 bd20 d0b2  ...... ...... ..
-00003a30: d0be d181 d0b5 d0bc d0bd d0b0 d0b4 d186  ................
-00003a40: d0b0 d182 d18b d0b9 20d0 b2d0 bed1 81d0  ........ .......
-00003a50: b5d0 bcd0 bdd0 b0d0 b4d1 86d0 b0d1 82d1  ................
-00003a60: 8c20 d0b2 d0be d181 d0b5 d0bc d18c 20d0  . ............ .
-00003a70: b2d0 bed1 81d1 8cd0 bcd0 bed0 b920 d0b2  ............. ..
-00003a80: d0be d182 20d0 b2d0 bfd1 80d0 bed1 87d0  .... ...........
-00003a90: b5d0 bc20 d0b2 d180 d0b5 d0bc d0b5 d0bd  ... ............
-00003aa0: d0b8 20d0 b2d1 80d0 b5d0 bcd1 8f20 d0b2  .. .......... ..
-00003ab0: d181 d0b5 20d0 b2d1 81d0 b5d0 b3d0 b4d0  .... ...........
-00003ac0: b020 d0b2 d181 d0b5 d0b3 d0be 20d0 b2d1  . .......... ...
-00003ad0: 81d0 b5d0 bc20 d0b2 d181 d0b5 d0bc d0b8  ..... ..........
-00003ae0: 20d0 b2d1 81d0 b5d0 bcd1 8320 d0b2 d181   .......... ....
-00003af0: d0b5 d185 20d0 b2d1 81d0 b5d1 8e20 d0b2  .... ........ ..
-00003b00: d181 d18e 20d0 b2d1 81d1 8ed0 b4d1 8320  .... .......... 
-00003b10: d0b2 d181 d18f 20d0 b2d1 81d1 9120 d0b2  ...... ...... ..
-00003b20: d182 d0be d180 d0be d0b9 20d0 b2d1 8b20  .......... .... 
-00003b30: d0b3 20d0 b3d0 b4d0 b520 d0b3 d0be d0b2  .. ...... ......
-00003b40: d0be d180 d0b8 d0bb 20d0 b3d0 bed0 b2d0  ........ .......
-00003b50: bed1 80d0 b8d1 8220 d0b3 d0be d0b4 20d0  ....... ...... .
-00003b60: b3d0 bed0 b4d0 b020 d0b3 d0be d0b4 d183  ....... ........
-00003b70: 20d0 b4d0 b020 d0b4 d0b0 d0b2 d0bd d0be   .... ..........
-00003b80: 20d0 b4d0 b0d0 b6d0 b520 d0b4 d0b0 d0bb   ........ ......
-00003b90: d0b5 d0ba d0be 20d0 b4d0 b0d0 bbd1 8cd1  ...... .........
-00003ba0: 88d0 b520 d0b4 d0b0 d180 d0be d0bc 20d0  ... .......... .
-00003bb0: b4d0 b2d0 b020 d0b4 d0b2 d0b0 d0b4 d186  ..... ..........
-00003bc0: d0b0 d182 d18b d0b9 20d0 b4d0 b2d0 b0d0  ........ .......
-00003bd0: b4d1 86d0 b0d1 82d1 8c20 d0b4 d0b2 d0b5  ......... ......
-00003be0: 20d0 b4d0 b2d0 b5d0 bdd0 b0d0 b4d1 86d0   ...............
-00003bf0: b0d1 82d1 8bd0 b920 d0b4 d0b2 d0b5 d0bd  ....... ........
-00003c00: d0b0 d0b4 d186 d0b0 d182 d18c 20d0 b4d0  ............ ...
-00003c10: b2d1 83d1 8520 d0b4 d0b5 d0b2 d18f d182  ..... ..........
-00003c20: d0bd d0b0 d0b4 d186 d0b0 d182 d18b d0b9  ................
-00003c30: 20d0 b4d0 b5d0 b2d1 8fd1 82d0 bdd0 b0d0   ...............
-00003c40: b4d1 86d0 b0d1 82d1 8c20 d0b4 d0b5 d0b2  ......... ......
-00003c50: d18f d182 d18b d0b9 20d0 b4d0 b5d0 b2d1  ........ .......
-00003c60: 8fd1 82d1 8c20 d0b4 d0b5 d0b9 d181 d182  ..... ..........
-00003c70: d0b2 d0b8 d182 d0b5 d0bb d18c d0bd d0be  ................
-00003c80: 20d0 b4d0 b5d0 bb20 d0b4 d0b5 d0bd d18c   ...... ........
-00003c90: 20d0 b4d0 b5d1 81d1 8fd1 82d1 8bd0 b920   .............. 
-00003ca0: d0b4 d0b5 d181 d18f d182 d18c 20d0 b4d0  ............ ...
-00003cb0: bbd1 8f20 d0b4 d0be 20d0 b4d0 bed0 b2d0  ... .... .......
-00003cc0: bed0 bbd1 8cd0 bdd0 be20 d0b4 d0be d0bb  ......... ......
-00003cd0: d0b3 d0be 20d0 b4d0 bed0 bbd0 b6d0 bdd0  .... ...........
-00003ce0: be20 d0b4 d180 d183 d0b3 d0b0 d18f 20d0  . ............ .
-00003cf0: b4d1 80d1 83d0 b3d0 b8d0 b520 d0b4 d180  ........... ....
-00003d00: d183 d0b3 d0b8 d185 20d0 b4d1 80d1 83d0  ........ .......
-00003d10: b3d0 be20 d0b4 d180 d183 d0b3 d0be d0b5  ... ............
-00003d20: 20d0 b4d1 80d1 83d0 b3d0 bed0 b920 d0b5   ............ ..
-00003d30: 20d0 b5d0 b3d0 be20 d0b5 d0b5 20d0 b5d0   ...... .... ...
-00003d40: b920 d0b5 d0bc d183 20d0 b5d1 81d0 bbd0  . ...... .......
-00003d50: b820 d0b5 d181 d182 d18c 20d0 b5d1 89d0  . ........ .....
-00003d60: b520 d0b5 d189 d191 20d0 b5d1 8e20 d0b5  . ...... .... ..
-00003d70: d191 20d0 b620 d0b6 d0b5 20d0 b6d0 b8d0  .. .. .... .....
-00003d80: b7d0 bdd1 8c20 d0b7 d0b0 20d0 b7d0 b0d0  ..... .... .....
-00003d90: bdd1 8fd1 8220 d0b7 d0b0 d0bd d18f d182  ..... ..........
-00003da0: d0b0 20d0 b7d0 b0d0 bdd1 8fd1 82d0 be20  .. ............ 
-00003db0: d0b7 d0b0 d0bd d18f d182 d18b 20d0 b7d0  ............ ...
-00003dc0: b0d1 82d0 b5d0 bc20 d0b7 d0b0 d182 d0be  ....... ........
-00003dd0: 20d0 b7d0 b0d1 87d0 b5d0 bc20 d0b7 d0b4   .......... ....
-00003de0: d0b5 d181 d18c 20d0 b7d0 bdd0 b0d1 87d0  ...... .........
-00003df0: b8d1 8220 d0b8 20d0 b8d0 b720 d0b8 d0bb  ... .. .... ....
-00003e00: d0b8 20d0 b8d0 bc20 d0b8 d0bc d0b5 d0bd  .. .... ........
-00003e10: d0bd d0be 20d0 b8d0 bcd0 b5d1 82d1 8c20  .... .......... 
-00003e20: d0b8 d0bc d0b8 20d0 b8d0 bcd1 8f20 d0b8  ...... ...... ..
-00003e30: d0bd d0be d0b3 d0b4 d0b0 20d0 b8d1 8520  .......... .... 
-00003e40: d0ba 20d0 bad0 b0d0 b6d0 b4d0 b0d1 8f20  .. ............ 
-00003e50: d0ba d0b0 d0b6 d0b4 d0be d0b5 20d0 bad0  ............ ...
-00003e60: b0d0 b6d0 b4d1 8bd0 b520 d0ba d0b0 d0b6  ......... ......
-00003e70: d0b4 d18b d0b9 20d0 bad0 b0d0 b6d0 b5d1  ...... .........
-00003e80: 82d1 81d1 8f20 d0ba d0b0 d0ba 20d0 bad0  ..... ...... ...
-00003e90: b0d0 bad0 b0d1 8f20 d0ba d0b0 d0ba d0be  ....... ........
-00003ea0: d0b9 20d0 bad0 b5d0 bc20 d0ba d0be d0b3  .. ...... ......
-00003eb0: d0b4 d0b0 20d0 bad0 bed0 b3d0 be20 d0ba  .... ........ ..
-00003ec0: d0be d0bc 20d0 bad0 bed0 bcd1 8320 d0ba  .... ........ ..
-00003ed0: d0be d0bd d0b5 d187 d0bd d0be 20d0 bad0  ............ ...
-00003ee0: bed1 82d0 bed1 80d0 b0d1 8f20 d0ba d0be  ........... ....
-00003ef0: d182 d0be d180 d0be d0b3 d0be 20d0 bad0  ............ ...
-00003f00: bed1 82d0 bed1 80d0 bed0 b920 d0ba d0be  ........... ....
-00003f10: d182 d0be d180 d18b d0b5 20d0 bad0 bed1  .......... .....
-00003f20: 82d0 bed1 80d1 8bd0 b920 d0ba d0be d182  ......... ......
-00003f30: d0be d180 d18b d185 20d0 bad1 80d0 bed0  ........ .......
-00003f40: bcd0 b520 d0ba d180 d183 d0b3 d0be d0bc  ... ............
-00003f50: 20d0 bad1 82d0 be20 d0ba d183 d0b4 d0b0   ...... ........
-00003f60: 20d0 bbd0 b5d1 8220 d0bb d0b8 20d0 bbd0   ...... .... ...
-00003f70: b8d1 88d1 8c20 d0bb d183 d187 d188 d0b5  ..... ..........
-00003f80: 20d0 bbd1 8ed0 b4d0 b820 d0bc 20d0 bcd0   ........ .. ...
-00003f90: b0d0 bbd0 be20 d0bc d0b5 d0b6 d0b4 d183  ..... ..........
-00003fa0: 20d0 bcd0 b5d0 bbd1 8f20 d0bc d0b5 d0bd   ........ ......
-00003fb0: d0b5 d0b5 20d0 bcd0 b5d0 bdd1 8cd1 88d0  .... ...........
-00003fc0: b520 d0bc d0b5 d0bd d18f 20d0 bcd0 b8d0  . ........ .....
-00003fd0: bbd0 bbd0 b8d0 bed0 bdd0 bed0 b220 d0bc  ............. ..
-00003fe0: d0b8 d0bc d0be 20d0 bcd0 b8d1 80d0 b020  ...... ........ 
-00003ff0: d0bc d0bd d0b5 20d0 bcd0 bdd0 bed0 b3d0  ...... .........
-00004000: be20 d0bc d0bd d0be d0b3 d0be d187 d0b8  . ..............
-00004010: d181 d0bb d0b5 d0bd d0bd d0b0 d18f 20d0  .............. .
-00004020: bcd0 bdd0 bed0 b3d0 bed1 87d0 b8d1 81d0  ................
-00004030: bbd0 b5d0 bdd0 bdd0 bed0 b520 d0bc d0bd  ........... ....
-00004040: d0be d0b3 d0be d187 d0b8 d181 d0bb d0b5  ................
-00004050: d0bd d0bd d18b d0b5 20d0 bcd0 bdd0 bed0  ........ .......
-00004060: b3d0 bed1 87d0 b8d1 81d0 bbd0 b5d0 bdd0  ................
-00004070: bdd1 8bd0 b920 d0bc d0bd d0be d0b9 20d0  ..... ........ .
-00004080: bcd0 bdd0 bed1 8e20 d0bc d0be d0b3 20d0  ....... ...... .
-00004090: bcd0 bed0 b3d1 83d1 8220 d0bc d0be d0b6  ......... ......
-000040a0: 20d0 bcd0 bed0 b6d0 b5d1 8220 d0bc d0be   .......... ....
-000040b0: d0b6 d0bd d0be 20d0 bcd0 bed0 b6d1 85d0  ...... .........
-000040c0: be20 d0bc d0be d0b8 20d0 bcd0 bed0 b920  . ...... ...... 
-000040d0: d0bc d0be d180 20d0 bcd0 bed1 87d1 8c20  ...... ........ 
-000040e0: d0bc d0be d18f 20d0 bcd0 bed1 9120 d0bc  ...... ...... ..
-000040f0: d18b 20d0 bdd0 b020 d0bd d0b0 d0b2 d0b5  .. .... ........
-00004100: d180 d185 d183 20d0 bdd0 b0d0 b420 d0bd  ...... ...... ..
-00004110: d0b0 d0b4 d0be 20d0 bdd0 b0d0 b7d0 b0d0  ...... .........
-00004120: b420 d0bd d0b0 d0b8 d0b1 d0be d0bb d0b5  . ..............
-00004130: d0b5 20d0 bdd0 b0d0 bad0 bed0 bdd0 b5d1  .. .............
-00004140: 8620 d0bd d0b0 d0bc 20d0 bdd0 b0d0 bcd0  . ...... .......
-00004150: b820 d0bd d0b0 d181 20d0 bdd0 b0d1 87d0  . ...... .......
-00004160: b0d0 bbd0 b020 d0bd d0b0 d188 20d0 bdd0  ..... ...... ...
-00004170: b0d1 88d0 b020 d0bd d0b0 d188 d0b5 20d0  ..... ........ .
-00004180: bdd0 b0d1 88d0 b820 d0bd d0b5 20d0 bdd0  ....... .... ...
-00004190: b5d0 b3d0 be20 d0bd d0b5 d0b4 d0b0 d0b2  ..... ..........
-000041a0: d0bd d0be 20d0 bdd0 b5d0 b4d0 b0d0 bbd0  .... ...........
-000041b0: b5d0 bad0 be20 d0bd d0b5 d0b5 20d0 bdd0  ..... ...... ...
-000041c0: b5d0 b920 d0bd d0b5 d0bb d18c d0b7 d18f  ... ............
-000041d0: 20d0 bdd0 b5d0 bc20 d0bd d0b5 d0bc d0bd   ...... ........
-000041e0: d0be d0b3 d0be 20d0 bdd0 b5d0 bcd1 8320  ...... ........ 
-000041f0: d0bd d0b5 d0bf d180 d0b5 d180 d18b d0b2  ................
-00004200: d0bd d0be 20d0 bdd0 b5d1 80d0 b5d0 b4d0  .... ...........
-00004210: bad0 be20 d0bd d0b5 d181 d0ba d0be d0bb  ... ............
-00004220: d18c d0ba d0be 20d0 bdd0 b5d1 8220 d0bd  ...... ...... ..
-00004230: d0b5 d18e 20d0 bdd0 b5d1 9120 d0bd d0b8  .... ...... ....
-00004240: 20d0 bdd0 b8d0 b1d1 83d0 b4d1 8c20 d0bd   ............ ..
-00004250: d0b8 d0b6 d0b5 20d0 bdd0 b8d0 b7d0 bad0  ...... .........
-00004260: be20 d0bd d0b8 d0ba d0be d0b3 d0b4 d0b0  . ..............
-00004270: 20d0 bdd0 b8d0 bad1 83d0 b4d0 b020 d0bd   ............ ..
-00004280: d0b8 d0bc d0b8 20d0 bdd0 b8d1 8520 d0bd  ...... ...... ..
-00004290: d0b8 d187 d0b5 d0b3 d0be 20d0 bdd0 be20  .......... .... 
-000042a0: d0bd d183 20d0 bdd1 83d0 b6d0 bdd0 be20  .... .......... 
-000042b0: d0bd d185 20d0 be20 d0be d0b1 20d0 bed0  .... .. .... ...
-000042c0: b1d0 b020 d0be d0b1 d18b d187 d0bd d0be  ... ............
-000042d0: 20d0 bed0 b4d0 b8d0 bd20 d0be d0b4 d0b8   ........ ......
-000042e0: d0bd d0bd d0b0 d0b4 d186 d0b0 d182 d18b  ................
-000042f0: d0b9 20d0 bed0 b4d0 b8d0 bdd0 bdd0 b0d0  .. .............
-00004300: b4d1 86d0 b0d1 82d1 8c20 d0be d0b4 d0bd  ......... ......
-00004310: d0b0 d0b6 d0b4 d18b 20d0 bed0 b4d0 bdd0  ........ .......
-00004320: b0d0 bad0 be20 d0be d0b4 d0bd d0be d0b3  ..... ..........
-00004330: d0be 20d0 bed0 b4d0 bdd0 bed0 b920 d0be  .. .......... ..
-00004340: d0ba d0be d0bb d0be 20d0 bed0 bd20 d0be  ........ .... ..
-00004350: d0bd d0b0 20d0 bed0 bdd0 b820 d0be d0bd  .... ...... ....
-00004360: d0be 20d0 bed0 bfd1 8fd1 82d1 8c20 d0be  .. .......... ..
-00004370: d181 d0be d0b1 d0b5 d0bd d0bd d0be 20d0  .............. .
-00004380: bed1 8220 d0be d182 d0be d0b2 d181 d18e  ... ............
-00004390: d0b4 d183 20d0 bed1 82d1 81d1 8ed0 b4d0  .... ...........
-000043a0: b020 d0be d187 d0b5 d0bd d18c 20d0 bfd0  . .......... ...
-000043b0: b5d1 80d0 b2d1 8bd0 b920 d0bf d0b5 d180  ......... ......
-000043c0: d0b5 d0b4 20d0 bfd0 be20 d0bf d0be d0b4  .... .... ......
-000043d0: 20d0 bfd0 bed0 b6d0 b0d0 bbd1 83d0 b9d1   ...............
-000043e0: 81d1 82d0 b020 d0bf d0be d0b7 d0b6 d0b5  ..... ..........
-000043f0: 20d0 bfd0 bed0 bad0 b020 d0bf d0be d180   ........ ......
-00004400: 20d0 bfd0 bed1 80d0 b020 d0bf d0be d181   ........ ......
-00004410: d0bb d0b5 20d0 bfd0 bed1 81d1 80d0 b5d0  .... ...........
-00004420: b4d0 b820 d0bf d0be d182 d0be d0bc 20d0  ... .......... .
-00004430: bfd0 bed1 82d0 bed0 bcd1 8320 d0bf d0be  ........... ....
-00004440: d187 d0b5 d0bc d183 20d0 bfd0 bed1 87d1  ........ .......
-00004450: 82d0 b820 d0bf d180 d0b5 d0ba d180 d0b0  ... ............
-00004460: d181 d0bd d0be 20d0 bfd1 80d0 b820 d0bf  ...... ...... ..
-00004470: d180 d0be 20d0 bfd1 80d0 bed1 81d1 82d0  .... ...........
-00004480: be20 d0bf d180 d0be d182 d0b8 d0b2 20d0  . ............ .
-00004490: bfd1 80d0 bed1 86d0 b5d0 bdd1 82d0 bed0  ................
-000044a0: b220 d0bf d18f d182 d0bd d0b0 d0b4 d186  . ..............
-000044b0: d0b0 d182 d18b d0b9 20d0 bfd1 8fd1 82d0  ........ .......
-000044c0: bdd0 b0d0 b4d1 86d0 b0d1 82d1 8c20 d0bf  ............. ..
-000044d0: d18f d182 d18b d0b9 20d0 bfd1 8fd1 82d1  ........ .......
-000044e0: 8c20 d180 d0b0 d0b7 20d1 80d0 b0d0 b7d0  . ...... .......
-000044f0: b2d0 b520 d180 d0b0 d0bd d0be 20d1 80d0  ... ........ ...
-00004500: b0d0 bdd1 8cd1 88d0 b520 d180 d18f d0b4  ......... ......
-00004510: d0be d0bc 20d1 8120 d181 d0b0 d0bc 20d1  .... .. ...... .
-00004520: 81d0 b0d0 bcd0 b020 d181 d0b0 d0bc d0b8  ....... ........
-00004530: 20d1 81d0 b0d0 bcd0 b8d0 bc20 d181 d0b0   .......... ....
-00004540: d0bc d0b8 d0bc d0b8 20d1 81d0 b0d0 bcd0  ........ .......
-00004550: b8d1 8520 d181 d0b0 d0bc d0be 20d1 81d0  ... ........ ...
-00004560: b0d0 bcd0 bed0 b3d0 be20 d181 d0b0 d0bc  ......... ......
-00004570: d0be d0b9 20d1 81d0 b0d0 bcd0 bed0 bc20  .... .......... 
-00004580: d181 d0b0 d0bc d0be d0bc d183 20d1 81d0  ............ ...
-00004590: b0d0 bcd1 8320 d181 d0b2 d0be d0b5 20d1  ..... ........ .
-000045a0: 81d0 b2d0 bed0 b5d0 b3d0 be20 d181 d0b2  ........... ....
-000045b0: d0be d0b5 d0b9 20d1 81d0 b2d0 bed0 b820  ...... ........ 
-000045c0: d181 d0b2 d0be d0b8 d185 20d1 81d0 b2d0  .......... .....
-000045d0: bed1 8e20 d181 d0b5 d0b0 d0be d0b9 20d1  ... .......... .
-000045e0: 81d0 b5d0 b1d0 b520 d181 d0b5 d0b1 d18f  ....... ........
-000045f0: 20d1 81d0 b5d0 b3d0 bed0 b4d0 bdd1 8f20   .............. 
-00004600: d181 d0b5 d0b4 d18c d0bc d0be d0b9 20d1  .............. .
-00004610: 81d0 b5d0 b9d1 87d0 b0d1 8120 d181 d0b5  ........... ....
-00004620: d0bc d0bd d0b0 d0b4 d186 d0b0 d182 d18b  ................
-00004630: d0b9 20d1 81d0 b5d0 bcd0 bdd0 b0d0 b4d1  .. .............
-00004640: 86d0 b0d1 82d1 8c20 d181 d0b5 d0bc d18c  ....... ........
-00004650: 20d1 81d0 b8d1 8520 d181 d0ba d0b0 d0b7   ...... ........
-00004660: d0b0 d0bb 20d1 81d0 bad0 b0d0 b7d0 b0d0  .... ...........
-00004670: bbd0 b020 d181 d0ba d0b0 d0b7 d0b0 d182  ... ............
-00004680: d18c 20d1 81d0 bad0 bed0 bbd1 8cd0 bad0  .. .............
-00004690: be20 d181 d0bb d0b8 d188 d0ba d0be d0bc  . ..............
-000046a0: 20d1 81d0 bdd0 b0d1 87d0 b0d0 bbd0 b020   .............. 
-000046b0: d181 d0bd d0be d0b2 d0b0 20d1 81d0 be20  .......... .... 
-000046c0: d181 d0be d0b1 d0be d0b9 20d1 81d0 bed0  .......... .....
-000046d0: b1d0 bed1 8e20 d181 d0be d0b2 d181 d0b5  ..... ..........
-000046e0: d0bc 20d1 81d0 bfd0 b0d1 81d0 b8d0 b1d0  .. .............
-000046f0: be20 d181 d182 d0b0 d0bb 20d1 81d1 83d1  . ........ .....
-00004700: 82d1 8c20 d182 20d1 82d0 b020 d182 d0b0  ... .. .... ....
-00004710: d0ba 20d1 82d0 b0d0 bad0 b0d1 8f20 d182  .. .......... ..
-00004720: d0b0 d0ba d0b6 d0b5 20d1 82d0 b0d0 bad0  ........ .......
-00004730: b8d0 b520 d182 d0b0 d0ba d0be d0b5 20d1  ... .......... .
-00004740: 82d0 b0d0 bad0 bed0 b920 d182 d0b0 d0bc  ......... ......
-00004750: 20d1 82d0 b2d0 bed0 b920 d182 d0b2 d0be   ........ ......
-00004760: d18f 20d1 82d0 b2d0 bed1 9120 d182 d0b5  .. ........ ....
-00004770: 20d1 82d0 b5d0 b1d0 b520 d182 d0b5 d0b1   ........ ......
-00004780: d18f 20d1 82d0 b5d0 bc20 d182 d0b5 d0bc  .. ...... ......
-00004790: d0b8 20d1 82d0 b5d0 bfd0 b5d1 80d1 8c20  .. ............ 
-000047a0: d182 d0b5 d185 20d1 82d0 be20 d182 d0be  ...... .... ....
-000047b0: d0b1 d0be d0b9 20d1 82d0 bed0 b1d0 bed1  ...... .........
-000047c0: 8e20 d182 d0be d0b3 d0b4 d0b0 20d1 82d0  . .......... ...
-000047d0: bed0 b3d0 be20 d182 d0be d0b6 d0b5 20d1  ..... ........ .
-000047e0: 82d0 bed0 bbd1 8cd0 bad0 be20 d182 d0be  ........... ....
-000047f0: d0bc 20d1 82d0 bed0 bcd1 8320 d182 d0be  .. ........ ....
-00004800: d182 20d1 82d0 bed1 8e20 d182 d180 d0b5  .. ...... ......
-00004810: d182 d0b8 d0b9 20d1 82d1 80d0 b820 d182  ...... ...... ..
-00004820: d180 d0b8 d0bd d0b0 d0b4 d186 d0b0 d182  ................
-00004830: d18b d0b9 20d1 82d1 80d0 b8d0 bdd0 b0d0  .... ...........
-00004840: b4d1 86d0 b0d1 82d1 8c20 d182 d183 20d1  ......... .... .
-00004850: 82d1 83d0 b4d0 b020 d182 d183 d182 20d1  ....... ...... .
-00004860: 82d1 8b20 d182 d18b d181 d18f d187 20d1  ... .......... .
-00004870: 8320 d183 d0b6 20d1 83d0 b6d0 b520 d183  . .... ...... ..
-00004880: d0bc d0b5 d182 d18c 20d1 85d0 bed1 80d0  ........ .......
-00004890: bed1 88d0 be20 d185 d0be d182 d0b5 d182  ..... ..........
-000048a0: d18c 20d1 85d0 bed1 82d1 8c20 d185 d0be  .. ........ ....
-000048b0: d182 d18f 20d1 85d0 bed1 87d0 b5d1 88d1  .... ...........
-000048c0: 8c20 d187 d0b0 d181 d182 d0be 20d1 87d0  . .......... ...
-000048d0: b0d1 89d0 b520 d187 d0b5 d0b3 d0be 20d1  ..... ........ .
-000048e0: 87d0 b5d0 bbd0 bed0 b2d0 b5d0 ba20 d187  ............. ..
-000048f0: d0b5 d0bc 20d1 87d0 b5d0 bcd1 8320 d187  .... ........ ..
-00004900: d0b5 d180 d0b5 d0b7 20d1 87d0 b5d1 82d0  ........ .......
-00004910: b2d0 b5d1 80d1 82d1 8bd0 b920 d187 d0b5  ........... ....
-00004920: d182 d18b d180 d0b5 20d1 87d0 b5d1 82d1  ........ .......
-00004930: 8bd1 80d0 bdd0 b0d0 b4d1 86d0 b0d1 82d1  ................
-00004940: 8bd0 b920 d187 d0b5 d182 d18b d180 d0bd  ... ............
-00004950: d0b0 d0b4 d186 d0b0 d182 d18c 20d1 87d1  ............ ...
-00004960: 82d0 be20 d187 d182 d0be d0b1 20d1 87d1  ... ........ ...
-00004970: 82d0 bed0 b1d1 8b20 d187 d183 d182 d18c  ....... ........
-00004980: 20d1 88d0 b5d1 81d1 82d0 bdd0 b0d0 b4d1   ...............
-00004990: 86d0 b0d1 82d1 8bd0 b920 d188 d0b5 d181  ......... ......
-000049a0: d182 d0bd d0b0 d0b4 d186 d0b0 d182 d18c  ................
-000049b0: 20d1 88d0 b5d1 81d1 82d0 bed0 b920 d188   ............ ..
-000049c0: d0b5 d181 d182 d18c 20d1 8dd1 82d0 b020  ........ ...... 
-000049d0: d18d d182 d0b8 20d1 8dd1 82d0 b8d0 bc20  ...... ........ 
-000049e0: d18d d182 d0b8 d0bc d0b8 20d1 8dd1 82d0  .......... .....
-000049f0: b8d1 8520 d18d d182 d0be 20d1 8dd1 82d0  ... ...... .....
-00004a00: bed0 b3d0 be20 d18d d182 d0be d0b9 20d1  ..... ........ .
-00004a10: 8dd1 82d0 bed0 bc20 d18d d182 d0be d0bc  ....... ........
-00004a20: d183 20d1 8dd1 82d0 bed1 8220 d18d d182  .. ........ ....
-00004a30: d183 20d1 8f20 efbb bfd0 b027 2e73 706c  .. .. .....'.spl
-00004a40: 6974 2827 2027 2929 3b0a 0a20 2020 206c  it(' '));..    l
-00004a50: 756e 722e 5069 7065 6c69 6e65 2e72 6567  unr.Pipeline.reg
-00004a60: 6973 7465 7246 756e 6374 696f 6e28 6c75  isterFunction(lu
-00004a70: 6e72 2e72 752e 7374 6f70 576f 7264 4669  nr.ru.stopWordFi
-00004a80: 6c74 6572 2c20 2773 746f 7057 6f72 6446  lter, 'stopWordF
-00004a90: 696c 7465 722d 7275 2729 3b0a 2020 7d3b  ilter-ru');.  };
-00004aa0: 0a7d 2929                                .}))
+00002a00: 2020 6361 7365 2032 3a0a 2020 2020 2020    case 2:.      
+00002a10: 2020 2020 2020 2020 2020 2020 2020 7362                sb
+00002a20: 702e 736c 6963 655f 6465 6c28 293b 0a20  p.slice_del();. 
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2062 7265 616b 3b0a 2020 2020 2020     break;.      
+00002a50: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002a60: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00002a70: 7275 653b 0a20 2020 2020 2020 2020 2020  rue;.           
+00002a80: 207d 0a20 2020 2020 2020 2020 2020 2072   }.            r
+00002a90: 6574 7572 6e20 6661 6c73 653b 0a20 2020  eturn false;.   
+00002aa0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00002ab0: 2020 2020 6675 6e63 7469 6f6e 2072 5f70      function r_p
+00002ac0: 6572 6665 6374 6976 655f 6765 7275 6e64  erfective_gerund
+00002ad0: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
+00002ae0: 2072 6574 7572 6e20 6861 6272 3228 615f   return habr2(a_
+00002af0: 302c 2039 293b 0a20 2020 2020 2020 2020  0, 9);.         
+00002b00: 207d 0a0a 2020 2020 2020 2020 2020 6675   }..          fu
+00002b10: 6e63 7469 6f6e 2068 6162 7231 2861 2c20  nction habr1(a, 
+00002b20: 6e29 207b 0a20 2020 2020 2020 2020 2020  n) {.           
+00002b30: 2076 6172 2061 6d6f 6e67 5f76 6172 3b0a   var among_var;.
+00002b40: 2020 2020 2020 2020 2020 2020 7362 702e              sbp.
+00002b50: 6b65 7420 3d20 7362 702e 6375 7273 6f72  ket = sbp.cursor
+00002b60: 3b0a 2020 2020 2020 2020 2020 2020 616d  ;.            am
+00002b70: 6f6e 675f 7661 7220 3d20 7362 702e 6669  ong_var = sbp.fi
+00002b80: 6e64 5f61 6d6f 6e67 5f62 2861 2c20 6e29  nd_among_b(a, n)
+00002b90: 3b0a 2020 2020 2020 2020 2020 2020 6966  ;.            if
+00002ba0: 2028 616d 6f6e 675f 7661 7229 207b 0a20   (among_var) {. 
+00002bb0: 2020 2020 2020 2020 2020 2020 2073 6270               sbp
+00002bc0: 2e62 7261 203d 2073 6270 2e63 7572 736f  .bra = sbp.curso
+00002bd0: 723b 0a20 2020 2020 2020 2020 2020 2020  r;.             
+00002be0: 2069 6620 2861 6d6f 6e67 5f76 6172 203d   if (among_var =
+00002bf0: 3d20 3129 0a20 2020 2020 2020 2020 2020  = 1).           
+00002c00: 2020 2020 2073 6270 2e73 6c69 6365 5f64       sbp.slice_d
+00002c10: 656c 2829 3b0a 2020 2020 2020 2020 2020  el();.          
+00002c20: 2020 2020 7265 7475 726e 2074 7275 653b      return true;
+00002c30: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00002c40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002c50: 6e20 6661 6c73 653b 0a20 2020 2020 2020  n false;.       
+00002c60: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00002c70: 6675 6e63 7469 6f6e 2072 5f61 646a 6563  function r_adjec
+00002c80: 7469 7665 2829 207b 0a20 2020 2020 2020  tive() {.       
+00002c90: 2020 2020 2072 6574 7572 6e20 6861 6272       return habr
+00002ca0: 3128 615f 312c 2032 3629 3b0a 2020 2020  1(a_1, 26);.    
+00002cb0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00002cc0: 2020 2066 756e 6374 696f 6e20 725f 6164     function r_ad
+00002cd0: 6a65 6374 6976 616c 2829 207b 0a20 2020  jectival() {.   
+00002ce0: 2020 2020 2020 2020 2076 6172 2061 6d6f           var amo
+00002cf0: 6e67 5f76 6172 3b0a 2020 2020 2020 2020  ng_var;.        
+00002d00: 2020 2020 6966 2028 725f 6164 6a65 6374      if (r_adject
+00002d10: 6976 6528 2929 207b 0a20 2020 2020 2020  ive()) {.       
+00002d20: 2020 2020 2020 2068 6162 7232 2861 5f32         habr2(a_2
+00002d30: 2c20 3829 3b0a 2020 2020 2020 2020 2020  , 8);.          
+00002d40: 2020 2020 7265 7475 726e 2074 7275 653b      return true;
+00002d50: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00002d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002d70: 6e20 6661 6c73 653b 0a20 2020 2020 2020  n false;.       
+00002d80: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00002d90: 6675 6e63 7469 6f6e 2072 5f72 6566 6c65  function r_refle
+00002da0: 7869 7665 2829 207b 0a20 2020 2020 2020  xive() {.       
+00002db0: 2020 2020 2072 6574 7572 6e20 6861 6272       return habr
+00002dc0: 3128 615f 332c 2032 293b 0a20 2020 2020  1(a_3, 2);.     
+00002dd0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00002de0: 2020 6675 6e63 7469 6f6e 2072 5f76 6572    function r_ver
+00002df0: 6228 2920 7b0a 2020 2020 2020 2020 2020  b() {.          
+00002e00: 2020 7265 7475 726e 2068 6162 7232 2861    return habr2(a
+00002e10: 5f34 2c20 3436 293b 0a20 2020 2020 2020  _4, 46);.       
+00002e20: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00002e30: 6675 6e63 7469 6f6e 2072 5f6e 6f75 6e28  function r_noun(
+00002e40: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00002e50: 6861 6272 3128 615f 352c 2033 3629 3b0a  habr1(a_5, 36);.
+00002e60: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
+00002e70: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
+00002e80: 725f 6465 7269 7661 7469 6f6e 616c 2829  r_derivational()
+00002e90: 207b 0a20 2020 2020 2020 2020 2020 2076   {.            v
+00002ea0: 6172 2061 6d6f 6e67 5f76 6172 3b0a 2020  ar among_var;.  
+00002eb0: 2020 2020 2020 2020 2020 7362 702e 6b65            sbp.ke
+00002ec0: 7420 3d20 7362 702e 6375 7273 6f72 3b0a  t = sbp.cursor;.
+00002ed0: 2020 2020 2020 2020 2020 2020 616d 6f6e              amon
+00002ee0: 675f 7661 7220 3d20 7362 702e 6669 6e64  g_var = sbp.find
+00002ef0: 5f61 6d6f 6e67 5f62 2861 5f36 2c20 3229  _among_b(a_6, 2)
+00002f00: 3b0a 2020 2020 2020 2020 2020 2020 6966  ;.            if
+00002f10: 2028 616d 6f6e 675f 7661 7229 207b 0a20   (among_var) {. 
+00002f20: 2020 2020 2020 2020 2020 2020 2073 6270               sbp
+00002f30: 2e62 7261 203d 2073 6270 2e63 7572 736f  .bra = sbp.curso
+00002f40: 723b 0a20 2020 2020 2020 2020 2020 2020  r;.             
+00002f50: 2069 6620 2872 5f52 3228 2920 2626 2061   if (r_R2() && a
+00002f60: 6d6f 6e67 5f76 6172 203d 3d20 3129 0a20  mong_var == 1). 
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002f80: 6270 2e73 6c69 6365 5f64 656c 2829 3b0a  bp.slice_del();.
+00002f90: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00002fa0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00002fb0: 2020 2020 2066 756e 6374 696f 6e20 725f       function r_
+00002fc0: 7469 6479 5f75 7028 2920 7b0a 2020 2020  tidy_up() {.    
+00002fd0: 2020 2020 2020 2020 7661 7220 616d 6f6e          var amon
+00002fe0: 675f 7661 723b 0a20 2020 2020 2020 2020  g_var;.         
+00002ff0: 2020 2073 6270 2e6b 6574 203d 2073 6270     sbp.ket = sbp
+00003000: 2e63 7572 736f 723b 0a20 2020 2020 2020  .cursor;.       
+00003010: 2020 2020 2061 6d6f 6e67 5f76 6172 203d       among_var =
+00003020: 2073 6270 2e66 696e 645f 616d 6f6e 675f   sbp.find_among_
+00003030: 6228 615f 372c 2034 293b 0a20 2020 2020  b(a_7, 4);.     
+00003040: 2020 2020 2020 2069 6620 2861 6d6f 6e67         if (among
+00003050: 5f76 6172 2920 7b0a 2020 2020 2020 2020  _var) {.        
+00003060: 2020 2020 2020 7362 702e 6272 6120 3d20        sbp.bra = 
+00003070: 7362 702e 6375 7273 6f72 3b0a 2020 2020  sbp.cursor;.    
+00003080: 2020 2020 2020 2020 2020 7377 6974 6368            switch
+00003090: 2028 616d 6f6e 675f 7661 7229 207b 0a20   (among_var) {. 
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000030b0: 6173 6520 313a 0a20 2020 2020 2020 2020  ase 1:.         
+000030c0: 2020 2020 2020 2020 2073 6270 2e73 6c69           sbp.sli
+000030d0: 6365 5f64 656c 2829 3b0a 2020 2020 2020  ce_del();.      
+000030e0: 2020 2020 2020 2020 2020 2020 7362 702e              sbp.
+000030f0: 6b65 7420 3d20 7362 702e 6375 7273 6f72  ket = sbp.cursor
+00003100: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00003110: 2020 2020 6966 2028 2173 6270 2e65 715f      if (!sbp.eq_
+00003120: 735f 6228 312c 2022 5c75 3034 3344 2229  s_b(1, "\u043D")
+00003130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003140: 2020 2020 2020 6272 6561 6b3b 0a20 2020        break;.   
+00003150: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003160: 6270 2e62 7261 203d 2073 6270 2e63 7572  bp.bra = sbp.cur
+00003170: 736f 723b 0a20 2020 2020 2020 2020 2020  sor;.           
+00003180: 2020 2020 2063 6173 6520 323a 0a20 2020       case 2:.   
+00003190: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000031a0: 6620 2821 7362 702e 6571 5f73 5f62 2831  f (!sbp.eq_s_b(1
+000031b0: 2c20 225c 7530 3433 4422 2929 0a20 2020  , "\u043D")).   
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2062 7265 616b 3b0a 2020 2020 2020 2020   break;.        
+000031e0: 2020 2020 2020 2020 6361 7365 2033 3a0a          case 3:.
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 2020 7362 702e 736c 6963 655f 6465 6c28    sbp.slice_del(
+00003210: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00003220: 2020 2020 2062 7265 616b 3b0a 2020 2020       break;.    
+00003230: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003240: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003250: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00003260: 7468 6973 2e73 7465 6d20 3d20 6675 6e63  this.stem = func
+00003270: 7469 6f6e 2829 207b 0a20 2020 2020 2020  tion() {.       
+00003280: 2020 2020 2072 5f6d 6172 6b5f 7265 6769       r_mark_regi
+00003290: 6f6e 7328 293b 0a20 2020 2020 2020 2020  ons();.         
+000032a0: 2020 2073 6270 2e63 7572 736f 7220 3d20     sbp.cursor = 
+000032b0: 7362 702e 6c69 6d69 743b 0a20 2020 2020  sbp.limit;.     
+000032c0: 2020 2020 2020 2069 6620 2873 6270 2e63         if (sbp.c
+000032d0: 7572 736f 7220 3c20 495f 7056 290a 2020  ursor < I_pV).  
+000032e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000032f0: 726e 2066 616c 7365 3b0a 2020 2020 2020  rn false;.      
+00003300: 2020 2020 2020 7362 702e 6c69 6d69 745f        sbp.limit_
+00003310: 6261 636b 7761 7264 203d 2049 5f70 563b  backward = I_pV;
+00003320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003330: 2821 725f 7065 7266 6563 7469 7665 5f67  (!r_perfective_g
+00003340: 6572 756e 6428 2929 207b 0a20 2020 2020  erund()) {.     
+00003350: 2020 2020 2020 2020 2073 6270 2e63 7572           sbp.cur
+00003360: 736f 7220 3d20 7362 702e 6c69 6d69 743b  sor = sbp.limit;
+00003370: 0a20 2020 2020 2020 2020 2020 2020 2069  .              i
+00003380: 6620 2821 725f 7265 666c 6578 6976 6528  f (!r_reflexive(
+00003390: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000033a0: 2020 2073 6270 2e63 7572 736f 7220 3d20     sbp.cursor = 
+000033b0: 7362 702e 6c69 6d69 743b 0a20 2020 2020  sbp.limit;.     
+000033c0: 2020 2020 2020 2020 2069 6620 2821 725f           if (!r_
+000033d0: 6164 6a65 6374 6976 616c 2829 2920 7b0a  adjectival()) {.
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 7362 702e 6375 7273 6f72 203d 2073 6270  sbp.cursor = sbp
+00003400: 2e6c 696d 6974 3b0a 2020 2020 2020 2020  .limit;.        
+00003410: 2020 2020 2020 2020 6966 2028 2172 5f76          if (!r_v
+00003420: 6572 6228 2929 207b 0a20 2020 2020 2020  erb()) {.       
+00003430: 2020 2020 2020 2020 2020 2073 6270 2e63             sbp.c
+00003440: 7572 736f 7220 3d20 7362 702e 6c69 6d69  ursor = sbp.limi
+00003450: 743b 0a20 2020 2020 2020 2020 2020 2020  t;.             
+00003460: 2020 2020 2072 5f6e 6f75 6e28 293b 0a20       r_noun();. 
+00003470: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00003480: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
+00003490: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+000034a0: 2020 2020 2020 2020 2020 2073 6270 2e63             sbp.c
+000034b0: 7572 736f 7220 3d20 7362 702e 6c69 6d69  ursor = sbp.limi
+000034c0: 743b 0a20 2020 2020 2020 2020 2020 2073  t;.            s
+000034d0: 6270 2e6b 6574 203d 2073 6270 2e63 7572  bp.ket = sbp.cur
+000034e0: 736f 723b 0a20 2020 2020 2020 2020 2020  sor;.           
+000034f0: 2069 6620 2873 6270 2e65 715f 735f 6228   if (sbp.eq_s_b(
+00003500: 312c 2022 5c75 3034 3338 2229 2920 7b0a  1, "\u0438")) {.
+00003510: 2020 2020 2020 2020 2020 2020 2020 7362                sb
+00003520: 702e 6272 6120 3d20 7362 702e 6375 7273  p.bra = sbp.curs
+00003530: 6f72 3b0a 2020 2020 2020 2020 2020 2020  or;.            
+00003540: 2020 7362 702e 736c 6963 655f 6465 6c28    sbp.slice_del(
+00003550: 293b 0a20 2020 2020 2020 2020 2020 207d  );.            }
+00003560: 2065 6c73 650a 2020 2020 2020 2020 2020   else.          
+00003570: 2020 2020 7362 702e 6375 7273 6f72 203d      sbp.cursor =
+00003580: 2073 6270 2e6c 696d 6974 3b0a 2020 2020   sbp.limit;.    
+00003590: 2020 2020 2020 2020 725f 6465 7269 7661          r_deriva
+000035a0: 7469 6f6e 616c 2829 3b0a 2020 2020 2020  tional();.      
+000035b0: 2020 2020 2020 7362 702e 6375 7273 6f72        sbp.cursor
+000035c0: 203d 2073 6270 2e6c 696d 6974 3b0a 2020   = sbp.limit;.  
+000035d0: 2020 2020 2020 2020 2020 725f 7469 6479            r_tidy
+000035e0: 5f75 7028 293b 0a20 2020 2020 2020 2020  _up();.         
+000035f0: 2020 2072 6574 7572 6e20 7472 7565 3b0a     return true;.
+00003600: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003610: 2020 2020 7d3b 0a0a 2020 2020 2020 2f2a      };..      /*
+00003620: 2061 6e64 2072 6574 7572 6e20 6120 6675   and return a fu
+00003630: 6e63 7469 6f6e 2074 6861 7420 7374 656d  nction that stem
+00003640: 7320 6120 776f 7264 2066 6f72 2074 6865  s a word for the
+00003650: 2063 7572 7265 6e74 206c 6f63 616c 6520   current locale 
+00003660: 2a2f 0a20 2020 2020 2072 6574 7572 6e20  */.      return 
+00003670: 6675 6e63 7469 6f6e 2874 6f6b 656e 2920  function(token) 
+00003680: 7b0a 2020 2020 2020 2020 2f2f 2066 6f72  {.        // for
+00003690: 206c 756e 7220 7665 7273 696f 6e20 320a   lunr version 2.
+000036a0: 2020 2020 2020 2020 6966 2028 7479 7065          if (type
+000036b0: 6f66 2074 6f6b 656e 2e75 7064 6174 6520  of token.update 
+000036c0: 3d3d 3d20 2266 756e 6374 696f 6e22 2920  === "function") 
+000036d0: 7b0a 2020 2020 2020 2020 2020 7265 7475  {.          retu
+000036e0: 726e 2074 6f6b 656e 2e75 7064 6174 6528  rn token.update(
+000036f0: 6675 6e63 7469 6f6e 2877 6f72 6429 207b  function(word) {
+00003700: 0a20 2020 2020 2020 2020 2020 2073 742e  .            st.
+00003710: 7365 7443 7572 7265 6e74 2877 6f72 6429  setCurrent(word)
+00003720: 3b0a 2020 2020 2020 2020 2020 2020 7374  ;.            st
+00003730: 2e73 7465 6d28 293b 0a20 2020 2020 2020  .stem();.       
+00003740: 2020 2020 2072 6574 7572 6e20 7374 2e67       return st.g
+00003750: 6574 4375 7272 656e 7428 293b 0a20 2020  etCurrent();.   
+00003760: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
+00003770: 2020 7d20 656c 7365 207b 202f 2f20 666f    } else { // fo
+00003780: 7220 6c75 6e72 2076 6572 7369 6f6e 203c  r lunr version <
+00003790: 3d20 310a 2020 2020 2020 2020 2020 7374  = 1.          st
+000037a0: 2e73 6574 4375 7272 656e 7428 746f 6b65  .setCurrent(toke
+000037b0: 6e29 3b0a 2020 2020 2020 2020 2020 7374  n);.          st
+000037c0: 2e73 7465 6d28 293b 0a20 2020 2020 2020  .stem();.       
+000037d0: 2020 2072 6574 7572 6e20 7374 2e67 6574     return st.get
+000037e0: 4375 7272 656e 7428 293b 0a20 2020 2020  Current();.     
+000037f0: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
+00003800: 207d 2928 293b 0a0a 2020 2020 6c75 6e72   })();..    lunr
+00003810: 2e50 6970 656c 696e 652e 7265 6769 7374  .Pipeline.regist
+00003820: 6572 4675 6e63 7469 6f6e 286c 756e 722e  erFunction(lunr.
+00003830: 7275 2e73 7465 6d6d 6572 2c20 2773 7465  ru.stemmer, 'ste
+00003840: 6d6d 6572 2d72 7527 293b 0a0a 2020 2020  mmer-ru');..    
+00003850: 6c75 6e72 2e72 752e 7374 6f70 576f 7264  lunr.ru.stopWord
+00003860: 4669 6c74 6572 203d 206c 756e 722e 6765  Filter = lunr.ge
+00003870: 6e65 7261 7465 5374 6f70 576f 7264 4669  nerateStopWordFi
+00003880: 6c74 6572 2827 d0b0 d0bb d0bb d0be 20d0  lter('........ .
+00003890: b1d0 b5d0 b720 d0b1 d0bb d0b8 d0b7 d0ba  ..... ..........
+000038a0: d0be 20d0 b1d0 bed0 bbd0 b5d0 b520 d0b1  .. .......... ..
+000038b0: d0be d0bb d18c d188 d0b5 20d0 b1d1 83d0  .......... .....
+000038c0: b4d0 b5d0 bc20 d0b1 d183 d0b4 d0b5 d182  ..... ..........
+000038d0: 20d0 b1d1 83d0 b4d0 b5d1 82d0 b520 d0b1   ............ ..
+000038e0: d183 d0b4 d0b5 d188 d18c 20d0 b1d1 83d0  .......... .....
+000038f0: b4d1 82d0 be20 d0b1 d183 d0b4 d183 20d0  ..... ........ .
+00003900: b1d1 83d0 b4d1 83d1 8220 d0b1 d183 d0b4  ......... ......
+00003910: d18c 20d0 b1d1 8b20 d0b1 d18b d0b2 d0b0  .. .... ........
+00003920: d0b5 d182 20d0 b1d1 8bd0 b2d1 8c20 d0b1  .... ........ ..
+00003930: d18b d0bb 20d0 b1d1 8bd0 bbd0 b020 d0b1  .... ........ ..
+00003940: d18b d0bb d0b8 20d0 b1d1 8bd0 bbd0 be20  ...... ........ 
+00003950: d0b1 d18b d182 d18c 20d0 b220 d0b2 d0b0  ........ .. ....
+00003960: d0b6 d0bd d0b0 d18f 20d0 b2d0 b0d0 b6d0  ........ .......
+00003970: bdd0 bed0 b520 d0b2 d0b0 d0b6 d0bd d18b  ..... ..........
+00003980: d0b5 20d0 b2d0 b0d0 b6d0 bdd1 8bd0 b920  .. ............ 
+00003990: d0b2 d0b0 d0bc 20d0 b2d0 b0d0 bcd0 b820  ...... ........ 
+000039a0: d0b2 d0b0 d181 20d0 b2d0 b0d1 8820 d0b2  ...... ...... ..
+000039b0: d0b0 d188 d0b0 20d0 b2d0 b0d1 88d0 b520  ...... ........ 
+000039c0: d0b2 d0b0 d188 d0b8 20d0 b2d0 b2d0 b5d1  ........ .......
+000039d0: 80d1 8520 d0b2 d0b4 d0b0 d0bb d0b8 20d0  ... .......... .
+000039e0: b2d0 b4d1 80d1 83d0 b320 d0b2 d0b5 d0b4  ......... ......
+000039f0: d18c 20d0 b2d0 b5d0 b7d0 b4d0 b520 d0b2  .. .......... ..
+00003a00: d0b5 d181 d18c 20d0 b2d0 bdd0 b8d0 b720  ...... ........ 
+00003a10: d0b2 d0bd d0b8 d0b7 d183 20d0 b2d0 be20  .......... .... 
+00003a20: d0b2 d0be d0ba d180 d183 d0b3 20d0 b2d0  ............ ...
+00003a30: bed0 bd20 d0b2 d0be d181 d0b5 d0bc d0bd  ... ............
+00003a40: d0b0 d0b4 d186 d0b0 d182 d18b d0b9 20d0  .............. .
+00003a50: b2d0 bed1 81d0 b5d0 bcd0 bdd0 b0d0 b4d1  ................
+00003a60: 86d0 b0d1 82d1 8c20 d0b2 d0be d181 d0b5  ....... ........
+00003a70: d0bc d18c 20d0 b2d0 bed1 81d1 8cd0 bcd0  .... ...........
+00003a80: bed0 b920 d0b2 d0be d182 20d0 b2d0 bfd1  ... ...... .....
+00003a90: 80d0 bed1 87d0 b5d0 bc20 d0b2 d180 d0b5  ......... ......
+00003aa0: d0bc d0b5 d0bd d0b8 20d0 b2d1 80d0 b5d0  ........ .......
+00003ab0: bcd1 8f20 d0b2 d181 d0b5 20d0 b2d1 81d0  ... ...... .....
+00003ac0: b5d0 b3d0 b4d0 b020 d0b2 d181 d0b5 d0b3  ....... ........
+00003ad0: d0be 20d0 b2d1 81d0 b5d0 bc20 d0b2 d181  .. ........ ....
+00003ae0: d0b5 d0bc d0b8 20d0 b2d1 81d0 b5d0 bcd1  ...... .........
+00003af0: 8320 d0b2 d181 d0b5 d185 20d0 b2d1 81d0  . ........ .....
+00003b00: b5d1 8e20 d0b2 d181 d18e 20d0 b2d1 81d1  ... ...... .....
+00003b10: 8ed0 b4d1 8320 d0b2 d181 d18f 20d0 b2d1  ..... ...... ...
+00003b20: 81d1 9120 d0b2 d182 d0be d180 d0be d0b9  ... ............
+00003b30: 20d0 b2d1 8b20 d0b3 20d0 b3d0 b4d0 b520   .... .. ...... 
+00003b40: d0b3 d0be d0b2 d0be d180 d0b8 d0bb 20d0  .............. .
+00003b50: b3d0 bed0 b2d0 bed1 80d0 b8d1 8220 d0b3  ............. ..
+00003b60: d0be d0b4 20d0 b3d0 bed0 b4d0 b020 d0b3  .... ........ ..
+00003b70: d0be d0b4 d183 20d0 b4d0 b020 d0b4 d0b0  ...... .... ....
+00003b80: d0b2 d0bd d0be 20d0 b4d0 b0d0 b6d0 b520  ...... ........ 
+00003b90: d0b4 d0b0 d0bb d0b5 d0ba d0be 20d0 b4d0  ............ ...
+00003ba0: b0d0 bbd1 8cd1 88d0 b520 d0b4 d0b0 d180  ......... ......
+00003bb0: d0be d0bc 20d0 b4d0 b2d0 b020 d0b4 d0b2  .... ...... ....
+00003bc0: d0b0 d0b4 d186 d0b0 d182 d18b d0b9 20d0  .............. .
+00003bd0: b4d0 b2d0 b0d0 b4d1 86d0 b0d1 82d1 8c20  ............... 
+00003be0: d0b4 d0b2 d0b5 20d0 b4d0 b2d0 b5d0 bdd0  ...... .........
+00003bf0: b0d0 b4d1 86d0 b0d1 82d1 8bd0 b920 d0b4  ............. ..
+00003c00: d0b2 d0b5 d0bd d0b0 d0b4 d186 d0b0 d182  ................
+00003c10: d18c 20d0 b4d0 b2d1 83d1 8520 d0b4 d0b5  .. ........ ....
+00003c20: d0b2 d18f d182 d0bd d0b0 d0b4 d186 d0b0  ................
+00003c30: d182 d18b d0b9 20d0 b4d0 b5d0 b2d1 8fd1  ...... .........
+00003c40: 82d0 bdd0 b0d0 b4d1 86d0 b0d1 82d1 8c20  ............... 
+00003c50: d0b4 d0b5 d0b2 d18f d182 d18b d0b9 20d0  .............. .
+00003c60: b4d0 b5d0 b2d1 8fd1 82d1 8c20 d0b4 d0b5  ........... ....
+00003c70: d0b9 d181 d182 d0b2 d0b8 d182 d0b5 d0bb  ................
+00003c80: d18c d0bd d0be 20d0 b4d0 b5d0 bb20 d0b4  ...... ...... ..
+00003c90: d0b5 d0bd d18c 20d0 b4d0 b5d1 81d1 8fd1  ...... .........
+00003ca0: 82d1 8bd0 b920 d0b4 d0b5 d181 d18f d182  ..... ..........
+00003cb0: d18c 20d0 b4d0 bbd1 8f20 d0b4 d0be 20d0  .. ...... .... .
+00003cc0: b4d0 bed0 b2d0 bed0 bbd1 8cd0 bdd0 be20  ............... 
+00003cd0: d0b4 d0be d0bb d0b3 d0be 20d0 b4d0 bed0  .......... .....
+00003ce0: bbd0 b6d0 bdd0 be20 d0b4 d180 d183 d0b3  ....... ........
+00003cf0: d0b0 d18f 20d0 b4d1 80d1 83d0 b3d0 b8d0  .... ...........
+00003d00: b520 d0b4 d180 d183 d0b3 d0b8 d185 20d0  . ............ .
+00003d10: b4d1 80d1 83d0 b3d0 be20 d0b4 d180 d183  ......... ......
+00003d20: d0b3 d0be d0b5 20d0 b4d1 80d1 83d0 b3d0  ...... .........
+00003d30: bed0 b920 d0b5 20d0 b5d0 b3d0 be20 d0b5  ... .. ...... ..
+00003d40: d0b5 20d0 b5d0 b920 d0b5 d0bc d183 20d0  .. .... ...... .
+00003d50: b5d1 81d0 bbd0 b820 d0b5 d181 d182 d18c  ....... ........
+00003d60: 20d0 b5d1 89d0 b520 d0b5 d189 d191 20d0   ...... ...... .
+00003d70: b5d1 8e20 d0b5 d191 20d0 b620 d0b6 d0b5  ... .... .. ....
+00003d80: 20d0 b6d0 b8d0 b7d0 bdd1 8c20 d0b7 d0b0   .......... ....
+00003d90: 20d0 b7d0 b0d0 bdd1 8fd1 8220 d0b7 d0b0   .......... ....
+00003da0: d0bd d18f d182 d0b0 20d0 b7d0 b0d0 bdd1  ........ .......
+00003db0: 8fd1 82d0 be20 d0b7 d0b0 d0bd d18f d182  ..... ..........
+00003dc0: d18b 20d0 b7d0 b0d1 82d0 b5d0 bc20 d0b7  .. .......... ..
+00003dd0: d0b0 d182 d0be 20d0 b7d0 b0d1 87d0 b5d0  ...... .........
+00003de0: bc20 d0b7 d0b4 d0b5 d181 d18c 20d0 b7d0  . .......... ...
+00003df0: bdd0 b0d1 87d0 b8d1 8220 d0b8 20d0 b8d0  ......... .. ...
+00003e00: b720 d0b8 d0bb d0b8 20d0 b8d0 bc20 d0b8  . ...... .... ..
+00003e10: d0bc d0b5 d0bd d0bd d0be 20d0 b8d0 bcd0  .......... .....
+00003e20: b5d1 82d1 8c20 d0b8 d0bc d0b8 20d0 b8d0  ..... ...... ...
+00003e30: bcd1 8f20 d0b8 d0bd d0be d0b3 d0b4 d0b0  ... ............
+00003e40: 20d0 b8d1 8520 d0ba 20d0 bad0 b0d0 b6d0   .... .. .......
+00003e50: b4d0 b0d1 8f20 d0ba d0b0 d0b6 d0b4 d0be  ..... ..........
+00003e60: d0b5 20d0 bad0 b0d0 b6d0 b4d1 8bd0 b520  .. ............ 
+00003e70: d0ba d0b0 d0b6 d0b4 d18b d0b9 20d0 bad0  ............ ...
+00003e80: b0d0 b6d0 b5d1 82d1 81d1 8f20 d0ba d0b0  ........... ....
+00003e90: d0ba 20d0 bad0 b0d0 bad0 b0d1 8f20 d0ba  .. .......... ..
+00003ea0: d0b0 d0ba d0be d0b9 20d0 bad0 b5d0 bc20  ........ ...... 
+00003eb0: d0ba d0be d0b3 d0b4 d0b0 20d0 bad0 bed0  .......... .....
+00003ec0: b3d0 be20 d0ba d0be d0bc 20d0 bad0 bed0  ... ...... .....
+00003ed0: bcd1 8320 d0ba d0be d0bd d0b5 d187 d0bd  ... ............
+00003ee0: d0be 20d0 bad0 bed1 82d0 bed1 80d0 b0d1  .. .............
+00003ef0: 8f20 d0ba d0be d182 d0be d180 d0be d0b3  . ..............
+00003f00: d0be 20d0 bad0 bed1 82d0 bed1 80d0 bed0  .. .............
+00003f10: b920 d0ba d0be d182 d0be d180 d18b d0b5  . ..............
+00003f20: 20d0 bad0 bed1 82d0 bed1 80d1 8bd0 b920   .............. 
+00003f30: d0ba d0be d182 d0be d180 d18b d185 20d0  .............. .
+00003f40: bad1 80d0 bed0 bcd0 b520 d0ba d180 d183  ......... ......
+00003f50: d0b3 d0be d0bc 20d0 bad1 82d0 be20 d0ba  ...... ...... ..
+00003f60: d183 d0b4 d0b0 20d0 bbd0 b5d1 8220 d0bb  ...... ...... ..
+00003f70: d0b8 20d0 bbd0 b8d1 88d1 8c20 d0bb d183  .. ........ ....
+00003f80: d187 d188 d0b5 20d0 bbd1 8ed0 b4d0 b820  ...... ........ 
+00003f90: d0bc 20d0 bcd0 b0d0 bbd0 be20 d0bc d0b5  .. ........ ....
+00003fa0: d0b6 d0b4 d183 20d0 bcd0 b5d0 bbd1 8f20  ...... ........ 
+00003fb0: d0bc d0b5 d0bd d0b5 d0b5 20d0 bcd0 b5d0  .......... .....
+00003fc0: bdd1 8cd1 88d0 b520 d0bc d0b5 d0bd d18f  ....... ........
+00003fd0: 20d0 bcd0 b8d0 bbd0 bbd0 b8d0 bed0 bdd0   ...............
+00003fe0: bed0 b220 d0bc d0b8 d0bc d0be 20d0 bcd0  ... ........ ...
+00003ff0: b8d1 80d0 b020 d0bc d0bd d0b5 20d0 bcd0  ..... ...... ...
+00004000: bdd0 bed0 b3d0 be20 d0bc d0bd d0be d0b3  ....... ........
+00004010: d0be d187 d0b8 d181 d0bb d0b5 d0bd d0bd  ................
+00004020: d0b0 d18f 20d0 bcd0 bdd0 bed0 b3d0 bed1  .... ...........
+00004030: 87d0 b8d1 81d0 bbd0 b5d0 bdd0 bdd0 bed0  ................
+00004040: b520 d0bc d0bd d0be d0b3 d0be d187 d0b8  . ..............
+00004050: d181 d0bb d0b5 d0bd d0bd d18b d0b5 20d0  .............. .
+00004060: bcd0 bdd0 bed0 b3d0 bed1 87d0 b8d1 81d0  ................
+00004070: bbd0 b5d0 bdd0 bdd1 8bd0 b920 d0bc d0bd  ........... ....
+00004080: d0be d0b9 20d0 bcd0 bdd0 bed1 8e20 d0bc  .... ........ ..
+00004090: d0be d0b3 20d0 bcd0 bed0 b3d1 83d1 8220  .... .......... 
+000040a0: d0bc d0be d0b6 20d0 bcd0 bed0 b6d0 b5d1  ...... .........
+000040b0: 8220 d0bc d0be d0b6 d0bd d0be 20d0 bcd0  . .......... ...
+000040c0: bed0 b6d1 85d0 be20 d0bc d0be d0b8 20d0  ....... ...... .
+000040d0: bcd0 bed0 b920 d0bc d0be d180 20d0 bcd0  ..... ...... ...
+000040e0: bed1 87d1 8c20 d0bc d0be d18f 20d0 bcd0  ..... ...... ...
+000040f0: bed1 9120 d0bc d18b 20d0 bdd0 b020 d0bd  ... .... .... ..
+00004100: d0b0 d0b2 d0b5 d180 d185 d183 20d0 bdd0  ............ ...
+00004110: b0d0 b420 d0bd d0b0 d0b4 d0be 20d0 bdd0  ... ........ ...
+00004120: b0d0 b7d0 b0d0 b420 d0bd d0b0 d0b8 d0b1  ....... ........
+00004130: d0be d0bb d0b5 d0b5 20d0 bdd0 b0d0 bad0  ........ .......
+00004140: bed0 bdd0 b5d1 8620 d0bd d0b0 d0bc 20d0  ....... ...... .
+00004150: bdd0 b0d0 bcd0 b820 d0bd d0b0 d181 20d0  ....... ...... .
+00004160: bdd0 b0d1 87d0 b0d0 bbd0 b020 d0bd d0b0  ........... ....
+00004170: d188 20d0 bdd0 b0d1 88d0 b020 d0bd d0b0  .. ........ ....
+00004180: d188 d0b5 20d0 bdd0 b0d1 88d0 b820 d0bd  .... ........ ..
+00004190: d0b5 20d0 bdd0 b5d0 b3d0 be20 d0bd d0b5  .. ........ ....
+000041a0: d0b4 d0b0 d0b2 d0bd d0be 20d0 bdd0 b5d0  .......... .....
+000041b0: b4d0 b0d0 bbd0 b5d0 bad0 be20 d0bd d0b5  ........... ....
+000041c0: d0b5 20d0 bdd0 b5d0 b920 d0bd d0b5 d0bb  .. ...... ......
+000041d0: d18c d0b7 d18f 20d0 bdd0 b5d0 bc20 d0bd  ...... ...... ..
+000041e0: d0b5 d0bc d0bd d0be d0b3 d0be 20d0 bdd0  ............ ...
+000041f0: b5d0 bcd1 8320 d0bd d0b5 d0bf d180 d0b5  ..... ..........
+00004200: d180 d18b d0b2 d0bd d0be 20d0 bdd0 b5d1  .......... .....
+00004210: 80d0 b5d0 b4d0 bad0 be20 d0bd d0b5 d181  ......... ......
+00004220: d0ba d0be d0bb d18c d0ba d0be 20d0 bdd0  ............ ...
+00004230: b5d1 8220 d0bd d0b5 d18e 20d0 bdd0 b5d1  ... ...... .....
+00004240: 9120 d0bd d0b8 20d0 bdd0 b8d0 b1d1 83d0  . .... .........
+00004250: b4d1 8c20 d0bd d0b8 d0b6 d0b5 20d0 bdd0  ... ........ ...
+00004260: b8d0 b7d0 bad0 be20 d0bd d0b8 d0ba d0be  ....... ........
+00004270: d0b3 d0b4 d0b0 20d0 bdd0 b8d0 bad1 83d0  ...... .........
+00004280: b4d0 b020 d0bd d0b8 d0bc d0b8 20d0 bdd0  ... ........ ...
+00004290: b8d1 8520 d0bd d0b8 d187 d0b5 d0b3 d0be  ... ............
+000042a0: 20d0 bdd0 be20 d0bd d183 20d0 bdd1 83d0   .... .... .....
+000042b0: b6d0 bdd0 be20 d0bd d185 20d0 be20 d0be  ..... .... .. ..
+000042c0: d0b1 20d0 bed0 b1d0 b020 d0be d0b1 d18b  .. ...... ......
+000042d0: d187 d0bd d0be 20d0 bed0 b4d0 b8d0 bd20  ...... ........ 
+000042e0: d0be d0b4 d0b8 d0bd d0bd d0b0 d0b4 d186  ................
+000042f0: d0b0 d182 d18b d0b9 20d0 bed0 b4d0 b8d0  ........ .......
+00004300: bdd0 bdd0 b0d0 b4d1 86d0 b0d1 82d1 8c20  ............... 
+00004310: d0be d0b4 d0bd d0b0 d0b6 d0b4 d18b 20d0  .............. .
+00004320: bed0 b4d0 bdd0 b0d0 bad0 be20 d0be d0b4  ........... ....
+00004330: d0bd d0be d0b3 d0be 20d0 bed0 b4d0 bdd0  ........ .......
+00004340: bed0 b920 d0be d0ba d0be d0bb d0be 20d0  ... .......... .
+00004350: bed0 bd20 d0be d0bd d0b0 20d0 bed0 bdd0  ... ...... .....
+00004360: b820 d0be d0bd d0be 20d0 bed0 bfd1 8fd1  . ...... .......
+00004370: 82d1 8c20 d0be d181 d0be d0b1 d0b5 d0bd  ... ............
+00004380: d0bd d0be 20d0 bed1 8220 d0be d182 d0be  .... .... ......
+00004390: d0b2 d181 d18e d0b4 d183 20d0 bed1 82d1  .......... .....
+000043a0: 81d1 8ed0 b4d0 b020 d0be d187 d0b5 d0bd  ....... ........
+000043b0: d18c 20d0 bfd0 b5d1 80d0 b2d1 8bd0 b920  .. ............ 
+000043c0: d0bf d0b5 d180 d0b5 d0b4 20d0 bfd0 be20  .......... .... 
+000043d0: d0bf d0be d0b4 20d0 bfd0 bed0 b6d0 b0d0  ...... .........
+000043e0: bbd1 83d0 b9d1 81d1 82d0 b020 d0bf d0be  ........... ....
+000043f0: d0b7 d0b6 d0b5 20d0 bfd0 bed0 bad0 b020  ...... ........ 
+00004400: d0bf d0be d180 20d0 bfd0 bed1 80d0 b020  ...... ........ 
+00004410: d0bf d0be d181 d0bb d0b5 20d0 bfd0 bed1  .......... .....
+00004420: 81d1 80d0 b5d0 b4d0 b820 d0bf d0be d182  ......... ......
+00004430: d0be d0bc 20d0 bfd0 bed1 82d0 bed0 bcd1  .... ...........
+00004440: 8320 d0bf d0be d187 d0b5 d0bc d183 20d0  . ............ .
+00004450: bfd0 bed1 87d1 82d0 b820 d0bf d180 d0b5  ......... ......
+00004460: d0ba d180 d0b0 d181 d0bd d0be 20d0 bfd1  ............ ...
+00004470: 80d0 b820 d0bf d180 d0be 20d0 bfd1 80d0  ... ...... .....
+00004480: bed1 81d1 82d0 be20 d0bf d180 d0be d182  ....... ........
+00004490: d0b8 d0b2 20d0 bfd1 80d0 bed1 86d0 b5d0  .... ...........
+000044a0: bdd1 82d0 bed0 b220 d0bf d18f d182 d0bd  ....... ........
+000044b0: d0b0 d0b4 d186 d0b0 d182 d18b d0b9 20d0  .............. .
+000044c0: bfd1 8fd1 82d0 bdd0 b0d0 b4d1 86d0 b0d1  ................
+000044d0: 82d1 8c20 d0bf d18f d182 d18b d0b9 20d0  ... .......... .
+000044e0: bfd1 8fd1 82d1 8c20 d180 d0b0 d0b7 20d1  ....... ...... .
+000044f0: 80d0 b0d0 b7d0 b2d0 b520 d180 d0b0 d0bd  ......... ......
+00004500: d0be 20d1 80d0 b0d0 bdd1 8cd1 88d0 b520  .. ............ 
+00004510: d180 d18f d0b4 d0be d0bc 20d1 8120 d181  .......... .. ..
+00004520: d0b0 d0bc 20d1 81d0 b0d0 bcd0 b020 d181  .... ........ ..
+00004530: d0b0 d0bc d0b8 20d1 81d0 b0d0 bcd0 b8d0  ...... .........
+00004540: bc20 d181 d0b0 d0bc d0b8 d0bc d0b8 20d1  . ............ .
+00004550: 81d0 b0d0 bcd0 b8d1 8520 d181 d0b0 d0bc  ......... ......
+00004560: d0be 20d1 81d0 b0d0 bcd0 bed0 b3d0 be20  .. ............ 
+00004570: d181 d0b0 d0bc d0be d0b9 20d1 81d0 b0d0  .......... .....
+00004580: bcd0 bed0 bc20 d181 d0b0 d0bc d0be d0bc  ..... ..........
+00004590: d183 20d1 81d0 b0d0 bcd1 8320 d181 d0b2  .. ........ ....
+000045a0: d0be d0b5 20d1 81d0 b2d0 bed0 b5d0 b3d0  .... ...........
+000045b0: be20 d181 d0b2 d0be d0b5 d0b9 20d1 81d0  . .......... ...
+000045c0: b2d0 bed0 b820 d181 d0b2 d0be d0b8 d185  ..... ..........
+000045d0: 20d1 81d0 b2d0 bed1 8e20 d181 d0b5 d0b0   ........ ......
+000045e0: d0be d0b9 20d1 81d0 b5d0 b1d0 b520 d181  .... ........ ..
+000045f0: d0b5 d0b1 d18f 20d1 81d0 b5d0 b3d0 bed0  ...... .........
+00004600: b4d0 bdd1 8f20 d181 d0b5 d0b4 d18c d0bc  ..... ..........
+00004610: d0be d0b9 20d1 81d0 b5d0 b9d1 87d0 b0d1  .... ...........
+00004620: 8120 d181 d0b5 d0bc d0bd d0b0 d0b4 d186  . ..............
+00004630: d0b0 d182 d18b d0b9 20d1 81d0 b5d0 bcd0  ........ .......
+00004640: bdd0 b0d0 b4d1 86d0 b0d1 82d1 8c20 d181  ............. ..
+00004650: d0b5 d0bc d18c 20d1 81d0 b8d1 8520 d181  ...... ...... ..
+00004660: d0ba d0b0 d0b7 d0b0 d0bb 20d1 81d0 bad0  .......... .....
+00004670: b0d0 b7d0 b0d0 bbd0 b020 d181 d0ba d0b0  ......... ......
+00004680: d0b7 d0b0 d182 d18c 20d1 81d0 bad0 bed0  ........ .......
+00004690: bbd1 8cd0 bad0 be20 d181 d0bb d0b8 d188  ....... ........
+000046a0: d0ba d0be d0bc 20d1 81d0 bdd0 b0d1 87d0  ...... .........
+000046b0: b0d0 bbd0 b020 d181 d0bd d0be d0b2 d0b0  ..... ..........
+000046c0: 20d1 81d0 be20 d181 d0be d0b1 d0be d0b9   .... ..........
+000046d0: 20d1 81d0 bed0 b1d0 bed1 8e20 d181 d0be   .......... ....
+000046e0: d0b2 d181 d0b5 d0bc 20d1 81d0 bfd0 b0d1  ........ .......
+000046f0: 81d0 b8d0 b1d0 be20 d181 d182 d0b0 d0bb  ....... ........
+00004700: 20d1 81d1 83d1 82d1 8c20 d182 20d1 82d0   ........ .. ...
+00004710: b020 d182 d0b0 d0ba 20d1 82d0 b0d0 bad0  . ...... .......
+00004720: b0d1 8f20 d182 d0b0 d0ba d0b6 d0b5 20d1  ... .......... .
+00004730: 82d0 b0d0 bad0 b8d0 b520 d182 d0b0 d0ba  ......... ......
+00004740: d0be d0b5 20d1 82d0 b0d0 bad0 bed0 b920  .... .......... 
+00004750: d182 d0b0 d0bc 20d1 82d0 b2d0 bed0 b920  ...... ........ 
+00004760: d182 d0b2 d0be d18f 20d1 82d0 b2d0 bed1  ........ .......
+00004770: 9120 d182 d0b5 20d1 82d0 b5d0 b1d0 b520  . .... ........ 
+00004780: d182 d0b5 d0b1 d18f 20d1 82d0 b5d0 bc20  ........ ...... 
+00004790: d182 d0b5 d0bc d0b8 20d1 82d0 b5d0 bfd0  ........ .......
+000047a0: b5d1 80d1 8c20 d182 d0b5 d185 20d1 82d0  ..... ...... ...
+000047b0: be20 d182 d0be d0b1 d0be d0b9 20d1 82d0  . .......... ...
+000047c0: bed0 b1d0 bed1 8e20 d182 d0be d0b3 d0b4  ....... ........
+000047d0: d0b0 20d1 82d0 bed0 b3d0 be20 d182 d0be  .. ........ ....
+000047e0: d0b6 d0b5 20d1 82d0 bed0 bbd1 8cd0 bad0  .... ...........
+000047f0: be20 d182 d0be d0bc 20d1 82d0 bed0 bcd1  . ...... .......
+00004800: 8320 d182 d0be d182 20d1 82d0 bed1 8e20  . ...... ...... 
+00004810: d182 d180 d0b5 d182 d0b8 d0b9 20d1 82d1  ............ ...
+00004820: 80d0 b820 d182 d180 d0b8 d0bd d0b0 d0b4  ... ............
+00004830: d186 d0b0 d182 d18b d0b9 20d1 82d1 80d0  .......... .....
+00004840: b8d0 bdd0 b0d0 b4d1 86d0 b0d1 82d1 8c20  ............... 
+00004850: d182 d183 20d1 82d1 83d0 b4d0 b020 d182  .... ........ ..
+00004860: d183 d182 20d1 82d1 8b20 d182 d18b d181  .... .... ......
+00004870: d18f d187 20d1 8320 d183 d0b6 20d1 83d0  .... .. .... ...
+00004880: b6d0 b520 d183 d0bc d0b5 d182 d18c 20d1  ... .......... .
+00004890: 85d0 bed1 80d0 bed1 88d0 be20 d185 d0be  ........... ....
+000048a0: d182 d0b5 d182 d18c 20d1 85d0 bed1 82d1  ........ .......
+000048b0: 8c20 d185 d0be d182 d18f 20d1 85d0 bed1  . ........ .....
+000048c0: 87d0 b5d1 88d1 8c20 d187 d0b0 d181 d182  ....... ........
+000048d0: d0be 20d1 87d0 b0d1 89d0 b520 d187 d0b5  .. ........ ....
+000048e0: d0b3 d0be 20d1 87d0 b5d0 bbd0 bed0 b2d0  .... ...........
+000048f0: b5d0 ba20 d187 d0b5 d0bc 20d1 87d0 b5d0  ... ...... .....
+00004900: bcd1 8320 d187 d0b5 d180 d0b5 d0b7 20d1  ... .......... .
+00004910: 87d0 b5d1 82d0 b2d0 b5d1 80d1 82d1 8bd0  ................
+00004920: b920 d187 d0b5 d182 d18b d180 d0b5 20d1  . ............ .
+00004930: 87d0 b5d1 82d1 8bd1 80d0 bdd0 b0d0 b4d1  ................
+00004940: 86d0 b0d1 82d1 8bd0 b920 d187 d0b5 d182  ......... ......
+00004950: d18b d180 d0bd d0b0 d0b4 d186 d0b0 d182  ................
+00004960: d18c 20d1 87d1 82d0 be20 d187 d182 d0be  .. ...... ......
+00004970: d0b1 20d1 87d1 82d0 bed0 b1d1 8b20 d187  .. .......... ..
+00004980: d183 d182 d18c 20d1 88d0 b5d1 81d1 82d0  ...... .........
+00004990: bdd0 b0d0 b4d1 86d0 b0d1 82d1 8bd0 b920  ............... 
+000049a0: d188 d0b5 d181 d182 d0bd d0b0 d0b4 d186  ................
+000049b0: d0b0 d182 d18c 20d1 88d0 b5d1 81d1 82d0  ...... .........
+000049c0: bed0 b920 d188 d0b5 d181 d182 d18c 20d1  ... .......... .
+000049d0: 8dd1 82d0 b020 d18d d182 d0b8 20d1 8dd1  ..... ...... ...
+000049e0: 82d0 b8d0 bc20 d18d d182 d0b8 d0bc d0b8  ..... ..........
+000049f0: 20d1 8dd1 82d0 b8d1 8520 d18d d182 d0be   ........ ......
+00004a00: 20d1 8dd1 82d0 bed0 b3d0 be20 d18d d182   .......... ....
+00004a10: d0be d0b9 20d1 8dd1 82d0 bed0 bc20 d18d  .... ........ ..
+00004a20: d182 d0be d0bc d183 20d1 8dd1 82d0 bed1  ........ .......
+00004a30: 8220 d18d d182 d183 20d1 8f20 efbb bfd0  . ...... .. ....
+00004a40: b027 2e73 706c 6974 2827 2027 2929 3b0a  .'.split(' '));.
+00004a50: 0a20 2020 206c 756e 722e 5069 7065 6c69  .    lunr.Pipeli
+00004a60: 6e65 2e72 6567 6973 7465 7246 756e 6374  ne.registerFunct
+00004a70: 696f 6e28 6c75 6e72 2e72 752e 7374 6f70  ion(lunr.ru.stop
+00004a80: 576f 7264 4669 6c74 6572 2c20 2773 746f  WordFilter, 'sto
+00004a90: 7057 6f72 6446 696c 7465 722d 7275 2729  pWordFilter-ru')
+00004aa0: 3b0a 2020 7d3b 0a7d 2929                 ;.  };.}))
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.sv.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.th.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.th.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 2% similar despite different names*

```diff
@@ -115,81 +115,78 @@
 00000720: 7661 7220 6973 4c75 6e72 3220 3d20 6c75  var isLunr2 = lu
 00000730: 6e72 2e76 6572 7369 6f6e 5b30 5d20 3d3d  nr.version[0] ==
 00000740: 2022 3222 3b0a 0a20 2020 202f 2a20 7265   "2";..    /* re
 00000750: 6769 7374 6572 2073 7065 6369 6669 6320  gister specific 
 00000760: 6c6f 6361 6c65 2066 756e 6374 696f 6e20  locale function 
 00000770: 2a2f 0a20 2020 206c 756e 722e 7468 203d  */.    lunr.th =
 00000780: 2066 756e 6374 696f 6e28 2920 7b0a 2020   function() {.  
-00000790: 2020 2020 2020 7468 6973 2e70 6970 656c        this.pipel
-000007a0: 696e 652e 7265 7365 7428 293b 0a20 2020  ine.reset();.   
-000007b0: 2020 2020 2074 6869 732e 7069 7065 6c69       this.pipeli
-000007c0: 6e65 2e61 6464 280a 2020 2020 2020 2020  ne.add(.        
-000007d0: 2020 2020 2f2a 6c75 6e72 2e74 682e 7374      /*lunr.th.st
-000007e0: 6f70 576f 7264 4669 6c74 6572 2c2a 2f0a  opWordFilter,*/.
-000007f0: 2020 2020 2020 2020 2020 2020 6c75 6e72              lunr
-00000800: 2e74 682e 7472 696d 6d65 720a 2020 2020  .th.trimmer.    
-00000810: 2020 2020 293b 0a0a 2020 2020 2020 2020      );..        
-00000820: 6966 2028 6973 4c75 6e72 3229 207b 202f  if (isLunr2) { /
-00000830: 2f20 666f 7220 6c75 6e72 2076 6572 7369  / for lunr versi
-00000840: 6f6e 2032 2e30 2e30 0a20 2020 2020 2020  on 2.0.0.       
-00000850: 2020 2020 2074 6869 732e 746f 6b65 6e69       this.tokeni
-00000860: 7a65 7220 3d20 6c75 6e72 2e74 682e 746f  zer = lunr.th.to
-00000870: 6b65 6e69 7a65 723b 0a20 2020 2020 2020  kenizer;.       
-00000880: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
-00000890: 2020 2020 2020 6966 2028 6c75 6e72 2e74        if (lunr.t
-000008a0: 6f6b 656e 697a 6572 2920 7b20 2f2f 2066  okenizer) { // f
-000008b0: 6f72 206c 756e 7220 7665 7273 696f 6e20  or lunr version 
-000008c0: 302e 362e 300a 2020 2020 2020 2020 2020  0.6.0.          
-000008d0: 2020 2020 2020 6c75 6e72 2e74 6f6b 656e        lunr.token
-000008e0: 697a 6572 203d 206c 756e 722e 7468 2e74  izer = lunr.th.t
-000008f0: 6f6b 656e 697a 6572 3b0a 2020 2020 2020  okenizer;.      
-00000900: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000910: 2020 2020 6966 2028 7468 6973 2e74 6f6b      if (this.tok
-00000920: 656e 697a 6572 466e 2920 7b20 2f2f 2066  enizerFn) { // f
-00000930: 6f72 206c 756e 7220 7665 7273 696f 6e20  or lunr version 
-00000940: 302e 372e 3020 2d3e 2031 2e30 2e30 0a20  0.7.0 -> 1.0.0. 
-00000950: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000960: 6869 732e 746f 6b65 6e69 7a65 7246 6e20  his.tokenizerFn 
-00000970: 3d20 6c75 6e72 2e74 682e 746f 6b65 6e69  = lunr.th.tokeni
-00000980: 7a65 723b 0a20 2020 2020 2020 2020 2020  zer;.           
-00000990: 207d 0a20 2020 2020 2020 207d 0a20 2020   }.        }.   
-000009a0: 207d 3b0a 0a20 2020 202f 2a20 6c75 6e72   };..    /* lunr
-000009b0: 2074 7269 6d6d 6572 2066 756e 6374 696f   trimmer functio
-000009c0: 6e20 2a2f 0a20 2020 206c 756e 722e 7468  n */.    lunr.th
-000009d0: 2e77 6f72 6443 6861 7261 6374 6572 7320  .wordCharacters 
-000009e0: 3d20 225b 5c75 3065 3030 2d5c 7530 6537  = "[\u0e00-\u0e7
-000009f0: 665d 223b 0a20 2020 206c 756e 722e 7468  f]";.    lunr.th
-00000a00: 2e74 7269 6d6d 6572 203d 206c 756e 722e  .trimmer = lunr.
-00000a10: 7472 696d 6d65 7253 7570 706f 7274 2e67  trimmerSupport.g
-00000a20: 656e 6572 6174 6554 7269 6d6d 6572 286c  enerateTrimmer(l
-00000a30: 756e 722e 7468 2e77 6f72 6443 6861 7261  unr.th.wordChara
-00000a40: 6374 6572 7329 3b0a 2020 2020 6c75 6e72  cters);.    lunr
-00000a50: 2e50 6970 656c 696e 652e 7265 6769 7374  .Pipeline.regist
-00000a60: 6572 4675 6e63 7469 6f6e 286c 756e 722e  erFunction(lunr.
-00000a70: 7468 2e74 7269 6d6d 6572 2c20 2774 7269  th.trimmer, 'tri
-00000a80: 6d6d 6572 2d74 6827 293b 0a0a 2020 2020  mmer-th');..    
-00000a90: 7661 7220 7365 676d 656e 7465 7220 3d20  var segmenter = 
-00000aa0: 6c75 6e72 2e77 6f72 6463 7574 3b0a 2020  lunr.wordcut;.  
-00000ab0: 2020 7365 676d 656e 7465 722e 696e 6974    segmenter.init
-00000ac0: 2829 3b0a 2020 2020 6c75 6e72 2e74 682e  ();.    lunr.th.
-00000ad0: 746f 6b65 6e69 7a65 7220 3d20 6675 6e63  tokenizer = func
-00000ae0: 7469 6f6e 2028 6f62 6a29 207b 0a20 2020  tion (obj) {.   
-00000af0: 2020 202f 2f63 6f6e 736f 6c65 2e6c 6f67     //console.log
-00000b00: 286f 626a 293b 0a20 2020 2020 2069 6620  (obj);.      if 
-00000b10: 2821 6172 6775 6d65 6e74 732e 6c65 6e67  (!arguments.leng
-00000b20: 7468 207c 7c20 6f62 6a20 3d3d 206e 756c  th || obj == nul
-00000b30: 6c20 7c7c 206f 626a 203d 3d20 756e 6465  l || obj == unde
-00000b40: 6669 6e65 6429 2072 6574 7572 6e20 5b5d  fined) return []
-00000b50: 0a20 2020 2020 2069 6620 2841 7272 6179  .      if (Array
-00000b60: 2e69 7341 7272 6179 286f 626a 2929 2072  .isArray(obj)) r
-00000b70: 6574 7572 6e20 6f62 6a2e 6d61 7028 6675  eturn obj.map(fu
-00000b80: 6e63 7469 6f6e 2028 7429 207b 2072 6574  nction (t) { ret
-00000b90: 7572 6e20 6973 4c75 6e72 3220 3f20 6e65  urn isLunr2 ? ne
-00000ba0: 7720 6c75 6e72 2e54 6f6b 656e 2874 2920  w lunr.Token(t) 
-00000bb0: 3a20 7420 7d29 0a0a 2020 2020 2020 7661  : t })..      va
-00000bc0: 7220 7374 7220 3d20 6f62 6a2e 746f 5374  r str = obj.toSt
-00000bd0: 7269 6e67 2829 2e72 6570 6c61 6365 282f  ring().replace(/
-00000be0: 5e5c 732b 2f2c 2027 2729 3b0a 2020 2020  ^\s+/, '');.    
-00000bf0: 2020 7265 7475 726e 2073 6567 6d65 6e74    return segment
-00000c00: 6572 2e63 7574 2873 7472 292e 7370 6c69  er.cut(str).spli
-00000c10: 7428 277c 2729 3b0a 2020 2020 7d0a 2020  t('|');.    }.  
-00000c20: 7d3b 0a7d 2929 0a                        };.})).
+00000790: 2020 2020 7468 6973 2e70 6970 656c 696e      this.pipelin
+000007a0: 652e 7265 7365 7428 293b 0a20 2020 2020  e.reset();.     
+000007b0: 2074 6869 732e 7069 7065 6c69 6e65 2e61   this.pipeline.a
+000007c0: 6464 280a 2020 2020 2020 2020 2f2a 6c75  dd(.        /*lu
+000007d0: 6e72 2e74 682e 7374 6f70 576f 7264 4669  nr.th.stopWordFi
+000007e0: 6c74 6572 2c2a 2f0a 2020 2020 2020 2020  lter,*/.        
+000007f0: 6c75 6e72 2e74 682e 7472 696d 6d65 720a  lunr.th.trimmer.
+00000800: 2020 2020 2020 293b 0a0a 2020 2020 2020        );..      
+00000810: 6966 2028 6973 4c75 6e72 3229 207b 202f  if (isLunr2) { /
+00000820: 2f20 666f 7220 6c75 6e72 2076 6572 7369  / for lunr versi
+00000830: 6f6e 2032 2e30 2e30 0a20 2020 2020 2020  on 2.0.0.       
+00000840: 2074 6869 732e 746f 6b65 6e69 7a65 7220   this.tokenizer 
+00000850: 3d20 6c75 6e72 2e74 682e 746f 6b65 6e69  = lunr.th.tokeni
+00000860: 7a65 723b 0a20 2020 2020 207d 2065 6c73  zer;.      } els
+00000870: 6520 7b0a 2020 2020 2020 2020 6966 2028  e {.        if (
+00000880: 6c75 6e72 2e74 6f6b 656e 697a 6572 2920  lunr.tokenizer) 
+00000890: 7b20 2f2f 2066 6f72 206c 756e 7220 7665  { // for lunr ve
+000008a0: 7273 696f 6e20 302e 362e 300a 2020 2020  rsion 0.6.0.    
+000008b0: 2020 2020 2020 6c75 6e72 2e74 6f6b 656e        lunr.token
+000008c0: 697a 6572 203d 206c 756e 722e 7468 2e74  izer = lunr.th.t
+000008d0: 6f6b 656e 697a 6572 3b0a 2020 2020 2020  okenizer;.      
+000008e0: 2020 7d0a 2020 2020 2020 2020 6966 2028    }.        if (
+000008f0: 7468 6973 2e74 6f6b 656e 697a 6572 466e  this.tokenizerFn
+00000900: 2920 7b20 2f2f 2066 6f72 206c 756e 7220  ) { // for lunr 
+00000910: 7665 7273 696f 6e20 302e 372e 3020 2d3e  version 0.7.0 ->
+00000920: 2031 2e30 2e30 0a20 2020 2020 2020 2020   1.0.0.         
+00000930: 2074 6869 732e 746f 6b65 6e69 7a65 7246   this.tokenizerF
+00000940: 6e20 3d20 6c75 6e72 2e74 682e 746f 6b65  n = lunr.th.toke
+00000950: 6e69 7a65 723b 0a20 2020 2020 2020 207d  nizer;.        }
+00000960: 0a20 2020 2020 207d 0a20 2020 207d 3b0a  .      }.    };.
+00000970: 0a20 2020 202f 2a20 6c75 6e72 2074 7269  .    /* lunr tri
+00000980: 6d6d 6572 2066 756e 6374 696f 6e20 2a2f  mmer function */
+00000990: 0a20 2020 206c 756e 722e 7468 2e77 6f72  .    lunr.th.wor
+000009a0: 6443 6861 7261 6374 6572 7320 3d20 225b  dCharacters = "[
+000009b0: 5c75 3065 3030 2d5c 7530 6537 665d 223b  \u0e00-\u0e7f]";
+000009c0: 0a20 2020 206c 756e 722e 7468 2e74 7269  .    lunr.th.tri
+000009d0: 6d6d 6572 203d 206c 756e 722e 7472 696d  mmer = lunr.trim
+000009e0: 6d65 7253 7570 706f 7274 2e67 656e 6572  merSupport.gener
+000009f0: 6174 6554 7269 6d6d 6572 286c 756e 722e  ateTrimmer(lunr.
+00000a00: 7468 2e77 6f72 6443 6861 7261 6374 6572  th.wordCharacter
+00000a10: 7329 3b0a 2020 2020 6c75 6e72 2e50 6970  s);.    lunr.Pip
+00000a20: 656c 696e 652e 7265 6769 7374 6572 4675  eline.registerFu
+00000a30: 6e63 7469 6f6e 286c 756e 722e 7468 2e74  nction(lunr.th.t
+00000a40: 7269 6d6d 6572 2c20 2774 7269 6d6d 6572  rimmer, 'trimmer
+00000a50: 2d74 6827 293b 0a0a 2020 2020 7661 7220  -th');..    var 
+00000a60: 7365 676d 656e 7465 7220 3d20 6c75 6e72  segmenter = lunr
+00000a70: 2e77 6f72 6463 7574 3b0a 2020 2020 7365  .wordcut;.    se
+00000a80: 676d 656e 7465 722e 696e 6974 2829 3b0a  gmenter.init();.
+00000a90: 2020 2020 6c75 6e72 2e74 682e 746f 6b65      lunr.th.toke
+00000aa0: 6e69 7a65 7220 3d20 6675 6e63 7469 6f6e  nizer = function
+00000ab0: 286f 626a 2920 7b0a 2020 2020 2020 2f2f  (obj) {.      //
+00000ac0: 636f 6e73 6f6c 652e 6c6f 6728 6f62 6a29  console.log(obj)
+00000ad0: 3b0a 2020 2020 2020 6966 2028 2161 7267  ;.      if (!arg
+00000ae0: 756d 656e 7473 2e6c 656e 6774 6820 7c7c  uments.length ||
+00000af0: 206f 626a 203d 3d20 6e75 6c6c 207c 7c20   obj == null || 
+00000b00: 6f62 6a20 3d3d 2075 6e64 6566 696e 6564  obj == undefined
+00000b10: 2920 7265 7475 726e 205b 5d0a 2020 2020  ) return [].    
+00000b20: 2020 6966 2028 4172 7261 792e 6973 4172    if (Array.isAr
+00000b30: 7261 7928 6f62 6a29 2920 7265 7475 726e  ray(obj)) return
+00000b40: 206f 626a 2e6d 6170 2866 756e 6374 696f   obj.map(functio
+00000b50: 6e28 7429 207b 0a20 2020 2020 2020 2072  n(t) {.        r
+00000b60: 6574 7572 6e20 6973 4c75 6e72 3220 3f20  eturn isLunr2 ? 
+00000b70: 6e65 7720 6c75 6e72 2e54 6f6b 656e 2874  new lunr.Token(t
+00000b80: 2920 3a20 740a 2020 2020 2020 7d29 0a0a  ) : t.      })..
+00000b90: 2020 2020 2020 7661 7220 7374 7220 3d20        var str = 
+00000ba0: 6f62 6a2e 746f 5374 7269 6e67 2829 2e72  obj.toString().r
+00000bb0: 6570 6c61 6365 282f 5e5c 732b 2f2c 2027  eplace(/^\s+/, '
+00000bc0: 2729 3b0a 2020 2020 2020 7265 7475 726e  ');.      return
+00000bd0: 2073 6567 6d65 6e74 6572 2e63 7574 2873   segmenter.cut(s
+00000be0: 7472 292e 7370 6c69 7428 277c 2729 3b0a  tr).split('|');.
+00000bf0: 2020 2020 7d0a 2020 7d3b 0a7d 2929           }.  };.}))
```

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.tr.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/lunr.vi.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/lunr-language/tinyseg.js` & `mkdocs-1.5.3/mkdocs/contrib/search/lunr-language/tinyseg.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/lunr.js` & `mkdocs-1.5.3/mkdocs/contrib/search/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/main.js` & `mkdocs-1.5.3/mkdocs/contrib/search/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/contrib/search/templates/search/worker.js` & `mkdocs-1.5.3/mkdocs/contrib/search/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/livereload/__init__.py` & `mkdocs-1.5.3/mkdocs/livereload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,28 @@
 import watchdog.events
 import watchdog.observers.polling
 
 _SCRIPT_TEMPLATE_STR = """
 var livereload = function(epoch, requestId) {
     var req = new XMLHttpRequest();
     req.onloadend = function() {
+        window.removeEventListener("beforeunload", abort);
         if (parseFloat(this.responseText) > epoch) {
             location.reload();
             return;
         }
         var launchNext = livereload.bind(this, epoch, requestId);
         if (this.status === 200) {
             launchNext();
         } else {
             setTimeout(launchNext, 3000);
         }
     };
+    var abort = req.abort.bind(req);
+    window.addEventListener("beforeunload", abort);
     req.open("GET", "/livereload/" + epoch + "/" + requestId);
     req.send();
 
     console.log('Enabled live reload');
 }
 livereload(${epoch}, ${request_id});
 """
@@ -186,15 +189,15 @@
                 self._to_rebuild.clear()
 
             try:
                 for func in funcs:
                     func()
             except Exception as e:
                 if isinstance(e, SystemExit):
-                    print(e, file=sys.stderr)
+                    print(e, file=sys.stderr)  # noqa: T201
                 else:
                     traceback.print_exc()
                 log.error(
                     "An error happened during the rebuild. The server will appear stuck until build errors are resolved."
                 )
                 continue
```

### Comparing `mkdocs-1.5.2/mkdocs/structure/__init__.py` & `mkdocs-1.5.3/mkdocs/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/structure/files.py` & `mkdocs-1.5.3/mkdocs/structure/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 import posixpath
 import shutil
 import warnings
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Callable, Iterable, Iterator, Sequence
 from urllib.parse import quote as urlquote
 
-import jinja2.environment
 import pathspec
 import pathspec.gitignore
 import pathspec.util
 
 from mkdocs import utils
 
 if TYPE_CHECKING:
+    import jinja2.environment
+
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.structure.pages import Page
 
 
 log = logging.getLogger(__name__)
```

### Comparing `mkdocs-1.5.2/mkdocs/structure/nav.py` & `mkdocs-1.5.3/mkdocs/structure/nav.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import warnings
 from typing import TYPE_CHECKING, Iterator, TypeVar
 from urllib.parse import urlsplit
 
 from mkdocs.structure import StructureItem
 from mkdocs.structure.pages import Page
 from mkdocs.utils import nest_paths
 
@@ -47,15 +48,16 @@
     def __init__(self, title: str, children: list[StructureItem]) -> None:
         self.title = title
         self.children = children
 
         self.active = False
 
     def __repr__(self):
-        return f"Section(title={self.title!r})"
+        name = self.__class__.__name__
+        return f"{name}(title={self.title!r})"
 
     title: str
     """The title of the section."""
 
     children: list[StructureItem]
     """An iterable of all child navigation objects. Children may include nested sections, pages and links."""
 
@@ -93,16 +95,17 @@
 
 class Link(StructureItem):
     def __init__(self, title: str, url: str):
         self.title = title
         self.url = url
 
     def __repr__(self):
+        name = self.__class__.__name__
         title = f"{self.title!r}" if self.title is not None else '[blank]'
-        return f"Link(title={title}, url={self.url!r})"
+        return f"{name}(title={title}, url={self.url!r})"
 
     title: str
     """The title of the link. This would generally be used as the label of the link."""
 
     url: str
     """The URL that the link points to. The URL should always be an absolute URLs and
     should not need to have `base_url` prepended."""
@@ -194,14 +197,30 @@
     if file:
         if file.inclusion.is_excluded():
             log.log(
                 min(logging.INFO, config.validation.nav.not_found),
                 f"A reference to '{file.src_path}' is included in the 'nav' "
                 "configuration, but this file is excluded from the built site.",
             )
+        page = file.page
+        if page is not None:
+            if isinstance(page, Page):
+                if type(page) is not Page:  # Strict subclass
+                    return page
+                warnings.warn(
+                    "A plugin has set File.page to an instance of Page and it got overwritten. "
+                    "The behavior of this will change in MkDocs 1.6.",
+                    DeprecationWarning,
+                )
+            else:
+                warnings.warn(  # type: ignore[unreachable]
+                    "A plugin has set File.page to a type other than Page. "
+                    "This will be an error in MkDocs 1.6.",
+                    DeprecationWarning,
+                )
         return Page(title, file, config)
     return Link(title, path)
 
 
 T = TypeVar('T')
```

### Comparing `mkdocs-1.5.2/mkdocs/structure/pages.py` & `mkdocs-1.5.3/mkdocs/structure/pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 import posixpath
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Iterator, MutableMapping, Sequence
 from urllib.parse import unquote as urlunquote
 from urllib.parse import urljoin, urlsplit, urlunsplit
 
 import markdown
+import markdown.postprocessors
 import markdown.treeprocessors
 from markdown.util import AMP_SUBSTITUTE
 
 from mkdocs import utils
 from mkdocs.structure import StructureItem
 from mkdocs.structure.toc import get_toc
 from mkdocs.utils import _removesuffix, get_build_date, get_markdown_title, meta, weak_property
 
 if TYPE_CHECKING:
     from xml.etree import ElementTree as etree
 
-    import markdown.postprocessors
-
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.structure.files import File, Files
     from mkdocs.structure.toc import TableOfContents
 
 
 log = logging.getLogger(__name__)
 
@@ -61,17 +60,18 @@
         return (
             isinstance(other, self.__class__)
             and self.title == other.title
             and self.file == other.file
         )
 
     def __repr__(self):
+        name = self.__class__.__name__
         title = f"{self.title!r}" if self.title is not None else '[blank]'
         url = self.abs_url or self.file.url
-        return f"Page(title={title}, url={url!r})"
+        return f"{name}(title={title}, url={url!r})"
 
     markdown: str | None
     """The original Markdown content from the file."""
 
     content: str | None
     """The rendered Markdown as HTML, this is the contents of the documentation."""
 
@@ -349,15 +349,15 @@
         scheme, netloc, path, query, fragment = urlsplit(url)
 
         warning_level, warning = 0, ''
 
         # Ignore URLs unless they are a relative link to a source file.
         if scheme or netloc:  # External link.
             return url
-        elif url.startswith('/') or url.startswith('\\'):  # Absolute link.
+        elif url.startswith(('/', '\\')):  # Absolute link.
             warning_level = self.config.validation.links.absolute_links
             warning = f"Doc file '{self.file.src_uri}' contains an absolute link '{url}', it was left as is."
         elif AMP_SUBSTITUTE in url:  # AMP_SUBSTITUTE is used internally by Markdown only for email.
             return url
         elif not path:  # Self-link containing only query or fragment.
             return url
```

### Comparing `mkdocs-1.5.2/mkdocs/structure/toc.py` & `mkdocs-1.5.3/mkdocs/structure/toc.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/templates/sitemap.xml` & `mkdocs-1.5.3/mkdocs/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/base.py` & `mkdocs-1.5.3/mkdocs/tests/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/build_tests.py` & `mkdocs-1.5.3/mkdocs/tests/build_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/cli_tests.py` & `mkdocs-1.5.3/mkdocs/tests/cli_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/get_deps_tests.py` & `mkdocs-1.5.3/mkdocs/tests/get_deps_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/gh_deploy_tests.py` & `mkdocs-1.5.3/mkdocs/tests/gh_deploy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/integration.py` & `mkdocs-1.5.3/mkdocs/tests/integration.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/livereload_tests.py` & `mkdocs-1.5.3/mkdocs/tests/livereload_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
             headers, output = do_request(server, "GET /")
             self.assertRegex(output, r"^<body>aaa</body>$")
             self.assertEqual(headers["_status"], "200 OK")
             self.assertEqual(headers.get("content-type"), "text/html")
             self.assertEqual(headers.get("content-length"), str(len(output)))
 
             for path in "/foo/", "/foo/index.html":
-                _, output = do_request(server, "GET /foo/")
+                _, output = do_request(server, f"GET {path}")
                 self.assertRegex(output, r"^<body>bbb</body>$")
 
             with self.assertLogs("mkdocs.livereload"):
                 headers, _ = do_request(server, "GET /foo/index.html/")
             self.assertEqual(headers["_status"], "404 Not Found")
 
     @tempdir(
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/localization_tests.py` & `mkdocs-1.5.3/mkdocs/tests/localization_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/new_tests.py` & `mkdocs-1.5.3/mkdocs/tests/new_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/plugin_tests.py` & `mkdocs-1.5.3/mkdocs/tests/plugin_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,25 +169,23 @@
             [prio.on_post_build],
         )
 
     def test_set_plugin_on_collection(self):
         collection = plugins.PluginCollection()
         plugin = DummyPlugin()
         collection['foo'] = plugin
-        self.assertEqual([(k, v) for k, v in collection.items()], [('foo', plugin)])
+        self.assertEqual(list(collection.items()), [('foo', plugin)])
 
     def test_set_multiple_plugins_on_collection(self):
         collection = plugins.PluginCollection()
         plugin1 = DummyPlugin()
         collection['foo'] = plugin1
         plugin2 = DummyPlugin()
         collection['bar'] = plugin2
-        self.assertEqual(
-            [(k, v) for k, v in collection.items()], [('foo', plugin1), ('bar', plugin2)]
-        )
+        self.assertEqual(list(collection.items()), [('foo', plugin1), ('bar', plugin2)])
 
     def test_run_event_on_collection(self):
         collection = plugins.PluginCollection()
         plugin = DummyPlugin()
         plugin.load_config({'foo': 'new'})
         collection['foo'] = plugin
         self.assertEqual(
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/search_tests.py` & `mkdocs-1.5.3/mkdocs/tests/search_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def test_lang_good_and_bad_code(self):
         option = search.LangOption()
         value = option.validate(['en', 'foo'])
         self.assertEqual(['en'], value)
 
     def test_lang_missing_and_with_territory(self):
         option = search.LangOption()
-        value = option.validate(['zh_CN', 'pt_BR', 'fr'])
+        value = option.validate(['cs_CZ', 'pt_BR', 'fr'])
         self.assertEqual(['fr', 'en', 'pt'], value)
 
 
 class SearchPluginTests(unittest.TestCase):
     def test_plugin_config_defaults(self):
         expected = {
             'lang': None,
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/theme_tests.py` & `mkdocs-1.5.3/mkdocs/tests/theme_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/config/base_tests.py` & `mkdocs-1.5.3/mkdocs/tests/config/base_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/config/config_options_legacy_tests.py` & `mkdocs-1.5.3/mkdocs/tests/config/config_options_legacy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/config/config_options_tests.py` & `mkdocs-1.5.3/mkdocs/tests/config/config_options_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1133,22 +1133,23 @@
         conf = self.get_config(Schema, {'option': "mkdocs"})
         assert_type(conf.option, Theme)
         assert_type(conf.option.name, Optional[str])
         self.assertEqual(conf.option.name, 'mkdocs')
 
     def test_uninstalled_theme_as_string(self) -> None:
         class Schema(Config):
-            option = c.Theme()
+            theme = c.Theme()
+            plugins = c.Plugins(theme_key='theme')
 
         with self.expect_error(
-            option=re.compile(
+            theme=re.compile(
                 r"Unrecognised theme name: 'mkdocs2'. The available installed themes are: .+"
             )
         ):
-            self.get_config(Schema, {'option': "mkdocs2"})
+            self.get_config(Schema, {'theme': "mkdocs2", 'plugins': "search"})
 
     def test_theme_default(self) -> None:
         class Schema(Config):
             option = c.Theme(default='mkdocs')
 
         conf = self.get_config(Schema, {'option': None})
         self.assertEqual(conf.option.name, 'mkdocs')
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/config/config_tests.py` & `mkdocs-1.5.3/mkdocs/tests/config/config_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.assertEqual(result['site_name'], expected_result['site_name'])
         self.assertEqual(result['nav'], expected_result['nav'])
 
     @tempdir()
     @tempdir()
     def test_theme(self, mytheme, custom):
         configs = [
-            dict(),  # default theme
+            {},  # default theme
             {"theme": "readthedocs"},  # builtin theme
             {"theme": {'name': 'readthedocs'}},  # builtin as complex
             {"theme": {'name': None, 'custom_dir': mytheme}},  # custom only as complex
             {
                 "theme": {'name': 'readthedocs', 'custom_dir': custom}
             },  # builtin and custom as complex
             {  # user defined variables
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/integration/projects.yaml` & `mkdocs-1.5.3/mkdocs/tests/integration/projects.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/integration/complicated_config/mkdocs.yml` & `mkdocs-1.5.3/mkdocs/tests/integration/complicated_config/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/image.png` & `mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/integration/subpages/docs/sub1/image.png` & `mkdocs-1.5.3/mkdocs/tests/integration/subpages/docs/sub1/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/structure/file_tests.py` & `mkdocs-1.5.3/mkdocs/tests/structure/file_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
             File('foo/bar.md', '/path/to/docs', '/path/to/site', use_directory_urls=True),
             File('foo/bar.html', '/path/to/docs', '/path/to/site', use_directory_urls=True),
             File('foo/bar.jpg', '/path/to/docs', '/path/to/site', use_directory_urls=True),
             File('foo/bar.js', '/path/to/docs', '/path/to/site', use_directory_urls=True),
             File('foo/bar.css', '/path/to/docs', '/path/to/site', use_directory_urls=True),
         ]
         files = Files(fs)
-        self.assertEqual([f for f in files], fs)
+        self.assertEqual(list(files), fs)
         self.assertEqual(len(files), 6)
         self.assertEqual(files.documentation_pages(), [fs[0], fs[1]])
         self.assertEqual(files.static_pages(), [fs[2]])
         self.assertEqual(files.media_files(), [fs[3], fs[4], fs[5]])
         self.assertEqual(files.javascript_files(), [fs[4]])
         self.assertEqual(files.css_files(), [fs[5]])
         self.assertEqual(files.get_file_from_path('foo/bar.jpg'), fs[3])
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/structure/nav_tests.py` & `mkdocs-1.5.3/mkdocs/tests/structure/nav_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,42 @@
         files = Files([File(s, cfg.docs_dir, cfg.site_dir, cfg.use_directory_urls) for s in fs])
         site_navigation = get_navigation(files, cfg)
         self.assertEqual(str(site_navigation).strip(), expected)
         self.assertEqual(len(site_navigation.items), 3)
         self.assertEqual(len(site_navigation.pages), 7)
         self.assertEqual(repr(site_navigation.homepage), "Page(title=[blank], url='/')")
 
+    def test_nav_page_subclass(self):
+        class PageSubclass(Page):
+            pass
+
+        nav_cfg = [
+            {'Home': 'index.md'},
+            {'About': 'about.md'},
+        ]
+        expected = dedent(
+            """
+            PageSubclass(title=[blank], url='/')
+            PageSubclass(title=[blank], url='/about/')
+            """
+        )
+        cfg = load_config(nav=nav_cfg, site_url='http://example.com/')
+        fs = [
+            File(list(item.values())[0], cfg.docs_dir, cfg.site_dir, cfg.use_directory_urls)
+            for item in nav_cfg
+        ]
+        files = Files(fs)
+        for file in files:
+            PageSubclass(None, file, cfg)
+        site_navigation = get_navigation(files, cfg)
+        self.assertEqual(str(site_navigation).strip(), expected)
+        self.assertEqual(len(site_navigation.items), 2)
+        self.assertEqual(len(site_navigation.pages), 2)
+        self.assertEqual(repr(site_navigation.homepage), "PageSubclass(title=[blank], url='/')")
+
     def test_active(self):
         nav_cfg = [
             {'Home': 'index.md'},
             {
                 'API Guide': [
                     {'Running': 'api-guide/running.md'},
                     {'Testing': 'api-guide/testing.md'},
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/structure/page_tests.py` & `mkdocs-1.5.3/mkdocs/tests/structure/page_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1106,25 +1106,25 @@
             ),
             '<a href="mail@example.com">contact</a>',
         )
 
     def test_possible_target_uris(self):
         def test(paths, expected='', exp_true=None, exp_false=None):
             """Test that `possible_target_uris` yields expected values, for use_directory_urls = true and false"""
-            for use_directory_urls, expected in (
+            for use_directory_urls, expected_paths in (
                 (True, exp_true or expected),
                 (False, exp_false or expected),
             ):
                 with self.subTest(paths, use_directory_urls=use_directory_urls):
                     src_path, dest_path = paths
                     f = File(src_path, '', '', use_directory_urls)
                     actual = _RelativePathTreeprocessor._possible_target_uris(
                         f, dest_path, use_directory_urls
                     )
-                    self.assertEqual(list(actual), expected.split(', '))
+                    self.assertEqual(list(actual), expected_paths.split(', '))
 
         test(('index.md', 'index.md'), expected='index.md')
         test(('index.md', 'foo/bar.md'), expected='foo/bar.md')
         test(
             ('index.md', 'foo/bar'),
             expected='foo/bar, foo/bar/index.md, foo/bar/README.md, foo/bar.md',
         )
```

### Comparing `mkdocs-1.5.2/mkdocs/tests/structure/toc_tests.py` & `mkdocs-1.5.3/mkdocs/tests/structure/toc_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/utils/babel_stub_tests.py` & `mkdocs-1.5.3/mkdocs/tests/utils/babel_stub_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/utils/templates_tests.py` & `mkdocs-1.5.3/mkdocs/tests/utils/templates_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/tests/utils/utils_tests.py` & `mkdocs-1.5.3/mkdocs/tests/utils/utils_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/base.html` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/keyboard-modal.html` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/keyboard-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/messages.pot` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/search-modal.html` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/search-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/toc.html` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/toc.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/base.css` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/css/base.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/bootstrap.min.css` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/css/font-awesome.min.css` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/img/favicon.ico` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/img/grid.png` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/img/grid.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/base.js` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/bootstrap.min.js` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/base.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/breadcrumbs.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/breadcrumbs.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href="{{ nav.homepage.url|url }}" class="icon icon-home" aria-label="{% trans %}Docs{% endtrans %}"></a> &raquo;</li>
+    <li><a href="{{ nav.homepage.url|url }}" class="icon icon-home" aria-label="{% trans %}Docs{% endtrans %}"></a></li>
     {%- if page %}
       {%- for doc in page.ancestors[::-1] %}
-        {%- if doc.link %}
-          <li class="breadcrumb-item"><a href="{{ doc.link|e }}">{{ doc.title }}</a></li>
+        {%- if doc.url %}
+          <li class="breadcrumb-item"><a href="{{ doc.url|url }}">{{ doc.title }}</a></li>
         {%- else %}
-          <li>{{ doc.title }} &raquo;</li>
+          <li class="breadcrumb-item">{{ doc.title }}</li>
         {%- endif %}
       {%- endfor %}
       <li class="breadcrumb-item active">{{ page.title }}</li>
     {%- endif %}
     <li class="wy-breadcrumbs-aside">
       {%- block repo %}
       {%- if page and page.edit_url %}
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-    * »
-    * {%- if page %} {%- for doc in page.ancestors[::-1] %} {%- if doc.link %}
+    * {%- if page %} {%- for doc in page.ancestors[::-1] %} {%- if doc.url %}
     * _{_{_ _d_o_c_._t_i_t_l_e_ _}_}
     * {%- else %}
-    * {{ doc.title }} »
+    * {{ doc.title }}
     * {%- endif %} {%- endfor %}
     * {{ page.title }}
     * {%- endif %}
     * {%- block repo %} {%- if page and page.edit_url %} {%- if
       config.repo_name|lower == 'github' %} _{_%_ _t_r_a_n_s_ _r_e_p_o___n_a_m_e_=_c_o_n_f_i_g_._r_e_p_o___n_a_m_e
       _%_}_E_d_i_t_ _o_n_ _{_{_ _r_e_p_o___n_a_m_e_ _}_}_{_%_ _e_n_d_t_r_a_n_s_ _%_} {%- elif config.repo_name|lower
       == 'bitbucket' %} _{_%_ _t_r_a_n_s_ _r_e_p_o___n_a_m_e_=_c_o_n_f_i_g_._r_e_p_o___n_a_m_e_ _%_}_E_d_i_t_ _o_n_ _{
```

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/footer.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/messages.pot` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/nav.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/search.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/versions.html` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/versions.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme.css` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/theme_extra.css` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/img/favicon.ico` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/html5shiv.min.js` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/js/theme.js` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.5.3/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/utils/__init__.py` & `mkdocs-1.5.3/mkdocs/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import EntryPoint, entry_points
 else:
     from importlib_metadata import EntryPoint, entry_points
 
 from mkdocs import exceptions
-from mkdocs.utils.yaml import get_yaml_loader, yaml_load  # noqa - legacy re-export
+from mkdocs.utils.yaml import get_yaml_loader, yaml_load  # noqa: F401 - legacy re-export
 
 if TYPE_CHECKING:
     from mkdocs.structure.pages import Page
 
 T = TypeVar('T')
 
 log = logging.getLogger(__name__)
```

### Comparing `mkdocs-1.5.2/mkdocs/utils/babel_stub.py` & `mkdocs-1.5.3/mkdocs/utils/babel_stub.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/utils/cache.py` & `mkdocs-1.5.3/mkdocs/utils/cache.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/utils/meta.py` & `mkdocs-1.5.3/mkdocs/utils/meta.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/utils/templates.py` & `mkdocs-1.5.3/mkdocs/utils/templates.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/mkdocs/utils/yaml.py` & `mkdocs-1.5.3/mkdocs/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/.gitignore` & `mkdocs-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/LICENSE` & `mkdocs-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/README.md` & `mkdocs-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-1.5.2/pyproject.toml` & `mkdocs-1.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 [tool.hatch.build.hooks.custom]
 dependencies = [
     "babel",
 ]
 
 [tool.hatch.envs.default.scripts]
 all = [
+    "hatch run style:fix",
     "hatch run types:check",
     "hatch run test:test",
-    "hatch run style:check",
     "hatch run lint:check",
     "hatch run +type=default integration:test",
 ]
 
 [tool.hatch.envs.test]
 features = ["i18n"]
 dependencies = [
@@ -156,26 +156,29 @@
 check = "mypy mkdocs"
 
 [tool.hatch.envs.style]
 detached = true
 dependencies = [
     "black",
     "isort",
-    "flake8",
-    "flake8-type-checking",
+    "ruff",
 ]
 [tool.hatch.envs.style.scripts]
-lint = [
-    "flake8 mkdocs",
-]
 check = [
     "isort --check-only --diff mkdocs docs",
     "black -q --check --diff mkdocs docs",
     "lint",
 ]
+lint = [
+    "ruff check mkdocs docs"
+]
+fix = [
+    "ruff check --fix mkdocs docs",
+    "format",
+]
 format = [
     "isort -q mkdocs docs",
     "black -q mkdocs docs",
 ]
 
 [tool.hatch.envs.lint]
 detached = true
@@ -206,12 +209,28 @@
 target-version = ["py37"]  # 3.7
 skip-string-normalization = true
 
 [tool.isort]
 profile = "black"
 line_length = 100
 
+[tool.ruff]
+select = [
+    "F", "W", "E", "UP", "YTT", "C4", "FA", "PIE", "T20", "RSE", "TCH", "DTZ",
+    "B002", "B003", "B005", "B007", "B009", "B012", "B013", "B014", "B015", "B018", "B020", "B021", "B023", "B026", "B033", "B034", "B905",
+    "COM818",
+    "PERF101",
+    "PGH002", "PGH004", "PGH005",
+    "PLE", "PLW0120", "PLW0127",
+    "RUF001", "RUF007", "RUF010", "RUF100", "RUF200",
+    "SIM101", "SIM107", "SIM201", "SIM202", "SIM208", "SIM210", "SIM211", "SIM300", "SIM401", "SIM910",
+]
+ignore = ["E501", "E731"]
+
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = true
+
 [tool.mypy]
 ignore_missing_imports = true
 warn_unreachable = true
 no_implicit_optional = true
 show_error_codes = true
```

### Comparing `mkdocs-1.5.2/PKG-INFO` & `mkdocs-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs
-Version: 1.5.2
+Version: 1.5.3
 Summary: Project documentation with Markdown.
 Project-URL: Documentation, https://www.mkdocs.org/
 Project-URL: Source, https://github.com/mkdocs/mkdocs
 Project-URL: Issues, https://github.com/mkdocs/mkdocs/issues
 Project-URL: History, https://www.mkdocs.org/about/release-notes/
 Author-email: Tom Christie <tom@tomchristie.com>
 License-Expression: BSD-2-Clause
```

