# Comparing `tmp/esanom-3.0.1.44.tar.gz` & `tmp/esanom-3.0.2.13384.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-3.0.1.44.tar", max compression
+gzip compressed data, was "esanom-3.0.2.13384.tar", max compression
```

## Comparing `esanom-3.0.1.44.tar` & `esanom-3.0.2.13384.tar`

### file list

```diff
@@ -1,220 +1,363 @@
--rw-r--r--   0        0        0        0 2024-04-19 05:16:47.993237 esanom-3.0.1.44/README.md
--rw-r--r--   0        0        0      144 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/CHANGELOG.txt
--rw-r--r--   0        0        0      388 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/COPYRIGHT.txt
--rw-r--r--   0        0        0    17260 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/LICENCE.txt
--rw-r--r--   0        0        0     1412 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/__init__.py
--rw-r--r--   0        0        0     5950 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/client.py
--rw-r--r--   0        0        0     5156 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/config.py
--rw-r--r--   0        0        0    47586 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/database.py
--rw-r--r--   0        0        0     1125 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/engine.py
--rw-r--r--   0        0        0     2496 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/monitor.py
--rw-r--r--   0        0        0    10320 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/orchestrator.py
--rw-r--r--   0        0        0    12985 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/pipeline.py
--rw-r--r--   0        0        0     1665 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/account.sql
--rw-r--r--   0        0        0     1828 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/api.sql
--rw-r--r--   0        0        0     1352 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/api_group.sql
--rw-r--r--   0        0        0     1326 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/api_role.sql
--rw-r--r--   0        0        0     1226 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/claim.sql
--rw-r--r--   0        0        0     1215 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/group.sql
--rw-r--r--   0        0        0     1828 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/io.sql
--rw-r--r--   0        0        0     1416 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/ioblock.sql
--rw-r--r--   0        0        0     1680 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/log.sql
--rw-r--r--   0        0        0     1950 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/mpin.sql
--rw-r--r--   0        0        0     1921 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/mport.sql
--rw-r--r--   0        0        0     1536 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/pin.sql
--rw-r--r--   0        0        0     1842 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/pipeline.sql
--rw-r--r--   0        0        0     1514 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/pipeline_task.sql
--rw-r--r--   0        0        0     1501 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/port.sql
--rw-r--r--   0        0        0     1388 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/port_pin.sql
--rw-r--r--   0        0        0     1126 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/role.sql
--rw-r--r--   0        0        0     1250 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/roleadmin.sql
--rw-r--r--   0        0        0     1257 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/roledashboard.sql
--rw-r--r--   0        0        0     2173 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/rolemodel.sql
--rw-r--r--   0        0        0     1655 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/roleuser.sql
--rw-r--r--   0        0        0     1319 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/schedule.sql
--rw-r--r--   0        0        0     1156 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/session.sql
--rw-r--r--   0        0        0     1236 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/system.sql
--rw-r--r--   0        0        0     1914 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/task.sql
--rw-r--r--   0        0        0     5741 2024-04-19 05:16:48.441235 esanom-3.0.1.44/esanom/resources/database/triggers.sql
--rw-r--r--   0        0        0     1497 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/resources/database/unit.sql
--rw-r--r--   0        0        0    11022 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/roleadmin.py
--rw-r--r--   0        0        0     4208 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/rolemodel.py
--rw-r--r--   0        0        0     3456 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/roleuser.py
--rw-r--r--   0        0        0      790 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/__init__.py
--rw-r--r--   0        0        0    38001 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/api.py
--rw-r--r--   0        0        0    40721 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/api.py-bak1
--rw-r--r--   0        0        0     8952 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/common.py
--rw-r--r--   0        0        0    80721 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   232803 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/bootstrap.min.css
--rw-r--r--   0        0        0      639 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/dashboard.css
--rw-r--r--   0        0        0    20832 2024-04-19 05:16:48.461235 esanom-3.0.1.44/esanom/routes/v3/static/datatables.min.css
--rw-r--r--   0        0        0   197654 2024-04-19 05:16:48.461235 esanom-3.0.1.44/esanom/routes/v3/static/datatables.min.js
--rw-r--r--   0        0        0      318 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/favicon.ico
--rw-r--r--   0        0        0    48036 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/htmx.min.js
--rw-r--r--   0        0        0       97 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/main.css
--rw-r--r--   0        0        0      422 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/main.js
--rw-r--r--   0        0        0     1723 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/nom-logo.png
--rw-r--r--   0        0        0  3620840 2024-04-19 05:16:48.461235 esanom-3.0.1.44/esanom/routes/v3/static/plotly.min.js
--rw-r--r--   0        0        0     1741 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/static/theme.css
--rw-r--r--   0        0        0      717 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/admin_db_pipeline_row.html
--rw-r--r--   0        0        0      627 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/admin_db_pipeline_rows.html
--rw-r--r--   0        0        0     1542 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/base.html
--rw-r--r--   0        0        0     1000 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/db_rolemodel_row.html
--rw-r--r--   0        0        0      633 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/db_rolemodel_rows.html
--rw-r--r--   0        0        0      140 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/dummy.html
--rw-r--r--   0        0        0      153 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/error_404.html
--rw-r--r--   0        0        0      114 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/error_500.html
--rw-r--r--   0        0        0       82 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
--rw-r--r--   0        0        0      731 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_model_io.html
--rw-r--r--   0        0        0     1331 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_model_io_port.html
--rw-r--r--   0        0        0      808 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_models.html
--rw-r--r--   0        0        0      836 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_pipelines.html
--rw-r--r--   0        0        0     2019 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_debug.html
--rw-r--r--   0        0        0      248 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_loggedin_nav.html
--rw-r--r--   0        0        0      586 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
--rw-r--r--   0        0        0      300 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
--rw-r--r--   0        0        0      282 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_loggedin_nav_member.html
--rw-r--r--   0        0        0      182 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_footer.html
--rw-r--r--   0        0        0      628 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_head.html
--rw-r--r--   0        0        0     1332 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_header.html
--rw-r--r--   0        0        0      173 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_header_logo.html
--rw-r--r--   0        0        0      487 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_header_nav.html
--rw-r--r--   0        0        0      240 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_header_toggle.html
--rw-r--r--   0        0        0      153 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/navigation.html
--rw-r--r--   0        0        0      327 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_admin_pipelines.html
--rw-r--r--   0        0        0      921 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_dashboard_tasks.html
--rw-r--r--   0        0        0      115 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_docs.html
--rw-r--r--   0        0        0      116 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_index.html
--rw-r--r--   0        0        0      121 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_interfaces.html
--rw-r--r--   0        0        0      516 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_model.html
--rw-r--r--   0        0        0      157 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/templates/page_models.html
--rw-r--r--   0        0        0      128 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin/main.html
--rw-r--r--   0        0        0       94 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
--rw-r--r--   0        0        0     1378 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
--rw-r--r--   0        0        0      188 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_account_create/main.html
--rw-r--r--   0        0        0        5 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
--rw-r--r--   0        0        0      110 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
--rw-r--r--   0        0        0      429 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
--rw-r--r--   0        0        0      299 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
--rw-r--r--   0        0        0      315 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/main.html
--rw-r--r--   0        0        0      272 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/read.html
--rw-r--r--   0        0        0      114 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
--rw-r--r--   0        0        0      248 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
--rw-r--r--   0        0        0      207 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/update.html
--rw-r--r--   0        0        0     1887 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
--rw-r--r--   0        0        0      113 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
--rw-r--r--   0        0        0      544 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_read/main.html
--rw-r--r--   0        0        0        6 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
--rw-r--r--   0        0        0     1221 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
--rw-r--r--   0        0        0      474 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
--rw-r--r--   0        0        0      256 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_update/main.html
--rw-r--r--   0        0        0      421 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
--rw-r--r--   0        0        0      369 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
--rw-r--r--   0        0        0      240 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_apis/main.html
--rw-r--r--   0        0        0       94 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
--rw-r--r--   0        0        0      324 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
--rw-r--r--   0        0        0      263 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_create/main.html
--rw-r--r--   0        0        0      111 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
--rw-r--r--   0        0        0      278 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_read/main.html
--rw-r--r--   0        0        0        6 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
--rw-r--r--   0        0        0      718 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
--rw-r--r--   0        0        0      352 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_update/main.html
--rw-r--r--   0        0        0       87 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
--rw-r--r--   0        0        0      425 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_groups/main.html
--rw-r--r--   0        0        0      111 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
--rw-r--r--   0        0        0      332 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_read/main.html
--rw-r--r--   0        0        0       24 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
--rw-r--r--   0        0        0      897 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
--rw-r--r--   0        0        0      403 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_update/main.html
--rw-r--r--   0        0        0      425 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_models/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
--rw-r--r--   0        0        0      245 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_models/main.html
--rw-r--r--   0        0        0       40 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
--rw-r--r--   0        0        0      307 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/inc_form_pins.html
--rw-r--r--   0        0        0      311 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/inc_form_ports.html
--rw-r--r--   0        0        0      413 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
--rw-r--r--   0        0        0      463 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
--rw-r--r--   0        0        0      380 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_settings/main.html
--rw-r--r--   0        0        0       82 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
--rw-r--r--   0        0        0       82 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
--rw-r--r--   0        0        0      118 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/main.html
--rw-r--r--   0        0        0      895 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/pipelines.html
--rw-r--r--   0        0        0      891 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/tasks.html
--rw-r--r--   0        0        0      640 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
--rw-r--r--   0        0        0     1218 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
--rw-r--r--   0        0        0       26 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
--rw-r--r--   0        0        0      770 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
--rw-r--r--   0        0        0      128 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/main.html
--rw-r--r--   0        0        0       60 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/login/hx_login.html
--rw-r--r--   0        0        0      766 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/login/main.html
--rw-r--r--   0        0        0      133 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/logout/main.html
--rw-r--r--   0        0        0      128 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member/main.html
--rw-r--r--   0        0        0      617 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
--rw-r--r--   0        0        0      789 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
--rw-r--r--   0        0        0      182 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_api_create/main.html
--rw-r--r--   0        0        0      347 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
--rw-r--r--   0        0        0      423 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/inc_table.html
--rw-r--r--   0        0        0      367 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
--rw-r--r--   0        0        0      416 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/main.html
--rw-r--r--   0        0        0      256 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/read.html
--rw-r--r--   0        0        0      129 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/update.html
--rw-r--r--   0        0        0      637 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
--rw-r--r--   0        0        0      347 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
--rw-r--r--   0        0        0      442 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/inc_table.html
--rw-r--r--   0        0        0      163 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
--rw-r--r--   0        0        0      241 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/main.html
--rw-r--r--   0        0        0      256 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/read.html
--rw-r--r--   0        0        0      129 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/update.html
--rw-r--r--   0        0        0      637 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
--rw-r--r--   0        0        0      428 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read.html
--rw-r--r--   0        0        0      160 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_info.html
--rw-r--r--   0        0        0     1331 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_port.html
--rw-r--r--   0        0        0     1331 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
--rw-r--r--   0        0        0      733 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_ports.html
--rw-r--r--   0        0        0      238 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/rows.html
--rw-r--r--   0        0        0      424 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/rows_inc_table.html
--rw-r--r--   0        0        0      607 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
--rw-r--r--   0        0        0      322 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/read.html
--rw-r--r--   0        0        0       92 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/read_inc_info.html
--rw-r--r--   0        0        0      174 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
--rw-r--r--   0        0        0      130 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
--rw-r--r--   0        0        0      432 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
--rw-r--r--   0        0        0      234 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/rows.html
--rw-r--r--   0        0        0      420 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
--rw-r--r--   0        0        0      339 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/read.html
--rw-r--r--   0        0        0       92 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/read_inc_info.html
--rw-r--r--   0        0        0      422 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/read_inc_table.html
--rw-r--r--   0        0        0      309 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
--rw-r--r--   0        0        0      125 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
--rw-r--r--   0        0        0      236 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/rows.html
--rw-r--r--   0        0        0      422 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
--rw-r--r--   0        0        0      340 2024-04-19 05:16:48.453235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-19 05:16:48.457235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
--rw-r--r--   0        0        0      265 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/register/hx_form.html
--rw-r--r--   0        0        0      387 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/register/main.html
--rw-r--r--   0        0        0     1037 2024-04-19 05:16:48.449235 esanom-3.0.1.44/esanom/routes/v3/templates/pages/register/main_inc_form.html
--rw-r--r--   0        0        0    53913 2024-04-19 05:16:48.445235 esanom-3.0.1.44/esanom/routes/v3/web.py
--rw-r--r--   0        0        0     1693 2024-04-19 05:16:48.461235 esanom-3.0.1.44/esanom/sample_gunicorn_config.py
--rw-r--r--   0        0        0      753 2024-04-19 05:16:48.465235 esanom-3.0.1.44/esanom/sample_nom_config.json
--rw-r--r--   0        0        0     5050 2024-04-19 05:16:48.465235 esanom-3.0.1.44/esanom/scheduler.py
--rw-r--r--   0        0        0     3698 2024-04-19 05:16:48.465235 esanom-3.0.1.44/esanom/server.py
--rw-r--r--   0        0        0    12199 2024-04-19 05:16:48.465235 esanom-3.0.1.44/esanom/util.py
--rw-r--r--   0        0        0      442 2024-04-19 05:16:50.977227 esanom-3.0.1.44/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 esanom-3.0.1.44/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 12:24:38.683824 esanom-3.0.2.13384/README.md
+-rw-r--r--   0        0        0      144 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/CHANGELOG.txt
+-rw-r--r--   0        0        0      388 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/COPYRIGHT.txt
+-rw-r--r--   0        0        0    17260 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/LICENCE.txt
+-rw-r--r--   0        0        0     1412 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/__init__.py
+-rw-r--r--   0        0        0     6268 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/client.py
+-rw-r--r--   0        0        0     5156 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/config.py
+-rw-r--r--   0        0        0    47611 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/database.py
+-rw-r--r--   0        0        0     1125 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/engine.py
+-rw-r--r--   0        0        0     2496 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/monitor.py
+-rw-r--r--   0        0        0    10320 2024-04-20 12:24:39.171822 esanom-3.0.2.13384/esanom/orchestrator.py
+-rw-r--r--   0        0        0    12985 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/pipeline.py
+-rw-r--r--   0        0        0     1665 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/account.sql
+-rw-r--r--   0        0        0     1828 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/api.sql
+-rw-r--r--   0        0        0     1352 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/api_group.sql
+-rw-r--r--   0        0        0     1326 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/api_role.sql
+-rw-r--r--   0        0        0     1226 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/claim.sql
+-rw-r--r--   0        0        0     1215 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/group.sql
+-rw-r--r--   0        0        0     1828 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/io.sql
+-rw-r--r--   0        0        0     1416 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/ioblock.sql
+-rw-r--r--   0        0        0     1680 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/log.sql
+-rw-r--r--   0        0        0     1950 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/mpin.sql
+-rw-r--r--   0        0        0     1921 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/mport.sql
+-rw-r--r--   0        0        0     1536 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/pin.sql
+-rw-r--r--   0        0        0     1842 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/pipeline.sql
+-rw-r--r--   0        0        0     1514 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/pipeline_task.sql
+-rw-r--r--   0        0        0     1501 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/port.sql
+-rw-r--r--   0        0        0     1388 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/port_pin.sql
+-rw-r--r--   0        0        0     1126 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/role.sql
+-rw-r--r--   0        0        0     1250 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/roleadmin.sql
+-rw-r--r--   0        0        0     1257 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/roledashboard.sql
+-rw-r--r--   0        0        0     2173 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/rolemodel.sql
+-rw-r--r--   0        0        0     1655 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/roleuser.sql
+-rw-r--r--   0        0        0     1319 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/schedule.sql
+-rw-r--r--   0        0        0     1156 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/session.sql
+-rw-r--r--   0        0        0     1236 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/system.sql
+-rw-r--r--   0        0        0     1914 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/task.sql
+-rw-r--r--   0        0        0     5904 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/triggers.sql
+-rw-r--r--   0        0        0     1497 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/database/unit.sql
+-rw-r--r--   0        0        0     1108 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/interfaces/pins.json
+-rw-r--r--   0        0        0      680 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/resources/interfaces/ports.json
+-rw-r--r--   0        0        0    11022 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/roleadmin.py
+-rw-r--r--   0        0        0     4208 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/rolemodel.py
+-rw-r--r--   0        0        0     3456 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/roleuser.py
+-rw-r--r--   0        0        0      790 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/__init__.py
+-rw-r--r--   0        0        0    37835 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/api.py
+-rw-r--r--   0        0        0    40721 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/api.py-bak1
+-rw-r--r--   0        0        0     8971 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/common.py
+-rw-r--r--   0        0        0    80721 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   232803 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/bootstrap.min.css
+-rw-r--r--   0        0        0      639 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/dashboard.css
+-rw-r--r--   0        0        0    20832 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/routes/v3/static/datatables.min.css
+-rw-r--r--   0        0        0   197654 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/routes/v3/static/datatables.min.js
+-rw-r--r--   0        0        0      318 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/favicon.ico
+-rw-r--r--   0        0        0    48036 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/htmx.min.js
+-rw-r--r--   0        0        0       97 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/static/main.css
+-rw-r--r--   0        0        0      422 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/main.js
+-rw-r--r--   0        0        0     2362 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/nom-logo.png
+-rw-r--r--   0        0        0  3620840 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/routes/v3/static/plotly.min.js
+-rw-r--r--   0        0        0     1741 2024-04-20 12:24:39.191822 esanom-3.0.2.13384/esanom/routes/v3/static/theme.css
+-rw-r--r--   0        0        0      717 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/admin_db_pipeline_row.html
+-rw-r--r--   0        0        0      627 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/admin_db_pipeline_rows.html
+-rw-r--r--   0        0        0     1542 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/base.html
+-rw-r--r--   0        0        0     1000 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/db_rolemodel_row.html
+-rw-r--r--   0        0        0      633 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/db_rolemodel_rows.html
+-rw-r--r--   0        0        0      140 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/dummy.html
+-rw-r--r--   0        0        0      153 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/error_404.html
+-rw-r--r--   0        0        0      114 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/error_500.html
+-rw-r--r--   0        0        0       82 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
+-rw-r--r--   0        0        0      731 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_model_io.html
+-rw-r--r--   0        0        0     1331 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_model_io_port.html
+-rw-r--r--   0        0        0      808 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_models.html
+-rw-r--r--   0        0        0      836 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_pipelines.html
+-rw-r--r--   0        0        0     2019 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_debug.html
+-rw-r--r--   0        0        0      248 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_loggedin_nav.html
+-rw-r--r--   0        0        0      586 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
+-rw-r--r--   0        0        0      300 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
+-rw-r--r--   0        0        0      282 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_loggedin_nav_member.html
+-rw-r--r--   0        0        0      182 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_footer.html
+-rw-r--r--   0        0        0      628 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_head.html
+-rw-r--r--   0        0        0     1332 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_header.html
+-rw-r--r--   0        0        0      173 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_header_logo.html
+-rw-r--r--   0        0        0      487 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_header_nav.html
+-rw-r--r--   0        0        0      240 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_header_toggle.html
+-rw-r--r--   0        0        0      153 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/navigation.html
+-rw-r--r--   0        0        0      327 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_admin_pipelines.html
+-rw-r--r--   0        0        0      921 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_dashboard_tasks.html
+-rw-r--r--   0        0        0      115 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_docs.html
+-rw-r--r--   0        0        0      367 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_index.html
+-rw-r--r--   0        0        0      121 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_interfaces.html
+-rw-r--r--   0        0        0      516 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_model.html
+-rw-r--r--   0        0        0      157 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/page_models.html
+-rw-r--r--   0        0        0      128 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin/main.html
+-rw-r--r--   0        0        0       94 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
+-rw-r--r--   0        0        0     1378 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
+-rw-r--r--   0        0        0      188 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_account_create/main.html
+-rw-r--r--   0        0        0        5 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
+-rw-r--r--   0        0        0      110 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
+-rw-r--r--   0        0        0      429 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
+-rw-r--r--   0        0        0      299 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
+-rw-r--r--   0        0        0      315 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/main.html
+-rw-r--r--   0        0        0      272 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/read.html
+-rw-r--r--   0        0        0      114 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
+-rw-r--r--   0        0        0      248 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
+-rw-r--r--   0        0        0      207 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/update.html
+-rw-r--r--   0        0        0     1887 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
+-rw-r--r--   0        0        0      113 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
+-rw-r--r--   0        0        0      544 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
+-rw-r--r--   0        0        0     1221 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
+-rw-r--r--   0        0        0      474 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
+-rw-r--r--   0        0        0      256 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_update/main.html
+-rw-r--r--   0        0        0      421 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
+-rw-r--r--   0        0        0      369 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
+-rw-r--r--   0        0        0      240 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_apis/main.html
+-rw-r--r--   0        0        0       94 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
+-rw-r--r--   0        0        0      324 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
+-rw-r--r--   0        0        0      263 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_create/main.html
+-rw-r--r--   0        0        0      111 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
+-rw-r--r--   0        0        0      278 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
+-rw-r--r--   0        0        0      718 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
+-rw-r--r--   0        0        0      352 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_update/main.html
+-rw-r--r--   0        0        0       87 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
+-rw-r--r--   0        0        0      425 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_groups/main.html
+-rw-r--r--   0        0        0      111 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
+-rw-r--r--   0        0        0      332 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_read/main.html
+-rw-r--r--   0        0        0       24 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
+-rw-r--r--   0        0        0      897 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
+-rw-r--r--   0        0        0      403 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_update/main.html
+-rw-r--r--   0        0        0      425 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_models/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
+-rw-r--r--   0        0        0      245 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_models/main.html
+-rw-r--r--   0        0        0       40 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
+-rw-r--r--   0        0        0      307 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/inc_form_pins.html
+-rw-r--r--   0        0        0      311 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/inc_form_ports.html
+-rw-r--r--   0        0        0      413 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
+-rw-r--r--   0        0        0      463 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
+-rw-r--r--   0        0        0      380 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_settings/main.html
+-rw-r--r--   0        0        0       82 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
+-rw-r--r--   0        0        0       82 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
+-rw-r--r--   0        0        0      118 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/main.html
+-rw-r--r--   0        0        0      895 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/pipelines.html
+-rw-r--r--   0        0        0      891 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/tasks.html
+-rw-r--r--   0        0        0      640 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
+-rw-r--r--   0        0        0     1218 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
+-rw-r--r--   0        0        0       26 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
+-rw-r--r--   0        0        0      770 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
+-rw-r--r--   0        0        0      128 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/main.html
+-rw-r--r--   0        0        0       60 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/login/hx_login.html
+-rw-r--r--   0        0        0      766 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/login/main.html
+-rw-r--r--   0        0        0      133 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/logout/main.html
+-rw-r--r--   0        0        0      128 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member/main.html
+-rw-r--r--   0        0        0      617 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
+-rw-r--r--   0        0        0      789 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
+-rw-r--r--   0        0        0      182 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_api_create/main.html
+-rw-r--r--   0        0        0      347 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
+-rw-r--r--   0        0        0      423 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/inc_table.html
+-rw-r--r--   0        0        0      367 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
+-rw-r--r--   0        0        0      416 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/main.html
+-rw-r--r--   0        0        0      256 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/read.html
+-rw-r--r--   0        0        0      129 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/update.html
+-rw-r--r--   0        0        0      637 2024-04-20 12:24:39.183822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
+-rw-r--r--   0        0        0      347 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
+-rw-r--r--   0        0        0      442 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/inc_table.html
+-rw-r--r--   0        0        0      163 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
+-rw-r--r--   0        0        0      241 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/main.html
+-rw-r--r--   0        0        0      256 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/read.html
+-rw-r--r--   0        0        0      129 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/update.html
+-rw-r--r--   0        0        0      637 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
+-rw-r--r--   0        0        0      428 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read.html
+-rw-r--r--   0        0        0      160 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_info.html
+-rw-r--r--   0        0        0     1331 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_port.html
+-rw-r--r--   0        0        0     1331 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
+-rw-r--r--   0        0        0      733 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_ports.html
+-rw-r--r--   0        0        0      238 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/rows.html
+-rw-r--r--   0        0        0      424 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/rows_inc_table.html
+-rw-r--r--   0        0        0      609 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
+-rw-r--r--   0        0        0      322 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/read.html
+-rw-r--r--   0        0        0       92 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/read_inc_info.html
+-rw-r--r--   0        0        0      174 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
+-rw-r--r--   0        0        0      130 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
+-rw-r--r--   0        0        0      432 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
+-rw-r--r--   0        0        0      234 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/rows.html
+-rw-r--r--   0        0        0      420 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
+-rw-r--r--   0        0        0      339 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/read.html
+-rw-r--r--   0        0        0       92 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/read_inc_info.html
+-rw-r--r--   0        0        0      422 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/read_inc_table.html
+-rw-r--r--   0        0        0      309 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
+-rw-r--r--   0        0        0      125 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
+-rw-r--r--   0        0        0      236 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/rows.html
+-rw-r--r--   0        0        0      422 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
+-rw-r--r--   0        0        0      340 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.187822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
+-rw-r--r--   0        0        0      265 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/register/hx_form.html
+-rw-r--r--   0        0        0      455 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/register/main.html
+-rw-r--r--   0        0        0     1037 2024-04-20 12:24:39.179822 esanom-3.0.2.13384/esanom/routes/v3/templates/pages/register/main_inc_form.html
+-rw-r--r--   0        0        0    54155 2024-04-20 12:24:39.175822 esanom-3.0.2.13384/esanom/routes/v3/web.py
+-rw-r--r--   0        0        0     1693 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/sample_gunicorn_config.py
+-rw-r--r--   0        0        0      753 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/sample_nom_config.json
+-rw-r--r--   0        0        0     5050 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/scheduler.py
+-rw-r--r--   0        0        0     3698 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/server.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/test_a_1.py
+-rw-r--r--   0        0        0      628 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_create/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/test_a_1.py
+-rw-r--r--   0        0        0      861 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/admin/admin_delete/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/test_a_1.py
+-rw-r--r--   0        0        0      903 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/test_a_1.py
+-rw-r--r--   0        0        0      606 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/test_a_1.py
+-rw-r--r--   0        0        0      665 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_state_table_row/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/test_a_1.py
+-rw-r--r--   0        0        0      843 2024-04-20 12:24:39.195822 esanom-3.0.2.13384/esanom/tests/admin/admin_update/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/__init__.py
+-rw-r--r--   0        0        0     1522 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/account.desc
+-rw-r--r--   0        0        0     1567 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/api.desc
+-rw-r--r--   0        0        0      323 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/api_group.desc
+-rw-r--r--   0        0        0      313 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/api_role.desc
+-rw-r--r--   0        0        0      676 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/claim.desc
+-rw-r--r--   0        0        0      519 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/group.desc
+-rw-r--r--   0        0        0     1511 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/io.desc
+-rw-r--r--   0        0        0      880 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/ioblock.desc
+-rw-r--r--   0        0        0     1163 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/log.desc
+-rw-r--r--   0        0        0     1485 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/mpin.desc
+-rw-r--r--   0        0        0     1491 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/mport.desc
+-rw-r--r--   0        0        0      979 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/pin.desc
+-rw-r--r--   0        0        0     1512 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/pipeline.desc
+-rw-r--r--   0        0        0      428 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/pipeline_task.desc
+-rw-r--r--   0        0        0      882 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/port.desc
+-rw-r--r--   0        0        0      415 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/port_pin.desc
+-rw-r--r--   0        0        0      419 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/role.desc
+-rw-r--r--   0        0        0      478 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/roleadmin.desc
+-rw-r--r--   0        0        0      478 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/roledashboard.desc
+-rw-r--r--   0        0        0     2205 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/rolemodel.desc
+-rw-r--r--   0        0        0     1451 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/roleuser.desc
+-rw-r--r--   0        0        0      574 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/schedule.desc
+-rw-r--r--   0        0        0      565 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/session.desc
+-rw-r--r--   0        0        0      765 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/system.desc
+-rw-r--r--   0        0        0     1872 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/task.desc
+-rw-r--r--   0        0        0      973 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/cache/unit.desc
+-rw-r--r--   0        0        0      154 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/run.sh
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/sample_nom_config.json
+-rw-r--r--   0        0        0      837 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/test_a_1.py
+-rw-r--r--   0        0        0     1468 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/schema/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/database/version/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/database/version/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/database/version/run.sh
+-rw-r--r--   0        0        0      209 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/database/version/sample_nom_config.json
+-rw-r--r--   0        0        0      837 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/database/version/test_a_1.py
+-rw-r--r--   0        0        0     1189 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/database/version/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/test_a_1.py
+-rw-r--r--   0        0        0     1665 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/tests/e2e/cancel_infiniteloop/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/test_a_1.py
+-rw-r--r--   0        0        0      846 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/ping/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/__init__.py
+-rw-r--r--   0        0        0    31700 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/cache/output.png
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/test_a_1.py
+-rw-r--r--   0        0        0     1451 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/pingplot/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/__init__.py
+-rw-r--r--   0        0        0    16864 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/cache/output.png
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/test_a_1.py
+-rw-r--r--   0        0        0     1429 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/plot/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/__init__.py
+-rw-r--r--   0        0        0    19796 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/cache/output_sd2_plot.png
+-rw-r--r--   0        0        0    55560 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/cache/output_trajx_plot.png
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/test_a_1.py
+-rw-r--r--   0        0        0     3070 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/__init__.py
+-rw-r--r--   0        0        0    19796 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/cache/output_sd2_plot.png
+-rw-r--r--   0        0        0    55560 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/cache/output_trajx_plot.png
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/test_a_1.py
+-rw-r--r--   0        0        0     1900 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_ae8ap8_sd2_email/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/__init__.py
+-rw-r--r--   0        0        0    18862 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/cache/output.xlsx
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/test_a_1.py
+-rw-r--r--   0        0        0     2045 2024-04-20 12:24:39.203822 esanom-3.0.2.13384/esanom/tests/e2e/trajx_xlsx/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/test_a_1.py
+-rw-r--r--   0        0        0      681 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/model/model_state/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/test_a_1.py
+-rw-r--r--   0        0        0      844 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_pipeline/test_b_1.py
+-rw-r--r--   0        0        0       76 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/nom_config.json
+-rwxr-xr-x   0        0        0      124 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/run.sh
+-rw-r--r--   0        0        0       93 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/sample_nom_config.json
+-rw-r--r--   0        0        0      752 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/test_a_1.py
+-rw-r--r--   0        0        0      638 2024-04-20 12:24:39.199822 esanom-3.0.2.13384/esanom/tests/user/user_state/test_b_1.py
+-rw-r--r--   0        0        0    12199 2024-04-20 12:24:39.207822 esanom-3.0.2.13384/esanom/util.py
+-rw-r--r--   0        0        0      445 2024-04-20 12:24:44.527804 esanom-3.0.2.13384/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 esanom-3.0.2.13384/PKG-INFO
```

### Comparing `esanom-3.0.1.44/esanom/LICENCE.txt` & `esanom-3.0.2.13384/esanom/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/__init__.py` & `esanom-3.0.2.13384/esanom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # This file is subject to the terms and conditions defined in file 'LICENCE.txt', 
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 #####################################################################
 
 from importlib.metadata import version
 
 print( f"NoM v{version('esanom')} Copyright 2024 © European Space Agency. All rights reserved." )
