# Comparing `tmp/esanom-3.0.2.128.tar.gz` & `tmp/esanom-3.0.3.176.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-3.0.2.128.tar", max compression
+gzip compressed data, was "esanom-3.0.3.176.tar", max compression
```

## Comparing `esanom-3.0.2.128.tar` & `esanom-3.0.3.176.tar`

### file list

```diff
@@ -1,220 +1,220 @@
--rw-r--r--   0        0        0        0 2024-04-20 13:36:28.438328 esanom-3.0.2.128/README.md
--rw-r--r--   0        0        0      144 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/CHANGELOG.txt
--rw-r--r--   0        0        0      388 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/COPYRIGHT.txt
--rw-r--r--   0        0        0    17260 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/LICENCE.txt
--rw-r--r--   0        0        0     1412 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/__init__.py
--rw-r--r--   0        0        0     6268 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/client.py
--rw-r--r--   0        0        0     5156 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/config.py
--rw-r--r--   0        0        0    47611 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/database.py
--rw-r--r--   0        0        0     1125 2024-04-20 13:36:28.922326 esanom-3.0.2.128/esanom/engine.py
--rw-r--r--   0        0        0     2496 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/monitor.py
--rw-r--r--   0        0        0    10320 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/orchestrator.py
--rw-r--r--   0        0        0    12985 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/pipeline.py
--rw-r--r--   0        0        0     1665 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/account.sql
--rw-r--r--   0        0        0     1828 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/api.sql
--rw-r--r--   0        0        0     1352 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/api_group.sql
--rw-r--r--   0        0        0     1326 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/api_role.sql
--rw-r--r--   0        0        0     1226 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/claim.sql
--rw-r--r--   0        0        0     1215 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/group.sql
--rw-r--r--   0        0        0     1828 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/io.sql
--rw-r--r--   0        0        0     1416 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/ioblock.sql
--rw-r--r--   0        0        0     1680 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/log.sql
--rw-r--r--   0        0        0     1950 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/mpin.sql
--rw-r--r--   0        0        0     1921 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/mport.sql
--rw-r--r--   0        0        0     1536 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/pin.sql
--rw-r--r--   0        0        0     1842 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/pipeline.sql
--rw-r--r--   0        0        0     1514 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/pipeline_task.sql
--rw-r--r--   0        0        0     1501 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/port.sql
--rw-r--r--   0        0        0     1388 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/port_pin.sql
--rw-r--r--   0        0        0     1126 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/role.sql
--rw-r--r--   0        0        0     1250 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/roleadmin.sql
--rw-r--r--   0        0        0     1257 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/roledashboard.sql
--rw-r--r--   0        0        0     2173 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/rolemodel.sql
--rw-r--r--   0        0        0     1655 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/roleuser.sql
--rw-r--r--   0        0        0     1319 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/schedule.sql
--rw-r--r--   0        0        0     1156 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/session.sql
--rw-r--r--   0        0        0     1236 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/system.sql
--rw-r--r--   0        0        0     1914 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/task.sql
--rw-r--r--   0        0        0     5904 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/triggers.sql
--rw-r--r--   0        0        0     1497 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/database/unit.sql
--rw-r--r--   0        0        0     1108 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/interfaces/pins.json
--rw-r--r--   0        0        0      680 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/resources/interfaces/ports.json
--rw-r--r--   0        0        0    11022 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/roleadmin.py
--rw-r--r--   0        0        0     4208 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/rolemodel.py
--rw-r--r--   0        0        0     3456 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/roleuser.py
--rw-r--r--   0        0        0      790 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/__init__.py
--rw-r--r--   0        0        0    37835 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/api.py
--rw-r--r--   0        0        0     8971 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/common.py
--rw-r--r--   0        0        0    80721 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   232803 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/bootstrap.min.css
--rw-r--r--   0        0        0      639 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/dashboard.css
--rw-r--r--   0        0        0    20832 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/routes/v3/static/datatables.min.css
--rw-r--r--   0        0        0   197654 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/routes/v3/static/datatables.min.js
--rw-r--r--   0        0        0      318 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/favicon.ico
--rw-r--r--   0        0        0    48036 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/htmx.min.js
--rw-r--r--   0        0        0       97 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/main.css
--rw-r--r--   0        0        0      422 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/main.js
--rw-r--r--   0        0        0     2362 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/nom-logo.png
--rw-r--r--   0        0        0  3620840 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/routes/v3/static/plotly.min.js
--rw-r--r--   0        0        0     1741 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/static/theme.css
--rw-r--r--   0        0        0      717 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/admin_db_pipeline_row.html
--rw-r--r--   0        0        0      627 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/admin_db_pipeline_rows.html
--rw-r--r--   0        0        0     1542 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/base.html
--rw-r--r--   0        0        0     1000 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/templates/db_rolemodel_row.html
--rw-r--r--   0        0        0      633 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/db_rolemodel_rows.html
--rw-r--r--   0        0        0      140 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/dummy.html
--rw-r--r--   0        0        0      153 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/error_404.html
--rw-r--r--   0        0        0      114 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/error_500.html
--rw-r--r--   0        0        0       82 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
--rw-r--r--   0        0        0      731 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_model_io.html
--rw-r--r--   0        0        0     1331 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_model_io_port.html
--rw-r--r--   0        0        0      808 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_models.html
--rw-r--r--   0        0        0      836 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_pipelines.html
--rw-r--r--   0        0        0     2019 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_debug.html
--rw-r--r--   0        0        0      248 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_loggedin_nav.html
--rw-r--r--   0        0        0      586 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
--rw-r--r--   0        0        0      300 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
--rw-r--r--   0        0        0      282 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_loggedin_nav_member.html
--rw-r--r--   0        0        0      182 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_footer.html
--rw-r--r--   0        0        0      628 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_head.html
--rw-r--r--   0        0        0     1332 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_header.html
--rw-r--r--   0        0        0      173 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_header_logo.html
--rw-r--r--   0        0        0      487 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_header_nav.html
--rw-r--r--   0        0        0      240 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_header_toggle.html
--rw-r--r--   0        0        0      153 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/navigation.html
--rw-r--r--   0        0        0      327 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_admin_pipelines.html
--rw-r--r--   0        0        0      921 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_dashboard_tasks.html
--rw-r--r--   0        0        0      115 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_docs.html
--rw-r--r--   0        0        0      367 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_index.html
--rw-r--r--   0        0        0      121 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_interfaces.html
--rw-r--r--   0        0        0      516 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_model.html
--rw-r--r--   0        0        0      157 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/page_models.html
--rw-r--r--   0        0        0      128 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin/main.html
--rw-r--r--   0        0        0       94 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
--rw-r--r--   0        0        0     1378 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
--rw-r--r--   0        0        0      188 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_account_create/main.html
--rw-r--r--   0        0        0        5 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
--rw-r--r--   0        0        0      110 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
--rw-r--r--   0        0        0      429 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
--rw-r--r--   0        0        0      299 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
--rw-r--r--   0        0        0      315 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/main.html
--rw-r--r--   0        0        0      272 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/read.html
--rw-r--r--   0        0        0      114 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
--rw-r--r--   0        0        0      248 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
--rw-r--r--   0        0        0      207 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/update.html
--rw-r--r--   0        0        0     1887 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
--rw-r--r--   0        0        0      113 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
--rw-r--r--   0        0        0      544 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_read/main.html
--rw-r--r--   0        0        0        6 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
--rw-r--r--   0        0        0     1221 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
--rw-r--r--   0        0        0      474 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
--rw-r--r--   0        0        0      256 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_update/main.html
--rw-r--r--   0        0        0      421 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
--rw-r--r--   0        0        0      369 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
--rw-r--r--   0        0        0      240 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_apis/main.html
--rw-r--r--   0        0        0       94 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
--rw-r--r--   0        0        0      324 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
--rw-r--r--   0        0        0      263 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_create/main.html
--rw-r--r--   0        0        0      111 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
--rw-r--r--   0        0        0      278 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_read/main.html
--rw-r--r--   0        0        0        6 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
--rw-r--r--   0        0        0      718 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
--rw-r--r--   0        0        0      352 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_update/main.html
--rw-r--r--   0        0        0       87 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
--rw-r--r--   0        0        0      425 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_groups/main.html
--rw-r--r--   0        0        0      111 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
--rw-r--r--   0        0        0      332 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_read/main.html
--rw-r--r--   0        0        0       24 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
--rw-r--r--   0        0        0      897 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
--rw-r--r--   0        0        0      403 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_update/main.html
--rw-r--r--   0        0        0      425 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_models/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
--rw-r--r--   0        0        0      245 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_models/main.html
--rw-r--r--   0        0        0       40 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
--rw-r--r--   0        0        0      307 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/inc_form_pins.html
--rw-r--r--   0        0        0      311 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/inc_form_ports.html
--rw-r--r--   0        0        0      413 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
--rw-r--r--   0        0        0      463 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
--rw-r--r--   0        0        0      380 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_settings/main.html
--rw-r--r--   0        0        0       82 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
--rw-r--r--   0        0        0       82 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
--rw-r--r--   0        0        0      118 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/main.html
--rw-r--r--   0        0        0      895 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/pipelines.html
--rw-r--r--   0        0        0      891 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/tasks.html
--rw-r--r--   0        0        0      640 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
--rw-r--r--   0        0        0     1218 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
--rw-r--r--   0        0        0       26 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
--rw-r--r--   0        0        0      770 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
--rw-r--r--   0        0        0      128 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/main.html
--rw-r--r--   0        0        0       60 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/login/hx_login.html
--rw-r--r--   0        0        0      766 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/login/main.html
--rw-r--r--   0        0        0      133 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/logout/main.html
--rw-r--r--   0        0        0      128 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member/main.html
--rw-r--r--   0        0        0      617 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
--rw-r--r--   0        0        0      789 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
--rw-r--r--   0        0        0      182 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_api_create/main.html
--rw-r--r--   0        0        0      347 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
--rw-r--r--   0        0        0      423 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/inc_table.html
--rw-r--r--   0        0        0      367 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
--rw-r--r--   0        0        0      416 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/main.html
--rw-r--r--   0        0        0      256 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/read.html
--rw-r--r--   0        0        0      129 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/update.html
--rw-r--r--   0        0        0      637 2024-04-20 13:36:28.934326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
--rw-r--r--   0        0        0      347 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
--rw-r--r--   0        0        0      442 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/inc_table.html
--rw-r--r--   0        0        0      163 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
--rw-r--r--   0        0        0      241 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/main.html
--rw-r--r--   0        0        0      256 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/read.html
--rw-r--r--   0        0        0      129 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/update.html
--rw-r--r--   0        0        0      637 2024-04-20 13:36:28.942326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
--rw-r--r--   0        0        0      428 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read.html
--rw-r--r--   0        0        0      160 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read_inc_info.html
--rw-r--r--   0        0        0     1331 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read_inc_port.html
--rw-r--r--   0        0        0      733 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read_inc_ports.html
--rw-r--r--   0        0        0      238 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/rows.html
--rw-r--r--   0        0        0      424 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/rows_inc_table.html
--rw-r--r--   0        0        0      609 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
--rw-r--r--   0        0        0      322 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/read.html
--rw-r--r--   0        0        0       92 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/read_inc_info.html
--rw-r--r--   0        0        0      174 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
--rw-r--r--   0        0        0      130 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
--rw-r--r--   0        0        0      432 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
--rw-r--r--   0        0        0      234 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/rows.html
--rw-r--r--   0        0        0      420 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
--rw-r--r--   0        0        0      339 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/read.html
--rw-r--r--   0        0        0       92 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/read_inc_info.html
--rw-r--r--   0        0        0      422 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/read_inc_table.html
--rw-r--r--   0        0        0      309 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
--rw-r--r--   0        0        0      125 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
--rw-r--r--   0        0        0      236 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/rows.html
--rw-r--r--   0        0        0      422 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
--rw-r--r--   0        0        0      340 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-20 13:36:28.938326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
--rw-r--r--   0        0        0      265 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/register/hx_form.html
--rw-r--r--   0        0        0      455 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/register/main.html
--rw-r--r--   0        0        0     1037 2024-04-20 13:36:28.930326 esanom-3.0.2.128/esanom/routes/v3/templates/pages/register/main_inc_form.html
--rw-r--r--   0        0        0    54155 2024-04-20 13:36:28.926326 esanom-3.0.2.128/esanom/routes/v3/web.py
--rw-r--r--   0        0        0     1693 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/sample_gunicorn_config.py
--rw-r--r--   0        0        0      753 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/sample_nom_config.json
--rw-r--r--   0        0        0     5050 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/scheduler.py
--rw-r--r--   0        0        0     3698 2024-04-20 13:36:28.946326 esanom-3.0.2.128/esanom/server.py
--rw-r--r--   0        0        0    12199 2024-04-20 13:36:28.958325 esanom-3.0.2.128/esanom/util.py
--rw-r--r--   0        0        0      443 2024-04-20 13:36:31.398316 esanom-3.0.2.128/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 esanom-3.0.2.128/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 15:45:35.859521 esanom-3.0.3.176/README.md
+-rw-r--r--   0        0        0      144 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/CHANGELOG.txt
+-rw-r--r--   0        0        0      388 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/COPYRIGHT.txt
+-rw-r--r--   0        0        0    17260 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/LICENCE.txt
+-rw-r--r--   0        0        0     1412 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/__init__.py
+-rw-r--r--   0        0        0     6268 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/client.py
+-rw-r--r--   0        0        0     5156 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/config.py
+-rw-r--r--   0        0        0    47611 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/database.py
+-rw-r--r--   0        0        0     1125 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/engine.py
+-rw-r--r--   0        0        0     2496 2024-04-20 15:45:36.267520 esanom-3.0.3.176/esanom/monitor.py
+-rw-r--r--   0        0        0    10320 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/orchestrator.py
+-rw-r--r--   0        0        0    12985 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/pipeline.py
+-rw-r--r--   0        0        0     1665 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/account.sql
+-rw-r--r--   0        0        0     1828 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/api.sql
+-rw-r--r--   0        0        0     1352 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/api_group.sql
+-rw-r--r--   0        0        0     1326 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/api_role.sql
+-rw-r--r--   0        0        0     1226 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/claim.sql
+-rw-r--r--   0        0        0     1215 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/group.sql
+-rw-r--r--   0        0        0     1828 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/io.sql
+-rw-r--r--   0        0        0     1416 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/ioblock.sql
+-rw-r--r--   0        0        0     1680 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/log.sql
+-rw-r--r--   0        0        0     1950 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/mpin.sql
+-rw-r--r--   0        0        0     1921 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/mport.sql
+-rw-r--r--   0        0        0     1536 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/pin.sql
+-rw-r--r--   0        0        0     1842 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/pipeline.sql
+-rw-r--r--   0        0        0     1514 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/pipeline_task.sql
+-rw-r--r--   0        0        0     1501 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/port.sql
+-rw-r--r--   0        0        0     1388 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/port_pin.sql
+-rw-r--r--   0        0        0     1126 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/role.sql
+-rw-r--r--   0        0        0     1250 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/roleadmin.sql
+-rw-r--r--   0        0        0     1257 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/roledashboard.sql
+-rw-r--r--   0        0        0     2173 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/rolemodel.sql
+-rw-r--r--   0        0        0     1655 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/roleuser.sql
+-rw-r--r--   0        0        0     1319 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/schedule.sql
+-rw-r--r--   0        0        0     1156 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/session.sql
+-rw-r--r--   0        0        0     1236 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/system.sql
+-rw-r--r--   0        0        0     1914 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/task.sql
+-rw-r--r--   0        0        0     5904 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/triggers.sql
+-rw-r--r--   0        0        0     1497 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/database/unit.sql
+-rw-r--r--   0        0        0     1049 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/interfaces/pins.json
+-rw-r--r--   0        0        0      667 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/resources/interfaces/ports.json
+-rw-r--r--   0        0        0    11022 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/roleadmin.py
+-rw-r--r--   0        0        0     4208 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/rolemodel.py
+-rw-r--r--   0        0        0     3456 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/roleuser.py
+-rw-r--r--   0        0        0      790 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/__init__.py
+-rw-r--r--   0        0        0    37835 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/api.py
+-rw-r--r--   0        0        0     8971 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/common.py
+-rw-r--r--   0        0        0    80721 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   232803 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/bootstrap.min.css
+-rw-r--r--   0        0        0      639 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/dashboard.css
+-rw-r--r--   0        0        0    20832 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/routes/v3/static/datatables.min.css
+-rw-r--r--   0        0        0   197654 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/routes/v3/static/datatables.min.js
+-rw-r--r--   0        0        0      318 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/favicon.ico
+-rw-r--r--   0        0        0    48036 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/htmx.min.js
+-rw-r--r--   0        0        0       97 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/main.css
+-rw-r--r--   0        0        0      422 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/main.js
+-rw-r--r--   0        0        0     2362 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/nom-logo.png
+-rw-r--r--   0        0        0  3620840 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/routes/v3/static/plotly.min.js
+-rw-r--r--   0        0        0     1741 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/static/theme.css
+-rw-r--r--   0        0        0      717 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/admin_db_pipeline_row.html
+-rw-r--r--   0        0        0      627 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/admin_db_pipeline_rows.html
+-rw-r--r--   0        0        0     1542 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/base.html
+-rw-r--r--   0        0        0     1000 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/db_rolemodel_row.html
+-rw-r--r--   0        0        0      633 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/db_rolemodel_rows.html
+-rw-r--r--   0        0        0      140 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/dummy.html
+-rw-r--r--   0        0        0      153 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/error_404.html
+-rw-r--r--   0        0        0      114 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/error_500.html
+-rw-r--r--   0        0        0       82 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
+-rw-r--r--   0        0        0      731 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_model_io.html
+-rw-r--r--   0        0        0     1331 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_model_io_port.html
+-rw-r--r--   0        0        0      808 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_models.html
+-rw-r--r--   0        0        0      836 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_pipelines.html
+-rw-r--r--   0        0        0     2019 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_debug.html
+-rw-r--r--   0        0        0      248 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_loggedin_nav.html
+-rw-r--r--   0        0        0      586 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
+-rw-r--r--   0        0        0      300 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
+-rw-r--r--   0        0        0      282 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_loggedin_nav_member.html
+-rw-r--r--   0        0        0      182 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_footer.html
+-rw-r--r--   0        0        0      628 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_head.html
+-rw-r--r--   0        0        0     1332 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_header.html
+-rw-r--r--   0        0        0      173 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_header_logo.html
+-rw-r--r--   0        0        0      495 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_header_nav.html
+-rw-r--r--   0        0        0      240 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_header_toggle.html
+-rw-r--r--   0        0        0      153 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/navigation.html
+-rw-r--r--   0        0        0      327 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/page_admin_pipelines.html
+-rw-r--r--   0        0        0      921 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/page_dashboard_tasks.html
+-rw-r--r--   0        0        0      115 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/page_docs.html
+-rw-r--r--   0        0        0      367 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/page_index.html
+-rw-r--r--   0        0        0      121 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/templates/page_interfaces.html
+-rw-r--r--   0        0        0      516 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/page_model.html
+-rw-r--r--   0        0        0      157 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/page_models.html
+-rw-r--r--   0        0        0      128 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin/main.html
+-rw-r--r--   0        0        0       94 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
+-rw-r--r--   0        0        0     1378 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
+-rw-r--r--   0        0        0      188 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_account_create/main.html
+-rw-r--r--   0        0        0        5 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
+-rw-r--r--   0        0        0      110 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
+-rw-r--r--   0        0        0      429 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
+-rw-r--r--   0        0        0      299 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
+-rw-r--r--   0        0        0      315 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/main.html
+-rw-r--r--   0        0        0      272 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/read.html
+-rw-r--r--   0        0        0      114 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
+-rw-r--r--   0        0        0      248 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
+-rw-r--r--   0        0        0      207 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/update.html
+-rw-r--r--   0        0        0     1887 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
+-rw-r--r--   0        0        0      113 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
+-rw-r--r--   0        0        0      544 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
+-rw-r--r--   0        0        0     1221 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
+-rw-r--r--   0        0        0      474 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
+-rw-r--r--   0        0        0      256 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_update/main.html
+-rw-r--r--   0        0        0      421 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
+-rw-r--r--   0        0        0      369 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
+-rw-r--r--   0        0        0      240 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_apis/main.html
+-rw-r--r--   0        0        0       94 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
+-rw-r--r--   0        0        0      324 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
+-rw-r--r--   0        0        0      263 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_create/main.html
+-rw-r--r--   0        0        0      111 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
+-rw-r--r--   0        0        0      278 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
+-rw-r--r--   0        0        0      718 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
+-rw-r--r--   0        0        0      352 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_update/main.html
+-rw-r--r--   0        0        0       87 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
+-rw-r--r--   0        0        0      425 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_groups/main.html
+-rw-r--r--   0        0        0      111 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
+-rw-r--r--   0        0        0      332 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_read/main.html
+-rw-r--r--   0        0        0       24 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
+-rw-r--r--   0        0        0      897 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
+-rw-r--r--   0        0        0      403 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_update/main.html
+-rw-r--r--   0        0        0      425 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_models/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
+-rw-r--r--   0        0        0      245 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_models/main.html
+-rw-r--r--   0        0        0       40 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
+-rw-r--r--   0        0        0      307 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/inc_form_pins.html
+-rw-r--r--   0        0        0      311 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/inc_form_ports.html
+-rw-r--r--   0        0        0      413 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
+-rw-r--r--   0        0        0      463 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
+-rw-r--r--   0        0        0      380 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_settings/main.html
+-rw-r--r--   0        0        0       82 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
+-rw-r--r--   0        0        0       82 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
+-rw-r--r--   0        0        0      118 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/main.html
+-rw-r--r--   0        0        0      895 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/pipelines.html
+-rw-r--r--   0        0        0      891 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/tasks.html
+-rw-r--r--   0        0        0      640 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
+-rw-r--r--   0        0        0     1218 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
+-rw-r--r--   0        0        0       26 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
+-rw-r--r--   0        0        0      770 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
+-rw-r--r--   0        0        0      128 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/main.html
+-rw-r--r--   0        0        0       60 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/login/hx_login.html
+-rw-r--r--   0        0        0      766 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/login/main.html
+-rw-r--r--   0        0        0      133 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/logout/main.html
+-rw-r--r--   0        0        0      128 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member/main.html
+-rw-r--r--   0        0        0      617 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
+-rw-r--r--   0        0        0      789 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
+-rw-r--r--   0        0        0      182 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_api_create/main.html
+-rw-r--r--   0        0        0      347 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
+-rw-r--r--   0        0        0      423 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/inc_table.html
+-rw-r--r--   0        0        0      367 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
+-rw-r--r--   0        0        0      416 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/main.html
+-rw-r--r--   0        0        0      256 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/read.html
+-rw-r--r--   0        0        0      129 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/update.html
+-rw-r--r--   0        0        0      637 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
+-rw-r--r--   0        0        0      347 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
+-rw-r--r--   0        0        0      442 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/inc_table.html
+-rw-r--r--   0        0        0      163 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
+-rw-r--r--   0        0        0      241 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/main.html
+-rw-r--r--   0        0        0      256 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/read.html
+-rw-r--r--   0        0        0      129 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/update.html
+-rw-r--r--   0        0        0      637 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
+-rw-r--r--   0        0        0      428 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read.html
+-rw-r--r--   0        0        0      160 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read_inc_info.html
+-rw-r--r--   0        0        0     1331 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read_inc_port.html
+-rw-r--r--   0        0        0      733 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read_inc_ports.html
+-rw-r--r--   0        0        0      238 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/rows.html
+-rw-r--r--   0        0        0      424 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/rows_inc_table.html
+-rw-r--r--   0        0        0      609 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 15:45:36.279520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
+-rw-r--r--   0        0        0      322 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/read.html
+-rw-r--r--   0        0        0       92 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/read_inc_info.html
+-rw-r--r--   0        0        0      174 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
+-rw-r--r--   0        0        0      130 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
+-rw-r--r--   0        0        0      432 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
+-rw-r--r--   0        0        0      234 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/rows.html
+-rw-r--r--   0        0        0      420 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
+-rw-r--r--   0        0        0      339 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/read.html
+-rw-r--r--   0        0        0       92 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/read_inc_info.html
+-rw-r--r--   0        0        0      422 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/read_inc_table.html
+-rw-r--r--   0        0        0      309 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
+-rw-r--r--   0        0        0      125 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
+-rw-r--r--   0        0        0      236 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/rows.html
+-rw-r--r--   0        0        0      422 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
+-rw-r--r--   0        0        0      340 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-20 15:45:36.283520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
+-rw-r--r--   0        0        0      265 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/register/hx_form.html
+-rw-r--r--   0        0        0      455 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/register/main.html
+-rw-r--r--   0        0        0     1037 2024-04-20 15:45:36.275520 esanom-3.0.3.176/esanom/routes/v3/templates/pages/register/main_inc_form.html
+-rw-r--r--   0        0        0    54155 2024-04-20 15:45:36.271520 esanom-3.0.3.176/esanom/routes/v3/web.py
+-rw-r--r--   0        0        0     1693 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/sample_gunicorn_config.py
+-rw-r--r--   0        0        0      753 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/sample_nom_config.json
+-rw-r--r--   0        0        0     5050 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/scheduler.py
+-rw-r--r--   0        0        0     3698 2024-04-20 15:45:36.287520 esanom-3.0.3.176/esanom/server.py
+-rw-r--r--   0        0        0    12199 2024-04-20 15:45:36.299520 esanom-3.0.3.176/esanom/util.py
+-rw-r--r--   0        0        0      443 2024-04-20 15:46:57.327410 esanom-3.0.3.176/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 esanom-3.0.3.176/PKG-INFO
```

### Comparing `esanom-3.0.2.128/esanom/LICENCE.txt` & `esanom-3.0.3.176/esanom/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/__init__.py` & `esanom-3.0.3.176/esanom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # This file is subject to the terms and conditions defined in file 'LICENCE.txt', 
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 #####################################################################
 
 from importlib.metadata import version
 
 print( f"NoM v{version('esanom')} Copyright 2024 © European Space Agency. All rights reserved." )
