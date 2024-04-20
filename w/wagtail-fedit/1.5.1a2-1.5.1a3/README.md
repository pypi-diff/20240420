# Comparing `tmp/wagtail_fedit-1.5.1a2.tar.gz` & `tmp/wagtail_fedit-1.5.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.1a2.tar", last modified: Tue Apr 16 10:54:06 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.1a3.tar", last modified: Fri Apr 19 16:35:49 2024, max compression
```

## Comparing `wagtail_fedit-1.5.1a2.tar` & `wagtail_fedit-1.5.1a3.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.837822 wagtail_fedit-1.5.1a2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/MANIFEST.in
--rw-rw-rw-   0        0        0    12405 2024-04-16 10:54:06.837822 wagtail_fedit-1.5.1a2/PKG-INFO
--rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.5.1a2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-16 10:54:06.846298 wagtail_fedit-1.5.1a2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.689880 wagtail_fedit-1.5.1a2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.725436 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     4711 2024-04-16 10:41:50.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4691 2024-04-16 10:42:08.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8541 2024-04-16 10:42:15.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.729956 wagtail_fedit-1.5.1a2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3186 2024-04-16 10:05:44.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.662117 wagtail_fedit-1.5.1a2/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.662117 wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.731954 wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.731954 wagtail_fedit-1.5.1a2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.736220 wagtail_fedit-1.5.1a2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.665115 wagtail_fedit-1.5.1a2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.666126 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.738219 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5159 2024-04-16 10:51:46.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.739490 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    17455 2024-04-16 10:50:35.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.667790 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.670476 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.740492 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.740492 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      493 2024-04-16 10:41:00.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.749591 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.757868 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.760887 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.764340 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.768875 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.774889 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10062 2024-04-16 10:41:26.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7418 2024-04-16 10:41:24.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.778237 wagtail_fedit-1.5.1a2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.785781 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.792684 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.819161 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    10055 2024-04-16 10:53:49.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.821100 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.828185 wagtail_fedit-1.5.1a2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6442 2024-04-16 10:36:27.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.837822 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1152 2024-04-16 10:06:54.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:54:06.720185 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12405 2024-04-16 10:54:06.000000 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4043 2024-04-16 10:54:06.000000 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 10:54:06.000000 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-16 10:54:06.000000 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 10:54:06.000000 wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12614 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/PKG-INFO
+-rw-rw-rw-   0        0        0    11357 2024-04-18 16:00:13.000000 wagtail_fedit-1.5.1a3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/pyproject.toml
+-rw-rw-rw-   0        0        0     1188 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.700359 wagtail_fedit-1.5.1a3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.778473 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     6121 2024-04-18 20:22:02.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     4828 2024-04-18 20:24:20.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     1943 2024-04-18 21:37:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.809803 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.605035 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.878071 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5245 2024-04-18 15:52:31.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19376 2024-04-18 15:41:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.622185 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.935345 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.966515 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      889 2024-04-18 15:45:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5980 2024-04-16 13:14:54.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.013475 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.013475 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.045132 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.048488 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.058142 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9382 2024-04-18 14:55:09.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6749 2024-04-18 14:55:07.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.058142 wagtail_fedit-1.5.1a3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.088461 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.140723 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.219894 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    10055 2024-04-16 10:53:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.259044 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    17203 2024-04-18 15:56:15.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.298620 wagtail_fedit-1.5.1a3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6429 2024-04-18 14:10:27.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12614 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4162 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.1a2/LICENSE` & `wagtail_fedit-1.5.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/PKG-INFO` & `wagtail_fedit-1.5.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.1a2
+Version: 1.5.1a3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,14 +23,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
@@ -40,14 +42,16 @@
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
+- [Adapters Python](#adapters-python)
+- [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
 - [How your content is rendered](#how-your-content-is-rendered)
@@ -224,14 +228,22 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
+## Adapters Python
+
+* TBA
+
+## Adapters Javascript
+
+* TBA
+
 ## Hooks
 
 ### wagtail_fedit.construct_adapter_toolbar
 
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
-(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
+wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
+Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
-(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
-[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters Python]
+(#adapters-python) - [Adapters Javascript](#adapters-javascript) - [Hooks]
+(#hooks) - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
+- [Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
 Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
 Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
 (#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
 output-html) - [Implemented](#implemented) Getting Started --------------- 1.
 Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
@@ -98,25 +100,26 @@
 %} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
-block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
-adapter. This is used to display the edit icon for the given adapter. How it is
-called: ```python items = [ FeditAdapterEditButton(), ] for hook in
-hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
-``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
-type. Example of how this type of renderer can be used: ```python
-@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
-This is a custom renderer for the Page model. # It will render the Page model
-as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
-value: format_html( '
+block=item block_id=item.id %} {% endfor %} ``` ## Adapters Python * TBA ##
+Adapters Javascript * TBA ## Hooks ### wagtail_fedit.construct_adapter_toolbar
+Construct the toolbar for the given adapter. This is used to display the edit
+icon for the given adapter. How it is called: ```python items =
+[ FeditAdapterEditButton(), ] for hook in hooks.get_hooks
+(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter) ``` ###
+wagtail_fedit.register_type_renderer Register a custom renderer for a type.
+Example of how this type of renderer can be used: ```python @hooks.register
+(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
+custom renderer for the Page model. # It will render the Page model as a simple
+h2 tag. renderer_map[Page] = lambda request, context, instance, value:
+format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.5.1a2/README.md` & `wagtail_fedit-1.5.1a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
+- [Adapters Python](#adapters-python)
+- [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
 - [How your content is rendered](#how-your-content-is-rendered)
@@ -194,14 +196,22 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
+## Adapters Python
+
+* TBA
+
+## Adapters Javascript
+
+* TBA
+
 ## Hooks
 
 ### wagtail_fedit.construct_adapter_toolbar
 
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
 Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
-(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
-[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters Python]
+(#adapters-python) - [Adapters Javascript](#adapters-javascript) - [Hooks]
+(#hooks) - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
+- [Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
 Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
 Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
 (#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
 output-html) - [Implemented](#implemented) Getting Started --------------- 1.
 Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
@@ -83,25 +84,26 @@
 %} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
-block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
-adapter. This is used to display the edit icon for the given adapter. How it is
-called: ```python items = [ FeditAdapterEditButton(), ] for hook in
-hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
-``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
-type. Example of how this type of renderer can be used: ```python
-@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
-This is a custom renderer for the Page model. # It will render the Page model
-as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
-value: format_html( '
+block=item block_id=item.id %} {% endfor %} ``` ## Adapters Python * TBA ##
+Adapters Javascript * TBA ## Hooks ### wagtail_fedit.construct_adapter_toolbar
+Construct the toolbar for the given adapter. This is used to display the edit
+icon for the given adapter. How it is called: ```python items =
+[ FeditAdapterEditButton(), ] for hook in hooks.get_hooks
+(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter) ``` ###
+wagtail_fedit.register_type_renderer Register a custom renderer for a type.
+Example of how this type of renderer can be used: ```python @hooks.register
+(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
+custom renderer for the Page model. # It will render the Page model as a simple
+h2 tag. renderer_map[Page] = lambda request, context, instance, value:
+format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.5.1a2/setup.cfg` & `wagtail_fedit-1.5.1a3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3161 320d 0a64 6573 6372 6970 7469 6f6e  1a2..description
+00000030: 3161 330d 0a64 6573 6372 6970 7469 6f6e  1a3..description
 00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
 00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
 00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import (
-    Optional, Any,
+    TYPE_CHECKING, Any,
 )
 from django import forms
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from django.utils.text import (
     slugify,
 )
@@ -14,15 +14,22 @@
     HttpRequest,
     HttpResponse,
 )
 
 from ..utils import (
     FeditIFrameMixin,
 )
+from ..utils import (
+    wrap_adapter,
+)
 
+if TYPE_CHECKING:
+    from ..toolbar import (
+        FeditToolbarComponent,
+    )
 
 class AdapterError(Exception):
     pass
 
 
 def content_id_from_parts(*parts: Any) -> str:
     return "-".join(map(slugify, map(str, parts)))
@@ -63,47 +70,98 @@
         self.field_name     = field_name
         self.meta_field     = object._meta.get_field(field_name)
         self.request        = request
         self.kwargs         = kwargs
 
     @property
     def field_value(self):
+        """
+        Call the value_from_object method on
+        the meta field to get the value from the instance.
+        """
         return self.meta_field.value_from_object(self.object)
     
     @property
     def model(self):
+        """
+        Return the model class of the object.
+        """
         return self.object.__class__
     
     def check_permissions(self):
+        """
+        Check if the user has the required permissions to edit the field.
+        If false; the field will be rendered as normal (read only).
+        """
         if not self.request.user.is_authenticated:
             return False
         return True
         
     def get_js_constructor(self) -> str:
+        """
+        Return the JS constructor for the adapter.
+        This is used to link actions from the adapter to the frontend.
+        """
         if not self.js_constructor:
             raise AdapterError("No JS constructor defined")
         
         return self.js_constructor
 
     def get_response_data(self) -> dict:
-        return {}
-    
+        """
+        The data which is returned to the frontend on a successful form submission.
+        """
+        return {
+            "adapter": {
+                "identifier":   self.identifier,
+                "constructor":  self.get_js_constructor(),
+                "element_id":   self.get_element_id(),
+                "model": {
+                    "pk":           self.object.pk,
+                    "app_label":    self.model._meta.app_label,
+                    "model_name":   self.model._meta.model_name,
+                },
+            }
+        }
+
+    def get_toolbar_buttons(self) -> list["FeditToolbarComponent"]:
+        """
+        Extra possible toolbar buttons.
+        This is where for example; the edit icon goes.
+        """
+        return []
+
     def get_element_id(self) -> str:
+        """
+        Return a unique identifier for the elements on the frontend.
+        """
         raise NotImplementedError
     
     def get_form_attrs(self) -> dict:
+        """
+        Extra possible form attributes rendered in the iFrame.
+        """
         return {}
     
     def get_form(self) -> "forms.Form":
+        """
+        Return the form which knows how to handle this datatype.
+        """
         raise NotImplementedError
 
     def form_valid(self, form: "forms.Form"):
+        """
+        Called if the form is valid; useful for saving the form or other things.
+        """
         pass
     
     def form_invalid(self, form: "forms.Form"):
+        """
+        Called if the form is not valid.
+        """
         pass
 
     @classmethod
     def render_from_kwargs(cls, context, **kwargs):
         """
         Render the content for the field from the kwargs if possible.
         This should NOT include the wagtail-fedit wrapper.
@@ -116,52 +174,39 @@
         """
         Render the content for the field.
         This should NOT include the wagtail-fedit wrapper.
         """
         raise NotImplementedError
     
     def encode_shared_context(self) -> dict:
+        """
+        Encode a dictionary to a string.
+        This will be passed as a GET parameter to the iFrame.
+        Make sure the data is not too large.
+        """
         if not self.kwargs:
             return ""
         return self.signer.sign_object(self.kwargs)# , serializer=PickleBlockSerializer)
 
     @classmethod
     def decode_shared_context(cls, context: str) -> dict:
+        """
+        Decode an encoded contex string back to a dictionary.
+        """
         if not context:
             return {}
         return cls.signer.unsign_object(context)# , serializer=PickleBlockSerializer)
-#     
-#     def get_wrapper_template(self) -> str:
-#         return self.wrapper_template
-#     
-#     def get_wrapper_context(self, parent_context: dict = None) -> dict:
-#         return {
-#             "adapter": self,
-#             "request": self.request,
-#             "wagtail_fedit_field": self.field_name,
-#             "wagtail_fedit_instance": self.object,
-#             "parent_context": parent_context,
-#             **self.kwargs,
-#         }
-# 
-#     def render_wrapped(self, parent_context: dict = None):
-#         """
-#         Render the output for the field.
-#         This should INCLUDE the wagtail-fedit wrapper.
-#         """
-# 
-#         template = self.get_wrapper_template()
-#         context = self.get_wrapper_context(parent_context)
-#         content = self.render_content()
-#         context["content"] = content
-# 
-#         if self.run_context_processors:
-#             return render_to_string(
-#                 template,
-#                 context,
-#                 request=self.request
-#             )
-#         
-#         return render_to_string(
-#             template,
-#             context
-#         )
+
+    
+class BlockFieldReplacementAdapter(BaseAdapter):
+    js_constructor = "wagtail_fedit.editors.BlockFieldEditor"
+
+    def get_response_data(self, parent_context = None):
+        data = super().get_response_data()
+        data["html"] = wrap_adapter(
+            request=self.request,
+            adapter=self,
+            context=parent_context,
+            run_context_processors=True
+        )
+        return data
+
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,34 @@
     BoundBlock,
 )
 from wagtail.models import (
     RevisionMixin,
 )
 
 from .base import (
-    BaseAdapter,
+    BlockFieldReplacementAdapter,
     AdapterError,
     VARIABLES,
 )
 from ..forms import (
     blocks as block_forms,
 )
 from .. import utils
 
 
 
 
-class BlockAdapter(BaseAdapter):
+class BlockAdapter(BlockFieldReplacementAdapter):
+    """
+    An adapter for editing Wagtail blocks.
+    This will render the block and replace it on the frontend
+    on successful form submission.
+    """
     identifier = "block"
     required_kwargs = ["block"]
-    js_constructor = "wagtail_fedit.editors.BlockEditor"
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.block = self.kwargs.pop("block", None)
         if self.block:
             if not isinstance(self.block, BoundBlock):
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.models import RevisionMixin
 from wagtail import hooks
 
 from .base import (
-    BaseAdapter,
+    BlockFieldReplacementAdapter,
     VARIABLES,
 )
 from ..hooks import (
     FIELD_EDITOR_SIZE,
 )
 from ..utils import (
     use_related_form,
@@ -26,17 +26,21 @@
 )
 from ..forms import (
     fields as field_forms,
 )
 
 
 
-class FieldAdapter(BaseAdapter):
+class FieldAdapter(BlockFieldReplacementAdapter):
+    """
+    An adapter for editing any model field.
+    This will render the field and replace it on the frontend
+    on successful form submission.
+    """
     identifier = "field"
-    js_constructor = "wagtail_fedit.editors.FieldEditor"
 
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.original_object = object
         self.initial_field_value = self.field_value
 
@@ -205,15 +209,14 @@
                 user=self.request.user,
                 uuid=uid,
                 data=data,
                 content_changed=True,
                 **extra_log_kwargs,
             )
 
-
     def render_content(self, parent_context=None):
         return get_field_content(
             self.request,
             self.original_object,
             self.meta_field,
             parent_context,
         )
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,29 +13,38 @@
 
 
 class AdapterRegistry:
     def __init__(self):
         self.adapters: dict[str, Type[BaseAdapter]] = {}
 
     def __getitem__(self, identifier: str) -> Type[BaseAdapter]:
+        """
+        Retrieve an adapter by its identifier or raise a RegistryLookUpError if not found.
+        """
         try:
             return self.adapters[identifier]
         except KeyError:
             raise RegistryLookUpError(f"No adapter found with identifier '{identifier}'.")
 
     def register(self, adapter_class: Type[BaseAdapter]):
+        """
+        Register an adapter class with the registry.
+        """
         if isinstance(adapter_class, BaseAdapter):
             raise AdapterSubclassError(f"{adapter_class.__class__.__name__} must be a subclass of BaseAdapter; got instance.")
         
         if adapter_class.identifier in self.adapters:
             raise DuplicateAdapterError(f"An adapter with identifier '{adapter_class.identifier}' is already registered.")
 
         self.adapters[adapter_class.identifier] = adapter_class
 
     def unregister(self, identifier):
+        """
+        Unregister an adapter by its identifier.
+        """
         if identifier not in self.adapters:
             raise RegistryLookUpError(f"No adapter found with identifier '{identifier}'.")
 
         del self.adapters[identifier]
 
 
 registry = AdapterRegistry()
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/forms/blocks.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,22 +14,29 @@
 
 class BlockWidgetWithErrors(BlockWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.form_errors = None
 
     def render(self, name, value, attrs=None, renderer=None):
+        """
+        Render the custom blockwidget class with any form errors if they exist.
+        Wagtail does not know about the `form_errors` attribute; this is set later by the BlockForm
+        if the form is invalid.
+        """
         if not self.form_errors:
             return super().render(name, value, attrs, renderer)
         
         return self.render_with_errors(name, value, attrs, self.form_errors, renderer)
 
 
 def get_block_form_class(block: blocks.Block):
-
+    """
+    Return a form class for a block.
+    """
     if isinstance(block, blocks.BoundBlock):
         block = block.block
 
     class BlockForm(BlockEditForm):
         value = BlockField(block=block, widget=BlockWidgetWithErrors(block))
 
     return BlockForm
@@ -47,21 +54,23 @@
             }
 
         super().__init__(*args, **kwargs)
 
     def full_clean(self):
         super().full_clean()
         if self.errors:
+            # Handle any errors which might be from sub-blocks.
             self.fields["value"].widget.form_errors = self.errors["value"]
 
     def save(self):
         block = self.cleaned_data["value"]
         self.block.value.update(block)
-        self.parent_instance.full_clean()
-
+        
+        # Can only save revisions if the parent instance is a RevisionMixin and a request is provided.
+        # Otherwise default to just saving the (live) model instance.
         if isinstance(self.parent_instance, RevisionMixin) and self.request:
             self.parent_instance = self.parent_instance.save_revision(
                 user=self.request.user,
                 log_action=False,
             )
         elif isinstance(self.parent_instance, RevisionMixin) and not self.request:
             warnings.warn((
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/forms/fields.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,37 +11,48 @@
 from wagtail.models import (
     RevisionMixin,
 )
 
 
 
 class PossiblePreviewForm(WagtailAdminModelForm):
+    """
+    A form that can save a revision if the model is a RevisionMixin.
+    Otherwise resorts to the default save method; this saves the (live) instance.
+    """
     def __init__(self, *args, request = None, **kwargs):
         self.request = request
         super().__init__(*args, **kwargs)
 
     def save(self, commit=True):
         instance = super().save(commit=False)
         if commit:
             instance = save_possible_revision(instance, self.request)
         return instance
 
 def save_possible_revision(instance: models.Model, request: HttpRequest, **kwargs) -> models.Model:
+    """
+    Save an instance as a revision if the model supports it.
+    """
     if isinstance(instance, RevisionMixin):
         instance = instance.save_revision(
             user=request.user,
             **kwargs,
         )
         instance = instance.as_object()
     else:
         instance.save()
 
     return instance
 
 def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[PossiblePreviewForm]:
+    """
+    Return a form class for a model with specific fields.
+    This is similar to django's modelform_factory.
+    """
 
     if hasattr(form_model, "get_fedit_form"):
         return form_model.get_fedit_form(form_fields)
 
     class Form(PossiblePreviewForm):
         class Meta:
             model = form_model
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/hooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,150 +51,214 @@
 00000320: 7175 6573 742c 2063 6f6e 7465 7874 2c20  quest, context, 
 00000330: 696e 7374 616e 6365 2c20 7661 6c75 653a  instance, value:
 00000340: 2066 6f72 6d61 745f 6874 6d6c 280d 0a20   format_html(.. 
 00000350: 2020 2020 2020 2027 3c68 323e 7b30 7d3c         '<h2>{0}<
 00000360: 2f68 323e 272c 0d0a 2020 2020 2020 2020  /h2>',..        
 00000370: 7661 6c75 652e 7469 746c 650d 0a20 2020  value.title..   
 00000380: 2029 0d0a 6060 600d 0a22 2222 0d0a 0d0a   )..```.."""....
-00000390: 0d0a 5245 4749 5354 4552 5f46 4945 4c44  ..REGISTER_FIELD
-000003a0: 5f52 454e 4445 5245 5220 203d 2070 7265  _RENDERER  = pre
-000003b0: 6669 7828 2272 6567 6973 7465 725f 6669  fix("register_fi
-000003c0: 656c 645f 7265 6e64 6572 6572 2229 0d0a  eld_renderer")..
-000003d0: 2222 220d 0a23 2323 2077 6167 7461 696c  """..### wagtail
-000003e0: 5f66 6564 6974 2e72 6567 6973 7465 725f  _fedit.register_
-000003f0: 6669 656c 645f 7265 6e64 6572 6572 0d0a  field_renderer..
-00000400: 5265 6769 7374 6572 2061 2063 7573 746f  Register a custo
-00000410: 6d20 7265 6e64 6572 6572 2066 6f72 2061  m renderer for a
-00000420: 2066 6965 6c64 2e0d 0a0d 0a45 7861 6d70   field.....Examp
-00000430: 6c65 206f 6620 686f 7720 7468 6973 2074  le of how this t
-00000440: 7970 6520 6f66 2072 656e 6465 7265 7220  ype of renderer 
-00000450: 6973 2075 7365 6420 696e 2077 6167 7461  is used in wagta
-00000460: 696c 5f68 6f6f 6b73 2f72 656e 6465 7265  il_hooks/rendere
-00000470: 7273 2e70 793a 0d0a 0d0a 6060 6070 7974  rs.py:....```pyt
-00000480: 686f 6e0d 0a40 686f 6f6b 732e 7265 6769  hon..@hooks.regi
-00000490: 7374 6572 2852 4547 4953 5445 525f 4649  ster(REGISTER_FI
-000004a0: 454c 445f 5245 4e44 4552 4552 290d 0a64  ELD_RENDERER)..d
-000004b0: 6566 2072 6567 6973 7465 725f 7265 6e64  ef register_rend
-000004c0: 6572 6572 7328 7265 6e64 6572 6572 5f6d  erers(renderer_m
-000004d0: 6170 293a 0d0a 0d0a 2020 2020 2320 5468  ap):....    # Th
-000004e0: 6973 2069 7320 6120 6375 7374 6f6d 2072  is is a custom r
-000004f0: 656e 6465 7265 7220 666f 7220 5269 6368  enderer for Rich
-00000500: 5465 7874 2066 6965 6c64 732e 0d0a 2020  Text fields...  
-00000510: 2020 2320 4974 2077 696c 6c20 7265 6e64    # It will rend
-00000520: 6572 2074 6865 2052 6963 6854 6578 7420  er the RichText 
-00000530: 6669 656c 6420 6173 2061 2052 6963 6854  field as a RichT
-00000540: 6578 7420 626c 6f63 6b2e 0d0a 2020 2020  ext block...    
-00000550: 7265 6e64 6572 6572 5f6d 6170 5b52 6963  renderer_map[Ric
-00000560: 6854 6578 7446 6965 6c64 5d20 3d5c 0d0a  hTextField] =\..
-00000570: 2020 2020 2020 2020 6c61 6d62 6461 2072          lambda r
-00000580: 6571 7565 7374 2c20 636f 6e74 6578 742c  equest, context,
-00000590: 2069 6e73 7461 6e63 652c 2076 616c 7565   instance, value
-000005a0: 3a20 7269 6368 7465 7874 2876 616c 7565  : richtext(value
-000005b0: 290d 0a60 6060 0d0a 2222 220d 0a0d 0a0d  )..```..""".....
-000005c0: 0a46 4945 4c44 5f45 4449 544f 525f 5349  .FIELD_EDITOR_SI
-000005d0: 5a45 203d 2070 7265 6669 7828 2266 6965  ZE = prefix("fie
-000005e0: 6c64 5f65 6469 746f 725f 7369 7a65 2229  ld_editor_size")
-000005f0: 0d0a 2222 220d 0a23 2323 2077 6167 7461  .."""..### wagta
-00000600: 696c 5f66 6564 6974 2e66 6965 6c64 5f65  il_fedit.field_e
-00000610: 6469 746f 725f 7369 7a65 0d0a 436f 6e74  ditor_size..Cont
-00000620: 726f 6c20 7468 6520 7369 7a65 206f 6620  rol the size of 
-00000630: 7468 6520 6564 6974 6f72 2066 6f72 2074  the editor for t
-00000640: 6865 2067 6976 656e 206d 6f64 656c 2d66  he given model-f
-00000650: 6965 6c64 2074 7970 652e 0d0a 0d0a 4578  ield type.....Ex
-00000660: 616d 706c 6520 6f66 2068 6f77 2074 6869  ample of how thi
-00000670: 7320 686f 6f6b 2069 7320 6361 6c6c 6564  s hook is called
-00000680: 3a0d 0a20 2020 200d 0a20 2020 2060 6060  :..    ..    ```
-00000690: 7079 7468 6f6e 0d0a 2020 2020 666f 7220  python..    for 
-000006a0: 686f 6f6b 2069 6e20 686f 6f6b 732e 6765  hook in hooks.ge
-000006b0: 745f 686f 6f6b 7328 4645 4449 545f 4649  t_hooks(FEDIT_FI
-000006c0: 454c 445f 4544 4954 4f52 5f53 495a 4529  ELD_EDITOR_SIZE)
-000006d0: 3a0d 0a20 2020 2020 2020 2073 697a 6520  :..        size 
-000006e0: 3d20 686f 6f6b 286d 6f64 656c 5f69 6e73  = hook(model_ins
-000006f0: 7461 6e63 652c 206d 6f64 656c 5f66 6965  tance, model_fie
-00000700: 6c64 290d 0a20 2020 2020 2020 2069 6620  ld)..        if 
-00000710: 7369 7a65 3a0d 0a20 2020 2020 2020 2020  size:..         
-00000720: 2020 2072 6574 7572 6e20 7369 7a65 0d0a     return size..
-00000730: 2020 2020 6060 600d 0a22 2222 0d0a 0d0a      ```.."""....
-00000740: 0d0a 4558 434c 5544 455f 4652 4f4d 5f52  ..EXCLUDE_FROM_R
-00000750: 454c 4154 4544 5f46 4f52 4d53 203d 2070  ELATED_FORMS = p
-00000760: 7265 6669 7828 2265 7863 6c75 6465 5f72  refix("exclude_r
-00000770: 656c 6174 6564 5f66 6f72 6d73 2229 0d0a  elated_forms")..
-00000780: 2222 220d 0a23 2323 2077 6167 7461 696c  """..### wagtail
-00000790: 5f66 6564 6974 2e65 7863 6c75 6465 5f72  _fedit.exclude_r
-000007a0: 656c 6174 6564 5f66 6f72 6d73 0d0a 4578  elated_forms..Ex
-000007b0: 636c 7564 6520 7468 6520 6769 7665 6e20  clude the given 
-000007c0: 6d6f 6465 6c20 7479 7065 2066 726f 6d20  model type from 
-000007d0: 7468 6520 7265 6c61 7465 6420 666f 726d  the related form
-000007e0: 732e 0d0a 5468 6973 2069 7320 7573 6564  s...This is used
-000007f0: 2069 6e74 6572 6e61 6c6c 7920 746f 2065   internally to e
-00000800: 7863 6c75 6465 2074 6865 2050 6167 652c  xclude the Page,
-00000810: 2049 6d61 6765 2c20 616e 6420 446f 6375   Image, and Docu
-00000820: 6d65 6e74 206d 6f64 656c 7320 6672 6f6d  ment models from
-00000830: 2074 6865 2072 656c 6174 6564 2066 6f72   the related for
-00000840: 6d73 2e0d 0a54 6869 7320 7761 793b 2074  ms...This way; t
-00000850: 6865 2075 7365 7220 7769 6c6c 2068 6176  he user will hav
-00000860: 6520 7468 6520 6163 7475 616c 2077 6964  e the actual wid
-00000870: 6765 7420 666f 7220 7468 6520 6669 656c  get for the fiel
-00000880: 6420 696e 7374 6561 6420 6f66 2074 6865  d instead of the
-00000890: 2072 656c 6174 6564 2066 6f72 6d2e 0d0a   related form...
-000008a0: 0d0a 4578 616d 706c 6520 6f66 2068 6f77  ..Example of how
-000008b0: 2074 6869 7320 686f 6f6b 2069 7320 6361   this hook is ca
-000008c0: 6c6c 6564 2061 6e64 2068 6f77 2069 7420  lled and how it 
-000008d0: 6973 2075 7365 6420 696e 7465 726e 616c  is used internal
-000008e0: 6c79 3a0d 0a0d 0a60 6060 7079 7468 6f6e  ly:....```python
-000008f0: 0d0a 6465 6620 7573 655f 7265 6c61 7465  ..def use_relate
-00000900: 645f 666f 726d 2866 6965 6c64 3a20 6d6f  d_form(field: mo
-00000910: 6465 6c73 2e46 6965 6c64 2920 2d3e 2062  dels.Field) -> b
-00000920: 6f6f 6c3a 0d0a 2020 2020 666f 7220 686f  ool:..    for ho
-00000930: 6f6b 2069 6e20 686f 6f6b 732e 6765 745f  ok in hooks.get_
-00000940: 686f 6f6b 7328 4558 434c 5544 455f 4652  hooks(EXCLUDE_FR
-00000950: 4f4d 5f52 454c 4154 4544 5f46 4f52 4d53  OM_RELATED_FORMS
-00000960: 293a 0d0a 2020 2020 2020 2020 6966 2068  ):..        if h
-00000970: 6f6f 6b28 6669 656c 6429 3a0d 0a20 2020  ook(field):..   
-00000980: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000990: 4661 6c73 650d 0a20 2020 2072 6574 7572  False..    retur
-000009a0: 6e20 5472 7565 0d0a 0d0a 2020 2020 0d0a  n True....    ..
-000009b0: 4068 6f6f 6b73 2e72 6567 6973 7465 7228  @hooks.register(
-000009c0: 4558 434c 5544 455f 4652 4f4d 5f52 454c  EXCLUDE_FROM_REL
-000009d0: 4154 4544 5f46 4f52 4d53 290d 0a64 6566  ATED_FORMS)..def
-000009e0: 2065 7863 6c75 6465 5f72 656c 6174 6564   exclude_related
-000009f0: 5f66 6f72 6d73 2866 6965 6c64 293a 0d0a  _forms(field):..
-00000a00: 2020 2020 6966 2066 6965 6c64 2e72 656c      if field.rel
-00000a10: 6174 6564 5f6d 6f64 656c 2069 6e20 5b50  ated_model in [P
-00000a20: 6167 652c 2049 6d61 6765 2c20 446f 6375  age, Image, Docu
-00000a30: 6d65 6e74 5d3a 0d0a 2020 2020 2020 2020  ment]:..        
-00000a40: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00000a50: 2072 6574 7572 6e20 4661 6c73 650d 0a60   return False..`
-00000a60: 6060 0d0a 2222 220d 0a0d 0a0d 0a41 4354  ``.."""......ACT
-00000a70: 494f 4e5f 4d45 4e55 5f49 5445 4d5f 4953  ION_MENU_ITEM_IS
-00000a80: 5f53 484f 574e 203d 2070 7265 6669 7828  _SHOWN = prefix(
-00000a90: 2261 6374 696f 6e5f 6d65 6e75 5f69 7465  "action_menu_ite
-00000aa0: 6d5f 6973 5f73 686f 776e 2229 0d0a 2222  m_is_shown")..""
-00000ab0: 220d 0a23 2323 2077 6167 7461 696c 5f66  "..### wagtail_f
-00000ac0: 6564 6974 2e61 6374 696f 6e5f 6d65 6e75  edit.action_menu
-00000ad0: 5f69 7465 6d5f 6973 5f73 686f 776e 0d0a  _item_is_shown..
-00000ae0: 4465 6369 6465 2069 6620 7468 6520 6163  Decide if the ac
-00000af0: 7469 6f6e 206d 656e 7520 6974 656d 2073  tion menu item s
-00000b00: 686f 756c 6420 6265 2073 686f 776e 2066  hould be shown f
-00000b10: 6f72 2074 6865 2067 6976 656e 2069 6e73  or the given ins
-00000b20: 7461 6e63 652e 0d0a 0d0a 5265 7475 726e  tance.....Return
-00000b30: 204e 6f6e 6520 6966 2079 6f75 2063 616e   None if you can
-00000b40: 6e6f 7420 6465 6369 6465 2c20 4661 6c73  not decide, Fals
-00000b50: 6520 6966 2079 6f75 2077 616e 7420 746f  e if you want to
-00000b60: 2068 6964 6520 7468 6520 6974 656d 2c20   hide the item, 
-00000b70: 616e 6420 5472 7565 2069 6620 796f 7520  and True if you 
-00000b80: 7761 6e74 2074 6f20 7368 6f77 2074 6865  want to show the
-00000b90: 2069 7465 6d2e 0d0a 0d0a 4578 616d 706c   item.....Exampl
-00000ba0: 6520 6f66 2068 6f77 2074 6869 7320 686f  e of how this ho
-00000bb0: 6f6b 2069 7320 6361 6c6c 6564 3a0d 0a0d  ok is called:...
-00000bc0: 0a60 6060 7079 7468 6f6e 0d0a 666f 7220  .```python..for 
-00000bd0: 686f 6f6b 2069 6e20 686f 6f6b 732e 6765  hook in hooks.ge
-00000be0: 745f 686f 6f6b 7328 4143 5449 4f4e 5f4d  t_hooks(ACTION_M
-00000bf0: 454e 555f 4954 454d 5f49 535f 5348 4f57  ENU_ITEM_IS_SHOW
-00000c00: 4e29 3a0d 0a20 2020 2072 6573 756c 7420  N):..    result 
-00000c10: 3d20 686f 6f6b 2863 6f6e 7465 7874 2c20  = hook(context, 
-00000c20: 696e 7374 616e 6365 290d 0a20 2020 2069  instance)..    i
-00000c30: 6620 7265 7375 6c74 2069 7320 6e6f 7420  f result is not 
-00000c40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2072  None:..        r
-00000c50: 6574 7572 6e20 7265 7375 6c74 2023 203c  eturn result # <
-00000c60: 2d20 626f 6f6c 0d0a 6060 600d 0a22 2222  - bool..```.."""
-00000c70: 0d0a                                     ..
+00000390: 5245 4749 5354 4552 5f43 5353 203d 2070  REGISTER_CSS = p
+000003a0: 7265 6669 7828 2272 6567 6973 7465 725f  refix("register_
+000003b0: 6373 7322 290d 0a22 2222 0d0a 2323 2320  css").."""..### 
+000003c0: 7761 6774 6169 6c5f 6665 6469 742e 7265  wagtail_fedit.re
+000003d0: 6769 7374 6572 5f63 7373 0d0a 5265 6769  gister_css..Regi
+000003e0: 7374 6572 2061 2063 7573 746f 6d20 4353  ster a custom CS
+000003f0: 5320 6669 6c65 2074 6f20 6265 2069 6e63  S file to be inc
+00000400: 6c75 6465 6420 7768 656e 2074 6865 2075  luded when the u
+00000410: 7469 6c73 2e46 4544 4954 5f50 5245 5649  tils.FEDIT_PREVI
+00000420: 4557 5f56 4152 2069 7320 7365 7420 746f  EW_VAR is set to
+00000430: 2054 7275 652e 0d0a 0d0a 4578 616d 706c   True.....Exampl
+00000440: 6520 6f66 2068 6f77 2074 6869 7320 686f  e of how this ho
+00000450: 6f6b 2069 7320 7573 6564 2069 6e20 7761  ok is used in wa
+00000460: 6774 6169 6c5f 686f 6f6b 732e 7079 3a0d  gtail_hooks.py:.
+00000470: 0a20 2020 200d 0a20 2020 2060 6060 7079  .    ..    ```py
+00000480: 7468 6f6e 0d0a 2020 2020 4068 6f6f 6b73  thon..    @hooks
+00000490: 2e72 6567 6973 7465 7228 5245 4749 5354  .register(REGIST
+000004a0: 4552 5f43 5353 290d 0a20 2020 2064 6566  ER_CSS)..    def
+000004b0: 2072 6567 6973 7465 725f 6373 7328 7265   register_css(re
+000004c0: 7175 6573 7429 3a0d 0a20 2020 2020 2020  quest):..       
+000004d0: 2072 6574 7572 6e20 5b0d 0a20 2020 2020   return [..     
+000004e0: 2020 2020 2020 2066 6f72 6d61 745f 6874         format_ht
+000004f0: 6d6c 280d 0a20 2020 2020 2020 2020 2020  ml(..           
+00000500: 2020 2020 2027 3c6c 696e 6b20 7265 6c3d       '<link rel=
+00000510: 2273 7479 6c65 7368 6565 7422 2068 7265  "stylesheet" hre
+00000520: 663d 227b 307d 223e 272c 0d0a 2020 2020  f="{0}">',..    
+00000530: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00000540: 6963 2827 6373 732f 6375 7374 6f6d 2e63  ic('css/custom.c
+00000550: 7373 2729 0d0a 2020 2020 2020 2020 2020  ss')..          
+00000560: 2020 292c 0d0a 2020 2020 2020 2020 5d0d    ),..        ].
+00000570: 0a20 2020 2060 6060 0d0a 2222 220d 0a0d  .    ```.."""...
+00000580: 0a52 4547 4953 5445 525f 4a53 203d 2070  .REGISTER_JS = p
+00000590: 7265 6669 7828 2272 6567 6973 7465 725f  refix("register_
+000005a0: 6a73 2229 0d0a 2222 220d 0a23 2323 2077  js").."""..### w
+000005b0: 6167 7461 696c 5f66 6564 6974 2e72 6567  agtail_fedit.reg
+000005c0: 6973 7465 725f 6a73 0d0a 5265 6769 7374  ister_js..Regist
+000005d0: 6572 2061 2063 7573 746f 6d20 4a53 2066  er a custom JS f
+000005e0: 696c 6520 746f 2062 6520 696e 636c 7564  ile to be includ
+000005f0: 6564 2077 6865 6e20 7468 6520 7574 696c  ed when the util
+00000600: 732e 4645 4449 545f 5052 4556 4945 575f  s.FEDIT_PREVIEW_
+00000610: 5641 5220 6973 2073 6574 2074 6f20 5472  VAR is set to Tr
+00000620: 7565 2e0d 0a54 6869 7320 6361 6e20 6265  ue...This can be
+00000630: 2075 7365 6420 746f 2072 6567 6973 7465   used to registe
+00000640: 7220 6375 7374 6f6d 2061 6461 7074 6572  r custom adapter
+00000650: 204a 532e 0d0a 0d0a 4578 616d 706c 6520   JS.....Example 
+00000660: 6f66 2068 6f77 2074 6869 7320 686f 6f6b  of how this hook
+00000670: 2069 7320 7573 6564 2069 6e20 7761 6774   is used in wagt
+00000680: 6169 6c5f 686f 6f6b 732e 7079 3a0d 0a20  ail_hooks.py:.. 
+00000690: 2020 200d 0a20 2020 2060 6060 7079 7468     ..    ```pyth
+000006a0: 6f6e 0d0a 2020 2020 4068 6f6f 6b73 2e72  on..    @hooks.r
+000006b0: 6567 6973 7465 7228 5245 4749 5354 4552  egister(REGISTER
+000006c0: 5f4a 5329 0d0a 2020 2020 6465 6620 7265  _JS)..    def re
+000006d0: 6769 7374 6572 5f6a 7328 7265 7175 6573  gister_js(reques
+000006e0: 7429 3a0d 0a20 2020 2020 2020 2072 6574  t):..        ret
+000006f0: 7572 6e20 5b0d 0a20 2020 2020 2020 2020  urn [..         
+00000700: 2020 2066 6f72 6d61 745f 6874 6d6c 280d     format_html(.
+00000710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000720: 2027 3c73 6372 6970 7420 7372 633d 227b   '<script src="{
+00000730: 307d 223e 3c2f 7363 7269 7074 3e27 2c0d  0}"></script>',.
+00000740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000750: 2073 7461 7469 6328 276a 732f 6375 7374   static('js/cust
+00000760: 6f6d 2e6a 7327 290d 0a20 2020 2020 2020  om.js')..       
+00000770: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00000780: 205d 0d0a 2020 2020 6060 600d 0a22 2222   ]..    ```.."""
+00000790: 0d0a 0d0a 0d0a 5245 4749 5354 4552 5f46  ......REGISTER_F
+000007a0: 4945 4c44 5f52 454e 4445 5245 5220 203d  IELD_RENDERER  =
+000007b0: 2070 7265 6669 7828 2272 6567 6973 7465   prefix("registe
+000007c0: 725f 6669 656c 645f 7265 6e64 6572 6572  r_field_renderer
+000007d0: 2229 0d0a 2222 220d 0a23 2323 2077 6167  ").."""..### wag
+000007e0: 7461 696c 5f66 6564 6974 2e72 6567 6973  tail_fedit.regis
+000007f0: 7465 725f 6669 656c 645f 7265 6e64 6572  ter_field_render
+00000800: 6572 0d0a 5265 6769 7374 6572 2061 2063  er..Register a c
+00000810: 7573 746f 6d20 7265 6e64 6572 6572 2066  ustom renderer f
+00000820: 6f72 2061 2066 6965 6c64 2e0d 0a0d 0a45  or a field.....E
+00000830: 7861 6d70 6c65 206f 6620 686f 7720 7468  xample of how th
+00000840: 6973 2074 7970 6520 6f66 2072 656e 6465  is type of rende
+00000850: 7265 7220 6973 2075 7365 6420 696e 2077  rer is used in w
+00000860: 6167 7461 696c 5f68 6f6f 6b73 2f72 656e  agtail_hooks/ren
+00000870: 6465 7265 7273 2e70 793a 0d0a 0d0a 6060  derers.py:....``
+00000880: 6070 7974 686f 6e0d 0a40 686f 6f6b 732e  `python..@hooks.
+00000890: 7265 6769 7374 6572 2852 4547 4953 5445  register(REGISTE
+000008a0: 525f 4649 454c 445f 5245 4e44 4552 4552  R_FIELD_RENDERER
+000008b0: 290d 0a64 6566 2072 6567 6973 7465 725f  )..def register_
+000008c0: 7265 6e64 6572 6572 7328 7265 6e64 6572  renderers(render
+000008d0: 6572 5f6d 6170 293a 0d0a 0d0a 2020 2020  er_map):....    
+000008e0: 2320 5468 6973 2069 7320 6120 6375 7374  # This is a cust
+000008f0: 6f6d 2072 656e 6465 7265 7220 666f 7220  om renderer for 
+00000900: 5269 6368 5465 7874 2066 6965 6c64 732e  RichText fields.
+00000910: 0d0a 2020 2020 2320 4974 2077 696c 6c20  ..    # It will 
+00000920: 7265 6e64 6572 2074 6865 2052 6963 6854  render the RichT
+00000930: 6578 7420 6669 656c 6420 6173 2061 2052  ext field as a R
+00000940: 6963 6854 6578 7420 626c 6f63 6b2e 0d0a  ichText block...
+00000950: 2020 2020 7265 6e64 6572 6572 5f6d 6170      renderer_map
+00000960: 5b52 6963 6854 6578 7446 6965 6c64 5d20  [RichTextField] 
+00000970: 3d5c 0d0a 2020 2020 2020 2020 6c61 6d62  =\..        lamb
+00000980: 6461 2072 6571 7565 7374 2c20 636f 6e74  da request, cont
+00000990: 6578 742c 2069 6e73 7461 6e63 652c 2076  ext, instance, v
+000009a0: 616c 7565 3a20 7269 6368 7465 7874 2876  alue: richtext(v
+000009b0: 616c 7565 290d 0a60 6060 0d0a 2222 220d  alue)..```..""".
+000009c0: 0a0d 0a0d 0a46 4945 4c44 5f45 4449 544f  .....FIELD_EDITO
+000009d0: 525f 5349 5a45 203d 2070 7265 6669 7828  R_SIZE = prefix(
+000009e0: 2266 6965 6c64 5f65 6469 746f 725f 7369  "field_editor_si
+000009f0: 7a65 2229 0d0a 2222 220d 0a23 2323 2077  ze").."""..### w
+00000a00: 6167 7461 696c 5f66 6564 6974 2e66 6965  agtail_fedit.fie
+00000a10: 6c64 5f65 6469 746f 725f 7369 7a65 0d0a  ld_editor_size..
+00000a20: 436f 6e74 726f 6c20 7468 6520 7369 7a65  Control the size
+00000a30: 206f 6620 7468 6520 6564 6974 6f72 2066   of the editor f
+00000a40: 6f72 2074 6865 2067 6976 656e 206d 6f64  or the given mod
+00000a50: 656c 2d66 6965 6c64 2074 7970 652e 0d0a  el-field type...
+00000a60: 0d0a 4578 616d 706c 6520 6f66 2068 6f77  ..Example of how
+00000a70: 2074 6869 7320 686f 6f6b 2069 7320 6361   this hook is ca
+00000a80: 6c6c 6564 3a0d 0a20 2020 200d 0a20 2020  lled:..    ..   
+00000a90: 2060 6060 7079 7468 6f6e 0d0a 2020 2020   ```python..    
+00000aa0: 666f 7220 686f 6f6b 2069 6e20 686f 6f6b  for hook in hook
+00000ab0: 732e 6765 745f 686f 6f6b 7328 4645 4449  s.get_hooks(FEDI
+00000ac0: 545f 4649 454c 445f 4544 4954 4f52 5f53  T_FIELD_EDITOR_S
+00000ad0: 495a 4529 3a0d 0a20 2020 2020 2020 2073  IZE):..        s
+00000ae0: 697a 6520 3d20 686f 6f6b 286d 6f64 656c  ize = hook(model
+00000af0: 5f69 6e73 7461 6e63 652c 206d 6f64 656c  _instance, model
+00000b00: 5f66 6965 6c64 290d 0a20 2020 2020 2020  _field)..       
+00000b10: 2069 6620 7369 7a65 3a0d 0a20 2020 2020   if size:..     
+00000b20: 2020 2020 2020 2072 6574 7572 6e20 7369         return si
+00000b30: 7a65 0d0a 2020 2020 6060 600d 0a22 2222  ze..    ```.."""
+00000b40: 0d0a 0d0a 0d0a 4558 434c 5544 455f 4652  ......EXCLUDE_FR
+00000b50: 4f4d 5f52 454c 4154 4544 5f46 4f52 4d53  OM_RELATED_FORMS
+00000b60: 203d 2070 7265 6669 7828 2265 7863 6c75   = prefix("exclu
+00000b70: 6465 5f72 656c 6174 6564 5f66 6f72 6d73  de_related_forms
+00000b80: 2229 0d0a 2222 220d 0a23 2323 2077 6167  ").."""..### wag
+00000b90: 7461 696c 5f66 6564 6974 2e65 7863 6c75  tail_fedit.exclu
+00000ba0: 6465 5f72 656c 6174 6564 5f66 6f72 6d73  de_related_forms
+00000bb0: 0d0a 4578 636c 7564 6520 7468 6520 6769  ..Exclude the gi
+00000bc0: 7665 6e20 6d6f 6465 6c20 7479 7065 2066  ven model type f
+00000bd0: 726f 6d20 7468 6520 7265 6c61 7465 6420  rom the related 
+00000be0: 666f 726d 732e 0d0a 5468 6973 2069 7320  forms...This is 
+00000bf0: 7573 6564 2069 6e74 6572 6e61 6c6c 7920  used internally 
+00000c00: 746f 2065 7863 6c75 6465 2074 6865 2050  to exclude the P
+00000c10: 6167 652c 2049 6d61 6765 2c20 616e 6420  age, Image, and 
+00000c20: 446f 6375 6d65 6e74 206d 6f64 656c 7320  Document models 
+00000c30: 6672 6f6d 2074 6865 2072 656c 6174 6564  from the related
+00000c40: 2066 6f72 6d73 2e0d 0a54 6869 7320 7761   forms...This wa
+00000c50: 793b 2074 6865 2075 7365 7220 7769 6c6c  y; the user will
+00000c60: 2068 6176 6520 7468 6520 6163 7475 616c   have the actual
+00000c70: 2077 6964 6765 7420 666f 7220 7468 6520   widget for the 
+00000c80: 6669 656c 6420 696e 7374 6561 6420 6f66  field instead of
+00000c90: 2074 6865 2072 656c 6174 6564 2066 6f72   the related for
+00000ca0: 6d2e 0d0a 0d0a 4578 616d 706c 6520 6f66  m.....Example of
+00000cb0: 2068 6f77 2074 6869 7320 686f 6f6b 2069   how this hook i
+00000cc0: 7320 6361 6c6c 6564 2061 6e64 2068 6f77  s called and how
+00000cd0: 2069 7420 6973 2075 7365 6420 696e 7465   it is used inte
+00000ce0: 726e 616c 6c79 3a0d 0a0d 0a60 6060 7079  rnally:....```py
+00000cf0: 7468 6f6e 0d0a 6465 6620 7573 655f 7265  thon..def use_re
+00000d00: 6c61 7465 645f 666f 726d 2866 6965 6c64  lated_form(field
+00000d10: 3a20 6d6f 6465 6c73 2e46 6965 6c64 2920  : models.Field) 
+00000d20: 2d3e 2062 6f6f 6c3a 0d0a 2020 2020 666f  -> bool:..    fo
+00000d30: 7220 686f 6f6b 2069 6e20 686f 6f6b 732e  r hook in hooks.
+00000d40: 6765 745f 686f 6f6b 7328 4558 434c 5544  get_hooks(EXCLUD
+00000d50: 455f 4652 4f4d 5f52 454c 4154 4544 5f46  E_FROM_RELATED_F
+00000d60: 4f52 4d53 293a 0d0a 2020 2020 2020 2020  ORMS):..        
+00000d70: 6966 2068 6f6f 6b28 6669 656c 6429 3a0d  if hook(field):.
+00000d80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000d90: 7572 6e20 4661 6c73 650d 0a20 2020 2072  urn False..    r
+00000da0: 6574 7572 6e20 5472 7565 0d0a 0d0a 2020  eturn True....  
+00000db0: 2020 0d0a 4068 6f6f 6b73 2e72 6567 6973    ..@hooks.regis
+00000dc0: 7465 7228 4558 434c 5544 455f 4652 4f4d  ter(EXCLUDE_FROM
+00000dd0: 5f52 454c 4154 4544 5f46 4f52 4d53 290d  _RELATED_FORMS).
+00000de0: 0a64 6566 2065 7863 6c75 6465 5f72 656c  .def exclude_rel
+00000df0: 6174 6564 5f66 6f72 6d73 2866 6965 6c64  ated_forms(field
+00000e00: 293a 0d0a 2020 2020 6966 2066 6965 6c64  ):..    if field
+00000e10: 2e72 656c 6174 6564 5f6d 6f64 656c 2069  .related_model i
+00000e20: 6e20 5b50 6167 652c 2049 6d61 6765 2c20  n [Page, Image, 
+00000e30: 446f 6375 6d65 6e74 5d3a 0d0a 2020 2020  Document]:..    
+00000e40: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+00000e50: 0a20 2020 2072 6574 7572 6e20 4661 6c73  .    return Fals
+00000e60: 650d 0a60 6060 0d0a 2222 220d 0a0d 0a0d  e..```..""".....
+00000e70: 0a41 4354 494f 4e5f 4d45 4e55 5f49 5445  .ACTION_MENU_ITE
+00000e80: 4d5f 4953 5f53 484f 574e 203d 2070 7265  M_IS_SHOWN = pre
+00000e90: 6669 7828 2261 6374 696f 6e5f 6d65 6e75  fix("action_menu
+00000ea0: 5f69 7465 6d5f 6973 5f73 686f 776e 2229  _item_is_shown")
+00000eb0: 0d0a 2222 220d 0a23 2323 2077 6167 7461  .."""..### wagta
+00000ec0: 696c 5f66 6564 6974 2e61 6374 696f 6e5f  il_fedit.action_
+00000ed0: 6d65 6e75 5f69 7465 6d5f 6973 5f73 686f  menu_item_is_sho
+00000ee0: 776e 0d0a 4465 6369 6465 2069 6620 7468  wn..Decide if th
+00000ef0: 6520 6163 7469 6f6e 206d 656e 7520 6974  e action menu it
+00000f00: 656d 2073 686f 756c 6420 6265 2073 686f  em should be sho
+00000f10: 776e 2066 6f72 2074 6865 2067 6976 656e  wn for the given
+00000f20: 2069 6e73 7461 6e63 652e 0d0a 0d0a 5265   instance.....Re
+00000f30: 7475 726e 204e 6f6e 6520 6966 2079 6f75  turn None if you
+00000f40: 2063 616e 6e6f 7420 6465 6369 6465 2c20   cannot decide, 
+00000f50: 4661 6c73 6520 6966 2079 6f75 2077 616e  False if you wan
+00000f60: 7420 746f 2068 6964 6520 7468 6520 6974  t to hide the it
+00000f70: 656d 2c20 616e 6420 5472 7565 2069 6620  em, and True if 
+00000f80: 796f 7520 7761 6e74 2074 6f20 7368 6f77  you want to show
+00000f90: 2074 6865 2069 7465 6d2e 0d0a 0d0a 4578   the item.....Ex
+00000fa0: 616d 706c 6520 6f66 2068 6f77 2074 6869  ample of how thi
+00000fb0: 7320 686f 6f6b 2069 7320 6361 6c6c 6564  s hook is called
+00000fc0: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00000fd0: 666f 7220 686f 6f6b 2069 6e20 686f 6f6b  for hook in hook
+00000fe0: 732e 6765 745f 686f 6f6b 7328 4143 5449  s.get_hooks(ACTI
+00000ff0: 4f4e 5f4d 454e 555f 4954 454d 5f49 535f  ON_MENU_ITEM_IS_
+00001000: 5348 4f57 4e29 3a0d 0a20 2020 2072 6573  SHOWN):..    res
+00001010: 756c 7420 3d20 686f 6f6b 2863 6f6e 7465  ult = hook(conte
+00001020: 7874 2c20 696e 7374 616e 6365 290d 0a20  xt, instance).. 
+00001030: 2020 2069 6620 7265 7375 6c74 2069 7320     if result is 
+00001040: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00001050: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00001060: 2023 203c 2d20 626f 6f6c 0d0a 6060 600d   # <- bool..```.
+00001070: 0a22 2222 0d0a                           ."""..
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/models.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 .wagtail-fedit-buttons {
     display: flex;
 }
 
 .wagtail-fedit-adapter-wrapper {
     position: relative;
+    min-height: 24px;
+}
+.wagtail-fedit-field_bg_image {
+    display: inline-flex;
 }
 .wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
     content: '';
     display: block;
     position: absolute;
     top: 0;
     left: 0;
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 5% similar despite different names*

```diff
@@ -97,21 +97,22 @@
 
 .wagtail-fedit-form-wrapper {
     display: flex;
     flex-direction: column;
     height: 100%;
     gap: 1em;
 }
-.wagtail-fedit-form-wrapper form {
+.wagtail-fedit-form-wrapper #wagtail-fedit-form {
     display: flex;
     flex-direction: column;
     justify-content: space-between;
     flex: 1;
 }
-.wagtail-fedit-form-wrapper form input {
+.wagtail-fedit-form-wrapper #wagtail-fedit-form .field > input
+.wagtail-fedit-form-wrapper #wagtail-fedit-form .field > * > input {
     margin-bottom: 0.5em;
 }
 .wagtail-fedit-form-wrapper .wagtail-fedit-form {
     display: flex;
     flex-direction: column;
 }
 .wagtail-fedit-form-wrapper .wagtail-fedit-publish-form {
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -117,15 +117,15 @@
 
     closeModal() {
         this.#editor.closeModal();
     }
 }
 
 
-class WagtailFeditEditor {
+class BaseWagtailFeditEditor {
     constructor(options) {
         const {
             element = null,
         } = options;
 
         this.initialTitle = document.title;
 
@@ -188,15 +188,15 @@
                                 this.iframe.window.initBlockWidget(uninitializedBlock.id);
                             }
 
                             const cancelButton = this.iframe.document.querySelector(".wagtail-fedit-cancel-button");
                             cancelButton.addEventListener("click", this.closeModal.bind(this));
                             return;
                         }
-                        this.setWrapperHtml(response.html);
+                        this.onResponse(response);
                         this.closeModal();
 
                         const event = new CustomEvent("wagtail-fedit:change", {
                             detail: {
                                 element: this.wrapperElement,
                             }
                         });
@@ -248,55 +248,21 @@
         const closeBtn = document.createElement("button");
         closeBtn.innerHTML = "&times;";
         closeBtn.classList.add("wagtail-fedit-close-button");
         closeBtn.addEventListener("click", this.closeModal.bind(this));
         this.modal.appendChild(closeBtn);
     }
 
-    setWrapperHtml(html) {
-
-        const anim = this.wrapperElement.animate([{
-            opacity: 1
-        }, {
-            opacity: 0
-        }, ], {
-            duration: 350,
-            easing: "ease-in-out",
-        });
-
-        anim.onfinish = () => {
-            const newBlock = document.createElement("div");
-            newBlock.innerHTML = html;
-            const blockWrapper = newBlock.firstElementChild;
-            blockWrapper.classList.add("wagtail-fedit-initialized");
-            this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
-            this.wrapperElement.parentNode.removeChild(this.wrapperElement);
-            blockWrapper.style.opacity = 0;
-            this.wrapperElement = blockWrapper;
-            this.initNewEditors();
-            this.init();
-
-            const anim = blockWrapper.animate([{
-                opacity: 0
-            }, {
-                opacity: 1
-            }, ], {
-                duration: 350,
-                easing: "ease-in-out",
-            });
-            anim.onfinish = () => {
-                blockWrapper.style.opacity = 1;
-            };
-        }
-    }
-
     closeModal() {
         this.modalWrapper.remove();
         window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]);
         document.title = this.initialTitle;
+        if ("onModalClose" in this) {
+            this.onModalClose();
+        }
     }
 
     get modalWrapper() {
         const modalWrapper = document.querySelector("#wagtail-fedit-modal-wrapper");
         if (modalWrapper) {
             return modalWrapper;
         }
@@ -340,14 +306,100 @@
                     console.error("No editor class found for element", editor);
                 }
             }
         }
     }
 }
 
+
+class BaseFuncEditor extends BaseWagtailFeditEditor {
+    static get funcMap() {
+        return window
+    }
+
+    onResponse(response) {
+        const name = response.func.name;
+        const targetElementSelector = response.func.target;
+        if (!name || !targetElementSelector) {
+            console.error("Invalid response", response);
+            return;
+        }
+
+        const targetElement = document.querySelector(targetElementSelector);
+        if (!targetElement) {
+            console.error("Target element not found", targetElementSelector);
+            return;
+        }
+
+        const func = this.constructor.funcMap[name];
+        if (!func) {
+            console.error("Function not found", name);
+            return;
+        }
+
+        func(targetElement, response);
+    }
+}
+
+
+class WagtailFeditFuncEditor extends BaseFuncEditor {
+    static get funcMap() {
+        return window.wagtailFedit.funcs;
+    }
+}
+
+
+class BlockFieldEditor extends BaseWagtailFeditEditor {
+    onResponse(response) {
+        const html = response.html;
+
+        // Fade out the old block
+        const anim = this.wrapperElement.animate([{
+            opacity: 1
+        }, {
+            opacity: 0
+        }, ], {
+            duration: 350,
+            easing: "ease-in-out",
+        });
+
+        anim.onfinish = () => {
+            // replace the HTML of the block we are editing with the new HTML
+            const newBlock = document.createElement("div");
+            newBlock.innerHTML = html;
+            const blockWrapper = newBlock.firstElementChild;
+            blockWrapper.classList.add("wagtail-fedit-initialized");
+            this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
+            this.wrapperElement.parentNode.removeChild(this.wrapperElement);
+            blockWrapper.style.opacity = 0;
+            this.wrapperElement = blockWrapper;
+
+            // reinitialize possibly new / replaced editor instances
+            this.initNewEditors();
+
+            // reinitialize proper variables with from new HTML
+            this.init();
+
+            // Fade in the new block
+            const anim = blockWrapper.animate([{
+                opacity: 0
+            }, {
+                opacity: 1
+            }, ], {
+                duration: 350,
+                easing: "ease-in-out",
+            });
+            anim.onfinish = () => {
+                blockWrapper.style.opacity = 1;
+            };
+        }
+    }
+}
+
+
 class WagtailFeditPublishMenu {
     constructor(publishButton) {
         this.publishButton = publishButton;
         this.publishButtonsWrapper = publishButton.parentElement.querySelector(".wagtail-fedit-form-buttons");
         const buttons = this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button");
         let initialIsHidden = false;
         for (const button of buttons) {
@@ -403,22 +455,24 @@
             anim.onfinish = () => {
                 this.publishButtonsWrapper.classList.add("open");
             };
         });
     }
 }
 
+
 function getEditorClass(element) {
     const editorClass = element.dataset.feditConstructor;
     if (editorClass) {
         return window.wagtailFedit.editors[editorClass];
     }
     return null;
 }
 
+
 function initFEditors() {
     const editors = document.querySelectorAll(".wagtail-fedit-adapter-wrapper");
     for (const editor of editors) {
         if (!editor.classList.contains("wagtail-fedit-initialized")) {
             editor.classList.add("wagtail-fedit-initialized");
             const editorClass = getEditorClass(editor);
             if (editorClass) {
@@ -503,24 +557,40 @@
 
         if (publishMenu) {
             const publisher = new WagtailFeditPublishMenu(publishMenu);
         }
     }
 }
 
+
+function wagtailFeditBackgroundImageAdapter(element, response) {
+    const url = response.url;
+    element.style.backgroundImage = `url(${url})`;
+}
+
+
 document.addEventListener("DOMContentLoaded", initFEditors);
 
 
 window.wagtailFedit = {
     initFEditors,
-    WagtailFeditEditor,
+    BaseWagtailFeditEditor,
+    BaseFuncEditor,
+    BlockFieldEditor,
     WagtailFeditPublishMenu,
     WagtailFeditorAPI,
     iFrame,
     editors: {
-        "wagtail_fedit.editors.BlockEditor": WagtailFeditEditor,
-        "wagtail_fedit.editors.FieldEditor": WagtailFeditEditor,
+        "wagtail_fedit.editors.BaseFuncEditor": BaseFuncEditor,
+        "wagtail_fedit.editors.BlockFieldEditor": BlockFieldEditor,
+        "wagtail_fedit.editors.WagtailFeditFuncEditor": WagtailFeditFuncEditor,
+    },
+    funcs: {
+        "wagtail_fedit.funcs.backgroundImageFunc": wagtailFeditBackgroundImageAdapter,
     },
     register: function(name, editor) {
         this.editors[name] = editor;
     },
+    registerFunc: function(name, func) {
+        this.funcs[name] = func;
+    },
 };
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% load i18n wagtailadmin_tags %}
 
 {% block content %}
     <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
 
         {{ block.super }}
 
-        <form id="wagtail-fedit-form" action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
+        <form id="wagtail-fedit-form" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
             {% csrf_token %}
             {% block form %}
                 {% panel id="wagtail-fedit-editor" icon="draft" heading=meta_field.verbose_name %}
                     <div class="wagtail-fedit-form">
                         {% for field in form %}
                             {% include "./field.html" %}
                         {% endfor %}
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         {% block header %}
             <header id="modal-header">
                 <h1 id="modal-title">{{ view.get_header_title }}</h1>
             </header>
         {% endblock %}
         <div class="messages" role="status">
             {# Always show messages div so it can be appended to by JS #}
-            {% if messages or form.errors %}
+            {% if messages or form.non_field_errors %}
                 <ul>
-                    {% if form.errors %}
+                    {% if form.non_field_errors %}
                         {% for error in form.non_field_errors %}
                             <li class="error">{{ error }}</li>
                         {% endfor %}
                     {% endif %}
                     {% for message in messages %}
                         <li class="{{ message.tags }}">{{ message }}</li>
                     {% endfor %}
@@ -68,22 +68,23 @@
                         <p>{% translate "This object is locked and cannot be edited." %}</p>
                     {% endhelp_block %}
                 {% endpanel %}
             {% else %}
             
                 {% block content %}
                     {% block errors %}
-                        {% if form.errors or form.non_field_errors %}
+                        {% if form.errors %}
                             <div class="error-message">
                                 <h2>{{ view.get_error_title }}</h2>
                                 <ul>
-                                    {% for error in form.non_field_errors %}
-                                        <li>{{ error }}</li>
+                                    {% for field in form %}
+                                        {% for error in field.errors %}
+                                            <li class="error">{{ field.label }}: {{ error }}</li>
+                                        {% endfor %}
                                     {% endfor %}
-                                    {{ form.errors.as_ul }}
                                 </ul>
                             </div>
                         {% endif %}
                     {% endblock %}
                 {% endblock %}
                 
             {% endif %}
```

#### html2text {}

```diff
@@ -4,16 +4,16 @@
 {% endblock %} {% block extra_js %}
 {% block page_js %}{% include "wagtailadmin/pages/_editor_js.html" %}{%
 endblock %} {{ block.super }} {{ form.media.js }} {% endblock %} {% block
 furniture %} {% block header %}
 ************ {{{{ vviieeww..ggeett__hheeaaddeerr__ttiittllee }}}} ************
 {% endblock %}
 {# Always show messages div so it can be appended to by JS #} {% if messages or
-form.errors %}
-    * {% if form.errors %} {% for error in form.non_field_errors %}
+form.non_field_errors %}
+    * {% if form.non_field_errors %} {% for error in form.non_field_errors %}
     * {{ error }}
     * {% endfor %} {% endif %} {% for message in messages %}
     * {{ message }}
     * {% endfor %}
 {% endif %}
 {% if help_text %} {% panel id="wagtail-fedit-help-text" icon="help"
 heading=help_text.heading %} {% help_block status=help_text.status %}
@@ -26,19 +26,19 @@
 {% translate "This object is locked" %}
 {% translate "You are still able to edit this object." %}
 {% endhelp_block %} {% endpanel %} {% endif %} {% if locked_for_user %} {%
 panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %} {%
 help_block status="info" %}
 {% translate "This object is locked and cannot be edited." %}
 {% endhelp_block %} {% endpanel %} {% else %} {% block content %} {% block
-errors %} {% if form.errors or form.non_field_errors %}
+errors %} {% if form.errors %}
 ********** {{{{ vviieeww..ggeett__eerrrroorr__ttiittllee }}}} **********
-    * {% for error in form.non_field_errors %}
-    * {{ error }}
-    * {% endfor %} {{ form.errors.as_ul }}
+    * {% for field in form %} {% for error in field.errors %}
+    * {{ field.label }}: {{ error }}
+    * {% endfor %} {% endfor %}
 {% endif %} {% endblock %} {% endblock %} {% endif %}
 {% block sidebar_root %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,33 +1,34 @@
 magic:    0xa70d0d0a
-moddate:  0xd4551e66 (Tue Apr 16 10:41:24 2024 UTC)
-files sz: 7418
+moddate:  0x4b342166 (Thu Apr 18 14:55:07 2024 UTC)
+files sz: 6749
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 11
+   stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a096d0a5a
-      0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e0100640064066c0f6d
-      105a100100640064076c116d125a120100640064086c136d145a14010064
-      0064096c156d165a1601006400640a6c175a17640b640c6c186d195a1901
-      00640b640d6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640b640e6c
-      1f6d205a200100640b640f6c166d215a210100020065036a220000000000
-      000000a6000000ab0000000000000000005a2364105a2464115a25020047
-      006412840064136504a6030000ab0300000000000000005a266523a02700
-      000000000000000000000000000000000000006414ac15a6010000ab0100
-      000000000000006416650c6417650d660464188404a6000000ab00000000
-      00000000005a286426641a6510641b651d641c6529641d652a641e652b66
-      0a641f84055a2c6523a02d00000000000000000000000000000000000000
-      006420ac21a6010000ab010000000000000000641c650a641b651d641e65
-      2b660664228404a6000000ab0000000000000000005a2e64276416650c64
-      23652f652b190000000000000000006424652f652b190000000000000000
-      00641e65296608642584055a30640a5300
+      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
+      00640064076c106d115a110100640064086c126d135a130100640064096c
+      145a14640a640b6c156d165a166d175a176d185a186d195a190100640a64
+      0c6c1a6d1b5a1b6d1c5a1c6d1d5a1d0100640a640d6c136d1e5a1e6d1f5a
+      1f0100020065036a200000000000000000a6000000ab0000000000000000
+      005a21640e5a22640f5a23020047006410840064116504a6030000ab0300
+      000000000000005a246521a0250000000000000000000000000000000000
+      0000006412ac13a6010000ab010000000000000000641465096415650a66
+      0464168404a6000000ab0000000000000000005a266521a0270000000000
+      0000000000000000000000000000006417ac18a6010000ab010000000000
+      00000064196507641a6518641b65286606641c8404a6000000ab00000000
+      00000000005a296521a02a00000000000000000000000000000000000000
+      00641d641e6417ac1fa6030000ab030000000000000000641b652b660264
+      208404a6000000ab0000000000000000005a2c6424641465096421652d65
+      28190000000000000000006422652d652819000000000000000000641b65
+      2b6608642384055a2e64095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -41,269 +42,261 @@
                 24 IMPORT_FROM              4 (Node)
                 26 STORE_NAME               4 (Node)
                 28 IMPORT_FROM              5 (TemplateSyntaxError)
                 30 STORE_NAME               5 (TemplateSyntaxError)
                 32 POP_TOP
    
      5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('render_to_string',))
-                38 IMPORT_NAME              6 (django.template.loader)
-                40 IMPORT_FROM              7 (render_to_string)
-                42 STORE_NAME               7 (render_to_string)
+                36 LOAD_CONST               3 (('Context',))
+                38 IMPORT_NAME              6 (django.template.context)
+                40 IMPORT_FROM              7 (Context)
+                42 STORE_NAME               7 (Context)
                 44 POP_TOP
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('make_context', 'Context'))
-                50 IMPORT_NAME              8 (django.template.context)
-                52 IMPORT_FROM              9 (make_context)
-                54 STORE_NAME               9 (make_context)
-                56 IMPORT_FROM             10 (Context)
-                58 STORE_NAME              10 (Context)
-                60 POP_TOP
-   
-    10          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('Parser', 'Token', 'FilterExpression'))
-                66 IMPORT_NAME             11 (django.template.base)
-                68 IMPORT_FROM             12 (Parser)
-                70 STORE_NAME              12 (Parser)
-                72 IMPORT_FROM             13 (Token)
-                74 STORE_NAME              13 (Token)
-                76 IMPORT_FROM             14 (FilterExpression)
-                78 STORE_NAME              14 (FilterExpression)
-                80 POP_TOP
-   
-    14          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               6 (('HttpRequest',))
-                86 IMPORT_NAME             15 (django.http)
-                88 IMPORT_FROM             16 (HttpRequest)
-                90 STORE_NAME              16 (HttpRequest)
-                92 POP_TOP
-   
-    15          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               7 (('reverse',))
-                98 IMPORT_NAME             17 (django.urls)
-               100 IMPORT_FROM             18 (reverse)
-               102 STORE_NAME              18 (reverse)
-               104 POP_TOP
-   
-    16         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('signing',))
-               110 IMPORT_NAME             19 (django.core)
-               112 IMPORT_FROM             20 (signing)
-               114 STORE_NAME              20 (signing)
-               116 POP_TOP
-   
-    18         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               9 (('hooks',))
-               122 IMPORT_NAME             21 (wagtail)
-               124 IMPORT_FROM             22 (hooks)
-               126 STORE_NAME              22 (hooks)
-               128 POP_TOP
-   
-    20         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (None)
-               134 IMPORT_NAME             23 (warnings)
-               136 STORE_NAME              23 (warnings)
-   
-    22         138 LOAD_CONST              11 (2)
-               140 LOAD_CONST              12 (('FeditAdapterEditButton',))
-               142 IMPORT_NAME             24 (toolbar)
-               144 IMPORT_FROM             25 (FeditAdapterEditButton)
-               146 STORE_NAME              25 (FeditAdapterEditButton)
-               148 POP_TOP
-   
-    25         150 LOAD_CONST              11 (2)
-               152 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
-               154 IMPORT_NAME             26 (adapters)
-               156 IMPORT_FROM             27 (adapter_registry)
-               158 STORE_NAME              27 (adapter_registry)
-               160 IMPORT_FROM             28 (RegistryLookUpError)
-               162 STORE_NAME              28 (RegistryLookUpError)
-               164 IMPORT_FROM             29 (BaseAdapter)
-               166 STORE_NAME              29 (BaseAdapter)
-               168 IMPORT_FROM             30 (AdapterError)
-               170 STORE_NAME              30 (AdapterError)
-               172 POP_TOP
-   
-    31         174 LOAD_CONST              11 (2)
-               176 LOAD_CONST              14 (('_can_edit',))
-               178 IMPORT_NAME             31 (utils)
-               180 IMPORT_FROM             32 (_can_edit)
-               182 STORE_NAME              32 (_can_edit)
-               184 POP_TOP
-   
-    34         186 LOAD_CONST              11 (2)
-               188 LOAD_CONST              15 (('CONSTRUCT_ADAPTER_TOOLBAR',))
-               190 IMPORT_NAME             22 (hooks)
-               192 IMPORT_FROM             33 (CONSTRUCT_ADAPTER_TOOLBAR)
-               194 STORE_NAME              33 (CONSTRUCT_ADAPTER_TOOLBAR)
-               196 POP_TOP
-   
-    39         198 PUSH_NULL
-               200 LOAD_NAME                3 (library)
-               202 LOAD_ATTR               34 (Library)
-               212 PRECALL                  0
-               216 CALL                     0
-               226 STORE_NAME              35 (register)
-   
-    42         228 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
-               230 STORE_NAME              36 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    43         232 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
-               234 STORE_NAME              37 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    47         236 PUSH_NULL
-               238 LOAD_BUILD_CLASS
-               240 LOAD_CONST              18 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 47>)
-               242 MAKE_FUNCTION            0
-               244 LOAD_CONST              19 ('AdapterNode')
-               246 LOAD_NAME                4 (Node)
-               248 PRECALL                  3
-               252 CALL                     3
-               262 STORE_NAME              38 (AdapterNode)
-   
-   124         264 LOAD_NAME               35 (register)
-               266 LOAD_METHOD             39 (tag)
-               288 LOAD_CONST              20 ('fedit')
-               290 KW_NAMES                21
-               292 PRECALL                  1
-               296 CALL                     1
-   
-   125         306 LOAD_CONST              22 ('parser')
-               308 LOAD_NAME               12 (Parser)
-               310 LOAD_CONST              23 ('token')
-               312 LOAD_NAME               13 (Token)
-               314 BUILD_TUPLE              4
-               316 LOAD_CONST              24 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 124>)
-               318 MAKE_FUNCTION            4 (annotations)
-   
-   124         320 PRECALL                  0
-               324 CALL                     0
-   
-   125         334 STORE_NAME              40 (do_render_fedit)
-   
-   163         336 LOAD_CONST              38 ((False,))
-               338 LOAD_CONST              26 ('request')
-               340 LOAD_NAME               16 (HttpRequest)
-               342 LOAD_CONST              27 ('adapter')
-               344 LOAD_NAME               29 (BaseAdapter)
-               346 LOAD_CONST              28 ('context')
-               348 LOAD_NAME               41 (dict)
-               350 LOAD_CONST              29 ('run_context_processors')
-               352 LOAD_NAME               42 (bool)
-               354 LOAD_CONST              30 ('return')
-               356 LOAD_NAME               43 (str)
-               358 BUILD_TUPLE             10
-               360 LOAD_CONST              31 (<code object wrap_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 163>)
-               362 MAKE_FUNCTION            5 (defaults, annotations)
-               364 STORE_NAME              44 (wrap_adapter)
-   
-   206         366 LOAD_NAME               35 (register)
-               368 LOAD_METHOD             45 (simple_tag)
-               390 LOAD_CONST              32 (True)
-               392 KW_NAMES                33
-               394 PRECALL                  1
-               398 CALL                     1
-   
-   207         408 LOAD_CONST              28 ('context')
-               410 LOAD_NAME               10 (Context)
-               412 LOAD_CONST              27 ('adapter')
-               414 LOAD_NAME               29 (BaseAdapter)
-               416 LOAD_CONST              30 ('return')
-               418 LOAD_NAME               43 (str)
-               420 BUILD_TUPLE              6
-               422 LOAD_CONST              34 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 206>)
-               424 MAKE_FUNCTION            4 (annotations)
-   
-   206         426 PRECALL                  0
-               430 CALL                     0
-   
-   207         440 STORE_NAME              46 (render_adapter)
-   
-   223         442 LOAD_CONST              39 ((None,))
-               444 LOAD_CONST              22 ('parser')
-               446 LOAD_NAME               12 (Parser)
-               448 LOAD_CONST              35 ('tokens')
-               450 LOAD_NAME               47 (list)
-               452 LOAD_NAME               43 (str)
-               454 BINARY_SUBSCR
-               464 LOAD_CONST              36 ('kwarg_list')
-               466 LOAD_NAME               47 (list)
-               468 LOAD_NAME               43 (str)
-               470 BINARY_SUBSCR
-               480 LOAD_CONST              30 ('return')
-               482 LOAD_NAME               41 (dict)
-               484 BUILD_TUPLE              8
-               486 LOAD_CONST              37 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 223>)
-               488 MAKE_FUNCTION            5 (defaults, annotations)
-               490 STORE_NAME              48 (get_kwargs)
-               492 LOAD_CONST              10 (None)
-               494 RETURN_VALUE
+     8          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('Parser', 'Token', 'FilterExpression'))
+                50 IMPORT_NAME              8 (django.template.base)
+                52 IMPORT_FROM              9 (Parser)
+                54 STORE_NAME               9 (Parser)
+                56 IMPORT_FROM             10 (Token)
+                58 STORE_NAME              10 (Token)
+                60 IMPORT_FROM             11 (FilterExpression)
+                62 STORE_NAME              11 (FilterExpression)
+                64 POP_TOP
+   
+    12          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               5 (('HttpRequest',))
+                70 IMPORT_NAME             12 (django.http)
+                72 IMPORT_FROM             13 (HttpRequest)
+                74 STORE_NAME              13 (HttpRequest)
+                76 POP_TOP
+   
+    13          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               6 (('reverse',))
+                82 IMPORT_NAME             14 (django.urls)
+                84 IMPORT_FROM             15 (reverse)
+                86 STORE_NAME              15 (reverse)
+                88 POP_TOP
+   
+    14          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               7 (('signing',))
+                94 IMPORT_NAME             16 (django.core)
+                96 IMPORT_FROM             17 (signing)
+                98 STORE_NAME              17 (signing)
+               100 POP_TOP
+   
+    16         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('hooks',))
+               106 IMPORT_NAME             18 (wagtail)
+               108 IMPORT_FROM             19 (hooks)
+               110 STORE_NAME              19 (hooks)
+               112 POP_TOP
+   
+    18         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST               9 (None)
+               118 IMPORT_NAME             20 (warnings)
+               120 STORE_NAME              20 (warnings)
+   
+    20         122 LOAD_CONST              10 (2)
+               124 LOAD_CONST              11 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               126 IMPORT_NAME             21 (adapters)
+               128 IMPORT_FROM             22 (adapter_registry)
+               130 STORE_NAME              22 (adapter_registry)
+               132 IMPORT_FROM             23 (RegistryLookUpError)
+               134 STORE_NAME              23 (RegistryLookUpError)
+               136 IMPORT_FROM             24 (BaseAdapter)
+               138 STORE_NAME              24 (BaseAdapter)
+               140 IMPORT_FROM             25 (AdapterError)
+               142 STORE_NAME              25 (AdapterError)
+               144 POP_TOP
+   
+    26         146 LOAD_CONST              10 (2)
+               148 LOAD_CONST              12 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR'))
+               150 IMPORT_NAME             26 (utils)
+               152 IMPORT_FROM             27 (wrap_adapter)
+               154 STORE_NAME              27 (wrap_adapter)
+               156 IMPORT_FROM             28 (_can_edit)
+               158 STORE_NAME              28 (_can_edit)
+               160 IMPORT_FROM             29 (FEDIT_PREVIEW_VAR)
+               162 STORE_NAME              29 (FEDIT_PREVIEW_VAR)
+               164 POP_TOP
+   
+    31         166 LOAD_CONST              10 (2)
+               168 LOAD_CONST              13 (('REGISTER_CSS', 'REGISTER_JS'))
+               170 IMPORT_NAME             19 (hooks)
+               172 IMPORT_FROM             30 (REGISTER_CSS)
+               174 STORE_NAME              30 (REGISTER_CSS)
+               176 IMPORT_FROM             31 (REGISTER_JS)
+               178 STORE_NAME              31 (REGISTER_JS)
+               180 POP_TOP
+   
+    37         182 PUSH_NULL
+               184 LOAD_NAME                3 (library)
+               186 LOAD_ATTR               32 (Library)
+               196 PRECALL                  0
+               200 CALL                     0
+               210 STORE_NAME              33 (register)
+   
+    40         212 LOAD_CONST              14 ('Field name is not available in the context for %(object)s.')
+               214 STORE_NAME              34 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    41         216 LOAD_CONST              15 ('Model instance is not available in the context for %(object)s.')
+               218 STORE_NAME              35 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    45         220 PUSH_NULL
+               222 LOAD_BUILD_CLASS
+               224 LOAD_CONST              16 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 45>)
+               226 MAKE_FUNCTION            0
+               228 LOAD_CONST              17 ('AdapterNode')
+               230 LOAD_NAME                4 (Node)
+               232 PRECALL                  3
+               236 CALL                     3
+               246 STORE_NAME              36 (AdapterNode)
+   
+   122         248 LOAD_NAME               33 (register)
+               250 LOAD_METHOD             37 (tag)
+               272 LOAD_CONST              18 ('fedit')
+               274 KW_NAMES                19
+               276 PRECALL                  1
+               280 CALL                     1
+   
+   123         290 LOAD_CONST              20 ('parser')
+               292 LOAD_NAME                9 (Parser)
+               294 LOAD_CONST              21 ('token')
+               296 LOAD_NAME               10 (Token)
+               298 BUILD_TUPLE              4
+               300 LOAD_CONST              22 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 122>)
+               302 MAKE_FUNCTION            4 (annotations)
+   
+   122         304 PRECALL                  0
+               308 CALL                     0
+   
+   123         318 STORE_NAME              38 (do_render_fedit)
+   
+   162         320 LOAD_NAME               33 (register)
+               322 LOAD_METHOD             39 (simple_tag)
+               344 LOAD_CONST              23 (True)
+               346 KW_NAMES                24
+               348 PRECALL                  1
+               352 CALL                     1
+   
+   163         362 LOAD_CONST              25 ('context')
+               364 LOAD_NAME                7 (Context)
+               366 LOAD_CONST              26 ('adapter')
+               368 LOAD_NAME               24 (BaseAdapter)
+               370 LOAD_CONST              27 ('return')
+               372 LOAD_NAME               40 (str)
+               374 BUILD_TUPLE              6
+               376 LOAD_CONST              28 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 162>)
+               378 MAKE_FUNCTION            4 (annotations)
+   
+   162         380 PRECALL                  0
+               384 CALL                     0
+   
+   163         394 STORE_NAME              41 (render_adapter)
+   
+   179         396 LOAD_NAME               33 (register)
+               398 LOAD_METHOD             42 (inclusion_tag)
+               420 LOAD_CONST              29 ('wagtail_fedit/_hook_output.html')
+               422 LOAD_CONST              30 ('fedit_scripts')
+               424 LOAD_CONST              23 (True)
+               426 KW_NAMES                31
+               428 PRECALL                  3
+               432 CALL                     3
+   
+   180         442 LOAD_CONST              27 ('return')
+               444 LOAD_NAME               43 (dict)
+               446 BUILD_TUPLE              2
+               448 LOAD_CONST              32 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 179>)
+               450 MAKE_FUNCTION            4 (annotations)
+   
+   179         452 PRECALL                  0
+               456 CALL                     0
+   
+   180         466 STORE_NAME              44 (static_hook_output)
+   
+   210         468 LOAD_CONST              36 ((None,))
+               470 LOAD_CONST              20 ('parser')
+               472 LOAD_NAME                9 (Parser)
+               474 LOAD_CONST              33 ('tokens')
+               476 LOAD_NAME               45 (list)
+               478 LOAD_NAME               40 (str)
+               480 BINARY_SUBSCR
+               490 LOAD_CONST              34 ('kwarg_list')
+               492 LOAD_NAME               45 (list)
+               494 LOAD_NAME               40 (str)
+               496 BINARY_SUBSCR
+               506 LOAD_CONST              27 ('return')
+               508 LOAD_NAME               43 (dict)
+               510 BUILD_TUPLE              8
+               512 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 210>)
+               514 MAKE_FUNCTION            5 (defaults, annotations)
+               516 STORE_NAME              46 (get_kwargs)
+               518 LOAD_CONST               9 (None)
+               520 RETURN_VALUE
    consts
       0
       ('Type',)
       ('library', 'Node', 'TemplateSyntaxError')
-      ('render_to_string',)
-      ('make_context', 'Context')
+      ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
       ('reverse',)
       ('signing',)
       ('hooks',)
       None
       2
-      ('FeditAdapterEditButton',)
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
-      ('_can_edit',)
-      ('CONSTRUCT_ADAPTER_TOOLBAR',)
+      ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR')
+      ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564016506650719000000000000000000640265
             0864036509650a190000000000000000006606640484045a0b640584005a
             0c640684005a0d64075300
-          47           0 RESUME                   0
+          45           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          48          10 PUSH_NULL
+          46          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          50          40 LOAD_CONST               1 ('adapter')
+          48          40 LOAD_CONST               1 ('adapter')
                       42 LOAD_NAME                6 (Type)
                       44 LOAD_NAME                7 (BaseAdapter)
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('model')
                       58 LOAD_NAME                8 (FilterExpression)
                       60 LOAD_CONST               3 ('getters')
                       62 LOAD_NAME                9 (list)
                       64 LOAD_NAME               10 (str)
                       66 BINARY_SUBSCR
                       76 BUILD_TUPLE              6
-                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 50>)
+                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 48>)
                       80 MAKE_FUNCTION            4 (annotations)
                       82 STORE_NAME              11 (__init__)
          
-          56          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 56>)
+          54          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 54>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              12 (_resolve_expressions)
          
-          66          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 66>)
+          64          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 64>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              13 (render)
                       96 LOAD_CONST               7 (None)
                       98 RETURN_VALUE
          consts
             'AdapterNode'
             'adapter'
@@ -314,42 +307,42 @@
                nlocals   : 5
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f03000000000000000064
                   005300
-                50           0 RESUME                   0
+                48           0 RESUME                   0
                
-                51           2 LOAD_FAST                1 (adapter)
+                49           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                52          16 LOAD_FAST                2 (model)
+                50          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                53          30 LOAD_FAST                3 (getters)
+                51          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                54          44 LOAD_FAST                4 (kwargs)
+                52          44 LOAD_FAST                4 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                             58 LOAD_CONST               0 (None)
                             60 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs')
                varnames   ('self', 'adapter', 'model', 'getters', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 50
+               firstlineno 48
                lnotab 0x02010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -357,70 +350,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                56           0 RESUME                   0
+                54           0 RESUME                   0
                
-                57           2 LOAD_FAST                3 (kwargs)
+                55           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                58          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                56          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                59          94 LOAD_FAST                5 (v)
+                57          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                61     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                59     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                62         186 LOAD_FAST                2 (model)
+                60         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                64     >>  228 LOAD_FAST                2 (model)
+                62     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 56
+               firstlineno 54
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 8
                flags     : 3
                code
@@ -450,254 +443,254 @@
                   00ab0100000000000000007d0a02007c006a07000000000000000064097c
                   067c057c0a64089c037c04a4018e017d0b7c0ba015000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007210742d00
                   0000000000000000007c0a7c06a6020000ab02000000000000000073157c
                   0ba01700000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000053007431000000000000000000007c0a7c0b7c01a6
                   030000ab0300000000000000005300
-                66           0 RESUME                   0
+                64           0 RESUME                   0
                
-                67           2 LOAD_FAST                0 (self)
+                65           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                68          16 LOAD_FAST                0 (self)
+                66          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                70          30 PUSH_NULL
+                68          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                71          44 LOAD_FAST                1 (context)
+                69          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                70          48 BUILD_TUPLE              2
+                68          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                71          52 LOAD_FAST                0 (self)
+                69          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                70          64 DICT_MERGE               1
+                68          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                74          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                72          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
                
-                75          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                73          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
                
-                76          92 LOAD_FAST                2 (model)
+                74          92 LOAD_FAST                2 (model)
                
-                75          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
+                73          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
                
-                78          96 LOAD_FAST                1 (context)
+                76          96 LOAD_FAST                1 (context)
                             98 LOAD_CONST               1 ('wagtail_fedit_field')
                            100 BINARY_SUBSCR
                            110 STORE_FAST               5 (field_name)
                
-                79         112 LOAD_FAST                1 (context)
+                77         112 LOAD_FAST                1 (context)
                            114 LOAD_CONST               2 ('wagtail_fedit_instance')
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (obj)
                            128 EXTENDED_ARG             1
                            130 JUMP_FORWARD           264 (to 660)
                
-                83     >>  132 LOAD_FAST                2 (model)
+                81     >>  132 LOAD_FAST                2 (model)
                            134 POP_JUMP_FORWARD_IF_TRUE   132 (to 400)
                
-                84         136 LOAD_GLOBAL              9 (NULL + warnings)
+                82         136 LOAD_GLOBAL              9 (NULL + warnings)
                            148 LOAD_ATTR                5 (warn)
                
-                85         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                83         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                86         170 LOAD_CONST               3 ('object')
+                84         170 LOAD_CONST               3 ('object')
                            172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                7 (adapter)
                            184 LOAD_ATTR                8 (__name__)
                
-                85         194 BUILD_MAP                1
+                83         194 BUILD_MAP                1
                            196 BINARY_OP                6 (%)
                
-                88         200 LOAD_GLOBAL             18 (RuntimeWarning)
+                86         200 LOAD_GLOBAL             18 (RuntimeWarning)
                
-                84         212 PRECALL                  2
+                82         212 PRECALL                  2
                            216 CALL                     2
                            226 POP_TOP
                
-                91         228 LOAD_FAST                1 (context)
+                89         228 LOAD_FAST                1 (context)
                            230 LOAD_METHOD             10 (flatten)
                            252 PRECALL                  0
                            256 CALL                     0
                            266 STORE_FAST               1 (context)
                
-                93         268 NOP
+                91         268 NOP
                
-                94         270 PUSH_NULL
+                92         270 PUSH_NULL
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                7 (adapter)
                            284 LOAD_ATTR               11 (render_from_kwargs)
                
-                95         294 LOAD_FAST                1 (context)
+                93         294 LOAD_FAST                1 (context)
                
-                94         296 BUILD_TUPLE              1
+                92         296 BUILD_TUPLE              1
                            298 BUILD_MAP                0
                
-                95         300 LOAD_FAST                4 (kwargs)
+                93         300 LOAD_FAST                4 (kwargs)
                
-                94         302 DICT_MERGE               1
+                92         302 DICT_MERGE               1
                            304 CALL_FUNCTION_EX         1
                            306 RETURN_VALUE
                        >>  308 PUSH_EXC_INFO
                
-                97         310 LOAD_GLOBAL             24 (AdapterError)
+                95         310 LOAD_GLOBAL             24 (AdapterError)
                            322 CHECK_EXC_MATCH
                            324 POP_JUMP_FORWARD_IF_FALSE    33 (to 392)
                            326 STORE_FAST               7 (e)
                
-                98         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
+                96         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
                            340 LOAD_GLOBAL             29 (NULL + str)
                            352 LOAD_FAST                7 (e)
                            354 PRECALL                  1
                            358 CALL                     1
                            368 PRECALL                  1
                            372 CALL                     1
                            382 RAISE_VARARGS            1
                        >>  384 LOAD_CONST               0 (None)
                            386 STORE_FAST               7 (e)
                            388 DELETE_FAST              7 (e)
                            390 RERAISE                  1
                
-                97     >>  392 RERAISE                  0
+                95     >>  392 RERAISE                  0
                        >>  394 COPY                     3
                            396 POP_EXCEPT
                            398 RERAISE                  1
                
-               100     >>  400 LOAD_FAST                3 (getters)
+                98     >>  400 LOAD_FAST                3 (getters)
                            402 LOAD_GLOBAL             31 (NULL + len)
                            414 LOAD_FAST                3 (getters)
                            416 PRECALL                  1
                            420 CALL                     1
                            430 LOAD_CONST               4 (1)
                            432 BINARY_OP               10 (-)
                            436 BINARY_SUBSCR
                            446 STORE_FAST               5 (field_name)
                
-               101         448 LOAD_FAST                2 (model)
+                99         448 LOAD_FAST                2 (model)
                            450 STORE_FAST               6 (obj)
                
-               102         452 LOAD_GLOBAL             33 (NULL + range)
+               100         452 LOAD_GLOBAL             33 (NULL + range)
                            464 LOAD_GLOBAL             31 (NULL + len)
                            476 LOAD_FAST                3 (getters)
                            478 PRECALL                  1
                            482 CALL                     1
                            492 LOAD_CONST               4 (1)
                            494 BINARY_OP               10 (-)
                            498 PRECALL                  1
                            502 CALL                     1
                            512 GET_ITER
                        >>  514 FOR_ITER                72 (to 660)
                            516 STORE_FAST               8 (i)
                
-               103         518 LOAD_FAST                3 (getters)
+               101         518 LOAD_FAST                3 (getters)
                            520 LOAD_FAST                8 (i)
                            522 BINARY_SUBSCR
                            532 STORE_FAST               9 (getter)
                
-               104         534 NOP
+               102         534 NOP
                
-               105         536 LOAD_GLOBAL             35 (NULL + getattr)
+               103         536 LOAD_GLOBAL             35 (NULL + getattr)
                            548 LOAD_FAST                6 (obj)
                            550 LOAD_FAST                9 (getter)
                            552 PRECALL                  2
                            556 CALL                     2
                            566 STORE_FAST               6 (obj)
                            568 JUMP_BACKWARD           28 (to 514)
                        >>  570 PUSH_EXC_INFO
                
-               106         572 LOAD_GLOBAL             36 (AttributeError)
+               104         572 LOAD_GLOBAL             36 (AttributeError)
                            584 CHECK_EXC_MATCH
                            586 POP_JUMP_FORWARD_IF_FALSE    32 (to 652)
                            588 POP_TOP
                
-               107         590 LOAD_GLOBAL             37 (NULL + AttributeError)
+               105         590 LOAD_GLOBAL             37 (NULL + AttributeError)
                            602 LOAD_CONST               5 ('Object ')
                            604 LOAD_FAST                2 (model)
                            606 LOAD_ATTR               19 (__class__)
                            616 LOAD_ATTR                8 (__name__)
                            626 FORMAT_VALUE             0
                            628 LOAD_CONST               6 (' does not have attribute ')
                            630 LOAD_FAST                9 (getter)
                            632 FORMAT_VALUE             0
                            634 BUILD_STRING             4
                            636 PRECALL                  1
                            640 CALL                     1
                            650 RAISE_VARARGS            1
                
-               106     >>  652 RERAISE                  0
+               104     >>  652 RERAISE                  0
                        >>  654 COPY                     3
                            656 POP_EXCEPT
                            658 RERAISE                  1
                
-               109     >>  660 LOAD_FAST                1 (context)
+               107     >>  660 LOAD_FAST                1 (context)
                            662 LOAD_METHOD             20 (get)
                            684 LOAD_CONST               7 ('request')
                            686 PRECALL                  1
                            690 CALL                     1
                            700 STORE_FAST              10 (request)
                
-               110         702 PUSH_NULL
+               108         702 PUSH_NULL
                            704 LOAD_FAST                0 (self)
                            706 LOAD_ATTR                7 (adapter)
                            716 LOAD_CONST               9 (())
                
-               111         718 LOAD_FAST                6 (obj)
+               109         718 LOAD_FAST                6 (obj)
                
-               112         720 LOAD_FAST                5 (field_name)
+               110         720 LOAD_FAST                5 (field_name)
                
-               113         722 LOAD_FAST               10 (request)
+               111         722 LOAD_FAST               10 (request)
                
-               110         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
+               108         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
                            726 BUILD_CONST_KEY_MAP      3
                
-               114         728 LOAD_FAST                4 (kwargs)
+               112         728 LOAD_FAST                4 (kwargs)
                
-               110         730 DICT_MERGE               1
+               108         730 DICT_MERGE               1
                            732 CALL_FUNCTION_EX         1
                            734 STORE_FAST              11 (adapter)
                
-               117         736 LOAD_FAST               11 (adapter)
+               115         736 LOAD_FAST               11 (adapter)
                            738 LOAD_METHOD             21 (check_permissions)
                            760 PRECALL                  0
                            764 CALL                     0
                            774 POP_JUMP_FORWARD_IF_FALSE    16 (to 808)
                
-               118         776 LOAD_GLOBAL             45 (NULL + _can_edit)
+               116         776 LOAD_GLOBAL             45 (NULL + _can_edit)
                            788 LOAD_FAST               10 (request)
                            790 LOAD_FAST                6 (obj)
                            792 PRECALL                  2
                            796 CALL                     2
                
-               117         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
+               115         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
                
-               119     >>  808 LOAD_FAST               11 (adapter)
+               117     >>  808 LOAD_FAST               11 (adapter)
                            810 LOAD_METHOD             23 (render_content)
                            832 LOAD_FAST                1 (context)
                            834 PRECALL                  1
                            838 CALL                     1
                            848 RETURN_VALUE
                
-               121     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
+               119     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
                            862 LOAD_FAST               10 (request)
                            864 LOAD_FAST               11 (adapter)
                            866 LOAD_FAST                1 (context)
                            868 PRECALL                  3
                            872 CALL                     3
                            882 RETURN_VALUE
                ExceptionTable:
@@ -720,28 +713,28 @@
                   ()
                names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 66
+               firstlineno 64
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
                   0116010c0118ff06030cfc100728020201180102ff040102ff0803120140
                   ff080330010401420110010201240112013eff08032a0110010201020102
                   fd040402fc060728011eff02022a02
             None
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 47
+         firstlineno 45
          lnotab 0x0a011e022c06060a
       'AdapterNode'
       'fedit'
       ('name',)
       'parser'
       'token'
       code
@@ -767,153 +760,153 @@
             00000000007c07a6010000ab01000000000000000064096b040000000072
             287c00a00700000000000000000000000000000000000000007c07a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             0000000000a6010000ab0100000000000000007d06741100000000000000
             0000007c007c027c056a090000000000000000a6030000ab030000000000
             0000007d09741500000000000000000000640b7c057c067c07640a9c037c
             09a4018e015300
-         124           0 RESUME                   0
+         122           0 RESUME                   0
          
-         127           2 LOAD_FAST                1 (token)
+         125           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         129          42 LOAD_FAST                2 (tokens)
+         127          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         130          84 LOAD_FAST                2 (tokens)
+         128          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         132         126 NOP
+         130         126 NOP
          
-         133         128 LOAD_GLOBAL              4 (adapter_registry)
+         131         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         134         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         132         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         135         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         133         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         134     >>  214 RERAISE                  0
+         132     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         137     >>  222 LOAD_CONST               4 ((None, None))
+         135     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         138         232 LOAD_FAST                2 (tokens)
+         136         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
          
-         139         236 LOAD_FAST                2 (tokens)
+         137         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         140         278 LOAD_FAST                8 (model__field)
+         138         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         142         320 LOAD_GLOBAL             13 (NULL + len)
+         140         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
          
-         143         358 LOAD_FAST                7 (model_tokens)
+         141         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
          
-         144         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         142         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         145         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         143         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         144         396 PRECALL                  1
+         142         396 PRECALL                  1
                      400 CALL                     1
                      410 RAISE_VARARGS            1
          
-         148     >>  412 LOAD_GLOBAL             13 (NULL + len)
+         146     >>  412 LOAD_GLOBAL             13 (NULL + len)
                      424 LOAD_FAST                7 (model_tokens)
                      426 PRECALL                  1
                      430 CALL                     1
                      440 LOAD_CONST               9 (1)
                      442 COMPARE_OP               4 (>)
                      448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
          
-         151         450 LOAD_FAST                0 (parser)
+         149         450 LOAD_FAST                0 (parser)
                      452 LOAD_METHOD              7 (compile_filter)
                      474 LOAD_FAST                7 (model_tokens)
                      476 LOAD_METHOD              1 (pop)
                      498 LOAD_CONST               1 (0)
                      500 PRECALL                  1
                      504 CALL                     1
                      514 PRECALL                  1
                      518 CALL                     1
                      528 STORE_FAST               6 (model)
          
-         153     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
+         151     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
                      542 LOAD_FAST                0 (parser)
                      544 LOAD_FAST                2 (tokens)
                      546 LOAD_FAST                5 (adapter)
                      548 LOAD_ATTR                9 (required_kwargs)
                      558 PRECALL                  3
                      562 CALL                     3
                      572 STORE_FAST               9 (kwargs)
          
-         155         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
+         153         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
                      586 LOAD_CONST              11 (())
          
-         156         588 LOAD_FAST                5 (adapter)
+         154         588 LOAD_FAST                5 (adapter)
          
-         157         590 LOAD_FAST                6 (model)
+         155         590 LOAD_FAST                6 (model)
          
-         158         592 LOAD_FAST                7 (model_tokens)
+         156         592 LOAD_FAST                7 (model_tokens)
          
-         155         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
+         153         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
                      596 BUILD_CONST_KEY_MAP      3
          
-         159         598 LOAD_FAST                9 (kwargs)
+         157         598 LOAD_FAST                9 (kwargs)
          
-         155         600 DICT_MERGE               1
+         153         600 DICT_MERGE               1
                      602 CALL_FUNCTION_EX         1
                      604 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -930,295 +923,81 @@
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 124
+         firstlineno 122
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
             010c0102ff1004260350022c020e010201020102fd040402fc
-      False
-      'request'
-      'adapter'
-      'context'
-      'run_context_processors'
-      'return'
-      code
-         argcount  : 4
-         nlocals   : 9
-         stacksize : 14
-         flags     : 3
-         code
-            0x870097007c02730269007d02740100000000000000000000a6000000ab
-            00000000000000000067017d047403000000000000000000006a02000000
-            0000000000740600000000000000000000a6010000ab0100000000000000
-            0044005d0f7d0502007c057c047c01ac01a6020000ab0200000000000000
-            0001008c1088006601640284087c044400a6000000ab0000000000000000
-            007d04740900000000000000000000740b0000000000000000000064007c
-            04a6020000ab020000000000000000a6010000ab0100000000000000007d
-            047c016a0600000000000000007c016a0700000000000000007c016a0800
-            000000000000006a0900000000000000006a0a00000000000000007c016a
-            0800000000000000006a0900000000000000006a0b00000000000000007c
-            016a0800000000000000006a0c000000000000000064039c057d067c01a0
-            0d0000000000000000000000000000000000000000a6000000ab00000000
-            00000000007d077c01a00e00000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d08741f0000000000000000000064
-            047c016a0600000000000000007c017c047c077c087c016a100000000000
-            0000007c0274230000000000000000000064057c06ac06a6020000ab0200
-            0000000000000064079c087c03720289006e016400ac08a6030000ab0300
-            000000000000005300
-                       0 MAKE_CELL                0 (request)
-         
-         163           2 RESUME                   0
-         
-         164           4 LOAD_FAST                2 (context)
-                       6 POP_JUMP_FORWARD_IF_TRUE     2 (to 12)
-         
-         165           8 BUILD_MAP                0
-                      10 STORE_FAST               2 (context)
-         
-         168     >>   12 LOAD_GLOBAL              1 (NULL + FeditAdapterEditButton)
-                      24 PRECALL                  0
-                      28 CALL                     0
-         
-         167          38 BUILD_LIST               1
-                      40 STORE_FAST               4 (items)
-         
-         171          42 LOAD_GLOBAL              3 (NULL + hooks)
-                      54 LOAD_ATTR                2 (get_hooks)
-                      64 LOAD_GLOBAL              6 (CONSTRUCT_ADAPTER_TOOLBAR)
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 GET_ITER
-                 >>   92 FOR_ITER                15 (to 124)
-                      94 STORE_FAST               5 (hook)
-         
-         172          96 PUSH_NULL
-                      98 LOAD_FAST                5 (hook)
-                     100 LOAD_FAST                4 (items)
-                     102 LOAD_FAST                1 (adapter)
-                     104 KW_NAMES                 1
-                     106 PRECALL                  2
-                     110 CALL                     2
-                     120 POP_TOP
-                     122 JUMP_BACKWARD           16 (to 92)
-         
-         174     >>  124 LOAD_CLOSURE             0 (request)
-                     126 BUILD_TUPLE              1
-                     128 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 174>)
-                     130 MAKE_FUNCTION            8 (closure)
-                     132 LOAD_FAST                4 (items)
-                     134 GET_ITER
-                     136 PRECALL                  0
-                     140 CALL                     0
-                     150 STORE_FAST               4 (items)
-         
-         175         152 LOAD_GLOBAL              9 (NULL + list)
-                     164 LOAD_GLOBAL             11 (NULL + filter)
-                     176 LOAD_CONST               0 (None)
-                     178 LOAD_FAST                4 (items)
-                     180 PRECALL                  2
-                     184 CALL                     2
-                     194 PRECALL                  1
-                     198 CALL                     1
-                     208 STORE_FAST               4 (items)
-         
-         178         210 LOAD_FAST                1 (adapter)
-                     212 LOAD_ATTR                6 (identifier)
-         
-         179         222 LOAD_FAST                1 (adapter)
-                     224 LOAD_ATTR                7 (field_name)
-         
-         180         234 LOAD_FAST                1 (adapter)
-                     236 LOAD_ATTR                8 (object)
-                     246 LOAD_ATTR                9 (_meta)
-                     256 LOAD_ATTR               10 (app_label)
-         
-         181         266 LOAD_FAST                1 (adapter)
-                     268 LOAD_ATTR                8 (object)
-                     278 LOAD_ATTR                9 (_meta)
-                     288 LOAD_ATTR               11 (model_name)
-         
-         182         298 LOAD_FAST                1 (adapter)
-                     300 LOAD_ATTR                8 (object)
-                     310 LOAD_ATTR               12 (pk)
-         
-         177         320 LOAD_CONST               3 (('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id'))
-                     322 BUILD_CONST_KEY_MAP      5
-                     324 STORE_FAST               6 (reverse_kwargs)
-         
-         185         326 LOAD_FAST                1 (adapter)
-                     328 LOAD_METHOD             13 (encode_shared_context)
-                     350 PRECALL                  0
-                     354 CALL                     0
-                     364 STORE_FAST               7 (shared)
-         
-         186         366 LOAD_FAST                1 (adapter)
-                     368 LOAD_METHOD             14 (get_js_constructor)
-                     390 PRECALL                  0
-                     394 CALL                     0
-                     404 STORE_FAST               8 (js_constructor)
-         
-         188         406 LOAD_GLOBAL             31 (NULL + render_to_string)
-         
-         189         418 LOAD_CONST               4 ('wagtail_fedit/content/editable_adapter.html')
-         
-         191         420 LOAD_FAST                1 (adapter)
-                     422 LOAD_ATTR                6 (identifier)
-         
-         192         432 LOAD_FAST                1 (adapter)
-         
-         193         434 LOAD_FAST                4 (items)
-         
-         194         436 LOAD_FAST                7 (shared)
-         
-         195         438 LOAD_FAST                8 (js_constructor)
-         
-         196         440 LOAD_FAST                1 (adapter)
-                     442 LOAD_ATTR               16 (kwargs)
-         
-         197         452 LOAD_FAST                2 (context)
-         
-         198         454 LOAD_GLOBAL             35 (NULL + reverse)
-         
-         199         466 LOAD_CONST               5 ('wagtail_fedit:edit')
-         
-         200         468 LOAD_FAST                6 (reverse_kwargs)
-         
-         198         470 KW_NAMES                 6
-                     472 PRECALL                  2
-                     476 CALL                     2
-         
-         190         486 LOAD_CONST               7 (('identifier', 'adapter', 'buttons', 'shared', 'js_constructor', 'shared_context', 'parent_context', 'edit_url'))
-                     488 BUILD_CONST_KEY_MAP      8
-         
-         203         490 LOAD_FAST                3 (run_context_processors)
-                     492 POP_JUMP_FORWARD_IF_FALSE     2 (to 498)
-                     494 LOAD_DEREF               0 (request)
-                     496 JUMP_FORWARD             1 (to 500)
-                 >>  498 LOAD_CONST               0 (None)
-         
-         188     >>  500 KW_NAMES                 8
-                     502 PRECALL                  3
-                     506 CALL                     3
-                     516 RETURN_VALUE
-         consts
-            None
-            ('items', 'adapter')
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 5
-               flags     : 19
-               code
-                  0x9501970067007c005d177d017c01a00000000000000000000000000000
-                  000000000000008902a6010000ab01000000000000000091028c185300
-                             0 COPY_FREE_VARS           1
-               
-               174           2 RESUME                   0
-                             4 BUILD_LIST               0
-                             6 LOAD_FAST                0 (.0)
-                       >>    8 FOR_ITER                23 (to 56)
-                            10 STORE_FAST               1 (item)
-                            12 LOAD_FAST                1 (item)
-                            14 LOAD_METHOD              0 (render)
-                            36 LOAD_DEREF               2 (request)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 LIST_APPEND              2
-                            54 JUMP_BACKWARD           24 (to 8)
-                       >>   56 RETURN_VALUE
-               consts
-               names      ('render',)
-               varnames   ('.0', 'item')
-               freevars   ('request',)
-               cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-               name       '<listcomp>'
-               firstlineno 174
-               lnotab 0x
-            ('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id')
-            'wagtail_fedit/content/editable_adapter.html'
-            'wagtail_fedit:edit'
-            ('kwargs',)
-            ('identifier', 'adapter', 'buttons', 'shared', 'js_constructor', 'shared_context', 'parent_context', 'edit_url')
-            ('request',)
-         names      ('FeditAdapterEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_ADAPTER_TOOLBAR', 'list', 'filter', 'identifier', 'field_name', 'object', '_meta', 'app_label', 'model_name', 'pk', 'encode_shared_context', 'get_js_constructor', 'render_to_string', 'kwargs', 'reverse')
-         varnames   ('request', 'adapter', 'context', 'run_context_processors', 'items', 'hook', 'reverse_kwargs', 'shared', 'js_constructor')
-         freevars   ()
-         cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
-         name       'wrap_adapter'
-         firstlineno 163
-         lnotab
-            0x0401040104031aff040436011c021c013a030c010c012001200116fb06
-            08280128020c0102020c0102010201020102010c0102010c01020102fe10
-            f8040d0af1
       True
       ('takes_context',)
+      'context'
+      'adapter'
+      'return'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c01a00400000000000000
             000000000000000000000000007c00a6010000ab01000000000000000053
             00
-         206           0 RESUME                   0
+         162           0 RESUME                   0
          
-         208           2 BUILD_MAP                0
+         164           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         210           6 LOAD_CONST               1 ('parent_context')
+         166           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         211          14 LOAD_FAST                0 (context)
+         167          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         212          30 LOAD_FAST                0 (context)
+         168          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         214     >>   36 LOAD_FAST                0 (context)
+         170     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         216          78 LOAD_FAST                1 (adapter)
+         172          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         217          98 LOAD_FAST                1 (adapter)
+         173          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         218         118 LOAD_FAST                1 (adapter)
+         174         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         220         138 LOAD_FAST                1 (adapter)
+         176         138 LOAD_FAST                1 (adapter)
                      140 LOAD_METHOD              4 (render_content)
                      162 LOAD_FAST                0 (context)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             None
@@ -1228,16 +1007,151 @@
             'request'
          names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 206
+         firstlineno 162
          lnotab 0x020204020801100106022a02140114011402
+      'wagtail_fedit/_hook_output.html'
+      'fedit_scripts'
+      ('name', 'takes_context')
+      code
+         argcount  : 2
+         nlocals   : 7
+         stacksize : 6
+         flags     : 3
+         code
+            0x97007c01a0000000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d017c0164017601720f740300000000000000
+            0000006402a6010000ab01000000000000000082017c00a0020000000000
+            0000000000000000000000000000006403a6010000ab0100000000000000
+            007d027c0164046b020000000072087406000000000000000000007d036e
+            077408000000000000000000007d03740b000000000000000000007c0274
+            0c000000000000000000006405a6030000ab030000000000000000730269
+            00530067007d04740f000000000000000000006a0800000000000000007c
+            03a6010000ab01000000000000000044005d417d0502007c057c02a60100
+            00ab0100000000000000007d067413000000000000000000007c06741400
+            0000000000000000007416000000000000000000006602a6020000ab0200
+            0000000000000073037c0667017d067c04a00c0000000000000000000000
+            0000000000000000007c06a6010000ab01000000000000000001008c4264
+            067c0469015300
+         179           0 RESUME                   0
+         
+         181           2 LOAD_FAST                1 (css_or_js)
+                       4 LOAD_METHOD              0 (lower)
+                      26 PRECALL                  0
+                      30 CALL                     0
+                      40 STORE_FAST               1 (css_or_js)
+         
+         183          42 LOAD_FAST                1 (css_or_js)
+                      44 LOAD_CONST               1 (('css', 'js'))
+                      46 CONTAINS_OP              1
+                      48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
+         
+         184          50 LOAD_GLOBAL              3 (NULL + ValueError)
+                      62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
+                      64 PRECALL                  1
+                      68 CALL                     1
+                      78 RAISE_VARARGS            1
+         
+         186     >>   80 LOAD_FAST                0 (context)
+                      82 LOAD_METHOD              2 (get)
+                     104 LOAD_CONST               3 ('request')
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 STORE_FAST               2 (request)
+         
+         188         122 LOAD_FAST                1 (css_or_js)
+                     124 LOAD_CONST               4 ('css')
+                     126 COMPARE_OP               2 (==)
+                     132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
+         
+         189         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+                     146 STORE_FAST               3 (hook_name)
+                     148 JUMP_FORWARD             7 (to 164)
+         
+         191     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+                     162 STORE_FAST               3 (hook_name)
+         
+         193     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+                     176 LOAD_FAST                2 (request)
+                     178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
+                     190 LOAD_CONST               5 (False)
+                     192 PRECALL                  3
+                     196 CALL                     3
+                     206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
+         
+         194         208 BUILD_MAP                0
+                     210 RETURN_VALUE
+         
+         196     >>  212 BUILD_LIST               0
+                     214 STORE_FAST               4 (files)
+         
+         197         216 LOAD_GLOBAL             15 (NULL + hooks)
+                     228 LOAD_ATTR                8 (get_hooks)
+                     238 LOAD_FAST                3 (hook_name)
+                     240 PRECALL                  1
+                     244 CALL                     1
+                     254 GET_ITER
+                 >>  256 FOR_ITER                65 (to 388)
+                     258 STORE_FAST               5 (hook)
+         
+         198         260 PUSH_NULL
+                     262 LOAD_FAST                5 (hook)
+                     264 LOAD_FAST                2 (request)
+                     266 PRECALL                  1
+                     270 CALL                     1
+                     280 STORE_FAST               6 (ret)
+         
+         200         282 LOAD_GLOBAL             19 (NULL + isinstance)
+                     294 LOAD_FAST                6 (ret)
+                     296 LOAD_GLOBAL             20 (list)
+                     308 LOAD_GLOBAL             22 (tuple)
+                     320 BUILD_TUPLE              2
+                     322 PRECALL                  2
+                     326 CALL                     2
+                     336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
+         
+         201         338 LOAD_FAST                6 (ret)
+                     340 BUILD_LIST               1
+                     342 STORE_FAST               6 (ret)
+         
+         203     >>  344 LOAD_FAST                4 (files)
+                     346 LOAD_METHOD             12 (extend)
+                     368 LOAD_FAST                6 (ret)
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 POP_TOP
+                     386 JUMP_BACKWARD           66 (to 256)
+         
+         206     >>  388 LOAD_CONST               6 ('hook_output')
+                     390 LOAD_FAST                4 (files)
+         
+         205         392 BUILD_MAP                1
+                     394 RETURN_VALUE
+         consts
+            None
+            ('css', 'js')
+            "Invalid argument, must be 'css' or 'js'"
+            'request'
+            'css'
+            False
+            'hook_output'
+         names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
+         varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'static_hook_output'
+         firstlineno 179
+         lnotab
+            0x0202280208011e022a020c0110020e022c01040204012c011602380106
+            022c0304ff
       'tokens'
       'kwarg_list'
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 5
          flags     : 3
@@ -1252,123 +1166,123 @@
             017c00a00400000000000000000000000000000000000000007c06a60100
             00ab0100000000000000007c047c027c05190000000000000000003c0000
             008c707c076405190000000000000000007d087c00a00400000000000000
             000000000000000000000000007c07640319000000000000000000a60100
             00ab0100000000000000007c047c083c00000064067d038c997c0244005d
             187d097c097c0476017212740b0000000000000000000064077c099b009d
             02a6010000ab01000000000000000082018c197c045300
-         223           0 RESUME                   0
+         210           0 RESUME                   0
          
-         224           2 LOAD_CONST               1 (False)
+         211           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         225           6 BUILD_MAP                0
+         212           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         227          10 LOAD_FAST                2 (kwarg_list)
+         214          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         228          14 BUILD_LIST               0
+         215          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         230     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
+         217     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
                       30 LOAD_FAST                1 (tokens)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 GET_ITER
                  >>   48 FOR_ITER               152 (to 354)
                       50 UNPACK_SEQUENCE          2
                       54 STORE_FAST               5 (i)
                       56 STORE_FAST               6 (token)
          
-         231          58 LOAD_FAST                6 (token)
+         218          58 LOAD_FAST                6 (token)
                       60 LOAD_METHOD              1 (split)
                       82 LOAD_CONST               2 ('=')
                       84 PRECALL                  1
                       88 CALL                     1
                       98 STORE_FAST               7 (split)
          
-         232         100 LOAD_GLOBAL              5 (NULL + len)
+         219         100 LOAD_GLOBAL              5 (NULL + len)
                      112 LOAD_FAST                7 (split)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 LOAD_CONST               3 (1)
                      130 COMPARE_OP               2 (==)
                      136 POP_JUMP_FORWARD_IF_FALSE    67 (to 272)
                      138 LOAD_GLOBAL              5 (NULL + len)
                      150 LOAD_FAST                2 (kwarg_list)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_FAST                5 (i)
                      168 COMPARE_OP               4 (>)
                      174 POP_JUMP_FORWARD_IF_FALSE    48 (to 272)
          
-         233         176 LOAD_FAST                3 (had_kwargs)
+         220         176 LOAD_FAST                3 (had_kwargs)
                      178 POP_JUMP_FORWARD_IF_FALSE    15 (to 210)
          
-         234         180 LOAD_GLOBAL              7 (NULL + ValueError)
+         221         180 LOAD_GLOBAL              7 (NULL + ValueError)
                      192 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RAISE_VARARGS            1
          
-         236     >>  210 LOAD_FAST                0 (parser)
+         223     >>  210 LOAD_FAST                0 (parser)
                      212 LOAD_METHOD              4 (compile_filter)
                      234 LOAD_FAST                6 (token)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_FAST                4 (kwargs)
                      252 LOAD_FAST                2 (kwarg_list)
                      254 LOAD_FAST                5 (i)
                      256 BINARY_SUBSCR
                      266 STORE_SUBSCR
                      270 JUMP_BACKWARD          112 (to 48)
          
-         238     >>  272 LOAD_FAST                7 (split)
+         225     >>  272 LOAD_FAST                7 (split)
                      274 LOAD_CONST               5 (0)
                      276 BINARY_SUBSCR
                      286 STORE_FAST               8 (key)
          
-         242         288 LOAD_FAST                0 (parser)
+         229         288 LOAD_FAST                0 (parser)
                      290 LOAD_METHOD              4 (compile_filter)
                      312 LOAD_FAST                7 (split)
                      314 LOAD_CONST               3 (1)
                      316 BINARY_SUBSCR
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                4 (kwargs)
                      342 LOAD_FAST                8 (key)
                      344 STORE_SUBSCR
          
-         243         348 LOAD_CONST               6 (True)
+         230         348 LOAD_CONST               6 (True)
                      350 STORE_FAST               3 (had_kwargs)
                      352 JUMP_BACKWARD          153 (to 48)
          
-         245     >>  354 LOAD_FAST                2 (kwarg_list)
+         232     >>  354 LOAD_FAST                2 (kwarg_list)
                      356 GET_ITER
                  >>  358 FOR_ITER                24 (to 408)
                      360 STORE_FAST               9 (kwarg)
          
-         246         362 LOAD_FAST                9 (kwarg)
+         233         362 LOAD_FAST                9 (kwarg)
                      364 LOAD_FAST                4 (kwargs)
                      366 CONTAINS_OP              1
                      368 POP_JUMP_FORWARD_IF_FALSE    18 (to 406)
          
-         247         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+         234         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
                      382 LOAD_CONST               7 ('Missing required keyword argument ')
                      384 LOAD_FAST                9 (kwarg)
                      386 FORMAT_VALUE             0
                      388 BUILD_STRING             2
                      390 PRECALL                  1
                      394 CALL                     1
                      404 RAISE_VARARGS            1
          
-         246     >>  406 JUMP_BACKWARD           25 (to 358)
+         233     >>  406 JUMP_BACKWARD           25 (to 358)
          
-         249     >>  408 LOAD_FAST                4 (kwargs)
+         236     >>  408 LOAD_FAST                4 (kwargs)
                      410 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -1377,23 +1291,23 @@
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'kwarg')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 223
+         firstlineno 210
          lnotab
             0x0201040104020401040228012a014c0104011e023e0210043c01060208
             01080124ff0203
-      (False,)
       (None,)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.loader', 'render_to_string', 'django.template.context', 'make_context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'toolbar', 'FeditAdapterEditButton', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', '_can_edit', 'CONSTRUCT_ADAPTER_TOOLBAR', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'dict', 'bool', 'str', 'wrap_adapter', 'simple_tag', 'render_adapter', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'str', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0114030c01100414040c010c010c020c0208020c0318060c
-      030c051e03040104041c4d2a010eff0e0102261e2b2a0112ff0e010210
+      0x00ff02010c0114030c0314040c010c010c020c0208021806140510061e
+      03040104041c4d2a010eff0e0102272a0112ff0e0102102e010aff0e0102
+      1e
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/views/adapters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,250 +1,199 @@
-from typing import Type
-from django.template import (
-    library, Node, TemplateSyntaxError,
-)
+from typing import Any
+from django.shortcuts import render
+from django.utils.translation import gettext as _
+from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
-from django.template.context import (
-    make_context,
-    Context,
-)
-from django.template.base import (
-    Parser, Token,
-    FilterExpression,
+from django.views.decorators.clickjacking import xframe_options_sameorigin
+from django.views.generic import View
+from django.http import (
+    HttpRequest,
+    HttpResponseBadRequest,
+    HttpResponseForbidden,
+    JsonResponse,
+    HttpResponse,
+)
+from django.apps import apps
+from wagtail.models import (
+    RevisionMixin,
+    PAGE_TEMPLATE_VAR,
+    Page,
 )
-from django.http import HttpRequest
-from django.urls import reverse
-from django.core import signing
-
-from wagtail import hooks
-
-import warnings
+from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 
-from ..toolbar import (
-    FeditAdapterEditButton,
-)
 from ..adapters import (
     adapter_registry,
-    RegistryLookUpError,
     BaseAdapter,
-    AdapterError,
-)
-from ..utils import (
-    _can_edit,
+    RegistryLookUpError,
 )
-from ..hooks import (
-    CONSTRUCT_ADAPTER_TOOLBAR,
+from ..templatetags.fedit import (
+    wrap_adapter,
 )
+from ..utils import (
+    FeditPermissionCheck,
+    FeditIFrameMixin,
+    FEDIT_PREVIEW_VAR,
+    lock_info,
+)
+
+@method_decorator(xframe_options_sameorigin, name="dispatch")
+class BaseAdapterView(FeditIFrameMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
+    template_name = "wagtail_fedit/editor/adapter_iframe.html"
+    ERROR_TITLE = _("Validation Errors")
+
+    def dispatch(self, 
+            request:    HttpRequest,
+            adapter_id: str = None,
+            field_name: str = None,
+            app_label:  str = None,
+            model_name: str = None,
+            model_id:   Any = None,
+        ) -> None:
+
+        # Fetch the adapter class from the registry
+        try:
+            self.adapter_class: BaseAdapter = adapter_registry[adapter_id]
+        except RegistryLookUpError:
+            return HttpResponseBadRequest("Invalid adapter ID")
+
+        # Retrieve the model class
+        try:
+            self.model = apps.get_model(app_label, model_name)
+            if not self.has_perms(request, self.model):
+                return HttpResponseForbidden("You do not have permission to view this page")
+        except LookupError:
+            return HttpResponseBadRequest("Invalid model")
+
+        # Only fetch latest reivision if it exists
+        # If not; it will be automatically created by the form.
+        model_instance = self.model._default_manager.get(pk=model_id)
+        if isinstance(model_instance, RevisionMixin) and model_instance.latest_revision_id:
+            self.instance = model_instance.latest_revision.as_object()
+        else:
+            self.instance = model_instance
 
+        if not hasattr(self.instance, field_name):
+            return HttpResponseBadRequest("Invalid field name for object")
 
-register = library.Library()
-
-
-WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for %(object)s."
-WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for %(object)s."
-
-
-
-class AdapterNode(Node):
-    signer = signing.TimestampSigner()
-
-    def __init__(self, adapter: Type[BaseAdapter], model: FilterExpression, getters: list[str], **kwargs):
-        self.adapter = adapter
-        self.model = model
-        self.getters = getters
-        self.kwargs = kwargs
-
-    def _resolve_expressions(self, context, model, **kwargs):
-        for k, v in kwargs.items():
-            if isinstance(v, FilterExpression):
-                kwargs[k] = v.resolve(context)
-        
-        if isinstance(model, FilterExpression):
-            model = model.resolve(context)
-
-        return model, kwargs
-
-    def render(self, context):
-        model = self.model
-        getters = self.getters
-
-        model, kwargs = self._resolve_expressions(
-            context, model, **self.kwargs,
-        )
-
-        if "wagtail_fedit_field" in context\
-            and "wagtail_fedit_instance" in context\
-            and not model:
-
-            field_name = context["wagtail_fedit_field"]
-            obj = context["wagtail_fedit_instance"]
 
+        shared_context = request.GET.get("shared_context")
+        if shared_context:
+            self.shared_context = self.adapter_class.decode_shared_context(
+                shared_context,
+            )
         else:
+            self.shared_context = {}
 
-            if not model:
-                warnings.warn(
-                    WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {
-                        "object": self.adapter.__name__,
-                    },
-                    RuntimeWarning,
-                )
-
-                context = context.flatten()
-
-                try:
-                    return self.adapter.render_from_kwargs(
-                        context, **kwargs,
-                    )
-                except AdapterError as e:
-                    raise TemplateSyntaxError(str(e))
-
-            field_name = getters[len(getters)-1]
-            obj = model
-            for i in range(len(getters) - 1):
-                getter = getters[i]
-                try:
-                    obj = getattr(obj, getter)
-                except AttributeError:
-                    raise AttributeError(f"Object {model.__class__.__name__} does not have attribute {getter}")
-
-        request = context.get("request")
-        adapter = self.adapter(
-            object=obj,
-            field_name=field_name,
+        self.adapter = self.adapter_class(
             request=request,
-            **kwargs,
+            object=self.instance,
+            field_name=field_name,
+            **self.shared_context,
         )
 
-        if not adapter.check_permissions()\
-          or not _can_edit(request, obj):
-            return adapter.render_content(context)
-
-        return wrap_adapter(request, adapter, context)
-
-
-@register.tag(name="fedit")
-def do_render_fedit(parser: Parser, token: Token):
-
-    tokens = token.split_contents()
-
-    _ = tokens.pop(0)
-    adapter_id = tokens.pop(0)
-
-    try:
-        adapter = adapter_registry[adapter_id]
-    except RegistryLookUpError:
-        raise TemplateSyntaxError(f"No adapter found with identifier '{adapter_id}'")
+        self.lock, self.locked_for_user = lock_info(
+            self.adapter.object, request.user,
+        )
 
-    model, model_tokens = None, None
-    if tokens:
-        model__field = tokens.pop(0)
-        model_tokens = model__field.split(".")
+        setattr(
+            self.request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
 
-        if len(model_tokens) < 2:
-            if model_tokens[0] != "from_context":
-                raise TemplateSyntaxError(
-                    "Model and field name are required: 'mymodel.myfield' or 'from_context'",
-                )
+        return super().dispatch(
+            request, adapter_id, field_name, app_label, model_name, model_id,
+        )
+    
 
-        if len(model_tokens) > 1:
-            # mymodel.myfield
-            # mymodel.related_field.myfield
-            model = parser.compile_filter(model_tokens.pop(0))
-
-    kwargs = get_kwargs(parser, tokens, adapter.required_kwargs)
-
-    return AdapterNode(
-        adapter=adapter,
-        model=model,
-        getters=model_tokens,
-        **kwargs,
-    )
-
-
-def wrap_adapter(request: HttpRequest, adapter: BaseAdapter, context: dict, run_context_processors: bool = False) -> str:
-    if not context:
-        context = {}
-
-    items = [
-        FeditAdapterEditButton(),
-    ]
-
-    for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
-        hook(items=items, adapter=adapter)
-
-    items = [item.render(request) for item in items]
-    items = list(filter(None, items))
-
-    reverse_kwargs = {
-        "adapter_id": adapter.identifier,
-        "field_name": adapter.field_name,
-        "app_label": adapter.object._meta.app_label,
-        "model_name": adapter.object._meta.model_name,
-        "model_id": adapter.object.pk,
-    }
+    def render_to_response(self, context: dict[str, Any], success: bool = True, extra: dict = None, **response_kwargs: Any) -> HttpResponse:
+        if not extra:
+            extra = {}
+
+        extra.update({
+            "success": success,
+        })
+
+        context.update(extra)
+
+        return render(
+            self.request,
+            self.template_name,
+            context,
+        )
+            
+    def get_header_title(self):
+        return self.adapter.get_header_title()
 
-    shared = adapter.encode_shared_context()
-    js_constructor = adapter.get_js_constructor()
+    def get_help_text(self):
+        return self.adapter.get_help_text()
     
-    return render_to_string(
-        "wagtail_fedit/content/editable_adapter.html",
-        {
-            "identifier": adapter.identifier,
-            "adapter": adapter,
-            "buttons": items,
-            "shared": shared,
-            "js_constructor": js_constructor,
-            "shared_context": adapter.kwargs,
-            "parent_context": context,
-            "edit_url": reverse(
-                "wagtail_fedit:edit",
-                kwargs=reverse_kwargs,
+    def get_context_data(self, **kwargs):
+        shared_context = None
+        if self.shared_context:
+            shared_context =\
+                self.request.GET["shared_context"]
+
+        return super().get_context_data(**kwargs) | {
+            "meta_field": self.adapter.meta_field,
+            "field_name": self.adapter.field_name,
+            "locked_for_user": self.locked_for_user,
+            "shared_context": shared_context,
+            "form_attrs": self.adapter.get_form_attrs(),
+            "locked": self.lock is not None,
+        }
+
+class EditAdapterView(BaseAdapterView):
+    def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
+        # Can omit data from context - we are not rendering the content.
+        form = self.adapter.get_form()
+
+        return self.render_to_response(
+            self.get_context_data(
+                form=form,
             ),
-        },
-        request=request if run_context_processors else None,
-    )
-
-@register.simple_tag(takes_context=True)
-def render_adapter(context: Context, adapter: BaseAdapter) -> str:
-    parent_context = {}
-    
-    if "parent_context" in context:
-        parent_context = context["parent_context"]
-        del context["parent_context"]
+            success=True,
+        )
 
-    context.update(parent_context)
+    def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
+        form = self.adapter.get_form()
 
-    context["wagtail_fedit_field"]    = adapter.field_name
-    context["wagtail_fedit_instance"] = adapter.object
-    context["request"]                = adapter.request
+        if not form.is_valid() or self.locked_for_user:
 
-    return adapter.render_content(context)
-    
+            self.adapter.form_invalid(form)
 
-def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None) -> dict:
-    had_kwargs = False
-    kwargs = {}
-
-    if not kwarg_list:
-        kwarg_list = []
-
-    for i, token in enumerate(tokens):
-        split = token.split("=")
-        if len(split) == 1 and len(kwarg_list) > i:
-            if had_kwargs:
-                raise ValueError("Unexpected positional argument after keyword argument")
-            
-            kwargs[kwarg_list[i]] = parser.compile_filter(token)
-        else:
-            key = split[0]
-            # if key not in kwargs_names:
-            #     raise ValueError(f"Unexpected keyword argument {key}")
-            
-            kwargs[key] = parser.compile_filter(split[1])
-            had_kwargs = True
+            return JsonResponse({
+                "success": False,
+                "errors": form.errors,
+                "locked": self.locked_for_user,
+                "html": render_to_string(
+                    self.template_name,
+                    context=self.get_context_data(
+                        form=form,
+                    ),
+                    request=request,
+                )
+            }, status=423 if self.locked_for_user else 400)
 
-    for kwarg in kwarg_list:
-        if kwarg not in kwargs:
-            raise TemplateSyntaxError(f"Missing required keyword argument {kwarg}")
+        
+        self.adapter.form_valid(form)
 
-    return kwargs
+        context = self.get_context_data()
+        if isinstance(self.instance, Page):
+            # Add the page template variable to the context.
+            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
+            context[PAGE_TEMPLATE_VAR] = self.instance
+
+        ## Render the frame HTML
+        #html = wrap_adapter(
+        #    request=self.request,
+        #    adapter=self.adapter,
+        #    context=context,
+        #    run_context_processors=True,
+        #)
+
+        return JsonResponse({
+            "success": True,
+            **self.adapter\
+              .get_response_data(context),
+        })
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Any
+from typing import Any, TYPE_CHECKING
 from collections import namedtuple
 from urllib.parse import urlencode
 from django.db import models
 from django.http import HttpRequest
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
+from django.template.loader import render_to_string
 from django.template.base import FilterExpression
 from django.conf import settings
 from django.urls import reverse
 
 from wagtail import hooks
 from wagtail.models import (
     DraftStateMixin,
@@ -17,21 +18,30 @@
     PreviewableMixin
 )
 from wagtail.admin.admin_url_finder import AdminURLFinder
 from wagtail.blocks.stream_block import StreamValue
 from wagtail.blocks.list_block import ListValue
 from wagtail import blocks
 
+from .toolbar import (
+    FeditToolbarComponent,
+    FeditAdapterEditButton,
+)
 from .hooks import (
     EXCLUDE_FROM_RELATED_FORMS,
     REGISTER_TYPE_RENDERER,
     REGISTER_FIELD_RENDERER,
+    CONSTRUCT_ADAPTER_TOOLBAR,
 )
 
 
+if TYPE_CHECKING:
+    from .adapters.base import BaseAdapter
+
+
 FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
 USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
 
 
 class FeditPermissionCheck:
     @staticmethod
     def has_perms(request: HttpRequest, model: Any) -> bool:
@@ -241,14 +251,18 @@
             break
 
     # The content might be a streamblock etc, we can render it as a block
     # if isinstance(content, (blocks.BoundBlock, blocks.StructValue)):
     if hasattr(content, "render_as_block"):
         content = content.render_as_block(context)
 
+    # The content might otherwise have a render method.
+    elif hasattr(content, "render"):
+        content = content.render(context)
+
     return content
 
 def is_draft_capable(model):
     """
     Check if a model is capable of drafts.
     """
     return isinstance(model, DraftStateMixin)\
@@ -450,8 +464,54 @@
         Resolve a list of possible templatetag filterexpressions.
     """
     def _map(expression):
         if isinstance(expression, FilterExpression):
             return expression.resolve(context)
         return expression
     
-    return tuple(map(_map, expressions))
+    return tuple(map(_map, expressions))
+
+
+
+def wrap_adapter(request: HttpRequest, adapter: "BaseAdapter", context: dict, run_context_processors: bool = False) -> str:
+    if not context:
+        context = {}
+
+    items: list[FeditToolbarComponent] = [
+        FeditAdapterEditButton(),
+        *adapter.get_toolbar_buttons(),
+    ]
+
+    for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
+        hook(items=items, adapter=adapter)
+
+    items = [item.render(request) for item in items]
+    items = list(filter(None, items))
+
+    reverse_kwargs = {
+        "adapter_id": adapter.identifier,
+        "field_name": adapter.field_name,
+        "app_label": adapter.object._meta.app_label,
+        "model_name": adapter.object._meta.model_name,
+        "model_id": adapter.object.pk,
+    }
+
+    shared = adapter.encode_shared_context()
+    js_constructor = adapter.get_js_constructor()
+    
+    return render_to_string(
+        "wagtail_fedit/content/editable_adapter.html",
+        {
+            "identifier": adapter.identifier,
+            "adapter": adapter,
+            "buttons": items,
+            "shared": shared,
+            "js_constructor": js_constructor,
+            "shared_context": adapter.kwargs,
+            "parent_context": context,
+            "edit_url": reverse(
+                "wagtail_fedit:edit",
+                kwargs=reverse_kwargs,
+            ),
+        },
+        request=request if run_context_processors else None,
+    )
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-fedit
-Version: 1.5.1a2
+Name: wagtail_fedit
+Version: 1.5.1a3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,14 +23,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
@@ -40,14 +42,16 @@
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
+- [Adapters Python](#adapters-python)
+- [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
 - [How your content is rendered](#how-your-content-is-rendered)
@@ -224,14 +228,22 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
+## Adapters Python
+
+* TBA
+
+## Adapters Javascript
+
+* TBA
+
 ## Hooks
 
 ### wagtail_fedit.construct_adapter_toolbar
 
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.1a2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
-(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
+wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
+Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
-(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
-[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters Python]
+(#adapters-python) - [Adapters Javascript](#adapters-javascript) - [Hooks]
+(#hooks) - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
+- [Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
 Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
 Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
 (#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
 output-html) - [Implemented](#implemented) Getting Started --------------- 1.
 Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
@@ -98,25 +100,26 @@
 %} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
-block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
-adapter. This is used to display the edit icon for the given adapter. How it is
-called: ```python items = [ FeditAdapterEditButton(), ] for hook in
-hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
-``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
-type. Example of how this type of renderer can be used: ```python
-@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
-This is a custom renderer for the Page model. # It will render the Page model
-as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
-value: format_html( '
+block=item block_id=item.id %} {% endfor %} ``` ## Adapters Python * TBA ##
+Adapters Javascript * TBA ## Hooks ### wagtail_fedit.construct_adapter_toolbar
+Construct the toolbar for the given adapter. This is used to display the edit
+icon for the given adapter. How it is called: ```python items =
+[ FeditAdapterEditButton(), ] for hook in hooks.get_hooks
+(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter) ``` ###
+wagtail_fedit.register_type_renderer Register a custom renderer for a type.
+Example of how this type of renderer can be used: ```python @hooks.register
+(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
+custom renderer for the Page model. # It will render the Page model as a simple
+h2 tag. renderer_map[Page] = lambda request, context, instance, value:
+format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.5.1a2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
 wagtail_fedit/adapters/__init__.py
 wagtail_fedit/adapters/base.py
 wagtail_fedit/adapters/block.py
 wagtail_fedit/adapters/field.py
+wagtail_fedit/adapters/funcs.py
+wagtail_fedit/adapters/misc.py
 wagtail_fedit/adapters/registry.py
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
+wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
```