```

### Comparing `esanom-3.0.1.44/esanom/client.py` & `esanom-3.0.2.13384/esanom/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,16 +215,22 @@
 def user_pipeline_await( pipeline ) :
 
     pipeline_name = pipeline.name
 
     t0 = time.time( )
 
     while not pipeline.done :
+        status={"PIPELINE":pipeline.status}
+        #pipeline.nodes[ "ping" ][ "task_status" ]
+        if pipeline.status!="RESERVED" :
+            for node_i , ( node_name , node_value ) in enumerate( pipeline.nodes.items( ) ) :
+                status[node_name]=node_value["task_status"]
         dt = int( time.time( ) - t0 )
         print( f"[{dt}] awaiting {pipeline_name}")
+        print( f"{status}")
         time.sleep( 5 )
         pipeline = user_pipeline( pipeline_name )
 
     if pipeline.done :
         print( "PIPELINE DONE" )
     else :
         print( "PIPELINE NOT DONE" )
```

### Comparing `esanom-3.0.1.44/esanom/config.py` & `esanom-3.0.2.13384/esanom/config.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/database.py` & `esanom-3.0.2.13384/esanom/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,24 +229,28 @@
 
     vals.append( id )
 
     kset_str = ",".join( kset )
 
     sql = f"UPDATE `{table}` SET {kset_str} WHERE `{cid}`=%s LIMIT 1"
 