```

### Comparing `esanom-3.0.2.128/esanom/client.py` & `esanom-3.0.3.176/esanom/client.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/config.py` & `esanom-3.0.3.176/esanom/config.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/database.py` & `esanom-3.0.3.176/esanom/database.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/engine.py` & `esanom-3.0.3.176/esanom/engine.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/monitor.py` & `esanom-3.0.3.176/esanom/monitor.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/orchestrator.py` & `esanom-3.0.3.176/esanom/orchestrator.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/pipeline.py` & `esanom-3.0.3.176/esanom/pipeline.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/account.sql` & `esanom-3.0.3.176/esanom/resources/database/account.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/api.sql` & `esanom-3.0.3.176/esanom/resources/database/api.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/api_group.sql` & `esanom-3.0.3.176/esanom/resources/database/api_group.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/api_role.sql` & `esanom-3.0.3.176/esanom/resources/database/api_role.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/claim.sql` & `esanom-3.0.3.176/esanom/resources/database/claim.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/group.sql` & `esanom-3.0.3.176/esanom/resources/database/group.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/io.sql` & `esanom-3.0.3.176/esanom/resources/database/io.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/ioblock.sql` & `esanom-3.0.3.176/esanom/resources/database/ioblock.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/log.sql` & `esanom-3.0.3.176/esanom/resources/database/log.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/mpin.sql` & `esanom-3.0.3.176/esanom/resources/database/mpin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/mport.sql` & `esanom-3.0.3.176/esanom/resources/database/mport.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/pin.sql` & `esanom-3.0.3.176/esanom/resources/database/pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/pipeline.sql` & `esanom-3.0.3.176/esanom/resources/database/pipeline.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/pipeline_task.sql` & `esanom-3.0.3.176/esanom/resources/database/pipeline_task.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/port.sql` & `esanom-3.0.3.176/esanom/resources/database/port.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/port_pin.sql` & `esanom-3.0.3.176/esanom/resources/database/port_pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/role.sql` & `esanom-3.0.3.176/esanom/resources/database/role.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/roleadmin.sql` & `esanom-3.0.3.176/esanom/resources/database/roleadmin.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/roledashboard.sql` & `esanom-3.0.3.176/esanom/resources/database/roledashboard.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/rolemodel.sql` & `esanom-3.0.3.176/esanom/resources/database/rolemodel.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/roleuser.sql` & `esanom-3.0.3.176/esanom/resources/database/roleuser.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/schedule.sql` & `esanom-3.0.3.176/esanom/resources/database/schedule.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/session.sql` & `esanom-3.0.3.176/esanom/resources/database/session.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/system.sql` & `esanom-3.0.3.176/esanom/resources/database/system.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/task.sql` & `esanom-3.0.3.176/esanom/resources/database/task.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/triggers.sql` & `esanom-3.0.3.176/esanom/resources/database/triggers.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/database/unit.sql` & `esanom-3.0.3.176/esanom/resources/database/unit.sql`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/resources/interfaces/pins.json` & `esanom-3.0.3.176/esanom/resources/interfaces/pins.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {'delete': "['zs']"}*

```diff
@@ -90,15 +90,9 @@
         }
     },
     "ys": {
         "type": "list",
         "units": {
             "u": {}
         }
-    },
-    "zs": {
-        "type": "list",
-        "units": {
-            "u": {}
-        }
     }
 }
