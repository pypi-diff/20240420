# Comparing `tmp/openbb_nightly-4.1.6.dev202404190009.tar.gz` & `tmp/openbb_nightly-4.1.6.dev202404200009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.6.dev202404190009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.6.dev202404200009.tar", max compression
```

## Comparing `openbb_nightly-4.1.6.dev202404190009.tar` & `openbb_nightly-4.1.6.dev202404200009.tar`

### file list

```diff
@@ -1,772 +1,775 @@
--rw-r--r--   0        0        0     6818 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/README.md
--rw-r--r--   0        0        0       19 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    18495 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1035 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      856 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/custom_parameter.py
--rw-r--r--   0        0        0      502 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1912 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/fast_api_settings.py
--rw-r--r--   0        0        0      694 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     8569 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1418 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0       37 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     3898 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21268 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-19 00:09:03.156187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10402 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3484 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1685 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    65186 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2224 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8142 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0      630 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1288 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     1591 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1750 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      888 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-19 00:09:03.160187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-19 00:09:03.164187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9681 2024-04-19 00:09:03.168187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.168187 openbb_nightly-4.1.6.dev202404190009/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-19 00:09:03.172187 openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9797 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-04-19 00:09:03.176187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.180187 openbb_nightly-4.1.6.dev202404190009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16765 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    57462 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0    19856 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-19 00:09:03.184187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    38235 2024-04-19 00:09:03.188187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.188187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-19 00:09:03.188187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-04-19 00:09:03.204187 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-04-19 00:09:03.228188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    25617 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3339 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0     1440 2024-04-19 00:09:03.232188 openbb_nightly-4.1.6.dev202404190009/openbb/__init__.py
--rw-r--r--   0        0        0  1190613 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2794 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6589 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11777 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/currency.py
--rw-r--r--   0        0        0     6481 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12160 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    53509 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/economy.py
--rw-r--r--   0        0        0    12686 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27675 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity.py
--rw-r--r--   0        0        0    18754 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2870 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    26107 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    40891 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   169108 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30694 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26819 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3567 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75740 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/etf.py
--rw-r--r--   0        0        0     4649 2024-04-19 00:09:03.236188 openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    20027 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7155 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26900 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    11204 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11927 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/index.py
--rw-r--r--   0        0        0    15535 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/regulators.py
--rw-r--r--   0        0        0    16573 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    17884 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9745 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-04-19 00:09:03.240188 openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-04-19 00:09:03.244188 openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-19 00:09:03.252188 openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      716 2024-04-19 00:09:03.300189 openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-19 00:09:03.300189 openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-19 00:09:03.300189 openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-19 00:09:03.300189 openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-04-19 00:09:03.304189 openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-19 00:09:03.308189 openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-19 00:09:03.308189 openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-19 00:09:03.308189 openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-04-19 00:09:03.308189 openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.364189 openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5202 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6768 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3521 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.368189 openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-19 00:09:03.392190 openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5269 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-19 00:09:03.396190 openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7321 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8829 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-19 00:09:03.400190 openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-19 00:09:03.412190 openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-04-19 00:09:03.416190 openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2100 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-19 00:09:03.420190 openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8328 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2615 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13896 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7434 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.436190 openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-04-19 00:09:03.528191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-19 00:09:03.532191 openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5162 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8843 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12451 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-19 00:09:03.540191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10325 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-04-19 00:09:03.544191 openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10264 2024-04-19 00:09:03.640193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.644193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-04-19 00:09:03.644193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-19 00:09:03.644193 openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4606 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4232 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1978 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5858 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10040 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-19 00:09:03.648193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-04-19 00:09:03.652193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-19 00:09:03.652193 openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     6884 2024-04-19 00:09:15.252312 openbb_nightly-4.1.6.dev202404190009/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404190009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/README.md
+-rw-r--r--   0        0        0       19 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.059865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    18672 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9094 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21268 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10402 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1685 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    65939 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2224 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8142 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-20 00:09:01.063865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0      630 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1288 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     1591 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1750 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      888 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-20 00:09:01.067865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3083 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.071865 openbb_nightly-4.1.6.dev202404200009/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-04-20 00:09:01.075865 openbb_nightly-4.1.6.dev202404200009/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-20 00:09:01.075865 openbb_nightly-4.1.6.dev202404200009/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-04-20 00:09:01.075865 openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-20 00:09:01.075865 openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-04-20 00:09:01.075865 openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-04-20 00:09:01.079865 openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0     9797 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-20 00:09:01.083865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-20 00:09:01.087865 openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    64220 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    19856 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-20 00:09:01.091865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-20 00:09:01.107865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-04-20 00:09:01.107865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-20 00:09:01.107865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-04-20 00:09:01.107865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-04-20 00:09:01.111865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-04-20 00:09:01.111865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-04-20 00:09:01.111865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-04-20 00:09:01.131865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-04-20 00:09:01.135865 openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0     1440 2024-04-20 00:09:01.139865 openbb_nightly-4.1.6.dev202404200009/openbb/__init__.py
+-rw-r--r--   0        0        0  1190613 2024-04-20 00:09:01.139865 openbb_nightly-4.1.6.dev202404200009/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2794 2024-04-20 00:09:01.139865 openbb_nightly-4.1.6.dev202404200009/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-20 00:09:01.139865 openbb_nightly-4.1.6.dev202404200009/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3299 2024-04-20 00:09:01.139865 openbb_nightly-4.1.6.dev202404200009/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6468 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    11706 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/currency.py
+-rw-r--r--   0        0        0     6360 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12047 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    52383 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27548 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2807 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    40717 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   167585 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30431 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26606 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3504 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75407 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19470 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7001 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11744 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/index.py
+-rw-r--r--   0        0        0    15304 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16380 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-20 00:09:01.143865 openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    17979 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9801 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-20 00:09:01.147865 openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-20 00:09:01.151865 openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-20 00:09:01.155865 openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      716 2024-04-20 00:09:01.203865 openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-20 00:09:01.203865 openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-20 00:09:01.203865 openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-04-20 00:09:01.203865 openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-04-20 00:09:01.211865 openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-20 00:09:01.211865 openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-20 00:09:01.211865 openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-20 00:09:01.211865 openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-04-20 00:09:01.211865 openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.267865 openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6076 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5308 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6768 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-20 00:09:01.271865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3521 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.275865 openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-20 00:09:01.295865 openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5269 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-20 00:09:01.299865 openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7321 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2550 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-20 00:09:01.303865 openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5109 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-20 00:09:01.315865 openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2100 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6283 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6255 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7150 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6142 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-20 00:09:01.323865 openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8328 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2615 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13896 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7434 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.339865 openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-20 00:09:01.431865 openbb_nightly-4.1.6.dev202404200009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-20 00:09:01.435865 openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-20 00:09:01.443865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-20 00:09:01.443865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-20 00:09:01.443865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-20 00:09:01.443865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-04-20 00:09:01.443865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10325 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-20 00:09:01.447865 openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6582 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9222 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-20 00:09:01.543865 openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-04-20 00:09:01.547865 openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4606 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4232 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     1978 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5858 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10102 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-20 00:09:01.551865 openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     6884 2024-04-20 00:09:10.619837 openbb_nightly-4.1.6.dev202404200009/pyproject.toml
+-rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404200009/PKG-INFO
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/README.md` & `openbb_nightly-4.1.6.dev202404200009/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/command_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,23 +312,26 @@
         extra_params = kwargs.get("extra_params", {})
 
         if hasattr(extra_params, "__dict__") and hasattr(extra_params, "chart_params"):
             chart_params = kwargs["extra_params"].__dict__.get("chart_params", {})
         elif isinstance(extra_params, dict) and "chart_params" in extra_params:
             chart_params = kwargs["extra_params"].get("chart_params", {})
 
-        if "chart_params" in kwargs:
+        if "chart_params" in kwargs and kwargs["chart_params"] is not None:
             chart_params.update(kwargs.pop("chart_params", {}))
 
-        if "kwargs" in kwargs:
+        if (
+            "kwargs" in kwargs
+            and "chart_params" in kwargs["kwargs"]
+            and kwargs["kwargs"].get("chart_params") is not None
+        ):
             chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
 
         if chart_params:
             kwargs.update(chart_params)
-
         obbject.charting.show(render=False, **kwargs)
 
     # pylint: disable=R0913, R0914
     @classmethod
     async def _execute_func(
         cls,
         route: str,
@@ -370,15 +373,14 @@
             } or None
 
             try:
                 obbject = await cls._command(func, kwargs)
                 # pylint: disable=protected-access
                 obbject._route = route
                 obbject._standard_params = kwargs.get("standard_params", None)
-
                 if chart and obbject.results:
                     cls._chart(obbject, **kwargs)
 
             except Exception as e:
                 raise OpenBBError(e) from e
             finally:
                 ls = LoggingService(system_settings, user_settings)
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/fast_api_settings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/api_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     model_config = ConfigDict(frozen=True)
 
     url: str = "http://localhost:8000"
     description: str = "Local OpenBB development server"
 
 
-class FastAPISettings(BaseModel):
+class APISettings(BaseModel):
     """Settings model for FastAPI configuration."""
 
     model_config = ConfigDict(frozen=True)
 
     version: str = "1"
     title: str = "OpenBB Platform API"
     description: str = "This is the OpenBB Platform API."
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/obbject.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,14 +239,32 @@
         ):
             df = df.T
         results = df.to_dict(orient=orient)
         if isinstance(results, dict) and orient == "list" and "index" in results:
             del results["index"]
         return results
 
+    def to_llm(self) -> Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]:
+        """Convert results field to an LLM compatible output.
+
+        Returns
+        -------
+        Union[Dict[Hashable, Any], List[Dict[Hashable, Any]]]
+            Dictionary of lists or list of dictionaries if orient is "records".
+        """
+        df = self.to_dataframe(index=None)
+
+        results = df.to_json(
+            orient="records",
+            date_format="iso",
+            date_unit="s",
+        )
+
+        return results
+
     def show(self, **kwargs: Any) -> None:
         """Display chart."""
         # pylint: disable=no-member
         if not self.chart or not self.chart.fig:
             raise OpenBBError("Chart not found.")
         show_function: Callable = getattr(self.chart.fig, "show")
         show_function(**kwargs)
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/preferences.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 
 from pydantic import BaseModel, ConfigDict, Field, PositiveInt
 
 
 class Preferences(BaseModel):
     """Preferences for the OpenBB platform."""
 
-    data_directory: str = str(Path.home() / "OpenBBUserData")
-    export_directory: str = str(Path.home() / "OpenBBUserData" / "exports")
-    user_styles_directory: str = str(Path.home() / "OpenBBUserData" / "styles" / "user")
     cache_directory: str = str(Path.home() / "OpenBBUserData" / "cache")
     chart_style: Literal["dark", "light"] = "dark"
+    data_directory: str = str(Path.home() / "OpenBBUserData")
+    export_directory: str = str(Path.home() / "OpenBBUserData" / "exports")
+    metadata: bool = True
+    output_type: Literal[
+        "OBBject", "dataframe", "polars", "numpy", "dict", "chart", "llm"
+    ] = Field(
+        default="OBBject",
+        description="Python default output type.",
+        validate_default=True,
+    )
     plot_enable_pywry: bool = True
-    plot_pywry_width: PositiveInt = 1400
-    plot_pywry_height: PositiveInt = 762
     plot_open_export: bool = (
         False  # Whether to open plot image exports after they are created
     )
-    table_style: Literal["dark", "light"] = "dark"
+    plot_pywry_height: PositiveInt = 762
+    plot_pywry_width: PositiveInt = 1400
     request_timeout: PositiveInt = 15
-    metadata: bool = True
-    output_type: Literal["OBBject", "dataframe", "polars", "numpy", "dict", "chart"] = (
-        Field(default="OBBject", description="Python default output type.")
-    )
     show_warnings: bool = True