+    #print(sql)
+    #print(vals)
+
     db_query_update( sql , vals )
 
 def delete_fromid( table , id ) :
     
     if not table in NOMTABLES : return( None )
 
     sql = f"DELETE from `{table}` WHERE id=%s LIMIT 1"
     vals = [ id ]
 
-    return( db_query_delete( sql , vals ) )
+    db_query_delete( sql , vals )
+
 
 #####################################################################
 
 def db_query_insert( sql , params = None ) :
 
     #print(sql)
     #print(params)
```

### Comparing `esanom-3.0.1.44/esanom/engine.py` & `esanom-3.0.2.13384/esanom/engine.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/monitor.py` & `esanom-3.0.2.13384/esanom/monitor.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/orchestrator.py` & `esanom-3.0.2.13384/esanom/orchestrator.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/pipeline.py` & `esanom-3.0.2.13384/esanom/pipeline.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/account.sql` & `esanom-3.0.2.13384/esanom/resources/database/account.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/api.sql` & `esanom-3.0.2.13384/esanom/resources/database/api.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/api_group.sql` & `esanom-3.0.2.13384/esanom/resources/database/api_group.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/api_role.sql` & `esanom-3.0.2.13384/esanom/resources/database/api_role.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/claim.sql` & `esanom-3.0.2.13384/esanom/resources/database/claim.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/group.sql` & `esanom-3.0.2.13384/esanom/resources/database/group.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/io.sql` & `esanom-3.0.2.13384/esanom/resources/database/io.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/ioblock.sql` & `esanom-3.0.2.13384/esanom/resources/database/ioblock.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/log.sql` & `esanom-3.0.2.13384/esanom/resources/database/log.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/mpin.sql` & `esanom-3.0.2.13384/esanom/resources/database/mpin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/mport.sql` & `esanom-3.0.2.13384/esanom/resources/database/mport.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/pin.sql` & `esanom-3.0.2.13384/esanom/resources/database/pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/pipeline.sql` & `esanom-3.0.2.13384/esanom/resources/database/pipeline.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/pipeline_task.sql` & `esanom-3.0.2.13384/esanom/resources/database/pipeline_task.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/port.sql` & `esanom-3.0.2.13384/esanom/resources/database/port.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/port_pin.sql` & `esanom-3.0.2.13384/esanom/resources/database/port_pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/role.sql` & `esanom-3.0.2.13384/esanom/resources/database/role.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/roleadmin.sql` & `esanom-3.0.2.13384/esanom/resources/database/roleadmin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/roledashboard.sql` & `esanom-3.0.2.13384/esanom/resources/database/roledashboard.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/rolemodel.sql` & `esanom-3.0.2.13384/esanom/resources/database/rolemodel.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/roleuser.sql` & `esanom-3.0.2.13384/esanom/resources/database/roleuser.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/schedule.sql` & `esanom-3.0.2.13384/esanom/resources/database/schedule.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/session.sql` & `esanom-3.0.2.13384/esanom/resources/database/session.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/system.sql` & `esanom-3.0.2.13384/esanom/resources/database/system.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/task.sql` & `esanom-3.0.2.13384/esanom/resources/database/task.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/resources/database/triggers.sql` & `esanom-3.0.2.13384/esanom/resources/database/triggers.sql`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 CREATE TRIGGER account_insert BEFORE INSERT ON account FOR EACH ROW BEGIN
 
     IF ( NEW.email_confirmed = 1 ) THEN
         SET NEW.email_confirmsent_at = NOW( ) ;
         SET NEW.email_confirmed_at = NOW( ) ;
     END IF ;
 
-    SET NEW.password = SHA2( NEW.password , 256 ) ;
+    IF NEW.password IS NULL THEN
+        SET NEW.password = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
+    ELSE
+        SET NEW.password = SHA2( NEW.password , 256 ) ;
+    END IF ;
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
 CREATE TRIGGER account_update BEFORE UPDATE ON account FOR EACH ROW BEGIN
```