```

### Comparing `esanom-3.0.2.128/esanom/resources/interfaces/ports.json` & `esanom-3.0.3.176/esanom/resources/interfaces/ports.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407407%*

 * *Differences: {"'points'": "{'pins': {delete: ['zs']}}"}*

```diff
@@ -25,16 +25,15 @@
             "subject": {},
             "to": {}
         }
     },
     "points": {
         "pins": {
             "xs": {},
-            "ys": {},
-            "zs": {}
+            "ys": {}
         }
     },
     "trajectory": {
         "pins": {
             "fp_json": {}
         }
     },
```

### Comparing `esanom-3.0.2.128/esanom/roleadmin.py` & `esanom-3.0.3.176/esanom/roleadmin.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/rolemodel.py` & `esanom-3.0.3.176/esanom/rolemodel.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/roleuser.py` & `esanom-3.0.3.176/esanom/roleuser.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/__init__.py` & `esanom-3.0.3.176/esanom/routes/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/api.py` & `esanom-3.0.3.176/esanom/routes/v3/api.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/common.py` & `esanom-3.0.3.176/esanom/routes/v3/common.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/bootstrap.bundle.min.js` & `esanom-3.0.3.176/esanom/routes/v3/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/bootstrap.min.css` & `esanom-3.0.3.176/esanom/routes/v3/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/dashboard.css` & `esanom-3.0.3.176/esanom/routes/v3/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/datatables.min.css` & `esanom-3.0.3.176/esanom/routes/v3/static/datatables.min.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/datatables.min.js` & `esanom-3.0.3.176/esanom/routes/v3/static/datatables.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/htmx.min.js` & `esanom-3.0.3.176/esanom/routes/v3/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/nom-logo.png` & `esanom-3.0.3.176/esanom/routes/v3/static/nom-logo.png`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/plotly.min.js` & `esanom-3.0.3.176/esanom/routes/v3/static/plotly.min.js`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/static/theme.css` & `esanom-3.0.3.176/esanom/routes/v3/static/theme.css`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/admin_db_pipeline_row.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/admin_db_pipeline_row.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/admin_db_pipeline_rows.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/admin_db_pipeline_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/base.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/base.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/db_rolemodel_row.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/db_rolemodel_row.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/db_rolemodel_rows.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/db_rolemodel_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_model_io.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_model_io.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_model_io_port.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_model_io_port.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_models.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_models.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_content_pipelines.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_content_pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_debug.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_debug.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_loggedin_nav_admin.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_loggedin_nav_admin.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_head.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_head.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/inc_page_header.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/inc_page_header.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/page_dashboard_tasks.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/page_dashboard_tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/page_model.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/page_model.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_read/main.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_read/main.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/pipelines.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/dashboard/tasks.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/login/main.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/login/main.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_api_create/hx_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_api_create/hx_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_api_create/inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_api_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read_inc_port.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read_inc_port.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/read_inc_ports.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/read_inc_ports.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/templates/pages/register/main_inc_form.html` & `esanom-3.0.3.176/esanom/routes/v3/templates/pages/register/main_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/routes/v3/web.py` & `esanom-3.0.3.176/esanom/routes/v3/web.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/sample_gunicorn_config.py` & `esanom-3.0.3.176/esanom/sample_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/sample_nom_config.json` & `esanom-3.0.3.176/esanom/sample_nom_config.json`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/scheduler.py` & `esanom-3.0.3.176/esanom/scheduler.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/server.py` & `esanom-3.0.3.176/esanom/server.py`

 * *Files identical despite different names*

### Comparing `esanom-3.0.2.128/esanom/util.py` & `esanom-3.0.3.176/esanom/util.py`

 * *Files identical despite different names*