+    table_style: Literal["dark", "light"] = "dark"
+    user_styles_directory: str = str(Path.home() / "OpenBBUserData" / "styles" / "user")
 
     model_config = ConfigDict(validate_assignment=True)
 
     def __repr__(self) -> str:
         """Return a string representation of the model."""
         return f"{self.__class__.__name__}\n\n" + "\n".join(
             f"{k}: {v}" for k, v in self.model_dump().items()
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/system_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from openbb_core.app.constants import (
     HOME_DIRECTORY,
     OPENBB_DIRECTORY,
     SYSTEM_SETTINGS_PATH,
     USER_SETTINGS_PATH,
 )
 from openbb_core.app.model.abstract.tagged import Tagged
-from openbb_core.app.model.fast_api_settings import FastAPISettings
+from openbb_core.app.model.api_settings import APISettings
+from openbb_core.app.model.python_settings import PythonSettings
 from openbb_core.app.version import CORE_VERSION, VERSION
 
 
 class SystemSettings(Tagged):
     """System settings model."""
 
     # System section
@@ -42,15 +43,18 @@
     logging_rolling_clock: bool = False
     logging_verbosity: int = 20
     logging_sub_app: Literal["python", "api", "pro"] = "python"
     logging_suppress: bool = False
     log_collect: bool = True
 
     # API section
-    api_settings: FastAPISettings = Field(default_factory=FastAPISettings)
+    api_settings: APISettings = Field(default_factory=APISettings)
+
+    # Python section
+    python_settings: PythonSettings = Field(default_factory=PythonSettings)
 
     # Others
     debug_mode: bool = False
     test_mode: bool = False
     headless: bool = False
 
     model_config = ConfigDict(validate_assignment=True, frozen=True)
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/system_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     SYSTEM_SETTINGS_PATH = SYSTEM_SETTINGS_PATH
     SYSTEM_SETTINGS_ALLOWED_FIELD_SET = {
         "log_collect",
         "test_mode",
         "headless",
         "logging_sub_app",
         "api_settings",
+        "python_settings",
         "debug_mode",
     }
 
     PRO_VALIDATION_HASH = "300ac59fdcc8f899e0bc5c18cda8652220735da1a00e2af365efe9d8e5fe8306"  # pragma: allowlist secret
 
     def __init__(
         self,
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/package_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # pylint: disable=too-many-lines
 import builtins
 import inspect
 import re
 import shutil
 import sys
-from dataclasses import Field
+from dataclasses import Field as DCField
 from functools import partial
 from inspect import Parameter, _empty, isclass, signature
 from json import dumps, load
 from pathlib import Path
 from typing import (
     Any,
     Callable,
@@ -34,22 +34,20 @@
 from importlib_metadata import entry_points
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 from starlette.routing import BaseRoute
 from typing_extensions import Annotated, _AnnotatedAlias
 
 from openbb_core.app.extension_loader import ExtensionLoader, OpenBBGroups
-from openbb_core.app.model.custom_parameter import (
-    OpenBBCustomChoices,
-    OpenBBCustomParameter,
-)
 from openbb_core.app.model.example import Example
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.provider_interface import ProviderInterface
 from openbb_core.app.router import RouterLoader
+from openbb_core.app.service.system_service import SystemService
 from openbb_core.app.static.utils.console import Console
 from openbb_core.app.static.utils.linters import Linters
 from openbb_core.app.version import CORE_VERSION, VERSION
 from openbb_core.env import Env
 from openbb_core.provider.abstract.data import Data
 
 try:
@@ -350,23 +348,23 @@
 
     @classmethod
     def build(cls, path: str) -> str:
         """Build the import definition."""
         hint_type_list = cls.get_path_hint_type_list(path=path)
         code = "from openbb_core.app.static.container import Container"
         code += "\nfrom openbb_core.app.model.obbject import OBBject"
-        code += "\nfrom openbb_core.app.model.custom_parameter import OpenBBCustomParameter, OpenBBCustomChoices"
 
         # These imports were not detected before build, so we add them manually and
         # ruff --fix the resulting code to remove unused imports.
         # TODO: Find a better way to handle this. This is a temporary solution.
         code += "\nimport openbb_core.provider"
         code += "\nimport pandas"
         code += "\nimport numpy"
         code += "\nimport datetime"
+        code += "\nfrom datetime import date"
         code += "\nimport pydantic"
         code += "\nfrom pydantic import BaseModel"
         code += "\nfrom inspect import Parameter"
         code += "\nimport typing"
         code += "\nfrom typing import List, Dict, Union, Optional, Literal, Any"
         code += "\nfrom annotated_types import Ge, Le, Gt, Lt"
         code += "\nfrom warnings import warn, simplefilter"
@@ -375,14 +373,15 @@
         else:
             code += "\nfrom typing_extensions import Annotated, deprecated"
         code += "\nfrom openbb_core.app.utils import df_to_basemodel"
         code += "\nfrom openbb_core.app.static.utils.decorators import exception_handler, validate\n"
         code += "\nfrom openbb_core.app.static.utils.filters import filter_inputs\n"
         code += "\nfrom openbb_core.provider.abstract.data import Data"
         code += "\nfrom openbb_core.app.deprecation import OpenBBDeprecationWarning\n"
+        code += "\nfrom openbb_core.app.model.field import OpenBBField"
         if path.startswith("/quantitative"):
             code += "\nfrom openbb_quantitative.models import "
             code += "(CAPMModel,NormalityModel,OmegaModel,SummaryModel,UnitRootModel)"
 
         module_list = [hint_type.__module__ for hint_type in hint_type_list]
         module_list = list(set(module_list))
         module_list.sort()
@@ -577,16 +576,16 @@
         # we need to add the chart parameter here bc of the docstring generation
         if CHARTING_INSTALLED and path.replace("/", "_")[1:] in Charting.functions():
             parameter_map["chart"] = Parameter(
                 name="chart",
                 kind=Parameter.POSITIONAL_OR_KEYWORD,
                 annotation=Annotated[
                     bool,
-                    OpenBBCustomParameter(
-                        description="Whether to create a chart or not, by default False."
+                    OpenBBField(
+                        description="Whether to create a chart or not, by default False.",
                     ),
                 ],
                 default=False,
             )
 
         formatted: Dict[str, Parameter] = {}
         var_kw = []
@@ -600,22 +599,22 @@
                 type_ = getattr(field, "type")
                 args = getattr(type_, "__args__")
                 first = args[0] if args else None
                 formatted["provider"] = Parameter(
                     name="provider",
                     kind=Parameter.POSITIONAL_OR_KEYWORD,
                     annotation=Annotated[
-                        Union[MethodDefinition.get_type(field), None],
-                        OpenBBCustomParameter(
+                        Optional[MethodDefinition.get_type(field)],
+                        OpenBBField(
                             description=(
                                 "The provider to use for the query, by default None.\n"
                                 f"    If None, the provider specified in defaults is selected or '{first}' if there is\n"
                                 "    no default."
                                 ""
-                            )
+                            ),
                         ),
                     ],
                     default=None,
                 )
             elif MethodDefinition.is_annotated_dc(param.annotation):
                 fields = param.annotation.__args__[0].__dataclass_fields__
                 for field_name, field in fields.items():
@@ -658,44 +657,43 @@
 
     @staticmethod
     def add_field_custom_annotations(
         od: OrderedDict[str, Parameter], model_name: Optional[str] = None
     ):
         """Add the field custom description and choices to the param signature as annotations."""
         if model_name:
-            available_fields: Dict[str, Field] = (
+            available_fields: Dict[str, DCField] = (
                 ProviderInterface().params[model_name]["standard"].__dataclass_fields__
             )
 
             for param, value in od.items():
                 if param not in available_fields:
                     continue
 
                 field_default = available_fields[param].default
-
                 choices = getattr(field_default, "json_schema_extra", {}).get(
                     "choices", []
                 )
                 description = getattr(field_default, "description", "")
 
-                if choices:
-                    new_value = value.replace(
-                        annotation=Annotated[
-                            value.annotation,
-                            OpenBBCustomParameter(description=description),
-                            OpenBBCustomChoices(choices=choices),
-                        ],
-                    )
-                else:
-                    new_value = value.replace(
-                        annotation=Annotated[
-                            value.annotation,
-                            OpenBBCustomParameter(description=description),
-                        ],
-                    )
+                PartialParameter = partial(
+                    OpenBBField,
+                    description=description,
+                )
+
+                new_value = value.replace(
+                    annotation=Annotated[
+                        value.annotation,
+                        (
+                            PartialParameter(choices=choices)
+                            if choices
+                            else PartialParameter()
+                        ),
+                    ],
+                )
 
                 od[param] = new_value
 
     @staticmethod
     def build_func_params(formatted_params: OrderedDict[str, Parameter]) -> str:
         """Stringify function params."""
         func_params = ",\n        ".join(
@@ -1040,14 +1038,15 @@
         cls,
         model_name: str,
         summary: str,
         explicit_params: dict,
         kwarg_params: dict,
         returns: Dict[str, FieldInfo],
         results_type: str,
+        sections: List[str],
     ) -> str:
         """Create the docstring for model."""
 
         def format_type(type_: str, char_limit: Optional[int] = None) -> str:
             """Format type in docstrings."""
             type_str = str(type_)
             type_str = type_str.replace("NoneType", "None")
@@ -1073,58 +1072,64 @@
             type_ = (
                 getattr(p_type, "__name__", "") if inspect.isclass(p_type) else p_type
             )
             metadata = getattr(annotation, "__metadata__", [])
             description = getattr(metadata[0], "description", "") if metadata else ""
             return type_, description
 
-        docstring = summary.strip("\n").replace("\n    ", f"\n{create_indent(2)}")
-        docstring += "\n\n"
-        docstring += f"{create_indent(2)}Parameters\n"
-        docstring += f"{create_indent(2)}----------\n"
-
-        # Explicit parameters
-        for param_name, param in explicit_params.items():
-            type_, description = get_param_info(param)
-            type_str = format_type(str(type_), char_limit=79)
-            docstring += f"{create_indent(2)}{param_name} : {type_str}\n"
-            docstring += f"{create_indent(3)}{format_description(description)}\n"
-
-        # Kwargs
-        for param_name, param in kwarg_params.items():
-            p_type = getattr(param, "type", "")
-            type_ = (
-                getattr(p_type, "__name__", "") if inspect.isclass(p_type) else p_type
-            )
+        # Description summary
+        if "description" in sections:
+            docstring = summary.strip("\n").replace("\n    ", f"\n{create_indent(2)}")
+            docstring += "\n\n"
+        if "parameters" in sections:
+            docstring += f"{create_indent(2)}Parameters\n"
+            docstring += f"{create_indent(2)}----------\n"
+
+            # Explicit parameters
+            for param_name, param in explicit_params.items():
+                type_, description = get_param_info(param)
+                type_str = format_type(str(type_), char_limit=79)
+                docstring += f"{create_indent(2)}{param_name} : {type_str}\n"
+                docstring += f"{create_indent(3)}{format_description(description)}\n"
+
+            # Kwargs
+            for param_name, param in kwarg_params.items():
+                p_type = getattr(param, "type", "")
+                type_ = (
+                    getattr(p_type, "__name__", "")
+                    if inspect.isclass(p_type)
+                    else p_type
+                )
 
-            if "NoneType" in str(type_):
-                type_ = f"Optional[{type_}]".replace(", NoneType", "")
+                if "NoneType" in str(type_):
+                    type_ = f"Optional[{type_}]".replace(", NoneType", "")
 
-            default = getattr(param, "default", "")
-            description = getattr(default, "description", "")
-            docstring += f"{create_indent(2)}{param_name} : {type_}\n"
-            docstring += f"{create_indent(3)}{format_description(description)}\n"
-
-        # Returns
-        docstring += "\n"
-        docstring += f"{create_indent(2)}Returns\n"
-        docstring += f"{create_indent(2)}-------\n"
-        providers, _ = get_param_info(explicit_params.get("provider", None))
-        docstring += cls.get_OBBject_description(results_type, providers)
-
-        # Schema
-        underline = "-" * len(model_name)
-        docstring += f"\n{create_indent(2)}{model_name}\n"
-        docstring += f"{create_indent(2)}{underline}\n"
-
-        for name, field in returns.items():
-            field_type = cls.get_field_type(field.annotation, field.is_required())
-            description = getattr(field, "description", "")
-            docstring += f"{create_indent(2)}{field.alias or name} : {field_type}\n"
-            docstring += f"{create_indent(3)}{format_description(description)}\n"
+                default = getattr(param, "default", "")
+                description = getattr(default, "description", "")
+                docstring += f"{create_indent(2)}{param_name} : {type_}\n"
+                docstring += f"{create_indent(3)}{format_description(description)}\n"
+
+        if "returns" in sections:
+            # Returns
+            docstring += "\n"
+            docstring += f"{create_indent(2)}Returns\n"
+            docstring += f"{create_indent(2)}-------\n"
+            providers, _ = get_param_info(explicit_params.get("provider", None))
+            docstring += cls.get_OBBject_description(results_type, providers)
+
+            # Schema
+            underline = "-" * len(model_name)
+            docstring += f"\n{create_indent(2)}{model_name}\n"
+            docstring += f"{create_indent(2)}{underline}\n"
+
+            for name, field in returns.items():
+                field_type = cls.get_field_type(field.annotation, field.is_required())
+                description = getattr(field, "description", "")
+                docstring += f"{create_indent(2)}{field.alias or name} : {field_type}\n"
+                docstring += f"{create_indent(3)}{format_description(description)}\n"
         return docstring
 
     @classmethod
     def generate(
         cls,
         path: str,
         func: Callable,
@@ -1132,14 +1137,19 @@
         model_name: Optional[str] = None,
         examples: Optional[List[Example]] = None,
     ) -> Optional[str]:
         """Generate the docstring for the function."""
         doc = func.__doc__ or ""
         param_types = {}
 
+        sections = SystemService().system_settings.python_settings.docstring_sections
+        max_length = (
+            SystemService().system_settings.python_settings.docstring_max_length
+        )
+
         # Parameters explicit in the function signature
         explicit_params = dict(formatted_params)
         explicit_params.pop("extra_params", None)
         # Map of parameter names to types
         param_types = {k: v.annotation for k, v in explicit_params.items()}
 
         if model_name:
@@ -1150,40 +1160,47 @@
                 kwarg_params = params["extra"].__dataclass_fields__
                 param_types.update({k: v.type for k, v in kwarg_params.items()})
                 # Format the annotation to hide the metadata, tags, etc.
                 annotation = func.__annotations__.get("return")
                 results_type = (
                     cls._get_repr(
                         cls._get_generic_types(
-                            annotation.model_fields["results"].annotation,  # type: ignore[union-attr]
+                            annotation.model_fields["results"].annotation,  # type: ignore[union-attr,arg-type]
                             [],
                         ),
                         model_name,
                     )
                     if isclass(annotation) and issubclass(annotation, OBBject)  # type: ignore[arg-type]
                     else model_name
                 )
                 doc = cls.generate_model_docstring(
                     model_name=model_name,
                     summary=func.__doc__ or "",
                     explicit_params=explicit_params,
                     kwarg_params=kwarg_params,
                     returns=return_schema.model_fields,
                     results_type=results_type,
+                    sections=sections,
                 )
         else:
             doc = doc.replace("\n    ", f"\n{create_indent(2)}")
 
-        if doc and examples:
+        if doc and examples and "examples" in sections:
             doc += cls.build_examples(
                 path.replace("/", "."),
                 param_types,
                 examples,
             )
 
+        if (
+            max_length  # pylint: disable=chained-comparison
+            and len(doc) > max_length
+            and max_length > 3
+        ):
+            doc = doc[: max_length - 3] + "..."
         return doc
 
     @classmethod
     def _get_generic_types(cls, type_: type, items: list) -> List[str]:
         """Unpack generic types recursively.
 
         Parameters
@@ -1669,18 +1686,18 @@
                 examples,  # type: ignore
             )
             # Add data for the endpoints having a standard model
             if route_method == {"GET"}:
                 reference[path]["description"] = getattr(
                     route, "description", "No description available."
                 )
+
+                # TODO: The reference is not getting populated when a command does not use a standard model
                 # Access model map from the ProviderInterface
-                model_map = cls.pi.map[
-                    standard_model
-                ]  # pylint: disable=protected-access
+                model_map = cls.pi.map.get(standard_model, {})
 
                 for provider in model_map:
                     if provider == "openbb":
                         # openbb provider is always present hence its the standard field
                         reference[path]["parameters"]["standard"] = (
                             cls._get_provider_field_params(
                                 standard_model, "QueryParams"
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/env.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/core/openbb_core/provider/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,12 +312,14 @@
                 return dt <= end_date
             return True
         return False
 
     return list(filter(_filter, data))
 
 
-def safe_fromtimestamp(timestamp: float, tz: Optional[timezone] = None) -> datetime:
+def safe_fromtimestamp(
+    timestamp: Union[float, int], tz: Optional[timezone] = None
+) -> datetime:
     """datetime.fromtimestamp alternative which supports negative timestamps on Windows platform."""
     if os.name == "nt" and timestamp < 0:
         return datetime(1970, 1, 1, tzinfo=tz) + timedelta(seconds=timestamp)
     return datetime.fromtimestamp(timestamp, tz)
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Technical Analysis Helpers."""
 
-import warnings
 from typing import Any, List, Literal, Optional, Tuple, Union
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 
-_warn = warnings.warn
-
 
 def validate_data(data: list, length: Union[int, List[int]]) -> None:
     """Validate data."""
     if isinstance(length, int):
         length = [length]
     for item in length:
         if item > len(data):
@@ -47,19 +45,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     rs = (1.0 / (4.0 * np.log(2.0))) * (
         (data["high"] / data["low"]).apply(np.log)
     ) ** 2.0
@@ -102,19 +100,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_return = (data["close"] / data["close"].shift(1)).apply(np.log)
 
     result = log_return.rolling(window=window, center=False).std() * np.sqrt(
@@ -155,19 +153,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_hl = (data["high"] / data["low"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
 
@@ -216,19 +214,19 @@
 
     Example
     -------
     >>> data = obb.equity.price.historical('BTC-USD')
     >>> df = obb.technical.hodges_tompkins(data, is_crypto = True)
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_return = (data["close"] / data["close"].shift(1)).apply(np.log)
 
     vol = log_return.rolling(window=window, center=False).std() * np.sqrt(
@@ -276,19 +274,19 @@
 
     Returns
     -------
     pd.Series : results
         Pandas Series with results.
     """
     if window < 1:
-        _warn("Error: Window must be at least 1, defaulting to 30.")
+        warn("Error: Window must be at least 1, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_ho = (data["high"] / data["open"]).apply(np.log)
     log_lo = (data["low"] / data["open"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
@@ -333,19 +331,19 @@
 
     Returns
     -------
     pd.DataFrame : results
         Dataframe with results.
     """
     if window < 2:
-        _warn("Error: Window must be at least 2, defaulting to 30.")
+        warn("Error: Window must be at least 2, defaulting to 30.")
         window = 30
 
     if trading_periods and is_crypto:
-        _warn("is_crypto is overridden by trading_periods.")
+        warn("is_crypto is overridden by trading_periods.")
 
     if not trading_periods:
         trading_periods = 365 if is_crypto else 252
 
     log_ho = (data["high"] / data["open"]).apply(np.log)
     log_lo = (data["low"] / data["open"]).apply(np.log)
     log_co = (data["close"] / data["open"]).apply(np.log)
@@ -543,20 +541,20 @@
     """
     if close_col not in data.columns:
         raise ValueError(f"Column {close_col} not in data")
 
     if start_date and end_date:
         if start_date not in data.index:
             date0 = data.index[data.index.get_indexer([end_date], method="nearest")[0]]
-            _warn(f"Start date not in data.  Using nearest: {date0}")
+            warn(f"Start date not in data.  Using nearest: {date0}")
         else:
             date0 = start_date
         if end_date not in data.index:
             date1 = data.index[data.index.get_indexer([end_date], method="nearest")[0]]
-            _warn(f"End date not in data.  Using nearest: {date1}")
+            warn(f"End date not in data.  Using nearest: {date1}")
         else:
             date1 = end_date
 
         data0 = data.loc[date0, close_col]
         data1 = data.loc[date1, close_col]
 
         min_pr = min(data0, data1)
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.6.dev202404200009/extensions/technical/openbb_technical/technical_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Technical Analysis Router."""
 
 # pylint: disable=too-many-lines
-from typing import List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
 import pandas_ta as ta
 from openbb_core.app.model.example import APIEx, PythonEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.router import Router
 from openbb_core.app.utils import (
@@ -13,29 +13,171 @@
     df_to_basemodel,
     get_target_column,
     get_target_columns,
 )
 from openbb_core.provider.abstract.data import Data
 from pydantic import NonNegativeFloat, NonNegativeInt, PositiveFloat, PositiveInt
 
-from .helpers import (
+from openbb_technical.helpers import (
     calculate_cones,
     calculate_fib_levels,
     clenow_momentum,
     validate_data,
 )
+from openbb_technical.relative_rotation import (
+    RelativeRotationData,
+    RelativeRotationFetcher,
+    RelativeRotationQueryParams,
+)
 
 # TODO: Split this into multiple files
 router = Router(prefix="", description="Technical Analysis tools.")
 
 
 @router.command(
     methods=["POST"],
     examples=[
         PythonEx(
+            description="Calculate the Relative Strength Ratio and Relative Strength Momentum"
+            + " for a group of symbols against a benchmark.",
+            code=[
+                "stock_data = obb.equity.price.historical("
+                + "symbol='AAPL,MSFT,GOOGL,META,AMZN,TSLA,SPY', start_date='2022-01-01', provider='yfinance')",
+                "rr_data = obb.technical.relative_rotation(data=stock_data.results, benchmark='SPY')",
+                "rs_ratios = rr_data.results.rs_ratios",
+                "rs_momentum = rr_data.results.rs_momentum",
+            ],
+        ),
+        PythonEx(
+            description="When the assets are not traded 252 days per year,"
+            + "adjust the momentum and volatility periods accordingly.",
+            code=[
+                "crypto_data = obb.crypto.price.historical("
+                + " symbol='BTCUSD,ETHUSD,SOLUSD', start_date='2021-01-01', provider='yfinance')",
+                "rr_data = obb.technical.relative_rotation(data=crypto_data.results, benchmark='BTCUSD',"
+                + " long_period=365, short_period=30, window=30, trading_periods=365)",
+            ],
+        ),
+        APIEx(
+            description="Note that the mock data displayed here is insufficient."
+            + " It must contain multiple symbols, with the benchmark, and be daily data at least 1 year in length.",
+            parameters={"benchmark": "SPY", "data": APIEx.mock_data("timeseries")},
+        ),
+    ],
+)
+async def relative_rotation(
+    data: List[Data],
+    benchmark: str,
+    study: Literal["price", "volume", "volatility"] = "price",
+    long_period: Optional[int] = 252,
+    short_period: Optional[int] = 21,
+    window: Optional[int] = 21,
+    trading_periods: Optional[int] = 252,
+    chart_params: Optional[Dict[str, Any]] = None,
+) -> OBBject[RelativeRotationData]:
+    """Calculate the Relative Strength Ratio and Relative Strength Momentum for a group of symbols against a benchmark.
+
+    Parameters
+    ----------
+    data : list[Data]
+        The data to be used for the relative rotation calculations.
+        This should be the multi-symbol output from the 'equity.price.historical' endpoint, or similar.
+        Or a pivot table with the 'date' column as the index, the symbols as the columns, and the 'study' as the values.
+        It is recommended to use the 'equity.price.historical' endpoint to get the data, and feed the results as-is.
+    benchmark : str
+        The symbol to be used as the benchmark.
+    study : Literal[price, volume, volatility]
+        The data point for the calculations. If 'price', the closing price will be used.
+        If 'volatility', the standard deviation of the closing price will be used.
+        If 'data' is supplied as a pivot table,
+        the 'study' will assume the values are the closing price and 'volume' will be ignored.
+    long_period : int, optional
+        The length of the long period for momentum calculation, by default 252.
+        Adjust this value when supplying a time series with an interval that is not daily.
+        For example, if the data is monthly, the long period should be 12.
+    short_period : int, optional
+        The length of the short period for momentum calculation, by default 21.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    window : int, optional
+        The length of window for the standard deviation calculation, by default 21.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    trading_periods : int, optional
+        The number of trading periods per year, for the standard deviation calculation, by default 252.
+        Adjust this value when supplying a time series with an interval that is not daily.
+    chart_params : dict[str, Any], optional
+        Additional parameters to pass when `chart=True` and the `openbb-charting` extension is installed.
+        Parameters can be passed again to redraw the chart using the charting.to_chart() method of the response.
+
+        ChartParams
+        -----------
+        date : str, optional
+            A target end date within the data to use for the chart, by default is the last date in the data.
+        show_tails : bool
+            Show the tails on the chart, by default True.
+        tail_periods : int
+            Number of periods to show in the tails, by default 16.
+        tail_interval : Literal[day, week, month]
+            Interval to show the tails, by default 'week'.
+        title : str, optional
+            Title of the chart.
+
+    Returns
+    -------
+    OBBject[RelativeRotationData]
+        results : RelativeRotationData
+            symbols : list[str]:
+                The symbols that are being compared against the benchmark.
+            benchmark : str
+                The benchmark symbol.
+            study : Literal[price, volume, volatility]
+                The data point for the selected.
+            long_period : int
+                The length of the long period for momentum calculation, as entered by the user.
+            short_period : int
+                The length of the short period for momentum calculation, as entered by the user.
+            window : int
+                The length of window for the standard deviation calculation.
+            trading_periods : int
+                The number of trading periods per year, for the standard deviation calculation.
+            start_date : str
+                The start date of the data after adjusting the length of the data for the calculations.
+            end_date : str
+                The end date of the data.
+            symbols_data : list[Data]
+                The data representing the selected 'study' for each symbol.
+            benchmark_data : list[Data]
+                The data representing the selected 'study' for the benchmark.
+            rs_ratios : list[Data]
+                The normalized relative strength ratios data.
+            rs_momentum : list[Data]
+                The normalized relative strength momentum data.
+    """
+
+    params = RelativeRotationQueryParams(
+        data=data,
+        benchmark=benchmark,
+        study=study,
+        long_period=long_period,
+        short_period=short_period,
+        window=window,
+        trading_periods=trading_periods,
+        chart_params=chart_params,
+    )
+
+    return OBBject(
+        results=RelativeRotationFetcher.transform_data(
+            params, RelativeRotationFetcher.extract_data(params, {})
+        )
+    )
+
+
+@router.command(
+    methods=["POST"],
+    examples=[
+        PythonEx(
             description="Get the Average True Range.",
             code=[
                 "stock_data = obb.equity.price.historical(symbol='TSLA', start_date='2023-01-01', provider='fmp')",
                 "atr_data = obb.technical.atr(data=stock_data.results)",
             ],
         ),
         APIEx(parameters={"length": 2, "data": APIEx.mock_data("timeseries")}),
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from plotly.graph_objs import Figure
 
 from openbb_charting.core.chart_style import ChartStyle
 from openbb_charting.core.openbb_figure import OpenBBFigure
 from openbb_charting.core.plotly_ta.ta_class import PlotlyTA
 from openbb_charting.core.to_chart import to_chart
 from openbb_charting.styles.colors import LARGE_CYCLER
+from openbb_charting.utils import relative_rotation
 from openbb_charting.utils.generic_charts import bar_chart
 from openbb_charting.utils.helpers import (
     calculate_returns,
     heikin_ashi,
     should_share_axis,
     z_score_standardization,
 )
@@ -441,14 +442,15 @@
         ),
         yaxis1=(
             dict(
                 side="right",
                 ticklen=0,
                 showgrid=True,
                 showline=True,
+                mirror=True,
                 gridcolor="rgba(128,128,128,0.3)",
                 title=dict(
                     text=y1title if y1title else None, standoff=20, font=dict(size=20)
                 ),
                 tickfont=dict(size=14),
                 anchor="x",
             )
@@ -467,16 +469,17 @@
             )
             if y2title
             else None
         ),
         xaxis=dict(
             ticklen=0,
             showgrid=True,
-            showline=True,
             gridcolor="rgba(128,128,128,0.3)",
+            showline=True,
+            mirror=True,
         ),
         margin=dict(l=20, r=20, b=20, t=20),
         dragmode="pan",
         hovermode="x",
     )
     if kwargs.get("title"):
         title = kwargs["title"]
@@ -1215,7 +1218,77 @@
     if kwargs.get("layout_kwargs"):
         fig.update_layout(kwargs.get("layout_kwargs"))
     if kwargs.get("title"):
         fig.set_title(str(kwargs.get("title")))
     content = fig.to_plotly_json()
 
     return fig, content
+
+
+def technical_relative_rotation(
+    **kwargs: Any,
+) -> Tuple["OpenBBFigure", Dict[str, Any]]:
+    """Relative Rotation Chart."""
+
+    ratios_df = basemodel_to_df(kwargs["obbject_item"].rs_ratios, index="date")  # type: ignore
+    momentum_df = basemodel_to_df(kwargs["obbject_item"].rs_momentum, index="date")  # type: ignore
+    benchmark_symbol = kwargs["obbject_item"].benchmark  # type: ignore
+    study = kwargs.get("study", None)
+    study = str(kwargs["obbject_item"].study) if study is None else str(study)
+    show_tails = kwargs.get("show_tails")
+    show_tails = True if show_tails is None else show_tails
+    tail_periods = int(kwargs.get("tail_periods")) if "tail_periods" in kwargs else 16  # type: ignore
+    tail_interval = str(kwargs.get("tail_interval")) if "tail_interval" in kwargs else "week"  # type: ignore
+    date = kwargs.get("date") if "date" in kwargs else None  # type: ignore
+    show_tails = False if date is not None else show_tails
+    if ratios_df.empty or momentum_df.empty:
+        raise RuntimeError("Error: No data to plot.")
+
+    if show_tails is True:
+        fig = relative_rotation.create_rrg_with_tails(
+            ratios_df, momentum_df, study, benchmark_symbol, tail_periods, tail_interval  # type: ignore
+        )
+
+    if show_tails is False:
+        fig = relative_rotation.create_rrg_without_tails(
+            ratios_df, momentum_df, benchmark_symbol, study, date  # type: ignore
+        )
+
+    figure = OpenBBFigure(fig)
+    font_color = "black" if ChartStyle().plt_style == "light" else "white"
+    figure.update_layout(
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(255,255,255,1)",
+        font=dict(color=font_color),
+        yaxis=dict(
+            showgrid=True,
+            gridcolor="rgba(128,128,128,0.3)",
+            side="left",
+            showline=True,
+            zeroline=True,
+            mirror=True,
+            ticklen=0,
+            tickfont=dict(size=14),
+            titlefont=dict(size=16),
+        ),
+        xaxis=dict(
+            showgrid=True,
+            gridcolor="rgba(128,128,128,0.3)",
+            showline=True,
+            zeroline=True,
+            mirror=True,
+            ticklen=0,
+            tickfont=dict(size=14),
+            titlefont=dict(size=16),
+            hoverformat="",
+        ),
+        hoverlabel=dict(
+            font_size=12,
+        ),
+        hovermode="x",
+        hoverdistance=50,
+    )
+    if kwargs.get("title") is not None:
+        figure.set_title(str(kwargs.get("title")))
+    content = figure.to_plotly_json()
+
+    return figure, content
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,25 @@
 from openbb_charting.core.to_chart import ChartIndicators
 
 MAMODES = Literal["ema", "sma", "wma", "hna", "zlma", "rma"]
 
 
 def _get_type_name(t):
     """Get the type name of a type hint."""
-
-    if hasattr(t, "__origin__") and hasattr(t.__origin__, "__name__"):
-        return f"{t.__origin__.__name__}[{', '.join([_get_type_name(arg) for arg in t.__args__])}]"
+    if hasattr(t, "__origin__"):
+        if hasattr(t.__origin__, "__name__"):
+            return f"{t.__origin__.__name__}[{', '.join([_get_type_name(arg) for arg in t.__args__])}]"
+        if hasattr(t.__origin__, "_name"):
+            return f"{t.__origin__._name}[{', '.join([_get_type_name(arg) for arg in t.__args__])}]"  # pylint: disable=W0212
+    if isinstance(t, str):
+        return t
     if hasattr(t, "__name__"):
         return t.__name__
+    if hasattr(t, "_name"):
+        return t._name  # pylint: disable=W0212
     return str(t)
 
 
 class BaseQueryParams(QueryParams):
     """Base Query Parmams Base Model."""
 
     def __init__(self, **data):
@@ -340,36 +346,62 @@
     )
     drift: Optional[int] = Field(
         default=1,
         description="Drift value for the RSI, by default is 1.",
     )
 
 
+class TechnicalRelativeRotationChartQueryParams(ChartQueryParams):
+    """Technical Relative Rotation Chart Query Params."""
+
+    date: Optional[str] = Field(
+        default=None,
+        description="A target end date within the data to use for the chart, by default is the last date in the data.",
+    )
+    show_tails: bool = Field(
+        default=True,
+        description="Show the tails on the chart, by default True.",
+    )
+    tail_periods: Optional[int] = Field(
+        default=16,
+        description="Number of periods to show in the tails, by default 16.",
+    )
+    tail_interval: Literal["day", "week", "month"] = Field(
+        default="week",
+        description="The interval to show the tails, by default 'week'.",
+    )
+    title: Optional[str] = Field(
+        default=None,
+        description="Title of the chart.",
+    )
+
+
 class ChartParams:
     """Chart Query Params."""
 
     crypto_price_historical = EquityPriceHistoricalChartQueryParams
     equity_price_historical = EquityPriceHistoricalChartQueryParams
     economy_fred_series = EconomyFredSeriesChartQueryParams
     equity_price_historical = EquityPriceHistoricalChartQueryParams
     equity_price_performance = EquityPricePerformanceChartQueryParams
     etf_historical = EtfPricePerformanceChartQueryParams
     etf_holdings = EtfHoldingsChartQueryParams
     etf_price_performance = EquityPricePerformanceChartQueryParams
     index_price_historical = EquityPriceHistoricalChartQueryParams
+    technical_adx = TechnicalADXChartQueryParams
+    technical_aroon = TechnicalArooonChartQueryParams
     technical_cones = TechnicalConesChartQueryParams
-    technical_sma = TechnicalSMAChartQueryParams
     technical_ema = TechnicalEMAChartQueryParams
     technical_hma = TechnicalHMAChartQueryParams
-    technical_wma = TechnicalWMAChartQueryParams
-    technical_zlma = TechnicalZLMAChartQueryParams
-    technical_adx = TechnicalADXChartQueryParams
-    technical_aroon = TechnicalArooonChartQueryParams
     technical_macd = TechnicalMACDChartQueryParams
+    technical_relative_rotation = TechnicalRelativeRotationChartQueryParams
     technical_rsi = TechnicalRSIChartQueryParams
+    technical_sma = TechnicalSMAChartQueryParams
+    technical_wma = TechnicalWMAChartQueryParams
+    technical_zlma = TechnicalZLMAChartQueryParams
 
 
 class IndicatorsQueryParams(BaseQueryParams):
     """Indicators Query Params."""
 
 
 class MAIndicatorsQueryParams(IndicatorsQueryParams):
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/colors.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998114630467572%*

 * *Differences: {"'layout'": "{'yaxis': {'gridcolor': 'rgba(128, 128, 128, 0.33)'}}"}*

```diff
@@ -112,15 +112,15 @@
             },
             "zeroline": false
         },
         "yaxis": {
             "anchor": "x",
             "automargin": true,
             "fixedrange": false,
-            "gridcolor": "rgba(128, 128, 128, 0.25)",
+            "gridcolor": "rgba(128, 128, 128, 0.33)",
             "linecolor": "#F5EFF3",
             "mirror": true,
             "showgrid": true,
             "showline": true,
             "side": "right",
             "tick0": 0.5,
             "ticks": "outside",
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996150703871293%*

 * *Differences: {"'layout'": "{'xaxis': {'title': {'font': OrderedDict([('size', 16)])}}, 'yaxis': {'title': "*

 * *             "{'font': OrderedDict([('size', 16)])}, 'gridcolor': 'rgba(128, 128, 128, 0.33)'}}"}*

```diff
@@ -101,31 +101,37 @@
             "showline": true,
             "tick0": 1,
             "tickfont": {
                 "size": 14
             },
             "ticks": "outside",
             "title": {
+                "font": {
+                    "size": 16
+                },
                 "standoff": 20
             },
             "zeroline": false
         },
         "yaxis": {
             "anchor": "x",
             "automargin": true,
             "fixedrange": false,
-            "gridcolor": "rgba(128, 128, 128, 0.25)",
+            "gridcolor": "rgba(128, 128, 128, 0.33)",
             "linecolor": "#A9A9A9",
             "mirror": true,
             "showgrid": true,
             "showline": true,
             "side": "right",
             "tick0": 0.5,
             "ticks": "outside",
             "title": {
+                "font": {
+                    "size": 16
+                },
                 "standoff": 20
             },
             "zeroline": false
         }
     },
     "line": {
         "color": "#111111",
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/assets/reference.json` & `openbb_nightly-4.1.6.dev202404200009/openbb/assets/reference.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999991187658298%*

 * *Differences: {"'paths'": "{'/equity/fundamental/filings': {'parameters': {'sec': {0: {'type': 'Union[str, "*

 * *            "int]'}}}, 'data': {'sec': {1: {'type': 'Union[str, int]'}, 5: {'type': 'Union[str, "*

 * *            "int]'}, 6: {'type': 'Union[str, int]'}, 7: {'type': 'Union[str, int]'}, 8: {'type': "*

 * *            "'Union[str, int]'}, 9: {'type': 'Union[str, int]'}, 10: {'type': 'Union[str, "*

 * *            "int]'}}}}, '/etf/holdings': {'data': {'sec': {44: {'type': 'Union[str, int]'}, 46: "*

 * *            "{'type': 'Union[s […]*

```diff
@@ -10359,15 +10359,15 @@
                         "type": "date"
                     },
                     {
                         "default": null,
                         "description": "The SEC Act number.",
                         "name": "act",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The SEC Item numbers.",
                         "name": "items",
                         "optional": true,
                         "type": "Union[str, float]"
@@ -10387,50 +10387,50 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The accession number.",
                         "name": "accession_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The file number.",
                         "name": "file_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The film number.",
                         "name": "film_number",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an inline XBRL filing.",
                         "name": "is_inline_xbrl",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an XBRL filing.",
                         "name": "is_xbrl",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The size of the filing.",
                         "name": "size",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The URL to the complete filing submission.",
                         "name": "complete_submission_url",
                         "optional": true,
                         "type": "str"
@@ -10529,15 +10529,15 @@
                 ],
                 "sec": [
                     {
                         "default": null,
                         "description": "Lookup filings by Central Index Key (CIK) instead of by symbol.",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "Type of the SEC filing form.",
                         "name": "type",
                         "optional": true,
                         "type": "Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']"
@@ -21204,29 +21204,29 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The rate tenor unit for reveivable portion of the swap.",
                         "name": "rate_tenor_unit_rec",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The reset date for reveivable portion of the swap.",
                         "name": "reset_date_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The reset date unit for reveivable portion of the swap.",
                         "name": "reset_date_unit_rec",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The type of rate for payment portion of the swap.",
                         "name": "rate_type_pmnt",
                         "optional": true,
                         "type": "str"
@@ -21267,29 +21267,29 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The rate tenor unit for payment portion of the swap.",
                         "name": "rate_tenor_unit_pmnt",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The reset date for payment portion of the swap.",
                         "name": "reset_date_pmnt",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The reset date unit for payment portion of the swap.",
                         "name": "reset_date_unit_pmnt",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     },
                     {
                         "default": null,
                         "description": "The type of repo.",
                         "name": "repo_type",
                         "optional": true,
                         "type": "str"
@@ -26845,15 +26845,15 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "Central Index Key (CIK)",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[int, str]"
+                        "type": "Union[str, int]"
                     }
                 ],
                 "standard": []
             },
             "deprecated": {
                 "flag": null,
                 "message": null
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/crypto.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/crypto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import Literal, Optional
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -27,19 +27,19 @@
         return crypto_price.ROUTER_crypto_price(command_runner=self._command_runner)
 
     @exception_handler
     @validate
     def search(
         self,
         query: Annotated[
-            Optional[str], OpenBBCustomParameter(description="Search query.")
+            Optional[str], OpenBBField(description="Search query.")
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search available cryptocurrency pairs within a provider.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/crypto_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -21,33 +21,29 @@
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "polygon", "tiingo", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical price data for cryptocurrency pair(s) within a provider.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/currency.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/currency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -29,15 +29,15 @@
 
     @exception_handler
     @validate
     def search(
         self,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Currency Search.
 
@@ -149,33 +149,33 @@
 
     @exception_handler
     @validate
     def snapshots(
         self,
         base: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The base currency symbol. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ] = "usd",
         quote_type: Annotated[
             Literal["direct", "indirect"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency."
             ),
         ] = "indirect",
         counter_currencies: Annotated[
             Union[List[str], str, None],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="An optional list of counter currency symbols to filter for. None returns all."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Snapshots of currency exchange rates from an indirect or direct perspective of a base currency.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/currency_price.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/currency_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -21,33 +21,29 @@
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "polygon", "tiingo", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Currency Historical Price. Currency historical data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/derivatives.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/derivatives_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import Literal, Optional
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -19,20 +19,18 @@
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def chains(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the complete options chain for a ticker.
 
@@ -179,21 +177,19 @@
 
     @exception_handler
     @validate
     def unusual(
         self,
         symbol: Annotated[
             Optional[str],
-            OpenBBCustomParameter(
-                description="Symbol to get data for. (the underlying symbol)"
-            ),
+            OpenBBField(description="Symbol to get data for. (the underlying symbol)"),
         ] = None,
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the complete options chain for a ticker.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/economy.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/economy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import (
-    OpenBBCustomChoices,
-    OpenBBCustomParameter,
-)
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -35,27 +32,23 @@
 
     @exception_handler
     @validate
     def calendar(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "tradingeconomics"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the upcoming, or historical, economic calendar of global events.
 
@@ -158,27 +151,23 @@
 
     @exception_handler
     @validate
     def composite_leading_indicator(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Use the composite leading indicator (CLI).
 
@@ -251,18 +240,16 @@
 
     @exception_handler
     @validate
     def cpi(
         self,
         country: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
-                description="The country to get data. Multiple comma separated items allowed for provider(s): fred."
-            ),
-            OpenBBCustomChoices(
+            OpenBBField(
+                description="The country to get data. Multiple comma separated items allowed for provider(s): fred.",
                 choices=[
                     "australia",
                     "austria",
                     "belgium",
                     "brazil",
                     "bulgaria",
                     "canada",
@@ -305,50 +292,43 @@
                     "south_africa",
                     "spain",
                     "sweden",
                     "switzerland",
                     "turkey",
                     "united_kingdom",
                     "united_states",
-                ]
+                ],
             ),
         ],
         units: Annotated[
             Literal["growth_previous", "growth_same", "index_2015"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The unit of measurement for the data.\n    Options:\n    - `growth_previous`: Percent growth from the previous period.\n      If monthly data, this is month-over-month, etc\n    - `growth_same`: Percent growth from the same period in the previous year.\n      If looking at monthly data, this would be year-over-year, etc.\n    - `index_2015`: Rescaled index value, such that the value in 2015 is 100."
             ),
         ] = "growth_same",
         frequency: Annotated[
             Literal["monthly", "quarter", "annual"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The frequency of the data.\n    Options: `monthly`, `quarter`, and `annual`."
             ),
         ] = "monthly",
         harmonized: Annotated[
-            bool,
-            OpenBBCustomParameter(
-                description="Whether you wish to obtain harmonized data."
-            ),
+            bool, OpenBBField(description="Whether you wish to obtain harmonized data.")
         ] = False,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Consumer Price Index (CPI).
 
@@ -431,36 +411,30 @@
             )
         )
 
     @exception_handler
     @validate
     def fred_regional(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 100000,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Query the Geo Fred API for regional economic data by series group.
 
@@ -548,15 +522,15 @@
 
         FredRegional
         ------------
         date : date
             The date of the data.
         region : Optional[str]
             The name of the region. (provider: fred)
-        code : Optional[Union[int, str]]
+        code : Optional[Union[str, int]]
             The code of the region. (provider: fred)
         value : Optional[Union[float, int]]
             The obersvation value. The units are defined in the search results by series ID. (provider: fred)
         series_id : Optional[str]
             The individual series ID for the region. (provider: fred)
 
         Examples
@@ -588,19 +562,19 @@
         )
 
     @exception_handler
     @validate
     def fred_search(
         self,
         query: Annotated[
-            Optional[str], OpenBBCustomParameter(description="The search word(s).")
+            Optional[str], OpenBBField(description="The search word(s).")
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for FRED series or economic releases by ID or string.
 
@@ -717,37 +691,33 @@
 
     @exception_handler
     @validate
     def fred_series(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fred."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 100000,
         provider: Annotated[
             Optional[Literal["fred", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get data by series ID from FRED.
 
@@ -871,27 +841,23 @@
 
     @exception_handler
     @validate
     def long_term_interest_rate(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Long-term interest rates that refer to government bonds maturing in ten years.
 
@@ -970,33 +936,27 @@
 
     @exception_handler
     @validate
     def money_measures(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         adjusted: Annotated[
             Optional[bool],
-            OpenBBCustomParameter(
-                description="Whether to return seasonally adjusted data."
-            ),
+            OpenBBField(description="Whether to return seasonally adjusted data."),
         ] = True,
         provider: Annotated[
             Optional[Literal["federal_reserve"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'federal_reserve' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Money Measures (M1/M2 and components).
 
@@ -1077,15 +1037,15 @@
 
     @exception_handler
     @validate
     def risk_premium(
         self,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Market Risk Premium by country.
 
@@ -1144,27 +1104,23 @@
 
     @exception_handler
     @validate
     def short_term_interest_rate(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Short-term interest rates.
 
@@ -1241,27 +1197,23 @@
 
     @exception_handler
     @validate
     def unemployment(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get global unemployment data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/economy_gdp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -23,39 +23,35 @@
 
     @exception_handler
     @validate
     def forecast(
         self,
         period: Annotated[
             Literal["quarter", "annual"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Time period of the data to return. Units for nominal GDP period. Either quarter or annual."
             ),
         ] = "annual",
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         type: Annotated[
             Literal["nominal", "real"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Type of GDP to get forecast of. Either nominal or real."
             ),
         ] = "real",
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Forecasted GDP Data.
 
@@ -126,33 +122,29 @@
 
     @exception_handler
     @validate
     def nominal(
         self,
         units: Annotated[
             Literal["usd", "usd_cap"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The unit of measurement for the data. Units to get nominal GDP in. Either usd or usd_cap indicating per capita."
             ),
         ] = "usd",
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Nominal GDP Data.
 
@@ -220,33 +212,29 @@
 
     @exception_handler
     @validate
     def real(
         self,
         units: Annotated[
             Literal["idx", "qoq", "yoy"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The unit of measurement for the data. Either idx (indicating 2015=100), qoq (previous period) or yoy (same period, previous year).)"
             ),
         ] = "yoy",
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["oecd"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'oecd' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Real GDP Data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -74,15 +74,15 @@
 
     @exception_handler
     @validate
     def market_snapshots(
         self,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get an updated equity market snapshot. This includes price data for thousands of stocks.
 
@@ -249,21 +249,21 @@
 
     @exception_handler
     @validate
     def profile(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get general information about a company. This includes company name, industry, sector and price data.
 
@@ -444,15 +444,15 @@
 
     @exception_handler
     @validate
     def screener(
         self,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Screen for companies meeting various criteria.
 
@@ -566,26 +566,24 @@
             )
         )
 
     @exception_handler
     @validate
     def search(
         self,
-        query: Annotated[str, OpenBBCustomParameter(description="Search query.")] = "",
+        query: Annotated[str, OpenBBField(description="Search query.")] = "",
         is_symbol: Annotated[
-            bool,
-            OpenBBCustomParameter(description="Whether to search by ticker symbol."),
+            bool, OpenBBField(description="Whether to search by ticker symbol.")
         ] = False,
         use_cache: Annotated[
-            Optional[bool],
-            OpenBBCustomParameter(description="Whether to use the cache or not."),
+            Optional[bool], OpenBBField(description="Whether to use the cache or not.")
         ] = True,
         provider: Annotated[
             Optional[Literal["intrinio", "sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for stock symbol, CIK, LEI, or company name.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -24,27 +24,23 @@
 
     @exception_handler
     @validate
     def dividend(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical and upcoming dividend payments. Includes dividend amount, ex-dividend and payment dates.
 
@@ -120,27 +116,23 @@
 
     @exception_handler
     @validate
     def earnings(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical and upcoming company earnings releases. Includes earnings per share (EPS) and revenue data.
 
@@ -221,35 +213,31 @@
         )
 
     @exception_handler
     @validate
     def ipo(
         self,
         symbol: Annotated[
-            Optional[str], OpenBBCustomParameter(description="Symbol to get data for.")
+            Optional[str], OpenBBField(description="Symbol to get data for.")
         ] = None,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 100,
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical and upcoming initial public offerings (IPOs).
 
@@ -365,27 +353,23 @@
 
     @exception_handler
     @validate
     def splits(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical and upcoming stock split operations.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_compare.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import Literal, Optional
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -18,20 +18,18 @@
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def peers(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the closest peers for a given company.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -28,21 +28,21 @@
 
     @exception_handler
     @validate
     def active(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the most actively traded stocks based on volume.
 
@@ -116,21 +116,21 @@
 
     @exception_handler
     @validate
     def aggressive_small_caps(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get top small cap stocks based on earnings growth.
 
@@ -204,37 +204,32 @@
 
     @exception_handler
     @validate
     def filings(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         form_type: Annotated[
             Optional[str],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Filter by form type. Visit https://www.sec.gov/forms for a list of supported form types."
             ),
         ] = None,
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 100,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more.
 
@@ -320,21 +315,21 @@
 
     @exception_handler
     @validate
     def gainers(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the top price gainers in the stock market.
 
@@ -408,21 +403,21 @@
 
     @exception_handler
     @validate
     def growth_tech(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get top tech stocks based on revenue and earnings growth.
 
@@ -496,21 +491,21 @@
 
     @exception_handler
     @validate
     def losers(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the top price losers in the stock market.
 
@@ -584,21 +579,21 @@
 
     @exception_handler
     @validate
     def undervalued_growth(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get potentially undervalued growth stocks.
 
@@ -672,21 +667,21 @@
 
     @exception_handler
     @validate
     def undervalued_large_caps(
         self,
         sort: Annotated[
             Literal["asc", "desc"],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Sort order. Possible values: 'asc', 'desc'. Default: 'desc'."
             ),
         ] = "desc",
         provider: Annotated[
             Optional[Literal["yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'yfinance' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get potentially undervalued large cap stocks.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_estimates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -25,27 +25,27 @@
 
     @exception_handler
     @validate
     def analyst_search(
         self,
         analyst_name: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Analyst names to return. Omitting will return all available analysts. Multiple comma separated items allowed for provider(s): benzinga."
             ),
         ] = None,
         firm_name: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Firm names to return. Omitting will return all available firms. Multiple comma separated items allowed for provider(s): benzinga."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["benzinga"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'benzinga' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for specific analysts and get their forecast track record.
 
@@ -233,21 +233,21 @@
 
     @exception_handler
     @validate
     def consensus(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get consensus price target and recommendation.
 
@@ -344,21 +344,21 @@
 
     @exception_handler
     @validate
     def forward_eps(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get forward EPS estimates.
 
@@ -463,21 +463,21 @@
 
     @exception_handler
     @validate
     def forward_sales(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get forward sales estimates.
 
@@ -586,21 +586,21 @@
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical analyst estimates for earnings and revenue.
 
@@ -704,25 +704,24 @@
 
     @exception_handler
     @validate
     def price_target(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp."
             ),
         ] = None,
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 200,
         provider: Annotated[
             Optional[Literal["benzinga", "fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'benzinga' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get analyst price targets by company.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_fundamental.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime
 from typing import List, Literal, Optional, Union
 from warnings import simplefilter, warn
 
 from annotated_types import Ge
 from openbb_core.app.deprecation import OpenBBDeprecationWarning
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated, deprecated
 
 
@@ -46,27 +46,25 @@
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def balance(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            str, OpenBBCustomParameter(description="Time period of the data to return.")
+            str, OpenBBField(description="Time period of the data to return.")
         ] = "annual",
         limit: Annotated[
             Optional[Annotated[int, Ge(ge=0)]],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 5,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the balance sheet for a given company.
 
@@ -408,24 +406,21 @@
             )
         )
 
     @exception_handler
     @validate
     def balance_growth(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 10,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the growth of a company's balance sheet items over time.
 
@@ -566,27 +561,25 @@
             )
         )
 
     @exception_handler
     @validate
     def cash(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            str, OpenBBCustomParameter(description="Time period of the data to return.")
+            str, OpenBBField(description="Time period of the data to return.")
         ] = "annual",
         limit: Annotated[
             Optional[Annotated[int, Ge(ge=0)]],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 5,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the cash flow statement for a given company.
 
@@ -836,24 +829,21 @@
             )
         )
 
     @exception_handler
     @validate
     def cash_growth(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 10,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the growth of a company's cash flow statement items over time.
 
@@ -976,32 +966,26 @@
             )
         )
 
     @exception_handler
     @validate
     def dividends(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical dividend data for a given company.
 
@@ -1082,20 +1066,18 @@
             )
         )
 
     @exception_handler
     @validate
     def employee_count(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical employee count data for a given company.
 
@@ -1167,29 +1149,28 @@
         )
 
     @exception_handler
     @validate
     def filings(
         self,
         symbol: Annotated[
-            Optional[str], OpenBBCustomParameter(description="Symbol to get data for.")
+            Optional[str], OpenBBField(description="Symbol to get data for.")
         ] = None,
         form_type: Annotated[
             Optional[str],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Filter by form type. Check the data provider for available types."
             ),
         ] = None,
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 100,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the URLs to SEC filings reported to EDGAR database, such as 10-K, 10-Q, 8-K, and more. SEC
         filings include Form 10-K, Form 10-Q, Form 8-K, the proxy statement, Forms 3, 4, and 5, Schedule 13, Form 114,
@@ -1212,15 +1193,15 @@
             no default.
         start_date : Optional[datetime.date]
             Start date of the data, in YYYY-MM-DD format. (provider: intrinio)
         end_date : Optional[datetime.date]
             End date of the data, in YYYY-MM-DD format. (provider: intrinio)
         thea_enabled : Optional[bool]
             Return filings that have been read by Intrinio's Thea NLP. (provider: intrinio)
-        cik : Optional[Union[int, str]]
+        cik : Optional[Union[str, int]]
             Lookup filings by Central Index Key (CIK) instead of by symbol. (provider: sec)
         type : Optional[Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']]
             Type of the SEC filing form. (provider: sec)
         use_cache : bool
             Whether or not to use cache.  If True, cache will store for one day. (provider: sec)
 
         Returns
@@ -1263,33 +1244,33 @@
             URL for the XBRL filing for the report. (provider: intrinio)
         industry_group : Optional[str]
             Industry group of the company. (provider: intrinio)
         industry_category : Optional[str]
             Industry category of the company. (provider: intrinio)
         report_date : Optional[date]
             The date of the filing. (provider: sec)
-        act : Optional[Union[int, str]]
+        act : Optional[Union[str, int]]
             The SEC Act number. (provider: sec)
         items : Optional[Union[str, float]]
             The SEC Item numbers. (provider: sec)
         primary_doc_description : Optional[str]
             The description of the primary document. (provider: sec)
         primary_doc : Optional[str]
             The filename of the primary document. (provider: sec)
-        accession_number : Optional[Union[int, str]]
+        accession_number : Optional[Union[str, int]]
             The accession number. (provider: sec)
-        file_number : Optional[Union[int, str]]
+        file_number : Optional[Union[str, int]]
             The file number. (provider: sec)
-        film_number : Optional[Union[int, str]]
+        film_number : Optional[Union[str, int]]
             The film number. (provider: sec)
-        is_inline_xbrl : Optional[Union[int, str]]
+        is_inline_xbrl : Optional[Union[str, int]]
             Whether the filing is an inline XBRL filing. (provider: sec)
-        is_xbrl : Optional[Union[int, str]]
+        is_xbrl : Optional[Union[str, int]]
             Whether the filing is an XBRL filing. (provider: sec)
-        size : Optional[Union[int, str]]
+        size : Optional[Union[str, int]]
             The size of the filing. (provider: sec)
         complete_submission_url : Optional[str]
             The URL to the complete filing submission. (provider: sec)
         filing_detail_url : Optional[str]
             The URL to the filing details. (provider: sec)
 
         Examples
@@ -1320,55 +1301,49 @@
 
     @exception_handler
     @validate
     def historical_attributes(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         tag: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         frequency: Annotated[
             Optional[Literal["daily", "weekly", "monthly", "quarterly", "yearly"]],
-            OpenBBCustomParameter(description="The frequency of the data."),
+            OpenBBField(description="The frequency of the data."),
         ] = "yearly",
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 1000,
         tag_type: Annotated[
-            Optional[str],
-            OpenBBCustomParameter(description="Filter by type, when applicable."),
+            Optional[str], OpenBBField(description="Filter by type, when applicable.")
         ] = None,
         sort: Annotated[
-            Optional[Literal["asc", "desc"]],
-            OpenBBCustomParameter(description="Sort order."),
+            Optional[Literal["asc", "desc"]], OpenBBField(description="Sort order.")
         ] = "desc",
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the historical values of a data tag from Intrinio.
 
@@ -1454,20 +1429,18 @@
             )
         )
 
     @exception_handler
     @validate
     def historical_eps(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical earnings per share data for a given company.
 
@@ -1542,20 +1515,18 @@
             )
         )
 
     @exception_handler
     @validate
     def historical_splits(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical stock splits for a given company.
 
@@ -1616,27 +1587,25 @@
             )
         )
 
     @exception_handler
     @validate
     def income(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            str, OpenBBCustomParameter(description="Time period of the data to return.")
+            str, OpenBBField(description="Time period of the data to return.")
         ] = "annual",
         limit: Annotated[
             Optional[Annotated[int, Ge(ge=0)]],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 5,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the income statement for a given company.
 
@@ -1980,28 +1949,25 @@
             )
         )
 
     @exception_handler
     @validate
     def income_growth(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 10,
         period: Annotated[
             Literal["annual", "quarter"],
-            OpenBBCustomParameter(description="Time period of the data to return."),
+            OpenBBField(description="Time period of the data to return."),
         ] = "annual",
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the growth of a company's income statement items over time.
 
@@ -2121,27 +2087,27 @@
 
     @exception_handler
     @validate
     def latest_attributes(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         tag: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the latest value of a data tag from Intrinio.
 
@@ -2207,20 +2173,18 @@
             )
         )
 
     @exception_handler
     @validate
     def management(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get executive management team data for a given company.
 
@@ -2293,21 +2257,21 @@
 
     @exception_handler
     @validate
     def management_compensation(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get executive management team compensation for a given company over time.
 
@@ -2395,29 +2359,29 @@
 
     @exception_handler
     @validate
     def metrics(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         period: Annotated[
             Optional[Literal["annual", "quarter"]],
-            OpenBBCustomParameter(description="Time period of the data to return."),
+            OpenBBField(description="Time period of the data to return."),
         ] = "annual",
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 100,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get fundamental metrics for a given company.
 
@@ -2716,21 +2680,21 @@
 
     @exception_handler
     @validate
     def multiples(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get equity valuation multiples for a given company.
 
@@ -2910,20 +2874,18 @@
     @validate
     @deprecated(
         "This endpoint is deprecated; use `/equity/profile` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.3.",
         category=OpenBBDeprecationWarning,
     )
     def overview(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get company general business and stock data for a given company.
 
@@ -3055,27 +3017,24 @@
             )
         )
 
     @exception_handler
     @validate
     def ratios(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            str, OpenBBCustomParameter(description="Time period of the data to return.")
+            str, OpenBBField(description="Time period of the data to return.")
         ] = "annual",
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 12,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get an extensive set of financial and accounting ratios for a given company over time.
 
@@ -3255,35 +3214,33 @@
             )
         )
 
     @exception_handler
     @validate
     def reported_financials(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            str, OpenBBCustomParameter(description="Time period of the data to return.")
+            str, OpenBBField(description="Time period of the data to return.")
         ] = "annual",
         statement_type: Annotated[
             str,
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The type of financial statement - i.e, balance, income, cash."
             ),
         ] = "balance",
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The number of data entries to return. Although the response object contains multiple results, because of the variance in the fields, year-to-year and quarter-to-quarter, it is recommended to view results in small chunks."
             ),
         ] = 100,
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get financial statements as reported by the company.
 
@@ -3359,40 +3316,38 @@
             )
         )
 
     @exception_handler
     @validate
     def revenue_per_geography(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            Literal["annual", "quarter"],
-            OpenBBCustomParameter(description="Time period of the data to return."),
+            Literal["quarter", "annual"],
+            OpenBBField(description="Time period of the data to return."),
         ] = "annual",
         structure: Annotated[
             Literal["hierarchical", "flat"],
-            OpenBBCustomParameter(description="Structure of the returned data."),
+            OpenBBField(description="Structure of the returned data."),
         ] = "flat",
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the revenue geographic breakdown for a given company over time.
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
-        period : Literal['annual', 'quarter']
+        period : Literal['quarter', 'annual']
             Time period of the data to return.
         structure : Literal['hierarchical', 'flat']
             Structure of the returned data.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
@@ -3450,40 +3405,38 @@
             )
         )
 
     @exception_handler
     @validate
     def revenue_per_segment(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         period: Annotated[
-            Literal["annual", "quarter"],
-            OpenBBCustomParameter(description="Time period of the data to return."),
+            Literal["quarter", "annual"],
+            OpenBBField(description="Time period of the data to return."),
         ] = "annual",
         structure: Annotated[
             Literal["hierarchical", "flat"],
-            OpenBBCustomParameter(description="Structure of the returned data."),
+            OpenBBField(description="Structure of the returned data."),
         ] = "flat",
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the revenue breakdown by business segment for a given company over time.
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
-        period : Literal['annual', 'quarter']
+        period : Literal['quarter', 'annual']
             Time period of the data to return.
         structure : Literal['hierarchical', 'flat']
             Structure of the returned data.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
@@ -3541,24 +3494,22 @@
             )
         )
 
     @exception_handler
     @validate
     def search_attributes(
         self,
-        query: Annotated[
-            str, OpenBBCustomParameter(description="Query to search for.")
-        ],
+        query: Annotated[str, OpenBBField(description="Query to search for.")],
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 1000,
         provider: Annotated[
             Optional[Literal["intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search Intrinio data tags to search in latest or historical attributes.
 
@@ -3636,26 +3587,24 @@
             )
         )
 
     @exception_handler
     @validate
     def trailing_dividend_yield(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The number of data entries to return. Default is 252, the number of trading days in a year."
             ),
         ] = 252,
         provider: Annotated[
             Optional[Literal["tiingo"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'tiingo' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the 1 year trailing dividend yield for a given company over time.
 
@@ -3716,24 +3665,21 @@
             )
         )
 
     @exception_handler
     @validate
     def transcript(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         year: Annotated[
-            int,
-            OpenBBCustomParameter(description="Year of the earnings call transcript."),
+            int, OpenBBField(description="Year of the earnings call transcript.")
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get earnings call transcripts for a given company.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_ownership.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -25,33 +25,33 @@
 
     @exception_handler
     @validate
     def form_13f(
         self,
         symbol: Annotated[
             str,
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. A CIK or Symbol can be used."
             ),
         ],
         date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="A specific date to get data for. The date represents the end of the reporting period. All form 13F-HR filings are based on the calendar year and are reported quarterly. If a date is not supplied, the most recent filing is returned. Submissions beginning 2013-06-30 are supported."
             ),
         ] = None,
         limit: Annotated[
             Optional[int],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The number of data entries to return. The number of previous filings to return. The date parameter takes priority over this parameter."
             ),
         ] = 1,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the form 13F.
 
@@ -148,24 +148,21 @@
             )
         )
 
     @exception_handler
     @validate
     def insider_trading(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            int, OpenBBField(description="The number of data entries to return.")
         ] = 500,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get data about trading by a company's management team and board of directors.
 
@@ -290,20 +287,18 @@
             )
         )
 
     @exception_handler
     @validate
     def institutional(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get data about institutional ownership for a given company over time.
 
@@ -432,28 +427,25 @@
             )
         )
 
     @exception_handler
     @validate
     def major_holders(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(description="A specific date to get data for."),
+            OpenBBField(description="A specific date to get data for."),
         ] = None,
         page: Annotated[
-            Optional[int],
-            OpenBBCustomParameter(description="Page number of the data to fetch."),
+            Optional[int], OpenBBField(description="Page number of the data to fetch.")
         ] = 0,
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get data about major holders for a given company over time.
 
@@ -593,21 +585,21 @@
 
     @exception_handler
     @validate
     def share_statistics(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get data about share float for a given company.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_price.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -24,37 +24,33 @@
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         interval: Annotated[
             Optional[str],
-            OpenBBCustomParameter(description="Time interval of the data to return."),
+            OpenBBField(description="Time interval of the data to return."),
         ] = "1d",
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "tiingo", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical price data for a given stock. This includes open, high, low, close, and volume.
 
@@ -203,20 +199,18 @@
             )
         )
 
     @exception_handler
     @validate
     def nbbo(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["polygon"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'polygon' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the National Best Bid and Offer for a given stock.
 
@@ -313,21 +307,21 @@
 
     @exception_handler
     @validate
     def performance(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get price performance data for a given stock. This includes price changes for different time periods.
 
@@ -417,21 +411,21 @@
 
     @exception_handler
     @validate
     def quote(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the latest quote for a given stock. Quote includes price, volume, and other data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/equity_shorts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import Literal, Optional
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -18,20 +18,18 @@
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def fails_to_deliver(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get reported Fail-to-deliver (FTD) data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/etf.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/etf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 from warnings import simplefilter, warn
 
 from openbb_core.app.deprecation import OpenBBDeprecationWarning
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated, deprecated
 
 
@@ -32,21 +32,21 @@
 
     @exception_handler
     @validate
     def countries(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. (ETF) Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """ETF Country weighting.
 
@@ -104,21 +104,21 @@
 
     @exception_handler
     @validate
     def equity_exposure(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. (Stock) Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the exposure to ETFs for a specific stock.
 
@@ -186,37 +186,33 @@
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         interval: Annotated[
             Optional[str],
-            OpenBBCustomParameter(description="Time interval of the data to return."),
+            OpenBBField(description="Time interval of the data to return."),
         ] = "1d",
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "tiingo", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """ETF Historical Market Price.
 
@@ -368,19 +364,19 @@
         )
 
     @exception_handler
     @validate
     def holdings(
         self,
         symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for. (ETF)")
+            str, OpenBBField(description="Symbol to get data for. (ETF)")
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the holdings for an individual ETF.
 
@@ -538,37 +534,37 @@
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_rec : Optional[str]
             The floating rate index for reveivable portion of the swap. (provider: sec)
         floating_rate_spread_rec : Optional[float]
             The floating rate spread for reveivable portion of the swap. (provider: sec)
         rate_tenor_rec : Optional[str]
             The rate tenor for reveivable portion of the swap. (provider: sec)
-        rate_tenor_unit_rec : Optional[Union[int, str]]
+        rate_tenor_unit_rec : Optional[Union[str, int]]
             The rate tenor unit for reveivable portion of the swap. (provider: sec)
         reset_date_rec : Optional[str]
             The reset date for reveivable portion of the swap. (provider: sec)
-        reset_date_unit_rec : Optional[Union[int, str]]
+        reset_date_unit_rec : Optional[Union[str, int]]
             The reset date unit for reveivable portion of the swap. (provider: sec)
         rate_type_pmnt : Optional[str]
             The type of rate for payment portion of the swap. (provider: sec)
         payment_currency : Optional[str]
             The payment currency of the swap. (provider: sec)
         upfront_payment : Optional[float]
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_pmnt : Optional[str]
             The floating rate index for payment portion of the swap. (provider: sec)
         floating_rate_spread_pmnt : Optional[float]
             The floating rate spread for payment portion of the swap. (provider: sec)
         rate_tenor_pmnt : Optional[str]
             The rate tenor for payment portion of the swap. (provider: sec)
-        rate_tenor_unit_pmnt : Optional[Union[int, str]]
+        rate_tenor_unit_pmnt : Optional[Union[str, int]]
             The rate tenor unit for payment portion of the swap. (provider: sec)
         reset_date_pmnt : Optional[str]
             The reset date for payment portion of the swap. (provider: sec)
-        reset_date_unit_pmnt : Optional[Union[int, str]]
+        reset_date_unit_pmnt : Optional[Union[str, int]]
             The reset date unit for payment portion of the swap. (provider: sec)
         repo_type : Optional[str]
             The type of repo. (provider: sec)
         is_cleared : Optional[str]
             If the repo is cleared. (provider: sec)
         is_tri_party : Optional[str]
             If the repo is tri party. (provider: sec)
@@ -629,19 +625,19 @@
         )
 
     @exception_handler
     @validate
     def holdings_date(
         self,
         symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for. (ETF)")
+            str, OpenBBField(description="Symbol to get data for. (ETF)")
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Use this function to get the holdings dates, if available.
 
@@ -704,21 +700,21 @@
         "This endpoint is deprecated; pass a list of holdings symbols directly to `/equity/price/performance` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.2.",
         category=OpenBBDeprecationWarning,
     )
     def holdings_performance(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the recent price performance of each ticker held in the ETF.
 
@@ -815,21 +811,21 @@
 
     @exception_handler
     @validate
     def info(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. (ETF) Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """ETF Information Overview.
 
@@ -1207,21 +1203,21 @@
 
     @exception_handler
     @validate
     def price_performance(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Price performance as a return, over different periods.
 
@@ -1344,20 +1340,18 @@
             )
         )
 
     @exception_handler
     @validate
     def search(
         self,
-        query: Annotated[
-            Optional[str], OpenBBCustomParameter(description="Search query.")
-        ] = "",
+        query: Annotated[Optional[str], OpenBBField(description="Search query.")] = "",
         provider: Annotated[
             Optional[Literal["fmp", "intrinio"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for ETFs.
 
@@ -1459,19 +1453,19 @@
         )
 
     @exception_handler
     @validate
     def sectors(
         self,
         symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for. (ETF)")
+            str, OpenBBField(description="Symbol to get data for. (ETF)")
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """ETF Sector weighting.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -52,27 +52,23 @@
 
     @exception_handler
     @validate
     def sofr(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Secured Overnight Financing Rate.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_corporate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import (
-    OpenBBCustomChoices,
-    OpenBBCustomParameter,
-)
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -28,38 +25,34 @@
 
     @exception_handler
     @validate
     def commercial_paper(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         maturity: Annotated[
             Literal["overnight", "7d", "15d", "30d", "60d", "90d"],
-            OpenBBCustomParameter(description="The maturity."),
+            OpenBBField(description="The maturity."),
         ] = "30d",
         category: Annotated[
             Literal["asset_backed", "financial", "nonfinancial"],
-            OpenBBCustomParameter(description="The category."),
+            OpenBBField(description="The category."),
         ] = "financial",
         grade: Annotated[
-            Literal["aa", "a2_p2"], OpenBBCustomParameter(description="The grade.")
+            Literal["aa", "a2_p2"], OpenBBField(description="The grade.")
         ] = "aa",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Commercial Paper.
 
@@ -137,23 +130,22 @@
 
     @exception_handler
     @validate
     def hqm(
         self,
         date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(description="A specific date to get data for."),
+            OpenBBField(description="A specific date to get data for."),
         ] = None,
         yield_curve: Annotated[
-            Literal["spot", "par"],
-            OpenBBCustomParameter(description="The yield curve type."),
+            Literal["spot", "par"], OpenBBField(description="The yield curve type.")
         ] = "spot",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """High Quality Market Corporate Bond.
 
@@ -228,31 +220,27 @@
 
     @exception_handler
     @validate
     def ice_bofa(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         index_type: Annotated[
             Literal["yield", "yield_to_worst", "total_return", "spread"],
-            OpenBBCustomParameter(description="The type of series."),
+            OpenBBField(description="The type of series."),
         ] = "yield",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """ICE BofA US Corporate Bond Indices.
 
@@ -333,31 +321,26 @@
 
     @exception_handler
     @validate
     def moody(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         index_type: Annotated[
-            Literal["aaa", "baa"],
-            OpenBBCustomParameter(description="The type of series."),
+            Literal["aaa", "baa"], OpenBBField(description="The type of series.")
         ] = "aaa",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Moody Corporate Bond Index.
 
@@ -431,40 +414,36 @@
 
     @exception_handler
     @validate
     def spot_rates(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         maturity: Annotated[
             Union[float, str, List[Union[float, str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Maturities in years. Multiple comma separated items allowed for provider(s): fred."
             ),
         ] = 10.0,
         category: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
-                description="Rate category. Options: spot_rate, par_yield. Multiple comma separated items allowed for provider(s): fred."
+            OpenBBField(
+                description="Rate category. Options: spot_rate, par_yield. Multiple comma separated items allowed for provider(s): fred.",
+                choices=["par_yield", "spot_rate"],
             ),
-            OpenBBCustomChoices(choices=["par_yield", "spot_rate"]),
         ] = "spot_rate",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Spot Rates.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_government.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -22,27 +22,23 @@
 
     @exception_handler
     @validate
     def treasury_rates(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["federal_reserve", "fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'federal_reserve' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Government Treasury Rates.
 
@@ -128,25 +124,24 @@
 
     @exception_handler
     @validate
     def us_yield_curve(
         self,
         date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="A specific date to get data for. Defaults to the most recent FRED entry."
             ),
         ] = None,
         inflation_adjusted: Annotated[
-            Optional[bool],
-            OpenBBCustomParameter(description="Get inflation adjusted rates."),
+            Optional[bool], OpenBBField(description="Get inflation adjusted rates.")
         ] = False,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """US Yield Curve. Get United States yield curve.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_rate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -28,27 +28,23 @@
 
     @exception_handler
     @validate
     def ameribor(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Ameribor.
 
@@ -118,27 +114,23 @@
 
     @exception_handler
     @validate
     def dpcredit(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Discount Window Primary Credit Rate.
 
@@ -209,31 +201,27 @@
 
     @exception_handler
     @validate
     def ecb(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         interest_rate_type: Annotated[
             Literal["deposit", "lending", "refinancing"],
-            OpenBBCustomParameter(description="The type of interest rate."),
+            OpenBBField(description="The type of interest rate."),
         ] = "lending",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """European Central Bank Interest Rates.
 
@@ -307,27 +295,23 @@
 
     @exception_handler
     @validate
     def effr(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["federal_reserve", "fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'federal_reserve' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Fed Funds Rate.
 
@@ -397,15 +381,15 @@
 
     @exception_handler
     @validate
     def effr_forecast(
         self,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Fed Funds Rate Projections.
 
@@ -481,27 +465,23 @@
 
     @exception_handler
     @validate
     def estr(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Euro Short-Term Rate.
 
@@ -572,27 +552,23 @@
 
     @exception_handler
     @validate
     def iorb(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Interest on Reserve Balances.
 
@@ -659,27 +635,23 @@
 
     @exception_handler
     @validate
     def sonia(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Sterling Overnight Index Average.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/fixedincome_spreads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import Literal, Optional, Union
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -23,31 +23,26 @@
 
     @exception_handler
     @validate
     def tcm(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         maturity: Annotated[
-            Optional[Literal["3m", "2y"]],
-            OpenBBCustomParameter(description="The maturity"),
+            Optional[Literal["3m", "2y"]], OpenBBField(description="The maturity")
         ] = "3m",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Treasury Constant Maturity.
 
@@ -119,31 +114,27 @@
 
     @exception_handler
     @validate
     def tcm_effr(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         maturity: Annotated[
             Optional[Literal["10y", "5y", "1y", "6m", "3m"]],
-            OpenBBCustomParameter(description="The maturity"),
+            OpenBBField(description="The maturity"),
         ] = "10y",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Select Treasury Constant Maturity.
 
@@ -215,31 +206,26 @@
 
     @exception_handler
     @validate
     def treasury_effr(
         self,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         maturity: Annotated[
-            Optional[Literal["3m", "6m"]],
-            OpenBBCustomParameter(description="The maturity"),
+            Optional[Literal["3m", "6m"]], OpenBBField(description="The maturity")
         ] = "3m",
         provider: Annotated[
             Optional[Literal["fred"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Select Treasury Bill.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/index.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 from warnings import simplefilter, warn
 
 from openbb_core.app.deprecation import OpenBBDeprecationWarning
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated, deprecated
 
 
@@ -26,15 +26,15 @@
 
     @exception_handler
     @validate
     def available(
         self,
         provider: Annotated[
             Optional[Literal["fmp", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """All indices available from a given provider.
 
@@ -96,20 +96,18 @@
             )
         )
 
     @exception_handler
     @validate
     def constituents(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["fmp"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Index Constituents.
 
@@ -184,37 +182,33 @@
         "This endpoint is deprecated; use `/index/price/historical` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.3.",
         category=OpenBBDeprecationWarning,
     )
     def market(
         self,
         symbol: Annotated[
             Union[str, List[str]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, polygon, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         interval: Annotated[
             Optional[str],
-            OpenBBCustomParameter(description="Time interval of the data to return."),
+            OpenBBField(description="Time interval of the data to return."),
         ] = "1d",
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon", "yfinance"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get Historical Market Indices.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/news.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
 
 from annotated_types import Ge
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -23,39 +23,35 @@
 
     @exception_handler
     @validate
     def company(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp, intrinio, polygon, tiingo, yfinance."
             ),
         ] = None,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         limit: Annotated[
             Optional[Annotated[int, Ge(ge=0)]],
-            OpenBBCustomParameter(description="The number of data entries to return."),
+            OpenBBField(description="The number of data entries to return."),
         ] = 2500,
         provider: Annotated[
             Optional[
                 Literal["benzinga", "fmp", "intrinio", "polygon", "tiingo", "yfinance"]
             ],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'benzinga' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Company News. Get news for one or more companies.
 
@@ -217,33 +213,29 @@
 
     @exception_handler
     @validate
     def world(
         self,
         limit: Annotated[
             int,
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The number of data entries to return. The number of articles to return."
             ),
         ] = 2500,
         start_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="Start date of the data, in YYYY-MM-DD format."),
         ] = None,
         end_date: Annotated[
             Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
+            OpenBBField(description="End date of the data, in YYYY-MM-DD format."),
         ] = None,
         provider: Annotated[
             Optional[Literal["benzinga", "fmp", "intrinio", "tiingo"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'benzinga' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """World News. Global news data.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/openbb/package/regulators_sec.py` & `openbb_nightly-4.1.6.dev202404200009/openbb/package/regulators_sec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 from typing import Literal, Optional
 
-from openbb_core.app.model.custom_parameter import OpenBBCustomParameter
+from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
@@ -23,20 +23,18 @@
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def cik_map(
         self,
-        symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
-        ],
+        symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Map a ticker symbol to a CIK number.
 
@@ -91,24 +89,24 @@
             )
         )
 
     @exception_handler
     @validate
     def institutions_search(
         self,
-        query: Annotated[str, OpenBBCustomParameter(description="Search query.")] = "",
+        query: Annotated[str, OpenBBField(description="Search query.")] = "",
         use_cache: Annotated[
             Optional[bool],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Whether or not to use cache. If True, cache will store for seven days."
             ),
         ] = True,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search SEC-regulated institutions by name and return a list of results with CIK numbers.
 
@@ -137,15 +135,15 @@
             extra : Dict[str, Any]
                 Extra info.
 
         InstitutionsSearch
         ------------------
         name : Optional[str]
             The name of the institution. (provider: sec)
-        cik : Optional[Union[int, str]]
+        cik : Optional[Union[str, int]]
             Central Index Key (CIK) (provider: sec)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.regulators.sec.institutions_search(provider='sec')
         >>> obb.regulators.sec.institutions_search(query='blackstone real estate', provider='sec')
@@ -171,15 +169,15 @@
 
     @exception_handler
     @validate
     def rss_litigation(
         self,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get the RSS feed that provides links to litigation releases concerning civil lawsuits brought by the Commission in federal court.
 
@@ -238,24 +236,24 @@
             )
         )
 
     @exception_handler
     @validate
     def schema_files(
         self,
-        query: Annotated[str, OpenBBCustomParameter(description="Search query.")] = "",
+        query: Annotated[str, OpenBBField(description="Search query.")] = "",
         use_cache: Annotated[
             Optional[bool],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Whether or not to use cache. If True, cache will store for seven days."
             ),
         ] = True,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Use tool for navigating the directory of SEC XML schema files by year.
 
@@ -333,24 +331,24 @@
             )
         )
 
     @exception_handler
     @validate
     def sic_search(
         self,
-        query: Annotated[str, OpenBBCustomParameter(description="Search query.")] = "",
+        query: Annotated[str, OpenBBField(description="Search query.")] = "",
         use_cache: Annotated[
             Optional[bool],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Whether or not to use cache. If True, cache will store for seven days."
             ),
         ] = True,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for Industry Titles, Reporting Office, and SIC Codes. An empty query string returns all results.
 
@@ -413,24 +411,24 @@
             )
         )
 
     @exception_handler
     @validate
     def symbol_map(
         self,
-        query: Annotated[str, OpenBBCustomParameter(description="Search query.")],
+        query: Annotated[str, OpenBBField(description="Search query.")],
         use_cache: Annotated[
             Optional[bool],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="Whether or not to use cache. If True, cache will store for seven days."
             ),
         ] = True,
         provider: Annotated[
             Optional[Literal["sec"]],
-            OpenBBCustomParameter(
+            OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Map a CIK number to a ticker symbol, leading 0s can be omitted or included.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Benzinga Analyst Search Model."""
 
 # pylint: disable=unused-argument
 
-from datetime import datetime
+from datetime import (
+    date as dateType,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.analyst_search import (
     AnalystSearchData,
     AnalystSearchQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request, get_querystring
+from openbb_core.provider.utils.helpers import (
+    amake_request,
+    get_querystring,
+    safe_fromtimestamp,
+)
 from pydantic import Field, field_validator, model_validator
-from pytz import UTC
 
 
 class BenzingaAnalystSearchQueryParams(AnalystSearchQueryParams):
     """Benzinga Analyst Search Query.
 
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-analysts
     """
@@ -354,20 +360,20 @@
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 3 years",
         json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
         alias="3y_success_rate",
     )
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
-    def validate_date(cls, v):
-        """Validate date."""
+    def validate_date(cls, v: float) -> Optional[dateType]:
+        """Validate last_updated."""
         if v:
-            dt = datetime.fromtimestamp(v, UTC)
+            dt = safe_fromtimestamp(v, tz=timezone.utc)
             return dt.date() if dt.time() == dt.min.time() else dt
-        return v
+        return None
 
     @model_validator(mode="before")
     @classmethod
     def replace_empty_strings(cls, values):
         """Check for empty strings and replace with None."""
         return (
             {k: None if v == "" else v for k, v in values.items()}
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.price_target import (
     PriceTargetData,
     PriceTargetQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_requests, get_querystring
+from openbb_core.provider.utils.helpers import (
+    amake_requests,
+    get_querystring,
+    safe_fromtimestamp,
+)
 from pydantic import Field, field_validator, model_validator
-from pytz import UTC
 
 COVERAGE_DICT = {
     "downgrades": "Downgrades",
     "maintains": "Maintains",
     "reinstates": "Reinstates",
     "reiterates": "Reiterates",
     "upgrades": "Upgrades",
@@ -217,20 +220,20 @@
     @classmethod
     def parse_date(cls, v: str):
         """Parse the publisihed_date."""
         return datetime.strptime(v, "%Y-%m-%d").date() if v else None
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
-    def validate_date(cls, v):
+    def validate_date(cls, v: float) -> Optional[dateType]:
         """Convert the Unix timestamp to a datetime object."""
         if v:
-            dt = datetime.fromtimestamp(v, UTC)
+            dt = safe_fromtimestamp(v, tz=timezone.utc)
             return dt.date() if dt.time() == dt.min.time() else dt
-        return v
+        return None
 
     @model_validator(mode="before")
     @classmethod
     def replace_empty_strings(cls, values):
         """Check for empty strings and replace with None."""
         return {k: None if v == "" else v for k, v in values.items()}
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.6.dev202404200009/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404200009/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """FMP Currency Snapshots Model."""
 
 # pylint: disable=unused-argument
 
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_snapshots import (
     CurrencySnapshotsData,
     CurrencySnapshotsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from pandas import DataFrame, concat
 from pydantic import Field, field_validator
 
 
 class FMPCurrencySnapshotsQueryParams(CurrencySnapshotsQueryParams):
     """FMP Currency Snapshots Query.
 
@@ -81,29 +84,27 @@
     @staticmethod
     async def aextract_data(
         query: FMPCurrencySnapshotsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the data from the FMP endpoint."""
-
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         url = f"https://financialmodelingprep.com/api/v3/quotes/forex?apikey={api_key}"
 
         return await amake_request(url, **kwargs)  # type: ignore
 
     @staticmethod
     def transform_data(
         query: FMPCurrencySnapshotsQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPCurrencySnapshotsData]:
         """Filter by the query parameters and validate the model."""
-
         if not data:
             raise EmptyDataError("No data was returned from the FMP endpoint.")
 
         # Drop all the zombie columns FMP returns.
         df = (
             DataFrame(data)
             .dropna(how="all", axis=1)
@@ -139,15 +140,15 @@
                     .filter(items=counter_currencies, axis=0)
                     .reset_index()
                 )
             # If there are no records, don't concatenate.
             if len(temp) > 0:
                 # Convert the Unix timestamp to a datetime.
                 temp.timestamp = temp.timestamp.apply(
-                    lambda x: datetime.fromtimestamp(x)
+                    lambda x: safe_fromtimestamp(x, tz=timezone.utc)
                 )
                 new_df = concat([new_df, temp])
             if len(new_df) == 0:
                 raise EmptyDataError(
                     "No data was found using the applied filters. Check the parameters."
                 )
             # Fill and replace any NaN values with NoneType.
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """FMP Equity Quote Model."""
 
+# pylint: disable=unused-argument
+
 import asyncio
-from datetime import datetime, timezone
-from typing import Any, Dict, List, Optional
+from datetime import (
+    date as dateType,
+    datetime,
+    timezone,
+)
+from typing import Any, Dict, List, Optional, Union
 from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_quote import (
     EquityQuoteData,
     EquityQuoteQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_fmp.utils.helpers import get_querystring, response_callback
 from pydantic import Field, field_validator
 
 
 class FMPEquityQuoteQueryParams(EquityQuoteQueryParams):
     """FMP Equity Quote Query.
 
@@ -59,30 +65,30 @@
     pe: Optional[float] = Field(default=None, description="Price earnings ratio.")
     earnings_announcement: Optional[datetime] = Field(
         default=None, description="Upcoming earnings announcement date."
     )
 
     @field_validator("last_timestamp", mode="before", check_fields=False)
     @classmethod
-    def validate_last_timestamp(cls, v):  # pylint: disable=E0213
+    def validate_last_timestamp(cls, v: Union[str, int]) -> Optional[dateType]:
         """Return the date as a datetime object."""
         if v:
             v = int(v) if isinstance(v, str) else v
-            return datetime.fromtimestamp(int(v), tz=timezone.utc)
+            return safe_fromtimestamp(v, tz=timezone.utc)
         return None
 
     @field_validator("earnings_announcement", mode="before", check_fields=False)
     @classmethod
-    def timestamp_validate(cls, v):  # pylint: disable=E0213
+    def timestamp_validate(cls, v: str) -> Optional[dateType]:
         """Return the datetime string as a datetime object."""
         if v:
             dt = datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.%f%z")
             dt = dt.replace(microsecond=0)
             timestamp = dt.timestamp()
-            return datetime.fromtimestamp(timestamp, tz=timezone.utc)
+            return safe_fromtimestamp(timestamp, tz=timezone.utc)
         return None
 
     @field_validator("change_percent", mode="after", check_fields=False)
     @classmethod
     def normalize_percent(cls, v):  # pylint: disable=E0213
         """Return the percent value as a normalized value."""
         return float(v) / 100 if v else None
@@ -111,15 +117,15 @@
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         symbols = query.symbol.split(",")
 
-        results = []
+        results: list = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = f"{base_url}/quote/{symbol}?{query_str}&apikey={api_key}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
             )
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """FMP Key Executives Model."""
 
-from datetime import datetime
-from typing import Any, Dict, List, Optional
+# pylint: disable=unused-argument
+
+from datetime import (
+    date as dateType,
+)
+from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.key_executives import (
     KeyExecutivesData,
     KeyExecutivesQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_fmp.utils.helpers import get_data_many
 from pydantic import field_validator
 
 
 class FMPKeyExecutivesQueryParams(KeyExecutivesQueryParams):
     """FMP Key Executives Query.
 
@@ -20,17 +25,20 @@
 
 
 class FMPKeyExecutivesData(KeyExecutivesData):
     """FMP Key Executives Data."""
 
     @field_validator("titleSince", mode="before", check_fields=False)
     @classmethod
-    def time_validate(cls, v):  # pylint: disable=E0213
+    def time_validate(cls, v: Union[float, int]) -> Optional[dateType]:
         """Return the date as a datetime object."""
-        return datetime.fromtimestamp(v / 1000)
+        if v:
+            v = v / 1000
+            return safe_fromtimestamp(v)
+        return v  # type: ignore
 
 
 class FMPKeyExecutivesFetcher(
     Fetcher[
         FMPKeyExecutivesQueryParams,
         List[FMPKeyExecutivesData],
     ]
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """FMP Market Indices Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_indices import (
     MarketIndicesData,
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """FMP Market Snapshots Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import (
     date as dateType,
     datetime,
+    timezone,
 )
 from typing import Any, Dict, List, Optional, Union
 
 from dateutil import parser
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_snapshots import (
     MarketSnapshotsData,
     MarketSnapshotsQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_fmp.utils.definitions import EXCHANGES
 from openbb_fmp.utils.helpers import get_data
 from pydantic import Field, field_validator
 
 
 class FMPMarketSnapshotsQueryParams(MarketSnapshotsQueryParams):
     """FMP Market Snapshots Query.
@@ -83,22 +87,28 @@
         description="The upcoming earnings announcement date.",
         alias="earningsAnnouncement",
         default=None,
     )
 
     @field_validator("last_price_timestamp", mode="before", check_fields=False)
     @classmethod
-    def validate_timestamp(cls, v):
+    def validate_timestamp(cls, v: Union[str, int, float]) -> Optional[dateType]:
         """Validate the timestamp."""
+        if isinstance(v, str):
+            try:
+                v = float(v)
+            except ValueError:
+                return None
+
         if isinstance(v, (int, float)) and v != 0:
             try:
-                v = datetime.fromtimestamp(v)
-                if v.hour == 0 and v.minute == 0 and v.second == 0:
-                    v = v.date()
-                return v
+                v = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore
+                if v.hour == 0 and v.minute == 0 and v.second == 0:  # type: ignore
+                    v = v.date()  # type: ignore
+                return v  # type: ignore
             except ValueError:
                 return None
         return None
 
     @field_validator("earnings_date", mode="before", check_fields=False)
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # pylint: disable=unused-argument
 
 import asyncio
 import gzip
 from datetime import (
     date as dateType,
     datetime,
+    timezone as datetime_timezone,
 )
 from io import BytesIO
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_snapshots import (
     MarketSnapshotsData,
     MarketSnapshotsQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from pandas import DataFrame, notna, read_csv, to_datetime
 from pydantic import Field
 from pytz import timezone
 
 
 class IntrinioMarketSnapshotsQueryParams(MarketSnapshotsQueryParams):
     """Intrinio Market Snapshots Query.
@@ -101,15 +102,15 @@
         transformed_params = params
 
         if "date" in transformed_params:
             if isinstance(transformed_params["date"], datetime):
                 dt = transformed_params["date"]
                 dt = dt.astimezone(tz=timezone("America/New_York"))
             if isinstance(transformed_params["date"], dateType):
-                dt = transformed_params["date"]
+                dt = transformed_params["date"]  # type: ignore
                 if isinstance(dt, dateType):
                     dt = datetime(
                         dt.year,
                         dt.month,
                         dt.day,
                         20,
                         0,
@@ -139,15 +140,14 @@
     @staticmethod
     async def aextract_data(
         query: IntrinioMarketSnapshotsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
-
         api_key = credentials.get("intrinio_api_key") if credentials else ""
 
         # This gets the URL to the actual file.
         url = f"https://api-v2.intrinio.com/securities/snapshots?api_key={api_key}"
         if query.date:
             url += f"&at_datetime={query.date}"
 
@@ -212,15 +212,15 @@
                 "last_bid_timestamp",
                 "last_ask_timestamp",
             ]:
                 df[col] = (
                     to_datetime(
                         df[col].apply(
                             lambda x: (
-                                datetime.fromtimestamp(x, tz=timezone("UTC"))
+                                safe_fromtimestamp(x, tz=datetime_timezone.utc)
                                 if notna(x)
                                 else x
                             )
                         )
                     )
                     .dt.tz_convert("America/New_York")
                     .dt.floor("S")
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.6.dev202404200009/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Nasdaq Earnings Calendar Model."""
 
+# pylint: disable=unused-argument
+
 from concurrent.futures import ThreadPoolExecutor
 from datetime import (
     date as dateType,
     datetime,
     timedelta,
 )
 from typing import Any, Dict, List, Optional
@@ -134,14 +136,16 @@
     Fetcher[
         NasdaqCalendarEarningsQueryParams,
         List[NasdaqCalendarEarningsData],
     ]
 ):
     """Transform the query, extract and transform the data from the Nasdaq endpoints."""
 
+    require_credentials = False
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqCalendarEarningsQueryParams:
         """Transform the query params."""
         now = datetime.today().date()
         transformed_params = params
 
         if params.get("start_date") is None:
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """Nasdaq Historical Dividends Model."""
 
 # pylint: disable=unused-argument
 import asyncio
-import warnings
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from dateutil import parser
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.historical_dividends import (
     HistoricalDividendsData,
     HistoricalDividendsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_nasdaq.utils.helpers import IPO_HEADERS
 from pydantic import Field, field_validator
 
-_warn = warnings.warn
-
 
 class NasdaqHistoricalDividendsQueryParams(HistoricalDividendsQueryParams):
     """Nasdaq Historical Dividends Query Params."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
 
@@ -88,14 +86,16 @@
 
 
 class NasdaqHistoricalDividendsFetcher(
     Fetcher[NasdaqHistoricalDividendsQueryParams, List[NasdaqHistoricalDividendsData]]
 ):
     """Nasdaq Historical Dividends Fetcher."""
 
+    require_credentials = False
+
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> NasdaqHistoricalDividendsQueryParams:
         """Transform the params to the provider-specific query."""
         return NasdaqHistoricalDividendsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
@@ -127,15 +127,15 @@
 
             if data:
                 if len(symbols) > 1:
                     for d in data:
                         d["symbol"] = symbol
                 results.extend(data)
             if not data:
-                _warn(f"No data found for {symbol}")
+                warn(f"No data found for {symbol}")
 
         tasks = [get_one(symbol) for symbol in symbols]
 
         await asyncio.gather(*tasks)
         if results:
             return results
         raise EmptyDataError()
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.6.dev202404200009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Polygon Crypto Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access,line-too-long
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.crypto_historical import (
     CryptoHistoricalData,
     CryptoHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
-from pytz import timezone
 
 _warn = warnings.warn
 
 
 class PolygonCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Polygon Crypto Historical Price Query.
 
@@ -142,25 +145,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore
+            results: list = data.get("results", [])  # type: ignore
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore
+                next_url = data.get("next_url", None)  # type: ignore
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(r["t"] / 1000, tz=timezone("UTC"))
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol.replace("X:", "")
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Polygon Currency Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access,line-too-long
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_historical import (
     CurrencyHistoricalData,
     CurrencyHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
-from pytz import timezone
 
 _warn = warnings.warn
 
 
 class PolygonCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Polygon Currency Historical Price Query.
 
@@ -139,25 +142,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore[union-attr]
+            results: list = data.get("results", [])  # type: ignore[union-attr]
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore[union-attr]
+                next_url = data.get("next_url", None)  # type: ignore[union-attr]
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(r["t"] / 1000, tz=timezone("UTC"))
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Polygon Equity Historical Price Model."""
 
 # pylint: disable=unused-argument,protected-access
 
 import warnings
-from datetime import datetime
+from datetime import (
+    datetime,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_historical import (
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pandas import to_datetime
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
@@ -148,27 +151,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore
+            results: list = data.get("results", [])  # type: ignore
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore
+                next_url = data.get("next_url", None)  # type: ignore
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(
-                    r["t"] / 1000, tz=timezone("America/New_York")
-                )
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone("America/New_York"))  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
+    safe_fromtimestamp,
 )
 from pydantic import (
     Field,
     PositiveInt,
     PrivateAttr,
     model_validator,
 )
@@ -139,27 +140,26 @@
 
         async def callback(
             response: ClientResponse, session: ClientSession
         ) -> List[Dict]:
             data = await response.json()
 
             symbol = response.url.parts[4]
-            next_url = data.get("next_url", None)
-            results: list = data.get("results", [])
+            next_url = data.get("next_url", None)  # type: ignore[union-attr]
+            results: list = data.get("results", [])  # type: ignore[union-attr]
 
             while next_url:
                 url = f"{next_url}&apiKey={api_key}"
                 data = await session.get_json(url)
-                results.extend(data.get("results", []))
-                next_url = data.get("next_url", None)
+                results.extend(data.get("results", []))  # type: ignore[union-attr]
+                next_url = data.get("next_url", None)  # type: ignore[union-attr]
 
             for r in results:
-                r["t"] = datetime.fromtimestamp(
-                    r["t"] / 1000, tz=timezone("America/New_York")
-                )
+                v = r["t"] / 1000  # milliseconds to seconds
+                r["t"] = safe_fromtimestamp(v, tz=timezone("America/New_York"))  # type: ignore[arg-type]
                 if query._timespan not in ["second", "minute", "hour"]:
                     r["t"] = r["t"].date().strftime("%Y-%m-%d")
                 else:
                     r["t"] = r["t"].strftime("%Y-%m-%dT%H:%M:%S%z")
                 if "," in query.symbol:
                     r["symbol"] = symbol
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Polygon Market Indices Model."""
 
-from datetime import datetime
+from datetime import (
+    datetime,
+)
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_indices import (
     MarketIndicesData,
     MarketIndicesQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_polygon.utils.helpers import get_data_many
 from pydantic import Field, PositiveInt
 
 
 class PolygonMarketIndicesQueryParams(MarketIndicesQueryParams):
     """Polygon Market Indices Query.
 
@@ -90,15 +93,16 @@
             f"I:{query.symbol}/range/{query.multiplier}/{query.timespan}/"
             f"{query.start_date}/{query.end_date}?adjusted={query.adjusted}"
             f"&sort={query.sort}&limit={query.limit}&apiKey={api_key}"
         )
         data = await get_data_many(request_url, "results", **kwargs)
 
         for d in data:
-            d["t"] = datetime.fromtimestamp(d["t"] / 1000)
+            v = d["t"] / 1000  # milliseconds to seconds
+            d["t"] = safe_fromtimestamp(v)
             if query.timespan not in ["minute", "hour"]:
                 d["t"] = d["t"].date()
 
         return data
 
     @staticmethod
     def transform_data(
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.6.dev202404200009/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404200009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.6.dev202404200009/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tradier Equity Historical Model"""
+"""Tradier Equity Historical Model."""
 
 # pylint: disable = unused-argument
 
 import asyncio
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Literal, Optional
 from warnings import warn
@@ -12,15 +12,15 @@
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     QUERY_DESCRIPTIONS,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import INTERVALS_DICT
 from pandas import to_datetime
 from pydantic import Field
 from pytz import timezone
 
 
 class TradierEquityHistoricalQueryParams(EquityHistoricalQueryParams):
@@ -52,15 +52,14 @@
     Fetcher[TradierEquityHistoricalQueryParams, List[TradierEquityHistoricalData]]
 ):
     """Tradier Equity Historical Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TradierEquityHistoricalQueryParams:
         """Transform the query."""
-
         if params.get("interval") in ["1d", "1W", "1M"]:
             if params.get("start_date") is None:
                 params["start_date"] = (datetime.now() - timedelta(days=365)).date()
             if params.get("end_date") is None:
                 params["end_date"] = datetime.now().date()
 
         if params.get("interval") in ["1m", "5m", "15m"]:
@@ -81,15 +80,14 @@
     @staticmethod
     async def aextract_data(
         query: TradierEquityHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Tradier endpoint."""
-
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -116,15 +114,14 @@
         end_point = "timesales" if query.interval in ["1m", "5m", "15m"] else "history"
         results = []
         start_time = "09:30" if query.extended_hours is False else "00:00"
         end_time = "16:00" if query.extended_hours is False else "20:00"
 
         async def get_one(symbol):
             """Get data for one symbol."""
-
             result = []
 
             url = (
                 f"{BASE_URL}v1/markets/{end_point}?symbol={symbol}&interval={interval}"
             )
 
             if query.interval in ["1m", "5m", "15m"]:
@@ -146,15 +143,15 @@
             if interval in ["1min", "5min", "15min"] and data.get("series"):  # type: ignore
                 result = data["series"].get("data")  # type: ignore
                 for r in result:
                     if len(query.symbol.split(",")) > 1:
                         r["symbol"] = symbol
                     _ = r.pop("time")
                     r["timestamp"] = (
-                        datetime.fromtimestamp(r.get("timestamp"))
+                        safe_fromtimestamp(r.get("timestamp"))
                         .replace(microsecond=0)
                         .astimezone(timezone("America/New_York"))
                     )
 
             if result != []:
                 results.extend(result)
             if result == []:
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tradier Equity Quote Model"""
+"""Tradier Equity Quote Model."""
 
 # pylint: disable = unused-argument
 
 from datetime import (
     date as dateType,
     datetime,
 )
@@ -11,15 +11,15 @@
 from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_quote import (
     EquityQuoteData,
     EquityQuoteQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Tradier Equity Quote Query."""
@@ -153,15 +153,16 @@
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_dates(cls, v):
         """Validate the dates."""
         if v != 0 and v is not None and isinstance(v, int):
-            v = datetime.fromtimestamp(int(v) / 1000)
+            v = int(v) / 1000  # milliseconds to seconds
+            v = safe_fromtimestamp(v)
             v = v.replace(microsecond=0)
             v = v.astimezone(timezone("America/New_York"))
             return v
         if v is not None and isinstance(v, str):
             v = parse(v)
             v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
             v = v.astimezone(timezone("America/New_York"))
@@ -198,15 +199,14 @@
     @staticmethod
     async def aextract_data(
         query: TradierEquityQuoteQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Tradier endpoint."""
-
         api_key = credentials.get("tradier_api_key") if credentials else ""
         sandbox = True
 
         if api_key and credentials.get("tradier_account_type") not in ["sandbox", "live"]:  # type: ignore
             raise ValueError(
                 "Invalid account type for Tradier. Must be either 'sandbox' or 'live'."
             )
@@ -241,15 +241,14 @@
     @staticmethod
     def transform_data(
         query: TradierEquityQuoteQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[TradierEquityQuoteData]:
         """Transform and validate the data."""
-
         results: List[TradierEquityQuoteData] = []
 
         for d in data:
 
             d["exch"] = (
                 OPTIONS_EXCHANGES.get(d["exch"])
                 if d.get("type") in ["option", "index"]
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dateutil.parser import parse
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.options_chains import (
     OptionsChainsData,
     OptionsChainsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_tradier.utils.constants import OPTIONS_EXCHANGES, STOCK_EXCHANGES
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierOptionsChainsQueryParams(OptionsChainsQueryParams):
     """Tradier Options Chains Query.
@@ -122,15 +122,16 @@
         mode="before",
         check_fields=False,
     )
     @classmethod
     def validate_dates(cls, v):
         """Validate the dates."""
         if v != 0 and v is not None and isinstance(v, int):
-            v = datetime.fromtimestamp(int(v) / 1000)
+            v = int(v) / 1000  # milliseconds to seconds
+            v = safe_fromtimestamp(v)
             v = v.replace(microsecond=0)
             v = v.astimezone(timezone("America/New_York"))
             return v
         if v is not None and isinstance(v, str):
             v = parse(v)
             v = v.replace(microsecond=0, tzinfo=timezone("UTC"))
             v = v.astimezone(timezone("America/New_York"))
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.6.dev202404200009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_info import (
     EtfInfoData,
     EtfInfoQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from pydantic import Field, field_validator
 from yfinance import Ticker
 
 _warn = warnings.warn
 
 
 class YFinanceEtfInfoQueryParams(EtfInfoQueryParams):
@@ -271,15 +272,15 @@
                                 result[field] = ticker.get(field, None)
                         if "firstTradeDateEpochUtc" in result:
                             _first_trade = result.pop("firstTradeDateEpochUtc")
                             if (
                                 "fundInceptionDate" not in result
                                 and _first_trade is not None
                             ):
-                                result["fundInceptionDate"] = datetime.fromtimestamp(
+                                result["fundInceptionDate"] = safe_fromtimestamp(
                                     _first_trade
                                 )
                     except Exception as e:
                         _warn(f"Error processing data for {symbol}: {e}")
                         result = {}
                 if quote_type != "ETF":
                     _warn(f"{symbol} is not an ETF.")
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.6.dev202404200009/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404190009/pyproject.toml` & `openbb_nightly-4.1.6.dev202404200009/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.6.dev202404190009"
+version = "4.1.6.dev202404200009"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
```

### Comparing `openbb_nightly-4.1.6.dev202404190009/PKG-INFO` & `openbb_nightly-4.1.6.dev202404200009/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.6.dev202404190009
+Version: 4.1.6.dev202404200009
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