### Comparing `esanom-3.0.1.44/esanom/resources/database/unit.sql` & `esanom-3.0.2.13384/esanom/resources/database/unit.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/roleadmin.py` & `esanom-3.0.2.13384/esanom/roleadmin.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/rolemodel.py` & `esanom-3.0.2.13384/esanom/rolemodel.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/roleuser.py` & `esanom-3.0.2.13384/esanom/roleuser.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/__init__.py` & `esanom-3.0.2.13384/esanom/routes/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/api.py` & `esanom-3.0.2.13384/esanom/routes/v3/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,15 @@
     if table.strip( ) == "" : return( _common.response_error( e_msg = "table blank" ) )
 
     id_str = request.args.get( "id" , default = "" ) 
     if not id_str.isdigit( ): return( _common.response_error( e_msg = "id not isdigit" ) )
     id = int( float( id_str ) )
     if not id > 0 : return( _common.response_error( e_msg = "not id" ) )
 
-    res = _database.update_fromdict( table , id , request.json )
-
-    if res == None : return( _common.response_error( e_msg = "res none" ) )
+    _database.update_fromdict( table , id , request.json )
 
     return( _common.response_default( ) )
 
 @ROUTES.route( "/admin_delete" , methods = [ "POST" ] )
 @_common.decorator_token_required
 @_common.decorator_role_required( "admin" )
 @_common.decorator_request_json
@@ -165,17 +163,15 @@
     if table.strip( ) == "" : return( _common.response_error( e_msg = "table blank" ) )
 
     id_str = request.args.get( "id" , default = "" ) 
     if not id_str.isdigit( ) : return( _common.response_error( e_msg = "id not isdigit" ) )
     id = int( float( id_str ) )
     if not id > 0 : return( _common.response_error( e_msg = "not id" ) )
 
-    res = _database.delete_fromid( table , id )
-
-    if res == None : return( _common.response_error( e_msg = "res none" ) )
+    _database.delete_fromid( table , id )
 
     return( _common.response_default( ) )
 
 
 @ROUTES.route( "/admin_delete_bulk" , methods = [ "POST" ] )
 @_common.decorator_token_required
 @_common.decorator_role_required( "admin" )
```

### Comparing `esanom-3.0.1.44/esanom/routes/v3/api.py-bak1` & `esanom-3.0.2.13384/esanom/routes/v3/api.py-bak1`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/common.py` & `esanom-3.0.2.13384/esanom/routes/v3/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
             for user_match_ip_part in user_match_ip_parts:
                 if remote_ip.startswith( user_match_ip_part ) :
                     flag_user_match_ip = True
                     break
 
             if not flag_user_match_ip :
-                if _g.api[ "ip_update" ] == 0 : return( response_error( e_msg = f"{remote_ip} api ip" , e_code = 9154 , http_code = 401 ) )
+                if _g.api[ "ip_update" ] == 0 : return( response_error( e_msg = f"{_g.api['name']=} {remote_ip=} api ip" , e_code = 9154 , http_code = 401 ) )
                 _database.update_fromdict( "api" , _g.api[ "id" ] , { "ip" : f"{remote_ip}" , "ip_update" : 0 } )
 
 
         return( f( *args , **kwargs ) )
 
     return( decorator_function )
```

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/bootstrap.bundle.min.js` & `esanom-3.0.2.13384/esanom/routes/v3/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/bootstrap.min.css` & `esanom-3.0.2.13384/esanom/routes/v3/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/dashboard.css` & `esanom-3.0.2.13384/esanom/routes/v3/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/datatables.min.css` & `esanom-3.0.2.13384/esanom/routes/v3/static/datatables.min.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/datatables.min.js` & `esanom-3.0.2.13384/esanom/routes/v3/static/datatables.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/htmx.min.js` & `esanom-3.0.2.13384/esanom/routes/v3/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/plotly.min.js` & `esanom-3.0.2.13384/esanom/routes/v3/static/plotly.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/static/theme.css` & `esanom-3.0.2.13384/esanom/routes/v3/static/theme.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/admin_db_pipeline_row.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/admin_db_pipeline_row.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/admin_db_pipeline_rows.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/admin_db_pipeline_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/base.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/base.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/db_rolemodel_row.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/db_rolemodel_row.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/db_rolemodel_rows.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/db_rolemodel_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_model_io.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_model_io.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_model_io_port.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_model_io_port.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_models.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_models.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_content_pipelines.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_content_pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_debug.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_debug.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_loggedin_nav_admin.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_loggedin_nav_admin.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_head.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_head.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/inc_page_header.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/inc_page_header.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/page_dashboard_tasks.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/page_dashboard_tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/page_model.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/page_model.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_read/main.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_read/main.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/pipelines.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/dashboard/tasks.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/login/main.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/login/main.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_api_create/hx_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_api_create/hx_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_api_create/inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_api_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_port.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_port.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/read_inc_ports.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/read_inc_ports.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     <td class="text-center"><a class="link-underline-light" href="{{ url_for('.page_models_read',uid=row['uid']) }}">👁</a></td>
 
 {% elif column=="[heartbeat_last]" %}
     <td>
     {% if row[column]<20 %}
         <span class="badge bg-success text-light">ONLINE</span>
     {% else %}
-        <span class="badge bg-warning text-dark">Since {{row[column]}} seconds</span>
+        <span class="badge bg-warning text-dark">{{row["[heartbeat_last_str]"]}}</span>
     {% endif %}
     </td>
 {% else %}
     <td>{{ row[column] }}</td>
 {% endif %}
 
 {% endfor %}
```

### Comparing `esanom-3.0.1.44/esanom/routes/v3/templates/pages/register/main_inc_form.html` & `esanom-3.0.2.13384/esanom/routes/v3/templates/pages/register/main_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/routes/v3/web.py` & `esanom-3.0.2.13384/esanom/routes/v3/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,25 @@
 @ROUTES.route( "/models" , methods = [ "GET" ] )
 def page_models( ) :
 
     rolemodel_rows = _database.db_query_select_rows( "SELECT * from `rolemodel` where enable=1" )
 
     for rolemodel_row in rolemodel_rows :
         if rolemodel_row[ "heartbeat_at" ] != None :
-            rolemodel_row[ "[heartbeat_last]" ] = round( time.time( ) - rolemodel_row[ "heartbeat_at" ].timestamp( ) )
+
+            seconds = round( time.time( ) - rolemodel_row[ "heartbeat_at" ].timestamp( ) )
+
+            mm, ss = divmod(seconds, 60)
+            hh, mm = divmod(mm, 60)
+
+            heartbeat_last_str = f"{hh}h {mm}m {ss}s"
+
+            rolemodel_row[ "[heartbeat_last_str]" ] = f"{hh}h {mm}m {ss}s"
+            rolemodel_row[ "[heartbeat_last]" ] = seconds
+
         else :
             rolemodel_row[ "[heartbeat_last]" ] = 99999
 
     columns = [ "uid" , "name" , "category" , "description" , "[heartbeat_last]" ]
 
     tdata = {
         "rows" : rolemodel_rows ,
@@ -1273,15 +1283,15 @@
     if api_row is None : raise Exception( f"api_row None" )
 
 
 
     api_row["[group_names]"]=[]
     api_group_rows = _database.db_query_select_rows( "SELECT * from `api_group` WHERE api_id=%s" , [api_row['id']])
 
-    print(f"{api_group_rows=}")
+    #print(f"{api_group_rows=}")
 
     for api_group_row in api_group_rows :
         group_row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [api_group_row['group_id']])
         api_row["[group_names]"].append(group_row["name"])
 
 
     tdata = {
```

### Comparing `esanom-3.0.1.44/esanom/sample_gunicorn_config.py` & `esanom-3.0.2.13384/esanom/sample_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/sample_nom_config.json` & `esanom-3.0.2.13384/esanom/sample_nom_config.json`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/scheduler.py` & `esanom-3.0.2.13384/esanom/scheduler.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/server.py` & `esanom-3.0.2.13384/esanom/server.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/esanom/util.py` & `esanom-3.0.2.13384/esanom/util.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.1.44/PKG-INFO` & `esanom-3.0.2.13384/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanom
-Version: 3.0.1.44
+Version: 3.0.2.13384
 Summary: ESANOM
 Author: Zafar Iqbal
 Author-email: zaf@sparc.space
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

